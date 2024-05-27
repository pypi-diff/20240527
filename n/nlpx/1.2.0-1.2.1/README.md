# Comparing `tmp/nlpx-1.2.0.tar.gz` & `tmp/nlpx-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.2.0.tar", last modified: Mon May 27 12:29:10 2024, max compression
+gzip compressed data, was "nlpx-1.2.1.tar", last modified: Mon May 27 13:23:47 2024, max compression
```

## Comparing `nlpx-1.2.0.tar` & `nlpx-1.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 12:29:10.086108 nlpx-1.2.0/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-27 12:29:10.084980 nlpx-1.2.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.0/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 12:29:10.049449 nlpx-1.2.0/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.0/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 12:29:10.059811 nlpx-1.2.0/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)      122 2024-05-25 21:19:20.000000 nlpx-1.2.0/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     5872 2024-05-27 12:29:03.000000 nlpx-1.2.0/nlpx/llm/_model_wrapper.py
--rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.2.0/nlpx/llm/_tokenize_vec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 12:29:10.064313 nlpx-1.2.0/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.0/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.2.0/nlpx/models/_text_cnn.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 12:29:10.078443 nlpx-1.2.0/nlpx/text_token/
--rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.0/nlpx/text_token/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.0/nlpx/text_token/_tokenizer.py
--rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.0/nlpx/text_token/_utils.py
--rw-r--r--   0 summy      (501) staff       (20)     3915 2024-05-27 12:03:24.000000 nlpx-1.2.0/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 12:29:10.056255 nlpx-1.2.0/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-27 12:29:09.000000 nlpx-1.2.0/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      412 2024-05-27 12:29:09.000000 nlpx-1.2.0/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-27 12:29:09.000000 nlpx-1.2.0/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 06:16:47.000000 nlpx-1.2.0/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-27 12:29:09.000000 nlpx-1.2.0/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-27 12:29:10.087740 nlpx-1.2.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-27 12:20:33.000000 nlpx-1.2.0/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 12:29:10.082674 nlpx-1.2.0/test/
--rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.2.0/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:23:47.653709 nlpx-1.2.1/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-27 13:23:47.652850 nlpx-1.2.1/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.1/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:23:47.626460 nlpx-1.2.1/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.1/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:23:47.633610 nlpx-1.2.1/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      122 2024-05-25 21:19:20.000000 nlpx-1.2.1/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     5886 2024-05-27 13:23:10.000000 nlpx-1.2.1/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.2.1/nlpx/llm/_tokenize_vec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:23:47.637465 nlpx-1.2.1/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.1/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.2.1/nlpx/models/_text_cnn.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:23:47.646211 nlpx-1.2.1/nlpx/text_token/
+-rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.1/nlpx/text_token/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.1/nlpx/text_token/_tokenizer.py
+-rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.1/nlpx/text_token/_utils.py
+-rw-r--r--   0 summy      (501) staff       (20)     3901 2024-05-27 13:08:01.000000 nlpx-1.2.1/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:23:47.630632 nlpx-1.2.1/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-27 13:23:47.000000 nlpx-1.2.1/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      412 2024-05-27 13:23:47.000000 nlpx-1.2.1/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-27 13:23:47.000000 nlpx-1.2.1/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 06:16:47.000000 nlpx-1.2.1/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-27 13:23:47.000000 nlpx-1.2.1/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-27 13:23:47.654141 nlpx-1.2.1/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-27 13:23:44.000000 nlpx-1.2.1/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 13:23:47.650649 nlpx-1.2.1/test/
+-rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.2.1/test/test.py
```

### Comparing `nlpx-1.2.0/PKG-INFO` & `nlpx-1.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.0
+Version: 1.2.1
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.0/nlpx/llm/_model_wrapper.py` & `nlpx-1.2.1/nlpx/llm/_model_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 	def predict_classes(self, X: torch.FloatTensor):
 		assert self.classes is not None, 'classes must be specified'
 		pred = self.predict(X)
 		return [self.classes[i] for i in pred.detach().numpy().ravel()]
 
 	def predict_proba(self, X: torch.FloatTensor):
 		logits = self.logits(X)
-		result = F.softmax(logits).max(1)
+		result = F.softmax(logits, dim=1).max(1)
 		return result.indices, result.values
 
 	def predict_classes_proba(self, X: torch.FloatTensor):
 		assert self.classes is not None, 'classes must be specified'
 		logits = self.logits(X)
 		result = F.softmax(logits).max(1)
 		return [self.classes[i] for i in result.indices.detach().numpy().ravel()], result.values
@@ -108,15 +108,15 @@
 		logits = self.logits(texts, max_length)
 		result = F.softmax(logits).max(1)
 		return result.indices, result.values
 
 	def predict_classes_proba(self, texts: List[str], max_length: int = 0):
 		assert self.classes is not None, 'classes must be specified'
 		logits = self.logits(texts, max_length)
-		result = F.softmax(logits).max(1)
+		result = F.softmax(logits, dim=1).max(1)
 		return [self.classes[i] for i in result.indices.detach().numpy().ravel()], result.values
 
 	def logits(self, texts: List[str], max_length: int = 0):
 		X = self.get_features(texts, max_length)
 		return super().logits(X)
 
 	def evaluate(self, texts: List[str], y: Union[torch.LongTensor, List, np.ndarray], batch_size=16, num_workers=0,
```

### Comparing `nlpx-1.2.0/nlpx/llm/_tokenize_vec.py` & `nlpx-1.2.1/nlpx/llm/_tokenize_vec.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.0/nlpx/models/_text_cnn.py` & `nlpx-1.2.1/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.0/nlpx/text_token/_tokenizer.py` & `nlpx-1.2.1/nlpx/text_token/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.0/nlpx/text_token/_utils.py` & `nlpx-1.2.1/nlpx/text_token/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.0/nlpx/training.py` & `nlpx-1.2.1/nlpx/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 				correct += (logits.argmax(1) == y).sum().item()
 				total += len(y)
 
 			val_loss, val_acc = evaluate(self.model, self.eval_loader, self.device)
 			print('epoch-{}/{}\tlr: {:.6f}, train_loss: {:.4f}, train_acc: {:.4f}, val_loss: {:.4f}, val_acc: {:.4f}'.format(
 				epoch + 1, self.max_iter, self.optimizer.param_groups[0]['lr'], losses / total, correct / total, val_loss, val_acc
 			))
-			if epoch > 5 and val_acc > best_acc:
+			if val_acc > best_acc:
 				best_acc = val_acc
 				best_model = self.model
 
 			if val_acc >= best_acc:  # val_acc提升
 				cnt = 0
 
 			if last_acc == val_acc:  # val_acc不在变化
```

### Comparing `nlpx-1.2.0/nlpx.egg-info/PKG-INFO` & `nlpx-1.2.1/nlpx.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.0
+Version: 1.2.1
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.0/setup.py` & `nlpx-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm', 'nlpx.text_token'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.0',
+    version='1.2.1',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

