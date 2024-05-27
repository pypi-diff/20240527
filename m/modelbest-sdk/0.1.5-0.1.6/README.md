# Comparing `tmp/modelbest_sdk-0.1.5.tar.gz` & `tmp/modelbest_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelbest_sdk-0.1.5.tar", last modified: Tue May 21 09:10:06 2024, max compression
+gzip compressed data, was "modelbest_sdk-0.1.6.tar", last modified: Mon May 27 13:11:04 2024, max compression
```

## Comparing `modelbest_sdk-0.1.5.tar` & `modelbest_sdk-0.1.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 09:10:06.420877 modelbest_sdk-0.1.5/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)       99 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/MANIFEST.in
--rw-r--r--   0 zhq4206  (9461428) zhq4206  (9461428)      705 2024-05-21 09:10:06.420877 modelbest_sdk-0.1.5/PKG-INFO
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      209 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/README.md
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 09:10:06.412876 modelbest_sdk-0.1.5/modelbest_sdk/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-03-15 03:01:27.000000 modelbest_sdk-0.1.5/modelbest_sdk/__init__.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 09:10:06.412876 modelbest_sdk-0.1.5/modelbest_sdk/dataset/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/__init__.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4892 2024-05-17 07:40:42.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/batched_dataset.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 09:10:06.412876 modelbest_sdk-0.1.5/modelbest_sdk/dataset/common/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-13 09:05:23.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/common/__init__.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2606 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/common/cache.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2667 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/common/range.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1065 2024-05-16 07:06:41.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/cuda_prefetcher.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)    11249 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/mbtable_iterable_dataset.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 09:10:06.412876 modelbest_sdk-0.1.5/modelbest_sdk/dataset/megatron/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-13 09:05:23.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/megatron/__init__.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     5045 2024-05-21 09:00:07.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/megatron/segment_dataset.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4938 2024-05-20 03:47:36.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/modelbest_dataloader.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 09:10:06.412876 modelbest_sdk-0.1.5/modelbest_sdk/dataset/sampler/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/sampler/__init__.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)       58 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/sampler/sampler.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      344 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/sampler/weighted_sampler.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 09:10:06.412876 modelbest_sdk-0.1.5/modelbest_sdk/dataset/thrift_wrapper/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/thrift_wrapper/__init__.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2801 2024-05-13 09:05:23.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/thrift_wrapper/base_doc.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     7642 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2220 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/thrift_wrapper/dataset_context.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      853 2024-05-16 06:51:40.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/thrift_wrapper/utils.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4004 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/modelbest_sdk/dataset/weighted_dataset.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 09:10:06.412876 modelbest_sdk-0.1.5/modelbest_sdk/file_format/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-03-15 03:01:27.000000 modelbest_sdk-0.1.5/modelbest_sdk/file_format/__init__.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 09:10:06.412876 modelbest_sdk-0.1.5/modelbest_sdk/file_format/lib/
--rwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)  7125976 2024-05-16 08:30:13.000000 modelbest_sdk-0.1.5/modelbest_sdk/file_format/lib/libmbtable_sdk_shared.so
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     5910 2024-05-16 12:04:38.000000 modelbest_sdk-0.1.5/modelbest_sdk/file_format/mbtable.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2953 2024-05-13 09:05:23.000000 modelbest_sdk-0.1.5/modelbest_sdk/file_format/mbtable_builder.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4765 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/modelbest_sdk/file_format/mbtable_partition.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 09:10:06.420877 modelbest_sdk-0.1.5/modelbest_sdk/proto/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      405 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.5/modelbest_sdk/proto/breadcrumb.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     3060 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.5/modelbest_sdk/proto/chatdoc.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     5833 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.5/modelbest_sdk/proto/const.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      830 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.5/modelbest_sdk/proto/context.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     3846 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.5/modelbest_sdk/proto/data_base.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      631 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.5/modelbest_sdk/proto/dataset_checkpoint.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      454 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.5/modelbest_sdk/proto/dataset_context.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1806 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.5/modelbest_sdk/proto/general_doc.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1624 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.5/modelbest_sdk/proto/general_servlet_rpc.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     3408 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.5/modelbest_sdk/proto/linkinfo.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1501 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.5/modelbest_sdk/proto/mergeddoc.thrift
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      497 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.5/modelbest_sdk/proto/traindoc.thrift
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 09:10:06.412876 modelbest_sdk-0.1.5/modelbest_sdk.egg-info/
--rw-r--r--   0 zhq4206  (9461428) zhq4206  (9461428)      705 2024-05-21 09:10:06.000000 modelbest_sdk-0.1.5/modelbest_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1913 2024-05-21 09:10:06.000000 modelbest_sdk-0.1.5/modelbest_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        1 2024-05-21 09:10:06.000000 modelbest_sdk-0.1.5/modelbest_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)       19 2024-05-21 09:10:06.000000 modelbest_sdk-0.1.5/modelbest_sdk.egg-info/top_level.txt
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)       38 2024-05-21 09:10:06.420877 modelbest_sdk-0.1.5/setup.cfg
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      708 2024-05-21 09:10:04.000000 modelbest_sdk-0.1.5/setup.py
-drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 09:10:06.420877 modelbest_sdk-0.1.5/test/
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-03-15 03:01:27.000000 modelbest_sdk-0.1.5/test/__init__.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4124 2024-05-17 08:41:24.000000 modelbest_sdk-0.1.5/test/test_base.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1258 2024-05-17 08:46:12.000000 modelbest_sdk-0.1.5/test/test_batched_dataset.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4820 2024-05-17 08:44:36.000000 modelbest_sdk-0.1.5/test/test_checkpoint.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      881 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/test/test_dataset_context.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2682 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/test/test_mbtable.py
--rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2248 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.5/test/test_mbtable_partition.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.089262 modelbest_sdk-0.1.6/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)       99 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/MANIFEST.in
+-rw-r--r--   0 zhq4206  (9461428) zhq4206  (9461428)      705 2024-05-27 13:11:04.089262 modelbest_sdk-0.1.6/PKG-INFO
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      209 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/README.md
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-03-15 03:01:27.000000 modelbest_sdk-0.1.6/modelbest_sdk/__init__.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk/dataset/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/__init__.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     5434 2024-05-27 13:08:02.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/batched_dataset.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk/dataset/common/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/common/__init__.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2606 2024-05-27 12:13:33.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/common/cache.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2667 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/common/range.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1065 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/cuda_prefetcher.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)    11228 2024-05-27 13:04:55.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/mbtable_iterable_dataset.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk/dataset/megatron/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/megatron/__init__.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     5045 2024-05-23 12:03:16.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/megatron/segment_dataset.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4938 2024-05-27 10:14:19.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/modelbest_dataloader.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk/dataset/sampler/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/sampler/__init__.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)       58 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/sampler/sampler.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      344 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/sampler/weighted_sampler.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/__init__.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2801 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/base_doc.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     7642 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2220 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/dataset_context.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      853 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/utils.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4133 2024-05-27 13:10:02.000000 modelbest_sdk-0.1.6/modelbest_sdk/dataset/weighted_dataset.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk/file_format/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-03-15 03:01:27.000000 modelbest_sdk-0.1.6/modelbest_sdk/file_format/__init__.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk/file_format/lib/
+-rwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)  7125976 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/modelbest_sdk/file_format/lib/libmbtable_sdk_shared.so
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     5910 2024-05-22 10:23:07.000000 modelbest_sdk-0.1.6/modelbest_sdk/file_format/mbtable.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2953 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/modelbest_sdk/file_format/mbtable_builder.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4765 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/modelbest_sdk/file_format/mbtable_partition.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.089262 modelbest_sdk-0.1.6/modelbest_sdk/proto/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      405 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/breadcrumb.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     3259 2024-05-21 11:42:27.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/chatdoc.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     5842 2024-05-21 11:42:24.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/const.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      830 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/context.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     3846 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/data_base.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      631 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/dataset_checkpoint.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      454 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/dataset_context.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1806 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/general_doc.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1624 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/general_servlet_rpc.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     3408 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/linkinfo.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1556 2024-05-21 11:42:24.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/mergeddoc.thrift
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      497 2024-05-15 06:42:45.000000 modelbest_sdk-0.1.6/modelbest_sdk/proto/traindoc.thrift
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.081261 modelbest_sdk-0.1.6/modelbest_sdk.egg-info/
+-rw-r--r--   0 zhq4206  (9461428) zhq4206  (9461428)      705 2024-05-27 13:11:04.000000 modelbest_sdk-0.1.6/modelbest_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1913 2024-05-27 13:11:04.000000 modelbest_sdk-0.1.6/modelbest_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        1 2024-05-27 13:11:04.000000 modelbest_sdk-0.1.6/modelbest_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)       19 2024-05-27 13:11:04.000000 modelbest_sdk-0.1.6/modelbest_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)       38 2024-05-27 13:11:04.089262 modelbest_sdk-0.1.6/setup.cfg
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      708 2024-05-27 13:10:44.000000 modelbest_sdk-0.1.6/setup.py
+drwxrwxr-x   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-05-27 13:11:04.089262 modelbest_sdk-0.1.6/test/
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)        0 2024-03-15 03:01:27.000000 modelbest_sdk-0.1.6/test/__init__.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4124 2024-05-27 07:16:24.000000 modelbest_sdk-0.1.6/test/test_base.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     1258 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/test/test_batched_dataset.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     4820 2024-05-21 12:02:37.000000 modelbest_sdk-0.1.6/test/test_checkpoint.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)      881 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/test/test_dataset_context.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2682 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/test/test_mbtable.py
+-rw-rw-r--   0 zhq4206  (9461428) zhq4206  (9461428)     2248 2024-04-16 11:47:52.000000 modelbest_sdk-0.1.6/test/test_mbtable_partition.py
```

### Comparing `modelbest_sdk-0.1.5/PKG-INFO` & `modelbest_sdk-0.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelbest_sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Everything about modelbest data include data format mbtable, dataset, dataloader, and tools
 Home-page: https://codeup.aliyun.com/64ddb0a87f62ff9b3d23ca15/modelbest_sdk
 Author: HankyZhao
 Author-email: zhq980115@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/dataset/batched_dataset.py` & `modelbest_sdk-0.1.6/modelbest_sdk/dataset/batched_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,87 +1,90 @@
 from collections import defaultdict
+import hashlib
 import numpy as np
 import torch
 
 # from modelbest_sdk.dataset.collater.collater import Collater
 from modelbest_sdk.dataset.weighted_dataset import WeightedDataset
 from modelbest_sdk.dataset.thrift_wrapper.base_doc import BaseDoc
 from modelbest_sdk.dataset.thrift_wrapper.dataset_checkpoint import *
 from modelbest_sdk.dataset.thrift_wrapper.dataset_context import DatasetContext
 
 def default_factory_list():
     return list()
 
 def default_factory_dict():
     return defaultdict(default_factory_list)
-
 class BatchedDataset(torch.utils.data.IterableDataset):
     def __init__(self, context, weighted_dataset, batch_size, max_len, drop_last=False):
         self.context = context
         self.weighted_dataset = weighted_dataset
         self.max_total_length = batch_size * max_len
         self.batch_size = 1
         self.drop_last = drop_last
         
         self.buffer = []
         self.current_length = 0
-        
 
+        # 初始化tag_to_index
+        self.tag_to_hash = defaultdict()
+      
     def put(self, data):
         self.buffer.append(data)
         self.current_length += len(data['doc'].token_ids)
     
     def pop(self):
         lengths = []
         indexes = defaultdict(default_factory_dict)        
         inputs = torch.zeros((self.batch_size, self.max_total_length), dtype=torch.int32)
         targets = torch.full((self.batch_size, self.max_total_length), dtype=torch.int32, fill_value=-100)
         dataset_ids = torch.full((self.batch_size, self.max_total_length), dtype=torch.int32, fill_value=-1)
         position_ids = torch.zeros((self.batch_size, self.max_total_length), dtype=torch.int32)
+        tags = torch.full((self.batch_size, self.max_total_length), dtype=torch.int64, fill_value=-1)
 
         span_begin = 0
         while self.buffer:
             data = self.buffer.pop()
             chunk = data['chunk']
             index = data['index']
             dataset_idx = data['dataset_idx']
             doc: BaseDoc = data['doc']
             token_ids = doc.token_ids
             mask = doc.mask
-            tag = doc.tag
-            target_ids = [token_id if not mask_val else -100 for token_id, mask_val in zip(token_ids[1:], mask[1:])] + [-100]
-            
+            tag = doc.tag[0] # TODO: support multiple tags
+            target_ids = np.where(mask[1:], -100, token_ids[1:]).tolist() + [-100]
             span_end = span_begin + len(token_ids)
             # TODO: what if the inputs is longer than max_total_length?
             # RuntimeError: The expanded size of the tensor (16) must match the existing size (385) at non-singleton dimension 0.  Target sizes: [16].  Tensor sizes: [385]
             inputs[0, span_begin:span_end] = torch.tensor(token_ids, dtype=torch.int32)
             targets[0, span_begin:span_end] = torch.tensor(target_ids, dtype=torch.int32)
             dataset_ids[0, span_begin:span_end] = torch.tensor(dataset_idx, dtype=torch.int32)
             position_ids[0, span_begin:span_end] = torch.from_numpy(np.arange(len(token_ids), dtype=np.int32))
             lengths.append(len(token_ids))
             indexes[int(dataset_idx)][chunk].append(index)
+            tags[0, span_begin:span_end] = self.encode_tags(token_ids, tag)
             span_begin = span_end
         cu_seqlens = torch.cat(
             [torch.tensor([0] + lengths).cumsum(dim=-1), torch.tensor([self.max_total_length], dtype=torch.int32)],
             dim=0,
         ).int()
         batch = {
             "input_ids": inputs,
             "target_ids": targets,
             "dataset_ids": dataset_ids,
             "indexes": indexes,
             "cu_seqlens": cu_seqlens,
             "max_seqlen": int(torch.max(cu_seqlens[1:] - cu_seqlens[:-1])),
             "lengths": torch.tensor(sum(lengths)).int(),
             "position_ids": position_ids,
-            # TODO: add tags
+            "tags": tags,
+            "tag_to_hash": self.tag_to_hash
         }
         self.current_length = 0
         return batch
-        # TODO: return data directly, and pack in collate_fn
         
 
     def will_exceed(self, data):
         return self.current_length + len(data['doc'].token_ids) > self.max_total_length
 
     def __iter__(self):
         for data in self.weighted_dataset:
@@ -91,26 +94,34 @@
         if not self.drop_last and self.buffer:
             yield self.pop()
 
     @staticmethod
     def collate_fn(batch):
         return batch[0]
     
+    def encode_tags(self, token_ids, tag):
+        tag_hash = self._get_tag_hash(tag)
+        self.tag_to_hash[tag] = tag_hash
+        return torch.full((len(token_ids),), tag_hash, dtype=torch.int64)
+    
+    def _get_tag_hash(self, tag: str) -> int:
+        hash_obj = hashlib.sha256(tag.encode('utf-8'))
+        return int(hash_obj.hexdigest(), 16) & ((1 << 63) - 1)
 
 if __name__ == '__main__':
     context = DatasetContext(world_size=1, rank=0, num_workers=1)
 
     dataset_info_list = [
         DatasetInfo(
-            path="/home/emr-user/modelbest_sdk/test/base_doc_simple",
+            path="human.BaseDoc.sstable",
             weight=1,
             max_epoch=1
         ),
         DatasetInfo(
-            path="/home/emr-user/modelbest_sdk/test/base_doc_easy",
+            path="hot_chars.BaseDoc.sstable",
             weight=2,
             max_epoch=2
         )
     ]
     
     dataset_info_list = DatasetInfoList(dataset_info_list)
     
@@ -118,16 +129,16 @@
         context=context,
         dataset_info_list=dataset_info_list
     )
     
     dataset = BatchedDataset(
         context=context,
         weighted_dataset=w_dataset,
-        batch_size=16,
-        max_len=1
+        batch_size=1,
+        max_len=8192
     )
     
     for data in dataset:
         print(data)
         print(data['indexes'].keys())
         print(data['indexes'].values())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/dataset/common/cache.py` & `modelbest_sdk-0.1.6/modelbest_sdk/dataset/common/cache.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/dataset/common/range.py` & `modelbest_sdk-0.1.6/modelbest_sdk/dataset/common/range.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/dataset/cuda_prefetcher.py` & `modelbest_sdk-0.1.6/modelbest_sdk/dataset/cuda_prefetcher.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/dataset/mbtable_iterable_dataset.py` & `modelbest_sdk-0.1.6/modelbest_sdk/dataset/mbtable_iterable_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
     def prefetch(self):
         while True:
             try:
                 chunk = self.cache.pull_task()
                 chunk_data = self.get_chunk_data(chunk)
                 unused_chunk_data = [
-                    dict(chunk=chunk, index=i, doc=BaseDoc.deserialize(data))
+                    dict(chunk=chunk, index=i, raw=data)
                     for i, data in zip(range(chunk.start, chunk.stop), chunk_data)
                     if (data is not None) and (i not in self.used.active.get(chunk, set()))
                 ]
                 self.cache.put_result(unused_chunk_data)
             except CacheFull:
                 time.sleep(0.1)
             except AllCached:
```

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/dataset/megatron/segment_dataset.py` & `modelbest_sdk-0.1.6/modelbest_sdk/dataset/megatron/segment_dataset.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/dataset/modelbest_dataloader.py` & `modelbest_sdk-0.1.6/modelbest_sdk/dataset/modelbest_dataloader.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/dataset/thrift_wrapper/base_doc.py` & `modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/base_doc.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py` & `modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/dataset/thrift_wrapper/dataset_context.py` & `modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/dataset_context.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/dataset/thrift_wrapper/utils.py` & `modelbest_sdk-0.1.6/modelbest_sdk/dataset/thrift_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/dataset/weighted_dataset.py` & `modelbest_sdk-0.1.6/modelbest_sdk/dataset/weighted_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import numpy as np
 import torch
 from modelbest_sdk.dataset.mbtable_iterable_dataset import MBTableIterableDataset
 from modelbest_sdk.dataset.sampler.weighted_sampler import WeightedSampler
+from modelbest_sdk.dataset.thrift_wrapper.base_doc import BaseDoc
 from modelbest_sdk.dataset.thrift_wrapper.dataset_checkpoint import *
 from modelbest_sdk.dataset.thrift_wrapper.dataset_context import DatasetContext
 
 logger = logging.getLogger(__name__)
 
 MAX_EPOCH = 2**31 - 1
 
@@ -59,14 +60,15 @@
                 continue
             chosen_iter = self.datasets_iter[idx]
             try:
                 data = next(chosen_iter)
                 if data is None:
                     continue
                 data['dataset_idx'] = idx
+                data['doc'] = BaseDoc.deserialize(data['raw'])
                 yield data
             except StopIteration:
                 continue
 
 
     def set_seed(self):
         np.random.seed(self.context.world_size + self.context.rank)
```

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/file_format/lib/libmbtable_sdk_shared.so` & `modelbest_sdk-0.1.6/modelbest_sdk/file_format/lib/libmbtable_sdk_shared.so`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/file_format/mbtable.py` & `modelbest_sdk-0.1.6/modelbest_sdk/file_format/mbtable.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/file_format/mbtable_builder.py` & `modelbest_sdk-0.1.6/modelbest_sdk/file_format/mbtable_builder.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/file_format/mbtable_partition.py` & `modelbest_sdk-0.1.6/modelbest_sdk/file_format/mbtable_partition.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/proto/chatdoc.thrift` & `modelbest_sdk-0.1.6/modelbest_sdk/proto/chatdoc.thrift`

 * *Files 16% similar despite different names*

```diff
@@ -41,14 +41,24 @@
     SAFETY = 10;
     // B站
     BILIBILI = 11;
     // 微博
     WEIBO = 12;
     // Hindi
     HINDI = 13;
+    // 表情包
+    STICKER = 14;
+    // nsfw-0
+    NSFW_ZERO_LEVEL = 15;
+    // nsfw-1
+    NSFW_FIRST_LEVEL = 16;
+    // nsfw-2
+    NSFW_SECOND_LEVEL = 17;
+    // nsfw-3
+    NSFW_THIRD_LEVEL = 18;
 }
 
 struct Profile {
     // 模型角色自称
     10: string role,
     // 基本信息
     20: optional string basic_info,
```

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/proto/const.thrift` & `modelbest_sdk-0.1.6/modelbest_sdk/proto/const.thrift`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 const string PROMPT_7 = "是"
 const string RAG_PROMPT = "下面会给你提供一段背景知识，请你在回答之前参考这段知识进行回答。"
 // prompt拼接字段list类型
 const list<string> PROMPT_0_LIST = ["现在请你假扮","现在请你扮演","你是角色扮演大师，你将扮演","你是一名知名演员，你要演绎",'现在请你扮演','请你此刻假装成','现在，我需要你假装自己是','现在，请你扮演一下','请你现在开始扮演','此刻，请你假扮成','现在，请你进行角色扮演','请你现在假扮成那个','现在请你进入角色扮演模式，扮演']
 const list<string> PROMPT_1_LIST = ["与我进行对话",'与我展开交流','与我进行交谈','与我进行沟通对话','与我进行语言交流','和我对话一番','与我进行互动对话','和我展开对话交流','与我进行深入的对话','与我进行对话交流吧']
 const list<string> PROMPT_2_LIST = ["接下来的对话里，你需要扮演",'在接下来的对话中，你需要扮演','在接下来的交流中，你需要担当','接下来的对话中，需要你扮演','请你在接下来的对话中，扮演','接下来的交流里，你的角色是','请你在接下来的对话中，担任','在对话的接下来部分，你需要扮演','接下来的对话中，你的任务是扮演','在接下来的对话环节，你需要化身']
 const list<string> PROMPT_3_LIST = ["我将扮演：",'我将扮演起：', '我将化身为：', '我将饰演：', '我将模仿：', '我将充当：', '我将演绎：', '我将假扮：', '我是']
-const list<string> PROMPT_4_LIST = ["我们的关系是：","你和我之间的关系是：","我们之间的关系是：",""]
+const list<string> PROMPT_4_LIST = ["我们的关系是：","你和我之间的关系是：","我们之间的关系是：","关系是"]
 const list<string> PROMPT_5_LIST = ["[开始对话]",'[展开对话]','[发起对话]','[启动对话]','[进行对话交流]','[开展对话]','[进行对话]','[开始交谈]','[发起沟通]','[展开交流]','[发起对话交流]']
 const list<string> PROMPT_6_LIST = ["指令：","命令：","你将要：","你需要："]
 const list<string> PROMPT_7_LIST = ["是","为"]
 const list<string> RAG_PROMPT_LIST = ["下面会给你提供一段背景知识，请你在回答之前参考这段知识进行回答。",'在你回答之前，我会先给你一段背景知识，请务必参考它。','请在回答之前，仔细阅读我提供的这段背景知识，以便更好地理解问题。','为了帮助你更好地回答，我会先给出一段背景知识，请务必参考。','在你给出答案之前，请确保已经阅读并理解了这段背景知识。','请参考我提供的背景知识来回答，这样你的答案会更加准确和全面。','在你开始回答之前，先阅读一下这段背景知识，这对你会有帮助的。','为了确保你的回答更加精准，请先参考我提供的这段背景知识。','在你构思答案时，请务必参考我所提供的背景知识。','我会先给出一段背景知识，你在回答时请以此为参考。','为了使你的回答更加有依据，请在阅读并理解这段背景知识后再进行回答。']
 // prompt大框架需要固定
 const string BASIC_INFO_TEXT = "基本信息"
 const string PERSONALITY_TEXT = "的性格"
```

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/proto/context.thrift` & `modelbest_sdk-0.1.6/modelbest_sdk/proto/context.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/proto/data_base.thrift` & `modelbest_sdk-0.1.6/modelbest_sdk/proto/data_base.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/proto/dataset_checkpoint.thrift` & `modelbest_sdk-0.1.6/modelbest_sdk/proto/dataset_checkpoint.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/proto/general_doc.thrift` & `modelbest_sdk-0.1.6/modelbest_sdk/proto/general_doc.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/proto/general_servlet_rpc.thrift` & `modelbest_sdk-0.1.6/modelbest_sdk/proto/general_servlet_rpc.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/proto/linkinfo.thrift` & `modelbest_sdk-0.1.6/modelbest_sdk/proto/linkinfo.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk/proto/mergeddoc.thrift` & `modelbest_sdk-0.1.6/modelbest_sdk/proto/mergeddoc.thrift`

 * *Files 11% similar despite different names*

```diff
@@ -47,8 +47,10 @@
   38: i32 language = 0,
   39: bool content_compressed,
   40: i32 domain_id = 0,
   42: i16 host_rank = 0,
   62: string title,
   65: optional list<breadcrumb.BreadCrumb_Item> breadcrumb_info,
   136: string body,
+  137: double perplexity,
+  138: i16 domain_level = 0,
 }
```

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk.egg-info/PKG-INFO` & `modelbest_sdk-0.1.6/modelbest_sdk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelbest-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Everything about modelbest data include data format mbtable, dataset, dataloader, and tools
 Home-page: https://codeup.aliyun.com/64ddb0a87f62ff9b3d23ca15/modelbest_sdk
 Author: HankyZhao
 Author-email: zhq980115@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `modelbest_sdk-0.1.5/modelbest_sdk.egg-info/SOURCES.txt` & `modelbest_sdk-0.1.6/modelbest_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/setup.py` & `modelbest_sdk-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modelbest_sdk',
-    version='0.1.5',
+    version='0.1.6',
     author='HankyZhao',
     author_email='zhq980115@gmail.com',
     description='Everything about modelbest data include data format mbtable, dataset, dataloader, and tools',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url='https://codeup.aliyun.com/64ddb0a87f62ff9b3d23ca15/modelbest_sdk',
     packages=find_packages(),
```

### Comparing `modelbest_sdk-0.1.5/test/test_base.py` & `modelbest_sdk-0.1.6/test/test_base.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/test/test_batched_dataset.py` & `modelbest_sdk-0.1.6/test/test_batched_dataset.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/test/test_checkpoint.py` & `modelbest_sdk-0.1.6/test/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/test/test_dataset_context.py` & `modelbest_sdk-0.1.6/test/test_dataset_context.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/test/test_mbtable.py` & `modelbest_sdk-0.1.6/test/test_mbtable.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.5/test/test_mbtable_partition.py` & `modelbest_sdk-0.1.6/test/test_mbtable_partition.py`

 * *Files identical despite different names*

