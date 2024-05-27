# Comparing `tmp/multi_modal_tokenizers-0.0.1.tar.gz` & `tmp/multi_modal_tokenizers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_modal_tokenizers-0.0.1.tar", last modified: Fri May 24 09:09:17 2024, max compression
+gzip compressed data, was "multi_modal_tokenizers-0.0.2.tar", last modified: Mon May 27 07:35:33 2024, max compression
```

## Comparing `multi_modal_tokenizers-0.0.1.tar` & `multi_modal_tokenizers-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 09:09:17.382206 multi_modal_tokenizers-0.0.1/
--rw-rw-rw-   0        0        0     3632 2024-05-24 09:09:17.382206 multi_modal_tokenizers-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2489 2024-05-24 08:47:21.000000 multi_modal_tokenizers-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 09:09:17.364206 multi_modal_tokenizers-0.0.1/multi_modal_tokenizers/
--rw-rw-rw-   0        0        0       89 2024-05-24 07:44:21.000000 multi_modal_tokenizers-0.0.1/multi_modal_tokenizers/__init__.py
--rw-rw-rw-   0        0        0     7217 2024-05-24 07:43:54.000000 multi_modal_tokenizers-0.0.1/multi_modal_tokenizers/tokenizer.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:09:17.381206 multi_modal_tokenizers-0.0.1/multi_modal_tokenizers.egg-info/
--rw-rw-rw-   0        0        0     3632 2024-05-24 09:09:17.000000 multi_modal_tokenizers-0.0.1/multi_modal_tokenizers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-05-24 09:09:17.000000 multi_modal_tokenizers-0.0.1/multi_modal_tokenizers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 09:09:17.000000 multi_modal_tokenizers-0.0.1/multi_modal_tokenizers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-24 09:09:17.000000 multi_modal_tokenizers-0.0.1/multi_modal_tokenizers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-24 09:09:17.000000 multi_modal_tokenizers-0.0.1/multi_modal_tokenizers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 09:09:17.382206 multi_modal_tokenizers-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      771 2024-05-24 07:59:33.000000 multi_modal_tokenizers-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:35:33.204651 multi_modal_tokenizers-0.0.2/
+-rw-rw-rw-   0        0        0     3782 2024-05-27 07:35:33.203651 multi_modal_tokenizers-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2591 2024-05-27 03:08:37.000000 multi_modal_tokenizers-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 07:35:33.170651 multi_modal_tokenizers-0.0.2/multi_modal_tokenizers/
+-rw-rw-rw-   0        0        0      192 2024-05-26 03:57:42.000000 multi_modal_tokenizers-0.0.2/multi_modal_tokenizers/__init__.py
+-rw-rw-rw-   0        0        0      608 2024-05-26 02:20:52.000000 multi_modal_tokenizers-0.0.2/multi_modal_tokenizers/image_processing.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:35:33.201652 multi_modal_tokenizers-0.0.2/multi_modal_tokenizers/tokenizers/
+-rw-rw-rw-   0        0        0      161 2024-05-26 02:25:47.000000 multi_modal_tokenizers-0.0.2/multi_modal_tokenizers/tokenizers/__init__.py
+-rw-rw-rw-   0        0        0      716 2024-05-27 07:08:23.000000 multi_modal_tokenizers-0.0.2/multi_modal_tokenizers/tokenizers/base_tokenizers.py
+-rw-rw-rw-   0        0        0     1714 2024-05-27 07:09:17.000000 multi_modal_tokenizers-0.0.2/multi_modal_tokenizers/tokenizers/dalle_tokenizer.py
+-rw-rw-rw-   0        0        0     4098 2024-05-27 07:26:23.000000 multi_modal_tokenizers-0.0.2/multi_modal_tokenizers/tokenizers/mixed_modal_tokenizer.py
+-rw-rw-rw-   0        0        0      543 2024-05-26 02:20:41.000000 multi_modal_tokenizers-0.0.2/multi_modal_tokenizers/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:35:33.192650 multi_modal_tokenizers-0.0.2/multi_modal_tokenizers.egg-info/
+-rw-rw-rw-   0        0        0     3782 2024-05-27 07:35:33.000000 multi_modal_tokenizers-0.0.2/multi_modal_tokenizers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2024-05-27 07:35:33.000000 multi_modal_tokenizers-0.0.2/multi_modal_tokenizers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 07:35:33.000000 multi_modal_tokenizers-0.0.2/multi_modal_tokenizers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-27 07:35:33.000000 multi_modal_tokenizers-0.0.2/multi_modal_tokenizers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-27 07:35:33.000000 multi_modal_tokenizers-0.0.2/multi_modal_tokenizers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 07:35:33.204651 multi_modal_tokenizers-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      771 2024-05-27 07:32:04.000000 multi_modal_tokenizers-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:35:33.202651 multi_modal_tokenizers-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-27 02:57:15.000000 multi_modal_tokenizers-0.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     2123 2024-05-27 07:28:42.000000 multi_modal_tokenizers-0.0.2/tests/test_tokenizer.py
```

### Comparing `multi_modal_tokenizers-0.0.1/PKG-INFO` & `multi_modal_tokenizers-0.0.2/multi_modal_tokenizers.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
-Name: multi_modal_tokenizers
-Version: 0.0.1
+Name: multi-modal-tokenizers
+Version: 0.0.2
 Summary: Multi-modal tokenizers for more than just text.
 Home-page: https://github.com/anothy1/multi-modal-tokenizers
 Author: Anthony Nguyen
 License: UNKNOWN
 Description: 
         
         # Multi-Modal Tokenizers
         
-        Multi-modal tokenizers for more than just text. This package provides tools for tokenizing and decoding images and mixed-modal inputs (text and images) using DALL-E and other models.
+        Multi-modal tokenizers for more than just text. This package provides tools for tokenizing and decoding images and mixed-modal inputs (text and images) using encoders like [DALL-E's VAE](https://github.com/openai/DALL-E).
         
         ## Installation
         
         To install the package, clone the repository and use pip to install it:
         
         ```sh
         git clone https://github.com/anothy1/multi-modal-tokenizers
         pip install ./multi-modal-tokenizers
         ```
         
+        Or from PyPI:
+        
+        ```sh
+        pip install multi-modal-tokenizers
+        ```
+        
         ## Usage
         
         ### Example: Using DalleTokenizer
         
         Below is an example script demonstrating how to use the `DalleTokenizer` to encode and decode images.
         
         ```python
@@ -71,15 +77,15 @@
         mixed_tokenizer = MixedModalTokenizer(
             text_tokenizer=text_tokenizer,
             image_tokenizer=image_tokenizer,
             device="cpu"
         )
         
         # Example usage
-        text = "This is an example with <new_image> in the middle."
+        text = "This is an example with <image> in the middle."
         img_path = "path/to/your/image.jpg"
         image = Image.open(img_path)
         
         # Encode the text and image
         encoded = mixed_tokenizer.encode(text=text, images=[image])
         print("Encoded mixed-modal tokens:", encoded)
```

### Comparing `multi_modal_tokenizers-0.0.1/README.md` & `multi_modal_tokenizers-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 
 
 # Multi-Modal Tokenizers
 
-Multi-modal tokenizers for more than just text. This package provides tools for tokenizing and decoding images and mixed-modal inputs (text and images) using DALL-E and other models.
+Multi-modal tokenizers for more than just text. This package provides tools for tokenizing and decoding images and mixed-modal inputs (text and images) using encoders like [DALL-E's VAE](https://github.com/openai/DALL-E).
 
 ## Installation
 
 To install the package, clone the repository and use pip to install it:
 
 ```sh
 git clone https://github.com/anothy1/multi-modal-tokenizers
 pip install ./multi-modal-tokenizers
 ```
 
+Or from PyPI:
+
+```sh
+pip install multi-modal-tokenizers
+```
+
 ## Usage
 
 ### Example: Using DalleTokenizer
 
 Below is an example script demonstrating how to use the `DalleTokenizer` to encode and decode images.
 
 ```python
@@ -64,15 +70,15 @@
 mixed_tokenizer = MixedModalTokenizer(
     text_tokenizer=text_tokenizer,
     image_tokenizer=image_tokenizer,
     device="cpu"
 )
 
 # Example usage
-text = "This is an example with <new_image> in the middle."
+text = "This is an example with <image> in the middle."
 img_path = "path/to/your/image.jpg"
 image = Image.open(img_path)
 
 # Encode the text and image
 encoded = mixed_tokenizer.encode(text=text, images=[image])
 print("Encoded mixed-modal tokens:", encoded)
```

### Comparing `multi_modal_tokenizers-0.0.1/multi_modal_tokenizers.egg-info/PKG-INFO` & `multi_modal_tokenizers-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
-Name: multi-modal-tokenizers
-Version: 0.0.1
+Name: multi_modal_tokenizers
+Version: 0.0.2
 Summary: Multi-modal tokenizers for more than just text.
 Home-page: https://github.com/anothy1/multi-modal-tokenizers
 Author: Anthony Nguyen
 License: UNKNOWN
 Description: 
         
         # Multi-Modal Tokenizers
         
-        Multi-modal tokenizers for more than just text. This package provides tools for tokenizing and decoding images and mixed-modal inputs (text and images) using DALL-E and other models.
+        Multi-modal tokenizers for more than just text. This package provides tools for tokenizing and decoding images and mixed-modal inputs (text and images) using encoders like [DALL-E's VAE](https://github.com/openai/DALL-E).
         
         ## Installation
         
         To install the package, clone the repository and use pip to install it:
         
         ```sh
         git clone https://github.com/anothy1/multi-modal-tokenizers
         pip install ./multi-modal-tokenizers
         ```
         
+        Or from PyPI:
+        
+        ```sh
+        pip install multi-modal-tokenizers
+        ```
+        
         ## Usage
         
         ### Example: Using DalleTokenizer
         
         Below is an example script demonstrating how to use the `DalleTokenizer` to encode and decode images.
         
         ```python
@@ -71,15 +77,15 @@
         mixed_tokenizer = MixedModalTokenizer(
             text_tokenizer=text_tokenizer,
             image_tokenizer=image_tokenizer,
             device="cpu"
         )
         
         # Example usage
-        text = "This is an example with <new_image> in the middle."
+        text = "This is an example with <image> in the middle."
         img_path = "path/to/your/image.jpg"
         image = Image.open(img_path)
         
         # Encode the text and image
         encoded = mixed_tokenizer.encode(text=text, images=[image])
         print("Encoded mixed-modal tokens:", encoded)
```

### Comparing `multi_modal_tokenizers-0.0.1/setup.py` & `multi_modal_tokenizers-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="multi_modal_tokenizers",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(),
     install_requires=[
         "torch",
         "torchvision",
         "Pillow",
         "dall_e",
         "huggingface_hub",
```

