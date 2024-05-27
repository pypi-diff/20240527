# Comparing `tmp/gen3_tracker-0.0.4rc7.tar.gz` & `tmp/gen3_tracker-0.0.4rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_tracker-0.0.4rc7.tar", last modified: Fri May 24 00:46:43 2024, max compression
+gzip compressed data, was "gen3_tracker-0.0.4rc8.tar", last modified: Sat May 25 13:55:30 2024, max compression
```

## Comparing `gen3_tracker-0.0.4rc7.tar` & `gen3_tracker-0.0.4rc8.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-24 00:46:43.928581 gen3_tracker-0.0.4rc7/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1065 2023-05-04 14:32:05.000000 gen3_tracker-0.0.4rc7/LICENSE
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2371 2024-05-24 00:46:43.928069 gen3_tracker-0.0.4rc7/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1524 2024-05-06 16:38:51.000000 gen3_tracker-0.0.4rc7/README.md
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-24 00:46:43.872515 gen3_tracker-0.0.4rc7/gen3_tracker/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5974 2024-05-22 00:42:43.000000 gen3_tracker-0.0.4rc7/gen3_tracker/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2963 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/cli.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-24 00:46:43.882881 gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-10-19 18:09:26.000000 gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-24 00:46:43.887071 gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/access/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3310 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5151 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/access/cli.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-24 00:46:43.893838 gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/access/policies/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-07 00:00:20.000000 gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/access/policies/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      189 2024-02-29 16:26:49.000000 gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/access/policies/add-project-default.yaml
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       76 2024-02-26 20:40:22.000000 gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/access/policies/add-user-read.yaml
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      204 2024-05-09 02:02:53.000000 gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/access/policies/add-user-write.yaml
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     6820 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/access/requestor.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1123 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/access/submitter.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    13796 2024-05-15 03:49:57.000000 gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/cli.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-24 00:46:43.894398 gen3_tracker-0.0.4rc7/gen3_tracker/common/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    18461 2024-05-21 23:43:06.000000 gen3_tracker-0.0.4rc7/gen3_tracker/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-24 00:46:43.895347 gen3_tracker-0.0.4rc7/gen3_tracker/config/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    10325 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      137 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc7/gen3_tracker/config.yaml
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-24 00:46:43.897255 gen3_tracker-0.0.4rc7/gen3_tracker/gen3/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-04-27 13:15:12.000000 gen3_tracker-0.0.4rc7/gen3_tracker/gen3/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-24 00:46:43.899518 gen3_tracker-0.0.4rc7/gen3_tracker/gen3/buckets/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1323 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/gen3/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      883 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc7/gen3_tracker/gen3/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      559 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc7/gen3_tracker/gen3/buckets/lister.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3354 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/gen3/indexd.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     6201 2024-05-15 20:04:35.000000 gen3_tracker-0.0.4rc7/gen3_tracker/gen3/jobs.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-24 00:46:43.910387 gen3_tracker-0.0.4rc7/gen3_tracker/git/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    23443 2024-05-16 06:52:43.000000 gen3_tracker-0.0.4rc7/gen3_tracker/git/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    11639 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/git/adder.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    37906 2024-05-16 19:45:28.000000 gen3_tracker-0.0.4rc7/gen3_tracker/git/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3026 2024-05-16 13:45:52.000000 gen3_tracker-0.0.4rc7/gen3_tracker/git/cloner.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1466 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/git/initializer.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2609 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/git/snapshotter.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-24 00:46:43.913993 gen3_tracker-0.0.4rc7/gen3_tracker/meta/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5924 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5107 2024-05-23 14:56:48.000000 gen3_tracker-0.0.4rc7/gen3_tracker/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    24570 2024-05-24 00:45:27.000000 gen3_tracker-0.0.4rc7/gen3_tracker/meta/dataframer.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    13547 2024-05-23 14:55:54.000000 gen3_tracker-0.0.4rc7/gen3_tracker/meta/skeleton.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4428 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/meta/validator.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1211 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/meta/visualizer.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-24 00:46:43.916561 gen3_tracker-0.0.4rc7/gen3_tracker/projects/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2781 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4799 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2411 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1566 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc7/gen3_tracker/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-24 00:46:43.881375 gen3_tracker-0.0.4rc7/gen3_tracker.egg-info/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2371 2024-05-24 00:46:43.000000 gen3_tracker-0.0.4rc7/gen3_tracker.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1857 2024-05-24 00:46:43.000000 gen3_tracker-0.0.4rc7/gen3_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        1 2024-05-24 00:46:43.000000 gen3_tracker-0.0.4rc7/gen3_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       45 2024-05-24 00:46:43.000000 gen3_tracker-0.0.4rc7/gen3_tracker.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      209 2024-05-24 00:46:43.000000 gen3_tracker-0.0.4rc7/gen3_tracker.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       13 2024-05-24 00:46:43.000000 gen3_tracker-0.0.4rc7/gen3_tracker.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       38 2024-05-24 00:46:43.928635 gen3_tracker-0.0.4rc7/setup.cfg
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      912 2024-05-24 00:46:22.000000 gen3_tracker-0.0.4rc7/setup.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-24 00:46:43.917035 gen3_tracker-0.0.4rc7/tests/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-04-16 13:21:28.000000 gen3_tracker-0.0.4rc7/tests/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-24 00:46:43.923568 gen3_tracker-0.0.4rc7/tests/integration/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2307 2024-05-15 03:31:16.000000 gen3_tracker-0.0.4rc7/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      470 2024-05-05 15:05:17.000000 gen3_tracker-0.0.4rc7/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3388 2024-05-16 02:28:15.000000 gen3_tracker-0.0.4rc7/tests/integration/test_bucket_import.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3394 2024-05-15 03:31:16.000000 gen3_tracker-0.0.4rc7/tests/integration/test_bundle.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3913 2024-05-16 03:02:50.000000 gen3_tracker-0.0.4rc7/tests/integration/test_end_to_end_workflow.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-24 00:46:43.926930 gen3_tracker-0.0.4rc7/tests/unit/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-05-02 22:49:35.000000 gen3_tracker-0.0.4rc7/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    20363 2024-05-01 22:45:46.000000 gen3_tracker-0.0.4rc7/tests/unit/test_flatten_fhir_example.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1285 2024-05-15 03:31:16.000000 gen3_tracker-0.0.4rc7/tests/unit/test_hash_types.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      601 2024-05-15 03:31:16.000000 gen3_tracker-0.0.4rc7/tests/unit/test_read_dvc.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-25 13:55:30.329281 gen3_tracker-0.0.4rc8/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_tracker-0.0.4rc8/LICENSE
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2371 2024-05-25 13:55:30.327540 gen3_tracker-0.0.4rc8/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1524 2024-05-06 16:38:51.000000 gen3_tracker-0.0.4rc8/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-25 13:55:30.246539 gen3_tracker-0.0.4rc8/gen3_tracker/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5974 2024-05-22 00:42:43.000000 gen3_tracker-0.0.4rc8/gen3_tracker/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2963 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-25 13:55:30.257993 gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-10-19 18:09:26.000000 gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-25 13:55:30.262084 gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/access/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3310 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/access/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5151 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/access/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-25 13:55:30.263947 gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/access/policies/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/access/policies/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      189 2024-02-29 16:26:49.000000 gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/access/policies/add-project-default.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142       76 2024-02-26 20:40:22.000000 gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/access/policies/add-user-read.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142      204 2024-05-09 02:02:53.000000 gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/access/policies/add-user-write.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6820 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/access/requestor.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1123 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/access/submitter.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    13796 2024-05-15 03:49:57.000000 gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-25 13:55:30.264837 gen3_tracker-0.0.4rc8/gen3_tracker/common/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    18461 2024-05-21 23:43:06.000000 gen3_tracker-0.0.4rc8/gen3_tracker/common/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-25 13:55:30.265540 gen3_tracker-0.0.4rc8/gen3_tracker/config/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    10325 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/config/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      137 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc8/gen3_tracker/config.yaml
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-25 13:55:30.266786 gen3_tracker-0.0.4rc8/gen3_tracker/gen3/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-04-27 13:15:12.000000 gen3_tracker-0.0.4rc8/gen3_tracker/gen3/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-25 13:55:30.269335 gen3_tracker-0.0.4rc8/gen3_tracker/gen3/buckets/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1323 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/gen3/buckets/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      883 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc8/gen3_tracker/gen3/buckets/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      559 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc8/gen3_tracker/gen3/buckets/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3397 2024-05-24 15:55:29.000000 gen3_tracker-0.0.4rc8/gen3_tracker/gen3/indexd.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6201 2024-05-15 20:04:35.000000 gen3_tracker-0.0.4rc8/gen3_tracker/gen3/jobs.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-25 13:55:30.284504 gen3_tracker-0.0.4rc8/gen3_tracker/git/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    24217 2024-05-25 12:16:14.000000 gen3_tracker-0.0.4rc8/gen3_tracker/git/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    11639 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/git/adder.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    38140 2024-05-25 13:22:14.000000 gen3_tracker-0.0.4rc8/gen3_tracker/git/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3026 2024-05-16 13:45:52.000000 gen3_tracker-0.0.4rc8/gen3_tracker/git/cloner.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1466 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/git/initializer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2609 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/git/snapshotter.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-25 13:55:30.288811 gen3_tracker-0.0.4rc8/gen3_tracker/meta/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5924 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/meta/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5107 2024-05-23 14:56:48.000000 gen3_tracker-0.0.4rc8/gen3_tracker/meta/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    24571 2024-05-25 13:20:26.000000 gen3_tracker-0.0.4rc8/gen3_tracker/meta/dataframer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    13227 2024-05-25 13:24:36.000000 gen3_tracker-0.0.4rc8/gen3_tracker/meta/skeleton.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4428 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/meta/validator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1211 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/meta/visualizer.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-25 13:55:30.304031 gen3_tracker-0.0.4rc8/gen3_tracker/projects/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2781 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/projects/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4799 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/projects/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2411 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/projects/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1566 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc8/gen3_tracker/projects/remover.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-25 13:55:30.254733 gen3_tracker-0.0.4rc8/gen3_tracker.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2371 2024-05-25 13:55:30.000000 gen3_tracker-0.0.4rc8/gen3_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1857 2024-05-25 13:55:30.000000 gen3_tracker-0.0.4rc8/gen3_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2024-05-25 13:55:30.000000 gen3_tracker-0.0.4rc8/gen3_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       45 2024-05-25 13:55:30.000000 gen3_tracker-0.0.4rc8/gen3_tracker.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      209 2024-05-25 13:55:30.000000 gen3_tracker-0.0.4rc8/gen3_tracker.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       13 2024-05-25 13:55:30.000000 gen3_tracker-0.0.4rc8/gen3_tracker.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2024-05-25 13:55:30.329355 gen3_tracker-0.0.4rc8/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142      912 2024-05-25 13:55:13.000000 gen3_tracker-0.0.4rc8/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-25 13:55:30.312730 gen3_tracker-0.0.4rc8/tests/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-04-16 13:21:28.000000 gen3_tracker-0.0.4rc8/tests/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-25 13:55:30.315819 gen3_tracker-0.0.4rc8/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2307 2024-05-15 03:31:16.000000 gen3_tracker-0.0.4rc8/tests/integration/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      470 2024-05-05 15:05:17.000000 gen3_tracker-0.0.4rc8/tests/integration/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3388 2024-05-16 02:28:15.000000 gen3_tracker-0.0.4rc8/tests/integration/test_bucket_import.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3428 2024-05-25 13:20:26.000000 gen3_tracker-0.0.4rc8/tests/integration/test_bundle.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3949 2024-05-25 13:20:26.000000 gen3_tracker-0.0.4rc8/tests/integration/test_end_to_end_workflow.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-25 13:55:30.326362 gen3_tracker-0.0.4rc8/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-05-02 22:49:35.000000 gen3_tracker-0.0.4rc8/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    20363 2024-05-01 22:45:46.000000 gen3_tracker-0.0.4rc8/tests/unit/test_flatten_fhir_example.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2024-05-15 03:31:16.000000 gen3_tracker-0.0.4rc8/tests/unit/test_hash_types.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      601 2024-05-15 03:31:16.000000 gen3_tracker-0.0.4rc8/tests/unit/test_read_dvc.py
```

### Comparing `gen3_tracker-0.0.4rc7/LICENSE` & `gen3_tracker-0.0.4rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/PKG-INFO` & `gen3_tracker-0.0.4rc8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_tracker
-Version: 0.0.4rc7
+Version: 0.0.4rc8
 Summary: A CLI for adding version control to Gen3 data submission projects.
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: walsbr
 Author-email: walsbr@ohsu.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `gen3_tracker-0.0.4rc7/README.md` & `gen3_tracker-0.0.4rc8/README.md`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/__init__.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/cli.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/access/__init__.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/access/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/access/cli.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/access/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/access/requestor.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/access/requestor.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/access/submitter.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/access/submitter.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/collaborator/cli.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/collaborator/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/common/__init__.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/common/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/config/__init__.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/gen3/buckets/__init__.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/gen3/buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/gen3/buckets/cli.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/gen3/buckets/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/gen3/buckets/lister.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/gen3/buckets/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/gen3/indexd.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/gen3/indexd.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,17 @@
             raise e
     return True
 
 
 def create_hashes_metadata(dvc: DVC, program, project):
     meta: DVCMeta = dvc.meta
 
+    if not meta:
+        meta = DVCMeta()
+
     hashes = {dvc.out.hash: getattr(dvc.out, dvc.out.hash)}
     metadata = {
         **{
             'document_reference_id': dvc.object_id,
             'specimen_identifier': meta.specimen,
             'patient_identifier': meta.patient,
             'task_identifier': meta.task,
```

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/gen3/jobs.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/gen3/jobs.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/git/__init__.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/git/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import typing
 import uuid
 import zipfile
 from abc import abstractmethod
 from datetime import datetime
 from typing import NamedTuple
 
+import inflection
 import pydantic
 import pytz
 import yaml
 from fhir.resources.attachment import Attachment
 from gen3.auth import Gen3Auth
 from pydantic import BaseModel, ConfigDict, field_validator
 
@@ -159,29 +160,43 @@
             document_reference (DocumentReference): loaded DocumentReferences
             references (dict): cross ref of Reference to Identifiers
 
         """
         attachment: Attachment = document_reference.content[0].attachment
         assert attachment.extension, document_reference
         source_path = [_.valueUrl for _ in attachment.extension if _.url.endswith('source_path')][0]
-        md5 = [_.valueString for _ in attachment.extension if _.url.endswith('md5')][0]
+
+        for k in ACCEPTABLE_HASHES.keys():
+            if [_.valueString for _ in attachment.extension if _.url.endswith(k)]:
+                hash_value = [_.valueString for _ in attachment.extension if _.url.endswith(k)][0]
+                hash_name = k
+                break
+
         assert source_path, document_reference
-        assert md5, document_reference
+        assert hash_value, document_reference
+
+        resource_type, resource_id = document_reference.subject.reference.split('/')
+        meta = DVCMeta()
+        if not resource_type == 'ResearchStudy':
+            resource_type = inflection.underscore(resource_type)
+            identifier = references[document_reference.subject.reference]
+            meta = DVCMeta(**{resource_type: identifier})
+
         dvc_object = DVC(
             project_id=config.gen3.project_id,
+            meta=meta,
             outs=[
                 DVCItem(
                     modified=attachment.creation.isoformat(),
                     path=attachment.url.replace('file:///', ''),
                     size=attachment.size,
                     realpath=source_path.replace('file:///', ''),
                     mime=attachment.contentType,
-                    md5=md5,
-                    hash='md5',
-                    object_id=document_reference.id
+                    object_id=document_reference.id,
+                    **{hash_name: hash_value, 'hash': hash_name}
                 )
             ],
         )
         if document_reference.subject:
 
             if document_reference.subject.reference in references:
                 key = document_reference.subject.reference.split('/')[0]
@@ -563,24 +578,28 @@
         current_time = datetime.now().strftime("%Y%m%d%H%M%S")  # Format datetime as you need
         manifest_file = pathlib.Path(work_dir) / f'manifest-{current_time}.json'
         manifest_file.parent.mkdir(parents=True, exist_ok=True)
         self.manifest_file_path = manifest_file
         self.manifest = []
 
     def save(self, dvc: DVC) -> str:
-        self.logger.info(f'Saving to {self.remote} {dvc}')
-        self.manifest.append(to_manifest(dvc))
+        if dvc.out.realpath:
+            self.logger.info(f'Saving to {self.remote} {dvc}')
+            self.manifest.append(to_manifest(dvc))
         return 'OK'
 
     def commit(self, dry_run=False, profile=None, upload_path=None, bucket_name=None, worker_count=(multiprocessing.cpu_count() - 1)):
         with open(self.manifest_file_path, 'w') as f:
             json.dump(self.manifest, f)
-        cmd = f"gen3-client upload-multiple --manifest {self.manifest_file_path} --profile {profile} --upload-path {upload_path} --bucket {bucket_name} --numparallel {worker_count}"
-        print(cmd)
-        run_command(cmd, dry_run=dry_run, raise_on_err=True, no_capture=True)
+        if len(self.manifest) > 0:
+            cmd = f"gen3-client upload-multiple --manifest {self.manifest_file_path} --profile {profile} --upload-path {upload_path} --bucket {bucket_name} --numparallel {worker_count}"
+            print(cmd)
+            run_command(cmd, dry_run=dry_run, raise_on_err=True, no_capture=True)
+        else:
+            print(f'No files to upload to {self.remote} by gen3-client.')
         return 'OK'
 
 
 def to_indexd(dvc_objects: list[DVC],
               auth: Gen3Auth,
               project_id: str,
               bucket_name: str,
```

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/git/adder.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/git/adder.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/git/cli.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/git/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,17 @@
         click.secho(str(e), fg=ERROR_COLOR, file=sys.stderr)
         if config.debug:
             raise
 
 
 def ensure_git_repo(config):
     # ensure a git repo
+    if pathlib.Path('.git').exists():
+        return
+
     if not pathlib.Path('.git').exists():
         command = 'git init'
         run_command(command, dry_run=config.dry_run, no_capture=True)
     else:
         click.secho('Git repository already exists.', fg=INFO_COLOR, file=sys.stderr)
     pathlib.Path('MANIFEST').mkdir(exist_ok=True)
     pathlib.Path('META').mkdir(exist_ok=True)
@@ -146,16 +149,17 @@
 #     ignore_unknown_options=True,
 #     allow_extra_args=True,
 # )
 
 
 @cli.command(context_settings=dict(ignore_unknown_options=True, allow_extra_args=True))
 @click.argument('target')
+@click.option('--no-git-add', default=False, is_flag=True, help="Do not automatically add the file to git.  I'll add it manually." )
 @click.pass_context
-def add(ctx, target):
+def add(ctx, target, no_git_add: bool):
     """
     Update references to data files to the repository.
 
     \b
     TARGET is a "data file", either files or urls.
     We commit their proxies - MANIFEST/<TARGET>.dvc files.
     \b
@@ -202,15 +206,15 @@
         else:
             all_changed_files, updates = add_file(ctx, target)
 
         #
         # if it is an update, we do not need to add the file to git
         #
         adds = [str(_) for _ in all_changed_files if _ not in updates]
-        if adds:
+        if adds and not no_git_add:
             adds.append('.gitignore')
             run_command(f'git add {" ".join([str(_) for _ in adds])}', dry_run=config.dry_run, no_capture=True)
 
     except Exception as e:
         click.secho(str(e), fg=ERROR_COLOR, file=sys.stderr)
         if config.debug:
             raise
@@ -400,15 +404,15 @@
                     ),
                     desc='Indexing', unit='file', leave=False, total=len(committed_files)):
                 pass
             click.secho(f'Indexed {len(committed_files)} files.', fg=INFO_COLOR, file=sys.stderr)
 
         if step in ['upload', 'all']:
 
-            click.secho(f'Uploading {len(dvc_objects)} files via {transfer_method}', fg=INFO_COLOR, file=sys.stderr)
+            click.secho(f'Checking {len(dvc_objects)} files for upload via {transfer_method}', fg=INFO_COLOR, file=sys.stderr)
             to_remote(
                 upload_method=transfer_method,
                 dvc_objects=dvc_objects,
                 bucket_name=bucket_name,
                 profile=config.gen3.profile,
                 dry_run=config.dry_run,
                 work_dir=config.work_dir
```

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/git/cloner.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/git/cloner.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/git/initializer.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/git/initializer.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/git/snapshotter.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/git/snapshotter.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/meta/__init__.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/meta/cli.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/meta/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/meta/dataframer.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/meta/dataframer.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,15 +452,15 @@
     db_path = (work_path / "local_fhir.db")
     db_path.unlink(missing_ok=True)
 
     db = LocalFHIRDatabase(db_name=db_path)
     db.load_ndjson_from_dir(path=directory_path)
 
     if data_type == "DocumentReference":
-        df = pd.DataFrame(db.flattened_document_reference())
+        df = pd.DataFrame(db.flattened_document_references())
     elif data_type == "Observation":
         df = pd.DataFrame(db.flattened_observations())
     else:
         raise ValueError(f"{data_type} not supported yet. Supported data types are DocumentReference and Observation")
     assert not df.empty, "Dataframe is empty, are there any DocumentReference resources?"
 
     front_column_names = ["resourceType", "identifier"]
```

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/meta/skeleton.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/meta/skeleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     for file in meta_dir.glob('*.ndjson'):
         with open(file, 'r') as f:
             for line in f:
                 record = orjson.loads(line)
                 _id = record.get('id')
                 resource_type = record.get('resourceType')
                 if resource_type == 'Bundle':
-                    continue
+                    break
                 official_identifier = next((identifier.get('value') for identifier in record.get('identifier', []) if identifier.get('use') == 'official'), None)
                 if not official_identifier and record.get('identifier'):
                     official_identifier = record['identifier'][0]['value']
 
                 if _id and official_identifier:
                     id_dict[f"{resource_type}/{_id}"] = official_identifier
 
@@ -94,17 +94,14 @@
     document_reference.content = [content]
 
 
 def create_id_from_strings(resource_type: str, project_id: str, identifier_string: str) -> str:
     """Create an id from strings."""
     if not identifier_string:
         return None
-    # cbds-smmart_labkey_demo/Specimen/https://aced-idp.org/cbds-smmart_labkey_demo|0000321955
-    # cbds-smmart_labkey_demo/Specimen/https://aced-idp.org/cbds-smmart_labkey_demo|0000321955
-    print(f"{project_id}/{resource_type}/{_get_system(identifier_string, project_id)}|{identifier_string}")
     return str(uuid.uuid5(ACED_NAMESPACE, f"{project_id}/{resource_type}/{_get_system(identifier_string, project_id)}|{identifier_string}"))
 
 
 def create_skeleton(dvc: dict, project_id: str, meta_index: set[str] = []) -> list[Resource]:
     """
     Create a skeleton graph for document and ancestors from a set of identifiers.
     """
@@ -185,16 +182,19 @@
         observation.id = create_id(observation, project_id)
 
         assert patient, "patient required for observation"
         observation.subject = {'reference': f"Patient/{patient.id}"}
         patient_id = patient.id
 
     if not specimen and specimen_identifier:
-        print(f'{specimen_identifier} Specimen/{specimen_id} not in {[(k, _) for k, _ in meta_index.items() if k.startswith("Specimen")]}')
-        exit(1)
+
+        # TODO:?
+        # print(f'{specimen_identifier} Specimen/{specimen_id} not in {[(k, _) for k, _ in meta_index.items() if k.startswith("Specimen")]}')
+        # exit(1)
+
         specimen = Specimen()
         specimen.identifier = [Identifier(value=specimen_identifier, system=_get_system(specimen_identifier, project_id=project_id), use='official')]
         specimen.id = create_id(specimen, project_id)
         specimen_id = specimen.id
 
         assert patient, "patient required for specimen"
         specimen.subject = {'reference': f"Patient/{patient.id}"}
@@ -256,51 +256,51 @@
     dvc_files = [_ for _ in manifest_path.rglob('*.dvc')]
 
     if not dvc_files:
         return []
 
     before_meta_files = [_ for _ in pathlib.Path('META').glob('*.ndjson')]
     before_meta_index = set(list(meta_index().keys()))
-
     emitted_already = []
 
     with EmitterContextManager('META') as emitter:
         for _ in dvc_data(dvc_files):
             resources = create_skeleton(_, project_id, meta_index())
             for resource in resources:
                 key = f"{resource.resource_type}/{resource.id}"
                 if key not in emitted_already:
                     emitter.emit(resource.resource_type).write(
                         resource.json(option=orjson.OPT_APPEND_NEWLINE)
                     )
-                    emitted_already.append(f"{resource.resource_type}/{resource.id}")
+                    emitted_already.append(key)
+
+    after_meta_index = set(list(meta_index().keys()))
+    orphaned_meta_index = before_meta_index - after_meta_index
 
-        after_meta_index = set(emitted_already)
+    if orphaned_meta_index:
+        # create a bundle to tell server about deletes
+        now = datetime.now(UTC).strftime("%Y-%m-%dT%H:%M:%S.%fZ")
+        bundle = Bundle(type='transaction', timestamp=now)
 
-        orphaned_meta_index = before_meta_index - after_meta_index
-        if orphaned_meta_index:
-            # create a bundle to tell server about deletes
-            now = datetime.now(UTC).strftime("%Y-%m-%dT%H:%M:%S.%fZ")
-            bundle = Bundle(type='transaction', timestamp=now)
-
-            bundle.identifier = Identifier(value=now, system=_get_system(project_id, project_id=project_id), use='official')
-            bundle.id = create_id(bundle, project_id)
-
-            bundle.entry = []
-            outcome = OperationOutcome(issue=[{'severity': 'warning', 'code': 'processing', 'diagnostics': 'Meta data items no longer in study.'}])
-            bundle.issues = outcome
-
-            for _ in orphaned_meta_index:
-                bundle_entry = BundleEntry()
-                bundle_entry.request = BundleEntryRequest(url=_, method='DELETE')
-                bundle.entry.append(bundle_entry)
+        bundle.identifier = Identifier(value=now, system=_get_system(project_id, project_id=project_id), use='official')
+        bundle.id = create_id(bundle, project_id)
 
+        bundle.entry = []
+        outcome = OperationOutcome(issue=[{'severity': 'warning', 'code': 'processing', 'diagnostics': 'Meta data items no longer in study.'}])
+        bundle.issues = outcome
+
+        for _ in orphaned_meta_index:
+            bundle_entry = BundleEntry()
+            bundle_entry.request = BundleEntryRequest(url=_, method='DELETE')
+            bundle.entry.append(bundle_entry)
+
+        with EmitterContextManager('META') as emitter:
             emitter.emit(bundle.resource_type, file_mode='a').write(
-                        bundle.json(option=orjson.OPT_APPEND_NEWLINE)
-                    )
+                    bundle.json(option=orjson.OPT_APPEND_NEWLINE)
+                )
 
     after_meta_files = [_ for _ in pathlib.Path('META').glob('*.ndjson')]
     new_meta_files = [str(_) for _ in after_meta_files if _ not in before_meta_files]
 
     if new_meta_files:
         run_command(f'git add {" ".join(new_meta_files)}', dry_run=dry_run, no_capture=True)
```

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/meta/validator.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/meta/validator.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/meta/visualizer.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/meta/visualizer.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/projects/__init__.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/projects/cli.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/projects/lister.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/projects/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker/projects/remover.py` & `gen3_tracker-0.0.4rc8/gen3_tracker/projects/remover.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker.egg-info/PKG-INFO` & `gen3_tracker-0.0.4rc8/gen3_tracker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3-tracker
-Version: 0.0.4rc7
+Version: 0.0.4rc8
 Summary: A CLI for adding version control to Gen3 data submission projects.
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: walsbr
 Author-email: walsbr@ohsu.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `gen3_tracker-0.0.4rc7/gen3_tracker.egg-info/SOURCES.txt` & `gen3_tracker-0.0.4rc8/gen3_tracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/setup.py` & `gen3_tracker-0.0.4rc8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 
 setup(
     name='gen3_tracker',
-    version='0.0.4rc7',
+    version='0.0.4rc8',
     description='A CLI for adding version control to Gen3 data submission projects.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='walsbr',
     author_email='walsbr@ohsu.edu',
     url='https://github.com/ACED-IDP/gen3_util',
     packages=find_packages(exclude=['tests', 'tests.*']),
```

### Comparing `gen3_tracker-0.0.4rc7/tests/integration/__init__.py` & `gen3_tracker-0.0.4rc8/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/tests/integration/test_bucket_import.py` & `gen3_tracker-0.0.4rc8/tests/integration/test_bucket_import.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/tests/integration/test_bundle.py` & `gen3_tracker-0.0.4rc8/tests/integration/test_bundle.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     run(runner, ["--debug", "init", project_id, "--approve", "--no-server"],
         expected_files=[".g3t", ".git"])
 
     for _ in CHANGE_PATIENT:
         run(runner, _.split())
 
     for _ in read_ndjson_file(pathlib.Path("META/Bundle.ndjson")):
+        print(_)
         bundle = Bundle(**_)
         break  # only one bundle
 
     assert len(bundle.entry) == 2, "Only two entries are expected."
 
     methods = [_.request.method for _ in bundle.entry]
     assert all([_ == "DELETE" for _ in methods]), "Only DELETE method is expected."
@@ -71,14 +72,15 @@
     run(runner, ["--debug", "init", project_id, "--approve", "--no-server"],
         expected_files=[".g3t", ".git"])
 
     for _ in CHANGE_FILE:
         run(runner, _.split())
 
     for _ in read_ndjson_file(pathlib.Path("META/Bundle.ndjson")):
+        print(_)
         bundle = Bundle(**_)
         break  # only one bundle
 
     assert len(bundle.entry) == 1, "Only one entry is expected."
 
     methods = [_.request.method for _ in bundle.entry]
     assert all([_ == "DELETE" for _ in methods]), "Only DELETE method is expected."
```

### Comparing `gen3_tracker-0.0.4rc7/tests/integration/test_end_to_end_workflow.py` & `gen3_tracker-0.0.4rc8/tests/integration/test_end_to_end_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     # validate the meta files
     run(runner, ["--debug", "meta", "validate"])
 
     # create a visualisation
     run(runner, ["--debug", "meta", "graph"], expected_files=["meta.html"])
 
     # create a dataframe
-    run(runner,  ["--debug", "meta", "dataframe"], expected_files=["meta.csv"])
+    run(runner,  ["--debug", "meta", "dataframe", '--data_type', 'DocumentReference'], expected_files=["meta.csv"])
 
     # push to the server
     run(runner, ["--debug", "push"])
 
     # list the files from indexd
     run(runner, ["--debug", "ls"], expected_output=["my-project-data/hello.txt"])
```

### Comparing `gen3_tracker-0.0.4rc7/tests/unit/test_flatten_fhir_example.py` & `gen3_tracker-0.0.4rc8/tests/unit/test_flatten_fhir_example.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/tests/unit/test_hash_types.py` & `gen3_tracker-0.0.4rc8/tests/unit/test_hash_types.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc7/tests/unit/test_read_dvc.py` & `gen3_tracker-0.0.4rc8/tests/unit/test_read_dvc.py`

 * *Files identical despite different names*

