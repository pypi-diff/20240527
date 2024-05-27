# Comparing `tmp/lions-1.3.2.tar.gz` & `tmp/lions-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lions-1.3.2.tar", last modified: Thu May 23 13:50:01 2024, max compression
+gzip compressed data, was "lions-1.4.0.tar", last modified: Mon May 27 09:44:53 2024, max compression
```

## Comparing `lions-1.3.2.tar` & `lions-1.4.0.tar`

### file list

```diff
@@ -1,40 +1,26 @@
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:50:01.772844 lions-1.3.2/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.3.2/LICENSE
--rw-r--r--   0 diogoferreira   (501) staff       (20)     7975 2024-05-23 13:50:01.772776 lions-1.3.2/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)     7122 2024-05-23 13:49:55.000000 lions-1.3.2/README.md
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:50:01.767344 lions-1.3.2/lions/
--rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.3.2/lions/__init__.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:50:01.768858 lions-1.3.2/lions/cpp_gen/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-07 11:54:56.000000 lions-1.3.2/lions/cpp_gen/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2705 2024-05-23 08:42:03.000000 lions-1.3.2/lions/cpp_gen/cpp_generator.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:50:01.770300 lions-1.3.2/lions/cpp_gen/templates/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1202 2024-05-22 12:07:18.000000 lions-1.3.2/lions/cpp_gen/templates/lions.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1125 2024-05-22 12:07:18.000000 lions-1.3.2/lions/cpp_gen/templates/lions.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2218 2024-05-23 08:42:03.000000 lions-1.3.2/lions/cpp_gen/templates/msg.cpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1519 2024-05-23 08:42:03.000000 lions-1.3.2/lions/cpp_gen/templates/msg.hpp.jinja
--rw-r--r--   0 diogoferreira   (501) staff       (20)     3480 2024-05-23 08:42:03.000000 lions-1.3.2/lions/errors.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:50:01.770604 lions-1.3.2/lions/js_gen/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-23 08:42:03.000000 lions-1.3.2/lions/js_gen/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2780 2024-05-23 08:42:03.000000 lions-1.3.2/lions/js_gen/js_generator.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     5223 2024-05-23 13:46:06.000000 lions-1.3.2/lions/lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     3176 2024-05-23 13:46:06.000000 lions-1.3.2/lions/main.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:50:01.770916 lions-1.3.2/lions/ts_gen/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:46:06.000000 lions-1.3.2/lions/ts_gen/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     3271 2024-05-23 13:46:06.000000 lions-1.3.2/lions/ts_gen/ts_generator.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.3.2/lions/yaml_parser.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:50:01.768508 lions-1.3.2/lions.egg-info/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     7975 2024-05-23 13:50:01.000000 lions-1.3.2/lions.egg-info/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)      748 2024-05-23 13:50:01.000000 lions-1.3.2/lions.egg-info/SOURCES.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-23 13:50:01.000000 lions-1.3.2/lions.egg-info/dependency_links.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-23 13:50:01.000000 lions-1.3.2/lions.egg-info/entry_points.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-23 13:50:01.000000 lions-1.3.2/lions.egg-info/requires.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-23 13:50:01.000000 lions-1.3.2/lions.egg-info/top_level.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-23 13:50:01.773118 lions-1.3.2/setup.cfg
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-23 13:49:55.000000 lions-1.3.2/setup.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-23 13:50:01.772135 lions-1.3.2/tests/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.3.2/tests/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1609 2024-05-23 08:42:03.000000 lions-1.3.2/tests/test_cpp_gen.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1551 2024-05-23 13:46:06.000000 lions-1.3.2/tests/test_js_gen copy.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-23 08:42:03.000000 lions-1.3.2/tests/test_lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1551 2024-05-23 13:46:06.000000 lions-1.3.2/tests/test_ts_gen.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-23 08:42:03.000000 lions-1.3.2/tests/test_yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-27 09:44:53.213848 lions-1.4.0/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.4.0/LICENSE
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8474 2024-05-27 09:44:53.213621 lions-1.4.0/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     7621 2024-05-27 09:43:31.000000 lions-1.4.0/README.md
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-27 09:44:53.209903 lions-1.4.0/lions/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.4.0/lions/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3446 2024-05-27 09:43:31.000000 lions-1.4.0/lions/errors.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     5223 2024-05-23 13:46:06.000000 lions-1.4.0/lions/lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3288 2024-05-27 09:43:31.000000 lions-1.4.0/lions/main.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.4.0/lions/yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-27 09:44:53.211784 lions-1.4.0/lions.egg-info/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8474 2024-05-27 09:44:53.000000 lions-1.4.0/lions.egg-info/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)      427 2024-05-27 09:44:53.000000 lions-1.4.0/lions.egg-info/SOURCES.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-27 09:44:53.000000 lions-1.4.0/lions.egg-info/dependency_links.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-27 09:44:53.000000 lions-1.4.0/lions.egg-info/entry_points.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-27 09:44:53.000000 lions-1.4.0/lions.egg-info/requires.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-27 09:44:53.000000 lions-1.4.0/lions.egg-info/top_level.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-27 09:44:53.214082 lions-1.4.0/setup.cfg
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-27 09:43:31.000000 lions-1.4.0/setup.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-27 09:44:53.212930 lions-1.4.0/tests/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.4.0/tests/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1621 2024-05-27 09:43:31.000000 lions-1.4.0/tests/test_cpp_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1563 2024-05-27 09:43:31.000000 lions-1.4.0/tests/test_js_gen copy.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-23 08:42:03.000000 lions-1.4.0/tests/test_lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1563 2024-05-27 09:43:31.000000 lions-1.4.0/tests/test_ts_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-23 08:42:03.000000 lions-1.4.0/tests/test_yaml_parser.py
```

### Comparing `lions-1.3.2/LICENSE` & `lions-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lions-1.3.2/PKG-INFO` & `lions-1.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.3.2
+Version: 1.4.0
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -58,15 +58,15 @@
 ## Usage
 
     $ lions <msg_files_dir> <output_dir> <target_language>
 
 -   **msg_files_dir**: Directory containing your .lmsg.yaml files
 -   **output_dir**: Directory to place the generated code
 -   **target_language**: Target language for the generated code
-    -   cpp; c; js; ts; py
+    -   cpp / c / js / ts / py
 
 ## Raw Message format
 
 The message structure is composed of a 6-byte header, followed by a variable-length payload. The payload length can range from 0 to 244 bytes, allowing for flexible data encapsulation. Fields within the payload are tightly packed, with no intervening spaces, to maximize message efficiency and minimize overhead.
 
 | Byte Index | Field    | Size (Bytes) | Description                                       |
 | ---------- | -------- | ------------ | ------------------------------------------------- |
@@ -78,14 +78,15 @@
 | 6-249      | payload  | 244          | Actual data payload                               |
 
 ### Code representation
 
 -   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c++/generated_code/lions.hpp)
 -   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/lions.js)
 -   [TypeScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/ts/generated_code/lions.ts)
+-   [Python](https://github.com/ItsNotSoftware/lions/blob/main/examples/python/generated_code/lions.py)
 
 ## Defining Messages
 
 LIONS uses `.lmsg.yaml` files to define message specifications for IoT networks. Each file can contain multiple message definitions that are used by the LIONS compiler to generate C++ code for message handling.
 
 ### Structure of Message Files
 
@@ -175,22 +176,28 @@
     - Transforms a generic, raw-form message (`LMsg`) into the structured format of the class. This conversion facilitates easier manipulation and interpretation of the message contents within the application.
 
 3. **Encode Method**
     - Converts the structured message back into its raw binary form (`LMsg`) for transmission. This method ensures that the message is properly packaged with its header and payload according to the protocol specifications before being sent over the network.
 
 ---
 
+Generated message classes examples:
+
 -   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c%2B%2B/generated_code/my_messages_lmsg.hpp)
 -   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/my_messages_lmsg.js)
 -   [TypeScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/ts/generated_code/my_messages_lmsg.ts)
+-   [Python](https://github.com/ItsNotSoftware/lions/blob/main/examples/python/generated_code/my_messages_lmsg.py)
 
 ## Examples
 
-[Examples](https://github.com/ItsNotSoftware/lions/tree/main/examples)
+-   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples)
+-   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js)
+-   [TypeScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/ts)
+-   [Python](https://github.com/ItsNotSoftware/lions/blob/main/examples/python)
 
 ## Target Language Support
 
 -   [x] C++
 -   [x] JavaScript
 -   [x] TypeScript
+-   [x] Python
 -   [ ] C
--   [ ] Python
```

### Comparing `lions-1.3.2/README.md` & `lions-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 ## Usage
 
     $ lions <msg_files_dir> <output_dir> <target_language>
 
 -   **msg_files_dir**: Directory containing your .lmsg.yaml files
 -   **output_dir**: Directory to place the generated code
 -   **target_language**: Target language for the generated code
-    -   cpp; c; js; ts; py
+    -   cpp / c / js / ts / py
 
 ## Raw Message format
 
 The message structure is composed of a 6-byte header, followed by a variable-length payload. The payload length can range from 0 to 244 bytes, allowing for flexible data encapsulation. Fields within the payload are tightly packed, with no intervening spaces, to maximize message efficiency and minimize overhead.
 
 | Byte Index | Field    | Size (Bytes) | Description                                       |
 | ---------- | -------- | ------------ | ------------------------------------------------- |
@@ -57,14 +57,15 @@
 | 6-249      | payload  | 244          | Actual data payload                               |
 
 ### Code representation
 
 -   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c++/generated_code/lions.hpp)
 -   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/lions.js)
 -   [TypeScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/ts/generated_code/lions.ts)
+-   [Python](https://github.com/ItsNotSoftware/lions/blob/main/examples/python/generated_code/lions.py)
 
 ## Defining Messages
 
 LIONS uses `.lmsg.yaml` files to define message specifications for IoT networks. Each file can contain multiple message definitions that are used by the LIONS compiler to generate C++ code for message handling.
 
 ### Structure of Message Files
 
@@ -154,22 +155,28 @@
     - Transforms a generic, raw-form message (`LMsg`) into the structured format of the class. This conversion facilitates easier manipulation and interpretation of the message contents within the application.
 
 3. **Encode Method**
     - Converts the structured message back into its raw binary form (`LMsg`) for transmission. This method ensures that the message is properly packaged with its header and payload according to the protocol specifications before being sent over the network.
 
 ---
 
+Generated message classes examples:
+
 -   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c%2B%2B/generated_code/my_messages_lmsg.hpp)
 -   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/my_messages_lmsg.js)
 -   [TypeScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/ts/generated_code/my_messages_lmsg.ts)
+-   [Python](https://github.com/ItsNotSoftware/lions/blob/main/examples/python/generated_code/my_messages_lmsg.py)
 
 ## Examples
 
-[Examples](https://github.com/ItsNotSoftware/lions/tree/main/examples)
+-   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples)
+-   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js)
+-   [TypeScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/ts)
+-   [Python](https://github.com/ItsNotSoftware/lions/blob/main/examples/python)
 
 ## Target Language Support
 
 -   [x] C++
 -   [x] JavaScript
 -   [x] TypeScript
+-   [x] Python
 -   [ ] C
--   [ ] Python
```

### Comparing `lions-1.3.2/lions/errors.py` & `lions-1.4.0/lions/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,9 +95,9 @@
         super().__init__(Fore.RED + message)
 
 
 class InvalidTargetLanguageError(Exception):
     """Exception raised when the target language is invalid."""
 
     def __init__(self, target_language):
-        message = f'Error: Invalid target language "{target_language}". Supported languages: "cpp", "js".'
+        message = f'Error: Invalid target language "{target_language}".'
         super().__init__(Fore.RED + message)
```

### Comparing `lions-1.3.2/lions/lmsg.py` & `lions-1.4.0/lions/lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.3.2/lions/main.py` & `lions-1.4.0/lions/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,28 @@
 License:
     Copyright (c) 2024 Diogo Ferreira. All rights reserved.
     This code is licensed under the MIT License.
 """
 
 import sys
 import colorama
-from lions.cpp_gen.cpp_generator import CppGenerator
-from lions.ts_gen.ts_generator import TsGenerator
+from lions.code_generation.cpp.cpp_generator import CppGenerator
+from lions.code_generation.js.js_generator import JsGenerator
+from lions.code_generation.ts.ts_generator import TsGenerator
+from lions.code_generation.python.python_generator import PythonGenerator
 from lions.yaml_parser import YamlParser
 from colorama import Fore, Style
-from lions.js_gen.js_generator import JsGenerator
 from lions.errors import InvalidTargetLanguageError
 
 
+def invalid_language(_):
+    """Raise an InvalidTargetLanguageError if the target language is invalid."""
+    raise InvalidTargetLanguageError(sys.argv[3])
+
+
 def print_title():
     """Function to print title of the program in ASCII art"""
 
     print(Fore.GREEN)
 
     print(
         """
@@ -60,36 +66,34 @@
         # targert language help
         print(
             """
     Target Language:
         cpp - C++
         js - JavaScript
         ts - TypeScript
+        py - Python
         """
         )
 
         sys.exit(1)
 
     msg_files_dir = sys.argv[1]
     output_dir = sys.argv[2]
 
     print_title()
 
     # Initialize the parser and generator objects
     parser = YamlParser(msg_files_dir)
-    code_generator = None
 
-    # Check the target language and initialize the corresponding code generator
-    if sys.argv[3] == "c++" or sys.argv[3] == "cpp":
-        code_generator = CppGenerator(output_dir)
-    elif sys.argv[3] == "js":
-        code_generator = JsGenerator(output_dir)
-    elif sys.argv[3] == "ts":
-        code_generator = TsGenerator(output_dir)
-    else:
-        raise InvalidTargetLanguageError(sys.argv[3])
+    # Initialize the code generator based on the target language
+    code_generator = {
+        "cpp": CppGenerator,
+        "js": JsGenerator,
+        "ts": TsGenerator,
+        "py": PythonGenerator,
+    }.get(sys.argv[3], invalid_language)(output_dir)
 
     # Parse the message files and generate the corresponding C++ files
     for filename, msgs in parser.parse_file():
         code_generator.generate_msg_files(filename, msgs)
 
     print_success_message()
```

### Comparing `lions-1.3.2/lions/yaml_parser.py` & `lions-1.4.0/lions/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `lions-1.3.2/lions.egg-info/PKG-INFO` & `lions-1.4.0/lions.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.3.2
+Version: 1.4.0
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -58,15 +58,15 @@
 ## Usage
 
     $ lions <msg_files_dir> <output_dir> <target_language>
 
 -   **msg_files_dir**: Directory containing your .lmsg.yaml files
 -   **output_dir**: Directory to place the generated code
 -   **target_language**: Target language for the generated code
-    -   cpp; c; js; ts; py
+    -   cpp / c / js / ts / py
 
 ## Raw Message format
 
 The message structure is composed of a 6-byte header, followed by a variable-length payload. The payload length can range from 0 to 244 bytes, allowing for flexible data encapsulation. Fields within the payload are tightly packed, with no intervening spaces, to maximize message efficiency and minimize overhead.
 
 | Byte Index | Field    | Size (Bytes) | Description                                       |
 | ---------- | -------- | ------------ | ------------------------------------------------- |
@@ -78,14 +78,15 @@
 | 6-249      | payload  | 244          | Actual data payload                               |
 
 ### Code representation
 
 -   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c++/generated_code/lions.hpp)
 -   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/lions.js)
 -   [TypeScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/ts/generated_code/lions.ts)
+-   [Python](https://github.com/ItsNotSoftware/lions/blob/main/examples/python/generated_code/lions.py)
 
 ## Defining Messages
 
 LIONS uses `.lmsg.yaml` files to define message specifications for IoT networks. Each file can contain multiple message definitions that are used by the LIONS compiler to generate C++ code for message handling.
 
 ### Structure of Message Files
 
@@ -175,22 +176,28 @@
     - Transforms a generic, raw-form message (`LMsg`) into the structured format of the class. This conversion facilitates easier manipulation and interpretation of the message contents within the application.
 
 3. **Encode Method**
     - Converts the structured message back into its raw binary form (`LMsg`) for transmission. This method ensures that the message is properly packaged with its header and payload according to the protocol specifications before being sent over the network.
 
 ---
 
+Generated message classes examples:
+
 -   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples/c%2B%2B/generated_code/my_messages_lmsg.hpp)
 -   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js/generated_code/my_messages_lmsg.js)
 -   [TypeScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/ts/generated_code/my_messages_lmsg.ts)
+-   [Python](https://github.com/ItsNotSoftware/lions/blob/main/examples/python/generated_code/my_messages_lmsg.py)
 
 ## Examples
 
-[Examples](https://github.com/ItsNotSoftware/lions/tree/main/examples)
+-   [C++](https://github.com/ItsNotSoftware/lions/blob/main/examples)
+-   [JavaScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/js)
+-   [TypeScript](https://github.com/ItsNotSoftware/lions/blob/main/examples/ts)
+-   [Python](https://github.com/ItsNotSoftware/lions/blob/main/examples/python)
 
 ## Target Language Support
 
 -   [x] C++
 -   [x] JavaScript
 -   [x] TypeScript
+-   [x] Python
 -   [ ] C
--   [ ] Python
```

### Comparing `lions-1.3.2/setup.py` & `lions-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lions",
-    version="1.3.2",
+    version="1.4.0",
     author="Diogo Ferreira",
     author_email="itsnotsoftware@gmail.com",
     description="LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={"lions": ["cpp_gen/templates/*.jinja"]},
     url="https://github.com/ItsNotSoftware/lions",
```

### Comparing `lions-1.3.2/tests/test_cpp_gen.py` & `lions-1.4.0/tests/test_cpp_gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from lions.cpp_gen.cpp_generator import CppGenerator
+from lions.code_generation.cpp.cpp_generator import CppGenerator
 from lions.yaml_parser import YamlParser
 from lions.lmsg import _used_ids, _used_names
 import functools
 import os
 
 
 def clear_directory(directory_path):
```

### Comparing `lions-1.3.2/tests/test_js_gen copy.py` & `lions-1.4.0/tests/test_js_gen copy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from lions.js_gen.js_generator import JsGenerator
+from lions.code_generation.js.js_generator import JsGenerator
 from lions.yaml_parser import YamlParser
 from lions.lmsg import _used_ids, _used_names
 import functools
 import os
 
 
 def clear_directory(directory_path):
```

### Comparing `lions-1.3.2/tests/test_lmsg.py` & `lions-1.4.0/tests/test_lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.3.2/tests/test_ts_gen.py` & `lions-1.4.0/tests/test_ts_gen.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from lions.ts_gen.ts_generator import TsGenerator
+from lions.code_generation.ts.ts_generator import TsGenerator
 from lions.yaml_parser import YamlParser
 from lions.lmsg import _used_ids, _used_names
 import functools
 import os
 
 
 def clear_directory(directory_path):
```

### Comparing `lions-1.3.2/tests/test_yaml_parser.py` & `lions-1.4.0/tests/test_yaml_parser.py`

 * *Files identical despite different names*

