# Comparing `tmp/mb_pytorch-1.0.50.tar.gz` & `tmp/mb_pytorch-1.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mb_pytorch-1.0.50.tar", last modified: Mon May 27 01:40:25 2024, max compression
+gzip compressed data, was "mb_pytorch-1.0.51.tar", last modified: Mon May 27 20:23:33 2024, max compression
```

## Comparing `mb_pytorch-1.0.50.tar` & `mb_pytorch-1.0.51.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 01:40:25.414439 mb_pytorch-1.0.50/
--rw-r--r--   0 malav     (1000) malav     (1000)      206 2024-05-27 01:40:25.414439 mb_pytorch-1.0.50/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)      742 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/README.md
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 01:40:25.410439 mb_pytorch-1.0.50/mb_pytorch/
--rw-rw-r--   0 malav     (1000) malav     (1000)       97 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 01:40:25.410439 mb_pytorch-1.0.50/mb_pytorch/classification/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:38:04.000000 mb_pytorch-1.0.50/mb_pytorch/classification/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     7166 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/classification/training.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 01:40:25.414439 mb_pytorch-1.0.50/mb_pytorch/dataloader/
--rw-rw-r--   0 malav     (1000) malav     (1000)       44 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/dataloader/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    19235 2024-05-27 01:40:00.000000 mb_pytorch-1.0.50/mb_pytorch/dataloader/loader.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 01:40:25.414439 mb_pytorch-1.0.50/mb_pytorch/detection/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:38:14.000000 mb_pytorch-1.0.50/mb_pytorch/detection/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     6583 2024-05-27 01:13:06.000000 mb_pytorch-1.0.50/mb_pytorch/detection/training.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 01:40:25.414439 mb_pytorch-1.0.50/mb_pytorch/metalearning/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/metalearning/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1385 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/metalearning/meta_utils.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1030 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/metalearning/proto_dataloader.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2861 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/metalearning/prototypical.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 01:40:25.414439 mb_pytorch-1.0.50/mb_pytorch/models/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/models/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 01:40:25.414439 mb_pytorch-1.0.50/mb_pytorch/models/blocks/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/models/blocks/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2801 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/models/blocks/attention_block.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     3629 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/models/blocks/cnn.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     4783 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/models/blocks/conv_block.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      920 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/models/blocks/conv_with_relu.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2256 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/models/blocks/model_out.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1184 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/models/blocks/rnn.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    21087 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/models/extra_models.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      920 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/models/lenet.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     3921 2024-05-17 14:58:48.000000 mb_pytorch-1.0.50/mb_pytorch/models/modelloader.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    10784 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/models/unet_models.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 01:40:25.414439 mb_pytorch-1.0.50/mb_pytorch/segmentation/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:59:50.000000 mb_pytorch-1.0.50/mb_pytorch/segmentation/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     4800 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/segmentation/training.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 01:40:25.414439 mb_pytorch-1.0.50/mb_pytorch/training/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:59:41.000000 mb_pytorch-1.0.50/mb_pytorch/training/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1630 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/training/accelerate_train.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1454 2024-05-17 23:03:52.000000 mb_pytorch-1.0.50/mb_pytorch/training/train_params.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      144 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/training/training.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 01:40:25.414439 mb_pytorch-1.0.50/mb_pytorch/utils/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/utils/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1055 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/utils/compiler.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      257 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/utils/dist.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     3391 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/utils/extra_utils.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     7097 2024-05-13 00:29:33.000000 mb_pytorch-1.0.50/mb_pytorch/utils/generate_emb.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2582 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/utils/losses.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1199 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/utils/metrics.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-05-27 01:40:19.000000 mb_pytorch-1.0.50/mb_pytorch/utils/version.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    10620 2024-05-23 19:25:11.000000 mb_pytorch-1.0.50/mb_pytorch/utils/viewer.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      994 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/mb_pytorch/utils/yaml_reader.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 01:40:25.414439 mb_pytorch-1.0.50/mb_pytorch.egg-info/
--rw-r--r--   0 malav     (1000) malav     (1000)      206 2024-05-27 01:40:25.000000 mb_pytorch-1.0.50/mb_pytorch.egg-info/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)     1607 2024-05-27 01:40:25.000000 mb_pytorch-1.0.50/mb_pytorch.egg-info/SOURCES.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-27 01:40:25.000000 mb_pytorch-1.0.50/mb_pytorch.egg-info/dependency_links.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-27 01:40:25.000000 mb_pytorch-1.0.50/mb_pytorch.egg-info/requires.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       19 2024-05-27 01:40:25.000000 mb_pytorch-1.0.50/mb_pytorch.egg-info/top_level.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/pyproject.toml
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 01:40:25.414439 mb_pytorch-1.0.50/scripts/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/scripts/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 01:40:25.414439 mb_pytorch-1.0.50/scripts/extra_utils/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/scripts/extra_utils/__init__.py
--rwxrwxr-x   0 malav     (1000) malav     (1000)     1314 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/scripts/extra_utils/dataload_results.py
--rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-27 01:40:25.414439 mb_pytorch-1.0.50/setup.cfg
--rw-rw-r--   0 malav     (1000) malav     (1000)      818 2024-05-06 17:42:04.000000 mb_pytorch-1.0.50/setup.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 20:23:33.425953 mb_pytorch-1.0.51/
+-rw-r--r--   0 malav     (1000) malav     (1000)      206 2024-05-27 20:23:33.425953 mb_pytorch-1.0.51/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)      742 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/README.md
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 20:23:33.421953 mb_pytorch-1.0.51/mb_pytorch/
+-rw-rw-r--   0 malav     (1000) malav     (1000)       97 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 20:23:33.421953 mb_pytorch-1.0.51/mb_pytorch/classification/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:38:04.000000 mb_pytorch-1.0.51/mb_pytorch/classification/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     7166 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/classification/training.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 20:23:33.421953 mb_pytorch-1.0.51/mb_pytorch/dataloader/
+-rw-rw-r--   0 malav     (1000) malav     (1000)       44 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/dataloader/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    19177 2024-05-27 20:23:12.000000 mb_pytorch-1.0.51/mb_pytorch/dataloader/loader.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 20:23:33.421953 mb_pytorch-1.0.51/mb_pytorch/detection/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:38:14.000000 mb_pytorch-1.0.51/mb_pytorch/detection/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     6583 2024-05-27 01:13:06.000000 mb_pytorch-1.0.51/mb_pytorch/detection/training.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 20:23:33.421953 mb_pytorch-1.0.51/mb_pytorch/metalearning/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/metalearning/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1385 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/metalearning/meta_utils.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1030 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/metalearning/proto_dataloader.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     2861 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/metalearning/prototypical.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 20:23:33.425953 mb_pytorch-1.0.51/mb_pytorch/models/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/models/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 20:23:33.425953 mb_pytorch-1.0.51/mb_pytorch/models/blocks/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/models/blocks/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     2801 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/models/blocks/attention_block.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     3629 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/models/blocks/cnn.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     4783 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/models/blocks/conv_block.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      920 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/models/blocks/conv_with_relu.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     2256 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/models/blocks/model_out.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1184 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/models/blocks/rnn.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    21087 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/models/extra_models.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      920 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/models/lenet.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     3921 2024-05-17 14:58:48.000000 mb_pytorch-1.0.51/mb_pytorch/models/modelloader.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    10784 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/models/unet_models.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 20:23:33.425953 mb_pytorch-1.0.51/mb_pytorch/segmentation/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:59:50.000000 mb_pytorch-1.0.51/mb_pytorch/segmentation/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     4800 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/segmentation/training.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 20:23:33.425953 mb_pytorch-1.0.51/mb_pytorch/training/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:59:41.000000 mb_pytorch-1.0.51/mb_pytorch/training/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1630 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/training/accelerate_train.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1454 2024-05-17 23:03:52.000000 mb_pytorch-1.0.51/mb_pytorch/training/train_params.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      144 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/training/training.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 20:23:33.425953 mb_pytorch-1.0.51/mb_pytorch/utils/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/utils/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1055 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/utils/compiler.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      257 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/utils/dist.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     3391 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/utils/extra_utils.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     7097 2024-05-13 00:29:33.000000 mb_pytorch-1.0.51/mb_pytorch/utils/generate_emb.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     2582 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/utils/losses.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1199 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/utils/metrics.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-05-27 20:23:18.000000 mb_pytorch-1.0.51/mb_pytorch/utils/version.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    10620 2024-05-23 19:25:11.000000 mb_pytorch-1.0.51/mb_pytorch/utils/viewer.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      994 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/mb_pytorch/utils/yaml_reader.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 20:23:33.425953 mb_pytorch-1.0.51/mb_pytorch.egg-info/
+-rw-r--r--   0 malav     (1000) malav     (1000)      206 2024-05-27 20:23:33.000000 mb_pytorch-1.0.51/mb_pytorch.egg-info/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1607 2024-05-27 20:23:33.000000 mb_pytorch-1.0.51/mb_pytorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-27 20:23:33.000000 mb_pytorch-1.0.51/mb_pytorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-27 20:23:33.000000 mb_pytorch-1.0.51/mb_pytorch.egg-info/requires.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       19 2024-05-27 20:23:33.000000 mb_pytorch-1.0.51/mb_pytorch.egg-info/top_level.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/pyproject.toml
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 20:23:33.425953 mb_pytorch-1.0.51/scripts/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/scripts/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 20:23:33.425953 mb_pytorch-1.0.51/scripts/extra_utils/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/scripts/extra_utils/__init__.py
+-rwxrwxr-x   0 malav     (1000) malav     (1000)     1314 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/scripts/extra_utils/dataload_results.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-27 20:23:33.425953 mb_pytorch-1.0.51/setup.cfg
+-rw-rw-r--   0 malav     (1000) malav     (1000)      818 2024-05-06 17:42:04.000000 mb_pytorch-1.0.51/setup.py
```

### Comparing `mb_pytorch-1.0.50/README.md` & `mb_pytorch-1.0.51/README.md`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/classification/training.py` & `mb_pytorch-1.0.51/mb_pytorch/classification/training.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/dataloader/loader.py` & `mb_pytorch-1.0.51/mb_pytorch/dataloader/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,29 +305,27 @@
 
             return out_dict
         
         if self.data_type == 'segmentation':
             if self.transform:
                 mask = cv2.imread(self.masks.iloc[idx],cv2.IMREAD_GRAYSCALE) ## considering mask is just binary class
                 img,mask = self.transform(img,mask)
-            out_dict = {'image':img}
-            out_dict['mask'] = mask
-            out_dict['label'] = self.label.iloc[idx]
+            mask_dict = {'mask':mask}
+            mask_dict['label'] = self.label.iloc[idx]
             
-            return out_dict
+            return img,mask_dict
         
         if self.data_type == 'detection':
             if self.transform:
                 img,bbox = self.transform(img,bbox)
-            out_dict = {'image':img}
-            out_dict['bbox'] = torch.tensor([[self.bbox.iloc[idx][0],self.bbox.iloc[idx][1],self.bbox.iloc[idx][2],self.bbox.iloc[idx][3]] 
-                                             for x in len(self.bbox.iloc[idx])],dtype=torch.float32)  ## should be list in a list. 
-            out_dict['label'] = self.label.iloc[idx]
+            bbox_dict = {'boxes':torch.tensor([[self.bbox.iloc[idx][0],self.bbox.iloc[idx][1],self.bbox.iloc[idx][2],self.bbox.iloc[idx][3]] 
+                                             for x in len(self.bbox.iloc[idx])],dtype=torch.float32)}  ## should be list in a list.
+            bbox_dict['label'] = self.label.iloc[idx]
 
-            return out_dict
+            return img,bbox_dict
 
 class DataLoader(data_fetcher):
     """
     Basic dataloader for pytorch1.0
     """
     def __init__(self,yaml,logger=None) -> None:
         super().__init__(yaml, logger=logger)
```

### Comparing `mb_pytorch-1.0.50/mb_pytorch/detection/training.py` & `mb_pytorch-1.0.51/mb_pytorch/detection/training.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/metalearning/meta_utils.py` & `mb_pytorch-1.0.51/mb_pytorch/metalearning/meta_utils.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/metalearning/proto_dataloader.py` & `mb_pytorch-1.0.51/mb_pytorch/metalearning/proto_dataloader.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/metalearning/prototypical.py` & `mb_pytorch-1.0.51/mb_pytorch/metalearning/prototypical.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/models/blocks/attention_block.py` & `mb_pytorch-1.0.51/mb_pytorch/models/blocks/attention_block.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/models/blocks/cnn.py` & `mb_pytorch-1.0.51/mb_pytorch/models/blocks/cnn.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/models/blocks/conv_block.py` & `mb_pytorch-1.0.51/mb_pytorch/models/blocks/conv_block.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/models/blocks/conv_with_relu.py` & `mb_pytorch-1.0.51/mb_pytorch/models/blocks/conv_with_relu.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/models/blocks/model_out.py` & `mb_pytorch-1.0.51/mb_pytorch/models/blocks/model_out.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/models/blocks/rnn.py` & `mb_pytorch-1.0.51/mb_pytorch/models/blocks/rnn.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/models/extra_models.py` & `mb_pytorch-1.0.51/mb_pytorch/models/extra_models.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/models/lenet.py` & `mb_pytorch-1.0.51/mb_pytorch/models/lenet.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/models/modelloader.py` & `mb_pytorch-1.0.51/mb_pytorch/models/modelloader.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/models/unet_models.py` & `mb_pytorch-1.0.51/mb_pytorch/models/unet_models.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/segmentation/training.py` & `mb_pytorch-1.0.51/mb_pytorch/segmentation/training.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/training/accelerate_train.py` & `mb_pytorch-1.0.51/mb_pytorch/training/accelerate_train.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/training/train_params.py` & `mb_pytorch-1.0.51/mb_pytorch/training/train_params.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/utils/compiler.py` & `mb_pytorch-1.0.51/mb_pytorch/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/utils/extra_utils.py` & `mb_pytorch-1.0.51/mb_pytorch/utils/extra_utils.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/utils/generate_emb.py` & `mb_pytorch-1.0.51/mb_pytorch/utils/generate_emb.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/utils/losses.py` & `mb_pytorch-1.0.51/mb_pytorch/utils/losses.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/utils/metrics.py` & `mb_pytorch-1.0.51/mb_pytorch/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/utils/viewer.py` & `mb_pytorch-1.0.51/mb_pytorch/utils/viewer.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch/utils/yaml_reader.py` & `mb_pytorch-1.0.51/mb_pytorch/utils/yaml_reader.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/mb_pytorch.egg-info/SOURCES.txt` & `mb_pytorch-1.0.51/mb_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/scripts/extra_utils/dataload_results.py` & `mb_pytorch-1.0.51/scripts/extra_utils/dataload_results.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.50/setup.py` & `mb_pytorch-1.0.51/setup.py`

 * *Files identical despite different names*

