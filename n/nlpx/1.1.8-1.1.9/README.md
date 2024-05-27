# Comparing `tmp/nlpx-1.1.8.tar.gz` & `tmp/nlpx-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.1.8.tar", last modified: Sun May 26 06:16:47 2024, max compression
+gzip compressed data, was "nlpx-1.1.9.tar", last modified: Mon May 27 05:12:56 2024, max compression
```

## Comparing `nlpx-1.1.8.tar` & `nlpx-1.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 06:16:47.641691 nlpx-1.1.8/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-26 06:16:47.641021 nlpx-1.1.8/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.8/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 06:16:47.610599 nlpx-1.1.8/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.8/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 06:16:47.620885 nlpx-1.1.8/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)      122 2024-05-25 21:19:20.000000 nlpx-1.1.8/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     5102 2024-05-26 05:21:03.000000 nlpx-1.1.8/nlpx/llm/_model_wrapper.py
--rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.1.8/nlpx/llm/_tokenize_vec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 06:16:47.627246 nlpx-1.1.8/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.1.8/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.1.8/nlpx/models/_text_cnn.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 06:16:47.636893 nlpx-1.1.8/nlpx/text_token/
--rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.1.8/nlpx/text_token/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.1.8/nlpx/text_token/_tokenizer.py
--rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.1.8/nlpx/text_token/_utils.py
--rw-r--r--   0 summy      (501) staff       (20)     3916 2024-05-25 22:26:52.000000 nlpx-1.1.8/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 06:16:47.615407 nlpx-1.1.8/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-26 06:16:47.000000 nlpx-1.1.8/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      412 2024-05-26 06:16:47.000000 nlpx-1.1.8/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 06:16:47.000000 nlpx-1.1.8/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 06:16:47.000000 nlpx-1.1.8/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-26 06:16:47.000000 nlpx-1.1.8/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-26 06:16:47.642005 nlpx-1.1.8/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-26 06:16:42.000000 nlpx-1.1.8/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 06:16:47.639640 nlpx-1.1.8/test/
--rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.1.8/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 05:12:56.595769 nlpx-1.1.9/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-27 05:12:56.595128 nlpx-1.1.9/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.9/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 05:12:56.563015 nlpx-1.1.9/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.9/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 05:12:56.577631 nlpx-1.1.9/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      122 2024-05-25 21:19:20.000000 nlpx-1.1.9/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     5777 2024-05-27 05:12:39.000000 nlpx-1.1.9/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.1.9/nlpx/llm/_tokenize_vec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 05:12:56.581997 nlpx-1.1.9/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.1.9/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.1.9/nlpx/models/_text_cnn.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 05:12:56.589070 nlpx-1.1.9/nlpx/text_token/
+-rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.1.9/nlpx/text_token/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.1.9/nlpx/text_token/_tokenizer.py
+-rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.1.9/nlpx/text_token/_utils.py
+-rw-r--r--   0 summy      (501) staff       (20)     3916 2024-05-25 22:26:52.000000 nlpx-1.1.9/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 05:12:56.572406 nlpx-1.1.9/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-27 05:12:56.000000 nlpx-1.1.9/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      412 2024-05-27 05:12:56.000000 nlpx-1.1.9/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-27 05:12:56.000000 nlpx-1.1.9/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 06:16:47.000000 nlpx-1.1.9/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-27 05:12:56.000000 nlpx-1.1.9/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-27 05:12:56.595991 nlpx-1.1.9/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-27 05:12:39.000000 nlpx-1.1.9/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 05:12:56.592769 nlpx-1.1.9/test/
+-rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.1.9/test/test.py
```

### Comparing `nlpx-1.1.8/PKG-INFO` & `nlpx-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.8
+Version: 1.1.9
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.8/nlpx/llm/_model_wrapper.py` & `nlpx-1.1.9/nlpx/llm/_model_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,28 +28,34 @@
 						  batch_size, eval_batch_size,
 						  num_workers, num_eval_workers,
 						  early_stopping_rounds,  # 早停，等10轮决策，评价指标不在变化，停止
 						  self.device)
 		self.model = trainer.train()
 
 	def predict(self, X: torch.FloatTensor):
-		logits = self._predict(X)
+		logits = self.logits(X)
 		return logits.argmax(1)
 
 	def predict_classes(self, X: torch.FloatTensor):
 		assert self.classes is not None, 'classes must be specified'
 		pred = self.predict(X)
 		return [self.classes[i] for i in pred.detach().numpy().ravel()]
 
 	def predict_proba(self, X: torch.FloatTensor):
-		logits = self._predict(X)
+		logits = self.logits(X)
 		result = F.softmax(logits).max(1)
 		return result.indices, result.values
 
-	def _predict(self, X: torch.FloatTensor):
+	def predict_classes_proba(self, X: torch.FloatTensor):
+		assert self.classes is not None, 'classes must be specified'
+		logits = self.logits(X)
+		result = F.softmax(logits).max(1)
+		return [self.classes[i] for i in result.indices.detach().numpy().ravel()], result.values
+
+	def logits(self, X: torch.FloatTensor):
 		self.model.eval()
 		with torch.no_grad():
 			logits = self.model(X)
 		return logits
 
 	def evaluate(self, eval_set: Dataset, batch_size=16, num_workers=0, max_length: int = 0,  collate_fn=None):
 		eval_loader = DataLoader(dataset=eval_set, batch_size=batch_size,
@@ -100,14 +106,24 @@
 		return [self.classes[i] for i in pred.detach().numpy().ravel()]
 	
 	def predict_proba(self, texts: List[str], max_length: int = 0):
 		max_length = self.get_max_length(texts, max_length)
 		X = self.get_vec(texts, max_length=max_length)
 		return super().predict_proba(X)
 
+	def predict_classes_proba(self, texts: List[str], max_length: int = 0):
+		max_length = self.get_max_length(texts, max_length)
+		X = self.get_vec(texts, max_length=max_length)
+		return super().predict_classes_proba(X)
+
+	def logits(self, texts: List[str], max_length: int = 0):
+		max_length = self.get_max_length(texts, max_length)
+		X = self.get_vec(texts, max_length=max_length)
+		return super().logits(X)
+
 	def evaluate(self, texts: List[str], y: Union[torch.LongTensor, List, np.ndarray], batch_size=16, num_workers=0,
 				 max_length: int = 0, collate_fn=None):
 		max_length = self.get_max_length(texts, max_length)
 		X = self.get_vec(texts, max_length=max_length)
 		if isinstance(y, List) or isinstance(y, np.ndarray):
 			y = torch.tensor(y, dtype=torch.long)
 		eval_set = TensorDataset(X, y)
```

### Comparing `nlpx-1.1.8/nlpx/llm/_tokenize_vec.py` & `nlpx-1.1.9/nlpx/llm/_tokenize_vec.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.8/nlpx/models/_text_cnn.py` & `nlpx-1.1.9/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.8/nlpx/text_token/_tokenizer.py` & `nlpx-1.1.9/nlpx/text_token/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.8/nlpx/text_token/_utils.py` & `nlpx-1.1.9/nlpx/text_token/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.8/nlpx/training.py` & `nlpx-1.1.9/nlpx/training.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.8/nlpx.egg-info/PKG-INFO` & `nlpx-1.1.9/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.8
+Version: 1.1.9
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.8/setup.py` & `nlpx-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm', 'nlpx.text_token'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.1.8',
+    version='1.1.9',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

