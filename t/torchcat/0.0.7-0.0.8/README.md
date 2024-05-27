# Comparing `tmp/torchcat-0.0.7.tar.gz` & `tmp/torchcat-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchcat-0.0.7.tar", last modified: Sat May 25 14:07:55 2024, max compression
+gzip compressed data, was "torchcat-0.0.8.tar", last modified: Mon May 27 07:58:04 2024, max compression
```

## Comparing `torchcat-0.0.7.tar` & `torchcat-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 14:07:55.946649 torchcat-0.0.7/
--rw-rw-rw-   0        0        0    35823 2024-05-25 05:07:21.000000 torchcat-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2960 2024-05-25 14:07:55.944477 torchcat-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2613 2024-05-25 14:07:16.000000 torchcat-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-25 14:07:55.946649 torchcat-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      711 2024-05-25 14:07:51.000000 torchcat-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-25 14:07:55.939025 torchcat-0.0.7/torchcat/
--rw-rw-rw-   0        0        0     4654 2024-05-25 03:58:51.000000 torchcat-0.0.7/torchcat/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 14:07:55.944477 torchcat-0.0.7/torchcat.egg-info/
--rw-rw-rw-   0        0        0     2960 2024-05-25 14:07:55.000000 torchcat-0.0.7/torchcat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2024-05-25 14:07:55.000000 torchcat-0.0.7/torchcat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 14:07:55.000000 torchcat-0.0.7/torchcat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-25 14:07:55.000000 torchcat-0.0.7/torchcat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-25 14:07:55.000000 torchcat-0.0.7/torchcat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 07:58:04.718958 torchcat-0.0.8/
+-rw-rw-rw-   0        0        0    35823 2024-05-25 05:07:21.000000 torchcat-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3133 2024-05-27 07:58:04.718958 torchcat-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2715 2024-05-25 14:13:32.000000 torchcat-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-27 07:58:04.718958 torchcat-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      751 2024-05-27 07:57:09.000000 torchcat-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:58:04.715451 torchcat-0.0.8/torchcat/
+-rw-rw-rw-   0        0        0       69 2024-05-27 07:56:57.000000 torchcat-0.0.8/torchcat/__init__.py
+-rw-rw-rw-   0        0        0     4750 2024-05-26 15:12:53.000000 torchcat-0.0.8/torchcat/cat.py
+-rw-rw-rw-   0        0        0      680 2024-05-26 14:41:00.000000 torchcat-0.0.8/torchcat/datasets.py
+-rw-rw-rw-   0        0        0      305 2024-05-25 15:14:30.000000 torchcat-0.0.8/torchcat/metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-27 07:58:04.717959 torchcat-0.0.8/torchcat.egg-info/
+-rw-rw-rw-   0        0        0     3133 2024-05-27 07:58:04.000000 torchcat-0.0.8/torchcat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-05-27 07:58:04.000000 torchcat-0.0.8/torchcat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 07:58:04.000000 torchcat-0.0.8/torchcat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-27 07:58:04.000000 torchcat-0.0.8/torchcat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 07:58:04.000000 torchcat-0.0.8/torchcat.egg-info/top_level.txt
```

### Comparing `torchcat-0.0.7/LICENSE` & `torchcat-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `torchcat-0.0.7/PKG-INFO` & `torchcat-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: torchcat
-Version: 0.0.7
-Summary: This is a test of the setup
-Home-page: https://gitee.com/kkkaiyu/torchcat
-Author: KaiYu
-Author-email: 2971934557@qq.com
-License: GPL-3.0
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: torchsummary
-
 # TorchCat 🐱
 
 # 简介
 
 TorchCat 是用于封装 PyTorch 模型的工具
 
 提供以下功能：
@@ -78,15 +64,15 @@
 | --------- | ------------------- |
 | train_set | 训练集              |
 | epochs    | 训练轮次            |
 | valid_set | 验证集（默认 None） |
 
 ## 验证模型
 
-使用 `net.valid(valid_set, show=True, train=False)`，能够验证模型
+使用 `net.valid(valid_set, show=True, train=False)`，能够验证模型在给定验证集上的性能，包括损失值、准确率。验证后模型将切换为推理模式
 
 | 参数      | 说明                                           |
 | --------- | ---------------------------------------------- |
 | valid_set | 验证集                                         |
 | show      | 是否输出验证集损失值、准确率（默认 True）      |
 | train     | 验证后，模型是否且切换为训练模式（默认 False） |
```

### Comparing `torchcat-0.0.7/README.md` & `torchcat-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: torchcat
+Version: 0.0.8
+Summary: TorchCat 是用于封装 PyTorch 模型的工具
+Home-page: https://gitee.com/kkkaiyu/torchcat
+Author: KaiYu
+Author-email: 2971934557@qq.com
+License: GPL-3.0
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch
+Requires-Dist: torchvision
+Requires-Dist: torchsummary
+Requires-Dist: numpy
+
 # TorchCat 🐱
 
 # 简介
 
 TorchCat 是用于封装 PyTorch 模型的工具
 
 提供以下功能：
@@ -64,15 +80,15 @@
 | --------- | ------------------- |
 | train_set | 训练集              |
 | epochs    | 训练轮次            |
 | valid_set | 验证集（默认 None） |
 
 ## 验证模型
 
-使用 `net.valid(valid_set, show=True, train=False)`，能够验证模型
+使用 `net.valid(valid_set, show=True, train=False)`，能够验证模型在给定验证集上的性能，包括损失值、准确率。验证后模型将切换为推理模式
 
 | 参数      | 说明                                           |
 | --------- | ---------------------------------------------- |
 | valid_set | 验证集                                         |
 | show      | 是否输出验证集损失值、准确率（默认 True）      |
 | train     | 验证后，模型是否且切换为训练模式（默认 False） |
```

### Comparing `torchcat-0.0.7/torchcat/__init__.py` & `torchcat-0.0.8/torchcat/cat.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
 from torchsummary import summary
 
+from . import metrics
+
 
 class Cat:
     def __init__(self, model, loss_fn=None, optimizer=None):
         '''
         封装模型
 
         Parameters
@@ -34,40 +36,39 @@
         valid_set: 验证集
 
         Returns
         --------
         log: 训练日志
         '''
         self.model.train()
-        for epoch in range(1, epochs+1):
-            acc_temp = []       # 储存一个 epoch 的准确率、损失值
-            loss_temp = []
+        for epoch in range(1, epochs + 1):
+            acc_temp, loss_temp = [], []  # 储存一个 epoch 的准确率、损失值
             for x, y in train_set:
                 if self.GPU_FLAG != 'cpu':
                     x, y = x.cuda(), y.cuda()
                 self.optimizer.zero_grad()
                 pred = self.model(x)
                 loss = self.loss_fn(pred, y)
                 loss_temp.append(loss.item())
                 loss.backward()
                 self.optimizer.step()
 
-                acc_temp.append((pred.argmax(-1) == y).float().mean().item())
+                acc_temp.append(metrics.accuracy(pred.argmax(-1).cpu().numpy(), y.argmax(-1).cpu().numpy()))
 
             train_acc, train_loss = np.mean(acc_temp), np.mean(loss_temp)
             # 记录、输出训练日志
             self.log['train acc'].append(train_acc)
             self.log['train loss'].append(train_loss)
 
-            output = f'Epoch {epoch}/{epochs} Train-Loss: {train_loss:.6f} Train-Accuracy: {train_acc:.6f}'
+            output = f'Epoch {epoch}/{epochs} Train - <Loss: {train_loss:.6f} Accuracy: {train_acc:.6f}>'
             if valid_set is not None:
                 valid_loss, valid_acc = self.valid(valid_set, show=False, train=True)
                 self.log['valid acc'].append(valid_acc)
                 self.log['valid loss'].append(valid_loss)
-                output += f' Valid-Loss: {valid_loss:.6f} Valid-Accuracy: {valid_acc:.6f}'
+                output += f' Valid - <Loss: {valid_loss:.6f} Accuracy: {valid_acc:.6f}>'
 
             print(output)
         return self.log
 
     def valid(self, valid_set, show=True, train=False):
         '''
         验证模型
@@ -79,27 +80,28 @@
         train : 最后是否切换为训练模式
 
         Returns
         --------
         loss, acc : 验证集上的的损失值、准确率
         '''
         self.model.eval()
-        acc_temp = []       # 储存一个 epoch 的准确率、损失值
-        loss_temp = []
+        acc_temp, loss_temp = [], []  # 储存一个 epoch 的准确率、损失值
         for x, y in valid_set:
             if self.GPU_FLAG != 'cpu':
                 x, y = x.cuda(), y.cuda()
             pred = self.model(x)
             loss_temp.append(self.loss_fn(pred, y).item())  # 计算验证集 loss
-            acc_temp.append((pred.argmax(-1) == y).float().mean().item())  # 计算验证集 accuracy
+            acc_temp.append(
+                metrics.accuracy(pred.argmax(-1).cpu().numpy(), y.argmax(-1).cpu().numpy()))  # 计算验证集 accuracy
         if train:
             self.model.train()
         if show:
             print(f'Loss: {np.mean(loss_temp):.6f}')
             print(f'Accuracy: {np.mean(acc_temp):.6f}')
+            return None
         return np.mean(loss_temp), np.mean(acc_temp)
 
     def summary(self, *input_size):
         '''
         查看架构
 
         Parameters
```

### Comparing `torchcat-0.0.7/torchcat.egg-info/PKG-INFO` & `torchcat-0.0.8/torchcat.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: torchcat
-Version: 0.0.7
-Summary: This is a test of the setup
+Version: 0.0.8
+Summary: TorchCat 是用于封装 PyTorch 模型的工具
 Home-page: https://gitee.com/kkkaiyu/torchcat
 Author: KaiYu
 Author-email: 2971934557@qq.com
 License: GPL-3.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
+Requires-Dist: torch
+Requires-Dist: torchvision
 Requires-Dist: torchsummary
+Requires-Dist: numpy
 
 # TorchCat 🐱
 
 # 简介
 
 TorchCat 是用于封装 PyTorch 模型的工具
 
@@ -78,15 +80,15 @@
 | --------- | ------------------- |
 | train_set | 训练集              |
 | epochs    | 训练轮次            |
 | valid_set | 验证集（默认 None） |
 
 ## 验证模型
 
-使用 `net.valid(valid_set, show=True, train=False)`，能够验证模型
+使用 `net.valid(valid_set, show=True, train=False)`，能够验证模型在给定验证集上的性能，包括损失值、准确率。验证后模型将切换为推理模式
 
 | 参数      | 说明                                           |
 | --------- | ---------------------------------------------- |
 | valid_set | 验证集                                         |
 | show      | 是否输出验证集损失值、准确率（默认 True）      |
 | train     | 验证后，模型是否且切换为训练模式（默认 False） |
```

