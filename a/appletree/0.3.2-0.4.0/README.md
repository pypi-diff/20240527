# Comparing `tmp/appletree-0.3.2.tar.gz` & `tmp/appletree-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appletree-0.3.2.tar", last modified: Wed Mar  6 08:24:42 2024, max compression
+gzip compressed data, was "appletree-0.4.0.tar", last modified: Mon May 27 19:53:07 2024, max compression
```

## Comparing `appletree-0.3.2.tar` & `appletree-0.4.0.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:24:42.917591 appletree-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-06 08:24:37.000000 appletree-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-03-06 08:24:42.917591 appletree-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-03-06 08:24:37.000000 appletree-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:24:42.909591 appletree-0.3.2/appletree/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22988 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:24:42.913591 appletree-0.3.2/appletree/components/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/components/ac.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/components/er.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/components/nr.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/components/yields.py
--rw-r--r--   0 runner    (1001) docker     (127)    17700 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:24:42.913591 appletree-0.3.2/appletree/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/contexts/er_only.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:24:42.913591 appletree-0.3.2/appletree/data/
--rw-r--r--   0 runner    (1001) docker     (127)   160762 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/data/AC_Rn220.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    20522 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/data/data_Ar37.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/data/data_Neutron.csv
--rw-r--r--   0 runner    (1001) docker     (127)    47270 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/data/data_Rn220.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/hist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:24:42.913591 appletree-0.3.2/appletree/instructs/
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/instructs/literature_lyqy.json
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/instructs/neutron_low.json
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/instructs/rn220.json
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/instructs/rn220_ar37.json
--rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    20448 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:24:42.913591 appletree-0.3.2/appletree/maps/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/maps/_3fold_recon_eff.json
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/maps/_elife.json
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/maps/_gas_gain_relative.json
--rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/maps/_nr_ly.json
--rw-r--r--   0 runner    (1001) docker     (127)    15790 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/maps/_nr_qy.json
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/maps/_nr_spectrum.json
--rw-r--r--   0 runner    (1001) docker     (127)     9979 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/maps/_posrec_reso.json
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/maps/_s1_bias.json
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/maps/_s1_correction.json
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/maps/_s1_cut_acc.json
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/maps/_s1_smearing.json
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/maps/_s2_bias.json
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/maps/_s2_correction.json
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/maps/_s2_cut_acc.json
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/maps/_s2_smearing.json
--rw-r--r--   0 runner    (1001) docker     (127)     9575 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:24:42.917591 appletree-0.3.2/appletree/parameters/
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/parameters/er.json
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/parameters/nestv2.json
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/parameters/nr_low.json
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:24:42.917591 appletree-0.3.2/appletree/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/plugins/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/plugins/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/plugins/efficiency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/plugins/er_microphys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/plugins/lyqy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/plugins/nestv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/plugins/reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/randgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/share.py
--rw-r--r--   0 runner    (1001) docker     (127)    18643 2024-03-06 08:24:37.000000 appletree-0.3.2/appletree/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:24:42.909591 appletree-0.3.2/appletree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-03-06 08:24:42.000000 appletree-0.3.2/appletree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-03-06 08:24:42.000000 appletree-0.3.2/appletree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 08:24:42.000000 appletree-0.3.2/appletree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 08:24:42.000000 appletree-0.3.2/appletree.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-06 08:24:42.000000 appletree-0.3.2/appletree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-06 08:24:42.000000 appletree-0.3.2/appletree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-06 08:24:42.917591 appletree-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-03-06 08:24:37.000000 appletree-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:53:07.753192 appletree-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-27 19:53:04.000000 appletree-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-27 19:53:07.753192 appletree-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-27 19:53:04.000000 appletree-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:53:07.745192 appletree-0.4.0/appletree/
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23580 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:53:07.749192 appletree-0.4.0/appletree/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/components/ac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/components/er.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/components/nr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/components/yields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17700 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:53:07.749192 appletree-0.4.0/appletree/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/contexts/er_only.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:53:07.749192 appletree-0.4.0/appletree/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   160762 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/data/AC_Rn220.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    20522 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/data/data_Ar37.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/data/data_Neutron.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    47270 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/data/data_Rn220.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/hist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:53:07.749192 appletree-0.4.0/appletree/instructs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/instructs/literature_lyqy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/instructs/neutron_low.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/instructs/rn220.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/instructs/rn220_ar37.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22274 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:53:07.753192 appletree-0.4.0/appletree/maps/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/maps/_3fold_recon_eff.json
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/maps/_elife.json
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/maps/_gas_gain_relative.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/maps/_nr_ly.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15790 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/maps/_nr_qy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/maps/_nr_spectrum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9979 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/maps/_posrec_reso.json
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/maps/_s1_bias.json
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/maps/_s1_correction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/maps/_s1_cut_acc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/maps/_s1_smearing.json
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/maps/_s2_bias.json
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/maps/_s2_correction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/maps/_s2_cut_acc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/maps/_s2_smearing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9575 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:53:07.753192 appletree-0.4.0/appletree/parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/parameters/er.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/parameters/er_rn220_ar37.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/parameters/nestv2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/parameters/nr_low.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12005 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:53:07.753192 appletree-0.4.0/appletree/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/plugins/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/plugins/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/plugins/efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/plugins/er_microphys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/plugins/lyqy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/plugins/nestv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/plugins/reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16720 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/randgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/share.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18659 2024-05-27 19:53:04.000000 appletree-0.4.0/appletree/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:53:07.749192 appletree-0.4.0/appletree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-27 19:53:07.000000 appletree-0.4.0/appletree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-27 19:53:07.000000 appletree-0.4.0/appletree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:53:07.000000 appletree-0.4.0/appletree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:53:07.000000 appletree-0.4.0/appletree.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-27 19:53:07.000000 appletree-0.4.0/appletree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 19:53:07.000000 appletree-0.4.0/appletree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-27 19:53:07.753192 appletree-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-27 19:53:04.000000 appletree-0.4.0/setup.py
```

### Comparing `appletree-0.3.2/LICENSE` & `appletree-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/PKG-INFO` & `appletree-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appletree
-Version: 0.3.2
+Version: 0.4.0
 Summary: A high-Performance Program simuLatEs and fiTs REsponse of xEnon.
 Home-page: https://github.com/XENONnT/appletree
 Author: Appletree contributors, the XENON collaboration
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -83,14 +83,31 @@
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 
+v0.4.0 / 2024-05-27
+-------------------
+* Try using jax.random.binomial by @dachengx in https://github.com/XENONnT/appletree/pull/148
+* Turn off add_eps_to_hist in NR and ER by @FaroutYLq in https://github.com/XENONnT/appletree/pull/152
+* Debug when `bins_type` is not set by @dachengx in https://github.com/XENONnT/appletree/pull/153
+* Specifically install `lxml_html_clean` by @dachengx in https://github.com/XENONnT/appletree/pull/157
+* Initialize context from backend by @zihaoxu98 in https://github.com/XENONnT/appletree/pull/156
+* Add `parameter_alias` to translate parameters in `par_config` by @dachengx in https://github.com/XENONnT/appletree/pull/160
+* Allow user to aggressively use memory by @dachengx in https://github.com/XENONnT/appletree/pull/164
+* Fix a bug of plotter which contains inf by @zihaoxu98 in https://github.com/XENONnT/appletree/pull/165
+
+New Contributors
+* @FaroutYLq made their first contribution in https://github.com/XENONnT/appletree/pull/152
+
+**Full Changelog**: https://github.com/XENONnT/appletree/compare/v0.3.2...v0.4.0
+
+
 v0.3.2 / 2024-03-06
 -------------------
 * Remove `scikit-learn` version requirement by @dachengx in https://github.com/XENONnT/appletree/pull/131
 * Use trusted publisher because username/password authentication is no longer supported by @dachengx in https://github.com/XENONnT/appletree/pull/132
 * Be compatible with `JAX_ENABLE_X64=1` by @dachengx in https://github.com/XENONnT/appletree/pull/134
 * Raise more information when file can not be found by @dachengx in https://github.com/XENONnT/appletree/pull/135
 * Preserve dtype of results in `multiple_simulations` by @dachengx in https://github.com/XENONnT/appletree/pull/137
```

### Comparing `appletree-0.3.2/README.md` & `appletree-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/component.py` & `appletree-0.4.0/appletree/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     """Base class of component."""
 
     # Do not initialize this class because it is base
     __is_base = True
 
     rate_name: str = ""
     norm_type: str = ""
+    # add_eps_to_hist==True was introduced as only a workaround
+    # for likelihood blowup problem when using meshgrid binning
     add_eps_to_hist: bool = True
     force_no_eff: bool = False
 
     def __init__(self, name: Optional[str] = None, llh_name: Optional[str] = None, **kwargs):
         """Initialization.
 
         Args:
@@ -47,20 +49,29 @@
         else:
             self.llh_name = llh_name
         self.needed_parameters: Set[str] = set()
 
         if "bins" in kwargs.keys() and "bins_type" in kwargs.keys():
             self.set_binning(**kwargs)
 
+            if self.bins_type != "meshgrid" and self.add_eps_to_hist:
+                warn(
+                    "It is empirically dangerous to have add_eps_to_hist==True, "
+                    "when your bins_type is not meshgrid! It may lead to very bad fit with "
+                    "lots of eff==0."
+                )
+
     def set_binning(self, **kwargs):
         """Set binning of component."""
         if "bins" not in kwargs.keys() or "bins_type" not in kwargs.keys():
             raise ValueError("bins and bins_type must be set!")
         self.bins = kwargs.get("bins")
         self.bins_type = kwargs.get("bins_type")
+        if self.bins_type not in ["irreg", "meshgrid", None]:
+            raise ValueError(f"Unsupported bins_type {self.bins_type}!")
 
         if self.bins_type == "meshgrid":
             warning = "The usage of meshgrid binning is highly discouraged."
             warn(warning)
 
     def _clip(self, result: list):
         """Clip simulated result."""
@@ -539,15 +550,15 @@
         """Generate new component with same binning, usually used on predicting yields."""
         if pass_binning:
             if hasattr(self, "bins") and hasattr(self, "bins_type"):
                 component = self.__class__(
                     name=self.name + "_copy",
                     llh_name=llh_name,
                     bins=self.bins,
-                    bins_type=self.bins,
+                    bins_type=self.bins_type,
                 )
             else:
                 raise ValueError("Should provide bins and bins_type if you want to pass binning!")
         else:
             component = self.__class__(
                 name=self.name + "_copy",
                 llh_name=llh_name,
```

### Comparing `appletree-0.3.2/appletree/components/er.py` & `appletree-0.4.0/appletree/components/er.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import appletree as apt
 
 from appletree.component import ComponentSim
 
 
 class ERBand(ComponentSim):
     norm_type = "on_pdf"
+    add_eps_to_hist = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.register(apt.plugins.common.UniformEnergySpectra)
         self.register(apt.plugins.common.PositionSpectra)
         self.register_all(apt.plugins.er_microphys)
         self.register_all(apt.plugins.detector)
         self.register_all(apt.plugins.reconstruction)
         self.register_all(apt.plugins.efficiency)
 
 
 class ERPeak(ComponentSim):
     norm_type = "on_pdf"
+    add_eps_to_hist = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.register(apt.plugins.common.MonoEnergySpectra)
         self.register(apt.plugins.common.PositionSpectra)
         self.register_all(apt.plugins.er_microphys)
```

### Comparing `appletree-0.3.2/appletree/components/nr.py` & `appletree-0.4.0/appletree/components/nr.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import appletree as apt
 
 from appletree.component import ComponentSim
 
 
 class NR(ComponentSim):
     norm_type = "on_pdf"
+    add_eps_to_hist = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.register(apt.plugins.common.FixedEnergySpectra)
         self.register(apt.plugins.common.PositionSpectra)
         self.register_all(apt.plugins.lyqy)
```

### Comparing `appletree-0.3.2/appletree/components/yields.py` & `appletree-0.4.0/appletree/components/yields.py`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/config.py` & `appletree-0.4.0/appletree/config.py`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/context.py` & `appletree-0.4.0/appletree/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import emcee
 import h5py
 
 import appletree as apt
 from appletree import randgen
 from appletree import Parameter
-from appletree.utils import load_json
+from appletree.utils import load_json, get_file_path
 from appletree.share import _cached_configs, set_global_config
 
 os.environ["OMP_NUM_THREADS"] = "1"
 
 
 class Context:
     """Combine all likelihood (e.g. Rn220, Ar37), handle MCMC and post-fitting analysis."""
@@ -51,14 +51,25 @@
             self.par_config = self.get_parameter_config(instruct["par_config"])
         self.needed_parameters = self.update_parameter_config(instruct["likelihoods"])
 
         self.par_manager = Parameter(self.par_config)
 
         self.register_all_likelihood(instruct)
 
+    @classmethod
+    def from_backend(cls, backend_h5_file_name):
+        """Initialize context from a backend_h5 file."""
+        with h5py.File(get_file_path(backend_h5_file_name)) as file:
+            instruct = eval(file["mcmc"].attrs["instruct"])
+            nwalkers = file["mcmc"].attrs["nwalkers"]
+            batch_size = file["mcmc"].attrs["batch_size"]
+        tree = cls(instruct)
+        tree.pre_fitting(nwalkers, batch_size=batch_size)
+        return tree
+
     def __getitem__(self, keys):
         """Get likelihood in context."""
         return self.likelihoods[keys]
 
     def register_all_likelihood(self, config):
         """Create all appletree likelihoods.
 
@@ -170,27 +181,27 @@
 
         return log_posterior, log_prior
 
     @property
     def _ndim(self):
         return len(self.par_manager.parameter_fit_array)
 
-    def _set_backend(self, nwalkers=100, read_only=True):
+    def _set_backend(self, nwalkers=100, read_only=True, reset=False):
         if self.backend_h5 is None:
             self._backend = None
             print("With no backend")
         else:
             self._backend = emcee.backends.HDFBackend(self.backend_h5, read_only=read_only)
-            if not read_only:
+            if reset:
                 self._backend.reset(nwalkers, self._ndim)
             print(f"With h5 backend {self.backend_h5}")
 
-    def pre_fitting(self, nwalkers=100, read_only=True, batch_size=1_000_000):
+    def pre_fitting(self, nwalkers=100, read_only=True, reset=False, batch_size=1_000_000):
         """Prepare for fitting, initialize backend and sampler."""
-        self._set_backend(nwalkers, read_only=read_only)
+        self._set_backend(nwalkers, read_only=read_only, reset=reset)
         self.sampler = emcee.EnsembleSampler(
             nwalkers,
             self._ndim,
             self.log_posterior,
             backend=self._backend,
             blobs_dtype=np.float32,
             parameter_names=self.par_manager.parameter_fit,
@@ -208,52 +219,57 @@
         self._sanity_check()
 
         p0 = []
         for _ in range(nwalkers):
             self.par_manager.sample_init()
             p0.append(self.par_manager.parameter_fit_array)
 
-        self.pre_fitting(nwalkers=nwalkers, read_only=False, batch_size=batch_size)
+        self.pre_fitting(nwalkers=nwalkers, read_only=False, reset=True, batch_size=batch_size)
 
         result = self.sampler.run_mcmc(
             p0,
             iteration,
             store=True,
             progress=True,
         )
 
-        self._dump_meta()
+        self._dump_meta(batch_size=batch_size)
         return result
 
-    def continue_fitting(self, context, iteration=500, batch_size=1_000_000):
+    def continue_fitting(self, context=None, iteration=500, batch_size=1_000_000):
         """Continue a fitting of another context.
 
         Args:
             context: appletree context.
             iteration: int, number of steps to generate.
 
         """
-        # Final iteration
-        final_iteration = context.sampler.get_chain()[-1, :, :]
-        p0 = final_iteration.tolist()
+        # If context is None, use self, i.e. continue the fitting defined in self
+        if context is None:
+            context = self
+            p0 = None
+        else:
+            # Final iteration
+            final_iteration = context.sampler.get_chain()[-1, :, :]
+            p0 = final_iteration.tolist()
 
-        nwalkers = len(p0)
+        nwalkers = context.sampler.get_chain().shape[1]
 
         # Init sampler for current context
-        self.pre_fitting(nwalkers=nwalkers, read_only=False, batch_size=batch_size)
+        self.pre_fitting(nwalkers=nwalkers, read_only=False, reset=False, batch_size=batch_size)
 
         result = self.sampler.run_mcmc(
             p0,
             iteration,
             store=True,
             progress=True,
             skip_initial_state_check=True,
         )
 
-        self._dump_meta()
+        self._dump_meta(batch_size=batch_size)
         return result
 
     def get_post_parameters(self):
         """Get parameters correspondes to max posterior."""
         logp = self.sampler.get_log_prob(flat=True)
         chain = self.sampler.get_chain(flat=True)
         mpe_parameters = chain[np.argmax(logp)]
@@ -272,15 +288,15 @@
 
     def dump_post_parameters(self, file_name):
         """Dump max posterior parameter in .json file."""
         parameters = self.get_post_parameters()
         with open(file_name, "w") as fp:
             json.dump(parameters, fp)
 
-    def _dump_meta(self, metadata=None):
+    def _dump_meta(self, batch_size, metadata=None):
         """Save parameters name as attributes."""
         if metadata is None:
             metadata = {
                 "version": apt.__version__,
                 "date": datetime.now().strftime("%Y%m%d_%H:%M:%S"),
             }
         if self.backend_h5 is not None:
@@ -295,14 +311,16 @@
                 opt[name].attrs["parameter_fit"] = self.par_manager.parameter_fit
                 # instructions
                 opt[name].attrs["instruct"] = json.dumps(self.instruct)
                 # configs
                 opt[name].attrs["config"] = json.dumps(self.config)
                 # configurations, maybe users will manually add some maps
                 opt[name].attrs["_cached_configs"] = json.dumps(_cached_configs)
+                # batch size
+                opt[name].attrs["batch_size"] = batch_size
 
     def get_template(
         self,
         likelihood_name: str,
         component_name: str,
         batch_size: int = 1_000_000,
         seed: Optional[int] = None,
```

### Comparing `appletree-0.3.2/appletree/contexts/er_only.py` & `appletree-0.4.0/appletree/contexts/er_only.py`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/data/AC_Rn220.pkl` & `appletree-0.4.0/appletree/data/AC_Rn220.pkl`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/data/data_Ar37.csv` & `appletree-0.4.0/appletree/data/data_Ar37.csv`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/data/data_Neutron.csv` & `appletree-0.4.0/appletree/data/data_Neutron.csv`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/data/data_Rn220.csv` & `appletree-0.4.0/appletree/data/data_Rn220.csv`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/hist.py` & `appletree-0.4.0/appletree/hist.py`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/instructs/literature_lyqy.json` & `appletree-0.4.0/appletree/instructs/literature_lyqy.json`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/instructs/neutron_low.json` & `appletree-0.4.0/appletree/instructs/neutron_low.json`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/instructs/rn220.json` & `appletree-0.4.0/appletree/instructs/rn220.json`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/interpolation.py` & `appletree-0.4.0/appletree/interpolation.py`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/likelihood.py` & `appletree-0.4.0/appletree/likelihood.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,71 @@
 from warnings import warn
 from typing import Type, Dict, Set, Optional, cast
+import inspect
+from copy import deepcopy
 
 import numpy as np
 from jax import numpy as jnp
 
 from scipy.stats import norm
 
 from appletree import randgen
 from appletree.hist import make_hist_mesh_grid, make_hist_irreg_bin_1d, make_hist_irreg_bin_2d
 from appletree.utils import load_data, get_equiprob_bins_1d, get_equiprob_bins_2d
 from appletree.component import Component, ComponentSim, ComponentFixed
 from appletree.randgen import TwoHalfNorm, BandTwoHalfNorm
 
 
+def need_replacing_alias(func):
+    """Decorator to replace alias in parameters from key to value."""
+
+    def wrapper(self, *args, **kwargs):
+        sig = inspect.signature(func)
+        bound = sig.bind(self, *args, **kwargs)
+        bound.apply_defaults()
+
+        # Check if 'parameters' is in the arguments and replace aliases
+        if "parameters" in bound.arguments:
+            # Replace alias in 'parameters'
+            bound.arguments["parameters"] = self.replace_alias(bound.arguments["parameters"])
+        else:
+            raise ValueError(f"'parameters' must be in the arguments of {func.__name__}!")
+
+        # Call the function with possibly modified arguments
+        return func(*bound.args, **bound.kwargs)
+
+    return wrapper
+
+
 class Likelihood:
     """Combine all components (e.g. ER, AC, Wall), and calculate log posterior likelihood."""
 
     def __init__(self, name: Optional[str] = None, **config):
         """Create an appletree likelihood.
 
         Args:
             config: Dictionary with configuration options that will be applied, should include:
                 * data_file_name: the data used in fitting, usually calibration data
                 * bins_type: either meshgrid or equiprob
                 * bins_on: observables where we will perform inference on, usually [cs1, cs2]
                 * x_clip, y_clip: ROI of the fitting, should be list of upper and lower boundary
+                * parameter_alias: alias of parameters that will be renamed from key to value
 
         """
         if name is None:
             self.name = self.__class__.__name__
         else:
             self.name = name
         self.components = cast(Dict[str, Component], dict())
         self._config = config
         self._data_file_name = config["data_file_name"]
         self._bins_type = config["bins_type"]
         self._bins_on = config["bins_on"]
         self._bins = config["bins"]
+        self._parameter_alias = config.get("parameter_alias", dict())
         if isinstance(self._bins_on, str):
             self._dim = 1
             self._bins_on = [self._bins_on]
             if isinstance(self._bins, int):
                 self._bins = [self._bins]
         elif isinstance(self._bins_on, list):
             self._dim = len(self._bins_on)
@@ -231,19 +256,38 @@
 
         # Update components sheet
         self.components[component_name] = component
 
         # Update needed parameters
         self.needed_parameters |= self.components[component_name].needed_parameters
 
+        # Replace alias in needed parameters
+        for k, v in self._parameter_alias.items():
+            if v in self.needed_parameters:
+                self.needed_parameters.add(k)
+                self.needed_parameters.remove(v)
+
+    def replace_alias(self, parameters):
+        """Replace alias in parameters from key to value.
+
+        Note that the value will be popped out.
+
+        """
+        _parameters = deepcopy(parameters)
+        for k, v in self._parameter_alias.items():
+            if k in _parameters:
+                _parameters[v] = _parameters.pop(k)
+        return _parameters
+
     def _sanity_check(self):
         """Check equality between number of bins group and observables."""
         if len(self._bins_on) != len(self._bins):
             raise RuntimeError("Length of bins must be the same as length of bins_on!")
 
+    @need_replacing_alias
     def _simulate_model_hist(self, key, batch_size, parameters):
         """Histogram of simulated observables.
 
         Args:
             key: a pseudo-random number generator (PRNG) key.
             batch_size: int of number of simulated events.
             parameters: dict of parameters used in simulation.
@@ -256,14 +300,15 @@
             elif isinstance(component, ComponentFixed):
                 _hist = component.simulate_hist(parameters)
             else:
                 raise TypeError(f"unsupported component type for {component_name}!")
             hist += _hist
         return key, hist
 
+    @need_replacing_alias
     def simulate_weighted_data(self, key, batch_size, parameters):
         """Simulate weighted histogram.
 
         Args:
             key: a pseudo-random number generator (PRNG) key.
             batch_size: int of number of simulated events.
             parameters: dict of parameters used in simulation.
@@ -277,14 +322,15 @@
                 _result = component.simulate_weighted_data(parameters)
             else:
                 raise TypeError(f"unsupported component type for {component_name}!")
             result.append(_result)
         result = list(r for r in np.hstack(result))
         return key, result
 
+    @need_replacing_alias
     def get_log_likelihood(self, key, batch_size, parameters):
         """Get log likelihood of given parameters.
 
         Args:
             key: a pseudo-random number generator (PRNG) key.
             batch_size: int of number of simulated events.
             parameters: dict of parameters used in simulation.
@@ -294,14 +340,15 @@
         # Poisson likelihood
         llh = jnp.sum(self.data_hist * jnp.log(model_hist) - model_hist)
         llh = float(llh)
         if np.isnan(llh):
             llh = -np.inf
         return key, llh
 
+    @need_replacing_alias
     def get_num_events_accepted(self, batch_size, parameters):
         """Get number of events in the histogram under given parameters.
 
         Args:
             batch_size: int of number of simulated events.
             parameters: dict of parameters used in simulation.
 
@@ -335,26 +382,26 @@
         for i, component_name in enumerate(self.components):
             name = component_name
             component = self[component_name]
             need = component.needed_parameters
 
             print(f"{indent}COMPONENT {i}: {name}")
             if isinstance(component, ComponentSim):
-                print(f"{indent*2}type: simulation")
-                print(f"{indent*2}rate_par: {component.rate_name}")
-                print(f"{indent*2}pars: {need}")
+                print(f"{indent * 2}type: simulation")
+                print(f"{indent * 2}rate_par: {component.rate_name}")
+                print(f"{indent * 2}pars: {need}")
                 if not short:
-                    print(f"{indent*2}worksheet: {component.worksheet}")
+                    print(f"{indent * 2}worksheet: {component.worksheet}")
             elif isinstance(component, ComponentFixed):
-                print(f"{indent*2}type: fixed")
-                print(f"{indent*2}file_name: {component._file_name}")
-                print(f"{indent*2}rate_par: {component.rate_name}")
-                print(f"{indent*2}pars: {need}")
+                print(f"{indent * 2}type: fixed")
+                print(f"{indent * 2}file_name: {component._file_name}")
+                print(f"{indent * 2}rate_par: {component.rate_name}")
+                print(f"{indent * 2}pars: {need}")
                 if not short:
-                    print(f"{indent*2}from_file: {component._file_name}")
+                    print(f"{indent * 2}from_file: {component._file_name}")
             else:
                 pass
             print()
 
         print("-" * 40)
 
 
@@ -380,14 +427,15 @@
             self.name = name
         self.components = dict()
         self._config = config
         self._bins = None
         self._bins_type = None
         self._bins_on = config["bins_on"]
         self._dim = len(self._bins_on)
+        self._parameter_alias = config.get("parameter_alias", dict())
 
         self.needed_parameters: Set[str] = set()
         self.component_bins_type = None
         logpdf_args = self._config["logpdf_args"]
         self.logpdf_args = {k: np.array(v) for k, v in zip(*logpdf_args)}
 
         self.variable_type = config["variable_type"]
@@ -407,14 +455,15 @@
     def _sanity_check(self):
         """Check sanities of supported distribution and dimension."""
         if self.variable_type not in ["twohalfnorm", "norm", "band"]:
             raise RuntimeError("Currently only twohalfnorm, norm and band are supported")
         if self._dim != 2:
             raise AssertionError(self.warning)
 
+    @need_replacing_alias
     def _simulate_yields(self, key, batch_size, parameters):
         """Histogram of simulated observables.
 
         Args:
             key: a pseudo-random number generator (PRNG) key.
             batch_size: int of number of simulated events.
             parameters: dict of parameters used in simulation.
@@ -430,14 +479,15 @@
     def register_component(self, *args, **kwargs):
         if len(self.components) != 0:
             raise AssertionError(self.warning)
         super().register_component(*args, **kwargs)
         # cache the component name
         self.only_component = list(self.components.keys())[0]
 
+    @need_replacing_alias
     def get_log_likelihood(self, key, batch_size, parameters):
         """Get log likelihood of given parameters.
 
         Args:
             key: a pseudo-random number generator (PRNG) key.
             batch_size: int of number of simulated events.
             parameters: dict of parameters used in simulation.
@@ -471,35 +521,35 @@
         print(f"{indent}variable_type: {self.variable_type}")
         print(f"{indent}variable: {self._bins_on}")
         print("\n" + "-" * 40)
 
         print("LOGPDF\n")
         print(f"{indent}logpdf_args:")
         for k, v in self.logpdf_args.items():
-            print(f"{indent*2}{k}: {v}")
+            print(f"{indent * 2}{k}: {v}")
         print("\n" + "-" * 40)
 
         print("MODEL\n")
         for i, component_name in enumerate(self.components):
             name = component_name
             component = self[component_name]
             need = component.needed_parameters
 
             print(f"{indent}COMPONENT {i}: {name}")
             if isinstance(component, ComponentSim):
-                print(f"{indent*2}type: simulation")
-                print(f"{indent*2}rate_par: {component.rate_name}")
-                print(f"{indent*2}pars: {need}")
+                print(f"{indent * 2}type: simulation")
+                print(f"{indent * 2}rate_par: {component.rate_name}")
+                print(f"{indent * 2}pars: {need}")
                 if not short:
-                    print(f"{indent*2}worksheet: {component.worksheet}")
+                    print(f"{indent * 2}worksheet: {component.worksheet}")
             elif isinstance(component, ComponentFixed):
-                print(f"{indent*2}type: fixed")
-                print(f"{indent*2}file_name: {component._file_name}")
-                print(f"{indent*2}rate_par: {component.rate_name}")
-                print(f"{indent*2}pars: {need}")
+                print(f"{indent * 2}type: fixed")
+                print(f"{indent * 2}file_name: {component._file_name}")
+                print(f"{indent * 2}rate_par: {component.rate_name}")
+                print(f"{indent * 2}pars: {need}")
                 if not short:
-                    print(f"{indent*2}from_file: {component._file_name}")
+                    print(f"{indent * 2}from_file: {component._file_name}")
             else:
                 pass
             print()
 
         print("-" * 40)
```

### Comparing `appletree-0.3.2/appletree/maps/_nr_ly.json` & `appletree-0.4.0/appletree/maps/_nr_ly.json`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/maps/_nr_qy.json` & `appletree-0.4.0/appletree/maps/_nr_qy.json`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/maps/_nr_spectrum.json` & `appletree-0.4.0/appletree/maps/_nr_spectrum.json`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/maps/_posrec_reso.json` & `appletree-0.4.0/appletree/maps/_posrec_reso.json`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/maps/_s1_correction.json` & `appletree-0.4.0/appletree/maps/_s1_correction.json`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/maps/_s1_smearing.json` & `appletree-0.4.0/appletree/maps/_s1_smearing.json`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/maps/_s2_smearing.json` & `appletree-0.4.0/appletree/maps/_s2_smearing.json`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/parameter.py` & `appletree-0.4.0/appletree/parameter.py`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/parameters/er.json` & `appletree-0.4.0/appletree/parameters/er.json`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/parameters/nestv2.json` & `appletree-0.4.0/appletree/parameters/nestv2.json`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/parameters/nr_low.json` & `appletree-0.4.0/appletree/parameters/nr_low.json`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/plot.py` & `appletree-0.4.0/appletree/plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,19 +23,31 @@
             thin: use samples every thin steps.
 
         """
         self.backend_file_name = backend_file_name
         backend = emcee.backends.HDFBackend(self.backend_file_name, read_only=True)
 
         self.chain = backend.get_chain(discard=discard, thin=thin)
-        self.flat_chain = backend.get_chain(discard=discard, thin=thin, flat=True)
         self.posterior = backend.get_log_prob(discard=discard, thin=thin)
-        self.flat_posterior = backend.get_log_prob(discard=discard, thin=thin, flat=True)
         self.prior = backend.get_blobs(discard=discard, thin=thin)
+        # We drop iterations with inf and nan posterior
+        mask = np.isfinite(self.posterior)
+        mask = np.all(mask, axis=1)
+        self.chain = self.chain[mask]
+        self.posterior = self.posterior[mask]
+        self.prior = self.prior[mask]
+
+        self.flat_chain = backend.get_chain(discard=discard, thin=thin, flat=True)
+        self.flat_posterior = backend.get_log_prob(discard=discard, thin=thin, flat=True)
         self.flat_prior = backend.get_blobs(discard=discard, thin=thin, flat=True)
+        # We drop samples with inf and nan posterior
+        mask = np.isfinite(self.flat_posterior)
+        self.flat_chain = self.flat_chain[mask]
+        self.flat_posterior = self.flat_posterior[mask]
+        self.flat_prior = self.flat_prior[mask]
 
         with h5py.File(self.backend_file_name, "r") as f:
             self.param_names = f["mcmc"].attrs["parameter_fit"]
             self.param_prior = json.loads(f["mcmc"].attrs["par_config"])
 
         param_mpe = self.flat_chain[np.argmax(self.flat_posterior), :]
         self.param_mpe = {key: param_mpe[i] for i, key in enumerate(self.param_names)}
@@ -195,15 +207,16 @@
             fig: the figure.
             axes: the axes of the figure.
 
         """
         if fig is None:
             fig = plt.figure(figsize=(2 * (self.n_param + 2), 2 * (self.n_param + 2)))
         samples = np.concatenate(
-            (self.flat_chain, self.flat_posterior[:, None], self.flat_prior[:, None]), axis=1
+            (self.flat_chain, self.flat_posterior[:, None], self.flat_prior[:, None]),
+            axis=1,
         )
         labels = np.concatenate((self.param_names, ["log posterior", "log prior"]))
 
         corner.corner(
             samples,
             labels=labels,
             quantiles=norm.cdf([-1, 0, 1]),
```

### Comparing `appletree-0.3.2/appletree/plugin.py` & `appletree-0.4.0/appletree/plugin.py`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/plugins/common.py` & `appletree-0.4.0/appletree/plugins/common.py`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/plugins/detector.py` & `appletree-0.4.0/appletree/plugins/detector.py`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/plugins/efficiency.py` & `appletree-0.4.0/appletree/plugins/efficiency.py`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/plugins/er_microphys.py` & `appletree-0.4.0/appletree/plugins/er_microphys.py`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/plugins/lyqy.py` & `appletree-0.4.0/appletree/plugins/lyqy.py`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/plugins/nestv2.py` & `appletree-0.4.0/appletree/plugins/nestv2.py`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/plugins/reconstruction.py` & `appletree-0.4.0/appletree/plugins/reconstruction.py`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/randgen.py` & `appletree-0.4.0/appletree/randgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from warnings import warn
 from functools import partial
 from time import time
 
 import jax
 from jax import numpy as jnp
 import numpy as np
 from jax import random, lax, jit, vmap
@@ -17,21 +18,14 @@
 if jax.config.x64_enabled:
     INT = np.int64
     FLOAT = np.float64
 else:
     INT = np.int32
     FLOAT = np.float32
 
-if os.environ.get("DO_NOT_USE_APPROX_IN_BINOM") is None:
-    ALWAYS_USE_NORMAL_APPROX_IN_BINOM = True
-    print("Using Normal as an approximation of Binomial")
-else:
-    ALWAYS_USE_NORMAL_APPROX_IN_BINOM = False
-    print("Using accurate Binomial, not Normal approximation")
-
 
 @export
 def get_key(seed=None):
     """Generate a key for jax.random."""
     if seed is None:
         seed = int(time() * 1e6)
     return random.PRNGKey(seed)
@@ -217,71 +211,110 @@
     shape = shape or jnp.shape(p)
     p = jnp.broadcast_to(p, shape).astype(FLOAT)
 
     rvs = random.bernoulli(seed, p, shape=shape)
     return key, rvs.astype(INT)
 
 
-@export
-@partial(jit, static_argnums=(3, 4))
-def binomial(key, p, n, shape=(), always_use_normal=ALWAYS_USE_NORMAL_APPROX_IN_BINOM):
-    """Binomial random sampler.
+if hasattr(random, "binomial"):
 
-    Args:
-        key: seed for random generator.
-        p: <jnp.array>-like probability in binomial distribution.
-        n: <jnp.array>-like count in binomial distribution.
-        shape: output shape.
-            If not given, output has shape jnp.broadcast_shapes(jnp.shape(p), jnp.shape(n)).
-        always_use_normal: If true, then Norm(np, sqrt(npq)) is always used.
-            Otherwise if n * p < 5, use the inversion method instead.
+    @export
+    @partial(jit, static_argnums=(3,))
+    def binomial(key, p, n, shape=()):
+        """Binomial random sampler.
+
+        Args:
+            key: seed for random generator.
+            p: <jnp.array>-like probability in binomial distribution.
+            n: <jnp.array>-like count in binomial distribution.
+            shape: output shape.
+                If not given, output has shape jnp.broadcast_shapes(jnp.shape(p), jnp.shape(n)).
+            always_use_normal: If true, then Norm(np, sqrt(npq)) is always used.
+                Otherwise if n * p < 5, use the inversion method instead.
+
+        Returns:
+            an updated seed, random variables.
+
+        """
+
+        key, seed = random.split(key)
+
+        shape = shape or jnp.broadcast_shapes(jnp.shape(p), jnp.shape(n))
+        p = jnp.broadcast_to(p, shape).astype(FLOAT)
+        n = jnp.broadcast_to(n, shape).astype(INT)
 
-    Returns:
-        an updated seed, random variables.
+        rvs = random.binomial(seed, n, p, shape=shape)
+        return key, rvs.astype(INT)
 
-    """
-
-    def _binomial_normal_approx_dispatch(seed, p, n):
-        q = 1.0 - p
-        mean = n * p
-        std = jnp.sqrt(n * p * q)
-        rvs = jnp.clip(random.normal(seed) * std + mean, a_min=0.0, a_max=n)
-        return rvs.round().astype(INT)
-
-    def _binomial_dispatch(seed, p, n):
-        use_normal_approx = n * p >= 5.0
-        return lax.cond(
-            use_normal_approx,
-            (seed, p, n),
-            lambda x: _binomial_normal_approx_dispatch(*x),
-            (seed, p, n),
-            lambda x: _binomial_dispatch_numpyro(*x),
-        )
-
-    key, seed = random.split(key)
-
-    shape = shape or lax.broadcast_shapes(jnp.shape(p), jnp.shape(n))
-    p = jnp.reshape(jnp.broadcast_to(p, shape), -1)
-    n = jnp.reshape(jnp.broadcast_to(n, shape), -1)
-    seed = random.split(seed, jnp.size(p))
-
-    if always_use_normal:
-        dispatch = _binomial_normal_approx_dispatch
+else:
+    warn("random.binomial is not available, using numpyro's _binomial_dispatch instead.")
+    if os.environ.get("DO_NOT_USE_APPROX_IN_BINOM") is None:
+        ALWAYS_USE_NORMAL_APPROX_IN_BINOM = True
+        print("Using Normal as an approximation of Binomial")
     else:
-        dispatch = _binomial_dispatch
+        ALWAYS_USE_NORMAL_APPROX_IN_BINOM = False
+        print("Using accurate Binomial, not Normal approximation")
 
-    if jax.default_backend() == "cpu":
-        ret = lax.map(lambda x: dispatch(*x), (seed, p, n))
-    else:
-        ret = vmap(lambda *x: dispatch(*x))(seed, p, n)
-    return key, jnp.reshape(ret, shape)
+    @export
+    @partial(jit, static_argnums=(3, 4))
+    def binomial(key, p, n, shape=(), always_use_normal=ALWAYS_USE_NORMAL_APPROX_IN_BINOM):
+        """Binomial random sampler.
+
+        Args:
+            key: seed for random generator.
+            p: <jnp.array>-like probability in binomial distribution.
+            n: <jnp.array>-like count in binomial distribution.
+            shape: output shape.
+                If not given, output has shape jnp.broadcast_shapes(jnp.shape(p), jnp.shape(n)).
+            always_use_normal: If true, then Norm(np, sqrt(npq)) is always used.
+                Otherwise if n * p < 5, use the inversion method instead.
+
+        Returns:
+            an updated seed, random variables.
+
+        """
+
+        def _binomial_normal_approx_dispatch(seed, p, n):
+            q = 1.0 - p
+            mean = n * p
+            std = jnp.sqrt(n * p * q)
+            rvs = jnp.clip(random.normal(seed) * std + mean, a_min=0.0, a_max=n)
+            return rvs.round().astype(INT)
+
+        def _binomial_dispatch(seed, p, n):
+            use_normal_approx = n * p >= 5.0
+            return lax.cond(
+                use_normal_approx,
+                (seed, p, n),
+                lambda x: _binomial_normal_approx_dispatch(*x),
+                (seed, p, n),
+                lambda x: _binomial_dispatch_numpyro(*x),
+            )
+
+        key, seed = random.split(key)
+
+        shape = shape or lax.broadcast_shapes(jnp.shape(p), jnp.shape(n))
+        p = jnp.reshape(jnp.broadcast_to(p, shape), -1)
+        n = jnp.reshape(jnp.broadcast_to(n, shape), -1)
+        seed = random.split(seed, jnp.size(p))
+
+        if always_use_normal:
+            dispatch = _binomial_normal_approx_dispatch
+        else:
+            dispatch = _binomial_dispatch
+
+        if jax.default_backend() == "cpu":
+            ret = lax.map(lambda x: dispatch(*x), (seed, p, n))
+        else:
+            ret = vmap(lambda *x: dispatch(*x))(seed, p, n)
+        return key, jnp.reshape(ret, shape)
 
 
 @export
-@partial(jit, static_argnums=(3, 4))
+@partial(jit, static_argnums=(3,))
 def negative_binomial(key, p, n, shape=()):
     """Negative binomial distribution random sampler. Using Gamma–Poisson mixture.
 
     Args:
         key: seed for random generator.
         p: <jnp.array>-like probability of a single success in negative binomial distribution.
         n: <jnp.array>-like number of successes in negative binomial distribution.
```

### Comparing `appletree-0.3.2/appletree/share.py` & `appletree-0.4.0/appletree/share.py`

 * *Files identical despite different names*

### Comparing `appletree-0.3.2/appletree/utils.py` & `appletree-0.4.0/appletree/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,17 +145,17 @@
     * fname begin with '/', return absolute path
     * url_base begin with '/', return url_base + name
     * can get file from _get_abspath, return appletree internal file path
     * can be found in local installed ntauxfiles, return ntauxfiles absolute path
     * can be downloaded from MongoDB, download and return cached path
 
     """
-    # 1. From absolute path
+    # 1. From absolute path if file exists
     # Usually Config.default is a absolute path
-    if fname.startswith("/"):
+    if os.path.isfile(fname):
         return fname
 
     # 2. From local folder
     # Use url_base as prefix
     if "url_base" in _cached_configs.keys():
         url_base = _cached_configs["url_base"]
 
@@ -240,18 +240,18 @@
 def set_gpu_memory_usage(fraction=0.3):
     """Set GPU memory usage.
 
     See more on https://jax.readthedocs.io/en/latest/gpu_memory_allocation.html
 
     """
     if fraction > 1:
-        fraction = 1
+        fraction = 0.99
     if fraction <= 0:
         raise ValueError("fraction must be positive!")
-    os.environ["XLA_PYTHON_CLIENT_MEM_FRACTION"] = f"{fraction:.2f}"
+    os.environ["XLA_PYTHON_CLIENT_MEM_FRACTION"] = f".{int(fraction * 100):d}"
 
 
 @export
 def get_equiprob_bins_1d(
     data,
     n_partitions,
     clip=(-np.inf, +np.inf),
@@ -331,15 +331,15 @@
 
     """
     hist = np.asarray(hist)
     bins_x = np.asarray(bins_x)
     bins_y = np.asarray(bins_y)
 
     density = kwargs.get("density", False)
-    cmap = mpl.cm.get_cmap("RdBu_r")
+    cmap = mpl.cm.RdBu_r
 
     loc = []
     width = []
     height = []
     area = []
     n = []
```

### Comparing `appletree-0.3.2/appletree.egg-info/PKG-INFO` & `appletree-0.4.0/appletree.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appletree
-Version: 0.3.2
+Version: 0.4.0
 Summary: A high-Performance Program simuLatEs and fiTs REsponse of xEnon.
 Home-page: https://github.com/XENONnT/appletree
 Author: Appletree contributors, the XENON collaboration
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -83,14 +83,31 @@
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 
+v0.4.0 / 2024-05-27
+-------------------
+* Try using jax.random.binomial by @dachengx in https://github.com/XENONnT/appletree/pull/148
+* Turn off add_eps_to_hist in NR and ER by @FaroutYLq in https://github.com/XENONnT/appletree/pull/152
+* Debug when `bins_type` is not set by @dachengx in https://github.com/XENONnT/appletree/pull/153
+* Specifically install `lxml_html_clean` by @dachengx in https://github.com/XENONnT/appletree/pull/157
+* Initialize context from backend by @zihaoxu98 in https://github.com/XENONnT/appletree/pull/156
+* Add `parameter_alias` to translate parameters in `par_config` by @dachengx in https://github.com/XENONnT/appletree/pull/160
+* Allow user to aggressively use memory by @dachengx in https://github.com/XENONnT/appletree/pull/164
+* Fix a bug of plotter which contains inf by @zihaoxu98 in https://github.com/XENONnT/appletree/pull/165
+
+New Contributors
+* @FaroutYLq made their first contribution in https://github.com/XENONnT/appletree/pull/152
+
+**Full Changelog**: https://github.com/XENONnT/appletree/compare/v0.3.2...v0.4.0
+
+
 v0.3.2 / 2024-03-06
 -------------------
 * Remove `scikit-learn` version requirement by @dachengx in https://github.com/XENONnT/appletree/pull/131
 * Use trusted publisher because username/password authentication is no longer supported by @dachengx in https://github.com/XENONnT/appletree/pull/132
 * Be compatible with `JAX_ENABLE_X64=1` by @dachengx in https://github.com/XENONnT/appletree/pull/134
 * Raise more information when file can not be found by @dachengx in https://github.com/XENONnT/appletree/pull/135
 * Preserve dtype of results in `multiple_simulations` by @dachengx in https://github.com/XENONnT/appletree/pull/137
```

### Comparing `appletree-0.3.2/appletree.egg-info/SOURCES.txt` & `appletree-0.4.0/appletree.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 appletree/maps/_s1_cut_acc.json
 appletree/maps/_s1_smearing.json
 appletree/maps/_s2_bias.json
 appletree/maps/_s2_correction.json
 appletree/maps/_s2_cut_acc.json
 appletree/maps/_s2_smearing.json
 appletree/parameters/er.json
+appletree/parameters/er_rn220_ar37.json
 appletree/parameters/nestv2.json
 appletree/parameters/nr_low.json
 appletree/plugins/__init__.py
 appletree/plugins/common.py
 appletree/plugins/detector.py
 appletree/plugins/efficiency.py
 appletree/plugins/er_microphys.py
```

### Comparing `appletree-0.3.2/setup.py` & `appletree-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     readme = file.read()
 
 with open("HISTORY.md") as file:
     history = file.read()
 
 setuptools.setup(
     name="appletree",
-    version="0.3.2",
+    version="0.4.0",
     description="A high-Performance Program simuLatEs and fiTs REsponse of xEnon.",
     author="Appletree contributors, the XENON collaboration",
     long_description=readme + "\n\n" + history,
     long_description_content_type="text/markdown",
     setup_requires=["pytest-runner"],
     install_requires=requires,
     python_requires=">=3.8",
```

