# Comparing `tmp/taibun-1.1.4.tar.gz` & `tmp/taibun-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taibun-1.1.4.tar", last modified: Fri May 24 06:35:52 2024, max compression
+gzip compressed data, was "taibun-1.1.5.tar", last modified: Sun May 26 22:48:54 2024, max compression
```

## Comparing `taibun-1.1.4.tar` & `taibun-1.1.5.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 06:35:52.077467 taibun-1.1.4/
--rw-rw-rw-   0        0        0     1099 2024-04-30 01:55:12.000000 taibun-1.1.4/LICENSE
--rw-rw-rw-   0        0        0    16546 2024-05-24 06:35:52.076236 taibun-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    15753 2024-05-24 06:27:44.000000 taibun-1.1.4/README.md
--rw-rw-rw-   0        0        0      103 2024-05-11 09:38:22.000000 taibun-1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      875 2024-05-24 06:35:52.082208 taibun-1.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-24 06:35:51.932963 taibun-1.1.4/taibun/
--rw-rw-rw-   0        0        0       85 2024-05-07 21:05:54.000000 taibun-1.1.4/taibun/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 06:35:51.988478 taibun-1.1.4/taibun/data/
--rw-rw-rw-   0        0        0     2188 2024-05-20 10:19:40.000000 taibun-1.1.4/taibun/data/simplified.json
--rw-rw-rw-   0        0        0    70011 2024-05-20 10:02:42.000000 taibun-1.1.4/taibun/data/traditional.json
--rw-rw-rw-   0        0        0      835 2024-05-20 08:22:03.000000 taibun-1.1.4/taibun/data/vars.json
--rw-rw-rw-   0        0        0  1893399 2024-05-20 08:22:41.000000 taibun-1.1.4/taibun/data/words.json
--rw-rw-rw-   0        0        0    25516 2024-05-22 09:22:31.000000 taibun-1.1.4/taibun/taibun.py
-drwxrwxrwx   0        0        0        0 2024-05-24 06:35:52.072377 taibun-1.1.4/taibun.egg-info/
--rw-rw-rw-   0        0        0    16546 2024-05-24 06:35:51.000000 taibun-1.1.4/taibun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      692 2024-05-24 06:35:51.000000 taibun-1.1.4/taibun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 06:35:51.000000 taibun-1.1.4/taibun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-24 06:35:51.000000 taibun-1.1.4/taibun.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-24 06:35:52.063372 taibun-1.1.4/tests/
--rw-rw-rw-   0        0        0     2350 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_additional.py
--rw-rw-rw-   0        0        0    17804 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_convert_non_cjk.py
--rw-rw-rw-   0        0        0     9343 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_delimiter.py
--rw-rw-rw-   0        0        0     6995 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_format.py
--rw-rw-rw-   0        0        0    18978 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_ipa_conversion.py
--rw-rw-rw-   0        0        0     6841 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_pingyim_conversion.py
--rw-rw-rw-   0        0        0     7306 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_poj_conversion.py
--rw-rw-rw-   0        0        0    12530 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_punctuation.py
--rw-rw-rw-   0        0        0    34066 2024-05-20 09:38:45.000000 taibun-1.1.4/tests/test_sandhi.py
--rw-rw-rw-   0        0        0     7214 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_tailo_conversion.py
--rw-rw-rw-   0        0        0     7304 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_tlpa_conversion.py
--rw-rw-rw-   0        0        0     1573 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_tokenisation.py
--rw-rw-rw-   0        0        0     7197 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_tongiong_conversion.py
--rw-rw-rw-   0        0        0    11681 2024-05-10 21:33:06.000000 taibun-1.1.4/tests/test_zhuyin_conversion.py
+drwxrwxrwx   0        0        0        0 2024-05-26 22:48:54.198033 taibun-1.1.5/
+-rw-rw-rw-   0        0        0     1099 2024-04-30 01:55:12.000000 taibun-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0    16499 2024-05-26 22:48:54.196735 taibun-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    15682 2024-05-26 01:22:11.000000 taibun-1.1.5/README.md
+-rw-rw-rw-   0        0        0      168 2024-05-25 22:32:43.000000 taibun-1.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      909 2024-05-26 22:48:54.202758 taibun-1.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 22:48:54.076652 taibun-1.1.5/taibun/
+-rw-rw-rw-   0        0        0       85 2024-05-07 21:05:54.000000 taibun-1.1.5/taibun/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 22:48:54.136942 taibun-1.1.5/taibun/data/
+-rw-rw-rw-   0        0        0      923 2024-05-25 22:22:35.000000 taibun-1.1.5/taibun/data/simplified.msgpack
+-rw-rw-rw-   0        0        0    36879 2024-05-25 22:22:35.000000 taibun-1.1.5/taibun/data/traditional.msgpack
+-rw-rw-rw-   0        0        0      355 2024-05-25 22:22:35.000000 taibun-1.1.5/taibun/data/vars.msgpack
+-rw-rw-rw-   0        0        0  1258650 2024-05-25 22:22:35.000000 taibun-1.1.5/taibun/data/words.msgpack
+-rw-rw-rw-   0        0        0    25812 2024-05-26 03:06:40.000000 taibun-1.1.5/taibun/taibun.py
+drwxrwxrwx   0        0        0        0 2024-05-26 22:48:54.194675 taibun-1.1.5/taibun.egg-info/
+-rw-rw-rw-   0        0        0    16499 2024-05-26 22:48:54.000000 taibun-1.1.5/taibun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      733 2024-05-26 22:48:54.000000 taibun-1.1.5/taibun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 22:48:54.000000 taibun-1.1.5/taibun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 22:48:54.000000 taibun-1.1.5/taibun.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 22:48:54.000000 taibun-1.1.5/taibun.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 22:48:54.192228 taibun-1.1.5/tests/
+-rw-rw-rw-   0        0        0     2350 2024-05-10 21:33:06.000000 taibun-1.1.5/tests/test_additional.py
+-rw-rw-rw-   0        0        0    17804 2024-05-10 21:33:06.000000 taibun-1.1.5/tests/test_convert_non_cjk.py
+-rw-rw-rw-   0        0        0     9343 2024-05-10 21:33:06.000000 taibun-1.1.5/tests/test_delimiter.py
+-rw-rw-rw-   0        0        0     6995 2024-05-10 21:33:06.000000 taibun-1.1.5/tests/test_format.py
+-rw-rw-rw-   0        0        0    18978 2024-05-10 21:33:06.000000 taibun-1.1.5/tests/test_ipa_conversion.py
+-rw-rw-rw-   0        0        0     6841 2024-05-10 21:33:06.000000 taibun-1.1.5/tests/test_pingyim_conversion.py
+-rw-rw-rw-   0        0        0     7306 2024-05-10 21:33:06.000000 taibun-1.1.5/tests/test_poj_conversion.py
+-rw-rw-rw-   0        0        0    12530 2024-05-26 21:29:57.000000 taibun-1.1.5/tests/test_punctuation.py
+-rw-rw-rw-   0        0        0    34066 2024-05-20 09:38:45.000000 taibun-1.1.5/tests/test_sandhi.py
+-rw-rw-rw-   0        0        0     7214 2024-05-10 21:33:06.000000 taibun-1.1.5/tests/test_tailo_conversion.py
+-rw-rw-rw-   0        0        0     7304 2024-05-10 21:33:06.000000 taibun-1.1.5/tests/test_tlpa_conversion.py
+-rw-rw-rw-   0        0        0     1875 2024-05-26 22:04:14.000000 taibun-1.1.5/tests/test_tokenisation.py
+-rw-rw-rw-   0        0        0     7197 2024-05-10 21:33:06.000000 taibun-1.1.5/tests/test_tongiong_conversion.py
+-rw-rw-rw-   0        0        0    11681 2024-05-10 21:33:06.000000 taibun-1.1.5/tests/test_zhuyin_conversion.py
```

### Comparing `taibun-1.1.4/LICENSE` & `taibun-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `taibun-1.1.4/PKG-INFO` & `taibun-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taibun
-Version: 1.1.4
+Version: 1.1.5
 Summary: Taiwanese Hokkien Transliterator and Tokeniser
 Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov
 Author-email: andrei.harbachov@gmail.com
 License: MIT
 Keywords: python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration,transliterator,tokenization,tokenizer
 Classifier: Topic :: Text Processing :: Linguistic
@@ -13,18 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-
-[台語](readme/README-oan.md) | [國語](readme/README-cmn.md)
-
-
+Requires-Dist: msgpack
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/andreihar/taibun">
     <img src="https://github.com/andreihar/taibun/raw/main/readme/logo.png" alt="Logo" width="90" height="80">
   </a>
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: taibun Version: 1.1.4 Summary: Taiwanese Hokkien
+Metadata-Version: 2.1 Name: taibun Version: 1.1.5 Summary: Taiwanese Hokkien
 Transliterator and Tokeniser Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov Author-email: andrei.harbachov@gmail.com License: MIT
 Keywords:
 python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration,transliterator,tokenization,tokenizer
 Classifier: Topic :: Text Processing :: Linguistic Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
 System :: Microsoft :: Windows Requires-Python: >=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE [å°èª](readme/README-oan.md) | [åèª]
-(readme/README-cmn.md)
+text/markdown License-File: LICENSE Requires-Dist: msgpack
  _[_L_o_g_o_]# Taibun [![Contributions][contributions-badge]][contributions] [![Live
  Demo][demo-badge]][demo] [![Tests][tests-badge]][tests] [![Release][release-
  badge]][release] [![Licence][licence-badge]][licence] [![LinkedIn][linkedin-
   badge]][linkedin] [![Downloads][downloads-badge]][pypi] **Taiwanese Hokkien
      Transliterator and Tokeniser** It has methods that allow to customise
 transliteration and retrieve any necessary information about Taiwanese Hokkien
                                 pronunciation.
```

### Comparing `taibun-1.1.4/README.md` & `taibun-1.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-[台語](readme/README-oan.md) | [國語](readme/README-cmn.md)
-
-
-
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/andreihar/taibun">
     <img src="https://github.com/andreihar/taibun/raw/main/readme/logo.png" alt="Logo" width="90" height="80">
   </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-[å°èª](readme/README-oan.md) | [åèª](readme/README-cmn.md)
+
  _[_L_o_g_o_]# Taibun [![Contributions][contributions-badge]][contributions] [![Live
  Demo][demo-badge]][demo] [![Tests][tests-badge]][tests] [![Release][release-
  badge]][release] [![Licence][licence-badge]][licence] [![LinkedIn][linkedin-
   badge]][linkedin] [![Downloads][downloads-badge]][pypi] **Taiwanese Hokkien
      Transliterator and Tokeniser** It has methods that allow to customise
 transliteration and retrieve any necessary information about Taiwanese Hokkien
                                 pronunciation.
```

### Comparing `taibun-1.1.4/setup.cfg` & `taibun-1.1.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6169 6275 6e0d 0a76 6572 7369   = taibun..versi
-00000020: 6f6e 203d 2031 2e31 2e34 0d0a 6175 7468  on = 1.1.4..auth
+00000020: 6f6e 203d 2031 2e31 2e35 0d0a 6175 7468  on = 1.1.5..auth
 00000030: 6f72 203d 2041 6e64 7265 6920 4861 7262  or = Andrei Harb
 00000040: 6163 686f 760d 0a61 7574 686f 725f 656d  achov..author_em
 00000050: 6169 6c20 3d20 616e 6472 6569 2e68 6172  ail = andrei.har
 00000060: 6261 6368 6f76 4067 6d61 696c 2e63 6f6d  bachov@gmail.com
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 5461 6977 616e 6573 6520 486f 6b6b 6965  Taiwanese Hokkie
 00000090: 6e20 5472 616e 736c 6974 6572 6174 6f72  n Transliterator
@@ -42,14 +42,16 @@
 00000290: 6f6d 616e 697a 6174 696f 6e2c 2074 7261  omanization, tra
 000002a0: 6e73 6c69 7465 7261 7469 6f6e 2c20 7472  nsliteration, tr
 000002b0: 616e 736c 6974 6572 6174 6f72 2c20 746f  ansliterator, to
 000002c0: 6b65 6e69 7a61 7469 6f6e 2c20 746f 6b65  kenization, toke
 000002d0: 6e69 7a65 720d 0a0d 0a5b 6f70 7469 6f6e  nizer....[option
 000002e0: 735d 0d0a 7079 7468 6f6e 5f72 6571 7569  s]..python_requi
 000002f0: 7265 7320 3d20 3e3d 332e 380d 0a70 6163  res = >=3.8..pac
-00000300: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a0d  kages = find:...
-00000310: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-00000320: 655f 6461 7461 5d0d 0a74 6169 6275 6e20  e_data]..taibun 
-00000330: 3d20 6461 7461 2f2a 2e6a 736f 6e0d 0a0d  = data/*.json...
-00000340: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000350: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000360: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000300: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a69  kages = find:..i
+00000310: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
+00000320: 3d20 0d0a 096d 7367 7061 636b 0d0a 0d0a  = ...msgpack....
+00000330: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+00000340: 5f64 6174 615d 0d0a 7461 6962 756e 203d  _data]..taibun =
+00000350: 2064 6174 612f 2a2e 6d73 6770 6163 6b0d   data/*.msgpack.
+00000360: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000370: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000380: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `taibun-1.1.4/taibun/taibun.py` & `taibun-1.1.5/taibun/taibun.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
-import json
+import msgpack
 import re
 import unicodedata
 
 data_dir = os.path.join(os.path.dirname(__file__), "data")
-with open(os.path.join(data_dir, "words.json"), 'r', encoding="utf-8") as f:
-    word_dict = json.load(f)
-with open(os.path.join(data_dir, "traditional.json"), 'r', encoding="utf-8") as f:
-    trad_dict = json.load(f)
-with open(os.path.join(data_dir, "simplified.json"), 'r', encoding="utf-8") as f:
-    simp_dict = {**{v: k for k, v in trad_dict.items() if len(k) == 1}, **json.load(f)}
-with open(os.path.join(data_dir, "vars.json"), 'r', encoding="utf-8") as f:
-    vars_dict = json.load(f)
+with open(os.path.join(data_dir, "words.msgpack"), 'rb') as f:
+    word_dict = msgpack.unpackb(f.read(), raw=False)
+with open(os.path.join(data_dir, "traditional.msgpack"), 'rb') as f:
+    trad_dict = msgpack.unpackb(f.read(), raw=False)
+with open(os.path.join(data_dir, "simplified.msgpack"), 'rb') as f:
+    simp_dict = {**{v: k for k, v in trad_dict.items() if len(k) == 1}, **msgpack.unpackb(f.read(), raw=False)}
+with open(os.path.join(data_dir, "vars.msgpack"), 'rb') as f:
+    vars_dict = msgpack.unpackb(f.read(), raw=False)
 
 # Helper to check if the character is a Chinese character
 def is_cjk(input):
     return all(
         0x4E00 <= ord(char) <= 0x9FFF or  # BASIC
         0x3400 <= ord(char) <= 0x4DBF or  # Ext A
         0x20000 <= ord(char) <= 0x2A6DF or  # Ext B
@@ -441,30 +441,36 @@
 class Tokeniser(object):
 
     def __init__(self, keep_original=True):
         self.keep_original = keep_original
 
     # Tokenise the text into separate words
     def tokenise(self, input):
-        tokenised = []
         traditional = to_traditional(input)
-        while traditional:
-            for j in range (4, 0, -1):
-                if len(traditional) < j:
-                    continue
-                word = traditional[:j]
-                if word_dict.get(word) or j == 1:
-                    if j == 1 and tokenised and not (is_cjk(tokenised[-1]) or is_cjk(word)):
-                        tokenised[-1] += word
-                    else:
-                        tokenised.append(word)
-                    traditional = traditional[j:]
-                    break
+        n = len(traditional)
+        dp = [{'score': float('inf'), 'last_word': None} for _ in range(n+1)]
+        dp[0]['score'] = 0
+        for i in range(1, n+1):
+            for j in range(max(0, i-4), i):
+                word = traditional[j:i]
+                if word_dict.get(word) or len(word) == 1:
+                    score = dp[j]['score'] + 1
+                    if score < dp[i]['score']:
+                        dp[i]['score'] = score
+                        dp[i]['last_word'] = word
+        tokenised = []
+        i = n
+        while i > 0:
+            word = dp[i]['last_word']
+            if tokenised and not (is_cjk(tokenised[-1]) or is_cjk(word)):
+                tokenised[-1] = word + tokenised[-1]
             else:
-                traditional = ""
+                tokenised.append(word)
+            i -= len(word)
+        tokenised.reverse()
         punctuations = re.compile(r"([.,!?\"#$%&()*+/:;<=>@[\]^`{|}~\t。．，、！？；：（）［］【】「」“”]\s*)")
         if self.keep_original:
             indices = [0] + [len(item) for item in tokenised]
             tokenised = [input[sum(indices[:i+1]):sum(indices[:i+2])] for i in range(len(indices)-1)]
         tokenised = [
             item 
             for word in tokenised
```

### Comparing `taibun-1.1.4/taibun.egg-info/PKG-INFO` & `taibun-1.1.5/taibun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taibun
-Version: 1.1.4
+Version: 1.1.5
 Summary: Taiwanese Hokkien Transliterator and Tokeniser
 Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov
 Author-email: andrei.harbachov@gmail.com
 License: MIT
 Keywords: python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration,transliterator,tokenization,tokenizer
 Classifier: Topic :: Text Processing :: Linguistic
@@ -13,18 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-
-[台語](readme/README-oan.md) | [國語](readme/README-cmn.md)
-
-
+Requires-Dist: msgpack
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/andreihar/taibun">
     <img src="https://github.com/andreihar/taibun/raw/main/readme/logo.png" alt="Logo" width="90" height="80">
   </a>
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: taibun Version: 1.1.4 Summary: Taiwanese Hokkien
+Metadata-Version: 2.1 Name: taibun Version: 1.1.5 Summary: Taiwanese Hokkien
 Transliterator and Tokeniser Home-page: https://github.com/andreihar/taibun
 Author: Andrei Harbachov Author-email: andrei.harbachov@gmail.com License: MIT
 Keywords:
 python,taiwan,taiwanese,taigi,hokkien,romanization,transliteration,transliterator,tokenization,tokenizer
 Classifier: Topic :: Text Processing :: Linguistic Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
 System :: Microsoft :: Windows Requires-Python: >=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE [å°èª](readme/README-oan.md) | [åèª]
-(readme/README-cmn.md)
+text/markdown License-File: LICENSE Requires-Dist: msgpack
  _[_L_o_g_o_]# Taibun [![Contributions][contributions-badge]][contributions] [![Live
  Demo][demo-badge]][demo] [![Tests][tests-badge]][tests] [![Release][release-
  badge]][release] [![Licence][licence-badge]][licence] [![LinkedIn][linkedin-
   badge]][linkedin] [![Downloads][downloads-badge]][pypi] **Taiwanese Hokkien
      Transliterator and Tokeniser** It has methods that allow to customise
 transliteration and retrieve any necessary information about Taiwanese Hokkien
                                 pronunciation.
```

### Comparing `taibun-1.1.4/taibun.egg-info/SOURCES.txt` & `taibun-1.1.5/taibun.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 pyproject.toml
 setup.cfg
 taibun/__init__.py
 taibun/taibun.py
 taibun.egg-info/PKG-INFO
 taibun.egg-info/SOURCES.txt
 taibun.egg-info/dependency_links.txt
+taibun.egg-info/requires.txt
 taibun.egg-info/top_level.txt
-taibun/data/simplified.json
-taibun/data/traditional.json
-taibun/data/vars.json
-taibun/data/words.json
+taibun/data/simplified.msgpack
+taibun/data/traditional.msgpack
+taibun/data/vars.msgpack
+taibun/data/words.msgpack
 tests/test_additional.py
 tests/test_convert_non_cjk.py
 tests/test_delimiter.py
 tests/test_format.py
 tests/test_ipa_conversion.py
 tests/test_pingyim_conversion.py
 tests/test_poj_conversion.py
```

### Comparing `taibun-1.1.4/tests/test_additional.py` & `taibun-1.1.5/tests/test_additional.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.4/tests/test_convert_non_cjk.py` & `taibun-1.1.5/tests/test_convert_non_cjk.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.4/tests/test_delimiter.py` & `taibun-1.1.5/tests/test_delimiter.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.4/tests/test_format.py` & `taibun-1.1.5/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.4/tests/test_ipa_conversion.py` & `taibun-1.1.5/tests/test_ipa_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.4/tests/test_pingyim_conversion.py` & `taibun-1.1.5/tests/test_pingyim_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.4/tests/test_poj_conversion.py` & `taibun-1.1.5/tests/test_poj_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.4/tests/test_punctuation.py` & `taibun-1.1.5/tests/test_punctuation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from taibun.taibun import Converter
 from utils import checker
 
 hanji_data = ["這是臺南，簡稱「南」（白話字：Tâi-lâm；注音符號：ㄊㄞˊ ㄋㄢˊ，國語：Táinán）。1623年，荷蘭佇臺南近海中个安平起基地。1624年，荷蘭退出澎湖了後，對遮个開發，建設了熱蘭遮城（Fort Zeelandia）。"]
 
 def test_format():
 	test_data = [
-		(['Tse sī Tâi-lâm, kán-tshing "lâm" (Pe̍h-uē-jī: Tâi-lâm; tsù-im hû-hō: ㄊㄞˊ ㄋㄢˊ, kok-gí: Táinán). 1623 nî, Hô-lân tī Tâi-lâm kīn-hái tiong ê an-pîng khí-ki tē. 1624 nî, Hô-lân thè tshut Phênn-ôo liáu-āu, tuì-tsia ê khai-huat, kiàn-siat liáu Jia̍t-lân-jia-siânn (Fort Zeelandia)./Tse sī Tâi-lâm, kán-tshing "lâm" (Pe̍h-uē-lī: Tâi-lâm; tsù-im hû-hō: ㄊㄞˊ ㄋㄢˊ, kok-gú: Táinán). 1623 nî, Hô-lân tī Tâi-lâm kūn-hái tiong ê an-pîng khí-ki tuē. 1624 nî, Hô-lân thè tshut Phênn-ôo liáu-āu, tuì-tsia ê khai-huat, kiàn-siat liáu Lia̍t-lân-lia-siânn (Fort Zeelandia).'], "Tailo"),
-		(['Che sī Tâi-lâm, kán-chheng "lâm" (Pe̍h-ōe-jī: Tâi-lâm; chù-im hû-hō: ㄊㄞˊ ㄋㄢˊ, kok-gí: Táinán). 1623 nî, Hô-lân tī Tâi-lâm kīn-hái tiong ê an-pêng khí-ki tē. 1624 nî, Hô-lân thè chhut Phêⁿ-ô͘ liáu-āu, tùi-chia ê khai-hoat, kiàn-siat liáu Jia̍t-lân-jia-siâⁿ (Fort Zeelandia)./Che sī Tâi-lâm, kán-chheng "lâm" (Pe̍h-ōe-lī: Tâi-lâm; chù-im hû-hō: ㄊㄞˊ ㄋㄢˊ, kok-gú: Táinán). 1623 nî, Hô-lân tī Tâi-lâm kūn-hái tiong ê an-pêng khí-ki tōe. 1624 nî, Hô-lân thè chhut Phêⁿ-ô͘ liáu-āu, tùi-chia ê khai-hoat, kiàn-siat liáu Lia̍t-lân-lia-siâⁿ (Fort Zeelandia).'], "POJ"),
+		(['Tse sī Tâi-lâm, kán-tshing "lâm" (Pe̍h-uē-jī: Tâi-lâm; tsù-im hû-hō: ㄊㄞˊ ㄋㄢˊ, kok-gí: Táinán). 1623 nî, Hô-lân tī Tâi-lâm kīn-hái tiong ê an-pîng khí ki-tē. 1624 nî, Hô-lân thè tshut Phênn-ôo liáu-āu, tuì-tsia ê khai-huat, kiàn-siat liáu Jia̍t-lân-jia-siânn (Fort Zeelandia)./Tse sī Tâi-lâm, kán-tshing "lâm" (Pe̍h-uē-lī: Tâi-lâm; tsù-im hû-hō: ㄊㄞˊ ㄋㄢˊ, kok-gú: Táinán). 1623 nî, Hô-lân tī Tâi-lâm kūn-hái tiong ê an-pîng khí ki-tuē. 1624 nî, Hô-lân thè tshut Phênn-ôo liáu-āu, tuì-tsia ê khai-huat, kiàn-siat liáu Lia̍t-lân-lia-siânn (Fort Zeelandia).'], "Tailo"),
+		(['Che sī Tâi-lâm, kán-chheng "lâm" (Pe̍h-ōe-jī: Tâi-lâm; chù-im hû-hō: ㄊㄞˊ ㄋㄢˊ, kok-gí: Táinán). 1623 nî, Hô-lân tī Tâi-lâm kīn-hái tiong ê an-pêng khí ki-tē. 1624 nî, Hô-lân thè chhut Phêⁿ-ô͘ liáu-āu, tùi-chia ê khai-hoat, kiàn-siat liáu Jia̍t-lân-jia-siâⁿ (Fort Zeelandia)./Che sī Tâi-lâm, kán-chheng "lâm" (Pe̍h-ōe-lī: Tâi-lâm; chù-im hû-hō: ㄊㄞˊ ㄋㄢˊ, kok-gú: Táinán). 1623 nî, Hô-lân tī Tâi-lâm kūn-hái tiong ê an-pêng khí ki-tōe. 1624 nî, Hô-lân thè chhut Phêⁿ-ô͘ liáu-āu, tùi-chia ê khai-hoat, kiàn-siat liáu Lia̍t-lân-lia-siâⁿ (Fort Zeelandia).'], "POJ"),
 		(['ㄗㆤ ㄒㄧ˫ ㄉㄞˊ ㄌㆰˊ, ㄍㄢˋ ㄑㄧㄥ "ㄌㆰˊ" (ㄅㆤㆷ˙ ㄨㆤ˫ ㆢㄧ˫: Tâi-lâm; ㄗㄨ˪ ㄧㆬ ㄏㄨˊ ㄏㄜ˫: ㄊㄞˊ ㄋㄢˊ, ㄍㆦㆶ ㆣㄧˋ: Táinán). 1623 ㄋㄧˊ, ㄏㄜˊ ㄌㄢˊ ㄉㄧ˫ ㄉㄞˊ ㄌㆰˊ ㄍㄧㄣ˫ ㄏㄞˋ ㄉㄧㆲ ㆤˊ ㄢ ㄅㄧㄥˊ ㄎㄧˋ ㄍㄧ ㄉㆤ˫. 1624 ㄋㄧˊ, ㄏㄜˊ ㄌㄢˊ ㄊㆤ˪ ㄘㄨㆵ ㄆㆥˊ ㆦˊ ㄌㄧㄠˋ ㄠ˫, ㄉㄨㄧ˪ ㄐㄧㄚ ㆤˊ ㄎㄞ ㄏㄨㄚㆵ, ㄍㄧㄢ˪ ㄒㄧㄚㆵ ㄌㄧㄠˋ ㆢㄧㄚㆵ˙ ㄌㄢˊ ㆢㄧㄚ ㄒㄧㆩˊ (Fort Zeelandia)./ㄗㆤ ㄒㄧ˫ ㄉㄞˊ ㄌㆰˊ, ㄍㄢˋ ㄑㄧㄥ "ㄌㆰˊ" (ㄅㆤㆷ˙ ㄨㆤ˫ ㄌㄧ˫: Tâi-lâm; ㄗㄨ˪ ㄧㆬ ㄏㄨˊ ㄏㄜ˫: ㄊㄞˊ ㄋㄢˊ, ㄍㆦㆶ ㆣㄨˋ: Táinán). 1623 ㄋㄧˊ, ㄏㄜˊ ㄌㄢˊ ㄉㄧ˫ ㄉㄞˊ ㄌㆰˊ ㄍㄨㄣ˫ ㄏㄞˋ ㄉㄧㆲ ㆤˊ ㄢ ㄅㄧㄥˊ ㄎㄧˋ ㄍㄧ ㄉㄨㆤ˫. 1624 ㄋㄧˊ, ㄏㄜˊ ㄌㄢˊ ㄊㆤ˪ ㄘㄨㆵ ㄆㆥˊ ㆦˊ ㄌㄧㄠˋ ㄠ˫, ㄉㄨㄧ˪ ㄐㄧㄚ ㆤˊ ㄎㄞ ㄏㄨㄚㆵ, ㄍㄧㄢ˪ ㄒㄧㄚㆵ ㄌㄧㄠˋ ㄌㄧㄚㆵ˙ ㄌㄢˊ ㄌㄧㄚ ㄒㄧㆩˊ (Fort Zeelandia).'], "Zhuyin"),
 		(['Ce1 si7 Tai5 lam5, kan2 ching1 "lam5" (Peh8 ue7 ji7: Tâi-lâm; cu3 im1 hu5 ho7: ㄊㄞˊ ㄋㄢˊ, kok4 gi2: Táinán). 1623 ni5, Ho5 lan5 ti7 Tai5 lam5 kin7 hai2 tiong1 e5 an1 ping5 khi2 ki1 te7. 1624 ni5, Ho5 lan5 the3 chut4 Phenn5 oo5 liau2 au7, tui3 cia1 e5 khai1 huat4, kian3 siat4 liau2 Jiat8 lan5 jia1 siann5 (Fort Zeelandia)./Ce1 si7 Tai5 lam5, kan2 ching1 "lam5" (Peh8 ue7 li7: Tâi-lâm; cu3 im1 hu5 ho7: ㄊㄞˊ ㄋㄢˊ, kok4 gu2: Táinán). 1623 ni5, Ho5 lan5 ti7 Tai5 lam5 kun7 hai2 tiong1 e5 an1 ping5 khi2 ki1 tue7. 1624 ni5, Ho5 lan5 the3 chut4 Phenn5 oo5 liau2 au7, tui3 cia1 e5 khai1 huat4, kian3 siat4 liau2 Liat8 lan5 lia1 siann5 (Fort Zeelandia).'], "TLPA"),
-		(['Zē sî Dáilám, gǎncīng "lám" (Béhwêzzî: Tâi-lâm; zùyīm húhô: ㄊㄞˊ ㄋㄢˊ, gōkggǐ: Táinán). 1623 lní, Hólán dî Dáilám gînhǎi diōng é ānbíng kǐgī dê. 1624 lní, Hólán tè cūt Pnéoó liǎoâo, duìziā é kāihuāt, giànsiāt liǎo Zziátlánzziāsiná (Fort Zeelandia)./Zē sî Dáilám, gǎncīng "lám" (Béhwêlî: Tâi-lâm; zùyīm húhô: ㄊㄞˊ ㄋㄢˊ, gōkggǔ: Táinán). 1623 lní, Hólán dî Dáilám gûnhǎi diōng é ānbíng kǐgī duê. 1624 lní, Hólán tè cūt Pnéoó liǎoâo, duìziā é kāihuāt, giànsiāt liǎo Liátlánliāsiná (Fort Zeelandia).'], "Pingyim"),
-		(['Ze sî Dāi-lăm, gan-cing "lăm" (Bê-uê-rī: Tâi-lâm; zù-īm hū-hōr: ㄊㄞˊ ㄋㄢˊ, gok-ghì: Táinán). 1623 nĭ, Hōr-lān dî Dāi-lām gîn-hai diōng ē ān-bīng ki-gī dē. 1624 nĭ, Hōr-lān tè cut Pēnn-ōr liau-āu, duì-ziā ē kāi-huāt, giàn-siat liau Riāt-lān-riā-siănn (Fort Zeelandia)./Ze sî Dâi-lăm, gan-cing "lăm" (Bê-uê-lī: Tâi-lâm; zù-īm hû-hōr: ㄊㄞˊ ㄋㄢˊ, gok-ghù: Táinán). 1623 nĭ, Hôr-lân dî Dâi-lâm gûn-hai diōng ê ān-bîng ki-gī duē. 1624 nĭ, Hôr-lân tè cut Pênn-ôr liau-āu, duì-ziā ê kāi-huāt, giàn-siat liau Liāt-lân-liā-siănn (Fort Zeelandia).'], "Tongiong"),
+		(['Zē sî Dáilám, gǎncīng "lám" (Béhwêzzî: Tâi-lâm; zùyīm húhô: ㄊㄞˊ ㄋㄢˊ, gōkggǐ: Táinán). 1623 lní, Hólán dî Dáilám gînhǎi diōng é ānbíng kǐ gīdê. 1624 lní, Hólán tè cūt Pnéoó liǎoâo, duìziā é kāihuāt, giànsiāt liǎo Zziátlánzziāsiná (Fort Zeelandia)./Zē sî Dáilám, gǎncīng "lám" (Béhwêlî: Tâi-lâm; zùyīm húhô: ㄊㄞˊ ㄋㄢˊ, gōkggǔ: Táinán). 1623 lní, Hólán dî Dáilám gûnhǎi diōng é ānbíng kǐ gīduê. 1624 lní, Hólán tè cūt Pnéoó liǎoâo, duìziā é kāihuāt, giànsiāt liǎo Liátlánliāsiná (Fort Zeelandia).'], "Pingyim"),
+		(['Ze sî Dāi-lăm, gan-cing "lăm" (Bê-uê-rī: Tâi-lâm; zù-īm hū-hōr: ㄊㄞˊ ㄋㄢˊ, gok-ghì: Táinán). 1623 nĭ, Hōr-lān dî Dāi-lām gîn-hai diōng ē ān-bīng ki gī-dē. 1624 nĭ, Hōr-lān tè cut Pēnn-ōr liau-āu, duì-ziā ē kāi-huāt, giàn-siat liau Riāt-lān-riā-siănn (Fort Zeelandia)./Ze sî Dâi-lăm, gan-cing "lăm" (Bê-uê-lī: Tâi-lâm; zù-īm hû-hōr: ㄊㄞˊ ㄋㄢˊ, gok-ghù: Táinán). 1623 nĭ, Hôr-lân dî Dâi-lâm gûn-hai diōng ê ān-bîng ki gī-duē. 1624 nĭ, Hôr-lân tè cut Pênn-ôr liau-āu, duì-ziā ê kāi-huāt, giàn-siat liau Liāt-lân-liā-siănn (Fort Zeelandia).'], "Tongiong"),
 		(['Tse⁴⁴ ɕi²² Tai²⁵ lam²⁵, kan⁵³ tɕʰiɪŋ⁴⁴ "lam²⁵" (Peʔ⁵ ue²² dʑi²²: Tâi-lâm; tsu¹¹ im⁴⁴ hu²⁵ hə²²: ㄊㄞˊ ㄋㄢˊ, kɔk̚²¹ gi⁵³: Táinán). 1623 nĩ²⁵, Hə²⁵ lan²⁵ ti²² Tai²⁵ lam²⁵ kin²² hai⁵³ tiɔŋ⁴⁴ e²⁵ an⁴⁴ piɪŋ²⁵ kʰi⁵³ ki⁴⁴ te²². 1624 nĩ²⁵, Hə²⁵ lan²⁵ tʰe¹¹ tsʰut̚²¹ Pʰẽ²⁵ ɔ²⁵ liau⁵³ au²², tui¹¹ tɕia⁴⁴ e²⁵ kʰai⁴⁴ huat̚²¹, kiɛn¹¹ ɕiɛt̚²¹ liau⁵³ Dʑiɛt̚⁵ lan²⁵ dʑia⁴⁴ ɕiã²⁵ (Fort Zeelandia)./Tse⁵⁵ ɕi³³ Tai²⁴ lam²⁴, kan⁵¹ tɕʰiɪŋ⁵⁵ "lam²⁴" (Peʔ⁴ ue³³ li³³: Tâi-lâm; tsu²¹ im⁵⁵ hu²⁴ ho³³: ㄊㄞˊ ㄋㄢˊ, kɔk̚³² gu⁵¹: Táinán). 1623 nĩ²⁴, Ho²⁴ lan²⁴ ti³³ Tai²⁴ lam²⁴ kun³³ hai⁵¹ tiɔŋ⁵⁵ e²⁴ an⁵⁵ piɪŋ²⁴ kʰi⁵¹ ki⁵⁵ tue³³. 1624 nĩ²⁴, Ho²⁴ lan²⁴ tʰe²¹ tsʰut̚³² Pʰẽ²⁴ ɔ²⁴ liau⁵¹ au³³, tui²¹ tɕia⁵⁵ e²⁴ kʰai⁵⁵ huat̚³², kiɛn²¹ ɕiɛt̚³² liau⁵¹ Liɛt̚⁴ lan²⁴ lia⁵⁵ ɕiã²⁴ (Fort Zeelandia).'], "IPA")
 	]
 	for transl, system in test_data:
 		data = list(zip(hanji_data, transl))
 		checker(data, Converter(system=system, punctuation='format'), Converter(system=system, dialect="north", punctuation='format'))
 
 def test_none():
 	test_data = [
-		(['tse sī Tâi-lâm，kán-tshing「lâm」（Pe̍h-uē-jī：Tâi-lâm；tsù-im hû-hō：ㄊㄞˊ ㄋㄢˊ，kok-gí：Táinán）。1623 nî，Hô-lân tī Tâi-lâm kīn-hái tiong ê an-pîng khí-ki tē。1624 nî，Hô-lân thè tshut Phênn-ôo liáu-āu，tuì-tsia ê khai-huat，kiàn-siat liáu Jia̍t-lân-jia-siânn（Fort Zeelandia）。/tse sī Tâi-lâm，kán-tshing「lâm」（Pe̍h-uē-lī：Tâi-lâm；tsù-im hû-hō：ㄊㄞˊ ㄋㄢˊ，kok-gú：Táinán）。1623 nî，Hô-lân tī Tâi-lâm kūn-hái tiong ê an-pîng khí-ki tuē。1624 nî，Hô-lân thè tshut Phênn-ôo liáu-āu，tuì-tsia ê khai-huat，kiàn-siat liáu Lia̍t-lân-lia-siânn（Fort Zeelandia）。'], "Tailo"),
-		(['che sī Tâi-lâm，kán-chheng「lâm」（Pe̍h-ōe-jī：Tâi-lâm；chù-im hû-hō：ㄊㄞˊ ㄋㄢˊ，kok-gí：Táinán）。1623 nî，Hô-lân tī Tâi-lâm kīn-hái tiong ê an-pêng khí-ki tē。1624 nî，Hô-lân thè chhut Phêⁿ-ô͘ liáu-āu，tùi-chia ê khai-hoat，kiàn-siat liáu Jia̍t-lân-jia-siâⁿ（Fort Zeelandia）。/che sī Tâi-lâm，kán-chheng「lâm」（Pe̍h-ōe-lī：Tâi-lâm；chù-im hû-hō：ㄊㄞˊ ㄋㄢˊ，kok-gú：Táinán）。1623 nî，Hô-lân tī Tâi-lâm kūn-hái tiong ê an-pêng khí-ki tōe。1624 nî，Hô-lân thè chhut Phêⁿ-ô͘ liáu-āu，tùi-chia ê khai-hoat，kiàn-siat liáu Lia̍t-lân-lia-siâⁿ（Fort Zeelandia）。'], "POJ"),
+		(['tse sī Tâi-lâm，kán-tshing「lâm」（Pe̍h-uē-jī：Tâi-lâm；tsù-im hû-hō：ㄊㄞˊ ㄋㄢˊ，kok-gí：Táinán）。1623 nî，Hô-lân tī Tâi-lâm kīn-hái tiong ê an-pîng khí ki-tē。1624 nî，Hô-lân thè tshut Phênn-ôo liáu-āu，tuì-tsia ê khai-huat，kiàn-siat liáu Jia̍t-lân-jia-siânn（Fort Zeelandia）。/tse sī Tâi-lâm，kán-tshing「lâm」（Pe̍h-uē-lī：Tâi-lâm；tsù-im hû-hō：ㄊㄞˊ ㄋㄢˊ，kok-gú：Táinán）。1623 nî，Hô-lân tī Tâi-lâm kūn-hái tiong ê an-pîng khí ki-tuē。1624 nî，Hô-lân thè tshut Phênn-ôo liáu-āu，tuì-tsia ê khai-huat，kiàn-siat liáu Lia̍t-lân-lia-siânn（Fort Zeelandia）。'], "Tailo"),
+		(['che sī Tâi-lâm，kán-chheng「lâm」（Pe̍h-ōe-jī：Tâi-lâm；chù-im hû-hō：ㄊㄞˊ ㄋㄢˊ，kok-gí：Táinán）。1623 nî，Hô-lân tī Tâi-lâm kīn-hái tiong ê an-pêng khí ki-tē。1624 nî，Hô-lân thè chhut Phêⁿ-ô͘ liáu-āu，tùi-chia ê khai-hoat，kiàn-siat liáu Jia̍t-lân-jia-siâⁿ（Fort Zeelandia）。/che sī Tâi-lâm，kán-chheng「lâm」（Pe̍h-ōe-lī：Tâi-lâm；chù-im hû-hō：ㄊㄞˊ ㄋㄢˊ，kok-gú：Táinán）。1623 nî，Hô-lân tī Tâi-lâm kūn-hái tiong ê an-pêng khí ki-tōe。1624 nî，Hô-lân thè chhut Phêⁿ-ô͘ liáu-āu，tùi-chia ê khai-hoat，kiàn-siat liáu Lia̍t-lân-lia-siâⁿ（Fort Zeelandia）。'], "POJ"),
 		(['ㄗㆤ ㄒㄧ˫ ㄉㄞˊ ㄌㆰˊ，ㄍㄢˋ ㄑㄧㄥ「ㄌㆰˊ」（ㄅㆤㆷ˙ ㄨㆤ˫ ㆢㄧ˫：Tâi-lâm；ㄗㄨ˪ ㄧㆬ ㄏㄨˊ ㄏㄜ˫：ㄊㄞˊ ㄋㄢˊ，ㄍㆦㆶ ㆣㄧˋ：Táinán）。1623 ㄋㄧˊ，ㄏㄜˊ ㄌㄢˊ ㄉㄧ˫ ㄉㄞˊ ㄌㆰˊ ㄍㄧㄣ˫ ㄏㄞˋ ㄉㄧㆲ ㆤˊ ㄢ ㄅㄧㄥˊ ㄎㄧˋ ㄍㄧ ㄉㆤ˫。1624 ㄋㄧˊ，ㄏㄜˊ ㄌㄢˊ ㄊㆤ˪ ㄘㄨㆵ ㄆㆥˊ ㆦˊ ㄌㄧㄠˋ ㄠ˫，ㄉㄨㄧ˪ ㄐㄧㄚ ㆤˊ ㄎㄞ ㄏㄨㄚㆵ，ㄍㄧㄢ˪ ㄒㄧㄚㆵ ㄌㄧㄠˋ ㆢㄧㄚㆵ˙ ㄌㄢˊ ㆢㄧㄚ ㄒㄧㆩˊ（Fort Zeelandia）。/ㄗㆤ ㄒㄧ˫ ㄉㄞˊ ㄌㆰˊ，ㄍㄢˋ ㄑㄧㄥ「ㄌㆰˊ」（ㄅㆤㆷ˙ ㄨㆤ˫ ㄌㄧ˫：Tâi-lâm；ㄗㄨ˪ ㄧㆬ ㄏㄨˊ ㄏㄜ˫：ㄊㄞˊ ㄋㄢˊ，ㄍㆦㆶ ㆣㄨˋ：Táinán）。1623 ㄋㄧˊ，ㄏㄜˊ ㄌㄢˊ ㄉㄧ˫ ㄉㄞˊ ㄌㆰˊ ㄍㄨㄣ˫ ㄏㄞˋ ㄉㄧㆲ ㆤˊ ㄢ ㄅㄧㄥˊ ㄎㄧˋ ㄍㄧ ㄉㄨㆤ˫。1624 ㄋㄧˊ，ㄏㄜˊ ㄌㄢˊ ㄊㆤ˪ ㄘㄨㆵ ㄆㆥˊ ㆦˊ ㄌㄧㄠˋ ㄠ˫，ㄉㄨㄧ˪ ㄐㄧㄚ ㆤˊ ㄎㄞ ㄏㄨㄚㆵ，ㄍㄧㄢ˪ ㄒㄧㄚㆵ ㄌㄧㄠˋ ㄌㄧㄚㆵ˙ ㄌㄢˊ ㄌㄧㄚ ㄒㄧㆩˊ（Fort Zeelandia）。'], "Zhuyin"),
 		(['ce1 si7 Tai5 lam5，kan2 ching1「lam5」（Peh8 ue7 ji7：Tâi-lâm；cu3 im1 hu5 ho7：ㄊㄞˊ ㄋㄢˊ，kok4 gi2：Táinán）。1623 ni5，Ho5 lan5 ti7 Tai5 lam5 kin7 hai2 tiong1 e5 an1 ping5 khi2 ki1 te7。1624 ni5，Ho5 lan5 the3 chut4 Phenn5 oo5 liau2 au7，tui3 cia1 e5 khai1 huat4，kian3 siat4 liau2 Jiat8 lan5 jia1 siann5（Fort Zeelandia）。/ce1 si7 Tai5 lam5，kan2 ching1「lam5」（Peh8 ue7 li7：Tâi-lâm；cu3 im1 hu5 ho7：ㄊㄞˊ ㄋㄢˊ，kok4 gu2：Táinán）。1623 ni5，Ho5 lan5 ti7 Tai5 lam5 kun7 hai2 tiong1 e5 an1 ping5 khi2 ki1 tue7。1624 ni5，Ho5 lan5 the3 chut4 Phenn5 oo5 liau2 au7，tui3 cia1 e5 khai1 huat4，kian3 siat4 liau2 Liat8 lan5 lia1 siann5（Fort Zeelandia）。'], "TLPA"),
-		(['zē sî Dáilám，gǎncīng「lám」（Béhwêzzî：Tâi-lâm；zùyīm húhô：ㄊㄞˊ ㄋㄢˊ，gōkggǐ：Táinán）。1623 lní，Hólán dî Dáilám gînhǎi diōng é ānbíng kǐgī dê。1624 lní，Hólán tè cūt Pnéoó liǎoâo，duìziā é kāihuāt，giànsiāt liǎo Zziátlánzziāsiná（Fort Zeelandia）。/zē sî Dáilám，gǎncīng「lám」（Béhwêlî：Tâi-lâm；zùyīm húhô：ㄊㄞˊ ㄋㄢˊ，gōkggǔ：Táinán）。1623 lní，Hólán dî Dáilám gûnhǎi diōng é ānbíng kǐgī duê。1624 lní，Hólán tè cūt Pnéoó liǎoâo，duìziā é kāihuāt，giànsiāt liǎo Liátlánliāsiná（Fort Zeelandia）。'], "Pingyim"),
-		(['ze sî Dāi-lăm，gan-cing「lăm」（Bê-uê-rī：Tâi-lâm；zù-īm hū-hōr：ㄊㄞˊ ㄋㄢˊ，gok-ghì：Táinán）。1623 nĭ，Hōr-lān dî Dāi-lām gîn-hai diōng ē ān-bīng ki-gī dē。1624 nĭ，Hōr-lān tè cut Pēnn-ōr liau-āu，duì-ziā ē kāi-huāt，giàn-siat liau Riāt-lān-riā-siănn（Fort Zeelandia）。/ze sî Dâi-lăm，gan-cing「lăm」（Bê-uê-lī：Tâi-lâm；zù-īm hû-hōr：ㄊㄞˊ ㄋㄢˊ，gok-ghù：Táinán）。1623 nĭ，Hôr-lân dî Dâi-lâm gûn-hai diōng ê ān-bîng ki-gī duē。1624 nĭ，Hôr-lân tè cut Pênn-ôr liau-āu，duì-ziā ê kāi-huāt，giàn-siat liau Liāt-lân-liā-siănn（Fort Zeelandia）。'], "Tongiong"),
+		(['zē sî Dáilám，gǎncīng「lám」（Béhwêzzî：Tâi-lâm；zùyīm húhô：ㄊㄞˊ ㄋㄢˊ，gōkggǐ：Táinán）。1623 lní，Hólán dî Dáilám gînhǎi diōng é ānbíng kǐ gīdê。1624 lní，Hólán tè cūt Pnéoó liǎoâo，duìziā é kāihuāt，giànsiāt liǎo Zziátlánzziāsiná（Fort Zeelandia）。/zē sî Dáilám，gǎncīng「lám」（Béhwêlî：Tâi-lâm；zùyīm húhô：ㄊㄞˊ ㄋㄢˊ，gōkggǔ：Táinán）。1623 lní，Hólán dî Dáilám gûnhǎi diōng é ānbíng kǐ gīduê。1624 lní，Hólán tè cūt Pnéoó liǎoâo，duìziā é kāihuāt，giànsiāt liǎo Liátlánliāsiná（Fort Zeelandia）。'], "Pingyim"),
+		(['ze sî Dāi-lăm，gan-cing「lăm」（Bê-uê-rī：Tâi-lâm；zù-īm hū-hōr：ㄊㄞˊ ㄋㄢˊ，gok-ghì：Táinán）。1623 nĭ，Hōr-lān dî Dāi-lām gîn-hai diōng ē ān-bīng ki gī-dē。1624 nĭ，Hōr-lān tè cut Pēnn-ōr liau-āu，duì-ziā ē kāi-huāt，giàn-siat liau Riāt-lān-riā-siănn（Fort Zeelandia）。/ze sî Dâi-lăm，gan-cing「lăm」（Bê-uê-lī：Tâi-lâm；zù-īm hû-hōr：ㄊㄞˊ ㄋㄢˊ，gok-ghù：Táinán）。1623 nĭ，Hôr-lân dî Dâi-lâm gûn-hai diōng ê ān-bîng ki gī-duē。1624 nĭ，Hôr-lân tè cut Pênn-ôr liau-āu，duì-ziā ê kāi-huāt，giàn-siat liau Liāt-lân-liā-siănn（Fort Zeelandia）。'], "Tongiong"),
 		(['tse⁴⁴ ɕi²² Tai²⁵ lam²⁵，kan⁵³ tɕʰiɪŋ⁴⁴「lam²⁵」（Peʔ⁵ ue²² dʑi²²：Tâi-lâm；tsu¹¹ im⁴⁴ hu²⁵ hə²²：ㄊㄞˊ ㄋㄢˊ，kɔk̚²¹ gi⁵³：Táinán）。1623 nĩ²⁵，Hə²⁵ lan²⁵ ti²² Tai²⁵ lam²⁵ kin²² hai⁵³ tiɔŋ⁴⁴ e²⁵ an⁴⁴ piɪŋ²⁵ kʰi⁵³ ki⁴⁴ te²²。1624 nĩ²⁵，Hə²⁵ lan²⁵ tʰe¹¹ tsʰut̚²¹ Pʰẽ²⁵ ɔ²⁵ liau⁵³ au²²，tui¹¹ tɕia⁴⁴ e²⁵ kʰai⁴⁴ huat̚²¹，kiɛn¹¹ ɕiɛt̚²¹ liau⁵³ Dʑiɛt̚⁵ lan²⁵ dʑia⁴⁴ ɕiã²⁵（Fort Zeelandia）。/tse⁵⁵ ɕi³³ Tai²⁴ lam²⁴，kan⁵¹ tɕʰiɪŋ⁵⁵「lam²⁴」（Peʔ⁴ ue³³ li³³：Tâi-lâm；tsu²¹ im⁵⁵ hu²⁴ ho³³：ㄊㄞˊ ㄋㄢˊ，kɔk̚³² gu⁵¹：Táinán）。1623 nĩ²⁴，Ho²⁴ lan²⁴ ti³³ Tai²⁴ lam²⁴ kun³³ hai⁵¹ tiɔŋ⁵⁵ e²⁴ an⁵⁵ piɪŋ²⁴ kʰi⁵¹ ki⁵⁵ tue³³。1624 nĩ²⁴，Ho²⁴ lan²⁴ tʰe²¹ tsʰut̚³² Pʰẽ²⁴ ɔ²⁴ liau⁵¹ au³³，tui²¹ tɕia⁵⁵ e²⁴ kʰai⁵⁵ huat̚³²，kiɛn²¹ ɕiɛt̚³² liau⁵¹ Liɛt̚⁴ lan²⁴ lia⁵⁵ ɕiã²⁴（Fort Zeelandia）。'], "IPA")
 	]
 	for transl, system in test_data:
 		data = list(zip(hanji_data, transl))
 		checker(data, Converter(system=system, punctuation='none'), Converter(system=system, dialect="north", punctuation='none'))
```

### Comparing `taibun-1.1.4/tests/test_sandhi.py` & `taibun-1.1.5/tests/test_sandhi.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.4/tests/test_tailo_conversion.py` & `taibun-1.1.5/tests/test_tailo_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.4/tests/test_tlpa_conversion.py` & `taibun-1.1.5/tests/test_tlpa_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.4/tests/test_tokenisation.py` & `taibun-1.1.5/tests/test_tokenisation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from taibun.taibun import Tokeniser
 
 def test_general():
 	t = Tokeniser()
 	assert ['太空', '朋友', '，', '恁好', '！', '恁', '食飽', '未', '？'] == t.tokenise("太空朋友，恁好！恁食飽未？")
 	assert ['漢字', '（', '閩南語', '注音', ':', 'ㄏㄢˋ', 'ㆡㄧˉ', '；', '白話字', ':', 'Hàn-jī', '；'] == t.tokenise('漢字（閩南語注音: ㄏㄢˋ ㆡㄧˉ；白話字: Hàn-jī；')
 
+def test_best_solution_tokenisation():
+    t = Tokeniser()
+    assert ['中國', '人民', '共和國'] == t.tokenise("中國人民共和國")
+    assert ['中國人', '民雄', '協會'] == t.tokenise('中國人民雄協會')
+    assert ['花蓮', '市議員'] == t.tokenise('花蓮市議員')
+
 def test_suffix():
 	t = Tokeniser()
-	assert ['咱', '的', '食飯', '是', '誠好', '食'] == t.tokenise("咱的食飯是誠好食")
+	assert ['咱', '的', '食飯', '是', '誠', '好食'] == t.tokenise("咱的食飯是誠好食")
 	assert ['卯死', '矣'] == t.tokenise("卯死矣")
 
 def test_simplified():
 	t = Tokeniser()
 	assert ['汉字', '是', '用来', '写', '几若', '种', '现代', '佮', '古代', '语文', '个', '书写', '文字', '系统', '。'] == t.tokenise('汉字是用来写几若种现代佮古代语文个书写文字系统。')
 	assert ['现代', '个', '中国', '、', '日本', '、', '韩国', '、', '台湾', '拢', '有', '使用', '汉字'] == t.tokenise('现代个中国、日本、韩国、台湾拢有使用汉字')
```

### Comparing `taibun-1.1.4/tests/test_tongiong_conversion.py` & `taibun-1.1.5/tests/test_tongiong_conversion.py`

 * *Files identical despite different names*

### Comparing `taibun-1.1.4/tests/test_zhuyin_conversion.py` & `taibun-1.1.5/tests/test_zhuyin_conversion.py`

 * *Files identical despite different names*

