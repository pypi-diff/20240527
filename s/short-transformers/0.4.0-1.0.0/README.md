# Comparing `tmp/short_transformers-0.4.0.tar.gz` & `tmp/short_transformers-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "short_transformers-0.4.0.tar", max compression
+gzip compressed data, was "short_transformers-1.0.0.tar", max compression
```

## Comparing `short_transformers-0.4.0.tar` & `short_transformers-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,16 @@
--rw-r--r--   0        0        0     5348 2024-05-06 09:45:19.335021 short_transformers-0.4.0/README.md
--rw-r--r--   0        0        0      379 2024-05-06 10:01:42.709668 short_transformers-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       98 2024-05-04 22:49:29.887096 short_transformers-0.4.0/short_transformers/__init__.py
--rw-r--r--   0        0        0     1137 2024-05-06 10:01:04.173722 short_transformers-0.4.0/short_transformers/dist.py
--rw-r--r--   0        0        0     6977 2024-05-06 09:56:23.130108 short_transformers-0.4.0/short_transformers/short_transformer.py
--rw-r--r--   0        0        0      281 2024-05-05 10:42:13.996656 short_transformers-0.4.0/short_transformers/utils/__init__.py
--rw-r--r--   0        0        0      529 2024-05-04 22:49:29.887096 short_transformers-0.4.0/short_transformers/utils/log.py
--rw-r--r--   0        0        0      965 2024-05-05 10:54:41.243629 short_transformers-0.4.0/short_transformers/utils/plot.py
--rw-r--r--   0        0        0     1200 2024-05-05 10:51:18.167907 short_transformers-0.4.0/short_transformers/utils/utils.py
--rw-r--r--   0        0        0     5960 1970-01-01 00:00:00.000000 short_transformers-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11134 2024-05-27 16:26:44.036476 short_transformers-1.0.0/README.md
+-rw-r--r--   0        0        0      379 2024-05-27 16:19:58.989926 short_transformers-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-05-17 13:09:37.090461 short_transformers-1.0.0/short_transformers/__init__.py
+-rw-r--r--   0        0        0     3628 2024-05-26 06:21:24.920284 short_transformers-1.0.0/short_transformers/dist.py
+-rw-r--r--   0        0        0     2175 2024-05-21 12:12:24.599648 short_transformers-1.0.0/short_transformers/model_factory/diff.txt
+-rw-r--r--   0        0        0     1825 2024-05-22 19:57:26.669605 short_transformers-1.0.0/short_transformers/model_factory/duplicate_layer.py
+-rw-r--r--   0        0        0     1695 2024-05-18 19:14:38.779683 short_transformers-1.0.0/short_transformers/model_factory/remove_and_duplicate.py
+-rw-r--r--   0        0        0     2324 2024-05-18 21:28:27.639503 short_transformers-1.0.0/short_transformers/model_factory/remove_and_duplicate_with_merging.py
+-rw-r--r--   0        0        0     4194 2024-05-25 15:00:15.311521 short_transformers-1.0.0/short_transformers/model_factory/remove_by_merging.py
+-rw-r--r--   0        0        0     5301 2024-05-18 10:18:20.262256 short_transformers-1.0.0/short_transformers/model_factory/replace_layer_and_cut.py
+-rw-r--r--   0        0        0     7500 2024-05-27 14:38:30.470717 short_transformers-1.0.0/short_transformers/short_transformer.py
+-rw-r--r--   0        0        0      325 2024-05-27 09:44:28.243900 short_transformers-1.0.0/short_transformers/utils/__init__.py
+-rw-r--r--   0        0        0      529 2024-05-17 13:09:37.090461 short_transformers-1.0.0/short_transformers/utils/log.py
+-rw-r--r--   0        0        0     1519 2024-05-27 14:41:17.195291 short_transformers-1.0.0/short_transformers/utils/plot.py
+-rw-r--r--   0        0        0     1200 2024-05-17 13:09:37.090461 short_transformers-1.0.0/short_transformers/utils/utils.py
+-rw-r--r--   0        0        0    11746 1970-01-01 00:00:00.000000 short_transformers-1.0.0/PKG-INFO
```

### Comparing `short_transformers-0.4.0/short_transformers/short_transformer.py` & `short_transformers-1.0.0/short_transformers/short_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,21 +98,27 @@
         return decorator
 
     @staticmethod
     def set_metric(model, criterion_callable):
         model.distance = criterion_callable
 
     @staticmethod
+    def group_batch(batch):
+        return {k: [v] for k, v in batch.items()}
+
+    @staticmethod
     def analyse_layers(
         model,
         dataset,
         tokenizer=None,
+        use_chat_template=False,
         key: str = "content",
         limit: int = 1,
         max_length: int = 1000,
+        batch_size: int = 1
     ) -> None:
         if tokenizer is None:
             logger.debug(
                 "Tokenizer not provided, will load tokenizer from config._name_or_path"
             )
             try:
                 tokenizer = AutoTokenizer.from_pretrained(model.config._name_or_path)
@@ -121,27 +127,34 @@
                     f"Loading the tokenizer failed wwth error: {e}.\nUse analyse_layers(... tokenizer=...) to manually set the tokenizer."
                 )
                 raise RuntimeError
 
         logger.debug(f"Running inference on {limit} samples.")
 
         model.model.eval()
+
+        if batch_size > 1:
+            dataset = dataset.map(ShortTransformer.group_batch, batched=True, batch_size=batch_size)
+
         with torch.no_grad():
             count = 0
             for d in tqdm(dataset):
                 content = d[key]
-                inputs = tokenizer(
-                    content,
-                    return_tensors="pt",
-                    padding=False,
-                    truncation=True,
-                    max_length=max_length,
-                ).to(model.device)
+                if use_chat_template:
+                    inputs = tokenizer.apply_chat_template(content, tokenize=True, add_generation_prompt=False)
+                else:
+                    inputs = tokenizer(
+                        content,
+                        return_tensors="pt",
+                        padding=True if batch_size>1 else False,
+                        truncation=True,
+                        max_length=max_length,
+                    ).to(model.device)
                 model(**inputs)
-                count += 1
+                count += batch_size
                 if count >= limit:
                     break
         result = model.memory.result
         model.clear_memory()
         return result
 
     @staticmethod
```

### Comparing `short_transformers-0.4.0/short_transformers/utils/log.py` & `short_transformers-1.0.0/short_transformers/utils/log.py`

 * *Files identical despite different names*

### Comparing `short_transformers-0.4.0/short_transformers/utils/plot.py` & `short_transformers-1.0.0/short_transformers/utils/plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,51 @@
 import matplotlib.pylab as plt
 import numpy as np
 import seaborn as sns
+import matplotlib
 
-
-def draw_diagram(results, output_file_path, title=None):
+def draw_diagram(results, output_file_path, title=None, normalized=True):
     plt.clf()
 
     mask = np.zeros_like(results)
     mask[np.triu_indices_from(mask, k=1)] = True
     mask = np.flip(mask, axis=0)
 
     # @TODO make row-wise normalization optional
     # rescale scores to 0-1 for each cut_layers value
-    masked_results = np.ma.masked_array(results, mask)
-    max_dist = np.ma.max(masked_results, axis=1)[:, np.newaxis]
-    min_dist = np.ma.min(masked_results, axis=1)[:, np.newaxis]
+    
+    if normalized:
+        masked_results = np.ma.masked_array(results, mask)
+        max_dist = np.ma.max(masked_results, axis=1)[:, np.newaxis]
+        min_dist = np.ma.min(masked_results, axis=1)[:, np.newaxis]
 
-    results = (results - min_dist) / (max_dist - min_dist)
+        results = (results - min_dist) / (max_dist - min_dist)
 
     ax = sns.heatmap(results, linewidth=0.5, mask=mask, cmap="viridis_r")
     ax.invert_yaxis()
     ax.set_xticklabels(ax.get_xticklabels(), ha="left")
     ax.set_yticklabels(ax.get_yticklabels(), va="bottom")
 
     plt.xlabel("Layer number, l")
     plt.ylabel("Block size, n")
 
     if title:
         ax.set_title(title)
 
     plt.savefig(output_file_path)
+
+
+def draw_layers_heatmap(results, metric_name, title, output_path, block_size=0, cmap=matplotlib.cm.viridis_r):
+
+    # @TODO make row-wise normalization?
+    if block_size:
+        data = results[0, :-block_size]
+    else:
+        data = results[0, :]
+    data = np.asarray(data).reshape(data.shape[0],1)
+
+    fig = plt.figure(figsize = (5,5))
+    ax = sns.heatmap(data, annot=False, cmap=cmap)
+
+    ax.set_xlabel(metric_name)
+    ax.set_title(title)
+    plt.savefig(output_path)
```

### Comparing `short_transformers-0.4.0/short_transformers/utils/utils.py` & `short_transformers-1.0.0/short_transformers/utils/utils.py`

 * *Files identical despite different names*

