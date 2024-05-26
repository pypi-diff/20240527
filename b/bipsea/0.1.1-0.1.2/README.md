# Comparing `tmp/bipsea-0.1.1.tar.gz` & `tmp/bipsea-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bipsea-0.1.1.tar", last modified: Sun May 26 13:24:02 2024, max compression
+gzip compressed data, was "bipsea-0.1.2.tar", last modified: Sun May 26 21:20:27 2024, max compression
```

## Comparing `bipsea-0.1.1.tar` & `bipsea-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 13:24:02.422500 bipsea-0.1.1/
--rw-r--r--   0 akarve     (501) staff       (20)    11356 2024-05-26 11:53:50.000000 bipsea-0.1.1/LICENSE.md
--rw-r--r--   0 akarve     (501) staff       (20)      676 2024-05-26 13:24:02.422308 bipsea-0.1.1/PKG-INFO
--rw-r--r--   0 akarve     (501) staff       (20)     8922 2024-05-26 11:53:50.000000 bipsea-0.1.1/README.md
--rw-r--r--   0 akarve     (501) staff       (20)       38 2024-05-26 13:24:02.422539 bipsea-0.1.1/setup.cfg
--rw-r--r--   0 akarve     (501) staff       (20)     1057 2024-05-26 13:21:53.000000 bipsea-0.1.1/setup.py
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 13:24:02.419278 bipsea-0.1.1/src/
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 13:24:02.420626 bipsea-0.1.1/src/bipsea/
--rw-r--r--   0 akarve     (501) staff       (20)        0 2024-05-26 11:53:50.000000 bipsea-0.1.1/src/bipsea/__init__.py
--rw-r--r--   0 akarve     (501) staff       (20)     8116 2024-05-26 12:50:48.000000 bipsea-0.1.1/src/bipsea/bip32.py
--rw-r--r--   0 akarve     (501) staff       (20)     3669 2024-05-26 12:51:31.000000 bipsea-0.1.1/src/bipsea/bip32types.py
--rw-r--r--   0 akarve     (501) staff       (20)     5797 2024-05-26 12:53:56.000000 bipsea-0.1.1/src/bipsea/bip85.py
--rw-r--r--   0 akarve     (501) staff       (20)     7814 2024-05-26 12:54:02.000000 bipsea-0.1.1/src/bipsea/bipsea.py
--rw-r--r--   0 akarve     (501) staff       (20)     3853 2024-05-26 12:54:08.000000 bipsea-0.1.1/src/bipsea/seedwords.py
--rw-r--r--   0 akarve     (501) staff       (20)      864 2024-05-26 13:18:45.000000 bipsea-0.1.1/src/bipsea/util.py
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 13:24:02.422088 bipsea-0.1.1/src/bipsea.egg-info/
--rw-r--r--   0 akarve     (501) staff       (20)      676 2024-05-26 13:24:02.000000 bipsea-0.1.1/src/bipsea.egg-info/PKG-INFO
--rw-r--r--   0 akarve     (501) staff       (20)      465 2024-05-26 13:24:02.000000 bipsea-0.1.1/src/bipsea.egg-info/SOURCES.txt
--rw-r--r--   0 akarve     (501) staff       (20)        1 2024-05-26 13:24:02.000000 bipsea-0.1.1/src/bipsea.egg-info/dependency_links.txt
--rw-r--r--   0 akarve     (501) staff       (20)       45 2024-05-26 13:24:02.000000 bipsea-0.1.1/src/bipsea.egg-info/entry_points.txt
--rw-r--r--   0 akarve     (501) staff       (20)       26 2024-05-26 13:24:02.000000 bipsea-0.1.1/src/bipsea.egg-info/requires.txt
--rw-r--r--   0 akarve     (501) staff       (20)        7 2024-05-26 13:24:02.000000 bipsea-0.1.1/src/bipsea.egg-info/top_level.txt
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 13:24:02.421906 bipsea-0.1.1/tests/
--rw-r--r--   0 akarve     (501) staff       (20)     1324 2024-05-26 13:11:18.000000 bipsea-0.1.1/tests/test_bip32.py
--rw-r--r--   0 akarve     (501) staff       (20)     2182 2024-05-26 13:11:18.000000 bipsea-0.1.1/tests/test_bip39.py
--rw-r--r--   0 akarve     (501) staff       (20)     3708 2024-05-26 13:11:18.000000 bipsea-0.1.1/tests/test_bip85.py
--rw-r--r--   0 akarve     (501) staff       (20)     6535 2024-05-26 13:11:18.000000 bipsea-0.1.1/tests/test_cli.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 21:20:27.725054 bipsea-0.1.2/
+-rw-r--r--   0 akarve     (501) staff       (20)    11356 2024-05-26 11:53:50.000000 bipsea-0.1.2/LICENSE.md
+-rw-r--r--   0 akarve     (501) staff       (20)      676 2024-05-26 21:20:27.724847 bipsea-0.1.2/PKG-INFO
+-rw-r--r--   0 akarve     (501) staff       (20)     9364 2024-05-26 21:11:08.000000 bipsea-0.1.2/README.md
+-rw-r--r--   0 akarve     (501) staff       (20)       38 2024-05-26 21:20:27.725091 bipsea-0.1.2/setup.cfg
+-rw-r--r--   0 akarve     (501) staff       (20)     1120 2024-05-26 21:19:37.000000 bipsea-0.1.2/setup.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 21:20:27.721891 bipsea-0.1.2/src/
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 21:20:27.723276 bipsea-0.1.2/src/bipsea/
+-rw-r--r--   0 akarve     (501) staff       (20)        0 2024-05-26 18:07:02.000000 bipsea-0.1.2/src/bipsea/__init__.py
+-rw-r--r--   0 akarve     (501) staff       (20)     8116 2024-05-26 18:07:02.000000 bipsea-0.1.2/src/bipsea/bip32.py
+-rw-r--r--   0 akarve     (501) staff       (20)     3669 2024-05-26 18:07:02.000000 bipsea-0.1.2/src/bipsea/bip32types.py
+-rw-r--r--   0 akarve     (501) staff       (20)     5521 2024-05-26 20:36:39.000000 bipsea-0.1.2/src/bipsea/bip85.py
+-rw-r--r--   0 akarve     (501) staff       (20)     7659 2024-05-26 21:19:37.000000 bipsea-0.1.2/src/bipsea/bipsea.py
+-rw-r--r--   0 akarve     (501) staff       (20)     3711 2024-05-26 20:36:39.000000 bipsea-0.1.2/src/bipsea/seedwords.py
+-rw-r--r--   0 akarve     (501) staff       (20)      760 2024-05-26 21:19:37.000000 bipsea-0.1.2/src/bipsea/util.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 21:20:27.724651 bipsea-0.1.2/src/bipsea.egg-info/
+-rw-r--r--   0 akarve     (501) staff       (20)      676 2024-05-26 21:20:27.000000 bipsea-0.1.2/src/bipsea.egg-info/PKG-INFO
+-rw-r--r--   0 akarve     (501) staff       (20)      465 2024-05-26 21:20:27.000000 bipsea-0.1.2/src/bipsea.egg-info/SOURCES.txt
+-rw-r--r--   0 akarve     (501) staff       (20)        1 2024-05-26 21:20:27.000000 bipsea-0.1.2/src/bipsea.egg-info/dependency_links.txt
+-rw-r--r--   0 akarve     (501) staff       (20)       45 2024-05-26 21:20:27.000000 bipsea-0.1.2/src/bipsea.egg-info/entry_points.txt
+-rw-r--r--   0 akarve     (501) staff       (20)       26 2024-05-26 21:20:27.000000 bipsea-0.1.2/src/bipsea.egg-info/requires.txt
+-rw-r--r--   0 akarve     (501) staff       (20)        7 2024-05-26 21:20:27.000000 bipsea-0.1.2/src/bipsea.egg-info/top_level.txt
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 21:20:27.724479 bipsea-0.1.2/tests/
+-rw-r--r--   0 akarve     (501) staff       (20)     1319 2024-05-26 20:36:39.000000 bipsea-0.1.2/tests/test_bip32.py
+-rw-r--r--   0 akarve     (501) staff       (20)     2182 2024-05-26 20:36:39.000000 bipsea-0.1.2/tests/test_bip39.py
+-rw-r--r--   0 akarve     (501) staff       (20)     4530 2024-05-26 20:36:39.000000 bipsea-0.1.2/tests/test_bip85.py
+-rw-r--r--   0 akarve     (501) staff       (20)     6535 2024-05-26 18:07:02.000000 bipsea-0.1.2/tests/test_cli.py
```

### Comparing `bipsea-0.1.1/LICENSE.md` & `bipsea-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bipsea-0.1.1/PKG-INFO` & `bipsea-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipsea
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python implementation of BIP 85 (and BIP 32)
 Author: Aneesh Karve
 Author-email: bonded_metals_0u@icloud.com
 Project-URL: Source, https://github.com/akarve/bipsea
 Keywords: Bitcoin BIP85 BIP32 cryptography
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bipsea-0.1.1/README.md` & `bipsea-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-# `bipsea`: unlimited cryptographic entropy for Bitcoin, passwords, and other secrets
+# `bipsea`: unlimited entropy for Bitcoin, passwords, and other secrets
 
 > _One Seed to rule them all,  
 > One Key to find them,  
 > One Path to bring them all,  
 > And in cryptography bind them._  
 > —[BIP-85](https://github.com/bitcoin/bips/blob/master/bip-0085.mediawiki)
 
+bipsea is currently for experimental purposes only.
 bipsea is a standalone, test-driven implementation of BIP-85 and BIP-32.
-bipsea is designed for readability and security. bipsea offers a command-line
+bipsea is designed for readability and correctness. bipsea offers a command-line
 interface and an API.
 
 bipsea relies on cryptographic primitives from Python (`secrets`, `hashlib`),
-and the [python-ecdsa](https://github.com/tlsfuzzer/python-ecdsa). bipsea does not
-rely on third-party libraries from any wallet vendor.
+and the [python-ecdsa](https://github.com/tlsfuzzer/python-ecdsa) and is therefore
+also [vulnerable to side-channel attacks](https://github.com/tlsfuzzer/python-ecdsa?tab=readme-ov-file#security).
+bipsea does not rely on third-party libraries
+from any wallet vendor.
 
 You can run bipsea offline on to generate general-use passwords, Bitcoin seed words,
 and more. Consider dedicated cold hardware that runs [Tails](https://tails.net),
 never has network access, and disables
 [Intel Management Engine](https://support.system76.com/articles/intel-me/)
 and other possible backdoors.
 
@@ -97,18 +100,14 @@
 ## How do I know the bipsea implementation is correct?
 
 bipsea passes all BIP-32 and BIP-85 test vectors plus its own unit tests with the
 following provisos:
 * Only generates seed phrases in English
 * Fails one partial test for derived entropy (but passes all others) from BIP-85
 
-### TODO
-
-* [ ] File the above and other "TODO" issues to BIP-85
-
 Run `make test` for details.
 
 # Usage
 
 ```
 pip install bipsea
 ```
@@ -144,53 +143,58 @@
     xprv9s21ZrQH143K3YwuXcacSSghcUfrrEyj9hTHU3a2gmr6SzPBaxmuTgKGBWtFdnnCjwGYMkU7mLvxba8FFPGLQUMvyACZTEdSCJ8uBwh5Aqs
 
 ## xprv from dice rolls (or any string)
 ```
 bipsea seed -f string -i "123456123456123456" -t xprv
 ```
 
-<pre><code style="color: #CCCC00">Warning: stretched 144 bits of entropy to 256 bits. Provide more entropy.</code></pre>
+<pre><code style="color: #CCCC00">Warning: 144 bits in, 256 bits out. Input more entropy.</code></pre>
 
-    xprv9s21ZrQH143K35QDSCrHfhTJNQGS8ehYV74s65pMwTHfHq89oqcqVQJU4iD3B2M68skmz32eT8Kdr1thXJ6tHXRpy77QtAN1dhEdvqYPiVm
+    xprv9s21ZrQH143K3Ee3pgdhHb9xdu3D1EPT8J45zZ5Th5xPvWT9sujnPDCpA8bZhjz73UkkNWR8WnNg39C3hEHeeXKWLEQKfx9gySgjzMowEwH
 
 This is similar to how coldcard implements
 [verifiable dice rolls](https://coldcard.com/docs/verifying-dice-roll-math/).
 If you are now thinking, _I could use any string to derive a master key_,
 then you get it. And we haven't even gottent into BIP-85.
 
-> That said, **do not get cute and derive valuable keys or secrets from short
+> **Do not get cute and derive valuable keys or secrets from short
 > strings**. You can only stretch entropy so far. **Weak entropy in, weaker entropy out**.
 > Short, common strings are also susceptible to
 [rainbow table attacks](https://en.wikipedia.org/wiki/Rainbow_table).
 
 
 ## `bipsea entropy`
 
 `bipsea entropy` requires you to pipe in an xprv.
 
 ### base64 password
 
 ```
 bipsea seed -f string -i "yoooooooooooooooo" -t xprv -n 12 | bipsea entropy -a base85 -n 10
 ```
-    C(s>@zBUg8
+    aqn+dPu%^~
 
 Increment the index to get a fresh password.
 
 ```
 bipsea seed -f string -i "yoooooooooooooooo" -t xprv -n 12 | bipsea entropy -a base85 -n 10 -i 1
 ```
     p6Ft=F40(*
 
 Alternatively you can pipe in an existing xprv:
 
 ```
 echo "$XPRV" | bipsea entropy -a base85 -n 10
 ```
 
+Or call `--input`:
+```
+bipsea seed -f string -i "yoooooooooooooooo" -t xprv -n 12 --input "$XPRV"
+```
+ 
 ### Derived seed words
 
 ```
 bipsea seed -t xprv | bipsea entropy -a words        
 ```
     loan height quality library maid defense minor token thought music claim actual hour ship robust burst live broccoli
 
@@ -237,7 +241,16 @@
 
 1. [BIP-32](https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki)
 hierarchical deterministic wallets
 1. [BIP-85](https://github.com/bitcoin/bips/blob/master/bip-0085.mediawiki)
 generalized cryptographic entropy
 1. [BIP-44](https://github.com/bitcoin/bips/blob/master/bip-0044.mediawiki)
 generalized BIP-32 paths
+
+
+# TODO
+
+* [x] File the above and other "TODO" issues to BIP-85
+  * https://github.com/bitcoin/bips/pull/1600
+* [ ] Investigate switch to secure ECDSA libs with constant-time programming and
+side-channel resistance.
+    * [ ] https://cryptography.io/en/latest/
```

### Comparing `bipsea-0.1.1/setup.py` & `bipsea-0.1.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from setuptools import find_packages, setup
 
+from src.bipsea.util import __app_name__, __version__
+
 setup(
-    name="bipsea",
-    version="0.1.1",
+    name=__app_name__,
+    version=__version__,
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     description="Python implementation of BIP 85 (and BIP 32)",
     author="Aneesh Karve",
     author_email="bonded_metals_0u@icloud.com",
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `bipsea-0.1.1/src/bipsea/bip32.py` & `bipsea-0.1.2/src/bipsea/bip32.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.1.1/src/bipsea/bip32types.py` & `bipsea-0.1.2/src/bipsea/bip32types.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.1.1/src/bipsea/bip85.py` & `bipsea-0.1.2/src/bipsea/bip85.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import base64
 import hashlib
 import logging
 import re
 from typing import Dict, Union
 
 import base58
+from ecdsa import SECP256k1
 
 from .bip32 import VERSIONS, ExtendedKey
 from .bip32 import derive_key as derive_key_bip32
 from .bip32 import hmac_sha512
 from .seedwords import entropy_to_words
 from .util import LOGGER, to_hex_string
 
@@ -49,74 +50,64 @@
     application, *indexes = segments[2:]
 
     entropy = to_entropy(derived_key.data[1:])
     # BIP 39
     if application == "39'":
         language, n_words = indexes[:2]
         if not language == LANGUAGE_CODES["English"]:
-            raise ValueError(f"Only English BIP39 words from BIP85 are supported.")
+            raise ValueError(f"Only English BIP-39 words from BIP-85 are supported.")
         if not n_words in CODE_39_TO_BITS:
             raise ValueError(f"Expected word codes {CODE_39_TO_BITS.keys()}")
         n_bytes = CODE_39_TO_BITS[n_words] // 8
         trimmed_entropy = entropy[:n_bytes]
         n_words_int = int(n_words[:-1])  # chop the ' from hardened derivation
         return {
             "entropy": trimmed_entropy,
             "application": " ".join(entropy_to_words(n_words_int, trimmed_entropy)),
         }
     # WIF
     elif application == "2'":
+        # https://en.bitcoin.it/wiki/Wallet_import_format
         trimmed_entropy = entropy[: 256 // 8]
         prefix = b"\x80" if derived_key.get_network() == "mainnet" else b"\xef"
         suffix = b"\x01"  # use with compressed public keys because BIP32
         extended = prefix + trimmed_entropy + suffix
         hash1 = hashlib.sha256(extended).digest()
         hash2 = hashlib.sha256(hash1).digest()
+        checksum = hash2[:4]
 
         return {
             "entropy": trimmed_entropy,
-            "application": base58.b58encode_check(extended),
-            "checksum": hash2[:4],
+            "application": base58.b58encode(extended + checksum).decode("utf-8"),
         }
     # XPRV
     elif application == "32'":
         derived_key = ExtendedKey(
-            # TODO: file against bip85 that there is no provision to specify
-            # main vs testnet
-            # TODO: file against bip85 that they are inconsistent with
-            # hmac entropy order :shrug:
             version=VERSIONS["mainnet"]["private"],
             depth=bytes(1),
             finger=bytes(4),
             child_number=bytes(4),
             chain_code=entropy[:32],
             data=bytes(1) + entropy[32:],
         )
 
         return {
-            # TODO: also file against bip85 that there is no consistency about
-            # returned entropy length in test vectors?
-            # TODO: this is wrong on multiple levels; first we use
-            # 64 bytes from the entropy for this application
-            # second this isn't even the chain_code which in some universe
-            # might be considered derived entropy :(
             "entropy": entropy[32:],
             "application": str(derived_key),
         }
     # HEX
     elif application == "128169'":
         num_bytes = int(indexes[0][:-1])
         if not (16 <= num_bytes <= 64):
             raise ValueError(f"Expected num_bytes in [16, 64], got {num_bytes}")
 
         return {"entropy": entropy, "application": to_hex_string(entropy[:num_bytes])}
     # PWD BASE64
     elif application == "707764'":
         pwd_len = int(indexes[0][:-1])
-        # TODO file Base64 typo in 85 "encode the all 64 bytes of entropy".
         if not (20 <= pwd_len <= 86):
             raise ValueError(f"Expected pwd_len in [20, 86], got {pwd_len}")
 
         return {
             "entropy": entropy,
             "application": base64.b64encode(entropy).decode("utf-8")[:pwd_len],
         }
@@ -164,7 +155,15 @@
     if segments[0] != "m":
         raise ValueError(f"Expected 'm' (xprv) at root of derivation path: {path}")
     pattern = r"^\d+['hH]?$"
     if not all(re.match(pattern, s) for s in segments[1:]):
         raise ValueError(f"Unexpected path segments: {path}")
 
     return segments
+
+
+def validate_key(entropy: bytes):
+    """per BIP-85 we should hard fail under these conditions"""
+    assert len(entropy) == 32
+    int_key = int.from_bytes(entropy, "big")
+    if not int_key or int_key > SECP256k1.order:
+        raise ValueError("Invalid derived key. Try again with next child index.")
```

### Comparing `bipsea-0.1.1/src/bipsea/bipsea.py` & `bipsea-0.1.2/src/bipsea/bipsea.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .seedwords import (
     N_WORDS_ALLOWED,
     bip39_english_words,
     entropy_to_words,
     to_master_seed,
     warn_stretching,
 )
-from .util import LOGGER, __version__, to_hex_string
+from .util import LOGGER, __app_name__, __version__, to_hex_string
 
 SEED_FROM_VALUES = [
     "string",
     "rand",
     "words",
 ]
 SEED_TO_VALUES = [
@@ -36,15 +36,15 @@
 APPLICATIONS = {
     "base64": "707764'",
     "base85": "707785'",
     "drng": None,
     "hex": "128169'",
     "words": "39'",
     "wif": "2'",
-    "xprv": "32'",  # TODO file to 85 is there a testnet here
+    "xprv": "32'",
 }
 
 RANGES = {
     "base64": (20, 86),
     "base85": (10, 80),
     "hex": (16, 64),
 }
@@ -58,15 +58,15 @@
 
 class InputThread(threading.Thread):
     def run(self):
         self.seed = click.get_text_stream("stdin").read().strip()
 
 
 @click.group()
-@click.version_option(version=__version__, prog_name="bipsea")
+@click.version_option(version=__version__, prog_name=__app_name__)
 def cli():
     pass
 
 
 @click.command(help="Generate a master private seed")
 @click.option(
     "-f",
@@ -226,17 +226,15 @@
         path += f"/0'/{number}'/{index}'"
     elif application in ("wif", "xprv"):
         path += f"/{index}'"
     elif application in ("hex", "base64", "base85"):
         path += f"/{number}'/{index}'"
         check_range(number, application)
     elif application == "drng":
-        # TODO file to 85: not clear structure if master root keys; is it {0'}/{index}'?
         path += f"/0'/{index}'"
-    # TODO do we need to derive testnet?
     derived = derive(master, path)
     if application == "drng":
         drng = DRNG(to_entropy(derived.data[1:]))
         output = to_hex_string(drng.read(number))
     else:
         output = apply_85(derived, path)["application"]
     click.echo(output)
```

### Comparing `bipsea-0.1.1/src/bipsea/seedwords.py` & `bipsea-0.1.2/src/bipsea/seedwords.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 #!/usr/bin/python
-"""Complete implementation of BIP-39 in Python with CLI
-https://en.bitcoin.it/wiki/BIP_0039
-
-TODO: CLI design:
-(xprv or seed or entropy) | derivation path > output?
-"""
+"""Complete BIP-39 implementation"""
 
 import hashlib
 import logging
 import secrets
 import warnings
 from hashlib import pbkdf2_hmac
 from typing import List
 from unicodedata import normalize
 
 import click
 
-from .util import LOGGER, from_hex
+from .util import LOGGER
 
 logger = logging.getLogger(LOGGER)
 
 
 # https://raw.githubusercontent.com/bitcoin/bips/master/bip-0039/english.txt
 DICT_NAME = "english.txt"
 DICT_HASH = "2f5eed53a4727b4bf8880d8f3f199efc90e58503646d9ff8eff3a2ed3b24dbda"
```

### Comparing `bipsea-0.1.1/src/bipsea/util.py` & `bipsea-0.1.2/src/bipsea/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 """constants and utilities"""
 
 import binascii
 import logging
 from hashlib import pbkdf2_hmac
 from unicodedata import normalize as unicode_normalize
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __app_name__ = "bipsea"
 
 FORMAT = "utf-8"
 NFKD = "NFKD"
 LOGGER = __app_name__
 
 
 logger = logging.getLogger(LOGGER)
 
 
-def from_hex(input: str, passphrase: str = "") -> bytes:
-    return bytes.fromhex(input + passphrase)
-
-
 def to_hex_string(data: bytes) -> str:
     return binascii.hexlify(data).decode("utf-8")
 
 
 def pbkdf2(
     mnemonic: str, passphrase: str, iterations: int = 2048, hash_name: str = "sha512"
 ) -> bytes:
```

### Comparing `bipsea-0.1.1/src/bipsea.egg-info/PKG-INFO` & `bipsea-0.1.2/src/bipsea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipsea
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python implementation of BIP 85 (and BIP 32)
 Author: Aneesh Karve
 Author-email: bonded_metals_0u@icloud.com
 Project-URL: Source, https://github.com/akarve/bipsea
 Keywords: Bitcoin BIP85 BIP32 cryptography
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bipsea-0.1.1/tests/test_bip32.py` & `bipsea-0.1.2/tests/test_bip32.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 import pytest
 from data.bip32_vectors import INVALID_KEYS, VECTORS
 
 from bipsea.bip32 import to_master_key
 from bipsea.bip32types import parse_ext_key
 from bipsea.bip85 import derive
-from bipsea.util import LOGGER, from_hex
+from bipsea.util import LOGGER
 
 logger = logging.getLogger(LOGGER)
 
 
 @pytest.mark.parametrize(
     "vector",
     VECTORS,
     ids=[
         f"Vector-{i + 1}-{', '.join(e['chain'].keys())}" for i, e in enumerate(VECTORS)
     ],
 )
 def test_vectors(vector):
-    seed = from_hex(vector["seed_hex"])
+    seed = bytes.fromhex(vector["seed_hex"])
     for ch, tests in vector["chain"].items():
         for type_, expected in tests.items():
             assert type_ in ("ext pub", "ext prv")
             master = to_master_key(seed, mainnet=True, private=True)
             derived = derive(master, ch, private=type_ == "ext prv")
             if not str(derived) == expected:
                 logger.error("derived:")
```

### Comparing `bipsea-0.1.1/tests/test_bip39.py` & `bipsea-0.1.2/tests/test_bip39.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,44 @@
 
 import pytest
 import requests
 from data.bip39_vectors import VECTORS
 
 from bipsea.bip32 import to_master_key
 from bipsea.seedwords import DICT_HASH, N_MNEMONICS, entropy_to_words, to_master_seed
-from bipsea.util import LOGGER, from_hex
+from bipsea.util import LOGGER
 
 logger = logging.getLogger(LOGGER)
 
 WORD_COUNTS = {12, 15, 18, 21, 24}
 
 
 @pytest.mark.parametrize(
     "language, vectors", VECTORS.items(), ids=[l for l in VECTORS.keys()]
 )
 def test_vectors(language, vectors):
     for vector in vectors:
         _, mnemonic, seed, xprv = vector
         expected_words = re.split(r"\s", mnemonic)
-        expected_seed = from_hex(seed)
+        expected_seed = bytes.fromhex(seed)
         computed_seed = to_master_seed(expected_words, passphrase="TREZOR")
         assert expected_seed == computed_seed
         computed_xprv = to_master_key(expected_seed, mainnet=True, private=True)
         assert str(computed_xprv) == xprv
 
 
 @pytest.mark.parametrize(
     "language, vectors", VECTORS.items(), ids=[l for l in VECTORS.keys()]
 )
 def test_seed_word_generation(language, vectors):
     for vector in vectors:
         entropy_str, mnemonic, seed, xprv = vector
         expected_words = re.split(r"\s", mnemonic)
         if language == "english":
-            entropy_bytes = from_hex(entropy_str)
+            entropy_bytes = bytes.fromhex(entropy_str)
             if all(b == 0 for b in entropy_bytes):
                 warnings.simplefilter("ignore")
             computed_words = entropy_to_words(
                 len(expected_words), user_entropy=entropy_bytes, passphrase="TREZOR"
             )
             assert expected_words == computed_words
         else:
```

### Comparing `bipsea-0.1.1/tests/test_cli.py` & `bipsea-0.1.2/tests/test_cli.py`

 * *Files identical despite different names*

