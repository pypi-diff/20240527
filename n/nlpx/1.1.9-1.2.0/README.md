# Comparing `tmp/nlpx-1.1.9.tar.gz` & `tmp/nlpx-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.1.9.tar", last modified: Mon May 27 05:12:56 2024, max compression
+gzip compressed data, was "nlpx-1.2.0.tar", last modified: Mon May 27 12:29:10 2024, max compression
```

## Comparing `nlpx-1.1.9.tar` & `nlpx-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 05:12:56.595769 nlpx-1.1.9/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-27 05:12:56.595128 nlpx-1.1.9/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.9/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 05:12:56.563015 nlpx-1.1.9/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.9/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 05:12:56.577631 nlpx-1.1.9/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)      122 2024-05-25 21:19:20.000000 nlpx-1.1.9/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     5777 2024-05-27 05:12:39.000000 nlpx-1.1.9/nlpx/llm/_model_wrapper.py
--rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.1.9/nlpx/llm/_tokenize_vec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 05:12:56.581997 nlpx-1.1.9/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.1.9/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.1.9/nlpx/models/_text_cnn.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 05:12:56.589070 nlpx-1.1.9/nlpx/text_token/
--rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.1.9/nlpx/text_token/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.1.9/nlpx/text_token/_tokenizer.py
--rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.1.9/nlpx/text_token/_utils.py
--rw-r--r--   0 summy      (501) staff       (20)     3916 2024-05-25 22:26:52.000000 nlpx-1.1.9/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 05:12:56.572406 nlpx-1.1.9/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-27 05:12:56.000000 nlpx-1.1.9/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      412 2024-05-27 05:12:56.000000 nlpx-1.1.9/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-27 05:12:56.000000 nlpx-1.1.9/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 06:16:47.000000 nlpx-1.1.9/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-27 05:12:56.000000 nlpx-1.1.9/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-27 05:12:56.595991 nlpx-1.1.9/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-27 05:12:39.000000 nlpx-1.1.9/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 05:12:56.592769 nlpx-1.1.9/test/
--rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.1.9/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 12:29:10.086108 nlpx-1.2.0/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-27 12:29:10.084980 nlpx-1.2.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.0/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 12:29:10.049449 nlpx-1.2.0/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.0/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 12:29:10.059811 nlpx-1.2.0/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      122 2024-05-25 21:19:20.000000 nlpx-1.2.0/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     5872 2024-05-27 12:29:03.000000 nlpx-1.2.0/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.2.0/nlpx/llm/_tokenize_vec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 12:29:10.064313 nlpx-1.2.0/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.0/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.2.0/nlpx/models/_text_cnn.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 12:29:10.078443 nlpx-1.2.0/nlpx/text_token/
+-rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.0/nlpx/text_token/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.0/nlpx/text_token/_tokenizer.py
+-rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.0/nlpx/text_token/_utils.py
+-rw-r--r--   0 summy      (501) staff       (20)     3915 2024-05-27 12:03:24.000000 nlpx-1.2.0/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 12:29:10.056255 nlpx-1.2.0/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-27 12:29:09.000000 nlpx-1.2.0/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      412 2024-05-27 12:29:09.000000 nlpx-1.2.0/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-27 12:29:09.000000 nlpx-1.2.0/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 06:16:47.000000 nlpx-1.2.0/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-27 12:29:09.000000 nlpx-1.2.0/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-27 12:29:10.087740 nlpx-1.2.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-27 12:20:33.000000 nlpx-1.2.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 12:29:10.082674 nlpx-1.2.0/test/
+-rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.2.0/test/test.py
```

### Comparing `nlpx-1.1.9/PKG-INFO` & `nlpx-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.9
+Version: 1.2.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.9/nlpx/llm/_model_wrapper.py` & `nlpx-1.2.0/nlpx/llm/_model_wrapper.py`

 * *Files 26% similar despite different names*

```diff
@@ -59,18 +59,18 @@
 
 	def evaluate(self, eval_set: Dataset, batch_size=16, num_workers=0, max_length: int = 0,  collate_fn=None):
 		eval_loader = DataLoader(dataset=eval_set, batch_size=batch_size,
 								 num_workers=num_workers, collate_fn=collate_fn)
 		_, acc = evaluate(self.model, eval_loader, self.device)
 		return acc
 
-	def save(self, model_path: Union[str, Path]):
+	def save(self, model_path: Union[str, Path] = './best_model.pt'):
 		torch.save(model_path, self.model)
 
-	def load(self, model_path: Union[str, Path]):
+	def load(self, model_path: Union[str, Path] = './best_model.pt'):
 		self.model = torch.load(model_path, map_location=self.device)
 
 
 class SimpleModelWrapper(ModelWrapper):
 
 	def __init__(self, tokenize_vec, model_path: Union[str, Path] = None, classes: List[str] = None,
 					device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
@@ -92,42 +92,40 @@
 								 batch_size, eval_batch_size,
 								 num_workers, num_eval_workers,
 								 early_stopping_rounds,
 								 self.device)
 		self.model = trainer.train()
 
 	def predict(self, texts: List[str], max_length: int = 0):
-		max_length = self.get_max_length(texts, max_length)
-		X = self.get_vec(texts, max_length=max_length)
-		return super().predict(X)
+		logits = self.logits(texts, max_length)
+		return logits.argmax(1)
 
 	def predict_classes(self, texts: List[str], max_length: int = 0):
 		assert self.classes is not None, 'classes must be specified'
 		pred = self.predict(texts, max_length)
 		return [self.classes[i] for i in pred.detach().numpy().ravel()]
 	
 	def predict_proba(self, texts: List[str], max_length: int = 0):
-		max_length = self.get_max_length(texts, max_length)
-		X = self.get_vec(texts, max_length=max_length)
-		return super().predict_proba(X)
+		logits = self.logits(texts, max_length)
+		result = F.softmax(logits).max(1)
+		return result.indices, result.values
 
 	def predict_classes_proba(self, texts: List[str], max_length: int = 0):
-		max_length = self.get_max_length(texts, max_length)
-		X = self.get_vec(texts, max_length=max_length)
-		return super().predict_classes_proba(X)
+		assert self.classes is not None, 'classes must be specified'
+		logits = self.logits(texts, max_length)
+		result = F.softmax(logits).max(1)
+		return [self.classes[i] for i in result.indices.detach().numpy().ravel()], result.values
 
 	def logits(self, texts: List[str], max_length: int = 0):
-		max_length = self.get_max_length(texts, max_length)
-		X = self.get_vec(texts, max_length=max_length)
+		X = self.get_features(texts, max_length)
 		return super().logits(X)
 
 	def evaluate(self, texts: List[str], y: Union[torch.LongTensor, List, np.ndarray], batch_size=16, num_workers=0,
 				 max_length: int = 0, collate_fn=None):
-		max_length = self.get_max_length(texts, max_length)
-		X = self.get_vec(texts, max_length=max_length)
+		X = self.get_features(texts, max_length)
 		if isinstance(y, List) or isinstance(y, np.ndarray):
 			y = torch.tensor(y, dtype=torch.long)
 		eval_set = TensorDataset(X, y)
 		return super().evaluate(eval_set, batch_size=batch_size, num_workers=num_workers, collate_fn=collate_fn)
 
 	@staticmethod
 	def get_max_length(texts: List[str], max_length: int = 0) -> int:
@@ -136,7 +134,11 @@
 		return get_texts_max_length(texts, cut_type='char')
 
 	def get_vec(self, texts: List[str], max_length: int):
 		return self.tokenize_vec.parallel_encode_plus(texts, max_length=max_length, padding='max_length',
 														truncation=True, add_special_tokens=True,
 														return_token_type_ids=True,return_attention_mask=True,
 														return_tensors='pt')
+
+	def get_features(self, texts: List[str], max_length: int = 0):
+		max_length = self.get_max_length(texts, max_length)
+		return self.get_vec(texts, max_length=max_length)
```

### Comparing `nlpx-1.1.9/nlpx/llm/_tokenize_vec.py` & `nlpx-1.2.0/nlpx/llm/_tokenize_vec.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.9/nlpx/models/_text_cnn.py` & `nlpx-1.2.0/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.9/nlpx/text_token/_tokenizer.py` & `nlpx-1.2.0/nlpx/text_token/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.9/nlpx/text_token/_utils.py` & `nlpx-1.2.0/nlpx/text_token/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.9/nlpx/training.py` & `nlpx-1.2.0/nlpx/training.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 			if last_acc == val_acc:  # val_acc不在变化
 				cnt2 += 1
 			else:
 				cnt2 = 0
 
 			last_acc = val_acc
 			cnt += 1
-			if epoch >= min(5, self.early_stopping_rounds) and max(cnt, cnt2) >= self.early_stopping_rounds:  # x次epoch的val_acc不提升或x次epoch的val_acc不变化
+			if epoch >= min(5, self.early_stopping_rounds) and max(cnt, cnt2) > self.early_stopping_rounds:  # x次epoch的val_acc不提升或x次epoch的val_acc不变化
 				print("Early stopping at epoch-{}/{}".format(epoch + 1, self.max_iter))
 				break
 
 		return best_model
 
 
 class SimpleTrainer(Trainer):
```

### Comparing `nlpx-1.1.9/nlpx.egg-info/PKG-INFO` & `nlpx-1.2.0/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.9
+Version: 1.2.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.9/setup.py` & `nlpx-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm', 'nlpx.text_token'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.1.9',
+    version='1.2.0',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

