# Comparing `tmp/kingsoftcloud_sdk_python-1.4.2.tar.gz` & `tmp/kingsoftcloud_sdk_python-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingsoftcloud_sdk_python-1.4.2.tar", last modified: Wed May 22 12:24:56 2024, max compression
+gzip compressed data, was "kingsoftcloud_sdk_python-1.4.3.tar", last modified: Mon May 27 07:54:27 2024, max compression
```

## Comparing `kingsoftcloud_sdk_python-1.4.2.tar` & `kingsoftcloud_sdk_python-1.4.3.tar`

### file list

```diff
@@ -1,324 +1,324 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.359630 kingsoftcloud_sdk_python-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-22 12:24:56.359630 kingsoftcloud_sdk_python-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.359630 kingsoftcloud_sdk_python-1.4.2/kingsoftcloud_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-22 12:24:56.000000 kingsoftcloud_sdk_python-1.4.2/kingsoftcloud_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-22 12:24:56.000000 kingsoftcloud_sdk_python-1.4.2/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:24:56.000000 kingsoftcloud_sdk_python-1.4.2/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 12:24:56.000000 kingsoftcloud_sdk_python-1.4.2/kingsoftcloud_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 12:24:56.000000 kingsoftcloud_sdk_python-1.4.2/kingsoftcloud_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.323629 kingsoftcloud_sdk_python-1.4.2/ksyun/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.323629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.323629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/actiontrail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/actiontrail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.323629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/actiontrail/v20190401/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/actiontrail/v20190401/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/actiontrail/v20190401/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/actiontrail/v20190401/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.323629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.323629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill/v20180601/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill/v20180601/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill/v20180601/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill/v20180601/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.323629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill/v20220601/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill/v20220601/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill/v20220601/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill/v20220601/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.323629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill_union/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill_union/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.327629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill_union/v20200101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill_union/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill_union/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill_union/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.327629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill_union/v20221222/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill_union/v20221222/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill_union/v20221222/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill_union/v20221222/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.327629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.327629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bws/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bws/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bws/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/bws/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.327629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.327629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20160901/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20160901/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20160901/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20160901/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.327629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20200630/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20200630/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16144 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20200630/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    49120 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20200630/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.327629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20200901/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20200901/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20200901/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20200901/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.327629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.327629 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cen/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cen/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22637 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cen/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20416 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/cen/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.331630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/clickhouse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.331630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/clickhouse/v20210101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/clickhouse/v20210101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26444 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/clickhouse/v20210101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28090 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/clickhouse/v20210101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.331630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.331630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/client/kcm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/client/kcm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.331630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/client/kcm/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/client/kcm/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/client/kcm/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/client/kcm/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.331630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/ebs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/ebs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.331630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/ebs/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/ebs/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17254 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/ebs/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21354 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/ebs/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.331630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/eip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/eip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.331630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/eip/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/eip/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/eip/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/eip/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.331630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/epc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/epc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.331630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/epc/v20151101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/epc/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52345 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/epc/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    61057 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/epc/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.331630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/iam/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/iam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.335630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/iam/v20151101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/iam/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57177 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/iam/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    47991 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/iam/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.335630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/iam/v20240513/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/iam/v20240513/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/iam/v20240513/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/iam/v20240513/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.335630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kad/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.335630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kad/v20161122/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kad/v20161122/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kad/v20161122/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kad/v20161122/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.335630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.335630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20180314/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20180314/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20180314/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20180314/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.335630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20190806/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20190806/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22732 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20190806/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28316 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20190806/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.335630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20201231/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20201231/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20201231/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20201231/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.335630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20230306/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20230306/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16375 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20230306/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20230306/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.335630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.339630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcm/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcm/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcm/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcm/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.339630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcrs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcrs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.339630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcrs/v20211109/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcrs/v20211109/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43427 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcrs/v20211109/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    38868 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcrs/v20211109/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.339630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.339630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcs/v20160701/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcs/v20160701/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53844 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcs/v20160701/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    64686 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcs/v20160701/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.339630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcs/v20170401/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcs/v20170401/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcs/v20170401/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcs/v20170401/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.339630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kead/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kead/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.339630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kead/v20200101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kead/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kead/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kead/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.339630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.339630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kec/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kec/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    90642 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kec/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   135161 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kec/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.339630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/ket/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/ket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.343630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/ket/v20170101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/ket/v20170101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/ket/v20170101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/ket/v20170101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.343630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kingpay/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kingpay/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.343630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kingpay/v20240501/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kingpay/v20240501/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kingpay/v20240501/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kingpay/v20240501/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.343630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kkms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kkms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.343630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kkms/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kkms/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kkms/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kkms/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.343630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/klog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/klog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.343630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/klog/v20200731/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/klog/v20200731/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40650 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/klog/v20200731/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    33045 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/klog/v20200731/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.343630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.343630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kls/v20170101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kls/v20170101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kls/v20170101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/kls/v20170101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.343630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/krds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/krds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.343630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/krds/v20160701/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/krds/v20160701/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63636 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/krds/v20160701/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    82562 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/krds/v20160701/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.347630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/krds/v20200825/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/krds/v20200825/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/krds/v20200825/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10179 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/krds/v20200825/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.347630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/memcached/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/memcached/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.347630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/memcached/v20180627/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/memcached/v20180627/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/memcached/v20180627/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/memcached/v20180627/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.347630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/mongodb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/mongodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.347630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/mongodb/v20170101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/mongodb/v20170101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32999 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/mongodb/v20170101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    37675 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/mongodb/v20170101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.347630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.347630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20100525/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20100525/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20100525/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20100525/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.347630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20181114/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20181114/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20181114/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20181114/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.347630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20210101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20210101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8574 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20210101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20210101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.347630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20220101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20220101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20220101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20220101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.347630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/pdns/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/pdns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.351630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/pdns/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/pdns/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22951 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/pdns/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15869 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/pdns/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.351630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.351630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/rabbitmq/v20191017/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/rabbitmq/v20191017/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/rabbitmq/v20191017/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/rabbitmq/v20191017/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.351630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/resourcemanager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/resourcemanager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.351630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/resourcemanager/v20210320/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/resourcemanager/v20210320/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/resourcemanager/v20210320/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/resourcemanager/v20210320/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.351630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/sks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/sks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.351630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/sks/v20151101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/sks/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/sks/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/sks/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.351630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/slb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/slb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.351630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/slb/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/slb/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    69354 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/slb/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    92352 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/slb/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.351630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/sts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/sts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.351630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/sts/v20151101/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/sts/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/sts/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/sts/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.351630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/tagv2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/tagv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.351630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/tagv2/v20200901/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/tagv2/v20200901/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/tagv2/v20200901/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/tagv2/v20200901/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.355630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/tidb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/tidb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.355630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/tidb/v20210520/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/tidb/v20210520/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16604 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/tidb/v20210520/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19021 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/tidb/v20210520/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.355630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/trade/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/trade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.355630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/trade/v20200114/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/trade/v20200114/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/trade/v20200114/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/trade/v20200114/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.355630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/trade/v20200831/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/trade/v20200831/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/trade/v20200831/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/trade/v20200831/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.355630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/vpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/vpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.355630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/vpc/v20160304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/vpc/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    84131 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/vpc/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    84692 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/vpc/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.355630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/waf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/waf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.355630 kingsoftcloud_sdk_python-1.4.2/ksyun/client/waf/v20200707/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/waf/v20200707/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/waf/v20200707/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/client/waf/v20200707/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.355630 kingsoftcloud_sdk_python-1.4.2/ksyun/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.359630 kingsoftcloud_sdk_python-1.4.2/ksyun/common/exception/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/common/exception/ksyun_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.359630 kingsoftcloud_sdk_python-1.4.2/ksyun/common/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:56.359630 kingsoftcloud_sdk_python-1.4.2/ksyun/common/profile/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/ksyun/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-22 12:24:56.359630 kingsoftcloud_sdk_python-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-22 12:24:52.000000 kingsoftcloud_sdk_python-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.123412 kingsoftcloud_sdk_python-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-27 07:54:27.123412 kingsoftcloud_sdk_python-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.123412 kingsoftcloud_sdk_python-1.4.3/kingsoftcloud_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-27 07:54:27.000000 kingsoftcloud_sdk_python-1.4.3/kingsoftcloud_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-27 07:54:27.000000 kingsoftcloud_sdk_python-1.4.3/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:54:27.000000 kingsoftcloud_sdk_python-1.4.3/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-27 07:54:27.000000 kingsoftcloud_sdk_python-1.4.3/kingsoftcloud_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 07:54:27.000000 kingsoftcloud_sdk_python-1.4.3/kingsoftcloud_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.079412 kingsoftcloud_sdk_python-1.4.3/ksyun/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.079412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.079412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/actiontrail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/actiontrail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.079412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/actiontrail/v20190401/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/actiontrail/v20190401/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/actiontrail/v20190401/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/actiontrail/v20190401/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.079412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.079412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill/v20180601/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill/v20180601/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill/v20180601/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill/v20180601/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.083412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill/v20220601/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill/v20220601/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill/v20220601/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill/v20220601/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.083412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill_union/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill_union/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.083412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill_union/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill_union/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill_union/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill_union/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.083412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill_union/v20221222/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill_union/v20221222/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill_union/v20221222/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill_union/v20221222/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.083412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.083412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bws/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bws/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bws/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/bws/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.083412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.083412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20160901/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20160901/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20160901/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20160901/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.083412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20200630/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20200630/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16144 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20200630/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49120 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20200630/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.087412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20200901/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20200901/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20200901/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20200901/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.087412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.087412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cen/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cen/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22637 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cen/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20416 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/cen/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.087412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/clickhouse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.087412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/clickhouse/v20210101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/clickhouse/v20210101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26444 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/clickhouse/v20210101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28090 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/clickhouse/v20210101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.087412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.087412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/client/kcm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/client/kcm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.087412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/client/kcm/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/client/kcm/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/client/kcm/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/client/kcm/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.087412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/ebs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/ebs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.087412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/ebs/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/ebs/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17254 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/ebs/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21354 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/ebs/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.087412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/eip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/eip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.091412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/eip/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/eip/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/eip/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/eip/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.091412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/epc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/epc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.091412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/epc/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/epc/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52345 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/epc/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61057 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/epc/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.091412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/iam/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/iam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.091412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/iam/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/iam/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58096 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/iam/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48826 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/iam/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.091412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/iam/v20240513/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/iam/v20240513/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/iam/v20240513/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/iam/v20240513/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.091412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kad/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.091412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kad/v20161122/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kad/v20161122/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kad/v20161122/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kad/v20161122/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.091412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.095412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20180314/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20180314/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20180314/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20180314/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.095412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20190806/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20190806/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22732 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20190806/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28316 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20190806/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.095412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20201231/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20201231/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20201231/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20201231/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.095412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20230306/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20230306/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16375 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20230306/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20230306/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.095412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.095412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcm/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcm/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcm/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcm/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.095412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcrs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcrs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.095412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcrs/v20211109/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcrs/v20211109/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43427 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcrs/v20211109/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38868 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcrs/v20211109/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.095412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.099412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcs/v20160701/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcs/v20160701/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53844 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcs/v20160701/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64686 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcs/v20160701/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.099412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcs/v20170401/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcs/v20170401/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcs/v20170401/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcs/v20170401/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.099412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kead/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kead/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.099412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kead/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kead/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kead/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kead/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.099412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.099412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kec/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kec/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90642 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kec/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135161 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kec/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.099412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/ket/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/ket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.099412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/ket/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/ket/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/ket/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/ket/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.099412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kingpay/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kingpay/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.103412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kingpay/v20240501/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kingpay/v20240501/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kingpay/v20240501/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kingpay/v20240501/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.103412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kkms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kkms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.103412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kkms/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kkms/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kkms/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kkms/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.103412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/klog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/klog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.103412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/klog/v20200731/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/klog/v20200731/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40650 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/klog/v20200731/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33045 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/klog/v20200731/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.103412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.103412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kls/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kls/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kls/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/kls/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.103412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/krds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/krds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.103412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/krds/v20160701/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/krds/v20160701/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63636 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/krds/v20160701/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82562 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/krds/v20160701/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.107412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/krds/v20200825/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/krds/v20200825/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/krds/v20200825/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10179 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/krds/v20200825/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.107412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/memcached/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/memcached/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.107412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/memcached/v20180627/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/memcached/v20180627/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/memcached/v20180627/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/memcached/v20180627/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.107412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/mongodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.107412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/mongodb/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/mongodb/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32999 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/mongodb/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37675 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/mongodb/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.107412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.107412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20100525/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20100525/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20100525/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20100525/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.107412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20181114/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20181114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20181114/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20181114/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.107412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20210101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20210101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8574 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20210101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20210101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.111412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20220101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20220101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20220101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20220101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.111412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/pdns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/pdns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.111412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/pdns/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/pdns/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22951 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/pdns/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15869 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/pdns/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.111412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.111412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/rabbitmq/v20191017/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/rabbitmq/v20191017/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/rabbitmq/v20191017/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/rabbitmq/v20191017/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.111412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/resourcemanager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/resourcemanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.111412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/resourcemanager/v20210320/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/resourcemanager/v20210320/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/resourcemanager/v20210320/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/resourcemanager/v20210320/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.111412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/sks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/sks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.111412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/sks/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/sks/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/sks/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/sks/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.111412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/slb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/slb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.115412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/slb/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/slb/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79930 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/slb/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105818 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/slb/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.115412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/sts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/sts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.115412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/sts/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/sts/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/sts/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/sts/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.115412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/tagv2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/tagv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.115412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/tagv2/v20200901/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/tagv2/v20200901/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/tagv2/v20200901/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/tagv2/v20200901/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.115412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/tidb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/tidb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.115412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/tidb/v20210520/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/tidb/v20210520/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16604 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/tidb/v20210520/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19021 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/tidb/v20210520/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.115412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/trade/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/trade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.115412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/trade/v20200114/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/trade/v20200114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/trade/v20200114/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/trade/v20200114/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.115412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/trade/v20200831/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/trade/v20200831/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/trade/v20200831/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/trade/v20200831/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.115412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/vpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/vpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.119412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/vpc/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/vpc/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84131 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/vpc/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84692 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/vpc/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.119412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/waf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/waf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.119412 kingsoftcloud_sdk_python-1.4.3/ksyun/client/waf/v20200707/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/waf/v20200707/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/waf/v20200707/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14036 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/client/waf/v20200707/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.119412 kingsoftcloud_sdk_python-1.4.3/ksyun/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.119412 kingsoftcloud_sdk_python-1.4.3/ksyun/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/common/exception/ksyun_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.119412 kingsoftcloud_sdk_python-1.4.3/ksyun/common/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:27.119412 kingsoftcloud_sdk_python-1.4.3/ksyun/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/ksyun/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 07:54:27.123412 kingsoftcloud_sdk_python-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-27 07:54:21.000000 kingsoftcloud_sdk_python-1.4.3/setup.py
```

### Comparing `kingsoftcloud_sdk_python-1.4.2/LICENSE` & `kingsoftcloud_sdk_python-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/PKG-INFO` & `kingsoftcloud_sdk_python-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.4.2
+Version: 1.4.3
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kingsoftcloud_sdk_python-1.4.2/README.rst` & `kingsoftcloud_sdk_python-1.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/kingsoftcloud_sdk_python.egg-info/PKG-INFO` & `kingsoftcloud_sdk_python-1.4.3/kingsoftcloud_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.4.2
+Version: 1.4.3
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kingsoftcloud_sdk_python-1.4.2/kingsoftcloud_sdk_python.egg-info/SOURCES.txt` & `kingsoftcloud_sdk_python-1.4.3/kingsoftcloud_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/__init__.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '1.4.2'
+__version__ = '1.4.3'
```

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/actiontrail/v20190401/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/actiontrail/v20190401/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/actiontrail/v20190401/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/actiontrail/v20190401/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill/v20180601/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill/v20180601/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill/v20180601/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill/v20180601/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill/v20220601/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill/v20220601/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill/v20220601/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill/v20220601/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill_union/v20200101/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill_union/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill_union/v20200101/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill_union/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill_union/v20221222/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill_union/v20221222/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/bill_union/v20221222/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/bill_union/v20221222/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/bws/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/bws/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/bws/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/bws/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20160901/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20160901/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20200630/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20200630/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20200630/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20200630/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20200901/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20200901/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/cdn/v20200901/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/cdn/v20200901/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/cen/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/cen/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/cen/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/cen/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/clickhouse/v20210101/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/clickhouse/v20210101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/clickhouse/v20210101/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/clickhouse/v20210101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/client/kcm/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/client/kcm/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/client/kcm/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/client/kcm/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/ebs/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/ebs/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/ebs/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/ebs/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/eip/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/eip/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/eip/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/eip/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/epc/v20151101/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/epc/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/epc/v20151101/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/epc/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/iam/v20151101/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/iam/v20151101/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -855,14 +855,37 @@
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
 
 
+    def UpdateProjectInfo(self, request):
+        """更新项目信息
+        :param request: Request instance for UpdateProjectInfo.
+        :type request: :class:`ksyun.client.iam.v20151101.models.UpdateProjectInfoRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call_judge("UpdateProjectInfo", params, "application/x-www-form-urlencoded")
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
     def GetAccountAllProjectList(self, request):
         """获取主/子用户项目列表
         :param request: Request instance for GetAccountAllProjectList.
         :type request: :class:`ksyun.client.iam.v20151101.models.GetAccountAllProjectListRequest`
         """
         try:
             params = request._serialize()
```

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/iam/v20151101/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/iam/v20151101/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -904,14 +904,40 @@
     def _deserialize(self, params):
         if params.get("ProjectName"):
             self.ProjectName = params.get("ProjectName")
         if params.get("ProjectDesc"):
             self.ProjectDesc = params.get("ProjectDesc")
 
 
+class UpdateProjectInfoRequest(AbstractModel):
+    """UpdateProjectInfo请求参数结构体
+    """
+
+    def __init__(self):
+        r"""更新项目信息
+        :param ProjectId: ProjectId
+        :type PathPrefix: Int
+        :param ProjectName: 项目名称，最多64个字符
+        :type PathPrefix: String
+        :param ProjectDesc: 项目描述，最多64个字符
+        :type PathPrefix: String
+        """
+        self.ProjectId = None
+        self.ProjectName = None
+        self.ProjectDesc = None
+
+    def _deserialize(self, params):
+        if params.get("ProjectId"):
+            self.ProjectId = params.get("ProjectId")
+        if params.get("ProjectName"):
+            self.ProjectName = params.get("ProjectName")
+        if params.get("ProjectDesc"):
+            self.ProjectDesc = params.get("ProjectDesc")
+
+
 class GetAccountAllProjectListRequest(AbstractModel):
     """GetAccountAllProjectList请求参数结构体
     """
 
     def __init__(self):
         r"""获取主/子用户项目列表
         """
```

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/iam/v20240513/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/iam/v20240513/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/iam/v20240513/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/iam/v20240513/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kad/v20161122/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kad/v20161122/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kad/v20161122/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kad/v20161122/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20180314/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20180314/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20180314/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20180314/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20190806/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20190806/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20190806/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20190806/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20201231/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20201231/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20201231/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20201231/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20230306/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20230306/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kce/v20230306/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kce/v20230306/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcm/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcm/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcm/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcm/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcrs/v20211109/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcrs/v20211109/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcrs/v20211109/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcrs/v20211109/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcs/v20160701/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcs/v20160701/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcs/v20160701/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcs/v20160701/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcs/v20170401/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcs/v20170401/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kcs/v20170401/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kcs/v20170401/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kead/v20200101/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kead/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kead/v20200101/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kead/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kec/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kec/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kec/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kec/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/ket/v20170101/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/ket/v20170101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/ket/v20170101/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/ket/v20170101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kingpay/v20240501/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kingpay/v20240501/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kkms/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kkms/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kkms/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kkms/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/klog/v20200731/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/klog/v20200731/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/klog/v20200731/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/klog/v20200731/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kls/v20170101/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kls/v20170101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/kls/v20170101/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/kls/v20170101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/krds/v20160701/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/krds/v20160701/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/krds/v20160701/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/krds/v20160701/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/krds/v20200825/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/krds/v20200825/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/krds/v20200825/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/krds/v20200825/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/memcached/v20180627/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/memcached/v20180627/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/memcached/v20180627/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/memcached/v20180627/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/mongodb/v20170101/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/mongodb/v20170101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/mongodb/v20170101/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/mongodb/v20170101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20100525/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20100525/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20100525/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20100525/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20181114/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20181114/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20181114/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20181114/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20210101/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20210101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20210101/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20210101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20220101/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20220101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/monitor/v20220101/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/monitor/v20220101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/pdns/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/pdns/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/pdns/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/pdns/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/rabbitmq/v20191017/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/rabbitmq/v20191017/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/rabbitmq/v20191017/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/rabbitmq/v20191017/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/resourcemanager/v20210320/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/resourcemanager/v20210320/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/resourcemanager/v20210320/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/resourcemanager/v20210320/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/sks/v20151101/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/sks/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/sks/v20151101/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/sks/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/slb/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/slb/v20160304/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -649,15 +649,15 @@
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
 
 
     def DescribeBackendServers(self, request):
-        """获取后端服务器列表
+        """查询服务器组中后端服务信息
         :param request: Request instance for DescribeBackendServers.
         :type request: :class:`ksyun.client.slb.v20160304.models.DescribeBackendServersRequest`
         """
         try:
             params = request._serialize()
             body = self.call_judge("DescribeBackendServers", params, "application/x-www-form-urlencoded")
             response = json.loads(body)
@@ -1698,14 +1698,267 @@
             response = json.loads(body)
             if "Error" not in response:
                 return body
             else:
                 code = response["Error"]["Code"]
                 message = response["Error"]["Message"]
                 req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def SetLBDeleteProtection(self, request):
+        """设置删除保护
+        :param request: Request instance for SetLBDeleteProtection.
+        :type request: :class:`ksyun.client.slb.v20160304.models.SetLBDeleteProtectionRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call_judge("SetLBDeleteProtection", params, "application/x-www-form-urlencoded")
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def SetLBModificationProtection(self, request):
+        """设置修改保护
+        :param request: Request instance for SetLBModificationProtection.
+        :type request: :class:`ksyun.client.slb.v20160304.models.SetLBModificationProtectionRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call_judge("SetLBModificationProtection", params, "application/x-www-form-urlencoded")
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def ModifyCertificateWithGroup(self, request):
+        """监听器维度更换同域名的证书
+        :param request: Request instance for ModifyCertificateWithGroup.
+        :type request: :class:`ksyun.client.slb.v20160304.models.ModifyCertificateWithGroupRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call_judge("ModifyCertificateWithGroup", params, "application/x-www-form-urlencoded")
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def CreateAlbBackendServerGroup(self, request):
+        """创建ALB服务器组
+        :param request: Request instance for CreateAlbBackendServerGroup.
+        :type request: :class:`ksyun.client.slb.v20160304.models.CreateAlbBackendServerGroupRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call_judge("CreateAlbBackendServerGroup", params, "application/x-www-form-urlencoded")
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def DeleteAlbBackendServerGroup(self, request):
+        """删除ALB服务器组
+        :param request: Request instance for DeleteAlbBackendServerGroup.
+        :type request: :class:`ksyun.client.slb.v20160304.models.DeleteAlbBackendServerGroupRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call_judge("DeleteAlbBackendServerGroup", params, "application/x-www-form-urlencoded")
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def ModifyAlbBackendServerGroup(self, request):
+        """修改ALB服务器组
+        :param request: Request instance for ModifyAlbBackendServerGroup.
+        :type request: :class:`ksyun.client.slb.v20160304.models.ModifyAlbBackendServerGroupRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call_judge("ModifyAlbBackendServerGroup", params, "application/x-www-form-urlencoded")
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def DescribeAlbBackendServerGroups(self, request):
+        """查询ALB服务器组
+        :param request: Request instance for DescribeAlbBackendServerGroups.
+        :type request: :class:`ksyun.client.slb.v20160304.models.DescribeAlbBackendServerGroupsRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call_judge("DescribeAlbBackendServerGroups", params, "application/x-www-form-urlencoded")
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def RegisterAlbBackendServer(self, request):
+        """ALB注册服务器到服务器组
+        :param request: Request instance for RegisterAlbBackendServer.
+        :type request: :class:`ksyun.client.slb.v20160304.models.RegisterAlbBackendServerRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call_judge("RegisterAlbBackendServer", params, "application/x-www-form-urlencoded")
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def DeregisterAlbBackendServer(self, request):
+        """ALB从服务器组移除服务器
+        :param request: Request instance for DeregisterAlbBackendServer.
+        :type request: :class:`ksyun.client.slb.v20160304.models.DeregisterAlbBackendServerRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call_judge("DeregisterAlbBackendServer", params, "application/x-www-form-urlencoded")
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def ModifyAlbBackendServer(self, request):
+        """修改ALB服务器信息
+        :param request: Request instance for ModifyAlbBackendServer.
+        :type request: :class:`ksyun.client.slb.v20160304.models.ModifyAlbBackendServerRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call_judge("ModifyAlbBackendServer", params, "application/x-www-form-urlencoded")
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
+                raise KsyunSDKException(code, message, req_id)
+        except Exception as e:
+            if isinstance(e, KsyunSDKException):
+                raise
+            else:
+                raise KsyunSDKException(e.message, e.message)
+
+
+    def DescribeAlbBackendServers(self, request):
+        """查询ALB服务器信息
+        :param request: Request instance for DescribeAlbBackendServers.
+        :type request: :class:`ksyun.client.slb.v20160304.models.DescribeAlbBackendServersRequest`
+        """
+        try:
+            params = request._serialize()
+            body = self.call_judge("DescribeAlbBackendServers", params, "application/x-www-form-urlencoded")
+            response = json.loads(body)
+            if "Error" not in response:
+                return body
+            else:
+                code = response["Error"]["Code"]
+                message = response["Error"]["Message"]
+                req_id = response["RequestId"]
                 raise KsyunSDKException(code, message, req_id)
         except Exception as e:
             if isinstance(e, KsyunSDKException):
                 raise
             else:
                 raise KsyunSDKException(e.message, e.message)
```

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/slb/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/slb/v20160304/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,16 @@
 
     def __init__(self):
         r"""修改监听器配置
         :param ListenerId: 监听器的ID
         :type PathPrefix: String
         :param ListenerName: 监听器的名称
         :type PathPrefix: String
+        :param BindType: 监听器支持的挂载类型(RealServer|BackendServerGroup)
+        :type PathPrefix: String
         :param ListenerState: 监听器的状态(start|stop)
         :type PathPrefix: String
         :param Method: 监听器的转发方式(RoundRobin|LeastConnections|MasterSlave|QUIC_CID|IPHash)
         :type PathPrefix: String
         :param BandWidthIn: 监听器的入带宽限速，单位Mbps，仅内网LB有此字段
         :type PathPrefix: Int
         :param BandWidthOut: 监听器的出带宽限速，单位Mbps，仅内网LB有此字段
@@ -82,14 +84,15 @@
         :param CertificateId: 证书的ID
         :type PathPrefix: String
         :param RedirectListenerId: 重定向监听器ID
         :type PathPrefix: String
         """
         self.ListenerId = None
         self.ListenerName = None
+        self.BindType = None
         self.ListenerState = None
         self.Method = None
         self.BandWidthIn = None
         self.BandWidthOut = None
         self.HttpProtocol = None
         self.TlsCipherPolicy = None
         self.EnableHttp2 = None
@@ -101,14 +104,16 @@
         self.RedirectListenerId = None
 
     def _deserialize(self, params):
         if params.get("ListenerId"):
             self.ListenerId = params.get("ListenerId")
         if params.get("ListenerName"):
             self.ListenerName = params.get("ListenerName")
+        if params.get("BindType"):
+            self.BindType = params.get("BindType")
         if params.get("ListenerState"):
             self.ListenerState = params.get("ListenerState")
         if params.get("Method"):
             self.Method = params.get("Method")
         if params.get("BandWidthIn"):
             self.BandWidthIn = params.get("BandWidthIn")
         if params.get("BandWidthOut"):
@@ -143,14 +148,16 @@
         :type PathPrefix: String
         :param ListenerName: 监听器的名称
         :type PathPrefix: String
         :param ListenerState: 监听器的状态(start|stop)
         :type PathPrefix: String
         :param ListenerProtocol: 监听器的协议(TCP|HTTP|HTTPS|UDP)
         :type PathPrefix: String
+        :param BindType: 监听器支持的挂载类型(RealServer|BackendServerGroup)
+        :type PathPrefix: String
         :param ListenerPort: 监听器的协议端口
         :type PathPrefix: Int
         :param Method: 监听器的转发方式(RoundRobin|LeastConnections|MasterSlave|QUIC_CID|IPHash)
         :type PathPrefix: String
         :param BandWidthIn: 监听器的入带宽限速，单位Mbps，仅内网LB有此字段
         :type PathPrefix: Int
         :param BandWidthOut: 监听器的出带宽限速，单位Mbps，仅内网LB有此字段
@@ -176,14 +183,15 @@
         :param CertificateId: 证书的ID
         :type PathPrefix: String
         """
         self.LoadBalancerId = None
         self.ListenerName = None
         self.ListenerState = None
         self.ListenerProtocol = None
+        self.BindType = None
         self.ListenerPort = None
         self.Method = None
         self.BandWidthIn = None
         self.BandWidthOut = None
         self.LoadBalancerAclId = None
         self.HttpProtocol = None
         self.TlsCipherPolicy = None
@@ -200,14 +208,16 @@
             self.LoadBalancerId = params.get("LoadBalancerId")
         if params.get("ListenerName"):
             self.ListenerName = params.get("ListenerName")
         if params.get("ListenerState"):
             self.ListenerState = params.get("ListenerState")
         if params.get("ListenerProtocol"):
             self.ListenerProtocol = params.get("ListenerProtocol")
+        if params.get("BindType"):
+            self.BindType = params.get("BindType")
         if params.get("ListenerPort"):
             self.ListenerPort = params.get("ListenerPort")
         if params.get("Method"):
             self.Method = params.get("Method")
         if params.get("BandWidthIn"):
             self.BandWidthIn = params.get("BandWidthIn")
         if params.get("BandWidthOut"):
@@ -236,42 +246,18 @@
 
 class ModifyInstancesWithListenerRequest(AbstractModel):
     """ModifyInstancesWithListener请求参数结构体
     """
 
     def __init__(self):
         r"""修改真实服务器信息
-        :param RegisterId: 后端服务器的ID
-        :type PathPrefix: String
-        :param Weight: 实例的权重
-        :type PathPrefix: Int
-        :param RealServerPort: 后端服务的端口
-        :type PathPrefix: Int
-        :param MasterSlaveType: RealServer的主备类型(Master | Slave)，仅MasterSlave监听器有此参数
-        :type PathPrefix: String
-        :param Tag: 标签
-        :type PathPrefix: String
         """
-        self.RegisterId = None
-        self.Weight = None
-        self.RealServerPort = None
-        self.MasterSlaveType = None
-        self.Tag = None
 
     def _deserialize(self, params):
-        if params.get("RegisterId"):
-            self.RegisterId = params.get("RegisterId")
-        if params.get("Weight"):
-            self.Weight = params.get("Weight")
-        if params.get("RealServerPort"):
-            self.RealServerPort = params.get("RealServerPort")
-        if params.get("MasterSlaveType"):
-            self.MasterSlaveType = params.get("MasterSlaveType")
-        if params.get("Tag"):
-            self.Tag = params.get("Tag")
+        return
 
 
 class RegisterInstancesWithListenerRequest(AbstractModel):
     """RegisterInstancesWithListener请求参数结构体
     """
 
     def __init__(self):
@@ -289,23 +275,26 @@
         :param InstanceId: - 实例ID
 - host类型，填写云主机或者云物理主机的ID
         :type PathPrefix: String
         :param Tag: 标签
         :type PathPrefix: String
         :param MasterSlaveType: RealServer的主备类型(Master | Slave)，仅MasterSlave监听器有此参数
         :type PathPrefix: String
+        :param NetworkInterfaceId: 弹性网卡ID
+        :type PathPrefix: String
         """
         self.RealServerType = None
         self.ListenerId = None
         self.Weight = None
         self.RealServerIp = None
         self.RealServerPort = None
         self.InstanceId = None
         self.Tag = None
         self.MasterSlaveType = None
+        self.NetworkInterfaceId = None
 
     def _deserialize(self, params):
         if params.get("RealServerType"):
             self.RealServerType = params.get("RealServerType")
         if params.get("ListenerId"):
             self.ListenerId = params.get("ListenerId")
         if params.get("Weight"):
@@ -316,14 +305,16 @@
             self.RealServerPort = params.get("RealServerPort")
         if params.get("InstanceId"):
             self.InstanceId = params.get("InstanceId")
         if params.get("Tag"):
             self.Tag = params.get("Tag")
         if params.get("MasterSlaveType"):
             self.MasterSlaveType = params.get("MasterSlaveType")
+        if params.get("NetworkInterfaceId"):
+            self.NetworkInterfaceId = params.get("NetworkInterfaceId")
 
 
 class DeregisterInstancesFromListenerRequest(AbstractModel):
     """DeregisterInstancesFromListener请求参数结构体
     """
 
     def __init__(self):
@@ -385,14 +376,16 @@
         :type PathPrefix: Int
         :param Interval: 健康检查时间间隔
         :type PathPrefix: Int
         :param Timeout: 健康检查超时时间
         :type PathPrefix: Int
         :param UnhealthyThreshold: 不健康阈值
         :type PathPrefix: Int
+        :param HealthProtocol: 健康检查协议 ,仅HTTP/HTTPS协议的监听器支持修改该值(TCP|HTTP)
+        :type PathPrefix: String
         :param HttpMethod: HTTP请求方式 (GET|HEAD)
         :type PathPrefix: String
         :param UrlPath: HTTP类型监听器健康检查的链接
         :type PathPrefix: String
         :param HostName: HTTP类型健康检查的域名
         :type PathPrefix: String
         :param HealthCheckReq: UDP监听健康检查的请求串
@@ -403,14 +396,15 @@
         self.HealthCheckId = None
         self.HealthCheckState = None
         self.HealthCheckConnectPort = None
         self.HealthyThreshold = None
         self.Interval = None
         self.Timeout = None
         self.UnhealthyThreshold = None
+        self.HealthProtocol = None
         self.HttpMethod = None
         self.UrlPath = None
         self.HostName = None
         self.HealthCheckReq = None
         self.HealthCheckExp = None
 
     def _deserialize(self, params):
@@ -424,14 +418,16 @@
             self.HealthyThreshold = params.get("HealthyThreshold")
         if params.get("Interval"):
             self.Interval = params.get("Interval")
         if params.get("Timeout"):
             self.Timeout = params.get("Timeout")
         if params.get("UnhealthyThreshold"):
             self.UnhealthyThreshold = params.get("UnhealthyThreshold")
+        if params.get("HealthProtocol"):
+            self.HealthProtocol = params.get("HealthProtocol")
         if params.get("HttpMethod"):
             self.HttpMethod = params.get("HttpMethod")
         if params.get("UrlPath"):
             self.UrlPath = params.get("UrlPath")
         if params.get("HostName"):
             self.HostName = params.get("HostName")
         if params.get("HealthCheckReq"):
@@ -503,14 +499,16 @@
         :type PathPrefix: Int
         :param Interval: 健康检查时间间隔
         :type PathPrefix: Int
         :param Timeout: 健康检查超时时间
         :type PathPrefix: Int
         :param UnhealthyThreshold: 不健康阈值
         :type PathPrefix: Int
+        :param HealthProtocol: 健康检查协议 (TCP|ICMP|UDP|HTTP), 当监听器为HTTP/HTTPS类型时可选值为UDP|HTTP ， 当监听器为UDP类型时可选值为UDP|ICMP
+        :type PathPrefix: String
         :param HttpMethod: HTTP请求方式 (GET|HEAD)
         :type PathPrefix: String
         :param UrlPath: HTTP类型监听器健康检查的链接
         :type PathPrefix: String
         :param HostName: HTTP类型健康检查的域名
         :type PathPrefix: String
         :param HealthCheckReq: UDP监听健康检查的请求串
@@ -521,14 +519,15 @@
         self.ListenerId = None
         self.HealthCheckState = None
         self.HealthCheckConnectPort = None
         self.HealthyThreshold = None
         self.Interval = None
         self.Timeout = None
         self.UnhealthyThreshold = None
+        self.HealthProtocol = None
         self.HttpMethod = None
         self.UrlPath = None
         self.HostName = None
         self.HealthCheckReq = None
         self.HealthCheckExp = None
 
     def _deserialize(self, params):
@@ -542,14 +541,16 @@
             self.HealthyThreshold = params.get("HealthyThreshold")
         if params.get("Interval"):
             self.Interval = params.get("Interval")
         if params.get("Timeout"):
             self.Timeout = params.get("Timeout")
         if params.get("UnhealthyThreshold"):
             self.UnhealthyThreshold = params.get("UnhealthyThreshold")
+        if params.get("HealthProtocol"):
+            self.HealthProtocol = params.get("HealthProtocol")
         if params.get("HttpMethod"):
             self.HttpMethod = params.get("HttpMethod")
         if params.get("UrlPath"):
             self.UrlPath = params.get("UrlPath")
         if params.get("HostName"):
             self.HostName = params.get("HostName")
         if params.get("HealthCheckReq"):
@@ -566,35 +567,50 @@
         r"""描述负载均衡
         :param ProjectId: 项目的ID
         :type PathPrefix: Filter
         :param LoadBalancerId: 多个负载均衡的ID
         :type PathPrefix: Filter
         :param Filter: 筛选Filter
         :type PathPrefix: Filter
-        :param MaxResults: 单次调用可返回的最大条目数量
+        :param IsContainTag: 是否在返回值中包含资源标签信息
+        :type PathPrefix: Boolean
+        :param TagKey: 多个标签的键
+        :type PathPrefix: Filter
+        :param TagKV: 多个标签的键
+        :type PathPrefix: Filter
+        :param MaxResults: 单次调用可返回的最大条目数量,默认值1000
         :type PathPrefix: Int
         :param NextToken: 获取另一页返回结果的 token.
         :type PathPrefix: String
         :param State: 负载均衡的状态，已绑定(associate)，未绑定(disassociate)
         :type PathPrefix: String
         """
         self.ProjectId = None
         self.LoadBalancerId = None
         self.Filter = None
+        self.IsContainTag = None
+        self.TagKey = None
+        self.TagKV = None
         self.MaxResults = None
         self.NextToken = None
         self.State = None
 
     def _deserialize(self, params):
         if params.get("ProjectId"):
             self.ProjectId = params.get("ProjectId")
         if params.get("LoadBalancerId"):
             self.LoadBalancerId = params.get("LoadBalancerId")
         if params.get("Filter"):
             self.Filter = params.get("Filter")
+        if params.get("IsContainTag"):
+            self.IsContainTag = params.get("IsContainTag")
+        if params.get("TagKey"):
+            self.TagKey = params.get("TagKey")
+        if params.get("TagKV"):
+            self.TagKV = params.get("TagKV")
         if params.get("MaxResults"):
             self.MaxResults = params.get("MaxResults")
         if params.get("NextToken"):
             self.NextToken = params.get("NextToken")
         if params.get("State"):
             self.State = params.get("State")
 
@@ -659,23 +675,29 @@
         :type PathPrefix: String
         :param IpVersion: 负载均衡的IP版本
         :type PathPrefix: String
         :param LbType: 负载均衡类型(classic|application)
         :type PathPrefix: String
         :param ProjectId: 项目的ID
         :type PathPrefix: String
+        :param DeleteProtection: 删除保护状态(on|off)
+        :type PathPrefix: String
+        :param ModificationProtection: 修改保护状态(on|off)
+        :type PathPrefix: String
         """
         self.VpcId = None
         self.LoadBalancerName = None
         self.Type = None
         self.SubnetId = None
         self.PrivateIpAddress = None
         self.IpVersion = None
         self.LbType = None
         self.ProjectId = None
+        self.DeleteProtection = None
+        self.ModificationProtection = None
 
     def _deserialize(self, params):
         if params.get("VpcId"):
             self.VpcId = params.get("VpcId")
         if params.get("LoadBalancerName"):
             self.LoadBalancerName = params.get("LoadBalancerName")
         if params.get("Type"):
@@ -686,14 +708,18 @@
             self.PrivateIpAddress = params.get("PrivateIpAddress")
         if params.get("IpVersion"):
             self.IpVersion = params.get("IpVersion")
         if params.get("LbType"):
             self.LbType = params.get("LbType")
         if params.get("ProjectId"):
             self.ProjectId = params.get("ProjectId")
+        if params.get("DeleteProtection"):
+            self.DeleteProtection = params.get("DeleteProtection")
+        if params.get("ModificationProtection"):
+            self.ModificationProtection = params.get("ModificationProtection")
 
 
 class CreateHostHeaderRequest(AbstractModel):
     """CreateHostHeader请求参数结构体
     """
 
     def __init__(self):
@@ -837,14 +863,16 @@
     """CreateBackendServerGroup请求参数结构体
     """
 
     def __init__(self):
         r"""创建后端服务组
         :param VpcId: Vpc的ID
         :type PathPrefix: String
+        :param Protocol: 后端协议, 默认HTTP
+        :type PathPrefix: String
         :param BackendServerGroupName: 后端服务组的名称
         :type PathPrefix: String
         :param BackendServerGroupType: 后端服务组类型(Server: 服务器|Mirror: 镜像服务器)
         :type PathPrefix: String
         :param HostName: HTTP类型健康检查的域名
         :type PathPrefix: String
         :param HealthCheckState: 健康检查保持的状态(start|stop)
@@ -857,33 +885,33 @@
         :type PathPrefix: Int
         :param UnhealthyThreshold: 不健康阈值，此参数镜像服务器不可为空
         :type PathPrefix: Int
         :param UrlPath: HTTP类型监听器健康检查的链接
         :type PathPrefix: String
         :param Region: Region机房
         :type PathPrefix: String
-        :param Type: 类型(Host|DirectConnect)
-        :type PathPrefix: String
         """
         self.VpcId = None
+        self.Protocol = None
         self.BackendServerGroupName = None
         self.BackendServerGroupType = None
         self.HostName = None
         self.HealthCheckState = None
         self.HealthyThreshold = None
         self.Interval = None
         self.Timeout = None
         self.UnhealthyThreshold = None
         self.UrlPath = None
         self.Region = None
-        self.Type = None
 
     def _deserialize(self, params):
         if params.get("VpcId"):
             self.VpcId = params.get("VpcId")
+        if params.get("Protocol"):
+            self.Protocol = params.get("Protocol")
         if params.get("BackendServerGroupName"):
             self.BackendServerGroupName = params.get("BackendServerGroupName")
         if params.get("BackendServerGroupType"):
             self.BackendServerGroupType = params.get("BackendServerGroupType")
         if params.get("HostName"):
             self.HostName = params.get("HostName")
         if params.get("HealthCheckState"):
@@ -896,16 +924,14 @@
             self.Timeout = params.get("Timeout")
         if params.get("UnhealthyThreshold"):
             self.UnhealthyThreshold = params.get("UnhealthyThreshold")
         if params.get("UrlPath"):
             self.UrlPath = params.get("UrlPath")
         if params.get("Region"):
             self.Region = params.get("Region")
-        if params.get("Type"):
-            self.Type = params.get("Type")
 
 
 class DeleteBackendServerGroupRequest(AbstractModel):
     """DeleteBackendServerGroup请求参数结构体
     """
 
     def __init__(self):
@@ -1020,15 +1046,15 @@
 
 
 class DescribeBackendServersRequest(AbstractModel):
     """DescribeBackendServers请求参数结构体
     """
 
     def __init__(self):
-        r"""获取后端服务器列表
+        r"""查询服务器组中后端服务信息
         :param RegisterId: 多个绑定服务器组的注册ID
         :type PathPrefix: Filter
         :param Filter: 筛选Filter
         :type PathPrefix: Filter
         :param MaxResults: 单次调用可返回的最大条目数量
         :type PathPrefix: Int
         :param NextToken: 获取另一页返回结果的 token.
@@ -1451,29 +1477,34 @@
         :type PathPrefix: Filter
         :param ProjectId: 项目的ID
         :type PathPrefix: Filter
         :param MaxResults: 单次调用可返回的最大条目数量
         :type PathPrefix: Int
         :param NextToken: 获取另一页返回结果的 token.
         :type PathPrefix: String
+        :param Fillter.N: 
+        :type PathPrefix: Object
         """
         self.PrivateLinkServerId = None
         self.ProjectId = None
         self.MaxResults = None
         self.NextToken = None
+        self.Fillter.N = None
 
     def _deserialize(self, params):
         if params.get("PrivateLinkServerId"):
             self.PrivateLinkServerId = params.get("PrivateLinkServerId")
         if params.get("ProjectId"):
             self.ProjectId = params.get("ProjectId")
         if params.get("MaxResults"):
             self.MaxResults = params.get("MaxResults")
         if params.get("NextToken"):
             self.NextToken = params.get("NextToken")
+        if params.get("Fillter.N"):
+            self.Fillter.N = params.get("Fillter.N")
 
 
 class DeletePrivateLinkServerRequest(AbstractModel):
     """DeletePrivateLinkServer请求参数结构体
     """
 
     def __init__(self):
@@ -1555,29 +1586,34 @@
         :type PathPrefix: Filter
         :param ProjectId: 项目的ID
         :type PathPrefix: Filter
         :param MaxResults: 单次调用可返回的最大条目数量
         :type PathPrefix: Int
         :param NextToken: 获取另一页返回结果的 token.
         :type PathPrefix: String
+        :param Filter.N: 
+        :type PathPrefix: Object
         """
         self.PrivateLinkId = None
         self.ProjectId = None
         self.MaxResults = None
         self.NextToken = None
+        self.Filter.N = None
 
     def _deserialize(self, params):
         if params.get("PrivateLinkId"):
             self.PrivateLinkId = params.get("PrivateLinkId")
         if params.get("ProjectId"):
             self.ProjectId = params.get("ProjectId")
         if params.get("MaxResults"):
             self.MaxResults = params.get("MaxResults")
         if params.get("NextToken"):
             self.NextToken = params.get("NextToken")
+        if params.get("Filter.N"):
+            self.Filter.N = params.get("Filter.N")
 
 
 class DeletePrivateLinkRequest(AbstractModel):
     """DeletePrivateLink请求参数结构体
     """
 
     def __init__(self):
@@ -1708,15 +1744,14 @@
         :param AlbVersion: 应用型负载均衡支持的版本
         :type PathPrefix: String
         :param AlbType: 应用型负载均衡的类型，public 为公网负载均衡，internal 为内网负载均衡
         :type PathPrefix: String
         :param VpcId: Vpc的ID
         :type PathPrefix: String
         :param IpVersion: 负载均衡的IP版本
-ipv4 
         :type PathPrefix: String
         :param ProjectId: 项目的ID
         :type PathPrefix: String
         :param AllocationId: 弹性IP的ID
         :type PathPrefix: String
         :param ChargeType: 计费类型(PrePaidByHourUsage，按小时用量实时付费（小时结))
         :type PathPrefix: String
@@ -1751,22 +1786,18 @@
 
 class DeleteAlbRequest(AbstractModel):
     """DeleteAlb请求参数结构体
     """
 
     def __init__(self):
         r"""DeleteAlb
-        :param AlbId: 应用型负载均衡的ID
-        :type PathPrefix: String
         """
-        self.AlbId = None
 
     def _deserialize(self, params):
-        if params.get("AlbId"):
-            self.AlbId = params.get("AlbId")
+        return
 
 
 class SetAlbNameRequest(AbstractModel):
     """SetAlbName请求参数结构体
     """
 
     def __init__(self):
@@ -1813,33 +1844,53 @@
 
     def __init__(self):
         r"""DescribeAlbs
         :param AlbId: 多个应用型负载均衡的ID
         :type PathPrefix: Filter
         :param Filter: 筛选Filter
         :type PathPrefix: Filter
+        :param IsContainTag: 是否在返回值中包含资源标签信息
+        :type PathPrefix: Boolean
+        :param TagKey: 多个标签的键
+        :type PathPrefix: Filter
+        :param TagKV: 多个标签的键
+        :type PathPrefix: Filter
         :param MaxResults: 单次调用可返回的最大条目数量
         :type PathPrefix: Int
         :param NextToken: 获取另一页返回结果的 token.
         :type PathPrefix: String
+        :param ProjectId: 项目制ID
+        :type PathPrefix: Filter
         """
         self.AlbId = None
         self.Filter = None
+        self.IsContainTag = None
+        self.TagKey = None
+        self.TagKV = None
         self.MaxResults = None
         self.NextToken = None
+        self.ProjectId = None
 
     def _deserialize(self, params):
         if params.get("AlbId"):
             self.AlbId = params.get("AlbId")
         if params.get("Filter"):
             self.Filter = params.get("Filter")
+        if params.get("IsContainTag"):
+            self.IsContainTag = params.get("IsContainTag")
+        if params.get("TagKey"):
+            self.TagKey = params.get("TagKey")
+        if params.get("TagKV"):
+            self.TagKV = params.get("TagKV")
         if params.get("MaxResults"):
             self.MaxResults = params.get("MaxResults")
         if params.get("NextToken"):
             self.NextToken = params.get("NextToken")
+        if params.get("ProjectId"):
+            self.ProjectId = params.get("ProjectId")
 
 
 class CreateAlbListenerRequest(AbstractModel):
     """CreateAlbListener请求参数结构体
     """
 
     def __init__(self):
@@ -1858,42 +1909,51 @@
         :type PathPrefix: String
         :param TlsCipherPolicy: TLS安全策略
         :type PathPrefix: String
         :param AlbListenerAclId: LoadBalancerAcl的ID
         :type PathPrefix: String
         :param AlbListenerState: 应用型监听器的状态(start|stop)
         :type PathPrefix: String
+        :param RedirectAlbListenerId: 重定向应用型监听器ID
+        :type PathPrefix: String
+        :param RedirectHttpCode: 重定向状态码
+        :type PathPrefix: String
         :param SessionState: 会话保持的状态(start|stop)
         :type PathPrefix: String
         :param SessionPersistencePeriod: 会话保持超时时间
         :type PathPrefix: Int
         :param CookieType: 会话类型
         :type PathPrefix: String
         :param CookieName: Cookie的名称
         :type PathPrefix: String
         :param EnableHttp2: 是否启用HTTP/2
         :type PathPrefix: Boolean
-        :param HttpProtocol: 后端协议版本(HTTP1.0|HTTP1.1)
+        :param BackendServerGroupId: 默认转发策略绑定的服务器组ID,目前仅支持创建转发类型的默认转发策略
         :type PathPrefix: String
+        :param FixedResponseConfig: 返回固定响应信息
+        :type PathPrefix: Object
         """
         self.AlbId = None
         self.AlbListenerName = None
         self.Method = None
         self.Protocol = None
         self.Port = None
         self.CertificateId = None
         self.TlsCipherPolicy = None
         self.AlbListenerAclId = None
         self.AlbListenerState = None
+        self.RedirectAlbListenerId = None
+        self.RedirectHttpCode = None
         self.SessionState = None
         self.SessionPersistencePeriod = None
         self.CookieType = None
         self.CookieName = None
         self.EnableHttp2 = None
-        self.HttpProtocol = None
+        self.BackendServerGroupId = None
+        self.FixedResponseConfig = None
 
     def _deserialize(self, params):
         if params.get("AlbId"):
             self.AlbId = params.get("AlbId")
         if params.get("AlbListenerName"):
             self.AlbListenerName = params.get("AlbListenerName")
         if params.get("Method"):
@@ -1906,26 +1966,32 @@
             self.CertificateId = params.get("CertificateId")
         if params.get("TlsCipherPolicy"):
             self.TlsCipherPolicy = params.get("TlsCipherPolicy")
         if params.get("AlbListenerAclId"):
             self.AlbListenerAclId = params.get("AlbListenerAclId")
         if params.get("AlbListenerState"):
             self.AlbListenerState = params.get("AlbListenerState")
+        if params.get("RedirectAlbListenerId"):
+            self.RedirectAlbListenerId = params.get("RedirectAlbListenerId")
+        if params.get("RedirectHttpCode"):
+            self.RedirectHttpCode = params.get("RedirectHttpCode")
         if params.get("SessionState"):
             self.SessionState = params.get("SessionState")
         if params.get("SessionPersistencePeriod"):
             self.SessionPersistencePeriod = params.get("SessionPersistencePeriod")
         if params.get("CookieType"):
             self.CookieType = params.get("CookieType")
         if params.get("CookieName"):
             self.CookieName = params.get("CookieName")
         if params.get("EnableHttp2"):
             self.EnableHttp2 = params.get("EnableHttp2")
-        if params.get("HttpProtocol"):
-            self.HttpProtocol = params.get("HttpProtocol")
+        if params.get("BackendServerGroupId"):
+            self.BackendServerGroupId = params.get("BackendServerGroupId")
+        if params.get("FixedResponseConfig"):
+            self.FixedResponseConfig = params.get("FixedResponseConfig")
 
 
 class ModifyAlbListenerRequest(AbstractModel):
     """ModifyAlbListener请求参数结构体
     """
 
     def __init__(self):
@@ -2059,14 +2125,16 @@
         :type PathPrefix: String
         :param BackendServerGroupId: 后端服务器组的ID
         :type PathPrefix: String
         :param ListenerSync: 是否同步监听器的健康检查、会话保持和转发算法(on|off)
         :type PathPrefix: String
         :param Method: 监听器的转发方式(RoundRobin|LeastConnections)
         :type PathPrefix: String
+        :param Type: 转发动作类型
+        :type PathPrefix: String
         :param SessionState: 会话保持的状态，在ListenerSync为off时有效
         :type PathPrefix: String
         :param SessionPersistencePeriod: 会话保持超时时间
         :type PathPrefix: Int
         :param CookieType: 会话类型(ImplantCookie|RewriteCookie)
         :type PathPrefix: String
         :param CookieName: Cookie的名称
@@ -2083,51 +2151,56 @@
         :type PathPrefix: Int
         :param UrlPath: HTTP类型监听器健康检查的链接
         :type PathPrefix: String
         :param HostName: HTTP类型健康检查的域名
         :type PathPrefix: String
         :param AlbRuleSet: 规则的信息
         :type PathPrefix: Array
-        :param RedirectHttpCode: 重定向状态码
-301|302|307
+        :param RedirectAlbListenerId: 重定向应用型监听器ID
         :type PathPrefix: String
-        :param RedirectAlbListenerId: 重定向的监听器ID
+        :param RedirectHttpCode: 重定向状态码,301|302|307
         :type PathPrefix: String
+        :param FixedResponseConfig: 返回固定响应信息
+        :type PathPrefix: Object
         """
         self.AlbRuleGroupName = None
         self.AlbListenerId = None
         self.BackendServerGroupId = None
         self.ListenerSync = None
         self.Method = None
+        self.Type = None
         self.SessionState = None
         self.SessionPersistencePeriod = None
         self.CookieType = None
         self.CookieName = None
         self.HealthCheckState = None
         self.Timeout = None
         self.Interval = None
         self.HealthyThreshold = None
         self.UnhealthyThreshold = None
         self.UrlPath = None
         self.HostName = None
         self.AlbRuleSet = None
-        self.RedirectHttpCode = None
         self.RedirectAlbListenerId = None
+        self.RedirectHttpCode = None
+        self.FixedResponseConfig = None
 
     def _deserialize(self, params):
         if params.get("AlbRuleGroupName"):
             self.AlbRuleGroupName = params.get("AlbRuleGroupName")
         if params.get("AlbListenerId"):
             self.AlbListenerId = params.get("AlbListenerId")
         if params.get("BackendServerGroupId"):
             self.BackendServerGroupId = params.get("BackendServerGroupId")
         if params.get("ListenerSync"):
             self.ListenerSync = params.get("ListenerSync")
         if params.get("Method"):
             self.Method = params.get("Method")
+        if params.get("Type"):
+            self.Type = params.get("Type")
         if params.get("SessionState"):
             self.SessionState = params.get("SessionState")
         if params.get("SessionPersistencePeriod"):
             self.SessionPersistencePeriod = params.get("SessionPersistencePeriod")
         if params.get("CookieType"):
             self.CookieType = params.get("CookieType")
         if params.get("CookieName"):
@@ -2144,18 +2217,20 @@
             self.UnhealthyThreshold = params.get("UnhealthyThreshold")
         if params.get("UrlPath"):
             self.UrlPath = params.get("UrlPath")
         if params.get("HostName"):
             self.HostName = params.get("HostName")
         if params.get("AlbRuleSet"):
             self.AlbRuleSet = params.get("AlbRuleSet")
-        if params.get("RedirectHttpCode"):
-            self.RedirectHttpCode = params.get("RedirectHttpCode")
         if params.get("RedirectAlbListenerId"):
             self.RedirectAlbListenerId = params.get("RedirectAlbListenerId")
+        if params.get("RedirectHttpCode"):
+            self.RedirectHttpCode = params.get("RedirectHttpCode")
+        if params.get("FixedResponseConfig"):
+            self.FixedResponseConfig = params.get("FixedResponseConfig")
 
 
 class DeleteAlbRuleGroupRequest(AbstractModel):
     """DeleteAlbRuleGroup请求参数结构体
     """
 
     def __init__(self):
@@ -2213,14 +2288,16 @@
         :type PathPrefix: String
         :param BackendServerGroupId: 后端服务器组的ID
         :type PathPrefix: String
         :param ListenerSync: 是否同步监听器的健康检查、会话保持和转发算法(on | off)
         :type PathPrefix: String
         :param Method: 监听器的转发方式(RoundRobin|LeastConnections)
         :type PathPrefix: String
+        :param Type: 转发动作类型
+        :type PathPrefix: String
         :param SessionState: 会话保持的状态，在ListenerSync为off时有效
         :type PathPrefix: String
         :param SessionPersistencePeriod: 会话保持超时时间
         :type PathPrefix: Int
         :param CookieType: 会话类型(ImplantCookie|RewriteCookie)
         :type PathPrefix: String
         :param CookieName: Cookie的名称
@@ -2237,50 +2314,56 @@
         :type PathPrefix: Int
         :param UrlPath: HTTP类型监听器健康检查的链接
         :type PathPrefix: String
         :param HostName: HTTP类型健康检查的域名
         :type PathPrefix: String
         :param AlbRuleSet: 规则的信息
         :type PathPrefix: Array
-        :param RedirectHttpCode: 重定向状态码
+        :param RedirectAlbListenerId: 重定向应用型监听器ID
         :type PathPrefix: String
-        :param RedirectAlbListenerId: 重定向的监听器ID
+        :param RedirectHttpCode: 重定向状态码,301|302|307
         :type PathPrefix: String
+        :param FixedResponseConfig: 返回固定响应信息
+        :type PathPrefix: Object
         """
         self.AlbRuleGroupId = None
         self.AlbRuleGroupName = None
         self.BackendServerGroupId = None
         self.ListenerSync = None
         self.Method = None
+        self.Type = None
         self.SessionState = None
         self.SessionPersistencePeriod = None
         self.CookieType = None
         self.CookieName = None
         self.HealthCheckState = None
         self.Timeout = None
         self.Interval = None
         self.HealthyThreshold = None
         self.UnhealthyThreshold = None
         self.UrlPath = None
         self.HostName = None
         self.AlbRuleSet = None
-        self.RedirectHttpCode = None
         self.RedirectAlbListenerId = None
+        self.RedirectHttpCode = None
+        self.FixedResponseConfig = None
 
     def _deserialize(self, params):
         if params.get("AlbRuleGroupId"):
             self.AlbRuleGroupId = params.get("AlbRuleGroupId")
         if params.get("AlbRuleGroupName"):
             self.AlbRuleGroupName = params.get("AlbRuleGroupName")
         if params.get("BackendServerGroupId"):
             self.BackendServerGroupId = params.get("BackendServerGroupId")
         if params.get("ListenerSync"):
             self.ListenerSync = params.get("ListenerSync")
         if params.get("Method"):
             self.Method = params.get("Method")
+        if params.get("Type"):
+            self.Type = params.get("Type")
         if params.get("SessionState"):
             self.SessionState = params.get("SessionState")
         if params.get("SessionPersistencePeriod"):
             self.SessionPersistencePeriod = params.get("SessionPersistencePeriod")
         if params.get("CookieType"):
             self.CookieType = params.get("CookieType")
         if params.get("CookieName"):
@@ -2297,18 +2380,20 @@
             self.UnhealthyThreshold = params.get("UnhealthyThreshold")
         if params.get("UrlPath"):
             self.UrlPath = params.get("UrlPath")
         if params.get("HostName"):
             self.HostName = params.get("HostName")
         if params.get("AlbRuleSet"):
             self.AlbRuleSet = params.get("AlbRuleSet")
-        if params.get("RedirectHttpCode"):
-            self.RedirectHttpCode = params.get("RedirectHttpCode")
         if params.get("RedirectAlbListenerId"):
             self.RedirectAlbListenerId = params.get("RedirectAlbListenerId")
+        if params.get("RedirectHttpCode"):
+            self.RedirectHttpCode = params.get("RedirectHttpCode")
+        if params.get("FixedResponseConfig"):
+            self.FixedResponseConfig = params.get("FixedResponseConfig")
 
 
 class AddAlbRuleRequest(AbstractModel):
     """AddAlbRule请求参数结构体
     """
 
     def __init__(self):
@@ -2491,28 +2576,28 @@
 
     def __init__(self):
         r"""SetAlbAccessLog
         :param AlbId: 应用型负载均衡的ID
         :type PathPrefix: String
         :param ProjectName: 访问日志投递的日志库
         :type PathPrefix: String
-        :param LogpoolName: 访问日志投递的日志池
+        :param LogPoolName: 访问日志投递的日志池
         :type PathPrefix: String
         """
         self.AlbId = None
         self.ProjectName = None
-        self.LogpoolName = None
+        self.LogPoolName = None
 
     def _deserialize(self, params):
         if params.get("AlbId"):
             self.AlbId = params.get("AlbId")
         if params.get("ProjectName"):
             self.ProjectName = params.get("ProjectName")
-        if params.get("LogpoolName"):
-            self.LogpoolName = params.get("LogpoolName")
+        if params.get("LogPoolName"):
+            self.LogPoolName = params.get("LogPoolName")
 
 
 class CloneLoadBalancerRequest(AbstractModel):
     """CloneLoadBalancer请求参数结构体
     """
 
     def __init__(self):
@@ -2533,7 +2618,283 @@
             self.VpcId = params.get("VpcId")
         if params.get("LoadBalancerName"):
             self.LoadBalancerName = params.get("LoadBalancerName")
         if params.get("Type"):
             self.Type = params.get("Type")
 
 
+class SetLBDeleteProtectionRequest(AbstractModel):
+    """SetLBDeleteProtection请求参数结构体
+    """
+
+    def __init__(self):
+        r"""设置删除保护
+        :param LoadBalancerId: 负载均衡id
+        :type PathPrefix: String
+        :param DeleteProtection: 删除保护状态(on|off)
+        :type PathPrefix: String
+        """
+        self.LoadBalancerId = None
+        self.DeleteProtection = None
+
+    def _deserialize(self, params):
+        if params.get("LoadBalancerId"):
+            self.LoadBalancerId = params.get("LoadBalancerId")
+        if params.get("DeleteProtection"):
+            self.DeleteProtection = params.get("DeleteProtection")
+
+
+class SetLBModificationProtectionRequest(AbstractModel):
+    """SetLBModificationProtection请求参数结构体
+    """
+
+    def __init__(self):
+        r"""设置修改保护
+        :param LoadBalancerId: 负载均衡id
+        :type PathPrefix: String
+        :param ModificationProtection: 修改保护状态(on|off)
+        :type PathPrefix: String
+        """
+        self.LoadBalancerId = None
+        self.ModificationProtection = None
+
+    def _deserialize(self, params):
+        if params.get("LoadBalancerId"):
+            self.LoadBalancerId = params.get("LoadBalancerId")
+        if params.get("ModificationProtection"):
+            self.ModificationProtection = params.get("ModificationProtection")
+
+
+class ModifyCertificateWithGroupRequest(AbstractModel):
+    """ModifyCertificateWithGroup请求参数结构体
+    """
+
+    def __init__(self):
+        r"""监听器维度更换同域名的证书
+        :param AlbListenerCertGroupId: 证书组的ID
+        :type PathPrefix: String
+        :param OldCertificateId: 旧证书的ID
+        :type PathPrefix: String
+        :param CertificateId: 新证书的ID
+        :type PathPrefix: String
+        """
+        self.AlbListenerCertGroupId = None
+        self.OldCertificateId = None
+        self.CertificateId = None
+
+    def _deserialize(self, params):
+        if params.get("AlbListenerCertGroupId"):
+            self.AlbListenerCertGroupId = params.get("AlbListenerCertGroupId")
+        if params.get("OldCertificateId"):
+            self.OldCertificateId = params.get("OldCertificateId")
+        if params.get("CertificateId"):
+            self.CertificateId = params.get("CertificateId")
+
+
+class CreateAlbBackendServerGroupRequest(AbstractModel):
+    """CreateAlbBackendServerGroup请求参数结构体
+    """
+
+    def __init__(self):
+        r"""创建ALB服务器组
+        :param VpcId: Vpc的ID
+        :type PathPrefix: String
+        :param Name: ALB负载均衡的名称
+        :type PathPrefix: String
+        :param BackendServerType: 服务器组的正实服务器类型
+        :type PathPrefix: String
+        :param UpstreamKeepalive: 后端长连接类型
+        :type PathPrefix: String
+        :param Protocol: 后端协议 (HTTP|gRPC)
+        :type PathPrefix: String
+        """
+        self.VpcId = None
+        self.Name = None
+        self.BackendServerType = None
+        self.UpstreamKeepalive = None
+        self.Protocol = None
+
+    def _deserialize(self, params):
+        if params.get("VpcId"):
+            self.VpcId = params.get("VpcId")
+        if params.get("Name"):
+            self.Name = params.get("Name")
+        if params.get("BackendServerType"):
+            self.BackendServerType = params.get("BackendServerType")
+        if params.get("UpstreamKeepalive"):
+            self.UpstreamKeepalive = params.get("UpstreamKeepalive")
+        if params.get("Protocol"):
+            self.Protocol = params.get("Protocol")
+
+
+class DeleteAlbBackendServerGroupRequest(AbstractModel):
+    """DeleteAlbBackendServerGroup请求参数结构体
+    """
+
+    def __init__(self):
+        r"""删除ALB服务器组
+        :param BackendServerGroupId: ALB服务器组id
+        :type PathPrefix: String
+        """
+        self.BackendServerGroupId = None
+
+    def _deserialize(self, params):
+        if params.get("BackendServerGroupId"):
+            self.BackendServerGroupId = params.get("BackendServerGroupId")
+
+
+class ModifyAlbBackendServerGroupRequest(AbstractModel):
+    """ModifyAlbBackendServerGroup请求参数结构体
+    """
+
+    def __init__(self):
+        r"""修改ALB服务器组
+        :param BackendServerGroupId: ALB服务器组id
+        :type PathPrefix: String
+        :param Name: ALB负载均衡的名称
+        :type PathPrefix: String
+        :param UpstreamKeepalive: 后端长连接类型
+        :type PathPrefix: String
+        """
+        self.BackendServerGroupId = None
+        self.Name = None
+        self.UpstreamKeepalive = None
+
+    def _deserialize(self, params):
+        if params.get("BackendServerGroupId"):
+            self.BackendServerGroupId = params.get("BackendServerGroupId")
+        if params.get("Name"):
+            self.Name = params.get("Name")
+        if params.get("UpstreamKeepalive"):
+            self.UpstreamKeepalive = params.get("UpstreamKeepalive")
+
+
+class DescribeAlbBackendServerGroupsRequest(AbstractModel):
+    """DescribeAlbBackendServerGroups请求参数结构体
+    """
+
+    def __init__(self):
+        r"""查询ALB服务器组
+        :param Filter: 筛选Filter
+        :type PathPrefix: Filter
+        :param MaxResults: 单次调用可返回的最大条目数量
+        :type PathPrefix: Int
+        :param NextToken: 获取另一页返回结果的 token.
+        :type PathPrefix: String
+        """
+        self.Filter = None
+        self.MaxResults = None
+        self.NextToken = None
+
+    def _deserialize(self, params):
+        if params.get("Filter"):
+            self.Filter = params.get("Filter")
+        if params.get("MaxResults"):
+            self.MaxResults = params.get("MaxResults")
+        if params.get("NextToken"):
+            self.NextToken = params.get("NextToken")
+
+
+class RegisterAlbBackendServerRequest(AbstractModel):
+    """RegisterAlbBackendServer请求参数结构体
+    """
+
+    def __init__(self):
+        r"""ALB注册服务器到服务器组
+        :param BackendServerGroupId: ALB服务器组id
+        :type PathPrefix: String
+        :param BackendServerIp: 服务器ip
+        :type PathPrefix: String
+        :param Port: 服务器端口
+        :type PathPrefix: Int
+        :param Weight: 服务器权重
+        :type PathPrefix: Int
+        :param NetworkInterfaceId: 网卡id
+        :type PathPrefix: String
+        :param DirectConnectGatewayId: 对等连接id
+        :type PathPrefix: String
+        """
+        self.BackendServerGroupId = None
+        self.BackendServerIp = None
+        self.Port = None
+        self.Weight = None
+        self.NetworkInterfaceId = None
+        self.DirectConnectGatewayId = None
+
+    def _deserialize(self, params):
+        if params.get("BackendServerGroupId"):
+            self.BackendServerGroupId = params.get("BackendServerGroupId")
+        if params.get("BackendServerIp"):
+            self.BackendServerIp = params.get("BackendServerIp")
+        if params.get("Port"):
+            self.Port = params.get("Port")
+        if params.get("Weight"):
+            self.Weight = params.get("Weight")
+        if params.get("NetworkInterfaceId"):
+            self.NetworkInterfaceId = params.get("NetworkInterfaceId")
+        if params.get("DirectConnectGatewayId"):
+            self.DirectConnectGatewayId = params.get("DirectConnectGatewayId")
+
+
+class DeregisterAlbBackendServerRequest(AbstractModel):
+    """DeregisterAlbBackendServer请求参数结构体
+    """
+
+    def __init__(self):
+        r"""ALB从服务器组移除服务器
+        :param BackendServerId: 服务器id
+        :type PathPrefix: String
+        """
+        self.BackendServerId = None
+
+    def _deserialize(self, params):
+        if params.get("BackendServerId"):
+            self.BackendServerId = params.get("BackendServerId")
+
+
+class ModifyAlbBackendServerRequest(AbstractModel):
+    """ModifyAlbBackendServer请求参数结构体
+    """
+
+    def __init__(self):
+        r"""修改ALB服务器信息
+        :param BackendServerId: 服务器id
+        :type PathPrefix: String
+        :param Weight: 服务器的权重
+        :type PathPrefix: Int
+        """
+        self.BackendServerId = None
+        self.Weight = None
+
+    def _deserialize(self, params):
+        if params.get("BackendServerId"):
+            self.BackendServerId = params.get("BackendServerId")
+        if params.get("Weight"):
+            self.Weight = params.get("Weight")
+
+
+class DescribeAlbBackendServersRequest(AbstractModel):
+    """DescribeAlbBackendServers请求参数结构体
+    """
+
+    def __init__(self):
+        r"""查询ALB服务器信息
+        :param Filter: 筛选Filter
+        :type PathPrefix: Filter
+        :param MaxResults: 单次调用可返回的最大条目数量
+        :type PathPrefix: Int
+        :param NextToken: 获取另一页返回结果的 token.
+        :type PathPrefix: String
+        """
+        self.Filter = None
+        self.MaxResults = None
+        self.NextToken = None
+
+    def _deserialize(self, params):
+        if params.get("Filter"):
+            self.Filter = params.get("Filter")
+        if params.get("MaxResults"):
+            self.MaxResults = params.get("MaxResults")
+        if params.get("NextToken"):
+            self.NextToken = params.get("NextToken")
+
+
```

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/sts/v20151101/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/sts/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/sts/v20151101/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/sts/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/tagv2/v20200901/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/tagv2/v20200901/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/tagv2/v20200901/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/tagv2/v20200901/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/tidb/v20210520/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/tidb/v20210520/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/tidb/v20210520/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/tidb/v20210520/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/trade/v20200114/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/trade/v20200114/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/trade/v20200831/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/trade/v20200831/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/trade/v20200831/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/trade/v20200831/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/vpc/v20160304/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/vpc/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/vpc/v20160304/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/vpc/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/waf/v20200707/client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/waf/v20200707/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/client/waf/v20200707/models.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/client/waf/v20200707/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/common/abstract_client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/common/abstract_model.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/common/common_client.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/common/common_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/common/credential.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/common/credential.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/common/exception/__init__.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/common/exception/ksyun_sdk_exception.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/common/exception/ksyun_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/common/http/request.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/common/http/request.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/common/profile/client_profile.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/ksyun/common/profile/http_profile.py` & `kingsoftcloud_sdk_python-1.4.3/ksyun/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud_sdk_python-1.4.2/setup.py` & `kingsoftcloud_sdk_python-1.4.3/setup.py`

 * *Files identical despite different names*

