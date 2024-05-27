# Comparing `tmp/mia_vgg-0.0.7.tar.gz` & `tmp/mia_vgg-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia_vgg-0.0.7.tar", last modified: Fri May 24 11:15:25 2024, max compression
+gzip compressed data, was "mia_vgg-0.0.8.tar", last modified: Mon May 27 08:41:05 2024, max compression
```

## Comparing `mia_vgg-0.0.7.tar` & `mia_vgg-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 11:15:25.615135 mia_vgg-0.0.7/
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-24 11:15:25.615135 mia_vgg-0.0.7/PKG-INFO
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      541 2024-05-24 11:14:17.000000 mia_vgg-0.0.7/pyproject.toml
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       38 2024-05-24 11:15:25.615135 mia_vgg-0.0.7/setup.cfg
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 11:15:25.615135 mia_vgg-0.0.7/src/
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 11:15:25.615135 mia_vgg-0.0.7/src/mia_vgg/
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-22 12:56:18.000000 mia_vgg-0.0.7/src/mia_vgg/__init__.py
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)     2228 2024-05-24 11:14:23.000000 mia_vgg-0.0.7/src/mia_vgg/train_target.py
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 11:15:25.615135 mia_vgg-0.0.7/src/mia_vgg.egg-info/
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-24 11:15:25.000000 mia_vgg-0.0.7/src/mia_vgg.egg-info/PKG-INFO
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      240 2024-05-24 11:15:25.000000 mia_vgg-0.0.7/src/mia_vgg.egg-info/SOURCES.txt
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        1 2024-05-24 11:15:25.000000 mia_vgg-0.0.7/src/mia_vgg.egg-info/dependency_links.txt
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       29 2024-05-24 11:15:25.000000 mia_vgg-0.0.7/src/mia_vgg.egg-info/requires.txt
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        8 2024-05-24 11:15:25.000000 mia_vgg-0.0.7/src/mia_vgg.egg-info/top_level.txt
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-27 08:41:05.803085 mia_vgg-0.0.8/
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-27 08:41:05.803085 mia_vgg-0.0.8/PKG-INFO
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      541 2024-05-27 08:41:01.000000 mia_vgg-0.0.8/pyproject.toml
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       38 2024-05-27 08:41:05.803085 mia_vgg-0.0.8/setup.cfg
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-27 08:41:05.803085 mia_vgg-0.0.8/src/
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-27 08:41:05.803085 mia_vgg-0.0.8/src/mia_vgg/
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-22 12:56:18.000000 mia_vgg-0.0.8/src/mia_vgg/__init__.py
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)     2714 2024-05-27 08:40:35.000000 mia_vgg-0.0.8/src/mia_vgg/train_target.py
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-27 08:41:05.803085 mia_vgg-0.0.8/src/mia_vgg.egg-info/
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-27 08:41:05.000000 mia_vgg-0.0.8/src/mia_vgg.egg-info/PKG-INFO
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      240 2024-05-27 08:41:05.000000 mia_vgg-0.0.8/src/mia_vgg.egg-info/SOURCES.txt
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        1 2024-05-27 08:41:05.000000 mia_vgg-0.0.8/src/mia_vgg.egg-info/dependency_links.txt
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       29 2024-05-27 08:41:05.000000 mia_vgg-0.0.8/src/mia_vgg.egg-info/requires.txt
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        8 2024-05-27 08:41:05.000000 mia_vgg-0.0.8/src/mia_vgg.egg-info/top_level.txt
```

### Comparing `mia_vgg-0.0.7/PKG-INFO` & `mia_vgg-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia_vgg
-Version: 0.0.7
+Version: 0.0.8
 Summary: MIA on VGG dataset using pytorch
 Author-email: Jan Aalmoes <jan.aalmoes@protonmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mia_vgg-0.0.7/pyproject.toml` & `mia_vgg-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mia_vgg"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Jan Aalmoes", email="jan.aalmoes@protonmail.com" },
 ]
 description = "MIA on VGG dataset using pytorch"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mia_vgg-0.0.7/src/mia_vgg/train_target.py` & `mia_vgg-0.0.8/src/mia_vgg/train_target.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,18 +58,31 @@
                 running_loss = 0
 
             if i>50:
                 break
 
     with torch.no_grad():
         correct = 0
+        values = {"yhat":[], "y":[]}
         for data in testloader:
             x,y = data
             x = x.to(device)
             y = y.to(device)
             soft = model(x)
             _, yhat = torch.max(soft, 1)
-            correct += (yhat == y).sum().item()
-        print(correct/len(testloader))
+            values["y"] += y.cpu().detach().numpy()
+            values["yhat"] += yhat.cpu().detach().numpy()
+        y = values["y"]
+        yhat = values["yhat"]
+    metric["accuracy"] = np.mean(y==yhat)
+    metric["balanced_accuracy"] = np.mean([np.mean(yhat[y==yy]==yy) for yy in np.unique(y)])
+
+    path = Path("result")
+    os.makedirs(path, exist_ok=True)
+    with open(Path(path, "metric.pickle"), 'rb') as f:
+        pickle.dump(metric, f)
+    with open(Path(path, "values.pickle"), 'rb') as f:
+        pickle.dump(values, f)
+
         
 if __name__=="__main__":
     train()
```

### Comparing `mia_vgg-0.0.7/src/mia_vgg.egg-info/PKG-INFO` & `mia_vgg-0.0.8/src/mia_vgg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia_vgg
-Version: 0.0.7
+Version: 0.0.8
 Summary: MIA on VGG dataset using pytorch
 Author-email: Jan Aalmoes <jan.aalmoes@protonmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

