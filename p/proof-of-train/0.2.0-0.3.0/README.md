# Comparing `tmp/proof_of_train-0.2.0.tar.gz` & `tmp/proof_of_train-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proof_of_train-0.2.0.tar", max compression
+gzip compressed data, was "proof_of_train-0.3.0.tar", max compression
```

## Comparing `proof_of_train-0.2.0.tar` & `proof_of_train-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3621 2024-05-23 09:19:26.093380 proof_of_train-0.2.0/README.md
--rw-r--r--   0        0        0      127 2024-05-27 02:01:43.425888 proof_of_train-0.2.0/proof_of_train/__init__.py
--rw-r--r--   0        0        0     1460 2024-05-22 11:02:00.944128 proof_of_train-0.2.0/proof_of_train/abi.json
--rw-r--r--   0        0        0     2649 2024-05-22 11:02:17.998383 proof_of_train-0.2.0/proof_of_train/model_metadata.py
--rw-r--r--   0        0        0     4418 2024-05-23 09:19:26.090913 proof_of_train-0.2.0/proof_of_train/proof_of_train.py
--rw-r--r--   0        0        0     1724 2024-05-27 02:01:43.422373 proof_of_train-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4069 1970-01-01 00:00:00.000000 proof_of_train-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4183 2024-05-27 02:33:29.423977 proof_of_train-0.3.0/README.md
+-rw-r--r--   0        0        0      128 2024-05-27 02:33:38.486255 proof_of_train-0.3.0/proof_of_train/__init__.py
+-rw-r--r--   0        0        0     1460 2024-05-22 11:02:00.944128 proof_of_train-0.3.0/proof_of_train/abi.json
+-rw-r--r--   0        0        0     2957 2024-05-27 02:33:38.510609 proof_of_train-0.3.0/proof_of_train/model_metadata.py
+-rw-r--r--   0        0        0     4418 2024-05-23 09:19:26.090913 proof_of_train-0.3.0/proof_of_train/proof_of_train.py
+-rw-r--r--   0        0        0     1724 2024-05-27 02:34:27.141041 proof_of_train-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4631 1970-01-01 00:00:00.000000 proof_of_train-0.3.0/PKG-INFO
```

### Comparing `proof_of_train-0.2.0/README.md` & `proof_of_train-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -41,18 +41,23 @@
 - `wait_for_confirmation` (optional): Whether to wait for the transaction to be confirmed (default: False).
 
 ```python
 from proof_of_train import ModelMetadata
 
 model_id = "your-model-id"
 metadata = ModelMetadata(
-    name="Model Name",
-    version="1.0.0",
-    description="Model description",
-    # Add other metadata fields as needed
+    model_name="Model Name",
+    model_md5="d4c2e8a2b3cb1a9c0a7b7f4c5a9a3b2e",
+    model_url="https://huggingface.co/bert-base-uncased",
+    dataset_url="https://huggingface.co/datasets/glue",
+    training_params={"epochs": 3, "batch_size": 32},
+    training_date="2024-05-27",
+    model_version="1.0",
+    author="Hugging Face",
+    description="BERT base model, uncased version, trained on the GLUE dataset."
 )
 
 tx_hash = pot.submit_proof(model_id, metadata, wait_for_confirmation=False)
 print(f"Transaction hash: {tx_hash}")
 ```
 
 If `wait_for_confirmation` is set to `False` (which is the default), the `submit_proof` method will return the transaction hash. You can use this hash to track the status of the transaction later.
@@ -70,26 +75,31 @@
 
 ```python
 model_id = "your-model-id"
 metadata = pot.get_proof(model_id)
 
 if metadata:
     print(f"Model ID: {model_id}")
-    print(f"Name: {metadata.name}")
-    print(f"Version: {metadata.version}")
+    print(f"Model Name: {metadata.model_name}")
+    print(f"Model MD5: {metadata.model_md5}")
+    print(f"Model URL: {metadata.model_url}")
+    print(f"Dataset URL: {metadata.dataset_url}")
+    print(f"Training Params: {metadata.training_params}")
+    print(f"Training Date: {metadata.training_date}")
+    print(f"Model Version: {metadata.model_version}")
+    print(f"Author: {metadata.author}")
     print(f"Description: {metadata.description}")
-    # Access other metadata fields as needed
 else:
     print(f"Model with ID {model_id} not found.")
 ```
 
 ## Error Handling
 
 The SDK handles common errors that may occur during the interaction with the blockchain network. If an error occurs, an appropriate exception will be raised with a descriptive error message.
 
 ## License
 
 This SDK is released under the [MIT License](LICENSE).
 
 ## Contributing
 
-Contributions to the ProofOfTrain Python SDK are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/RSS3-Network/pot).
+Contributions to the ProofOfTrain Python SDK are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/RSS3-Network/pot).
```

### Comparing `proof_of_train-0.2.0/proof_of_train/abi.json` & `proof_of_train-0.3.0/proof_of_train/abi.json`

 * *Files identical despite different names*

### Comparing `proof_of_train-0.2.0/proof_of_train/model_metadata.py` & `proof_of_train-0.3.0/proof_of_train/model_metadata.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,58 @@
 class ModelMetadata:
     def __init__(
         self,
+        model_name,
         model_md5,
-        dataset_url,
         model_url,
+        dataset_url,
         training_params=None,
         training_date=None,
         model_version=None,
         author=None,
         description=None,
     ):
         """
         Initialize the model metadata.
 
+        :param model_name: The name of the model.
         :param model_md5: The MD5 hash value of the model, used to uniquely identify the model.
-        :param dataset_url: The URL of the dataset used for training the model.
         :param model_url: The URL where the trained model is stored.
+        :param dataset_url: The URL of the dataset used for training the model.
         :param training_params: The parameters used for training the model, such as number of epochs, batch size, etc.
         :param training_date: The date when the model was trained.
         :param model_version: The version of the model, useful for tracking model iterations.
         :param author: The author or entity responsible for training the model.
         :param description: A brief description of the model, including its purpose and any other relevant information.
+        :param protocol_version: The protocol version of the metadata structure.
         """
         self.model_md5 = model_md5
-        self.dataset_url = dataset_url
+        self.model_name = model_name
         self.model_url = model_url
+        self.dataset_url = dataset_url
         self.training_params = training_params
         self.training_date = training_date
         self.model_version = model_version
         self.author = author
         self.description = description
-        self.version = "1.0.0"
+        self.protocol_version = ("1.0.0",)
 
     @classmethod
     def from_dict(cls, data):
         """
         Create a ModelMetadata instance from a dictionary.
 
         :param data: A dictionary containing the model metadata.
         :return: A ModelMetadata instance.
         """
         return cls(
             model_md5=data.get("model_md5"),
-            dataset_url=data.get("dataset_url"),
+            model_name=data.get("model_name"),
             model_url=data.get("model_url"),
+            dataset_url=data.get("dataset_url"),
             training_params=data.get("training_params"),
             training_date=data.get("training_date"),
             model_version=data.get("model_version"),
             author=data.get("author"),
             description=data.get("description"),
         )
 
@@ -55,16 +60,17 @@
         """
         Convert the ModelMetadata instance to a dictionary.
 
         :return: A dictionary representation of the ModelMetadata instance.
         """
         return {
             "model_md5": self.model_md5,
-            "dataset_url": self.dataset_url,
+            "model_name": self.model_name,
             "model_url": self.model_url,
+            "dataset_url": self.dataset_url,
             "training_params": self.training_params,
             "training_date": self.training_date,
             "model_version": self.model_version,
             "author": self.author,
             "description": self.description,
-            "version": self.version,
+            "protocol_version": self.protocol_version,
         }
```

### Comparing `proof_of_train-0.2.0/proof_of_train/proof_of_train.py` & `proof_of_train-0.3.0/proof_of_train/proof_of_train.py`

 * *Files identical despite different names*

### Comparing `proof_of_train-0.2.0/pyproject.toml` & `proof_of_train-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proof-of-train"
-version = "0.2.0"
+version = "0.3.0"
 description = "Proof of Train SDK for submitting and verifying model training metadata on blockchain."
 authors = ["Thomas <wxy_000000@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 web3 = "^6.19.0"
```

### Comparing `proof_of_train-0.2.0/PKG-INFO` & `proof_of_train-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proof-of-train
-Version: 0.2.0
+Version: 0.3.0
 Summary: Proof of Train SDK for submitting and verifying model training metadata on blockchain.
 Author: Thomas
 Author-email: wxy_000000@qq.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pytest (>=8.2.1,<9.0.0)
@@ -54,18 +54,23 @@
 - `wait_for_confirmation` (optional): Whether to wait for the transaction to be confirmed (default: False).
 
 ```python
 from proof_of_train import ModelMetadata
 
 model_id = "your-model-id"
 metadata = ModelMetadata(
-    name="Model Name",
-    version="1.0.0",
-    description="Model description",
-    # Add other metadata fields as needed
+    model_name="Model Name",
+    model_md5="d4c2e8a2b3cb1a9c0a7b7f4c5a9a3b2e",
+    model_url="https://huggingface.co/bert-base-uncased",
+    dataset_url="https://huggingface.co/datasets/glue",
+    training_params={"epochs": 3, "batch_size": 32},
+    training_date="2024-05-27",
+    model_version="1.0",
+    author="Hugging Face",
+    description="BERT base model, uncased version, trained on the GLUE dataset."
 )
 
 tx_hash = pot.submit_proof(model_id, metadata, wait_for_confirmation=False)
 print(f"Transaction hash: {tx_hash}")
 ```
 
 If `wait_for_confirmation` is set to `False` (which is the default), the `submit_proof` method will return the transaction hash. You can use this hash to track the status of the transaction later.
@@ -83,18 +88,23 @@
 
 ```python
 model_id = "your-model-id"
 metadata = pot.get_proof(model_id)
 
 if metadata:
     print(f"Model ID: {model_id}")
-    print(f"Name: {metadata.name}")
-    print(f"Version: {metadata.version}")
+    print(f"Model Name: {metadata.model_name}")
+    print(f"Model MD5: {metadata.model_md5}")
+    print(f"Model URL: {metadata.model_url}")
+    print(f"Dataset URL: {metadata.dataset_url}")
+    print(f"Training Params: {metadata.training_params}")
+    print(f"Training Date: {metadata.training_date}")
+    print(f"Model Version: {metadata.model_version}")
+    print(f"Author: {metadata.author}")
     print(f"Description: {metadata.description}")
-    # Access other metadata fields as needed
 else:
     print(f"Model with ID {model_id} not found.")
 ```
 
 ## Error Handling
 
 The SDK handles common errors that may occur during the interaction with the blockchain network. If an error occurs, an appropriate exception will be raised with a descriptive error message.
@@ -102,7 +112,8 @@
 ## License
 
 This SDK is released under the [MIT License](LICENSE).
 
 ## Contributing
 
 Contributions to the ProofOfTrain Python SDK are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/RSS3-Network/pot).
+
```

