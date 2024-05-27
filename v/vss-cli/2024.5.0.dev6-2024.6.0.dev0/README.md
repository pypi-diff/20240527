# Comparing `tmp/vss-cli-2024.5.0.dev6.tar.gz` & `tmp/vss-cli-2024.6.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vss-cli-2024.5.0.dev6.tar", last modified: Fri May 24 16:05:16 2024, max compression
+gzip compressed data, was "vss-cli-2024.6.0.dev0.tar", last modified: Mon May 27 16:01:16 2024, max compression
```

## Comparing `vss-cli-2024.5.0.dev6.tar` & `vss-cli-2024.6.0.dev0.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:05:16.061564 vss-cli-2024.5.0.dev6/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13950 2024-05-24 16:05:16.061564 vss-cli-2024.5.0.dev6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10991 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/README.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1257 2024-05-24 16:05:16.061564 vss-cli-2024.5.0.dev6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3827 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:05:16.045564 vss-cli-2024.5.0.dev6/tests/
--rw-rw-rw-   0 root         (0) root         (0)     5569 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/tests/test_vss_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:05:16.049564 vss-cli-2024.5.0.dev6/vss_cli/
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19671 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/autocompletion.py
--rw-rw-rw-   0 root         (0) root         (0)     7449 2024-05-23 18:19:57.000000 vss-cli-2024.5.0.dev6/vss_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    64867 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/config.py
--rw-rw-rw-   0 root         (0) root         (0)    15466 2024-05-24 16:04:34.000000 vss-cli-2024.5.0.dev6/vss_cli/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:05:16.049564 vss-cli-2024.5.0.dev6/vss_cli/data/
--rw-rw-rw-   0 root         (0) root         (0)     4500 2024-05-24 16:04:34.000000 vss-cli-2024.5.0.dev6/vss_cli/data/clib.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4288 2024-05-24 16:04:34.000000 vss-cli-2024.5.0.dev6/vss_cli/data/clone.yaml
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/data/config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2892 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/data/image.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2926 2024-05-24 16:04:34.000000 vss-cli-2024.5.0.dev6/vss_cli/data/shell.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4198 2024-05-24 16:04:34.000000 vss-cli-2024.5.0.dev6/vss_cli/data/template.yaml
--rw-rw-rw-   0 root         (0) root         (0)    25848 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/data_types.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/hcio.py
--rw-rw-rw-   0 root         (0) root         (0)    12512 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:05:16.053563 vss-cli-2024.5.0.dev6/vss_cli/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 16:05:11.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15976 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/account.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/completion.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2024-05-24 16:04:34.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:05:16.057564 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8906 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/callbacks.py
--rw-rw-rw-   0 root         (0) root         (0)     4015 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/contentlib.py
--rw-rw-rw-   0 root         (0) root         (0)     2813 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/domain.py
--rw-rw-rw-   0 root         (0) root         (0)     3133 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/floppy.py
--rw-rw-rw-   0 root         (0) root         (0)     8680 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/helper.py
--rw-rw-rw-   0 root         (0) root         (0)     3287 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/image.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     3046 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/iso.py
--rw-rw-rw-   0 root         (0) root         (0)     3477 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/net.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/os.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/rel_args.py
--rw-rw-rw-   0 root         (0) root         (0)     9604 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/rel_opts.py
--rw-rw-rw-   0 root         (0) root         (0)     3790 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/template.py
--rw-rw-rw-   0 root         (0) root         (0)   150500 2024-05-24 16:04:34.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/vm.py
--rw-rw-rw-   0 root         (0) root         (0)     1907 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/vmdks.py
--rw-rw-rw-   0 root         (0) root         (0)    10871 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/configure.py
--rw-rw-rw-   0 root         (0) root         (0)     3481 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/key.py
--rw-rw-rw-   0 root         (0) root         (0)     3010 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/message.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     4310 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/ovf.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/plugins.py
--rw-rw-rw-   0 root         (0) root         (0)     1362 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/raw.py
--rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:05:16.057564 vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5330 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/change.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/export.py
--rw-rw-rw-   0 root         (0) root         (0)     2372 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     2362 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/image.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     2860 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/new.py
--rw-rw-rw-   0 root         (0) root         (0)     2366 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/restore.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/retirement.py
--rw-rw-rw-   0 root         (0) root         (0)     3307 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/snapshot.py
--rw-rw-rw-   0 root         (0) root         (0)     2246 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/vmdk.py
--rw-rw-rw-   0 root         (0) root         (0)     1614 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/service.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/shell.py
--rw-rw-rw-   0 root         (0) root         (0)     2325 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/status.py
--rw-rw-rw-   0 root         (0) root         (0)     6761 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/stor.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/token.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/plugins/upgrade.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/rel_opts.py
--rw-rw-rw-   0 root         (0) root         (0)     2864 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/sstatus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:05:16.057564 vss-cli-2024.5.0.dev6/vss_cli/utils/
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    75203 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/utils/emoji.py
--rw-rw-rw-   0 root         (0) root         (0)     2929 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/utils/threading.py
--rw-rw-rw-   0 root         (0) root         (0)     4734 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/vss.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/vssconst.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev6/vss_cli/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 16:05:16.057564 vss-cli-2024.5.0.dev6/vss_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13950 2024-05-24 16:05:16.000000 vss-cli-2024.5.0.dev6/vss_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2453 2024-05-24 16:05:16.000000 vss-cli-2024.5.0.dev6/vss_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 16:05:16.000000 vss-cli-2024.5.0.dev6/vss_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-24 16:05:16.000000 vss-cli-2024.5.0.dev6/vss_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 16:05:16.000000 vss-cli-2024.5.0.dev6/vss_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      732 2024-05-24 16:05:16.000000 vss-cli-2024.5.0.dev6/vss_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-24 16:05:16.000000 vss-cli-2024.5.0.dev6/vss_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.038016 vss-cli-2024.6.0.dev0/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13950 2024-05-27 16:01:16.038016 vss-cli-2024.6.0.dev0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10991 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2024-05-27 16:01:16.038016 vss-cli-2024.6.0.dev0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3827 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.022016 vss-cli-2024.6.0.dev0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5569 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/tests/test_vss_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.026016 vss-cli-2024.6.0.dev0/vss_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19671 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/autocompletion.py
+-rw-rw-rw-   0 root         (0) root         (0)     7659 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    65652 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15583 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.026016 vss-cli-2024.6.0.dev0/vss_cli/data/
+-rw-rw-rw-   0 root         (0) root         (0)     4500 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/data/clib.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4288 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/data/clone.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/data/config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/data/image.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2926 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/data/shell.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/data/template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    25960 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/hcio.py
+-rw-rw-rw-   0 root         (0) root         (0)    12512 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.030016 vss-cli-2024.6.0.dev0/vss_cli/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 16:01:11.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15976 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/completion.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2024-05-24 16:04:34.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.034016 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8906 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/callbacks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/contentlib.py
+-rw-rw-rw-   0 root         (0) root         (0)     2813 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3133 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/floppy.py
+-rw-rw-rw-   0 root         (0) root         (0)     8680 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3287 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/iso.py
+-rw-rw-rw-   0 root         (0) root         (0)     3477 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/net.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/os.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/rel_args.py
+-rw-rw-rw-   0 root         (0) root         (0)     9604 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/rel_opts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3790 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/template.py
+-rw-rw-rw-   0 root         (0) root         (0)   150500 2024-05-24 16:04:34.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/vm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1907 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/vmdks.py
+-rw-rw-rw-   0 root         (0) root         (0)    10871 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/key.py
+-rw-rw-rw-   0 root         (0) root         (0)     3010 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4310 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/ovf.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/raw.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.034016 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/change.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/export.py
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2362 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/new.py
+-rw-rw-rw-   0 root         (0) root         (0)     2366 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/restore.py
+-rw-rw-rw-   0 root         (0) root         (0)     3924 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/retirement.py
+-rw-rw-rw-   0 root         (0) root         (0)     3307 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/snapshot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2246 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/vmdk.py
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)     2325 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/status.py
+-rw-rw-rw-   0 root         (0) root         (0)     6761 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/stor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/token.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/upgrade.py
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2024-05-27 16:00:32.000000 vss-cli-2024.6.0.dev0/vss_cli/plugins/vpn.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/rel_opts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2864 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/sstatus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.034016 vss-cli-2024.6.0.dev0/vss_cli/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    75203 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/utils/emoji.py
+-rw-rw-rw-   0 root         (0) root         (0)     2929 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/utils/threading.py
+-rw-rw-rw-   0 root         (0) root         (0)     4734 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/vss.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/vssconst.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2024-05-21 00:52:44.000000 vss-cli-2024.6.0.dev0/vss_cli/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 16:01:16.034016 vss-cli-2024.6.0.dev0/vss_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13950 2024-05-27 16:01:15.000000 vss-cli-2024.6.0.dev0/vss_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2476 2024-05-27 16:01:16.000000 vss-cli-2024.6.0.dev0/vss_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 16:01:15.000000 vss-cli-2024.6.0.dev0/vss_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-27 16:01:15.000000 vss-cli-2024.6.0.dev0/vss_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 16:01:15.000000 vss-cli-2024.6.0.dev0/vss_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      732 2024-05-27 16:01:16.000000 vss-cli-2024.6.0.dev0/vss_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-27 16:01:16.000000 vss-cli-2024.6.0.dev0/vss_cli.egg-info/top_level.txt
```

### Comparing `vss-cli-2024.5.0.dev6/LICENSE` & `vss-cli-2024.6.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/PKG-INFO` & `vss-cli-2024.6.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vss-cli
-Version: 2024.5.0.dev6
+Version: 2024.6.0.dev0
 Summary: ITS Private Cloud Command Line Interface
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.5.0-dev6.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.6.0-dev0.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/issues
 Project-URL: Documentation, https://eis.utoronto.ca/~vss/vss-cli/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Systems Administration
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyvss==2024.5.0
+Requires-Dist: pyvss>=2024.5.0
 Requires-Dist: click==8.1.7
 Requires-Dist: click-log==0.4.0
 Requires-Dist: click-plugins==1.1.1
 Requires-Dist: click-repl==0.2.0
 Requires-Dist: click-threading==0.5.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: jsonpath-ng<2,>=1.5.1
```

### Comparing `vss-cli-2024.5.0.dev6/README.md` & `vss-cli-2024.6.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/setup.cfg` & `vss-cli-2024.6.0.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/setup.py` & `vss-cli-2024.6.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/tests/test_vss_cli.py` & `vss-cli-2024.6.0.dev0/tests/test_vss_cli.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/autocompletion.py` & `vss-cli-2024.6.0.dev0/vss_cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/cli.py` & `vss-cli-2024.6.0.dev0/vss_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,14 +233,22 @@
     '--s3-server',
     '-w',
     help='The Webdav server.',
     default=None,
     show_default=True,
     envvar='VSS_S3_SERVER',
 )
+@click.option(
+    '--vpn-server',
+    '-vpn',
+    help='The VPN server.',
+    default=None,
+    show_default=True,
+    envvar='VSS_VPN_SERVER',
+)
 @click.version_option(
     version=f'{const.__version__} ('
     f'pyvss/{pyvss_version} '
     f'{platform.python_implementation()}/{platform.python_version()})',
     message='%(prog)s v%(version)s',
 )
 @pass_context
@@ -260,14 +268,15 @@
     columns: str,
     columns_width: int,
     no_headers: bool,
     table_format: str,
     sort_by: Optional[str],
     wait: Optional[bool],
     s3_server: Optional[str],
+    vpn_server: Optional[str],
 ):
     """Command line interface for the ITS Private Cloud."""
     ctx.verbose = verbose
     ctx.endpoint = endpoint
     ctx.token = token
     ctx.config_path = config
     ctx.username = username
@@ -280,9 +289,10 @@
     ctx.columns = to_tuples(columns)
     ctx.columns_width = columns_width
     ctx.no_headers = no_headers
     ctx.table_format = table_format
     ctx.sort_by = sort_by  # type: ignore
     ctx.wait_for_requests = wait
     ctx.s3_server = s3_server
+    ctx.vpn_server = vpn_server
 
     _LOGGER.debug(f"Using settings: {ctx}")
```

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/config.py` & `vss-cli-2024.6.0.dev0/vss_cli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,16 @@
         self._endpoint = const.DEFAULT_ENDPOINT  # type: str
         self.base_endpoint = self.endpoint  # type: str
         self.endpoint_name = const.DEFAULT_ENDPOINT_NAME
         # end of endpoint settings
         self.history = const.DEFAULT_HISTORY  # type: str
         self.s3_server = None  # type: Optional[str]
         self._s3_server = const.DEFAULT_S3_SERVER  # type: str
+        self.vpn_server = None  # type: Optional[str]
+        self._vpn_server = const.DEFAULT_VPN_SERVER
         self.username = None  # type: Optional[str]
         self.password = None  # type: Optional[str]
         self.totp = None  # type: Optional[str]
         self.token = None  # type: Optional[str]
         self.timeout = None  # type: Optional[int]
         self._debug = False  # type: Optional[bool]
         self.showexceptions = False  # type: bool
@@ -190,14 +192,15 @@
             "output": self.output,
             "timeout": self.timeout,
             "debug": self.debug,
             "verbose": self.verbose,
             "wait": self.wait,
             "dry_run": self.dry_run,
             "s3_server": self.s3_server,
+            "vpn_server": self.vpn_server,
         }
 
         return f"<Configuration({view})"
 
     def auto_output(self, auto_output: str) -> str:
         """Configure output format."""
         if self.output == "auto":
@@ -886,14 +889,33 @@
         )
         _LOGGING.debug(
             f's3_endpoint={self.vskey_stor_s3api} '
             f'vskey_stor_s3_gui={self.vskey_stor_s3_gui}'
         )
         return self.vskey_stor
 
+    def enable_vss_vpn(self, **kwargs):
+        """Enable VPN."""
+        self.init_vss_vpn(self.vpn_server)
+        _LOGGING.debug(f'{self.totp=} {self.username=} -> {self.vpn_server=}')
+        rv = super().enable_vss_vpn(
+            user=self.username, password=self.password, otp=self.totp
+        )
+        return rv
+
+    def disable_vss_vpn(self, **kwargs):
+        """Disable VPN."""
+        self.init_vss_vpn(self.vpn_server)
+        _LOGGING.debug(f'{self.username=} -> {self.vpn_server=}')
+        rv = super().disable_vss_vpn(
+            user=self.username,
+            password=self.password,
+        )
+        return rv
+
     def get_vm_by_id_or_name(self, vm_id: str, silent=False) -> Optional[List]:
         """Get virtual machine by identifier or name."""
         is_moref = validate_vm_moref('', '', vm_id)
         is_uuid = validate_uuid('', '', vm_id)
         _LOGGING.debug(f'is_moref={is_moref}, is_uuid={is_uuid}')
         if is_moref or is_uuid:
             if is_moref:
```

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/const.py` & `vss-cli-2024.6.0.dev0/vss_cli/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Constants used by VSS CLI (vss-cli)."""
 import os
 from importlib import resources
 
 PACKAGE_NAME = "vss_cli"
 
-__version__ = "2024.5.0-dev6"
+__version__ = "2024.6.0-dev0"
 
 
 DEFAULT_TIMEOUT = 30
 DEFAULT_ENDPOINT = "https://cloud-api.eis.utoronto.ca"
 DEFAULT_ENDPOINT_NAME = "cloud-api"
 DEFAULT_S3_SERVER = "https://vskey-stor.eis.utoronto.ca"
+DEFAULT_VPN_SERVER = "https://vskey-vn.eis.utoronto.ca"
 _LEGACY_CONFIG = ("~", ".vss-cli", "config.json")
 _DEFAULT_CONFIG = ("~", ".vss-cli", "config.yaml")
 _DEFAULT_HISTORY = ("~", ".vss-cli", "history")
 RAW_ALLOWED_DOMAINS_REGEX = r'https?:\/\/.*\.?utoronto\.(ca|edu):?\d*\/?.*'
 
 COLUMNS_WIDTH_DEFAULT = -1
 COLUMNS_WIDTH_STR = "\u2026"
@@ -37,14 +38,15 @@
 DEFAULT_COLUMNS_WIDTH = -1
 DEFAULT_WAIT_FOR_REQUESTS = False
 
 DEFAULT_SETTINGS = {
     "endpoint": DEFAULT_ENDPOINT,
     "output": DEFAULT_OUTPUT,
     "s3_server": DEFAULT_S3_SERVER,
+    "vpn_server": DEFAULT_VPN_SERVER,
     "table_format": DEFAULT_TABLE_FORMAT,
     "check_for_messages": DEFAULT_CHECK_MESSAGES,
     "check_for_updates": DEFAULT_CHECK_UPDATES,
     "timeout": DEFAULT_TIMEOUT,
     "verbose": DEFAULT_VERBOSE,
     "debug": DEFAULT_DEBUG,
 }
@@ -55,14 +57,15 @@
     "check_for_messages": bool,
     "check_for_updates": bool,
     "debug": bool,
     "verbose": bool,
     "default_endpoint_name": str,
     "output": str,
     "s3_server": str,
+    "vpn_server": str,
     "table_format": str,
     "timeout": int,
     "columns_width": int,
     "wait_for_requests": bool,
 }
 
 DEFAULT_HOST_REGEX = (
```

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/data/clib.yaml` & `vss-cli-2024.6.0.dev0/vss_cli/data/clib.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from CLib 2024.5.0-dev6             #
+#     VSS-CLI Spec from CLib 2024.6.0-dev0             #
 ####################################################
 built: clib               # Required: Do not remove.
 machine:
   item: ubuntu-22.04      # Required: Source content library id OVF.
   cpu: 1                  # Optional: CPU count (Default: 1).
   memory: 1               # Optional: Memory in GB (Default: 1GB).
   name: &name Vm-Name     # Required: Target virtual machine name.
```

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/data/clone.yaml` & `vss-cli-2024.6.0.dev0/vss_cli/data/clone.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from Clone 2024.5.0-dev6             #
+#     VSS-CLI Spec from Clone 2024.6.0-dev0             #
 ####################################################
 built: clone              # Required: Do not remove.
 machine:
   source: SourceVM        # Required: Can be a vm name or a vm id.
   name: &name Vm-Name     # Required: Target virtual machine name
   disks:                  # Optional: Disks (Default: source vm disk layout)
     - capacity_gb: 40     # Optional: Disk capacity in GB (Default: source vm disk capacity)
```

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/data/config.yaml` & `vss-cli-2024.6.0.dev0/vss_cli/data/config.yaml`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/data/image.yaml` & `vss-cli-2024.6.0.dev0/vss_cli/data/image.yaml`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/data/shell.yaml` & `vss-cli-2024.6.0.dev0/vss_cli/data/shell.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec shell VM 2024.5.0-dev6             #
+#     VSS-CLI Spec shell VM 2024.6.0-dev0             #
 ####################################################
 built: os_install         # Required: Do not remove.
 machine:
   name: Vm-Name            # Required: Target virtual machine name.
   os: ubuntu64Guest              # Required: Guest Operating System name or Id.
   cpu: 1                   # Optional: CPU count (Default: 1).
   memory: 1                # Optional: Memory in GB (Default: 1GB).
```

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/data/template.yaml` & `vss-cli-2024.6.0.dev0/vss_cli/data/template.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from Template 2024.5.0-dev6        #
+#     VSS-CLI Spec from Template 2024.6.0-dev0        #
 ####################################################
 built: template           # Required: Do not remove.
 machine:
   source: NixSource                # Required: Can be a vm name or a vm id.
   name: &name Vm-Name     # Required: Target virtual machine name
   folder: MyFolder       # Optional: Folder name, path or ID (Default: source vm folder)
   disks:                  # Optional: Disks (Default: source vm disk layout)
```

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/data_types.py` & `vss-cli-2024.6.0.dev0/vss_cli/data_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Data types definitions."""
+import logging
+import re
 from dataclasses import dataclass, field
 from ipaddress import (
     AddressValueError, IPv4Address, IPv4Network, NetmaskValueError)
-import logging
 from pathlib import Path
-import re
 from typing import Dict, List, Optional, Tuple, Union
 
 from click import BadArgumentUsage, BadParameter
-from dataclasses_json import config as dc_config, dataclass_json
+from dataclasses_json import config as dc_config
+from dataclasses_json import dataclass_json
 from ruamel.yaml import YAML
 from ruamel.yaml.scanner import ScannerError
-from validators import (
-    domain as is_domain, email as is_email_address, url as is_url)
+from validators import domain as is_domain
+from validators import email as is_email_address
+from validators import url as is_url
 
 import vss_cli.const as const
 from vss_cli.exceptions import ValidationError
 from vss_cli.validators import validate_email
 
 _LOGGING = logging.getLogger(__name__)
 
@@ -37,14 +39,15 @@
 class ConfigFileGeneral:
     """Configuration General section class."""
 
     check_for_updates: bool = const.DEFAULT_CHECK_UPDATES
     check_for_messages: bool = const.DEFAULT_CHECK_MESSAGES
     default_endpoint_name: str = const.DEFAULT_ENDPOINT_NAME
     s3_server: str = const.DEFAULT_S3_SERVER
+    vpn_server: str = const.DEFAULT_VPN_SERVER
     debug: bool = const.DEFAULT_DEBUG
     output: str = const.DEFAULT_RAW_OUTPUT
     table_format: str = const.DEFAULT_TABLE_FORMAT
     timeout: int = const.DEFAULT_TIMEOUT
     verbose: bool = const.DEFAULT_VERBOSE
     columns_width: int = const.DEFAULT_COLUMNS_WIDTH
     wait_for_requests: bool = const.DEFAULT_WAIT_FOR_REQUESTS
```

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/hcio.py` & `vss-cli-2024.6.0.dev0/vss_cli/hcio.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/helper.py` & `vss-cli-2024.6.0.dev0/vss_cli/helper.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/account.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/account.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/completion.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/completion.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/callbacks.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/callbacks.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/contentlib.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/contentlib.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/domain.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/domain.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/floppy.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/floppy.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/folder.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/folder.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/helper.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/helper.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/image.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/image.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/inventory.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/inventory.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/iso.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/iso.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/net.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/net.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/os.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/os.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/rel_args.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/rel_args.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/rel_opts.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/rel_opts.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/template.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/template.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/vm.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/vm.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/compute_plugins/vmdks.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/compute_plugins/vmdks.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/configure.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/configure.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/key.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/key.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/message.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/message.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/misc.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/misc.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/ovf.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/ovf.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/plugins.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/raw.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/raw.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/request.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/request.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/change.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/change.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/export.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/export.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/folder.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/folder.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/image.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/image.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/inventory.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/inventory.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/new.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/new.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/restore.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/restore.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/retirement.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/retirement.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/snapshot.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/snapshot.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/request_plugins/vmdk.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/request_plugins/vmdk.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/service.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/service.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/shell.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/status.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/status.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/stor.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/stor.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/token.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/token.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/plugins/upgrade.py` & `vss-cli-2024.6.0.dev0/vss_cli/plugins/upgrade.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/rel_opts.py` & `vss-cli-2024.6.0.dev0/vss_cli/rel_opts.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/sstatus.py` & `vss-cli-2024.6.0.dev0/vss_cli/sstatus.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/utils/emoji.py` & `vss-cli-2024.6.0.dev0/vss_cli/utils/emoji.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/utils/threading.py` & `vss-cli-2024.6.0.dev0/vss_cli/utils/threading.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/validators.py` & `vss-cli-2024.6.0.dev0/vss_cli/validators.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/vss.py` & `vss-cli-2024.6.0.dev0/vss_cli/vss.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli/yaml.py` & `vss-cli-2024.6.0.dev0/vss_cli/yaml.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2024.5.0.dev6/vss_cli.egg-info/PKG-INFO` & `vss-cli-2024.6.0.dev0/vss_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vss-cli
-Version: 2024.5.0.dev6
+Version: 2024.6.0.dev0
 Summary: ITS Private Cloud Command Line Interface
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.5.0-dev6.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.6.0-dev0.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/issues
 Project-URL: Documentation, https://eis.utoronto.ca/~vss/vss-cli/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Systems Administration
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyvss==2024.5.0
+Requires-Dist: pyvss>=2024.5.0
 Requires-Dist: click==8.1.7
 Requires-Dist: click-log==0.4.0
 Requires-Dist: click-plugins==1.1.1
 Requires-Dist: click-repl==0.2.0
 Requires-Dist: click-threading==0.5.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: jsonpath-ng<2,>=1.5.1
```

### Comparing `vss-cli-2024.5.0.dev6/vss_cli.egg-info/SOURCES.txt` & `vss-cli-2024.6.0.dev0/vss_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 vss_cli/plugins/request.py
 vss_cli/plugins/service.py
 vss_cli/plugins/shell.py
 vss_cli/plugins/status.py
 vss_cli/plugins/stor.py
 vss_cli/plugins/token.py
 vss_cli/plugins/upgrade.py
+vss_cli/plugins/vpn.py
 vss_cli/plugins/compute_plugins/__init__.py
 vss_cli/plugins/compute_plugins/callbacks.py
 vss_cli/plugins/compute_plugins/contentlib.py
 vss_cli/plugins/compute_plugins/domain.py
 vss_cli/plugins/compute_plugins/floppy.py
 vss_cli/plugins/compute_plugins/folder.py
 vss_cli/plugins/compute_plugins/helper.py
```

### Comparing `vss-cli-2024.5.0.dev6/vss_cli.egg-info/requires.txt` & `vss-cli-2024.6.0.dev0/vss_cli.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pyvss==2024.5.0
+pyvss>=2024.5.0
 click==8.1.7
 click-log==0.4.0
 click-plugins==1.1.1
 click-repl==0.2.0
 click-threading==0.5.0
 tabulate==0.9.0
 jsonpath-ng<2,>=1.5.1
```

