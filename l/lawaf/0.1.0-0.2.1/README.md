# Comparing `tmp/lawaf-0.1.0.tar.gz` & `tmp/lawaf-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lawaf-0.1.0.tar", last modified: Fri Apr 19 14:18:10 2024, max compression
+gzip compressed data, was "lawaf-0.2.1.tar", last modified: Mon May 27 17:49:00 2024, max compression
```

## Comparing `lawaf-0.1.0.tar` & `lawaf-0.2.1.tar`

### file list

```diff
@@ -1,69 +1,93 @@
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:18:10.933896 lawaf-0.1.0/
--rw-r--r--   0 hexu      (1032) phythema   (500)    18092 2023-05-04 08:11:40.000000 lawaf-0.1.0/LICENSE
--rw-r--r--   0 hexu      (1032) phythema   (500)     1345 2024-04-19 14:18:10.933896 lawaf-0.1.0/PKG-INFO
--rw-r--r--   0 hexu      (1032) phythema   (500)      588 2023-05-04 08:13:58.000000 lawaf-0.1.0/README.md
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:18:10.933896 lawaf-0.1.0/lawaf/
--rw-r--r--   0 hexu      (1032) phythema   (500)      178 2024-04-11 09:27:48.000000 lawaf-0.1.0/lawaf/__init__.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:18:10.933896 lawaf-0.1.0/lawaf/interfaces/
--rw-r--r--   0 hexu      (1032) phythema   (500)      114 2024-04-11 09:26:59.000000 lawaf-0.1.0/lawaf/interfaces/__init__.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:18:10.933896 lawaf-0.1.0/lawaf/interfaces/anaddb/
--rw-r--r--   0 hexu      (1032) phythema   (500)        0 2024-04-08 10:01:09.000000 lawaf-0.1.0/lawaf/interfaces/anaddb/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     9975 2024-04-19 13:43:48.000000 lawaf-0.1.0/lawaf/interfaces/downfolder.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:18:10.933896 lawaf-0.1.0/lawaf/interfaces/phonopy/
--rw-r--r--   0 hexu      (1032) phythema   (500)       81 2024-04-12 07:37:21.000000 lawaf-0.1.0/lawaf/interfaces/phonopy/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1769 2024-04-11 09:22:35.000000 lawaf-0.1.0/lawaf/interfaces/phonopy/ifcwrapper.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3756 2024-04-11 09:13:22.000000 lawaf-0.1.0/lawaf/interfaces/phonopy/phonon_downfolder.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    14864 2024-04-11 08:58:56.000000 lawaf-0.1.0/lawaf/interfaces/phonopy/phonopywrapper.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:18:10.933896 lawaf-0.1.0/lawaf/interfaces/siesta/
--rw-r--r--   0 hexu      (1032) phythema   (500)       47 2024-04-11 09:25:31.000000 lawaf-0.1.0/lawaf/interfaces/siesta/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     5634 2024-04-11 09:25:14.000000 lawaf-0.1.0/lawaf/interfaces/siesta/siesta_downfolder.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:18:10.933896 lawaf-0.1.0/lawaf/interfaces/wannier90/
--rw-r--r--   0 hexu      (1032) phythema   (500)       74 2024-04-11 09:24:53.000000 lawaf-0.1.0/lawaf/interfaces/wannier90/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      399 2024-04-19 13:30:57.000000 lawaf-0.1.0/lawaf/interfaces/wannier90/wannier_downfolder.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:18:10.933896 lawaf-0.1.0/lawaf/mathutils/
--rw-r--r--   0 hexu      (1032) phythema   (500)       23 2023-05-04 08:13:08.000000 lawaf-0.1.0/lawaf/mathutils/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      321 2024-04-11 09:12:23.000000 lawaf-0.1.0/lawaf/mathutils/evals_freq.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      564 2023-05-04 08:13:08.000000 lawaf-0.1.0/lawaf/mathutils/geometry.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      295 2024-04-11 08:58:56.000000 lawaf-0.1.0/lawaf/mathutils/linalg.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     5553 2023-05-04 08:13:08.000000 lawaf-0.1.0/lawaf/mathutils/pert.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:18:10.933896 lawaf-0.1.0/lawaf/plot/
--rw-r--r--   0 hexu      (1032) phythema   (500)       28 2023-05-04 08:13:08.000000 lawaf-0.1.0/lawaf/plot/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    28996 2023-05-04 08:13:08.000000 lawaf-0.1.0/lawaf/plot/cif.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    31851 2023-06-20 09:24:44.000000 lawaf-0.1.0/lawaf/plot/mcif.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2902 2023-05-22 07:17:36.000000 lawaf-0.1.0/lawaf/plot/plot.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      483 2023-05-04 08:13:08.000000 lawaf-0.1.0/lawaf/plot/testpath.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:18:10.933896 lawaf-0.1.0/lawaf/utils/
--rw-r--r--   0 hexu      (1032) phythema   (500)        0 2023-05-04 08:13:08.000000 lawaf-0.1.0/lawaf/utils/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      281 2023-05-08 12:28:16.000000 lawaf-0.1.0/lawaf/utils/gatherphonopy.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1147 2023-05-12 08:19:21.000000 lawaf-0.1.0/lawaf/utils/kpoints.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6884 2024-04-11 08:58:56.000000 lawaf-0.1.0/lawaf/utils/lwf_to_atoms.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6364 2023-05-04 08:13:08.000000 lawaf-0.1.0/lawaf/utils/nckit.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1507 2024-04-11 08:58:56.000000 lawaf-0.1.0/lawaf/utils/plotphon.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1368 2023-05-09 08:02:31.000000 lawaf-0.1.0/lawaf/utils/structurebuilder.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    15087 2023-05-04 08:13:08.000000 lawaf-0.1.0/lawaf/utils/supercell.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     1165 2023-05-04 08:13:08.000000 lawaf-0.1.0/lawaf/utils/symbol.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:18:10.933896 lawaf-0.1.0/lawaf/wannierization/
--rw-r--r--   0 hexu      (1032) phythema   (500)        0 2024-04-11 09:07:33.000000 lawaf-0.1.0/lawaf/wannierization/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8115 2024-04-11 08:58:56.000000 lawaf-0.1.0/lawaf/wannierization/density_scdmk.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    19147 2024-04-11 09:07:54.000000 lawaf-0.1.0/lawaf/wannierization/scdmk.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:18:10.933896 lawaf-0.1.0/lawaf/wrapper/
--rw-r--r--   0 hexu      (1032) phythema   (500)        0 2023-05-04 08:13:08.000000 lawaf-0.1.0/lawaf/wrapper/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      490 2023-05-04 08:13:08.000000 lawaf-0.1.0/lawaf/wrapper/gpawwrapper.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     9507 2024-04-11 08:58:56.000000 lawaf-0.1.0/lawaf/wrapper/ijR.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    18228 2024-04-19 12:57:57.000000 lawaf-0.1.0/lawaf/wrapper/myTB.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     9527 2023-05-09 18:44:59.000000 lawaf-0.1.0/lawaf/wrapper/sislwrapper.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     7075 2023-05-04 08:13:08.000000 lawaf-0.1.0/lawaf/wrapper/utils.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4349 2024-04-19 12:57:57.000000 lawaf-0.1.0/lawaf/wrapper/w90_parser.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:18:10.933896 lawaf-0.1.0/lawaf.egg-info/
--rw-r--r--   0 hexu      (1032) phythema   (500)     1345 2024-04-19 14:18:10.000000 lawaf-0.1.0/lawaf.egg-info/PKG-INFO
--rw-r--r--   0 hexu      (1032) phythema   (500)     1425 2024-04-19 14:18:10.000000 lawaf-0.1.0/lawaf.egg-info/SOURCES.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)        1 2024-04-19 14:18:10.000000 lawaf-0.1.0/lawaf.egg-info/dependency_links.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)      191 2024-04-19 14:18:10.000000 lawaf-0.1.0/lawaf.egg-info/requires.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)        6 2024-04-19 14:18:10.000000 lawaf-0.1.0/lawaf.egg-info/top_level.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)      723 2024-04-19 14:18:08.000000 lawaf-0.1.0/pyproject.toml
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:18:10.933896 lawaf-0.1.0/scripts/
--rwxr-xr-x   0 hexu      (1032) phythema   (500)      138 2023-05-04 08:13:52.000000 lawaf-0.1.0/scripts/phonopy_to_netcdf.py
--rw-r--r--   0 hexu      (1032) phythema   (500)       38 2024-04-19 14:18:10.933896 lawaf-0.1.0/setup.cfg
--rw-r--r--   0 hexu      (1032) phythema   (500)      651 2024-03-18 09:15:13.000000 lawaf-0.1.0/setup.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-19 14:18:10.933896 lawaf-0.1.0/tests/
--rw-r--r--   0 hexu      (1032) phythema   (500)      445 2023-05-08 12:28:16.000000 lawaf-0.1.0/tests/testmcif.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.478916 lawaf-0.2.1/
+-rw-r--r--   0 hexu      (1032) phythema   (500)    18092 2023-05-04 08:11:40.000000 lawaf-0.2.1/LICENSE
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1351 2024-05-27 17:49:00.478916 lawaf-0.2.1/PKG-INFO
+-rw-r--r--   0 hexu      (1032) phythema   (500)      588 2023-05-04 08:13:58.000000 lawaf-0.2.1/README.md
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      223 2024-05-10 07:32:01.000000 lawaf-0.2.1/lawaf/__init__.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/gui/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      297 2024-05-10 07:32:01.000000 lawaf-0.2.1/lawaf/gui/test.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/hamitonian/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2631 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/hamitonian/eigen_modifer.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/interfaces/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      135 2024-05-10 07:32:01.000000 lawaf-0.2.1/lawaf/interfaces/__init__.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/interfaces/anaddb/
+-rw-r--r--   0 hexu      (1032) phythema   (500)        0 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/interfaces/anaddb/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    11549 2024-05-27 17:45:15.000000 lawaf-0.2.1/lawaf/interfaces/downfolder.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/interfaces/magnon/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       70 2024-05-27 17:45:15.000000 lawaf-0.2.1/lawaf/interfaces/magnon/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     5210 2024-05-27 17:45:15.000000 lawaf-0.2.1/lawaf/interfaces/magnon/magnon_downfolder.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/interfaces/phonopy/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      128 2024-05-10 07:32:01.000000 lawaf-0.2.1/lawaf/interfaces/phonopy/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1814 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/interfaces/phonopy/ifcwrapper.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    12254 2024-05-27 08:55:13.000000 lawaf-0.2.1/lawaf/interfaces/phonopy/phonon_downfolder.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    15176 2024-05-27 08:55:13.000000 lawaf-0.2.1/lawaf/interfaces/phonopy/phonopywrapper.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/interfaces/siesta/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       48 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/interfaces/siesta/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     5609 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/interfaces/siesta/siesta_downfolder.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/interfaces/wannier90/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       75 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/interfaces/wannier90/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      397 2024-05-10 07:32:01.000000 lawaf-0.2.1/lawaf/interfaces/wannier90/wannier_downfolder.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/io/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3022 2024-05-10 07:32:01.000000 lawaf-0.2.1/lawaf/io/LWF_json.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4653 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/io/xsf.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/lwf/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      187 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/lwf/dipdip.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     2018 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/lwf/gen_atoms.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    19794 2024-05-27 17:45:15.000000 lawaf-0.2.1/lawaf/lwf/lwf.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     7236 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/lwf/lwf_supercell.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/mathutils/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       23 2023-05-04 08:13:08.000000 lawaf-0.2.1/lawaf/mathutils/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3627 2024-05-27 08:55:13.000000 lawaf-0.2.1/lawaf/mathutils/align_evecs.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      514 2024-05-27 08:55:13.000000 lawaf-0.2.1/lawaf/mathutils/evals_freq.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      566 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/mathutils/geometry.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2822 2024-05-27 08:55:13.000000 lawaf-0.2.1/lawaf/mathutils/kR_convert.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      501 2024-05-10 07:32:01.000000 lawaf-0.2.1/lawaf/mathutils/linalg.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2388 2024-05-27 08:55:13.000000 lawaf-0.2.1/lawaf/mathutils/lowdin.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      969 2024-05-10 07:32:01.000000 lawaf-0.2.1/lawaf/mathutils/occupation_functions.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     5618 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/mathutils/pert.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2274 2024-05-10 07:32:01.000000 lawaf-0.2.1/lawaf/params.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/plot/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       28 2023-05-04 08:13:08.000000 lawaf-0.2.1/lawaf/plot/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    29030 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/plot/cif.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    32337 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/plot/mcif.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2926 2024-05-27 17:45:15.000000 lawaf-0.2.1/lawaf/plot/plot.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      500 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/plot/testpath.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/utils/
+-rw-r--r--   0 hexu      (1032) phythema   (500)        0 2023-05-04 08:13:08.000000 lawaf-0.2.1/lawaf/utils/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      309 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/utils/gatherphonopy.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2796 2024-05-27 17:45:15.000000 lawaf-0.2.1/lawaf/utils/kpoints.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6569 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/utils/lwf_to_atoms.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6310 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/utils/nckit.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1540 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/utils/plotphon.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1505 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/utils/structurebuilder.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    15138 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/utils/supercell.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1197 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/utils/symbol.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/wannierization/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      243 2024-05-10 07:32:01.000000 lawaf-0.2.1/lawaf/wannierization/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     7465 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/wannierization/density_scdmk.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4124 2024-05-10 07:32:01.000000 lawaf-0.2.1/lawaf/wannierization/projectedWF.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     5550 2024-05-10 07:32:01.000000 lawaf-0.2.1/lawaf/wannierization/scdmk.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      449 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/wannierization/semodeWF.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9100 2024-05-27 08:55:13.000000 lawaf-0.2.1/lawaf/wannierization/wannierizer.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/wrapper/
+-rw-r--r--   0 hexu      (1032) phythema   (500)        0 2023-05-04 08:13:08.000000 lawaf-0.2.1/lawaf/wrapper/__init__.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/lawaf/wrapper/deprecated/
+-rw-r--r--   0 hexu      (1032) phythema   (500)    13361 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/wrapper/deprecated/wannier90.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      515 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/wrapper/gpawwrapper.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9334 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/wrapper/ijR.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    17484 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/wrapper/myTB.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9272 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/wrapper/sislwrapper.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6845 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/wrapper/utils.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4242 2024-05-10 07:31:52.000000 lawaf-0.2.1/lawaf/wrapper/w90_parser.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.478916 lawaf-0.2.1/lawaf.egg-info/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1351 2024-05-27 17:49:00.000000 lawaf-0.2.1/lawaf.egg-info/PKG-INFO
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1959 2024-05-27 17:49:00.000000 lawaf-0.2.1/lawaf.egg-info/SOURCES.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)        1 2024-05-27 17:49:00.000000 lawaf-0.2.1/lawaf.egg-info/dependency_links.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)      196 2024-05-27 17:49:00.000000 lawaf-0.2.1/lawaf.egg-info/requires.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)        6 2024-05-27 17:49:00.000000 lawaf-0.2.1/lawaf.egg-info/top_level.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)      735 2024-05-27 17:48:49.000000 lawaf-0.2.1/pyproject.toml
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/scripts/
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)      138 2023-05-04 08:13:52.000000 lawaf-0.2.1/scripts/phonopy_to_netcdf.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)       38 2024-05-27 17:49:00.478916 lawaf-0.2.1/setup.cfg
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-05-27 17:49:00.474916 lawaf-0.2.1/tests/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      445 2023-05-08 12:28:16.000000 lawaf-0.2.1/tests/testmcif.py
```

### Comparing `lawaf-0.1.0/LICENSE` & `lawaf-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lawaf-0.1.0/PKG-INFO` & `lawaf-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: lawaf
-Version: 0.1.0
+Version: 0.2.1
 Summary: A library for constructing Lattice and other Wannier functions 
-Author: Xu He
 Author-email: Xu He <mailhexu@gmail.com>
 License: BSD-2
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: scipy>=1.7.0
 Requires-Dist: sisl>=0.9.0
-Requires-Dist: HamiltonIO>=0.1.0
+Requires-Dist: HamiltonIO>=0.1.2
 Requires-Dist: matplotlib>=3.4.0
 Requires-Dist: ase>=3.19
 Requires-Dist: phonopy>=2.11.0
+Requires-Dist: toml
 Provides-Extra: test
 Requires-Dist: pytest>=6.2.0; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pytest>=6.2.0; extra == "dev"
 Requires-Dist: black>=21.6b0; extra == "dev"
 Requires-Dist: pre-commit>=2.13.0; extra == "dev"
 Requires-Dist: sphinx>=4.1.2; extra == "dev"
```

### Comparing `lawaf-0.1.0/README.md` & `lawaf-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lawaf-0.1.0/lawaf/interfaces/downfolder.py` & `lawaf-0.2.1/lawaf/interfaces/downfolder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,168 +1,70 @@
 from dataclasses import dataclass
 from typing import Tuple, Union, List
 import os
 import copy
 import json
+from ase import Atoms
 from lawaf.utils.kpoints import monkhorst_pack
 import numpy as np
-from lawaf.wannierization.scdmk import (
-    WannierProjectedBuilder,
-    WannierScdmkBuilder,
-    occupation_func,
+from lawaf.wannierization import (
+    ProjectedWannierizer,
+    ScdmkWannierizer,
+    MaxProjectedWannierizer,
 )
+from lawaf.params import WannierParams
 import matplotlib.pyplot as plt
 from lawaf.plot import plot_band
+from lawaf.utils.kpoints import kmesh_to_R, build_Rgrid
+from lawaf.utils.kpoints import autopath
 
 
-@dataclass
-class WFParams:
-    method = "scdmk"
-    kmesh: Tuple[int] = (5, 5, 5)
-    kshift = np.array([1e-7, 3e-6, 5e-9])
-    gamma: bool = True
-    nwann: int = 0
-    weight_func: str = "unity"
-    mu: float = 0.0
-    sigma: float = 2.0
-    selected_basis: Union[None, List[int]] = None
-    anchors: Union[None, List[int]] = None
-    anchor_kpt: Tuple[int] = (0, 0, 0)
-    use_proj: bool = True
-    exclude_bands: Tuple[int] = ()
-
-
-def make_builder(
-    model,
-    kmesh,
-    nwann,
-    has_phase=False,
-    weight_func="unity",
-    mu=0,
-    sigma=0.01,
-    kshift=None,
-    exclude_bands=[],
-    use_proj=False,
-    method="projected",
-    selected_basis=[],
-    anchor_kpt=(0, 0, 0),
-    anchors=None,
-    gamma=True,
-):
-    k = kmesh[0]
-    kpts = monkhorst_pack(kmesh, gamma=gamma) 
-    nk = len(kpts)
-    kweights = [1.0 / nk for k in kpts]
-    if kshift is not None:
-        kpts+=kshift[None, :]
-        anchor_kpt=np.array(anchor_kpt)+kshift
-
-    #if model.has_nac:
-    #    evals, evecs, Hks, Hshorts, Hlongs = model.solve_all(kpts)
-    #else:
-    evals, evecs = model.solve_all(kpts)
-
-    anchor_kpts = []
-    if anchors is not None:
-        for anchor in anchors:
-            anchor_kpts.append(anchor)
-    if anchor_kpt is not None:
-        anchor_kpts.append(anchor_kpt)
-    evals_anchor, evecs_anchor = model.solve_all(anchor_kpts)[0:2]
-    wfn_anchor = {}
-    for ik, k in enumerate(anchor_kpts):
-        wfn_anchor[tuple(k)] = evecs_anchor[ik, :, :]
-
-    try:
-        positions = model.positions
-    except Exception:
-        positions = None
-    if isinstance(weight_func, str):
-        weight_func = occupation_func(ftype=weight_func, mu=mu, sigma=sigma)
-
-    if method == "scdmk":
-        wann_builder = WannierScdmkBuilder(
-            evals=evals,
-            wfn=evecs,
-            positions=positions,
-            kpts=kpts,
-            kweights=kweights,
-            #kshift=kshift,
-            nwann=nwann,
-            weight_func=weight_func,
-            has_phase=has_phase,
-            Rgrid=kmesh,
-            exclude_bands=exclude_bands,
-            use_proj=use_proj,
-            wfn_anchor=wfn_anchor,
-        )
-        if selected_basis:
-            wann_builder.set_selected_cols(selected_basis)
-        elif anchors:
-            wann_builder.set_anchors(anchors)
-        else:
-            wann_builder.auto_set_anchors(anchor_kpt)
-
-    elif method == "projected":
-        wann_builder = WannierProjectedBuilder(
-            evals=evals,
-            wfn=evecs,
-            has_phase=has_phase,
-            positions=positions,
-            kpts=kpts,
-            kweights=kweights,
-            kshift=kshift,
-            nwann=nwann,
-            weight_func=weight_func,
-            Rgrid=kmesh,
-            exclude_bands=exclude_bands,
-            wfn_anchor=wfn_anchor,
-        )
-        if selected_basis:
-            wann_builder.set_projectors_with_basis(selected_basis)
-        elif anchors:
-            wann_builder.set_projectors_with_anchors(anchors)
+def select_wannierizer(method):
+    # select the Wannierizer based on the method.
+    if method.lower().startswith("scdmk"):
+        w = ScdmkWannierizer
+    elif method.lower().startswith("projected"):
+        w = ProjectedWannierizer
+    elif method.lower().startswith("maxprojected"):
+        w = MaxProjectedWannierizer
     else:
-        raise ValueError("method should be scdmk or projected")
-
-    #if model.has_nac:
-    #    wann_builder.set_nac_Hks(Hks, Hshorts, Hlongs)
-    return wann_builder
+        raise ValueError("Unknown method")
+    print(f"Using {w.__name__} method")
+    return w
 
 
 class Lawaf:
     params = {}
-    builder: Union[WannierProjectedBuilder, WannierScdmkBuilder] = None
-    model  = None
+    builder: Union[ProjectedWannierizer, ScdmkWannierizer] = None
+    model = None
 
-    def __init__(self, model):
+    def __init__(self, model, params=None):
         """
         Setup the model
         """
         self.model = model
         self.params = {}
-        self.builder: Union[WannierProjectedBuilder, WannierScdmkBuilder] = None
+        self.builder = None
+        self.Rgrid = None
 
     def set_parameters(
         self,
         method="scdmk",
         kmesh=(5, 5, 5),
         gamma=True,
         nwann=0,
         weight_func="unity",
-        mu=0.0,
-        sigma=2.0,
+        weight_func_params={0, 0.01},
         selected_basis=None,
         anchors=None,
         anchor_kpt=(0, 0, 0),
         kshift=np.array([1e-7, 2e-8, 3e-9]),
         use_proj=True,
         exclude_bands=[],
         post_func=None,
-        has_nac=False,
     ):
         """
         Downfold the Band structure.
         The method first get the eigenvalues and eigenvectors in a Monkhorst-Pack grid from the model.
         It then use the scdm-k or the projected wannier function method to downfold the Hamiltonian at each k-point.
         And finally it Fourier transform the new basis functions(Wannier functions) from k-space to real space.
         The Hamiltonian can be written.
@@ -184,69 +86,182 @@
         anchors: Anchor points. The index of band at one k-point. e.g.(0, 0, 0): (6, 7, 8)
         anchor_kpt: the kpoint used for automatically selecting of anchor points.
         use_proj: Whether to use projection to the anchor points in the weight function.
         write_hr_nc: write the Hamiltonian into a netcdf file. It require the NETCDF4 python library. use write_nc=None if not needed.
         write_hr_txt: write the Hamiltonian into a txt file.
         """
 
-        self.params = copy.deepcopy(locals())
-        self.params.pop("self")
+        self.params = WannierParams(
+            method=method,
+            kmesh=kmesh,
+            gamma=gamma,
+            nwann=nwann,
+            weight_func=weight_func,
+            weight_func_params=weight_func_params,
+            selected_basis=selected_basis,
+            anchors=anchors,
+            anchor_kpt=anchor_kpt,
+            kshift=kshift,
+            use_proj=use_proj,
+            exclude_bands=exclude_bands,
+        )
+        self.nwann = self.params.nwann
+
+        self._prepare_data()
+
+    def _prepare_data(self):
+        """
+        Prepare the data for the downfolding. e.g. eigen values, eigen vectors, kpoints
+        """
+        self._prepare_kpoints()
+        self._prepare_eigen()
+        self._prepare_Rlist()
+        self._prepare_positions()
+        self._parepare_builder()
+
+    def _parepare_builder(self):
+        params = self.params
+        wannierizer = select_wannierizer(params.method)
+        self.builder = wannierizer(
+            evals=self.evals,
+            evecs=self.evecs,
+            kpts=self.kpts,
+            kweights=self.kweights,
+            params=self.params,
+        )
+
+    def _prepare_positions(self):
+        try:
+            self.atoms = self.model.atoms
+        except:
+            self.atoms = Atoms(cell=np.eye(3))
+        try:
+            positions = self.model.positions
+        except Exception:
+            positions = None
+        self.positions = positions
+
+    def _prepare_kpoints(self):
+        """
+        Prepare the kpoints
+        """
+        if self.params.kpts is not None:
+            self.kpts = np.array(self.params.kpts)
+        else:
+            self.kpts = monkhorst_pack(self.params.kmesh, gamma=self.params.gamma)
+
+        self.nkpt = len(self.kpts)
+        if self.params.kshift is not None:
+            kshift = np.array(self.params.kshift)
+            self.kpts += kshift[None, :]
+            self.params.anchor_kpt = np.array(self.params.anchor_kpt) + kshift
+        if not self.params.kweights:
+            self.kweights = np.ones(self.nkpt, dtype=float) / self.nkpt
+        else:
+            self.kweights = self.params.kweights
+
+        self.anchor_kpt = np.array(self.params.anchor_kpt)
+
+        abs_kdistance_to_anchor = np.abs(
+            np.linalg.norm(self.kpts - self.anchor_kpt[None, :], axis=1)
+        )
+        if not np.any(abs_kdistance_to_anchor < 1e-5):
+            self.nkpt += 1
+            self.kpts = np.vstack([self.kpts, self.anchor_kpt])
+            self.kweights = np.hstack([self.kweights, 0.0])
+            self.anchor_kpt = self.kpts[-1]
+        else:
+            self.anchor_kpt = self.kpts[0]
+
+    def _prepare_Rlist(self):
+        self.Rgrid = self.params.kmesh
+        if self.Rgrid is None:
+            self.Rlist = kmesh_to_R(self.params.kmesh)
+        else:
+            self.Rlist = build_Rgrid(self.Rgrid)
+
+    def _prepare_eigen(self, has_phase=False):
+        evals, evecs = self.model.solve_all(self.kpts)
+        # remove e^ikr from wfn
+        self.has_phase = has_phase
+        if not has_phase:
+            self.psi = evecs
+        else:
+            self._remove_phase(evecs)
+        self.evals = evals
+        self.evecs = evecs
+        return self.evals, self.evecs
+
+    def _remove_phase_k(self, wfnk, k, positions):
+        # phase = np.exp(-2j * np.pi * np.einsum('j, kj->k', k, self.positions))
+        # return wfnk[:, :] * phase[:, None]
+        nbasis = wfnk.shape[0]
+        psi = np.zeros_like(wfnk)
+        for ibasis in range(self.nbasis):
+            phase = np.exp(-2j * np.pi * np.dot(k, positions[ibasis, :]))
+            psi[ibasis, :] = wfnk[ibasis, :] * phase
+        return psi
+
+    def _remove_phase(self, wfn):
+        self.psi = np.zeros_like(wfn)
+        for ik, k in enumerate(self.kpts):
+            self.psi[ik, :, :] = self._remove_phase_k(wfn[ik, :, :], k)
 
     def save_info(self, output_path="./", fname="Downfold.json"):
         results = {"params": self.params}
         with open(os.path.join(output_path, fname), "w") as myfile:
             json.dump(results, myfile, sort_keys=True, indent=2)
 
     def downfold(
         self,
         post_func=None,
         output_path="./",
-        write_hr_nc="LWF.nc",
-        write_hr_txt="LWF.txt",
+        write_hr_nc=None,
+        write_hr_txt=None,
         **params,
     ):
         self.params.update(params)
-        if "post_func" in self.params:
-            self.params.pop("post_func")
-        self.builder = make_builder(self.model, **self.params)
         self.atoms = self.model.atoms
-        self.ewf = self.builder.get_wannier()
-        if post_func is not None:
-            post_func(self.ewf)
+        self.ewf = self.builder.get_wannier(Rlist=self.Rlist)
+
         if not os.path.exists(output_path):
             os.makedirs(output_path)
         try:
             self.save_info(output_path=output_path)
-        except:
+        except Exception as E:
+            print(E)
             pass
-        if write_hr_txt is not None:
-            self.ewf.save_txt(os.path.join(output_path, write_hr_txt))
-        if write_hr_nc is not None:
-            # self.ewf.write_lwf_nc(os.path.join(output_path, write_hr_nc), atoms=self.atoms)
-            self.ewf.write_nc(os.path.join(output_path, write_hr_nc), atoms=self.atoms)
+        # if write_hr_txt is not None:
+        #    self.ewf.save_txt(os.path.join(output_path, write_hr_txt))
+        # if write_hr_nc is not None:
+        #    # self.ewf.write_lwf_nc(os.path.join(output_path, write_hr_nc), atoms=self.atoms)
+        #    self.ewf.write_nc(os.path.join(output_path, write_hr_nc), atoms=self.atoms)
         return self.ewf
 
     def plot_band_fitting(
         self,
-        kvectors=np.array(
-            [[0, 0, 0], [0.5, 0, 0], [0.5, 0.5, 0], [0, 0, 0], [0.5, 0.5, 0.5]]
-        ),
-        knames=["$\Gamma$", "X", "M", "$\Gamma$", "R"],
+        # kvectors=np.array(
+        #    [[0, 0, 0], [0.5, 0, 0], [0.5, 0.5, 0], [0, 0, 0], [0.5, 0.5, 0.5]]
+        # ),
+        # knames=["$\Gamma$", "X", "M", "$\Gamma$", "R"],
+        kvectors=None,
+        knames=None,
         supercell_matrix=None,
         npoints=100,
         efermi=None,
         erange=None,
         fullband_color="blue",
         downfolded_band_color="green",
         marker="o",
         ax=None,
         savefig="Downfolded_band.png",
         cell=np.eye(3),
         plot_original=True,
         plot_downfolded=True,
+        plot_nonac=False,
         show=True,
         fix_LOTO=False,
         **kwargs,
     ):
         """
         Parameters:
         ========================================
@@ -293,14 +308,30 @@
                 marker=marker,
                 erange=erange,
                 cell=cell,
                 ax=ax,
                 fix_LOTO=fix_LOTO,
                 **kwargs,
             )
+        if plot_nonac:
+            self.ewf.set_nac(False)
+            ax = plot_band(
+                self.ewf,
+                kvectors=kvectors,
+                knames=knames,
+                supercell_matrix=supercell_matrix,
+                npoints=npoints,
+                efermi=efermi,
+                color="red",
+                alpha=0.5,
+                marker=marker,
+                erange=erange,
+                cell=cell,
+                ax=ax,
+                fix_LOTO=fix_LOTO,
+                **kwargs,
+            )
         if savefig is not None:
             plt.savefig(savefig)
         if show:
             plt.show()
         return ax
-
-
```

### Comparing `lawaf-0.1.0/lawaf/interfaces/phonopy/ifcwrapper.py` & `lawaf-0.2.1/lawaf/interfaces/phonopy/ifcwrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 simple IFC wrapper
 """
 
 from scipy.linalg import eigh
 import numpy as np
 from lawaf.plot import plot_band
 import matplotlib.pyplot as plt
-#from lawaf.utils import read_ifc_from_netcdf, save_ifc_to_netcdf
 
+# from lawaf.utils import read_ifc_from_netcdf, save_ifc_to_netcdf
 
-class IFC():
+
+class IFC:
     def __init__(self, atoms, Rlist, ifc):
         self.atoms = atoms
         self.Rlist = Rlist
         self.ifc = ifc
         self.natoms = len(atoms)
         self.natoms3 = 3 * self.natoms
 
@@ -22,16 +23,21 @@
         """
         read netcdf
         """
         atoms, Rlist, ifc = read_ifc_from_netcdf(fname)
         return IFC(atoms, Rlist, ifc)
 
     def save_to_netcdf(self, fname):
-        save_ifc_to_netcdf(fname=fname, ifc=self.ifc, Rlist=self.Rlist,
-                           atoms=self.atoms, ref_energy=0.0)
+        save_ifc_to_netcdf(
+            fname=fname,
+            ifc=self.ifc,
+            Rlist=self.Rlist,
+            atoms=self.atoms,
+            ref_energy=0.0,
+        )
 
     def eval_modifier(self, kmesh, func):
         pass
 
     def solve_all(self, kpts):
         """
         calculate the eigen values and vectors
@@ -49,16 +55,16 @@
         return evals, evecs
 
     def plot_band(self, **kwargs):
         plot_band(self, **kwargs)
 
 
 def test():
-    #fname = './R_VO2_ifc_scaled.nc'
+    # fname = './R_VO2_ifc_scaled.nc'
     fname = "/home/hexu/projects/VO2_new/perhaps_good_potential/latt_lwf/R_VO2_ifc_scaled.nc"
     ifc = IFC.load_from_netcdf(fname)
     ifc.plot_band()
     plt.show()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     test()
```

### Comparing `lawaf-0.1.0/lawaf/interfaces/phonopy/phonopywrapper.py` & `lawaf-0.2.1/lawaf/interfaces/phonopy/phonopywrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # from minimulti.ioput.ifc_netcdf import save_ifc_to_netcdf
 from lawaf.plot import plot_band
 from .ifcwrapper import IFC
 import matplotlib.pyplot as plt
 
 # from supercellmap import SupercellMaker
 from lawaf.utils.supercell import SupercellMaker
+from lawaf.mathutils.align_evecs import align_all_degenerate_eigenvectors
 
 
 class MyDynamicalMatrixGL(DynamicalMatrixGL):
     def __init__(
         self,
         supercell: PhonopyAtoms,
         primitive: Primitive,
@@ -35,24 +36,23 @@
         with_full_terms=False,
         decimals=None,
         symprec=0.00001,
         log_level=0,
         use_openmp=False,
     ):
         super().__init__(
-            supercell,
-            primitive,
-            force_constants,
-            nac_params,
-            num_G_points,
-            with_full_terms,
-            decimals,
-            symprec,
-            log_level,
-            use_openmp,
+            supercell=supercell,
+            primitive=primitive,
+            force_constants=force_constants,
+            nac_params=nac_params,
+            num_G_points=num_G_points,
+            with_full_terms=with_full_terms,
+            decimals=decimals,
+            log_level=log_level,
+            use_openmp=use_openmp,
         )
         self._short_range_dynamical_matrix = None
         self._long_range_dynamical_matrix = None
 
     def get_dynamical_matrix(self, q, lang="C", split_short_long=False):
         """
         Return dynamical matrix at q.
@@ -160,23 +160,25 @@
 
     def __init__(
         self, phonon=None, phonon_fname="phonopy_params.yaml", mode="ifc", has_nac=False
     ):
         if phonon is not None:
             self.phonon = phonon
         else:
-            self.phonon = load(phonon_fname)
+            self.phonon = load(phonon_fname, is_nac=has_nac)
+            print(f"Phonon loaded from file {phonon_fname} ")
         if has_nac:
             self.has_nac = True
             self.get_nac_params()
+            print("replace_phonon_dynamics_with_myGL")
             replace_phonon_dynamics_with_myGL(self.phonon)
         else:
             self.has_nac = False
 
-        #if self.has_nac:
+        # if self.has_nac:
         #    print(
         #        f"Phonopy DM replaces with myGL. Has NAC: {self.has_nac} \n"
         #        + f" born charges: {self.born}, dielectric constant: {self.dielectric}"
         #    )
 
         self._prepare()
         prim = self.phonon.get_primitive()
@@ -207,36 +209,37 @@
     def solve(self, k):
         # Hk = self.phonon.get_dynamical_matrix_at_q(k)
         if self.phonon._dynamical_matrix is None:
             msg = "Dynamical matrix has not yet built."
             raise RuntimeError(msg)
 
         if self.has_nac:
-                    # replace_phonon_dynamics_with_myGL(self.phonon)
+            # replace_phonon_dynamics_with_myGL(self.phonon)
             # self.phonon._dynamical_matrix.run(k)
             # return self.phonon._dynamical_matrix.get_dynamical_matrix()
             # self.phonon.dynamical_matrix._compute_dynamical_matrix(k, [0, 0, 0])
             # Hk, Hshort, Hlong = self.phonon.dynamical_matrix.get_dynamical_matrix(split_short_long=True)
             Hk = self.phonon.get_dynamical_matrix_at_q(k)
             # Hk=self.phonon.dynamical_matrix.dynamical_matrix
-            Hshort = self.phonon.dynamical_matrix.short_range_dynamical_matrix
-            Hlong = self.phonon.dynamical_matrix.long_range_dynamical_matrix
+            Hshort = self.phonon.dynamical_matrix._short_range_dynamical_matrix
+            Hlong = self.phonon.dynamical_matrix._long_range_dynamical_matrix
         else:
             Hk = self.phonon.get_dynamical_matrix_at_q(k)
         phase = np.exp(-2.0j * np.pi * np.einsum("ijk, k->ij", self.dr, k))
         Hk *= phase
         if self.has_nac:
             Hshort *= phase
             Hlong *= phase
         if self.mode == "ifc":
             Hk *= self.Mmat
             if self.has_nac:
                 Hshort *= self.Mmat
                 Hlong *= self.Mmat
         evals, evecs = eigh(Hk)
+        evecs = align_all_degenerate_eigenvectors(evals, evecs)
         if self.has_nac:
             return evals, evecs, Hk, Hshort, Hlong
         else:
             return evals, evecs
 
     def assure_ASR(self, HR, Rlist):
         igamma = np.argmin(np.linalg.norm(Rlist, axis=1))
@@ -284,17 +287,15 @@
         if not self.has_nac:
             for ik, k in enumerate(kpts):
                 evalue, evec = self.solve(k)
                 evals.append(evalue)
                 evecs.append(evec)
         else:
             for ik, k in enumerate(kpts):
-                evalue, evec, Hk, Hshort, Hlong = self.solve(
-                    k 
-                )
+                evalue, evec, Hk, Hshort, Hlong = self.solve(k)
                 evals.append(evalue)
                 evecs.append(evec)
                 Hks.append(Hk)
                 Hshorts.append(Hshort)
                 Hlongs.append(Hlong)
         if self.has_nac:
             return (
```

### Comparing `lawaf-0.1.0/lawaf/interfaces/siesta/siesta_downfolder.py` & `lawaf-0.2.1/lawaf/interfaces/siesta/siesta_downfolder.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import sisl
 from lawaf.interfaces.downfolder import Lawaf
 from lawaf.wrapper.sislwrapper import SislHSWrapper, SislWFSXWrapper
 
 __all__ = ["SiestaDownfolder"]
 
+
 class SislDownfolder(Lawaf):
     def __init__(
         self,
         folder=None,
         fdf_file=None,
         mode="HS",
         ispin=None,
@@ -55,21 +56,21 @@
             H = fdf.read_hamiltonian()
             try:
                 self.efermi = fdf.read_fermi_level().data[0]
             except:
                 self.efermi = fdf.read_fermi_level()
             if recover_fermi:
                 self.shift_fermi = self.efermi
-                self.model = SislHSWrapper(
-                    H,
-                    shift_fermi=self.shift_fermi,
-                    ispin=ispin,
-                    format=format,
-                    nbands=nbands,
-                )
+            self.model = SislHSWrapper(
+                H,
+                shift_fermi=self.shift_fermi,
+                ispin=ispin,
+                format=format,
+                nbands=nbands,
+            )
         elif mode == "WFSX":
             wfsx_sile = sisl.get_sile(os.path.join(folder, wfsx_file))
             fdf = sisl.get_sile(os.path.join(folder, fdf_file))
             geom = fdf.read_geometry()
             spin = sisl.Spin(fdf.get("Spin"))
             try:
                 self.efermi = fdf.read_fermi_level().data[0]
@@ -148,8 +149,9 @@
         #    coeffs = coeffs.sel(k=k)
 
         # Project the orbitals with the coefficients on the grid
         wavefunction(coeffs, grid, geometry=geom)
 
         return grid
 
-SiestaDownfolder = SislDownfolder
+
+SiestaDownfolder = SislDownfolder
```

### Comparing `lawaf-0.1.0/lawaf/mathutils/geometry.py` & `lawaf-0.2.1/lawaf/mathutils/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 from math import sin, cos
 
 
-#@numba.njit('float64[:](float64[:],float64[:])', fastmath=True)
+# @numba.njit('float64[:](float64[:],float64[:])', fastmath=True)
 def cross(a, b):
     ret = np.empty(shape=3, dtype=numba.float64)
     ret[0] = a[1] * b[2] - a[2] * b[1]
     ret[1] = a[2] * b[0] - a[0] * b[2]
     ret[2] = a[0] * b[1] - a[1] * b[0]
     return ret
 
 
-#@numba.njit('float64[:](float64, float64[:], float64[:])', fastmath=True)
+# @numba.njit('float64[:](float64, float64[:], float64[:])', fastmath=True)
 def rotate_vec(angle, axis, vec):
     half_angle = 0.5 * angle
     r = axis * sin(half_angle)
     w = cos(half_angle)
     return vec + 2.0 * cross(r, (cross(r, vec) + w * vec))
```

### Comparing `lawaf-0.1.0/lawaf/mathutils/pert.py` & `lawaf-0.2.1/lawaf/mathutils/pert.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This module is the perturbation to matrix.
 """
 import numpy as np
 from scipy.linalg import eigh
 
 
-class Pert():
+class Pert:
     def __init__(self, H0=None, evals=None, evecs=None):
         if evals is not None and evecs is not None:
             self.evals, self.evecs = evals, evecs
         elif H0 is not None:
             self.evals, self.evecs = eigh(self.H0)
         else:
             raise ValueError("at least H0| evals, evecs should be given")
@@ -28,70 +28,73 @@
 
     @staticmethod
     def Epert1(evecs, dH):
         return np.diag(evecs.T.conj().dot(dH).dot(evecs))
 
     @staticmethod
     def Vpert1(evals, evecs, dH, n):
-        dV = np.zeros((n, n), dtype='complex')
+        dV = np.zeros((n, n), dtype="complex")
         dHH = evecs.T.conj() @ dH @ evecs
         for i in range(n):
             for k in range(n):
                 if abs(evals[k] - evals[i]) > 0.000001:
                     dV[:, i] += dHH[k, i] / (evals[i] - evals[k]) * evecs[:, k]
         return dV
 
     @staticmethod
     def Epert2(evals, evecs, dH, n):
-        d2E = np.zeros(n, dtype='complex')
+        d2E = np.zeros(n, dtype="complex")
         dHH = evecs.T.conj() @ dH @ evecs
         for i in range(n):
             for k in range(n):
                 if abs(evals[k] - evals[i]) > 1e-10:
                     d2E[i] += dHH[i, k] * dHH[k, i] / (evals[i] - evals[k])
         return d2E
 
+
 def unit2(x=0.3):
-    return np.array([[np.cos(x), np.sin(x)],[-np.sin(x), np.cos(x)]])
+    return np.array([[np.cos(x), np.sin(x)], [-np.sin(x), np.cos(x)]])
+
 
 def test_pert_degenerate_2d(x=0.01):
-    H0=np.array([[2,0],[0,2]])
-    evals0, evecs0=np.linalg.eigh(H0)
+    H0 = np.array([[2, 0], [0, 2]])
+    evals0, evecs0 = np.linalg.eigh(H0)
 
-    H1=np.array([[1,2],[3,4]])
-    H1+=H1.T
+    H1 = np.array([[1, 2], [3, 4]])
+    H1 += H1.T
     print(evals0)
 
-    H=H0+H1*x
-    evals, evecs=eigh(H)
-    print("Fdiff of eval: ",(evals-evals0)/x)
-    print("Fdiff of evec: ", (evecs-evecs0))
+    H = H0 + H1 * x
+    evals, evecs = eigh(H)
+    print("Fdiff of eval: ", (evals - evals0) / x)
+    print("Fdiff of evec: ", (evecs - evecs0))
 
-    m=evecs0.T.conj().dot(H1).dot(evecs0)
-    E1, c=eigh(m)
+    m = evecs0.T.conj().dot(H1).dot(evecs0)
+    E1, c = eigh(m)
     print("Pert of eval: ", E1)
-    c=c-np.eye(2)
-    V10=np.dot( c[:,0], evecs0,)
-    V11=np.dot(evecs0, c[:,1])
+    c = c - np.eye(2)
+    V10 = np.dot(
+        c[:, 0],
+        evecs0,
+    )
+    V11 = np.dot(evecs0, c[:, 1])
     print(V10)
     print(V11)
 
 
+# test_pert_degenerate_2d()
 
 
-
-#test_pert_degenerate_2d()
-
 def test_pert(x, n=4):
     H0 = np.random.random([n, n])
     H0 = H0 + H0.T
     evals0, evecs0 = eigh(H0)
 
     dH = np.random.random([n, n])
-    dH = (dH + dH.T.conj())
+    dH = dH + dH.T.conj()
 
     H = H0 + dH * x
     evals, evecs = eigh(H)
 
     # eigen value perturbation (1st order)
     dE = Pert.Epert1(evecs0, dH)
     dE2 = Pert.Epert2(evals0, evecs0, dH, n)
@@ -103,15 +106,15 @@
     print(np.linalg.norm(evals0 - evals))
     print(np.linalg.norm(evals0 + x * dE - evals))
     print(np.linalg.norm(evals0 + x * dE + x * x * dE2 - evals))
 
     # eigen value perturbation (2nd order)
 
     # eigen vector perturbation
-    dV = (Pert.Vpert1(evals0, evecs0, dH, n))
+    dV = Pert.Vpert1(evals0, evecs0, dH, n)
     print("dV:", dV)
     print("dV_fD:", (evecs - evecs0) / x)
 
 
 def gen_degerate_mat(n):
     H0 = np.random.random([n, n])
     H0 = H0 + H0.T
@@ -125,15 +128,15 @@
 
 def test_pert_degenerate(x, n=2):
     H0 = gen_degerate_mat(n=n)
     evals0, evecs0 = eigh(H0)
 
     dH = np.random.random([n, n])
     dH = (dH + dH.T.conj()) * 1
-    #dH = gen_degerate_mat(n=n)
+    # dH = gen_degerate_mat(n=n)
 
     H = H0 + dH * x
     evals, evecs = eigh(H)
 
     # eigen value perturbation (1st order)
     dE = Pert.Epert1(evecs0, dH)
     dE2 = Pert.Epert2(evals0, evecs0, dH, n)
@@ -147,15 +150,15 @@
     print("diff sumtot e0:", np.linalg.norm(evals0 - evals))
     print("diff sumtot e1:", np.linalg.norm(evals0 + x * dE - evals))
     print("diff sumtot e2:", np.linalg.norm(evals0 + x * dE - x * x * dE2 - evals))
 
     # eigen value perturbation (2nd order)
 
     # eigen vector perturbation
-    dV = (Pert.Vpert1(evals0, evecs0, dH, n))
+    dV = Pert.Vpert1(evals0, evecs0, dH, n)
     print("dV:", dV)
     print("dV_fD:", (evecs - evecs0) / x)
 
 
 def test_pert_2only(x, n=2):
     k = 2 * np.pi * 0.400050
     H0 = np.array([[0, 1 + np.exp(1j * k)], [1 + np.exp(-1j * k), 0]])
@@ -184,21 +187,22 @@
     print("diff: E0+E1+E2-E:")
     print(np.linalg.norm(evals0 + x * dE + x * x * dE2 - evals))
 
     # eigen value perturbation (2nd order)
 
     # eigen vector perturbation
     print(evecs0)
-    dV = (Pert.Vpert1(evals0, evecs0, dH, n))
+    dV = Pert.Vpert1(evals0, evecs0, dH, n)
     print("dV:", dV)
     V = evecs0 + dV * x
     print(H)
     print("H:", V @ np.diag(evals) @ V.T.conj())
     print("dV_fD:", (evecs - evecs0) / x)
 
-if __name__=="__main__":
+
+if __name__ == "__main__":
     pass
-    #test_pert(x=0.1, n=4)
-    #print("========= Degenerate test=========")
-    #test_pert_degenerate(x=0.11, n=4)
-    #print("========= Degenerate test=========")
-    #test_pert_2only(x=0.04)
+    # test_pert(x=0.1, n=4)
+    # print("========= Degenerate test=========")
+    # test_pert_degenerate(x=0.11, n=4)
+    # print("========= Degenerate test=========")
+    # test_pert_2only(x=0.04)
```

### Comparing `lawaf-0.1.0/lawaf/plot/cif.py` & `lawaf-0.2.1/lawaf/plot/cif.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,135 +22,139 @@
 from ase.io.cif_unicode import format_unicode, handle_subscripts
 from ase.utils import iofunction
 
 
 rhombohedral_spacegroups = {146, 148, 155, 160, 161, 166, 167}
 
 
-old_spacegroup_names = {'Abm2': 'Aem2',
-                        'Aba2': 'Aea2',
-                        'Cmca': 'Cmce',
-                        'Cmma': 'Cmme',
-                        'Ccca': 'Ccc1'}
+old_spacegroup_names = {
+    "Abm2": "Aem2",
+    "Aba2": "Aea2",
+    "Cmca": "Cmce",
+    "Cmma": "Cmme",
+    "Ccca": "Ccc1",
+}
 
 # CIF maps names to either single values or to multiple values via loops.
 CIFDataValue = Union[str, int, float]
 CIFData = Union[CIFDataValue, List[CIFDataValue]]
 
 
 def convert_value(value: str) -> CIFDataValue:
     """Convert CIF value string to corresponding python type."""
     value = value.strip()
-    if re.match('(".*")|(\'.*\')$', value):
+    if re.match("(\".*\")|('.*')$", value):
         return handle_subscripts(value[1:-1])
-    elif re.match(r'[+-]?\d+$', value):
+    elif re.match(r"[+-]?\d+$", value):
         return int(value)
-    elif re.match(r'[+-]?(?:\d+(?:\.\d*)?|\.\d+)(?:[eE][+-]?\d+)?$', value):
+    elif re.match(r"[+-]?(?:\d+(?:\.\d*)?|\.\d+)(?:[eE][+-]?\d+)?$", value):
         return float(value)
-    elif re.match(r'[+-]?(?:\d+(?:\.\d*)?|\.\d+)(?:[eE][+-]?\d+)?\(\d+\)$',
-                  value):
-        return float(value[:value.index('(')])  # strip off uncertainties
-    elif re.match(r'[+-]?(?:\d+(?:\.\d*)?|\.\d+)(?:[eE][+-]?\d+)?\(\d+$',
-                  value):
+    elif re.match(r"[+-]?(?:\d+(?:\.\d*)?|\.\d+)(?:[eE][+-]?\d+)?\(\d+\)$", value):
+        return float(value[: value.index("(")])  # strip off uncertainties
+    elif re.match(r"[+-]?(?:\d+(?:\.\d*)?|\.\d+)(?:[eE][+-]?\d+)?\(\d+$", value):
         warnings.warn('Badly formed number: "{0}"'.format(value))
-        return float(value[:value.index('(')])  # strip off uncertainties
+        return float(value[: value.index("(")])  # strip off uncertainties
     else:
         return handle_subscripts(value)
 
 
 def parse_multiline_string(lines: List[str], line: str) -> str:
     """Parse semicolon-enclosed multiline string and return it."""
-    assert line[0] == ';'
+    assert line[0] == ";"
     strings = [line[1:].lstrip()]
     while True:
         line = lines.pop().strip()
-        if line[:1] == ';':
+        if line[:1] == ";":
             break
         strings.append(line)
-    return '\n'.join(strings).strip()
+    return "\n".join(strings).strip()
 
 
 def parse_singletag(lines: List[str], line: str) -> Tuple[str, CIFDataValue]:
     """Parse a CIF tag (entries starting with underscore). Returns
     a key-value pair."""
     kv = line.split(None, 1)
     if len(kv) == 1:
         key = line
         line = lines.pop().strip()
-        while not line or line[0] == '#':
+        while not line or line[0] == "#":
             line = lines.pop().strip()
-        if line[0] == ';':
+        if line[0] == ";":
             value = parse_multiline_string(lines, line)
         else:
             value = line
     else:
         key, value = kv
     return key, convert_value(value)
 
 
 def parse_cif_loop_headers(lines: List[str]) -> Iterator[str]:
-    header_pattern = r'\s*(_\S*)'
+    header_pattern = r"\s*(_\S*)"
 
     while lines:
         line = lines.pop()
         match = re.match(header_pattern, line)
 
         if match:
             header = match.group(1).lower()
             yield header
-        elif re.match(r'\s*#', line):
+        elif re.match(r"\s*#", line):
             # XXX we should filter comments out already.
             continue
         else:
             lines.append(line)  # 'undo' pop
             return
 
 
-def parse_cif_loop_data(lines: List[str],
-                        ncolumns: int) -> List[List[CIFDataValue]]:
+def parse_cif_loop_data(lines: List[str], ncolumns: int) -> List[List[CIFDataValue]]:
     columns: List[List[CIFDataValue]] = [[] for _ in range(ncolumns)]
 
     tokens = []
     while lines:
         line = lines.pop().strip()
         lowerline = line.lower()
-        if (not line or
-              line.startswith('_') or
-              lowerline.startswith('data_') or
-              lowerline.startswith('loop_')):
+        if (
+            not line
+            or line.startswith("_")
+            or lowerline.startswith("data_")
+            or lowerline.startswith("loop_")
+        ):
             lines.append(line)
             break
 
-        if line.startswith('#'):
+        if line.startswith("#"):
             continue
 
-        if line.startswith(';'):
+        if line.startswith(";"):
             moretokens = [parse_multiline_string(lines, line)]
         else:
             if ncolumns == 1:
                 moretokens = [line]
             else:
                 moretokens = shlex.split(line, posix=False)
 
         tokens += moretokens
         if len(tokens) < ncolumns:
             continue
         if len(tokens) == ncolumns:
             for i, token in enumerate(tokens):
                 columns[i].append(convert_value(token))
         else:
-            warnings.warn('Wrong number {} of tokens, expected {}: {}'
-                          .format(len(tokens), ncolumns, tokens))
+            warnings.warn(
+                "Wrong number {} of tokens, expected {}: {}".format(
+                    len(tokens), ncolumns, tokens
+                )
+            )
 
         # (Due to continue statements we cannot move this to start of loop)
         tokens = []
 
     if tokens:
         assert len(tokens) < ncolumns
-        raise RuntimeError('CIF loop ended unexpectedly with incomplete row')
+        raise RuntimeError("CIF loop ended unexpectedly with incomplete row")
 
     return columns
 
 
 def parse_loop(lines: List[str]) -> Dict[str, List[CIFDataValue]]:
     """Parse a CIF loop. Returns a dict with column tag names as keys
     and a lists of the column content as values."""
@@ -159,15 +163,15 @@
     # Dict would be better.  But there can be repeated headers.
 
     columns = parse_cif_loop_data(lines, len(headers))
 
     columns_dict = {}
     for i, header in enumerate(headers):
         if header in columns_dict:
-            warnings.warn('Duplicated loop tags: {0}'.format(header))
+            warnings.warn("Duplicated loop tags: {0}".format(header))
         else:
             columns_dict[header] = columns[i]
     return columns_dict
 
 
 def parse_items(lines: List[str], line: str) -> Dict[str, CIFData]:
     """Parse a CIF data items and return a dict with all tags."""
@@ -176,26 +180,26 @@
     while True:
         if not lines:
             break
         line = lines.pop().strip()
         if not line:
             continue
         lowerline = line.lower()
-        if not line or line.startswith('#'):
+        if not line or line.startswith("#"):
             continue
-        elif line.startswith('_'):
+        elif line.startswith("_"):
             key, value = parse_singletag(lines, line)
             tags[key.lower()] = value
-        elif lowerline.startswith('loop_'):
+        elif lowerline.startswith("loop_"):
             tags.update(parse_loop(lines))
-        elif lowerline.startswith('data_'):
+        elif lowerline.startswith("data_"):
             if line:
                 lines.append(line)
             break
-        elif line.startswith(';'):
+        elif line.startswith(";"):
             parse_multiline_string(lines, line)
         else:
             raise ValueError('Unexpected CIF file entry: "{0}"'.format(line))
     return tags
 
 
 class NoStructureData(RuntimeError):
@@ -203,24 +207,30 @@
 
 
 class CIFBlock(collections.abc.Mapping):
     """A block (i.e., a single system) in a crystallographic information file.
 
     Use this object to query CIF tags or import information as ASE objects."""
 
-    cell_tags = ['_cell_length_a', '_cell_length_b', '_cell_length_c',
-                 '_cell_angle_alpha', '_cell_angle_beta', '_cell_angle_gamma']
+    cell_tags = [
+        "_cell_length_a",
+        "_cell_length_b",
+        "_cell_length_c",
+        "_cell_angle_alpha",
+        "_cell_angle_beta",
+        "_cell_angle_gamma",
+    ]
 
     def __init__(self, name: str, tags: Dict[str, CIFData]):
         self.name = name
         self._tags = tags
 
     def __repr__(self) -> str:
         tags = set(self._tags)
-        return f'CIFBlock({self.name}, tags={tags})'
+        return f"CIFBlock({self.name}, tags={tags})"
 
     def __getitem__(self, key: str) -> CIFData:
         return self._tags[key]
 
     def __iter__(self) -> Iterator[str]:
         return iter(self._tags)
 
@@ -239,67 +249,74 @@
     def get_cell(self) -> Cell:
         cellpar = self.get_cellpar()
         if cellpar is None:
             return Cell.new([0, 0, 0])
         return Cell.new(cellpar)
 
     def _raw_scaled_positions(self) -> Optional[np.ndarray]:
-        coords = [self.get(name) for name in ['_atom_site_fract_x',
-                                              '_atom_site_fract_y',
-                                              '_atom_site_fract_z']]
+        coords = [
+            self.get(name)
+            for name in [
+                "_atom_site_fract_x",
+                "_atom_site_fract_y",
+                "_atom_site_fract_z",
+            ]
+        ]
         # XXX Shall we try to handle mixed coordinates?
         # (Some scaled vs others fractional)
         if None in coords:
             return None
         return np.array(coords).T
 
     def _raw_positions(self) -> Optional[np.ndarray]:
-        coords = [self.get('_atom_site_cartn_x'),
-                  self.get('_atom_site_cartn_y'),
-                  self.get('_atom_site_cartn_z')]
+        coords = [
+            self.get("_atom_site_cartn_x"),
+            self.get("_atom_site_cartn_y"),
+            self.get("_atom_site_cartn_z"),
+        ]
         if None in coords:
             return None
         return np.array(coords).T
 
     def _get_site_coordinates(self):
         scaled = self._raw_scaled_positions()
 
         if scaled is not None:
-            return 'scaled', scaled
+            return "scaled", scaled
 
         cartesian = self._raw_positions()
 
         if cartesian is None:
-            raise NoStructureData('No positions found in structure')
+            raise NoStructureData("No positions found in structure")
 
-        return 'cartesian', cartesian
+        return "cartesian", cartesian
 
     def _get_symbols_with_deuterium(self):
-        labels = self._get_any(['_atom_site_type_symbol',
-                                '_atom_site_label'])
+        labels = self._get_any(["_atom_site_type_symbol", "_atom_site_label"])
         if labels is None:
-            raise NoStructureData('No symbols')
+            raise NoStructureData("No symbols")
 
         symbols = []
         for label in labels:
-            if label == '.' or label == '?':
-                raise NoStructureData('Symbols are undetermined')
+            if label == "." or label == "?":
+                raise NoStructureData("Symbols are undetermined")
             # Strip off additional labeling on chemical symbols
-            match = re.search(r'([A-Z][a-z]?)', label)
+            match = re.search(r"([A-Z][a-z]?)", label)
             symbol = match.group(0)
             symbols.append(symbol)
         return symbols
 
     def get_symbols(self) -> List[str]:
         symbols = self._get_symbols_with_deuterium()
-        return [symbol if symbol != 'D' else 'H' for symbol in symbols]
+        return [symbol if symbol != "D" else "H" for symbol in symbols]
 
     def _where_deuterium(self):
-        return np.array([symbol == 'D' for symbol
-                         in self._get_symbols_with_deuterium()], bool)
+        return np.array(
+            [symbol == "D" for symbol in self._get_symbols_with_deuterium()], bool
+        )
 
     def _get_masses(self) -> Optional[np.ndarray]:
         mask = self._where_deuterium()
         if not any(mask):
             return None
 
         symbols = self.get_symbols()
@@ -314,98 +331,114 @@
         return None
 
     def _get_spacegroup_number(self):
         # Symmetry specification, see
         # http://www.iucr.org/resources/cif/dictionaries/cif_sym for a
         # complete list of official keys.  In addition we also try to
         # support some commonly used depricated notations
-        return self._get_any(['_space_group.it_number',
-                              '_space_group_it_number',
-                              '_symmetry_int_tables_number'])
+        return self._get_any(
+            [
+                "_space_group.it_number",
+                "_space_group_it_number",
+                "_symmetry_int_tables_number",
+            ]
+        )
 
     def _get_spacegroup_name(self):
-        hm_symbol = self._get_any(['_space_group_name_h-m_alt',
-                                   '_symmetry_space_group_name_h-m',
-                                   '_space_group.Patterson_name_h-m',
-                                   '_space_group.patterson_name_h-m'])
+        hm_symbol = self._get_any(
+            [
+                "_space_group_name_h-m_alt",
+                "_symmetry_space_group_name_h-m",
+                "_space_group.Patterson_name_h-m",
+                "_space_group.patterson_name_h-m",
+            ]
+        )
 
         hm_symbol = old_spacegroup_names.get(hm_symbol, hm_symbol)
         return hm_symbol
 
     def _get_sitesym(self):
-        sitesym = self._get_any(['_space_group_symop_operation_xyz',
-                                 '_space_group_symop.operation_xyz',
-                                 '_symmetry_equiv_pos_as_xyz'])
+        sitesym = self._get_any(
+            [
+                "_space_group_symop_operation_xyz",
+                "_space_group_symop.operation_xyz",
+                "_symmetry_equiv_pos_as_xyz",
+            ]
+        )
         if isinstance(sitesym, str):
             sitesym = [sitesym]
         return sitesym
 
     def _get_fractional_occupancies(self):
-        return self.get('_atom_site_occupancy')
+        return self.get("_atom_site_occupancy")
 
     def _get_setting(self) -> Optional[int]:
-        setting_str = self.get('_symmetry_space_group_setting')
+        setting_str = self.get("_symmetry_space_group_setting")
         if setting_str is None:
             return None
 
         setting = int(setting_str)
         if setting not in [1, 2]:
-            raise ValueError(
-                f'Spacegroup setting must be 1 or 2, not {setting}')
+            raise ValueError(f"Spacegroup setting must be 1 or 2, not {setting}")
         return setting
 
     def get_spacegroup(self, subtrans_included) -> Spacegroup:
         # XXX The logic in this method needs serious cleaning up!
         # The setting needs to be passed as either 1 or two, not None (default)
         no = self._get_spacegroup_number()
         hm_symbol = self._get_spacegroup_name()
         sitesym = self._get_sitesym()
 
         setting = 1
         spacegroup = 1
         if sitesym is not None:
             subtrans = [(0.0, 0.0, 0.0)] if subtrans_included else None
             spacegroup = spacegroup_from_data(
-                no=no, symbol=hm_symbol, sitesym=sitesym, subtrans=subtrans,
-                setting=setting)
+                no=no,
+                symbol=hm_symbol,
+                sitesym=sitesym,
+                subtrans=subtrans,
+                setting=setting,
+            )
         elif no is not None:
             spacegroup = no
         elif hm_symbol is not None:
             spacegroup = hm_symbol
         else:
             spacegroup = 1
 
         setting_std = self._get_setting()
 
         setting_name = None
-        if '_symmetry_space_group_setting' in self:
+        if "_symmetry_space_group_setting" in self:
             assert setting_std is not None
             setting = setting_std
-        elif '_space_group_crystal_system' in self:
-            setting_name = self['_space_group_crystal_system']
-        elif '_symmetry_cell_setting' in self:
-            setting_name = self['_symmetry_cell_setting']
+        elif "_space_group_crystal_system" in self:
+            setting_name = self["_space_group_crystal_system"]
+        elif "_symmetry_cell_setting" in self:
+            setting_name = self["_symmetry_cell_setting"]
 
         if setting_name:
             no = Spacegroup(spacegroup).no
             if no in rhombohedral_spacegroups:
-                if setting_name == 'hexagonal':
+                if setting_name == "hexagonal":
                     setting = 1
-                elif setting_name in ('trigonal', 'rhombohedral'):
+                elif setting_name in ("trigonal", "rhombohedral"):
                     setting = 2
                 else:
                     warnings.warn(
-                        'unexpected crystal system %r for space group %r' % (
-                            setting_name, spacegroup))
+                        "unexpected crystal system %r for space group %r"
+                        % (setting_name, spacegroup)
+                    )
             # FIXME - check for more crystal systems...
             else:
                 warnings.warn(
-                    'crystal system %r is not interpreted for space group %r. '
-                    'This may result in wrong setting!' % (
-                        setting_name, spacegroup))
+                    "crystal system %r is not interpreted for space group %r. "
+                    "This may result in wrong setting!" % (setting_name, spacegroup)
+                )
 
         spg = Spacegroup(spacegroup, setting)
         if no is not None:
             assert int(spg) == no, (int(spg), no)
         return spg
 
     def get_unsymmetrized_structure(self) -> Atoms:
@@ -415,160 +448,175 @@
         corresponding only to those coordinates included
         in the CIF file, useful for e.g. debugging.
 
         This method may change behaviour in the future."""
         symbols = self.get_symbols()
         coordtype, coords = self._get_site_coordinates()
 
-        atoms = Atoms(symbols=symbols,
-                      cell=self.get_cell(),
-                      masses=self._get_masses())
+        atoms = Atoms(symbols=symbols, cell=self.get_cell(), masses=self._get_masses())
 
-        if coordtype == 'scaled':
+        if coordtype == "scaled":
             atoms.set_scaled_positions(coords)
         else:
-            assert coordtype == 'cartesian'
+            assert coordtype == "cartesian"
             atoms.positions[:] = coords
 
         return atoms
 
     def has_structure(self):
         """Whether this CIF block has an atomic configuration."""
         try:
             self.get_symbols()
             self._get_site_coordinates()
         except NoStructureData:
             return False
         else:
             return True
 
-    def get_atoms(self, store_tags=False, primitive_cell=False,
-                  subtrans_included=True, fractional_occupancies=True) -> Atoms:
+    def get_atoms(
+        self,
+        store_tags=False,
+        primitive_cell=False,
+        subtrans_included=True,
+        fractional_occupancies=True,
+    ) -> Atoms:
         """Returns an Atoms object from a cif tags dictionary.  See read_cif()
         for a description of the arguments."""
         if primitive_cell and subtrans_included:
             raise RuntimeError(
-                'Primitive cell cannot be determined when sublattice '
-                'translations are included in the symmetry operations listed '
-                'in the CIF file, i.e. when `subtrans_included` is True.')
+                "Primitive cell cannot be determined when sublattice "
+                "translations are included in the symmetry operations listed "
+                "in the CIF file, i.e. when `subtrans_included` is True."
+            )
 
         cell = self.get_cell()
         assert cell.rank in [0, 3]
 
         kwargs: Dict[str, Any] = {}
         if store_tags:
-            kwargs['info'] = self._tags.copy()
+            kwargs["info"] = self._tags.copy()
 
         if fractional_occupancies:
             occupancies = self._get_fractional_occupancies()
         else:
             occupancies = None
 
         if occupancies is not None:
             # no warnings in this case
-            kwargs['onduplicates'] = 'keep'
+            kwargs["onduplicates"] = "keep"
 
         # The unsymmetrized_structure is not the asymmetric unit
         # because the asymmetric unit should have (in general) a smaller cell,
         # whereas we have the full cell.
         unsymmetrized_structure = self.get_unsymmetrized_structure()
 
         if cell.rank == 3:
             spacegroup = self.get_spacegroup(subtrans_included)
-            atoms = crystal(unsymmetrized_structure,
-                            spacegroup=spacegroup,
-                            setting=spacegroup.setting,
-                            occupancies=occupancies,
-                            primitive_cell=primitive_cell,
-                            **kwargs)
+            atoms = crystal(
+                unsymmetrized_structure,
+                spacegroup=spacegroup,
+                setting=spacegroup.setting,
+                occupancies=occupancies,
+                primitive_cell=primitive_cell,
+                **kwargs,
+            )
         else:
             atoms = unsymmetrized_structure
-            if kwargs.get('info') is not None:
-                atoms.info.update(kwargs['info'])
+            if kwargs.get("info") is not None:
+                atoms.info.update(kwargs["info"])
             if occupancies is not None:
                 # Compile an occupancies dictionary
                 occ_dict = {}
                 for i, sym in enumerate(atoms.symbols):
                     occ_dict[str(i)] = {sym: occupancies[i]}
-                atoms.info['occupancy'] = occ_dict
+                atoms.info["occupancy"] = occ_dict
 
         return atoms
 
 
 def parse_block(lines: List[str], line: str) -> CIFBlock:
-    assert line.lower().startswith('data_')
-    blockname = line.split('_', 1)[1].rstrip()
+    assert line.lower().startswith("data_")
+    blockname = line.split("_", 1)[1].rstrip()
     tags = parse_items(lines, line)
     return CIFBlock(blockname, tags)
 
 
-def parse_cif(fileobj, reader='ase') -> Iterator[CIFBlock]:
-    if reader == 'ase':
+def parse_cif(fileobj, reader="ase") -> Iterator[CIFBlock]:
+    if reader == "ase":
         return parse_cif_ase(fileobj)
-    elif reader == 'pycodcif':
+    elif reader == "pycodcif":
         return parse_cif_pycodcif(fileobj)
     else:
-        raise ValueError(f'No such reader: {reader}')
+        raise ValueError(f"No such reader: {reader}")
 
 
 def parse_cif_ase(fileobj) -> Iterator[CIFBlock]:
     """Parse a CIF file using ase CIF parser."""
 
     if isinstance(fileobj, str):
-        with open(fileobj, 'rb') as fileobj:
+        with open(fileobj, "rb") as fileobj:
             data = fileobj.read()
     else:
         data = fileobj.read()
 
     if isinstance(data, bytes):
-        data = data.decode('latin1')
+        data = data.decode("latin1")
     data = format_unicode(data)
-    lines = [e for e in data.split('\n') if len(e) > 0]
-    if len(lines) > 0 and lines[0].rstrip() == '#\\#CIF_2.0':
-        warnings.warn('CIF v2.0 file format detected; `ase` CIF reader might '
-                      'incorrectly interpret some syntax constructions, use '
-                      '`pycodcif` reader instead')
-    lines = [''] + lines[::-1]    # all lines (reversed)
+    lines = [e for e in data.split("\n") if len(e) > 0]
+    if len(lines) > 0 and lines[0].rstrip() == "#\\#CIF_2.0":
+        warnings.warn(
+            "CIF v2.0 file format detected; `ase` CIF reader might "
+            "incorrectly interpret some syntax constructions, use "
+            "`pycodcif` reader instead"
+        )
+    lines = [""] + lines[::-1]  # all lines (reversed)
 
     while lines:
         line = lines.pop().strip()
-        if not line or line.startswith('#'):
+        if not line or line.startswith("#"):
             continue
 
         yield parse_block(lines, line)
 
 
 def parse_cif_pycodcif(fileobj) -> Iterator[CIFBlock]:
     """Parse a CIF file using pycodcif CIF parser."""
     if not isinstance(fileobj, str):
         fileobj = fileobj.name
 
     try:
         from pycodcif import parse
     except ImportError:
         raise ImportError(
-            'parse_cif_pycodcif requires pycodcif ' +
-            '(http://wiki.crystallography.net/cod-tools/pycodcif/)')
+            "parse_cif_pycodcif requires pycodcif "
+            + "(http://wiki.crystallography.net/cod-tools/pycodcif/)"
+        )
 
     data, _, _ = parse(fileobj)
 
     for datablock in data:
-        tags = datablock['values']
+        tags = datablock["values"]
         for tag in tags.keys():
             values = [convert_value(x) for x in tags[tag]]
             if len(values) == 1:
                 tags[tag] = values[0]
             else:
                 tags[tag] = values
-        yield CIFBlock(datablock['name'], tags)
+        yield CIFBlock(datablock["name"], tags)
 
 
-def read_cif(fileobj, index, store_tags=False, primitive_cell=False,
-             subtrans_included=True, fractional_occupancies=True,
-             reader='ase') -> Iterator[Atoms]:
+def read_cif(
+    fileobj,
+    index,
+    store_tags=False,
+    primitive_cell=False,
+    subtrans_included=True,
+    fractional_occupancies=True,
+    reader="ase",
+) -> Iterator[Atoms]:
     """Read Atoms object from CIF file. *index* specifies the data
     block number or name (if string) to return.
 
     If *index* is None or a slice object, a list of atoms objects will
     be returned. In the case of *index* is *None* or *slice(None)*,
     only blocks with valid crystal data will be included.
 
@@ -602,83 +650,90 @@
     # Find all CIF blocks with valid crystal data
     images = []
     for block in parse_cif(fileobj, reader):
         if not block.has_structure():
             continue
 
         atoms = block.get_atoms(
-            store_tags, primitive_cell,
+            store_tags,
+            primitive_cell,
             subtrans_included,
-            fractional_occupancies=fractional_occupancies)
+            fractional_occupancies=fractional_occupancies,
+        )
         images.append(atoms)
 
     for atoms in images[index]:
         yield atoms
 
 
 def format_cell(cell: Cell) -> str:
     assert cell.rank == 3
     lines = []
     for name, value in zip(CIFBlock.cell_tags, cell.cellpar()):
-        line = '{:20} {:g}\n'.format(name, value)
+        line = "{:20} {:g}\n".format(name, value)
         lines.append(line)
     assert len(lines) == 6
-    return ''.join(lines)
+    return "".join(lines)
 
 
 def format_generic_spacegroup_info() -> str:
     # We assume no symmetry whatsoever
-    return '\n'.join([
-        '_space_group_name_H-M_alt    "P 1"',
-        '_space_group_IT_number       1',
-        '',
-        'loop_',
-        '  _space_group_symop_operation_xyz',
-        "  'x, y, z'",
-        '',
-    ])
+    return "\n".join(
+        [
+            '_space_group_name_H-M_alt    "P 1"',
+            "_space_group_IT_number       1",
+            "",
+            "loop_",
+            "  _space_group_symop_operation_xyz",
+            "  'x, y, z'",
+            "",
+        ]
+    )
 
 
 class CIFLoop:
     def __init__(self):
         self.names = []
         self.formats = []
         self.arrays = []
 
     def add(self, name, array, fmt):
-        assert name.startswith('_')
+        assert name.startswith("_")
         self.names.append(name)
         self.formats.append(fmt)
         self.arrays.append(array)
         if len(self.arrays[0]) != len(self.arrays[-1]):
-            raise ValueError(f'Loop data "{name}" has {len(array)} '
-                             'elements, expected {len(self.arrays[0])}')
+            raise ValueError(
+                f'Loop data "{name}" has {len(array)} '
+                "elements, expected {len(self.arrays[0])}"
+            )
 
     def tostring(self):
         lines = []
         append = lines.append
-        append('loop_')
+        append("loop_")
         for name in self.names:
-            append(f'  {name}')
+            append(f"  {name}")
 
-        template = '  ' + '  '.join(self.formats)
+        template = "  " + "  ".join(self.formats)
 
         ncolumns = len(self.arrays)
         nrows = len(self.arrays[0]) if ncolumns > 0 else 0
         for row in range(nrows):
             arraydata = [array[row] for array in self.arrays]
             line = template.format(*arraydata)
             append(line)
-        append('')
-        return '\n'.join(lines)
+        append("")
+        return "\n".join(lines)
 
 
-@iofunction('wb')
-def write_cif(fd, images, cif_format=None,
-              wrap=True, labels=None, loop_keys=None) -> None:
+@iofunction("wb")
+def write_cif(
+    fd, images, cif_format=None, wrap=True, labels=None, loop_keys=None
+) -> None:
     """Write *images* to CIF file.
 
     wrap: bool
         Wrap atoms into unit cell.
 
     labels: list
         Use this list (shaped list[i_frame][i_atom] = string) for the
@@ -693,34 +748,41 @@
         string`. The strings are printed as they are, so take care of
         formating. Information can be re-read using the `store_tags`
         option of the cif reader.
 
     """
 
     if cif_format is not None:
-        warnings.warn('The cif_format argument is deprecated and may be '
-                      'removed in the future.  Use loop_keys to customize '
-                      'data written in loop.', FutureWarning)
+        warnings.warn(
+            "The cif_format argument is deprecated and may be "
+            "removed in the future.  Use loop_keys to customize "
+            "data written in loop.",
+            FutureWarning,
+        )
 
     if loop_keys is None:
         loop_keys = {}
 
-    if hasattr(images, 'get_positions'):
+    if hasattr(images, "get_positions"):
         images = [images]
 
-    fd = io.TextIOWrapper(fd, encoding='latin-1')
+    fd = io.TextIOWrapper(fd, encoding="latin-1")
     try:
         for i, atoms in enumerate(images):
-            blockname = f'data_image{i}\n'
+            blockname = f"data_image{i}\n"
             image_loop_keys = {key: loop_keys[key][i] for key in loop_keys}
 
-            write_cif_image(blockname, atoms, fd,
-                            wrap=wrap,
-                            labels=None if labels is None else labels[i],
-                            loop_keys=image_loop_keys)
+            write_cif_image(
+                blockname,
+                atoms,
+                fd,
+                wrap=wrap,
+                labels=None if labels is None else labels[i],
+                loop_keys=image_loop_keys,
+            )
 
     finally:
         # Using the TextIOWrapper somehow causes the file to close
         # when this function returns.
         # Detach in order to circumvent this highly illogical problem:
         fd.detach()
 
@@ -729,123 +791,123 @@
     no: Dict[str, int] = {}
     labels = []
     for symbol in symbols:
         if symbol in no:
             no[symbol] += 1
         else:
             no[symbol] = 1
-        labels.append('%s%d' % (symbol, no[symbol]))
+        labels.append("%s%d" % (symbol, no[symbol]))
     return labels
 
 
 def chemical_formula_header(atoms):
     counts = atoms.symbols.formula.count()
-    formula_sum = ' '.join(f'{sym}{count}' for sym, count
-                           in counts.items())
-    return (f'_chemical_formula_structural       {atoms.symbols}\n'
-            f'_chemical_formula_sum              "{formula_sum}"\n')
+    formula_sum = " ".join(f"{sym}{count}" for sym, count in counts.items())
+    return (
+        f"_chemical_formula_structural       {atoms.symbols}\n"
+        f'_chemical_formula_sum              "{formula_sum}"\n'
+    )
 
 
 class BadOccupancies(ValueError):
     pass
 
 
 def expand_kinds(atoms, coords):
     # try to fetch occupancies // spacegroup_kinds - occupancy mapping
     symbols = list(atoms.symbols)
     coords = list(coords)
     occupancies = [1] * len(symbols)
-    occ_info = atoms.info.get('occupancy')
-    kinds = atoms.arrays.get('spacegroup_kinds')
+    occ_info = atoms.info.get("occupancy")
+    kinds = atoms.arrays.get("spacegroup_kinds")
     if occ_info is not None and kinds is not None:
         for i, kind in enumerate(kinds):
             occ_info_kind = occ_info[str(kind)]
             symbol = symbols[i]
             if symbol not in occ_info_kind:
-                raise BadOccupancies('Occupancies present but no occupancy '
-                                     'info for "{symbol}"')
+                raise BadOccupancies(
+                    "Occupancies present but no occupancy " 'info for "{symbol}"'
+                )
             occupancies[i] = occ_info_kind[symbol]
             # extend the positions array in case of mixed occupancy
             for sym, occ in occ_info[str(kind)].items():
                 if sym != symbols[i]:
                     symbols.append(sym)
                     coords.append(coords[i])
                     occupancies.append(occ)
     return symbols, coords, occupancies
 
 
 def atoms_to_loop_data(atoms, wrap, labels, loop_keys):
     if atoms.cell.rank == 3:
-        coord_type = 'fract'
+        coord_type = "fract"
         coords = atoms.get_scaled_positions(wrap).tolist()
     else:
-        coord_type = 'Cartn'
+        coord_type = "Cartn"
         coords = atoms.get_positions(wrap).tolist()
 
     try:
         symbols, coords, occupancies = expand_kinds(atoms, coords)
     except BadOccupancies as err:
         warnings.warn(str(err))
         occupancies = [1] * len(atoms)
         symbols = list(atoms.symbols)
 
     if labels is None:
         labels = autolabel(symbols)
 
-    coord_headers = [f'_atom_site_{coord_type}_{axisname}'
-                     for axisname in 'xyz']
+    coord_headers = [f"_atom_site_{coord_type}_{axisname}" for axisname in "xyz"]
 
     loopdata = {}
-    loopdata['_atom_site_label'] = (labels, '{:<8s}')
-    loopdata['_atom_site_occupancy'] = (occupancies, '{:6.4f}')
+    loopdata["_atom_site_label"] = (labels, "{:<8s}")
+    loopdata["_atom_site_occupancy"] = (occupancies, "{:6.4f}")
 
     _coords = np.array(coords)
     for i, key in enumerate(coord_headers):
-        loopdata[key] = (_coords[:, i], '{:7.5f}')
+        loopdata[key] = (_coords[:, i], "{:7.5f}")
 
-    loopdata['_atom_site_type_symbol'] = (symbols, '{:<2s}')
-    loopdata['_atom_site_symmetry_multiplicity'] = (
-        [1.0] * len(symbols), '{}')
+    loopdata["_atom_site_type_symbol"] = (symbols, "{:<2s}")
+    loopdata["_atom_site_symmetry_multiplicity"] = ([1.0] * len(symbols), "{}")
 
     for key in loop_keys:
         # Should expand the loop_keys like we expand the occupancy stuff.
         # Otherwise user will never figure out how to do this.
         values = [loop_keys[key][i] for i in range(len(symbols))]
-        loopdata['_' + key] = (values, '{}')
+        loopdata["_" + key] = (values, "{}")
 
     return loopdata, coord_headers
 
 
-def write_cif_image(blockname, atoms, fd, *, wrap,
-                    labels, loop_keys):
+def write_cif_image(blockname, atoms, fd, *, wrap, labels, loop_keys):
     fd.write(blockname)
     fd.write(chemical_formula_header(atoms))
 
     rank = atoms.cell.rank
     if rank == 3:
         fd.write(format_cell(atoms.cell))
-        fd.write('\n')
+        fd.write("\n")
         fd.write(format_generic_spacegroup_info())
-        fd.write('\n')
+        fd.write("\n")
     elif rank != 0:
-        raise ValueError('CIF format can only represent systems with '
-                         f'0 or 3 lattice vectors.  Got {rank}.')
+        raise ValueError(
+            "CIF format can only represent systems with "
+            f"0 or 3 lattice vectors.  Got {rank}."
+        )
 
-    loopdata, coord_headers = atoms_to_loop_data(atoms, wrap, labels,
-                                                 loop_keys)
+    loopdata, coord_headers = atoms_to_loop_data(atoms, wrap, labels, loop_keys)
 
     headers = [
-        '_atom_site_type_symbol',
-        '_atom_site_label',
-        '_atom_site_symmetry_multiplicity',
+        "_atom_site_type_symbol",
+        "_atom_site_label",
+        "_atom_site_symmetry_multiplicity",
         *coord_headers,
-        '_atom_site_occupancy',
+        "_atom_site_occupancy",
     ]
 
-    headers += ['_' + key for key in loop_keys]
+    headers += ["_" + key for key in loop_keys]
 
     loop = CIFLoop()
     for header in headers:
         array, fmt = loopdata[header]
         loop.add(header, array, fmt)
 
     fd.write(loop.tostring())
```

### Comparing `lawaf-0.1.0/lawaf/plot/mcif.py` & `lawaf-0.2.1/lawaf/plot/mcif.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 """
 Modified from ase cif module:
 https://gitlab.com/ase/ase/-/tree/91e5660cb468b411bb6141ea1394ae9e570f51b8/ase/io
 """
 
 
 """Module to read and write atoms in cif file format.
@@ -30,136 +29,139 @@
 from ase.io.cif_unicode import format_unicode, handle_subscripts
 from ase.utils import iofunction
 
 
 rhombohedral_spacegroups = {146, 148, 155, 160, 161, 166, 167}
 
 
-old_spacegroup_names = {'Abm2': 'Aem2',
-                        'Aba2': 'Aea2',
-                        'Cmca': 'Cmce',
-                        'Cmma': 'Cmme',
-                        'Ccca': 'Ccc1'}
+old_spacegroup_names = {
+    "Abm2": "Aem2",
+    "Aba2": "Aea2",
+    "Cmca": "Cmce",
+    "Cmma": "Cmme",
+    "Ccca": "Ccc1",
+}
 
 # CIF maps names to either single values or to multiple values via loops.
 CIFDataValue = Union[str, int, float]
 CIFData = Union[CIFDataValue, List[CIFDataValue]]
 
 
 def convert_value(value: str) -> CIFDataValue:
     """Convert CIF value string to corresponding python type."""
     value = value.strip()
-    if re.match('(".*")|(\'.*\')$', value):
+    if re.match("(\".*\")|('.*')$", value):
         return handle_subscripts(value[1:-1])
-    elif re.match(r'[+-]?\d+$', value):
+    elif re.match(r"[+-]?\d+$", value):
         return int(value)
-    elif re.match(r'[+-]?(?:\d+(?:\.\d*)?|\.\d+)(?:[eE][+-]?\d+)?$', value):
+    elif re.match(r"[+-]?(?:\d+(?:\.\d*)?|\.\d+)(?:[eE][+-]?\d+)?$", value):
         return float(value)
-    elif re.match(r'[+-]?(?:\d+(?:\.\d*)?|\.\d+)(?:[eE][+-]?\d+)?\(\d+\)$',
-                  value):
-        return float(value[:value.index('(')])  # strip off uncertainties
-    elif re.match(r'[+-]?(?:\d+(?:\.\d*)?|\.\d+)(?:[eE][+-]?\d+)?\(\d+$',
-                  value):
+    elif re.match(r"[+-]?(?:\d+(?:\.\d*)?|\.\d+)(?:[eE][+-]?\d+)?\(\d+\)$", value):
+        return float(value[: value.index("(")])  # strip off uncertainties
+    elif re.match(r"[+-]?(?:\d+(?:\.\d*)?|\.\d+)(?:[eE][+-]?\d+)?\(\d+$", value):
         warnings.warn('Badly formed number: "{0}"'.format(value))
-        return float(value[:value.index('(')])  # strip off uncertainties
+        return float(value[: value.index("(")])  # strip off uncertainties
     else:
         return handle_subscripts(value)
 
 
 def parse_multiline_string(lines: List[str], line: str) -> str:
     """Parse semicolon-enclosed multiline string and return it."""
-    assert line[0] == ';'
+    assert line[0] == ";"
     strings = [line[1:].lstrip()]
     while True:
         line = lines.pop().strip()
-        if line[:1] == ';':
+        if line[:1] == ";":
             break
         strings.append(line)
-    return '\n'.join(strings).strip()
+    return "\n".join(strings).strip()
 
 
 def parse_singletag(lines: List[str], line: str) -> Tuple[str, CIFDataValue]:
     """Parse a CIF tag (entries starting with underscore). Returns
     a key-value pair."""
     kv = line.split(None, 1)
     if len(kv) == 1:
         key = line
         line = lines.pop().strip()
-        while not line or line[0] == '#':
+        while not line or line[0] == "#":
             line = lines.pop().strip()
-        if line[0] == ';':
+        if line[0] == ";":
             value = parse_multiline_string(lines, line)
         else:
             value = line
     else:
         key, value = kv
     return key, convert_value(value)
 
 
-
 def parse_cif_loop_headers(lines: List[str]) -> Iterator[str]:
-    header_pattern = r'\s*(_\S*)'
+    header_pattern = r"\s*(_\S*)"
 
     while lines:
         line = lines.pop()
         match = re.match(header_pattern, line)
 
         if match:
             header = match.group(1).lower()
             yield header
-        elif re.match(r'\s*#', line):
+        elif re.match(r"\s*#", line):
             # XXX we should filter comments out already.
             continue
         else:
             lines.append(line)  # 'undo' pop
             return
 
 
-def parse_cif_loop_data(lines: List[str],
-                        ncolumns: int) -> List[List[CIFDataValue]]:
+def parse_cif_loop_data(lines: List[str], ncolumns: int) -> List[List[CIFDataValue]]:
     columns: List[List[CIFDataValue]] = [[] for _ in range(ncolumns)]
 
     tokens = []
     while lines:
         line = lines.pop().strip()
         lowerline = line.lower()
-        if (not line or
-              line.startswith('_') or
-              lowerline.startswith('data_') or
-              lowerline.startswith('loop_')):
+        if (
+            not line
+            or line.startswith("_")
+            or lowerline.startswith("data_")
+            or lowerline.startswith("loop_")
+        ):
             lines.append(line)
             break
 
-        if line.startswith('#'):
+        if line.startswith("#"):
             continue
 
-        if line.startswith(';'):
+        if line.startswith(";"):
             moretokens = [parse_multiline_string(lines, line)]
         else:
             if ncolumns == 1:
                 moretokens = [line]
             else:
                 moretokens = shlex.split(line, posix=False)
 
         tokens += moretokens
         if len(tokens) < ncolumns:
             continue
         if len(tokens) == ncolumns:
             for i, token in enumerate(tokens):
                 columns[i].append(convert_value(token))
         else:
-            warnings.warn('Wrong number {} of tokens, expected {}: {}'
-                          .format(len(tokens), ncolumns, tokens))
+            warnings.warn(
+                "Wrong number {} of tokens, expected {}: {}".format(
+                    len(tokens), ncolumns, tokens
+                )
+            )
 
         # (Due to continue statements we cannot move this to start of loop)
         tokens = []
 
     if tokens:
         assert len(tokens) < ncolumns
-        raise RuntimeError('CIF loop ended unexpectedly with incomplete row')
+        raise RuntimeError("CIF loop ended unexpectedly with incomplete row")
 
     return columns
 
 
 def parse_loop(lines: List[str]) -> Dict[str, List[CIFDataValue]]:
     """Parse a CIF loop. Returns a dict with column tag names as keys
     and a lists of the column content as values."""
@@ -168,15 +170,15 @@
     # Dict would be better.  But there can be repeated headers.
 
     columns = parse_cif_loop_data(lines, len(headers))
 
     columns_dict = {}
     for i, header in enumerate(headers):
         if header in columns_dict:
-            warnings.warn('Duplicated loop tags: {0}'.format(header))
+            warnings.warn("Duplicated loop tags: {0}".format(header))
         else:
             columns_dict[header] = columns[i]
     return columns_dict
 
 
 def parse_items(lines: List[str], line: str) -> Dict[str, CIFData]:
     """Parse a CIF data items and return a dict with all tags."""
@@ -184,26 +186,26 @@
     while True:
         if not lines:
             break
         line = lines.pop().strip()
         if not line:
             continue
         lowerline = line.lower()
-        if not line or line.startswith('#'):
+        if not line or line.startswith("#"):
             continue
-        elif line.startswith('_'):
+        elif line.startswith("_"):
             key, value = parse_singletag(lines, line)
             tags[key.lower()] = value
-        elif lowerline.startswith('loop_'):
+        elif lowerline.startswith("loop_"):
             tags.update(parse_loop(lines))
-        elif lowerline.startswith('data_'):
+        elif lowerline.startswith("data_"):
             if line:
                 lines.append(line)
             break
-        elif line.startswith(';'):
+        elif line.startswith(";"):
             parse_multiline_string(lines, line)
         else:
             raise ValueError('Unexpected CIF file entry: "{0}"'.format(line))
     return tags
 
 
 class NoStructureData(RuntimeError):
@@ -211,24 +213,30 @@
 
 
 class CIFBlock(collections.abc.Mapping):
     """A block (i.e., a single system) in a crystallographic information file.
 
     Use this object to query CIF tags or import information as ASE objects."""
 
-    cell_tags = ['_cell_length_a', '_cell_length_b', '_cell_length_c',
-                 '_cell_angle_alpha', '_cell_angle_beta', '_cell_angle_gamma']
+    cell_tags = [
+        "_cell_length_a",
+        "_cell_length_b",
+        "_cell_length_c",
+        "_cell_angle_alpha",
+        "_cell_angle_beta",
+        "_cell_angle_gamma",
+    ]
 
     def __init__(self, name: str, tags: Dict[str, CIFData]):
         self.name = name
         self._tags = tags
 
     def __repr__(self) -> str:
         tags = set(self._tags)
-        return f'CIFBlock({self.name}, tags={tags})'
+        return f"CIFBlock({self.name}, tags={tags})"
 
     def __getitem__(self, key: str) -> CIFData:
         return self._tags[key]
 
     def __iter__(self) -> Iterator[str]:
         return iter(self._tags)
 
@@ -247,66 +255,73 @@
     def get_cell(self) -> Cell:
         cellpar = self.get_cellpar()
         if cellpar is None:
             return Cell.new([0, 0, 0])
         return Cell.new(cellpar)
 
     def _raw_scaled_positions(self) -> Optional[np.ndarray]:
-        coords = [self.get(name) for name in ['_atom_site_fract_x',
-                                              '_atom_site_fract_y',
-                                              '_atom_site_fract_z']]
+        coords = [
+            self.get(name)
+            for name in [
+                "_atom_site_fract_x",
+                "_atom_site_fract_y",
+                "_atom_site_fract_z",
+            ]
+        ]
         # XXX Shall we try to handle mixed coordinates?
         # (Some scaled vs others fractional)
         if None in coords:
             return None
         return np.array(coords).T
 
     def _raw_positions(self) -> Optional[np.ndarray]:
-        coords = [self.get('_atom_site_cartn_x'),
-                  self.get('_atom_site_cartn_y'),
-                  self.get('_atom_site_cartn_z')]
+        coords = [
+            self.get("_atom_site_cartn_x"),
+            self.get("_atom_site_cartn_y"),
+            self.get("_atom_site_cartn_z"),
+        ]
         if None in coords:
             return None
         return np.array(coords).T
 
     def _get_site_coordinates(self):
         scaled = self._raw_scaled_positions()
 
         if scaled is not None:
-            return 'scaled', scaled
+            return "scaled", scaled
 
         cartesian = self._raw_positions()
 
         if cartesian is None:
-                raise NoStructureData('No positions found in structure')
-        return 'cartesian', cartesian
+            raise NoStructureData("No positions found in structure")
+        return "cartesian", cartesian
 
     def _get_symbols_with_deuterium(self):
-        labels = self._get_any(['_atom_site_type_symbol',
-                                '_atom_site_label'])
+        labels = self._get_any(["_atom_site_type_symbol", "_atom_site_label"])
         if labels is None:
-            raise NoStructureData('No symbols')
+            raise NoStructureData("No symbols")
 
         symbols = []
         for label in labels:
-            if label == '.' or label == '?':
-                raise NoStructureData('Symbols are undetermined')
+            if label == "." or label == "?":
+                raise NoStructureData("Symbols are undetermined")
             # Strip off additional labeling on chemical symbols
-            match = re.search(r'([A-Z][a-z]?)', label)
+            match = re.search(r"([A-Z][a-z]?)", label)
             symbol = match.group(0)
             symbols.append(symbol)
         return symbols
 
     def get_symbols(self) -> List[str]:
         symbols = self._get_symbols_with_deuterium()
-        return [symbol if symbol != 'D' else 'H' for symbol in symbols]
+        return [symbol if symbol != "D" else "H" for symbol in symbols]
 
     def _where_deuterium(self):
-        return np.array([symbol == 'D' for symbol
-                         in self._get_symbols_with_deuterium()], bool)
+        return np.array(
+            [symbol == "D" for symbol in self._get_symbols_with_deuterium()], bool
+        )
 
     def _get_masses(self) -> Optional[np.ndarray]:
         mask = self._where_deuterium()
         if not any(mask):
             return None
 
         symbols = self.get_symbols()
@@ -321,98 +336,114 @@
         return None
 
     def _get_spacegroup_number(self):
         # Symmetry specification, see
         # http://www.iucr.org/resources/cif/dictionaries/cif_sym for a
         # complete list of official keys.  In addition we also try to
         # support some commonly used depricated notations
-        return self._get_any(['_space_group.it_number',
-                              '_space_group_it_number',
-                              '_symmetry_int_tables_number'])
+        return self._get_any(
+            [
+                "_space_group.it_number",
+                "_space_group_it_number",
+                "_symmetry_int_tables_number",
+            ]
+        )
 
     def _get_spacegroup_name(self):
-        hm_symbol = self._get_any(['_space_group_name_h-m_alt',
-                                   '_symmetry_space_group_name_h-m',
-                                   '_space_group.Patterson_name_h-m',
-                                   '_space_group.patterson_name_h-m'])
+        hm_symbol = self._get_any(
+            [
+                "_space_group_name_h-m_alt",
+                "_symmetry_space_group_name_h-m",
+                "_space_group.Patterson_name_h-m",
+                "_space_group.patterson_name_h-m",
+            ]
+        )
 
         hm_symbol = old_spacegroup_names.get(hm_symbol, hm_symbol)
         return hm_symbol
 
     def _get_sitesym(self):
-        sitesym = self._get_any(['_space_group_symop_operation_xyz',
-                                 '_space_group_symop.operation_xyz',
-                                 '_symmetry_equiv_pos_as_xyz'])
+        sitesym = self._get_any(
+            [
+                "_space_group_symop_operation_xyz",
+                "_space_group_symop.operation_xyz",
+                "_symmetry_equiv_pos_as_xyz",
+            ]
+        )
         if isinstance(sitesym, str):
             sitesym = [sitesym]
         return sitesym
 
     def _get_fractional_occupancies(self):
-        return self.get('_atom_site_occupancy')
+        return self.get("_atom_site_occupancy")
 
     def _get_setting(self) -> Optional[int]:
-        setting_str = self.get('_symmetry_space_group_setting')
+        setting_str = self.get("_symmetry_space_group_setting")
         if setting_str is None:
             return None
 
         setting = int(setting_str)
         if setting not in [1, 2]:
-            raise ValueError(
-                f'Spacegroup setting must be 1 or 2, not {setting}')
+            raise ValueError(f"Spacegroup setting must be 1 or 2, not {setting}")
         return setting
 
     def get_spacegroup(self, subtrans_included) -> Spacegroup:
         # XXX The logic in this method needs serious cleaning up!
         # The setting needs to be passed as either 1 or two, not None (default)
         no = self._get_spacegroup_number()
         hm_symbol = self._get_spacegroup_name()
         sitesym = self._get_sitesym()
 
         setting = 1
         spacegroup = 1
         if sitesym is not None:
             subtrans = [(0.0, 0.0, 0.0)] if subtrans_included else None
             spacegroup = spacegroup_from_data(
-                no=no, symbol=hm_symbol, sitesym=sitesym, subtrans=subtrans,
-                setting=setting)
+                no=no,
+                symbol=hm_symbol,
+                sitesym=sitesym,
+                subtrans=subtrans,
+                setting=setting,
+            )
         elif no is not None:
             spacegroup = no
         elif hm_symbol is not None:
             spacegroup = hm_symbol
         else:
             spacegroup = 1
 
         setting_std = self._get_setting()
 
         setting_name = None
-        if '_symmetry_space_group_setting' in self:
+        if "_symmetry_space_group_setting" in self:
             assert setting_std is not None
             setting = setting_std
-        elif '_space_group_crystal_system' in self:
-            setting_name = self['_space_group_crystal_system']
-        elif '_symmetry_cell_setting' in self:
-            setting_name = self['_symmetry_cell_setting']
+        elif "_space_group_crystal_system" in self:
+            setting_name = self["_space_group_crystal_system"]
+        elif "_symmetry_cell_setting" in self:
+            setting_name = self["_symmetry_cell_setting"]
 
         if setting_name:
             no = Spacegroup(spacegroup).no
             if no in rhombohedral_spacegroups:
-                if setting_name == 'hexagonal':
+                if setting_name == "hexagonal":
                     setting = 1
-                elif setting_name in ('trigonal', 'rhombohedral'):
+                elif setting_name in ("trigonal", "rhombohedral"):
                     setting = 2
                 else:
                     warnings.warn(
-                        'unexpected crystal system %r for space group %r' % (
-                            setting_name, spacegroup))
+                        "unexpected crystal system %r for space group %r"
+                        % (setting_name, spacegroup)
+                    )
             # FIXME - check for more crystal systems...
             else:
                 warnings.warn(
-                    'crystal system %r is not interpreted for space group %r. '
-                    'This may result in wrong setting!' % (
-                        setting_name, spacegroup))
+                    "crystal system %r is not interpreted for space group %r. "
+                    "This may result in wrong setting!" % (setting_name, spacegroup)
+                )
 
         spg = Spacegroup(spacegroup, setting)
         if no is not None:
             assert int(spg) == no, (int(spg), no)
         return spg
 
     def get_unsymmetrized_structure(self) -> Atoms:
@@ -422,160 +453,175 @@
         corresponding only to those coordinates included
         in the CIF file, useful for e.g. debugging.
 
         This method may change behaviour in the future."""
         symbols = self.get_symbols()
         coordtype, coords = self._get_site_coordinates()
 
-        atoms = Atoms(symbols=symbols,
-                     cell=self.get_cell(),
-                      masses=self._get_masses())
+        atoms = Atoms(symbols=symbols, cell=self.get_cell(), masses=self._get_masses())
 
-        if coordtype == 'scaled':
+        if coordtype == "scaled":
             atoms.set_scaled_positions(coords)
         else:
-            assert coordtype == 'cartesian'
+            assert coordtype == "cartesian"
             atoms.positions[:] = coords
 
         return atoms
 
     def has_structure(self):
         """Whether this CIF block has an atomic configuration."""
         try:
             self.get_symbols()
             self._get_site_coordinates()
         except NoStructureData:
             return False
         else:
             return True
 
-    def get_atoms(self, store_tags=False, primitive_cell=False,
-                  subtrans_included=True, fractional_occupancies=True) -> Atoms:
+    def get_atoms(
+        self,
+        store_tags=False,
+        primitive_cell=False,
+        subtrans_included=True,
+        fractional_occupancies=True,
+    ) -> Atoms:
         """Returns an Atoms object from a cif tags dictionary.  See read_cif()
         for a description of the arguments."""
         if primitive_cell and subtrans_included:
             raise RuntimeError(
-                'Primitive cell cannot be determined when sublattice '
-                'translations are included in the symmetry operations listed '
-                'in the CIF file, i.e. when `subtrans_included` is True.')
+                "Primitive cell cannot be determined when sublattice "
+                "translations are included in the symmetry operations listed "
+                "in the CIF file, i.e. when `subtrans_included` is True."
+            )
 
         cell = self.get_cell()
         assert cell.rank in [0, 3]
 
         kwargs: Dict[str, Any] = {}
         if store_tags:
-            kwargs['info'] = self._tags.copy()
+            kwargs["info"] = self._tags.copy()
 
         if fractional_occupancies:
             occupancies = self._get_fractional_occupancies()
         else:
             occupancies = None
 
         if occupancies is not None:
             # no warnings in this case
-            kwargs['onduplicates'] = 'keep'
+            kwargs["onduplicates"] = "keep"
 
         # The unsymmetrized_structure is not the asymmetric unit
         # because the asymmetric unit should have (in general) a smaller cell,
         # whereas we have the full cell.
         unsymmetrized_structure = self.get_unsymmetrized_structure()
 
         if cell.rank == 3:
             spacegroup = self.get_spacegroup(subtrans_included)
-            atoms = crystal(unsymmetrized_structure,
-                            spacegroup=spacegroup,
-                            setting=spacegroup.setting,
-                            occupancies=occupancies,
-                            primitive_cell=primitive_cell,
-                            **kwargs)
+            atoms = crystal(
+                unsymmetrized_structure,
+                spacegroup=spacegroup,
+                setting=spacegroup.setting,
+                occupancies=occupancies,
+                primitive_cell=primitive_cell,
+                **kwargs,
+            )
         else:
             atoms = unsymmetrized_structure
-            if kwargs.get('info') is not None:
-                atoms.info.update(kwargs['info'])
+            if kwargs.get("info") is not None:
+                atoms.info.update(kwargs["info"])
             if occupancies is not None:
                 # Compile an occupancies dictionary
                 occ_dict = {}
                 for i, sym in enumerate(atoms.symbols):
                     occ_dict[str(i)] = {sym: occupancies[i]}
-                atoms.info['occupancy'] = occ_dict
+                atoms.info["occupancy"] = occ_dict
 
         return atoms
 
 
 def parse_block(lines: List[str], line: str) -> CIFBlock:
-    assert line.lower().startswith('data_')
-    blockname = line.split('_', 1)[1].rstrip()
+    assert line.lower().startswith("data_")
+    blockname = line.split("_", 1)[1].rstrip()
     tags = parse_items(lines, line)
     return CIFBlock(blockname, tags)
 
 
-def parse_cif(fileobj, reader='ase') -> Iterator[CIFBlock]:
-    if reader == 'ase':
+def parse_cif(fileobj, reader="ase") -> Iterator[CIFBlock]:
+    if reader == "ase":
         return parse_cif_ase(fileobj)
-    elif reader == 'pycodcif':
+    elif reader == "pycodcif":
         return parse_cif_pycodcif(fileobj)
     else:
-        raise ValueError(f'No such reader: {reader}')
+        raise ValueError(f"No such reader: {reader}")
 
 
 def parse_cif_ase(fileobj) -> Iterator[CIFBlock]:
     """Parse a CIF file using ase CIF parser."""
 
     if isinstance(fileobj, str):
-        with open(fileobj, 'rb') as fileobj:
+        with open(fileobj, "rb") as fileobj:
             data = fileobj.read()
     else:
         data = fileobj.read()
 
     if isinstance(data, bytes):
-        data = data.decode('latin1')
+        data = data.decode("latin1")
     data = format_unicode(data)
-    lines = [e for e in data.split('\n') if len(e) > 0]
-    if len(lines) > 0 and lines[0].rstrip() == '#\\#CIF_2.0':
-        warnings.warn('CIF v2.0 file format detected; `ase` CIF reader might '
-                      'incorrectly interpret some syntax constructions, use '
-                      '`pycodcif` reader instead')
-    lines = [''] + lines[::-1]    # all lines (reversed)
+    lines = [e for e in data.split("\n") if len(e) > 0]
+    if len(lines) > 0 and lines[0].rstrip() == "#\\#CIF_2.0":
+        warnings.warn(
+            "CIF v2.0 file format detected; `ase` CIF reader might "
+            "incorrectly interpret some syntax constructions, use "
+            "`pycodcif` reader instead"
+        )
+    lines = [""] + lines[::-1]  # all lines (reversed)
 
     while lines:
         line = lines.pop().strip()
-        if not line or line.startswith('#'):
+        if not line or line.startswith("#"):
             continue
 
         yield parse_block(lines, line)
 
 
 def parse_cif_pycodcif(fileobj) -> Iterator[CIFBlock]:
     """Parse a CIF file using pycodcif CIF parser."""
     if not isinstance(fileobj, str):
         fileobj = fileobj.name
 
     try:
         from pycodcif import parse
     except ImportError:
         raise ImportError(
-            'parse_cif_pycodcif requires pycodcif ' +
-            '(http://wiki.crystallography.net/cod-tools/pycodcif/)')
+            "parse_cif_pycodcif requires pycodcif "
+            + "(http://wiki.crystallography.net/cod-tools/pycodcif/)"
+        )
 
     data, _, _ = parse(fileobj)
 
     for datablock in data:
-        tags = datablock['values']
+        tags = datablock["values"]
         for tag in tags.keys():
             values = [convert_value(x) for x in tags[tag]]
             if len(values) == 1:
                 tags[tag] = values[0]
             else:
                 tags[tag] = values
-        yield CIFBlock(datablock['name'], tags)
+        yield CIFBlock(datablock["name"], tags)
 
 
-def read_cif(fileobj, index, store_tags=False, primitive_cell=False,
-             subtrans_included=True, fractional_occupancies=True,
-             reader='ase') -> Iterator[Atoms]:
+def read_cif(
+    fileobj,
+    index,
+    store_tags=False,
+    primitive_cell=False,
+    subtrans_included=True,
+    fractional_occupancies=True,
+    reader="ase",
+) -> Iterator[Atoms]:
     """Read Atoms object from CIF file. *index* specifies the data
     block number or name (if string) to return.
 
     If *index* is None or a slice object, a list of atoms objects will
     be returned. In the case of *index* is *None* or *slice(None)*,
     only blocks with valid crystal data will be included.
 
@@ -606,83 +652,90 @@
     # Find all CIF blocks with valid crystal data
     images = []
     for block in parse_cif(fileobj, reader):
         if not block.has_structure():
             continue
 
         atoms = block.get_atoms(
-            store_tags, primitive_cell,
+            store_tags,
+            primitive_cell,
             subtrans_included,
-            fractional_occupancies=fractional_occupancies)
+            fractional_occupancies=fractional_occupancies,
+        )
         images.append(atoms)
 
     for atoms in images[index]:
         yield atoms
 
 
 def format_cell(cell: Cell) -> str:
     assert cell.rank == 3
     lines = []
     for name, value in zip(CIFBlock.cell_tags, cell.cellpar()):
-        line = '{:20} {:g}\n'.format(name, value)
+        line = "{:20} {:g}\n".format(name, value)
         lines.append(line)
     assert len(lines) == 6
-    return ''.join(lines)
+    return "".join(lines)
 
 
 def format_generic_spacegroup_info() -> str:
     # We assume no symmetry whatsoever
-    return '\n'.join([
-        '_space_group_name_H-M_alt    "P 1"',
-        '_space_group_IT_number       1',
-        '',
-        'loop_',
-        '  _space_group_symop_operation_xyz',
-        "  'x, y, z'",
-        '',
-    ])
+    return "\n".join(
+        [
+            '_space_group_name_H-M_alt    "P 1"',
+            "_space_group_IT_number       1",
+            "",
+            "loop_",
+            "  _space_group_symop_operation_xyz",
+            "  'x, y, z'",
+            "",
+        ]
+    )
 
 
 class CIFLoop:
     def __init__(self):
         self.names = []
         self.formats = []
         self.arrays = []
 
     def add(self, name, array, fmt):
-        assert name.startswith('_')
+        assert name.startswith("_")
         self.names.append(name)
         self.formats.append(fmt)
         self.arrays.append(array)
         if len(self.arrays[0]) != len(self.arrays[-1]):
-            raise ValueError(f'Loop data "{name}" has {len(array)} '
-                             'elements, expected {len(self.arrays[0])}')
+            raise ValueError(
+                f'Loop data "{name}" has {len(array)} '
+                "elements, expected {len(self.arrays[0])}"
+            )
 
     def tostring(self):
         lines = []
         append = lines.append
-        append('loop_')
+        append("loop_")
         for name in self.names:
-            append(f'  {name}')
+            append(f"  {name}")
 
-        template = '  ' + '  '.join(self.formats)
+        template = "  " + "  ".join(self.formats)
 
         ncolumns = len(self.arrays)
         nrows = len(self.arrays[0]) if ncolumns > 0 else 0
         for row in range(nrows):
             arraydata = [array[row] for array in self.arrays]
             line = template.format(*arraydata)
             append(line)
-        append('')
-        return '\n'.join(lines)
+        append("")
+        return "\n".join(lines)
 
 
-@iofunction('wb')
-def write_cif(fd, images, cif_format=None,
-              wrap=True, labels=None, loop_keys=None) -> None:
+@iofunction("wb")
+def write_cif(
+    fd, images, cif_format=None, wrap=True, labels=None, loop_keys=None
+) -> None:
     """Write *images* to CIF file.
 
     wrap: bool
         Wrap atoms into unit cell.
 
     labels: list
         Use this list (shaped list[i_frame][i_atom] = string) for the
@@ -697,34 +750,41 @@
         string`. The strings are printed as they are, so take care of
         formating. Information can be re-read using the `store_tags`
         option of the cif reader.
 
     """
 
     if cif_format is not None:
-        warnings.warn('The cif_format argument is deprecated and may be '
-                      'removed in the future.  Use loop_keys to customize '
-                      'data written in loop.', FutureWarning)
+        warnings.warn(
+            "The cif_format argument is deprecated and may be "
+            "removed in the future.  Use loop_keys to customize "
+            "data written in loop.",
+            FutureWarning,
+        )
 
     if loop_keys is None:
         loop_keys = {}
 
-    if hasattr(images, 'get_positions'):
+    if hasattr(images, "get_positions"):
         images = [images]
 
-    fd = io.TextIOWrapper(fd, encoding='latin-1')
+    fd = io.TextIOWrapper(fd, encoding="latin-1")
     try:
         for i, atoms in enumerate(images):
-            blockname = f'data_image{i}\n'
+            blockname = f"data_image{i}\n"
             image_loop_keys = {key: loop_keys[key][i] for key in loop_keys}
 
-            write_cif_image(blockname, atoms, fd,
-                            wrap=wrap,
-                            labels=None if labels is None else labels[i],
-                            loop_keys=image_loop_keys)
+            write_cif_image(
+                blockname,
+                atoms,
+                fd,
+                wrap=wrap,
+                labels=None if labels is None else labels[i],
+                loop_keys=image_loop_keys,
+            )
 
     finally:
         # Using the TextIOWrapper somehow causes the file to close
         # when this function returns.
         # Detach in order to circumvent this highly illogical problem:
         fd.detach()
 
@@ -733,184 +793,219 @@
     no: Dict[str, int] = {}
     labels = []
     for symbol in symbols:
         if symbol in no:
             no[symbol] += 1
         else:
             no[symbol] = 1
-        labels.append('%s%d' % (symbol, no[symbol]))
+        labels.append("%s%d" % (symbol, no[symbol]))
     return labels
 
 
 def chemical_formula_header(atoms):
     counts = atoms.symbols.formula.count()
-    formula_sum = ' '.join(f'{sym}{count}' for sym, count
-                           in counts.items())
-    return (f'_chemical_formula_structural       {atoms.symbols}\n'
-            f'_chemical_formula_sum              "{formula_sum}"\n')
+    formula_sum = " ".join(f"{sym}{count}" for sym, count in counts.items())
+    return (
+        f"_chemical_formula_structural       {atoms.symbols}\n"
+        f'_chemical_formula_sum              "{formula_sum}"\n'
+    )
 
 
 class BadOccupancies(ValueError):
     pass
 
 
 def expand_kinds(atoms, coords, extra_data=[]):
     # try to fetch occupancies // spacegroup_kinds - occupancy mapping
     symbols = list(atoms.symbols)
     coords = list(coords)
     for data_i in range(len(extra_data)):
         extra_data[data_i] = list(extra_data[data_i])
     occupancies = [1] * len(symbols)
-    occ_info = atoms.info.get('occupancy')
-    kinds = atoms.arrays.get('spacegroup_kinds')
+    occ_info = atoms.info.get("occupancy")
+    kinds = atoms.arrays.get("spacegroup_kinds")
     if occ_info is not None and kinds is not None:
         for i, kind in enumerate(kinds):
             occ_info_kind = occ_info[kind]
             symbol = symbols[i]
-            print('ARGH', symbol)
+            print("ARGH", symbol)
             if symbol not in occ_info_kind:
-                raise BadOccupancies('Occupancies present but no occupancy '
-                                     'info for "{symbol}"')
+                raise BadOccupancies(
+                    "Occupancies present but no occupancy " 'info for "{symbol}"'
+                )
             occupancies[i] = occ_info_kind[symbol]
             # extend the positions array in case of mixed occupancy
             for sym, occ in occ_info[kind].items():
                 if sym != symbols[i]:
                     symbols.append(sym)
                     coords.append(coords[i])
                     occupancies.append(occ)
                     for data_i in range(len(extra_data)):
                         extra_data[data_i].append(extra_data[data_i][i])
     return symbols, coords, occupancies, extra_data
 
 
 def atoms_to_loop_data(atoms, wrap, labels, loop_keys):
     if all(atoms.pbc):
-        coord_type = 'fract'
+        coord_type = "fract"
         coords = atoms.get_scaled_positions(wrap).tolist()
     else:
-        coord_type = 'Cartn'
+        coord_type = "Cartn"
         coords = atoms.get_positions(wrap).tolist()
 
     extra_data = []
-    if atoms.has('initial_magmoms'):
+    if atoms.has("initial_magmoms"):
         extra_data.append(atoms.get_initial_magnetic_moments())
 
     try:
-        symbols, coords, occupancies, extra_data = expand_kinds(atoms, coords, extra_data)
+        symbols, coords, occupancies, extra_data = expand_kinds(
+            atoms, coords, extra_data
+        )
     except BadOccupancies as err:
         warnings.warn(str(err))
         occupancies = [1] * len(atoms)
         symbols = list(atoms.symbols)
 
     if labels is None:
         labels = autolabel(symbols)
 
-    coord_headers = [f'_atom_site_{coord_type}_{axisname}'
-                     for axisname in 'xyz']
+    coord_headers = [f"_atom_site_{coord_type}_{axisname}" for axisname in "xyz"]
 
     loopdata = {}
-    loopdata['_atom_site_label'] = (labels, '{:<8s}')
-    loopdata['_atom_site_occupancy'] = (occupancies, '{:6.4f}')
+    loopdata["_atom_site_label"] = (labels, "{:<8s}")
+    loopdata["_atom_site_occupancy"] = (occupancies, "{:6.4f}")
 
     _coords = np.array(coords)
     for i, key in enumerate(coord_headers):
-        loopdata[key] = (_coords[:, i], '{:7.5f}')
+        loopdata[key] = (_coords[:, i], "{:7.5f}")
 
-    loopdata['_atom_site_type_symbol'] = (symbols, '{:<2s}')
-    loopdata['_atom_site_symmetry_multiplicity'] = (
-        [1.0] * len(symbols), '{}')
+    loopdata["_atom_site_type_symbol"] = (symbols, "{:<2s}")
+    loopdata["_atom_site_symmetry_multiplicity"] = ([1.0] * len(symbols), "{}")
 
     for key in loop_keys:
         # Should expand the loop_keys like we expand the occupancy stuff.
         # Otherwise user will never figure out how to do this.
         values = [loop_keys[key][i] for i in range(len(symbols))]
-        loopdata['_' + key] = (values, '{}')
+        loopdata["_" + key] = (values, "{}")
 
     output_data_headers = [(loopdata, coord_headers)]
 
     if len(extra_data) > 0:
         magmoms = np.asarray(extra_data[0])
 
-        mag_headers = ['_atom_site_moment.label']
-        mag_loopdata = {'_atom_site_moment.label': loopdata['_atom_site_label']}
-        smagmoms=atoms.cell.scaled_positions(magmoms)
-
-        if len(magmoms.shape) == 1 or (len(magmoms.shape) == 2 and magmoms.shape[1] == 1):
+        mag_headers = ["_atom_site_moment.label"]
+        mag_loopdata = {"_atom_site_moment.label": loopdata["_atom_site_label"]}
+        smagmoms = atoms.cell.scaled_positions(magmoms)
+
+        if len(magmoms.shape) == 1 or (
+            len(magmoms.shape) == 2 and magmoms.shape[1] == 1
+        ):
             # scalar, orientation meaningless, do || crystal z
-            mag_headers.extend([f'_atom_site_moment.crystalaxis_{axisname}' for axisname in 'xyz'])
-            mag_loopdata['_atom_site_moment.crystalaxis_x'] = (np.array([0.0] * len(magmoms)), '{:7.3f}')
-            mag_loopdata['_atom_site_moment.crystalaxis_y'] = (np.array([0.0] * len(magmoms)), '{:7.3f}')
-            mag_loopdata['_atom_site_moment.crystalaxis_z'] = (magmoms, '{:7.3f}')
-        elif (len(magmoms.shape) == 2 and magmoms.shape[1] == 3):
-            #mag_headers.extend([f'_atom_site_moment.Cartn_{axisname}' for axisname in 'xyz'])
-            #mag_loopdata['_atom_site_moment.Cartn_x'] = (magmoms[:,0], '{:7.3f}')
-            #mag_loopdata['_atom_site_moment.Cartn_y'] = (magmoms[:,1], '{:7.3f}')
-            #mag_loopdata['_atom_site_moment.Cartn_z'] = (magmoms[:,2], '{:7.3f}')
-            mag_headers.extend([f'_atom_site_moment.crystalaxis_{axisname}' for axisname in 'xyz'])
-            mag_loopdata['_atom_site_moment.crystalaxis_x'] = (smagmoms[:,0], '{:7.3f}')
-            mag_loopdata['_atom_site_moment.crystalaxis_y'] = (smagmoms[:,1], '{:7.3f}')
-            mag_loopdata['_atom_site_moment.crystalaxis_z'] = (smagmoms[:,2], '{:7.3f}')
-
-        else:
-            raise IndexError('Cannot handle magmoms shape {}, neither scalar nor 3-vector'.
-                             format(magmoms.shape))
+            mag_headers.extend(
+                [f"_atom_site_moment.crystalaxis_{axisname}" for axisname in "xyz"]
+            )
+            mag_loopdata["_atom_site_moment.crystalaxis_x"] = (
+                np.array([0.0] * len(magmoms)),
+                "{:7.3f}",
+            )
+            mag_loopdata["_atom_site_moment.crystalaxis_y"] = (
+                np.array([0.0] * len(magmoms)),
+                "{:7.3f}",
+            )
+            mag_loopdata["_atom_site_moment.crystalaxis_z"] = (magmoms, "{:7.3f}")
+        elif len(magmoms.shape) == 2 and magmoms.shape[1] == 3:
+            # mag_headers.extend([f'_atom_site_moment.Cartn_{axisname}' for axisname in 'xyz'])
+            # mag_loopdata['_atom_site_moment.Cartn_x'] = (magmoms[:,0], '{:7.3f}')
+            # mag_loopdata['_atom_site_moment.Cartn_y'] = (magmoms[:,1], '{:7.3f}')
+            # mag_loopdata['_atom_site_moment.Cartn_z'] = (magmoms[:,2], '{:7.3f}')
+            mag_headers.extend(
+                [f"_atom_site_moment.crystalaxis_{axisname}" for axisname in "xyz"]
+            )
+            mag_loopdata["_atom_site_moment.crystalaxis_x"] = (
+                smagmoms[:, 0],
+                "{:7.3f}",
+            )
+            mag_loopdata["_atom_site_moment.crystalaxis_y"] = (
+                smagmoms[:, 1],
+                "{:7.3f}",
+            )
+            mag_loopdata["_atom_site_moment.crystalaxis_z"] = (
+                smagmoms[:, 2],
+                "{:7.3f}",
+            )
+
+        else:
+            raise IndexError(
+                "Cannot handle magmoms shape {}, neither scalar nor 3-vector".format(
+                    magmoms.shape
+                )
+            )
         output_data_headers.append((mag_loopdata, mag_headers))
 
     return output_data_headers
 
 
-def write_cif_image(blockname, atoms, fd, *, wrap,
-                    labels, loop_keys):
+def write_cif_image(blockname, atoms, fd, *, wrap, labels, loop_keys):
     fd.write(blockname)
     fd.write(chemical_formula_header(atoms))
 
     rank = atoms.cell.rank
     if rank == 3:
         fd.write(format_cell(atoms.cell))
-        fd.write('\n')
+        fd.write("\n")
         fd.write(format_generic_spacegroup_info())
-        fd.write('\n')
+        fd.write("\n")
     elif rank != 0:
-        raise ValueError('CIF format can only represent systems with '
-                         f'0 or 3 lattice vectors.  Got {rank}.')
+        raise ValueError(
+            "CIF format can only represent systems with "
+            f"0 or 3 lattice vectors.  Got {rank}."
+        )
 
     all_data = atoms_to_loop_data(atoms, wrap, labels, loop_keys)
 
     loopdata, coord_headers = all_data[0]
 
     headers = [
-        '_atom_site_type_symbol',
-        '_atom_site_label',
-        '_atom_site_symmetry_multiplicity',
+        "_atom_site_type_symbol",
+        "_atom_site_label",
+        "_atom_site_symmetry_multiplicity",
         *coord_headers,
-        '_atom_site_occupancy',
+        "_atom_site_occupancy",
     ]
 
-    headers += ['_' + key for key in loop_keys]
+    headers += ["_" + key for key in loop_keys]
 
     loop = CIFLoop()
     for header in headers:
         array, fmt = loopdata[header]
         loop.add(header, array, fmt)
 
     fd.write(loop.tostring())
 
     # write other loops
     for loopdata, headers in all_data[1:]:
-
-        fd.write('\n')
+        fd.write("\n")
         loop = CIFLoop()
         for header in headers:
             array, fmt = loopdata[header]
             loop.add(header, array, fmt)
 
         fd.write(loop.tostring())
 
-@iofunction('wb')
-def write_mcif(fd, images, cif_format=None,
-              wrap=True, labels=None, loop_keys=None, vectors=None, factor=1.0) -> None:
-    catoms=copy.deepcopy(images)
-    catoms.set_initial_magnetic_moments(None)
-    catoms.set_initial_magnetic_moments(np.array(vectors)*factor)
-    write_cif(fd, catoms, cif_format=cif_format,
-              wrap=wrap, labels=labels, loop_keys=loop_keys)
 
+@iofunction("wb")
+def write_mcif(
+    fd,
+    images,
+    cif_format=None,
+    wrap=True,
+    labels=None,
+    loop_keys=None,
+    vectors=None,
+    factor=1.0,
+) -> None:
+    catoms = copy.deepcopy(images)
+    catoms.set_initial_magnetic_moments(None)
+    catoms.set_initial_magnetic_moments(np.array(vectors) * factor)
+    write_cif(
+        fd, catoms, cif_format=cif_format, wrap=wrap, labels=labels, loop_keys=loop_keys
+    )
```

### Comparing `lawaf-0.1.0/lawaf/plot/plot.py` & `lawaf-0.2.1/lawaf/plot/plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,99 @@
 import numpy as np
 import copy
 from ase.dft.kpoints import bandpath
+from lawaf.utils.kpoints import autopath
 import matplotlib.pyplot as plt
 
+
 def fix_evals_LOTO(evals, xs, kpts, N=4):
     fixed_evals = copy.deepcopy(evals)
     for i, (x, kv) in enumerate(zip(xs, kpts)):
         if np.isclose(kv, np.array([0.0, 0.0, 0.0]), rtol=1e-5, atol=1e-3).all():
-            if i==0:
-                fixed_evals[i] = (N*evals[i+1] - evals[i+2])/(N-1)
-            #elif i==len(xs)-1:
+            if i == 0:
+                fixed_evals[i] = (N * evals[i + 1] - evals[i + 2]) / (N - 1)
+            # elif i==len(xs)-1:
             #    fixed_evals[i] = (10*evals[i-1] - evals[i-2])/9
             else:
-                fixed_evals[i] = (N*evals[i-1] - evals[i-2])/(N-1)
-                #fixed_evals[i] = evals[i-1]
+                fixed_evals[i] = (N * evals[i - 1] - evals[i - 2]) / (N - 1)
+                # fixed_evals[i] = evals[i-1]
     return fixed_evals
 
 
-def plot_band(model,
-              kvectors=np.array([[0, 0, 0], [0.5, 0, 0], [0.5, 0.5, 0],
-                                 [0, 0, 0], [.5, .5, .5]]),
-              knames=['$\Gamma$', 'X', 'M', '$\Gamma$', 'R'],
-              supercell_matrix=None,
-              npoints=100,
-              efermi=None,
-              erange=None,
-              color='blue',
-              alpha=0.8,
-              marker='',
-              label=None,
-              cell=np.eye(3),
-              evals_to_freq=False,
-              unit_factor=1,
-              ylabel='Energy (eV)',
-              fix_LOTO=False,
-              ax=None):
+def plot_band(
+    model,
+    # kvectors=np.array(
+    #    [[0, 0, 0], [0.5, 0, 0], [0.5, 0.5, 0], [0, 0, 0], [0.5, 0.5, 0.5]]
+    # ),
+    # knames=["$\Gamma$", "X", "M", "$\Gamma$", "R"],
+    kvectors=None,
+    knames=None,
+    supercell_matrix=None,
+    npoints=100,
+    efermi=None,
+    erange=None,
+    color="blue",
+    alpha=0.8,
+    marker="",
+    label=None,
+    cell=np.eye(3),
+    evals_to_freq=False,
+    unit_factor=1,
+    ylabel="Energy (eV)",
+    fix_LOTO=False,
+    ax=None,
+):
     if ax is None:
         _fig, ax = plt.subplots()
 
-    if supercell_matrix is None:
-        supercell_matrix = np.eye(3)
-    kvectors = [np.dot(k, supercell_matrix) for k in kvectors]
-    if 'cell' not in model.__dict__:
-        band = bandpath(kvectors, cell @ supercell_matrix, npoints)
-    else:
-        band = bandpath(kvectors, cell @ supercell_matrix, npoints)
-    kpts = band.kpts
-    x, X, _labels = band.get_linear_kpoint_axis()
+    # if supercell_matrix is None:
+    #    supercell_matrix = np.eye(3)
+    # kvectors = [np.dot(k, supercell_matrix) for k in kvectors]
+    if cell is None:
+        if "atoms" in model.__dict__:
+            cell = model.atoms.cell
+        elif "cell" in model.__dict__:
+            cell = model.cell
+
+    knames, kpts, xs, Xs = autopath(
+        knames=knames,
+        kvectors=kvectors,
+        npoints=npoints,
+        supercell_matrix=supercell_matrix,
+        cell=cell,
+    )
+    kpts = np.vstack(kpts)
+    xs = np.hstack(xs)
     _evalues, _evecs = model.solve_all(kpts=kpts)[:2]
 
     if fix_LOTO:
-        evalues = fix_evals_LOTO(_evalues, x, kpts)
+        evalues = fix_evals_LOTO(_evalues, xs, kpts)
     else:
         evalues = copy.deepcopy(_evalues)
     if evals_to_freq:
-        #evalues = np.where(evalues < 0, -np.sqrt(-evalues), np.sqrt(evalues))
+        # evalues = np.where(evalues < 0, -np.sqrt(-evalues), np.sqrt(evalues))
         evalues = np.sign(evalues) * (np.sqrt(np.abs(evalues)))
     evalues *= unit_factor
     for i in range(evalues.shape[1]):
         if i == 0:
-            ax.plot(x,
-                    evalues[:, i],
-                    color=color,
-                    alpha=alpha,
-                    marker=marker,
-                    label=label)
+            ax.plot(
+                xs, evalues[:, i], color=color, alpha=alpha, marker=marker, label=label
+            )
         else:
-            ax.plot(x, evalues[:, i], color=color, alpha=alpha, marker=marker)
+            ax.plot(xs, evalues[:, i], color=color, alpha=alpha, marker=marker)
 
     if efermi is not None:
-        ax.axhline(efermi, linestyle='--', color='gray')
+        ax.axhline(efermi, linestyle="--", color="gray")
     else:
         try:
-            plt.axhline(model.get_fermi_level(), linestyle='--', color='gray')
+            plt.axhline(model.get_fermi_level(), linestyle="--", color="gray")
         except AttributeError:
             pass
     ax.set_ylabel(ylabel)
-    ax.set_xlim(x[0], x[-1])
-    ax.set_xticks(X)
+    ax.set_xlim(xs[0], xs[-1])
+    ax.set_xticks(Xs)
     ax.set_xticklabels(knames)
     if erange is not None:
         ax.set_ylim(erange)
-    for x in X:
-        ax.axvline(x, linewidth=0.6, color='gray')
+    for X in Xs:
+        ax.axvline(X, linewidth=0.6, color="gray")
     return ax
```

### Comparing `lawaf-0.1.0/lawaf/utils/lwf_to_atoms.py` & `lawaf-0.2.1/lawaf/utils/lwf_to_atoms.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,50 +13,45 @@
 def lwf_to_atoms(mylwf: LWF, scmaker, amplist, thr=0.01):
     patoms = mylwf.atoms
     scatoms = scmaker.sc_atoms(patoms)
     positions = scatoms.get_positions()
     nR, natom3, nlwf = mylwf.wannR.shape
     scnatom = len(scatoms)
     displacement = np.zeros_like(positions.flatten())
-    #stds = np.zeros_like(positions.flatten())
-    for (R, iwann, ampwann) in amplist:
+    # stds = np.zeros_like(positions.flatten())
+    for R, iwann, ampwann in amplist:
         iwann = int(iwann) - 1
         for Rwann, iRwann in mylwf.Rdict.items():
             for j in range(natom3):
                 clwf = mylwf.wannR[iRwann, j, iwann]
                 if abs(clwf.real) > thr:
                     sc_j, sc_R = scmaker.sc_jR_to_scjR(j, Rwann, R, natom3)
                     amp = ampwann * clwf
                     displacement[sc_j] += amp.real
-                    #stds[sc_j] += std.real
+                    # stds[sc_j] += std.real
     sc_pos = positions + displacement.reshape((scnatom, 3))
     scatoms.set_positions(sc_pos)
     return scatoms, displacement
 
 
-def lwf_to_atoms_batch(mylwf: LWF,
-                       scmaker,
-                       fname,
-                       itimes,
-                       out_prefix,
-                       thr=0.01):
+def lwf_to_atoms_batch(mylwf: LWF, scmaker, fname, itimes, out_prefix, thr=0.01):
     amplist = load_amplist(fname)
     patoms = mylwf.atoms
     scatoms = scmaker.sc_atoms(patoms)
     scatoms.set_pbc(True)
-    write('scatoms.cif', scatoms)
-    write('scatoms.vasp', scatoms)
+    write("scatoms.cif", scatoms)
+    write("scatoms.vasp", scatoms)
     positions = scatoms.get_positions()
     nR, natom3, nlwf = mylwf.wannR.shape
     scnatom = len(scatoms)
     npos = np.product(positions.shape)
     ntime = len(itimes)
     print(npos, ntime)
     displacement = np.zeros((ntime, npos), dtype=float)
-    #stds = np.zeros_like(positions.flatten())
+    # stds = np.zeros_like(positions.flatten())
 
     for Rwann, iRwann in mylwf.Rdict.items():
         for j in range(natom3):
             for R, iwann, ampwann in zip(*amplist):
                 iwann = int(iwann) - 1
                 clwf = mylwf.wannR[iRwann, j, iwann]
                 if abs(clwf.real) > thr:
@@ -66,43 +61,43 @@
         p = copy.deepcopy(positions)
         print(displacement[it])
         disp = displacement[it, :].reshape((scnatom, 3))
         sc_pos = p + disp
         d = copy.deepcopy(scatoms)
         d.set_positions(sc_pos)
         d.set_pbc(True)
-        write(f'cifs/{out_prefix}_{itime:03d}.cif', d)
-        np.save(f'cifs/{out_prefix}_{itime:03d}_disp.npy', disp)
-    return scatoms  #, stds
+        write(f"cifs/{out_prefix}_{itime:03d}.cif", d)
+        np.save(f"cifs/{out_prefix}_{itime:03d}_disp.npy", disp)
+    return scatoms  # , stds
 
 
 def load_amplist(fname, itime=None):
-    root = Dataset(fname, 'r')
-    nlwf = root.dimensions['nlwf'].size
-    Rlist = root.variables['lwf_rvec'][:].filled(np.nan)
-    ilwf = root.variables['ilwf_prim'][:]
-    amps = root.variables['lwf'][:][:, :] * Bohr  # itime, iwann
+    root = Dataset(fname, "r")
+    nlwf = root.dimensions["nlwf"].size
+    Rlist = root.variables["lwf_rvec"][:].filled(np.nan)
+    ilwf = root.variables["ilwf_prim"][:]
+    amps = root.variables["lwf"][:][:, :] * Bohr  # itime, iwann
     root.close()
     return Rlist, ilwf, amps[itime, :]
 
 
 def load_map(fname):
-    root = Dataset(fname, 'r')
+    root = Dataset(fname, "r")
     ndisp = root.dimensions["natom3"].size
     nlwf = root.dimensions["nlwf"].size
     idisp = root.variables["lwf_latt_map_id_displacement"][:]
     ilwf = root.variables["lwf_latt_map_id_lwf"][:]
-    vals = root.variables['lwf_latt_map_values'][:]
+    vals = root.variables["lwf_latt_map_values"][:]
     root.close()
     mat_map = coo_matrix((vals, (idisp - 1, ilwf - 1)), shape=(ndisp, nlwf))
     return mat_map
 
 
 def load_ref_atoms(fname):
-    root = Dataset(fname, 'r')
+    root = Dataset(fname, "r")
     ndisp = root.dimensions["natom3"].size
     ref_cell = root.variables["ref_cell"][:] * Bohr
     ref_xcart = root.variables["ref_xcart"][:] * Bohr
     zion = root.variables["zion"][:]
     root.close()
     return ref_cell, ref_xcart, zion
 
@@ -111,86 +106,88 @@
     ref_cell, ref_xcart, zion = load_ref_atoms(fname)
     dmap = load_map(fname)
     amp = load_amplist(fname, itime)[2]
     disp = dmap @ amp
     natom = len(disp) // 3
     xcart = ref_xcart + disp.reshape(natom, 3)
     atoms = Atoms(numbers=zion, positions=xcart, cell=ref_cell)
-    write_atoms_to_netcdf('sample.nc',atoms)
+    write_atoms_to_netcdf("sample.nc", atoms)
     return atoms
 
 
 def write_atoms_to_netcdf(fname, atoms: Atoms, nd=5):
-    root = Dataset(fname, 'w')
+    root = Dataset(fname, "w")
     natom = len(atoms)
-    natom_id = root.createDimension(dimname='natom', size=natom)
-    three_id = root.createDimension(dimname='three', size=3)
+    natom_id = root.createDimension(dimname="natom", size=natom)
+    three_id = root.createDimension(dimname="three", size=3)
 
-    cell_id = root.createVariable("cell",
-                                  float, ('three', 'three'),
-                                  zlib=True,
-                                  least_significant_digit=nd)
-    numbers_id = root.createVariable("numbers", int, ('natom', ))
-    xcart_id = root.createVariable("xcart",
-                                   float, ('natom', 'three'),
-                                   zlib=True,
-                                   least_significant_digit=nd)
-
-    root.variables['cell'][:] = atoms.get_cell()
-    root.variables['numbers'][:] = atoms.get_atomic_numbers()
-    root.variables['xcart'][:] = atoms.get_positions()
+    cell_id = root.createVariable(
+        "cell", float, ("three", "three"), zlib=True, least_significant_digit=nd
+    )
+    numbers_id = root.createVariable("numbers", int, ("natom",))
+    xcart_id = root.createVariable(
+        "xcart", float, ("natom", "three"), zlib=True, least_significant_digit=nd
+    )
+
+    root.variables["cell"][:] = atoms.get_cell()
+    root.variables["numbers"][:] = atoms.get_atomic_numbers()
+    root.variables["xcart"][:] = atoms.get_positions()
     root.close()
 
 
 def read_atoms_from_netcdf(fname):
-    root = Dataset(fname, 'r')
-    cell = root.variables['cell'][:]
-    numbers = root.variables['numbers'][:]
-    positions = root.variables['xcart'][:]
+    root = Dataset(fname, "r")
+    cell = root.variables["cell"][:]
+    numbers = root.variables["numbers"][:]
+    positions = root.variables["xcart"][:]
     return Atoms(numbers=numbers, positions=positions, cell=cell)
 
 
-atoms=get_atoms(fname="./lwf.out_T0007_lwfhist.nc", itime=30)
+atoms = get_atoms(fname="./lwf.out_T0007_lwfhist.nc", itime=30)
 vesta_view(atoms)
 
 
-def get_atoms(fname='./lwf.out_lwfhist.nc',
-              scmaker=SupercellMaker(np.diag([16, 16, 16])),
-              out_prefix=None,
-              itime=None):
+def get_atoms(
+    fname="./lwf.out_lwfhist.nc",
+    scmaker=SupercellMaker(np.diag([16, 16, 16])),
+    out_prefix=None,
+    itime=None,
+):
     print(f"Getting atoms from file {fname}, itime:{itime}")
     amplist = load_amplist(fname, itime=itime)
-    mylwf = LWF.load_nc(fname='./VO2_othermodes.nc')
+    mylwf = LWF.load_nc(fname="./VO2_othermodes.nc")
     atoms = lwf_to_atoms(
         mylwf,
         scmaker=scmaker,
         amplist=amplist,
     )
-    #amplist=[[(0, 0, 0), 0, 1],
+    # amplist=[[(0, 0, 0), 0, 1],
     #         [(0, 0, 0), 1, 1]])
     atoms.set_pbc(True)
     print(f"Writting to file: {out_prefix}_{itime:03d}.cif")
-    write(f'{out_prefix}_{itime:03d}.cif', atoms)
+    write(f"{out_prefix}_{itime:03d}.cif", atoms)
     return (fname, itime)
-    #np.savetxt(out_prefix + '.std', stds)
+    # np.savetxt(out_prefix + '.std', stds)
 
 
 def main():
     import concurrent.futures
+
     scmaker = SupercellMaker(np.diag([32, 32, 32]))
     itimes = list(range(1, 20, 1))
-    mylwf = LWF.load_nc(fname='./VO2_othermodes.nc')
+    mylwf = LWF.load_nc(fname="./VO2_othermodes.nc")
 
     with concurrent.futures.ProcessPoolExecutor(max_workers=13) as executor:
         for i in range(1, 21, 1):
             T = (i - 1) * 30
             fname = f"lwf.out_T{i:04d}_lwfhist.nc"
-            #lwf_to_atoms_batch(mylwf, scmaker, fname, itimes, out_prefix= f'T{T}K', thr=0.01)
-            futures = executor.submit(lwf_to_atoms_batch, mylwf, scmaker,
-                                      fname, itimes, f'n{i}', 0.03)
+            # lwf_to_atoms_batch(mylwf, scmaker, fname, itimes, out_prefix= f'T{T}K', thr=0.01)
+            futures = executor.submit(
+                lwf_to_atoms_batch, mylwf, scmaker, fname, itimes, f"n{i}", 0.03
+            )
         for x in concurrent.futures.as_completed(futures):
             print(x, result())
 
 
-#load_map("lwf.out_T0061_lwfhist.nc")
+# load_map("lwf.out_T0061_lwfhist.nc")
 
-#main()
+# main()
```

### Comparing `lawaf-0.1.0/lawaf/utils/nckit.py` & `lawaf-0.2.1/lawaf/utils/nckit.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,153 +19,165 @@
     value: the value to be added.
 
     Example:
       add_variable('out2.nc', 'ref_spin_orientation', 'f8', ('nspin', 'three'),
                  np.array([[0, 0, 1.0]], dtype='float'))
 
     """
-    with nc.Dataset(fname, 'r+', data_model='NETCDF3_CLASSIC') as myfile:
+    with nc.Dataset(fname, "r+", data_model="NETCDF3_CLASSIC") as myfile:
         myfile.createVariable(varname, datatype, dimension_strings)
         myfile.variables[varname][:] = value
 
 
 def change_varname(fname, outfname, change_dict={}):
     """
     Rename variable names.
     fname: input filename
     outfname: output filename
-    change_dict: key: the name to be changed, 
+    change_dict: key: the name to be changed,
                  value: the name to be changed into
                  multi vars can be changed.
     """
     dimensions = {}
-    with nc.Dataset(outfname, 'w', data_model='NETCDF3_CLASSIC') as dst:
+    with nc.Dataset(outfname, "w", data_model="NETCDF3_CLASSIC") as dst:
         with nc.Dataset(fname) as src:
             # copy attributes
             for name in src.ncattrs():
                 if name in change_dict:
                     newname = change_dict[name]
                 else:
                     newname = name
                 dst.setncattr(newname, src.getncattr(name))
                 # copy dimensions
             for name, dimension in src.dimensions.items():
                 if name not in dimensions:
                     dst.createDimension(
-                        name, (len(dimension)
-                               if not dimension.isunlimited() else 0))
+                        name, (len(dimension) if not dimension.isunlimited() else 0)
+                    )
                     dimensions[name] = dimension
                 else:
                     pass
             # copy all file data for variables that are included in the toinclude list
             for name, variable in src.variables.items():
                 # copy variables
                 if name in change_dict:
                     newname = change_dict[name]
                 else:
                     newname = name
-                x = dst.createVariable(newname, variable.datatype,
-                                       variable.dimensions)
+                x = dst.createVariable(newname, variable.datatype, variable.dimensions)
                 dst.variables[newname][:] = src.variables[name][:]
                 # copy atrribute of varibles
                 for attr in variable.ncattrs():
                     content = src.variables[name].getncattr(attr)
                     setattr(x, attr, content)
 
 
 def merge(fnames, outfname):
     """
     Merge multi netcdf files into one.
     fnames: list of nc files.
     outfname: the output filename
-    NOTE: right now, there is no consistency check. And if there are duplicate variables, 
+    NOTE: right now, there is no consistency check. And if there are duplicate variables,
           the one comes latter in the list of files will over-write previos ones.
-    TODO: add check. 
+    TODO: add check.
     """
     dimensions = {}
     var_names = set()
     attrs = set()
-    with nc.Dataset(outfname, 'w', data_model='NETCDF3_CLASSIC') as dst:
+    with nc.Dataset(outfname, "w", data_model="NETCDF3_CLASSIC") as dst:
         for fname in fnames:
             with nc.Dataset(fname) as src:
                 # copy attributes
                 for name in src.ncattrs():
                     if name not in attrs:
                         dst.setncattr(name, src.getncattr(name))
                         attrs.add(name)
                     # copy dimensions
                 for name, dimension in src.dimensions.items():
                     if name not in dimensions:
                         dst.createDimension(
-                            name, (len(dimension)
-                                   if not dimension.isunlimited() else 0))
+                            name, (len(dimension) if not dimension.isunlimited() else 0)
+                        )
                         dimensions[name] = dimension
                     else:
                         pass
                 # copy all file data for variables that are included in the toinclude list
                 for name, variable in src.variables.items():
                     # copy variables
                     if name not in var_names:
-                        x = dst.createVariable(name, variable.datatype,
-                                               variable.dimensions)
+                        x = dst.createVariable(
+                            name, variable.datatype, variable.dimensions
+                        )
                         dst.variables[name][:] = src.variables[name][:]
                         for attr in variable.ncattrs():
                             content = src.variables[name].getncattr(attr)
                             setattr(x, attr, content)
                         var_names.add(name)
                     else:
                         print(
-                            "Warning: Duplicate variables %s found, it will be neglected! " % name)
+                            "Warning: Duplicate variables %s found, it will be neglected! "
+                            % name
+                        )
                     # copy atrribute of varibles
 
 
 def flip_one_spin(fname, ispin):
     """
     flip a spin of the last step in the spinhist.nc file .
     """
-    with nc.Dataset(fname, 'r+') as dtset:
-        print("Initial spin", dtset['S'][-1, ispin, :])
-        dtset['S'][-1, ispin, :] = -dtset['S'][:][-1, ispin, :]
-        print("After flip:", dtset['S'][:][-1, ispin, :])
+    with nc.Dataset(fname, "r+") as dtset:
+        print("Initial spin", dtset["S"][-1, ispin, :])
+        dtset["S"][-1, ispin, :] = -dtset["S"][:][-1, ispin, :]
+        print("After flip:", dtset["S"][:][-1, ispin, :])
 
 
 # ============================
 # Examples and tests
 
 
 def test_change_varname():
     """
     Examample: change the varname xcart to ref_xcart in exchange.nc. Output file: exchang2.nc
 
     """
-    change_varname('pot.nc', 'pot2.nc', change_dict={'xcart': 'ref_xcart',
-                                                     'ref_spin_qpoint': 'spin_ref_qpoint',
-                                                     'ref_spin_rotate_axis': 'spin_ref_rotate_axis',
-                                                     })
+    change_varname(
+        "pot.nc",
+        "pot2.nc",
+        change_dict={
+            "xcart": "ref_xcart",
+            "ref_spin_qpoint": "spin_ref_qpoint",
+            "ref_spin_rotate_axis": "spin_ref_rotate_axis",
+        },
+    )
 
 
 def test_add_variable():
     print("Adding variable ref_spin_orientation to out2.nc")
-    add_variable('out2.nc', 'ref_spin_orientation', 'f8', ('nspin', 'three'),
-                 np.array([[0, 0, 1.0]], dtype='float'))
+    add_variable(
+        "out2.nc",
+        "ref_spin_orientation",
+        "f8",
+        ("nspin", "three"),
+        np.array([[0, 0, 1.0]], dtype="float"),
+    )
 
 
 def test_merge():
     """
     merge ifc.nc, Oiju... into out.nc
     """
-    #merge(["ifc.nc", "Oiju_matij.nc", "exchange2.nc", "Tijuv.nc"], "out.nc")
-    merge(["results/onebody.nc", "results/Downfolded_hr.nc"], 'results/LAO_wann.nc')
+    # merge(["ifc.nc", "Oiju_matij.nc", "exchange2.nc", "Tijuv.nc"], "out.nc")
+    merge(["results/onebody.nc", "results/Downfolded_hr.nc"], "results/LAO_wann.nc")
 
 
 def test_flip_one_spin():
     """
     Flip the first spin of the last step in the hist file
     """
-    flip_one_spin(fname='./test.out_spinhist.nc', ispin=0)
+    flip_one_spin(fname="./test.out_spinhist.nc", ispin=0)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     test_merge()
     # test_add_variable()
     # test_change_varname()
     # test_flip_one_spin()
```

### Comparing `lawaf-0.1.0/lawaf/utils/plotphon.py` & `lawaf-0.2.1/lawaf/utils/plotphon.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 #!/usr/bin/env python3
 import os
 import matplotlib.pyplot as plt
 from pyDFTutils.ase_utils.kpoints import kpath
 from phonopy import load
 
 
-def plot_phonon(path='./',color='blue', unit="cm^-1"):
-    #phonon=load(force_sets_filename="FORCE_SETS", born_filename="./BORN", unitcell_filename="POSCAR-unitcell",supercell_matrix=np.eye(3)*3 )
-    phonon=load(phonopy_yaml=os.path.join(path,'phonopy_params.yaml'))
-    cell=phonon._primitive.cell
-    kpts,xs,xs_special,names=kpath(cell,npoints=300, path='GXMGRX')
+def plot_phonon(path="./", color="blue", unit="cm^-1"):
+    # phonon=load(force_sets_filename="FORCE_SETS", born_filename="./BORN", unitcell_filename="POSCAR-unitcell",supercell_matrix=np.eye(3)*3 )
+    phonon = load(phonopy_yaml=os.path.join(path, "phonopy_params.yaml"))
+    cell = phonon._primitive.cell
+    kpts, xs, xs_special, names = kpath(cell, npoints=300, path="GXMGRX")
     phonon.symmetrize_force_constants()
-    #phonon.symmetrize_force_constants_by_space_group()
+    # phonon.symmetrize_force_constants_by_space_group()
     phonon.set_qpoints_phonon(kpts, is_eigenvectors=True)
-    #phonon.symmetrize_force_constants()
+    # phonon.symmetrize_force_constants()
     freqs, eigvecs = phonon.get_qpoints_phonon()
-    #print(freqs)
-    #print(eigvecs.shape)
-    #print(eigvecs[9,-1,:])
-    #weight=np.zeros_like(freqs)
-    #for ki in range(freqs.shape[0]):
+    # print(freqs)
+    # print(eigvecs.shape)
+    # print(eigvecs[9,-1,:])
+    # weight=np.zeros_like(freqs)
+    # for ki in range(freqs.shape[0]):
     #    for i in range(freqs.shape[1]):
     #        weight[ki,i]=np.linalg.norm(eigvecs[ki,i,-3:])
     for i in range(freqs.shape[1]):
-        plt.plot(xs, freqs[:, i]*33.356,color=color,linewidth=1.3,alpha=0.8)
-        #plt.plot(xs, freqs[:, i]*33.356/8.065,color=color,linewidth=1.3,alpha=0.8)
-        #plt.scatter(x, freqs[:, i]*33.356,s=weight[:,i]*10,color='blue',alpha=0.3)
-    plt.xlim(xs[0],xs[-1])
+        plt.plot(xs, freqs[:, i] * 33.356, color=color, linewidth=1.3, alpha=0.8)
+        # plt.plot(xs, freqs[:, i]*33.356/8.065,color=color,linewidth=1.3,alpha=0.8)
+        # plt.scatter(x, freqs[:, i]*33.356,s=weight[:,i]*10,color='blue',alpha=0.3)
+    plt.xlim(xs[0], xs[-1])
     for x in xs_special:
-        plt.axvline(x,color='gray',alpha=0.7)
+        plt.axvline(x, color="gray", alpha=0.7)
     plt.xticks(xs_special, names)
-    plt.ylabel('Frequency (cm$^{-1}$)')
+    plt.ylabel("Frequency (cm$^{-1}$)")
     plt.show()
 
-if __name__=='__main__':
+
+if __name__ == "__main__":
     plot_phonon()
```

### Comparing `lawaf-0.1.0/lawaf/utils/structurebuilder.py` & `lawaf-0.2.1/lawaf/utils/structurebuilder.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,44 +8,51 @@
 from ase.atoms import Atoms
 from ase.io import write, read
 from spglib import spglib
 from pyDFTutils.ase_utils.geometry import force_near_0
 from dataclasses import dataclass
 from typing import Tuple, List
 
+
 @dataclass
-class PhonMode():
+class PhonMode:
     kpt: Tuple[float]
-    ind : int
-
+    ind: int
 
 
-
-class PhonStructureGenerator():
+class PhonStructureGenerator:
     def __init__(self, phonon, supercell_matrix):
-        self.phonon=copy.deepcopy(myphonon)
+        self.phonon = copy.deepcopy(myphonon)
 
     def get_distorted_structure(self, phonon_modes):
-
-
-
+        pass
 
 
 def gen(mod, amp):
-    myphonon=load(phonopy_yaml='../phonopy_params.yaml')
+    myphonon = load(phonopy_yaml="../phonopy_params.yaml")
     for i in [0]:
-        phonon=copy.copy(myphonon)
-        phonon.set_modulations(dimension=np.array([[1,0,-1],[0,1,0],[0,0,2]]).T, phonon_modes=[[(.5, 0.0, .5), i,amp, 0]])
+        phonon = copy.copy(myphonon)
+        phonon.set_modulations(
+            dimension=np.array([[1, 0, -1], [0, 1, 0], [0, 0, 2]]).T,
+            phonon_modes=[[(0.5, 0.0, 0.5), i, amp, 0]],
+        )
         modes, sc = phonon.get_modulations_and_supercell()
-        sc=Atoms(sc.symbols, cell=sc.cell,scaled_positions=sc.get_scaled_positions(), pbc=True)
-        datoms=copy.deepcopy(sc)
-        positions=sc.get_positions()
+        sc = Atoms(
+            sc.symbols,
+            cell=sc.cell,
+            scaled_positions=sc.get_scaled_positions(),
+            pbc=True,
+        )
+        datoms = copy.deepcopy(sc)
+        positions = sc.get_positions()
         for mode in modes:
-            positions+=np.real(mode)
+            positions += np.real(mode)
         datoms.set_positions(positions)
-        spg=spglib.get_spacegroup(datoms,symprec=0.001)
+        spg = spglib.get_spacegroup(datoms, symprec=0.001)
         write(f"POSCAR_{i}.vasp", datoms, vasp5=True)
         print(datoms.cell)
         print(f"{spg}")
     return datoms
 
+
 def test():
+    pass
```

### Comparing `lawaf-0.1.0/lawaf/utils/supercell.py` & `lawaf-0.2.1/lawaf/utils/supercell.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,60 +19,72 @@
         """
         sc_matrix = np.array(sc_matrix, dtype=int)
         if len(sc_matrix.flatten()) == 3:
             sc_matrix = np.diag(sc_matrix)
         elif sc_matrix.shape == (3, 3):
             pass
         else:
-            raise ValueError('sc_matrix should be 3 or 3*3 matrix')
+            raise ValueError("sc_matrix should be 3 or 3*3 matrix")
         self.sc_matrix = sc_matrix
         self.center = center
         if center:
             self.shift = np.array([0.5, 0.5, 0.5])
         else:
             self.shift = np.zeros(3, dtype=float)
         self.inv_scmat = np.linalg.inv(self.sc_matrix.T)
         self.build_sc_vec()
         self.ncell = int(round(abs(np.linalg.det(sc_matrix))))
 
     def to_red_sc(self, x):
         return np.dot(self.inv_scmat, x) + self.shift
 
-
     def build_sc_vec(self):
-        eps_shift = np.sqrt(
-            2.0) * 1.0E-8  # shift of the grid, so to avoid double counting
-        #max_R = np.max(np.abs(self.sc_matrix)) * 3
+        eps_shift = (
+            np.sqrt(2.0) * 1.0e-8
+        )  # shift of the grid, so to avoid double counting
+        # max_R = np.max(np.abs(self.sc_matrix)) * 3
         if self.center:
             minr = -0.5
             maxr = 0.5
         else:
             minr = 0.0
             maxr = 1.0
         sc_vec = []
         newcell = self.sc_matrix
-        scorners_newcell = np.array([[0., 0., 0.], [0., 0., 1.], [0., 1., 0.],
-                                     [0., 1., 1.], [1., 0., 0.], [1., 0., 1.],
-                                     [1., 1., 0.], [1., 1., 1.]])
+        scorners_newcell = np.array(
+            [
+                [0.0, 0.0, 0.0],
+                [0.0, 0.0, 1.0],
+                [0.0, 1.0, 0.0],
+                [0.0, 1.0, 1.0],
+                [1.0, 0.0, 0.0],
+                [1.0, 0.0, 1.0],
+                [1.0, 1.0, 0.0],
+                [1.0, 1.0, 1.0],
+            ]
+        )
         corners = np.dot(scorners_newcell - self.shift, newcell)
         scorners = corners
-        #rep = np.ceil(scorners.ptp(axis=0)).astype('int') + 1
-        minrep = np.ceil(np.min(scorners, axis=0)).astype('int')
-        maxrep = np.ceil(np.max(scorners, axis=0)).astype('int') + 1
+        # rep = np.ceil(scorners.ptp(axis=0)).astype('int') + 1
+        minrep = np.ceil(np.min(scorners, axis=0)).astype("int")
+        maxrep = np.ceil(np.max(scorners, axis=0)).astype("int") + 1
 
         # sc_vec: supercell vector (map atom from unit cell to supercell)
-        #for vec in product(range(rep[0]), range(rep[1]), range(rep[2])):
-        for vec in product(range(minrep[0], maxrep[0]),
-                           range(minrep[1], maxrep[1]),
-                           range(minrep[2], maxrep[2])):
+        # for vec in product(range(rep[0]), range(rep[1]), range(rep[2])):
+        for vec in product(
+            range(minrep[0], maxrep[0]),
+            range(minrep[1], maxrep[1]),
+            range(minrep[2], maxrep[2]),
+        ):
             # compute reduced coordinates of this candidate vector in the super-cell frame
             tmp_red = self.to_red_sc(vec)
             # check if in the interior
             if (not (tmp_red <= -eps_shift).any()) and (
-                    not (tmp_red > 1.0 - eps_shift).any()):
+                not (tmp_red > 1.0 - eps_shift).any()
+            ):
                 sc_vec.append(np.array(vec))
 
         # number of times unit cell is repeated in the super-cell
         num_sc = len(sc_vec)
 
         # check that found enough super-cell vectors
         if int(round(np.abs(np.linalg.det(self.sc_matrix)))) != num_sc:
@@ -129,48 +141,45 @@
         if return_R:
             return sc_q, sc_R
         else:
             return sc_q
 
     def sc_trans_kvector(self, x, kpt, phase=0.0, real=False):
         """
-        x is a vector of quantities inside the primitive cell. 
+        x is a vector of quantities inside the primitive cell.
         qpoint is the wavevector
         phase
         x_sc= x * exp(i(qR + phase))
 
         Note: if x is a 2D m*n array, the first m*n block is the primitive cell.
         [block1, block2, block3, ... block_ncell]
         """
         factor = self.phase_factor(kpt, phase=phase)
-        ret= np.kron(factor, x)
+        ret = np.kron(factor, x)
         if real:
-            ret=np.real(ret)
+            ret = np.real(ret)
         return ret
 
     def Rvector_for_each_element(self, n_ind=1):
         """
         repeat the R_sc vectors.
         """
         return np.kron(self.sc_vec, np.ones((n_ind, 1)))
 
-
-
     def sc_index(self, indices, n_ind=None):
         """
         Note that the number of indices could be inequal to the repeat period.
         e.g. for n_orb of orbitals, the indices of atoms iatom for each orbital.
         In that case, in the second unit cell (c=1 here), iatom-> iatom+n_ind,
         where n_ind=natoms in primitive cell.
         """
         sc_ind = []
         if n_ind is None:
             n_ind = len(indices)
-        for c, cur_sc_vec in enumerate(
-                self.sc_vec):  # go over all super-cell vectors
+        for c, cur_sc_vec in enumerate(self.sc_vec):  # go over all super-cell vectors
             for ind in indices:
                 sc_ind.append(ind + c * n_ind)
         return sc_ind
 
     @lru_cache(maxsize=5000)
     def _sc_R_to_pair_ind(self, R_plus_Rv):
         """
@@ -189,40 +198,36 @@
         pair_ind1 = self.sc_vec_dict[tuple(orig_part)]
         return sc_part, pair_ind1
 
     def sc_jR_to_scjR(self, j, R, Rv, n_basis):
         """
         (j, R) in primitive cell to (j', R') in supercell.
         """
-        Rprim, pair_ind = self._sc_R_to_pair_ind(
-            tuple(np.array(R) + np.array(Rv)))
+        Rprim, pair_ind = self._sc_R_to_pair_ind(tuple(np.array(R) + np.array(Rv)))
         return j + pair_ind * n_basis, tuple(Rprim)
 
     def sc_i_to_sci(self, i, ind_Rv, n_basis):
         return i + ind_Rv * n_basis
 
     def sc_ijR_only(self, i, j, R, n_basis):
         ret = []
-        for c, cur_sc_vec in enumerate(
-                self.sc_vec):  # go over all super-cell vectors
+        for c, cur_sc_vec in enumerate(self.sc_vec):  # go over all super-cell vectors
             sc_part, pair_ind = self._sc_R_to_pair_ind(tuple(R + cur_sc_vec))
             sc_i = i + c * n_basis
             sc_j = j + pair_ind * n_basis
             ret.append((sc_i, sc_j, tuple(sc_part)))
         return ret
 
     def sc_jR(self, jlist, Rjlist, n_basis):
         sc_jlist = []
         sc_Rjlist = []
-        for c, cur_sc_vec in enumerate(
-                self.sc_vec):  # go over all super-cell vectors
-            #for i , j, ind_R, val in
+        for c, cur_sc_vec in enumerate(self.sc_vec):  # go over all super-cell vectors
+            # for i , j, ind_R, val in
             for j, Rj in zip(jlist, Rjlist):
-                sc_part, pair_ind = self._sc_R_to_pair_ind(
-                    tuple(Rj + cur_sc_vec))
+                sc_part, pair_ind = self._sc_R_to_pair_ind(tuple(Rj + cur_sc_vec))
                 sc_j = j + pair_ind * n_basis
                 sc_jlist.append(sc_j)
                 sc_Rjlist.append(tuple(sc_part))
         return sc_jlist, sc_Rjlist
 
     def sc_ijR(self, terms, n_basis):
         """
@@ -233,20 +238,18 @@
         ========================
         terms: either list of [i, j, R, val] or  dict{(i,j, R): val}
         pos: reduced positions in the unit cell.
         Returns:
         =======================
         """
         ret_dict = OrderedDict()
-        for c, cur_sc_vec in enumerate(
-                self.sc_vec):  # go over all super-cell vectors
-            #for i , j, ind_R, val in
+        for c, cur_sc_vec in enumerate(self.sc_vec):  # go over all super-cell vectors
+            # for i , j, ind_R, val in
             for (i, j, ind_R), val in terms.items():
-                sc_part, pair_ind = self._sc_R_to_pair_ind(
-                    tuple(ind_R + cur_sc_vec))
+                sc_part, pair_ind = self._sc_R_to_pair_ind(tuple(ind_R + cur_sc_vec))
                 # index of "from" and "to" hopping indices
                 sc_i = i + c * n_basis
                 sc_j = j + pair_ind * n_basis
 
                 # hi = self._hoppings[h][1] + c * self._norb
                 # hj = self._hoppings[h][2] + pair_ind * self._norb
                 ret_dict[(sc_i, sc_j, tuple(sc_part))] = val
@@ -259,24 +262,23 @@
         terms: either list of [i, j, R, val] or  dict{(i,j, R): val}
         pos: reduced positions in the unit cell.
         Returns:
         =======================
         """
         sc_Rlist = []
         sc_HR = []
-        for c, cur_sc_vec in enumerate(
-                self.sc_vec):  # go over all super-cell vectors
-            #for i , j, ind_R, val in
+        for c, cur_sc_vec in enumerate(self.sc_vec):  # go over all super-cell vectors
+            # for i , j, ind_R, val in
             for iR, R in enumerate(Rlist):
                 H = HR[iR]
-                sc_part, pair_ind = self._sc_R_to_pair_ind(
-                    tuple(R + cur_sc_vec))
+                sc_part, pair_ind = self._sc_R_to_pair_ind(tuple(R + cur_sc_vec))
                 sc_Rlist.append(sc_part)
-                sc_val = np.zeros((n_basis * self.ncell, n_basis * self.ncell),
-                                  dtype=HR.dtype)
+                sc_val = np.zeros(
+                    (n_basis * self.ncell, n_basis * self.ncell), dtype=HR.dtype
+                )
                 for i in range(n_basis):
                     for j in range(n_basis):
                         sc_i = i + c * n_basis
                         sc_j = j + pair_ind * n_basis
                         sc_val[sc_i, sc_j] = H[i, j]
                 sc_HR.append(sc_val)
         return np.array(sc_Rlist, dtype=int), np.array(sc_HR)
@@ -286,77 +288,80 @@
         terms: H[R][i,j] = val
         ========================
         terms: either list of [i, j, R, val] or  dict{(i,j, R): val}
         pos: reduced positions in the unit cell.
         Returns:
         =======================
         """
-        sc_RHdict = defaultdict(lambda: np.zeros(
-            (n_basis * self.ncell, n_basis * self.ncell), dtype=H.dtype))
-        for c, cur_sc_vec in enumerate(
-                self.sc_vec):  # go over all super-cell vectors
+        sc_RHdict = defaultdict(
+            lambda: np.zeros(
+                (n_basis * self.ncell, n_basis * self.ncell), dtype=H.dtype
+            )
+        )
+        for c, cur_sc_vec in enumerate(self.sc_vec):  # go over all super-cell vectors
             for R, H in RHdict.items():
-                sc_part, pair_ind = self._sc_R_to_pair_ind(
-                    tuple(R + cur_sc_vec))
+                sc_part, pair_ind = self._sc_R_to_pair_ind(tuple(R + cur_sc_vec))
                 ii = c * n_basis
                 jj = pair_ind * n_basis
-                sc_RHdict[R][ii:ii + n_basis, jj:jj + n_basis] += H
+                sc_RHdict[R][ii : ii + n_basis, jj : jj + n_basis] += H
         return sc_RHdict
 
     def sc_atoms(self, atoms):
         """
         This function is compatible with ase.build.make_supercell.
         They should produce the same result.
         """
         from ase.atoms import Atoms
+
         sc_cell = self.sc_cell(atoms.get_cell())
         sc_pos = self.sc_pos(atoms.get_scaled_positions())
         sc_numbers = self.sc_trans_invariant(atoms.get_atomic_numbers())
-        sc_magmoms = self.sc_trans_invariant(
-            atoms.get_initial_magnetic_moments())
-        return Atoms(cell=sc_cell,
-                     scaled_positions=sc_pos,
-                     numbers=sc_numbers,
-                     magmoms=sc_magmoms)
+        sc_magmoms = self.sc_trans_invariant(atoms.get_initial_magnetic_moments())
+        return Atoms(
+            cell=sc_cell,
+            scaled_positions=sc_pos,
+            numbers=sc_numbers,
+            magmoms=sc_magmoms,
+        )
 
     def phase_factor(self, qpoint, phase=0, real=True):
-        f = np.exp(2j * np.pi * np.einsum('i, ji -> j', qpoint, self.sc_vec) +
-                   1j * phase)
+        f = np.exp(
+            2j * np.pi * np.einsum("i, ji -> j", qpoint, self.sc_vec) + 1j * phase
+        )
         if real:
             f = np.real(f)
         return f
 
     def modulation_function_R(self, func):
         return [func(R) for R in self.R_sc]
 
-
-
     def _make_translate_maps(positions, basis, sc_mat, tol_r=1e-4):
         """
         find the mapping between supercell and translated cell.
         Returns:
         ===============
         A N * nbasis array.
         index[i] is the mapping from supercell to translated supercell so that
         T(r_i) psi = psi[indices[i]].
-    
+
         """
-        a1 = Atoms(symbols='H', positions=[(0, 0, 0)], cell=[1, 1, 1])
+        a1 = Atoms(symbols="H", positions=[(0, 0, 0)], cell=[1, 1, 1])
         sc = make_supercell(a1, self._scmat)
         rs = sc.get_scaled_positions()
 
-        indices = np.zeros([len(rs), len(positions)], dtype='int32')
+        indices = np.zeros([len(rs), len(positions)], dtype="int32")
         for i, ri in enumerate(rs):
             inds = []
             Tpositions = positions + np.array(ri)
             for i_basis, pos in enumerate(positions):
                 for j_basis, Tpos in enumerate(Tpositions):
                     dpos = Tpos - pos
                     if close_to_int(dpos, tol_r) and (
-                            self._basis[i_basis] == self._basis[j_basis]):
+                        self._basis[i_basis] == self._basis[j_basis]
+                    ):
                         indices[i, j_basis] = i_basis
 
         self._trans_rs = rs
         self._trans_indices = indices
 
 
 def smod(x):
@@ -367,18 +372,18 @@
 smod = np.vectorize(smod)
 
 
 def map_to_primitive(atoms, primitive_atoms, offset=(0, 0, 0)):
     """
     Find the mapping of a supercell to a primitive cell.
     :param atoms: the positions of atoms
-    :param primitive_atoms: 
-    :param offset: 
-    :param 0: 
-    :param 0): 
+    :param primitive_atoms:
+    :param offset:
+    :param 0:
+    :param 0):
 
     """
     ilist = []
     Rlist = []
     offset = np.array(offset, dtype=float)
     ppos = primitive_atoms.get_positions()
     pos = atoms.get_positions()
@@ -396,33 +401,40 @@
         if not found:
             print("Not found")
     return np.array(ilist, dtype=int), np.array(Rlist, dtype=int)
 
 
 def test():
     sc_mat = np.diag([1, 1, 3])
-    #sc_mat[0, 1] = 2
+    # sc_mat[0, 1] = 2
     spm = SupercellMaker(sc_matrix=sc_mat, center=False)
     print("sc_vec", spm.sc_vec)
     print(spm.sc_cell([1, 1, 1]))
     print(spm.sc_pos([[0.5, 1, 1]]))
     print(spm.sc_pos([[0.5, 1, 0.5]]))
-    print(spm.sc_trans_invariant(['Fe']))
-    print(spm.sc_ijR({
-        (0, 0, (0, 0, 1)): 1.2,
-        (1, 1, (0, 0, 1)): 1.2,
-    }, 2))
+    print(spm.sc_trans_invariant(["Fe"]))
+    print(
+        spm.sc_ijR(
+            {
+                (0, 0, (0, 0, 1)): 1.2,
+                (1, 1, (0, 0, 1)): 1.2,
+            },
+            2,
+        )
+    )
     print(spm.sc_index(indices=(1, 2)))
     print(spm.sc_index(indices=(1, 2), n_ind=4))
     from ase.atoms import Atoms
-    atoms = Atoms('HO', positions=[[0, 0, 0], [0, 0.2, 0]], cell=[1, 1, 1])
+
+    atoms = Atoms("HO", positions=[[0, 0, 0], [0, 0.2, 0]], cell=[1, 1, 1])
     from ase.build import make_supercell
+
     atoms2 = make_supercell(atoms, sc_mat)
     atoms3 = spm.sc_atoms(atoms)
-    #print(atoms2.get_positions())
-    #print(atoms3.get_positions())
-    assert (atoms2 == atoms3)
+    # print(atoms2.get_positions())
+    # print(atoms3.get_positions())
+    assert atoms2 == atoms3
     assert (atoms2.get_positions() == atoms3.get_positions()).all()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     test()
```

### Comparing `lawaf-0.1.0/lawaf/utils/symbol.py` & `lawaf-0.2.1/lawaf/utils/symbol.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 import re
 from collections import OrderedDict
 from ase.io import read
 
+
 def symbol_number(symbols):
     """
     symbols can be also atoms. Thus the chemical symbols will be used.
     Fe Fe Fe O -> {Fe1:0 Fe2:1 Fe3:2 O1:3}
     """
     try:
-        symbs=symbols.copy().get_chemical_symbols()
+        symbs = symbols.copy().get_chemical_symbols()
     except Exception:
-        symbs=symbols
-    symdict={}
-    result=OrderedDict()
-    for i,sym in enumerate(symbs):
+        symbs = symbols
+    symdict = {}
+    result = OrderedDict()
+    for i, sym in enumerate(symbs):
         if sym in symdict:
-            symdict[sym]=symdict[sym]+1
+            symdict[sym] = symdict[sym] + 1
         else:
-            symdict[sym]=1
-        result[sym+str(symdict[sym])]=i
+            symdict[sym] = 1
+        result[sym + str(symdict[sym])] = i
     return result
 
 
 def symnum_to_sym(symbol_number):
     """
     symnum-> sym. eg: Fe1-> Fe
     """
     try:
-        a=re.search('[A-Za-z]+',symbol_number).group()
+        a = re.search("[A-Za-z]+", symbol_number).group()
         return a
     except AttributeError:
-        raise AttributeError('%s is not a good symbol_number'%symbol_number)
+        raise AttributeError("%s is not a good symbol_number" % symbol_number)
+
 
-def get_symdict(filename='POSCAR',atoms=None):
+def get_symdict(filename="POSCAR", atoms=None):
     """
     get a symbol_number: index dict.
     """
     if atoms is not None:
-        syms=atoms.get_chemical_symbols()
+        syms = atoms.get_chemical_symbols()
     elif filename is not None and atoms is None:
-        syms=read(filename).get_chemical_symbols()
+        syms = read(filename).get_chemical_symbols()
 
-    symdict=symbol_number(syms)
+    symdict = symbol_number(syms)
     return symdict
-
```

### Comparing `lawaf-0.1.0/lawaf/wannierization/density_scdmk.py` & `lawaf-0.2.1/lawaf/wannierization/density_scdmk.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,26 +6,28 @@
 from lawaf.scdm.lwf import LWF
 from lawaf.scdm.scdmk import Lawaf, scdm, occupation_func
 from ase.dft.kpoints import monkhorst_pack
 import os
 
 
 class SpinDensityMatricesDownfolder(Lawaf):
-    def __init__(self,
-                 evals,
-                 density_matrices,
-                 positions,
-                 kmesh,
-                 nwann,
-                 Hks,
-                 Sk=None,
-                 has_phase=True,
-                 Rgrid=None,
-                 sort_cols=True,
-                 atoms=None):
+    def __init__(
+        self,
+        evals,
+        density_matrices,
+        positions,
+        kmesh,
+        nwann,
+        Hks,
+        Sk=None,
+        has_phase=True,
+        Rgrid=None,
+        sort_cols=True,
+        atoms=None,
+    ):
         self.nspin = 2
         self.dm = density_matrices
         self.positions = positions
         self.kmesh = kmesh
         self.kpts = monkhorst_pack(kmesh)
         self.nkpt = len(self.kpts)
         self.kweight = [1.0 / self.nkpt] * self.nkpt
@@ -41,166 +43,177 @@
         self.sort_cols = sort_cols
 
         self.Rgrid = Rgrid
         self._prepare_Rlist()
         self.nR = self.Rlist.shape[0]
         self.Amn = np.zeros((self.nkpt, self.nband, self.nwann), dtype=complex)
 
-        self.wannk = np.zeros((self.nkpt, self.nbasis, self.nwann),
-                              dtype=complex)
+        self.wannk = np.zeros((self.nkpt, self.nbasis, self.nwann), dtype=complex)
         self.Hwann_k = np.zeros(
-            (self.nspin, self.nkpt, self.nwann, self.nwann), dtype=complex)
+            (self.nspin, self.nkpt, self.nwann, self.nwann), dtype=complex
+        )
 
-        self.HwannR = np.zeros((self.nspin, self.nR, self.nwann, self.nwann),
-                               dtype=complex)
-        self.wannR = np.zeros((self.nR, self.nbasis, self.nwann),
-                              dtype=complex)
+        self.HwannR = np.zeros(
+            (self.nspin, self.nR, self.nwann, self.nwann), dtype=complex
+        )
+        self.wannR = np.zeros((self.nR, self.nbasis, self.nwann), dtype=complex)
         self.atoms = atoms
 
     @classmethod
-    def from_wannier(cls,
-                     path,
-                     prefix_up,
-                     prefix_down,
-                     kmesh=[3, 3, 3],
-                     weight_func_type='Fermi',
-                     mu=None,
-                     sigma=None,
-                     nwann=None):
+    def from_wannier(
+        cls,
+        path,
+        prefix_up,
+        prefix_down,
+        kmesh=[3, 3, 3],
+        weight_func_type="Fermi",
+        mu=None,
+        sigma=None,
+        nwann=None,
+    ):
         from lawaf.wrapper.myTB import MyTB
+
         k = kmesh[0]
         kpts = monkhorst_pack(kmesh)
 
         model_up = MyTB.read_from_wannier_dir(path, prefix_up)
         model_down = MyTB.read_from_wannier_dir(path, prefix_down)
 
-        #evals_up, evecs_up = model_up.solve_all(kpts)
-        #evals_down, evecs_down = model_down.solve_all(kpts)
+        # evals_up, evecs_up = model_up.solve_all(kpts)
+        # evals_down, evecs_down = model_down.solve_all(kpts)
 
         hams_up, _, evals_up, evecs_up = model_up.HS_and_eigen(kpts)
         hams_down, _, evals_down, evecs_down = model_down.HS_and_eigen(kpts)
         evals = np.array([evals_up, evals_down])
         try:
             positions = model_up.positions
         except Exception:
             positions = None
 
-        weight_func = occupation_func(ftype=weight_func_type,
-                                      mu=mu,
-                                      sigma=sigma)
+        weight_func = occupation_func(ftype=weight_func_type, mu=mu, sigma=sigma)
 
         nk = len(kpts)
-        rho = np.zeros(shape=(nk, model_up.nbasis, model_down.nbasis),
-                       dtype=complex)
+        rho = np.zeros(shape=(nk, model_up.nbasis, model_down.nbasis), dtype=complex)
         for ik, k in enumerate(kpts):
-            rho[ik] = evecs_up[ik] @ np.diag(weight_func(evals_up[
-                ik])) @ evecs_up[ik].T.conj() - evecs_down[ik] @ np.diag(
-                    weight_func(evals_down[ik])) @ evecs_down[ik].T.conj()
+            rho[ik] = (
+                evecs_up[ik]
+                @ np.diag(weight_func(evals_up[ik]))
+                @ evecs_up[ik].T.conj()
+                - evecs_down[ik]
+                @ np.diag(weight_func(evals_down[ik]))
+                @ evecs_down[ik].T.conj()
+            )
 
         if nwann is None:
             nwann = model_up.nbasis
-        return SpinDensityMatricesDownfolder(evals=evals,
-                                             density_matrices=rho,
-                                             positions=positions,
-                                             kmesh=kmesh,
-                                             nwann=nwann,
-                                             Hks=np.array([hams_up,
-                                                           hams_down]),
-                                             Sk=None,
-                                             has_phase=False,
-                                             Rgrid=None,
-                                             sort_cols=True)
+        return SpinDensityMatricesDownfolder(
+            evals=evals,
+            density_matrices=rho,
+            positions=positions,
+            kmesh=kmesh,
+            nwann=nwann,
+            Hks=np.array([hams_up, hams_down]),
+            Sk=None,
+            has_phase=False,
+            Rgrid=None,
+            sort_cols=True,
+        )
 
     def auto_set_anchors(self, kpt=(0.0, 0.0, 0.0)):
         """
         Automatically find the columns using an anchor kpoint.
         kpt: the kpoint used to set as anchor points. default is Gamma (0,0,0)
         """
         ik = self.find_k(kpt)
         density = np.real(np.diag(np.sum(self.spin_dm, axis=0))) / self.nkpt
         self.cols = scdm(self.spin_dm[ik], self.nwann)
         print(f"anchor_kpt={kpt}. Selected columns: {self.cols}.")
         if self.sort_cols:
             self.cols = np.sort(self.cols)
-        #print(f"The eigenvalues at anchor k: {self.get_eval_k(ik)}")
+        # print(f"The eigenvalues at anchor k: {self.get_eval_k(ik)}")
         print(f"anchor_kpt={kpt}. Selected columns: {self.cols}.")
         return self.cols
 
     def get_wannk_and_Hk(self):
         """
         calculate Wannier function and H in k-space.
         """
         spin_dm = np.average(self.spin_dm[:, :], axis=0)
 
         spin_dmc = spin_dm[:, self.cols]
         for ik in range(self.nkpt):
             self.wannk[ik] = self.spin_dm[ik][:, self.cols]
             ##self.wannk[ik] = spin_dm
-            #self.wannk[ik] = np.eye(self.nbasis)
+            # self.wannk[ik] = np.eye(self.nbasis)
 
             U, E, VT = np.linalg.svd(spin_dmc, full_matrices=False)
-            #self.wannk[ik] = U[:,:self.nwann] @  VT[:self.nwann, :self.nwann]
+            # self.wannk[ik] = U[:,:self.nwann] @  VT[:self.nwann, :self.nwann]
 
             U, E, VT = np.linalg.svd(self.wannk[ik], full_matrices=False)
-            self.wannk[ik] = U@VT
-            #self.wannk[ik], _ = qr(self.wannk[ik], mode='economic')
+            self.wannk[ik] = U @ VT
+            # self.wannk[ik], _ = qr(self.wannk[ik], mode='economic')
             # h = self.Amn[ik, :, :].T.conj() @ np.diag(
             #    self.get_eval_k(ik)) @ self.Amn[ik, :, :]
-            #self.wannk[ik] = np.eye(self.nbasis)
+            # self.wannk[ik] = np.eye(self.nbasis)
             # self.wannk[ik] = self.wannk[ik] / np.linalg.norm(self.wannk[ik],
             #                                                 axis=0)[None, :]
             # self.wannk[ik]=np.linalg.eig(self.wannk[ik])[1]
 
-            #print(np.real(self.wannk[ik].T.conj() @ self.wannk[ik]))
-            #print(np.imag(self.wannk[ik].T.conj() @ self.wannk[ik]))
+            # print(np.real(self.wannk[ik].T.conj() @ self.wannk[ik]))
+            # print(np.imag(self.wannk[ik].T.conj() @ self.wannk[ik]))
             h_up = self.wannk[ik].T.conj() @ self.Hks[0, ik] @ self.wannk[ik]
             h_dn = self.wannk[ik].T.conj() @ self.Hks[1, ik] @ self.wannk[ik]
             self.Hwann_k[0, ik] = h_up
             self.Hwann_k[1, ik] = h_dn
         return self.wannk, self.Hwann_k
 
     def k_to_R(self):
         """
         Calculate Wannier function and Hamiltonian from K space to R space.
         """
         for iR, R in enumerate(self.Rlist):
             for ik, k in enumerate(self.kpts):
                 phase = np.exp(-2j * np.pi * np.dot(R, k))
-                self.wannR[iR] += self.wannk[
-                    ik, :, :] * phase * self.kweight[ik]
+                self.wannR[iR] += self.wannk[ik, :, :] * phase * self.kweight[ik]
                 for ispin in [0, 1]:
-                    self.HwannR[ispin, iR] += self.Hwann_k[
-                        ispin, ik, :, :] * phase * self.kweight[ik]
+                    self.HwannR[ispin, iR] += (
+                        self.Hwann_k[ispin, ik, :, :] * phase * self.kweight[ik]
+                    )
             if np.linalg.norm(R) < 0.01:
                 print(self.wannR[iR])
         self.get_wannier_centers()
-        self.lwf_up = LWF(self.wannR,
-                          self.HwannR[0],
-                          self.Rlist,
-                          cell=np.eye(3),
-                          wann_centers=self.wann_centers)
-        self.lwf_down = LWF(self.wannR,
-                            self.HwannR[1],
-                            self.Rlist,
-                            cell=np.eye(3),
-                            wann_centers=self.wann_centers)
+        self.lwf_up = LWF(
+            self.wannR,
+            self.HwannR[0],
+            self.Rlist,
+            cell=np.eye(3),
+            wann_centers=self.wann_centers,
+        )
+        self.lwf_down = LWF(
+            self.wannR,
+            self.HwannR[1],
+            self.Rlist,
+            cell=np.eye(3),
+            wann_centers=self.wann_centers,
+        )
         return self.lwf_up, self.lwf_down
 
-    def save_to_nc(self, output_path='./', prefix='Downfolded'):
+    def save_to_nc(self, output_path="./", prefix="Downfolded"):
         txt_fname = os.path.join(output_path, f"{prefix}_up.txt")
         nc_fname = os.path.join(output_path, f"{prefix}_up.nc")
         self.lwf_up.save_txt(txt_fname)
         self.lwf_up.write_nc(nc_fname, atoms=self.atoms)
 
         txt_fname = os.path.join(output_path, f"{prefix}_down.txt")
         nc_fname = os.path.join(output_path, f"{prefix}_down.nc")
         self.lwf_down.save_txt(txt_fname)
         self.lwf_down.write_nc(nc_fname, atoms=self.atoms)
 
         from lawaf.plot import plot_band
+
         ax = plot_band(self.lwf_up)
 
-        ax = plot_band(self.lwf_down, color='red')
+        ax = plot_band(self.lwf_down, color="red")
         # plt.show()
 
     def get_wannier():
         pass
```

### Comparing `lawaf-0.1.0/lawaf/wrapper/ijR.py` & `lawaf-0.2.1/lawaf/wrapper/ijR.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,31 @@
 from scipy.linalg import eigh
 from scipy.sparse import csr_matrix
 from netCDF4 import Dataset
 from collections import defaultdict
 from lawaf.utils.supercell import SupercellMaker
 from ase.dft.kpoints import bandpath
 
+
 class ijR(object):
-    def __init__(self,
-                 nbasis,
-                 cell=np.eye(3, dtype=float),
-                 data=None,
-                 positions=None,
-                 sparse=False,
-                 double_site_energy=2.0):
+    def __init__(
+        self,
+        nbasis,
+        cell=np.eye(3, dtype=float),
+        data=None,
+        positions=None,
+        sparse=False,
+        double_site_energy=2.0,
+    ):
         self.cell = cell
         self.nbasis = nbasis
         if data is not None:
             self.data = data
         else:
-            self.data = defaultdict(lambda: np.zeros(
-                (nbasis, nbasis), dtype=float))
+            self.data = defaultdict(lambda: np.zeros((nbasis, nbasis), dtype=float))
         if positions is None:
             self.positions = np.zeros((nbasis, 3))
         else:
             self.positions = positions
         self.sparse = sparse
         self.double_site_energy = double_site_energy
         if sparse:
@@ -46,16 +48,15 @@
             ret.positions = scmaker.sc_pos(self.positions)
         ret.cell = scmaker.sc_cell(self.cell)
         ret.sparse = self.sparse
         ret.double_site_energy = self.double_site_energy
         for R, mat in self.data.items():
             for i in range(self.nbasis):
                 for j in range(self.nbasis):
-                    for sc_i, sc_j, sc_R in scmaker.sc_ijR_only(
-                            i, j, R, self.nbasis):
+                    for sc_i, sc_j, sc_R in scmaker.sc_ijR_only(i, j, R, self.nbasis):
                         ret.data[sc_R][sc_i, sc_j] = mat[i, j]
         return ret
 
     @property
     def Rlist(self):
         return list(self.data.keys())
 
@@ -89,26 +90,25 @@
             newmat = (mat + mat.T.conj()) / 2.0
         else:
             newR = R
             newmat = mat
         return newR, newmat
 
     def _to_positive_R(self):
-        new_ijR = ijR(self.nbasis,
-                      cell=self.cell,
-                      positions=self.positions,
-                      sparse=self.sparse)
+        new_ijR = ijR(
+            self.nbasis, cell=self.cell, positions=self.positions, sparse=self.sparse
+        )
         for R, mat in self.data:
             newR, newmat = self._positive_R_mat(R, mat)
             new_ijR.data[newR] = newmat
         return new_ijR
 
     def shift_position(self, rpos):
         pos = self.positions
-        shift = np.zeros((self.nbasis, 3), dtype='int')
+        shift = np.zeros((self.nbasis, 3), dtype="int")
         shift[:, :] = np.round(pos - rpos)
         newpos = copy.deepcopy(pos)
         for i in range(self.nbasis):
             newpos[i] = pos[i] - shift[i]
         d = ijR(self.nbasis)
         d.positions = newpos
         for R, v in self.data.items():
@@ -128,140 +128,144 @@
         return d
 
     def save(self, fname):
         try:
             from netCDF4 import Dataset
         except ImportError():
             print("Warning: ")
-        root = Dataset(fname, 'w', format="NETCDF4")
+        root = Dataset(fname, "w", format="NETCDF4")
         root.createDimension("nR", self.nR)
         root.createDimension("three", 3)
         root.createDimension("nbasis", self.nbasis)
-        R = root.createVariable("R", 'i4', ("nR", "three"))
-        data = root.createVariable("data", 'f8', ("nR", "nbasis", "nbasis"))
-        positions = root.createVariable("positions", 'f8', ("nbasis", "three"))
-        cell = root.createVariable("cell", 'f8', ("three", "three"))
+        R = root.createVariable("R", "i4", ("nR", "three"))
+        data = root.createVariable("data", "f8", ("nR", "nbasis", "nbasis"))
+        positions = root.createVariable("positions", "f8", ("nbasis", "three"))
+        cell = root.createVariable("cell", "f8", ("three", "three"))
         R[:] = np.array(self.Rlist)
         data[:] = np.array(tuple(self.data.values()))
         positions[:] = np.array(self.positions)
         cell[:] = np.array(self.cell)
         root.close()
 
     def write_txt(self, fname):
-        with open(fname, 'w') as myfile:
+        with open(fname, "w") as myfile:
             myfile.write(f"Number_of_R: {self.nR}\n")
             myfile.write(f"Number_of_basis_functions: {self.nbasis}\n")
             myfile.write(f"Cell parameter: {self.cell}\n")
-            myfile.write("Hamiltonian:  \n" + "="*60+'\n')
-            for iR,R in enumerate(self.Rlist):
+            myfile.write("Hamiltonian:  \n" + "=" * 60 + "\n")
+            for iR, R in enumerate(self.Rlist):
                 myfile.write(f"index of R: {iR}.  R = {R}\n")
-                d=self.data[R]
+                d = self.data[R]
                 for i in rang(nbais):
                     for j in range(nbasis):
                         myfile.write(f"R = {R}\t. i = {i}, j={j}, H(i,j,R)= {d[i,j]}")
-                myfile.write('-'*60+'\n')
+                myfile.write("-" * 60 + "\n")
 
     @staticmethod
     def load_ijR(fname):
-        root = Dataset(fname, 'r')
-        nbasis = root.dimensions['nbasis'].size
-        Rlist = root.variables['R'][:]
+        root = Dataset(fname, "r")
+        nbasis = root.dimensions["nbasis"].size
+        Rlist = root.variables["R"][:]
         m = ijR(nbasis)
-        mdata = root.variables['data'][:]
+        mdata = root.variables["data"][:]
         for iR, R in enumerate(Rlist):
             m.data[tuple(R)] = mdata[iR]
-        m.positions = root.variables['positions'][:]
-        m.cell = root.variables['cell'][:]
+        m.positions = root.variables["positions"][:]
+        m.cell = root.variables["cell"][:]
         return m
 
     @staticmethod
     def from_tbmodel(model):
         ret = ijR(nbasis=model.size)
         for R, v in model.hop.items():
             ret.data[R] = v
         ret.positions = np.reshape(model.pos, (model.size, 3))
         ret.cell = model.uc
         return ret
 
     @staticmethod
     def from_tbmodel_hdf5(fname):
         from tbmodels import Model
+
         m = Model.from_hdf5_file(fname)
         ret = ijR(nbasis=m.size)
         for R, v in m.hop.items():
             ret.data[R] = v
         ret.positions = np.reshape(m.pos, (m.size, 3))
         ret.cell = m.uc
         return ret
 
     def to_spin_polarized(self, order=1):
         """
-        repeat 
+        repeat
         order =1 : orb1_up, orb1_dn, orb2_up, orb2_dn...
         order =2 : orb1_up, orb2_up, ... orb1_dn, orb2_dn...
         """
         ret = ijR(self.nbasis * 2)
         if self.positions is None:
             ret.positions = None
         else:
             ret.positions = np.repeat(self.positions, 2, axis=0)
         for R, mat in self.data.items():
             ret.data[R][::2, ::2] = mat
             ret.data[R][1::2, 1::2] = mat
         return ret
 
     def gen_ham(self, k):
-        Hk = np.zeros((self.nbasis, self.nbasis), dtype='complex')
+        Hk = np.zeros((self.nbasis, self.nbasis), dtype="complex")
         np.fill_diagonal(Hk, self.site_energies)
         for R, mat in self.hoppings.items():
             phase = np.exp(2j * np.pi * np.dot(k, R))
             Hk += mat * phase + (mat * phase).T.conj()
         return Hk
 
     def solve_all(self, kpts):
         nk = len(kpts)
         evals = np.zeros((nk, self.nbasis))
-        evecs = np.zeros((nk, self.nbasis, self.nbasis),dtype=complex)
+        evecs = np.zeros((nk, self.nbasis, self.nbasis), dtype=complex)
         for ik, k in enumerate(kpts):
             evals_k, evecs_k = eigh(self.gen_ham(k))
             evals[ik, :] = evals_k
             evecs[ik, :, :] = evecs_k
         return evals, evecs
 
-    def plot_band(self,
-                  kvectors=np.array([[0, 0, 0], [0.5, 0, 0], [0.5, 0.5, 0],
-                                     [0, 0, 0], [.5, .5, .5]]),
-                  knames=['$\Gamma$', 'X', 'M', '$\Gamma$', 'R'],
-                  supercell_matrix=None,
-                  npoints=100,
-                  efermi=None,
-                  ax=None):
+    def plot_band(
+        self,
+        kvectors=np.array(
+            [[0, 0, 0], [0.5, 0, 0], [0.5, 0.5, 0], [0, 0, 0], [0.5, 0.5, 0.5]]
+        ),
+        knames=["$\Gamma$", "X", "M", "$\Gamma$", "R"],
+        supercell_matrix=None,
+        npoints=100,
+        efermi=None,
+        ax=None,
+    ):
         if ax is None:
             _fig, ax = plt.subplots()
         if supercell_matrix is not None:
             kvectors = [np.dot(k, supercell_matrix) for k in kvectors]
         kpts, x, X = bandpath(kvectors, self.cell, npoints)
         evalues, _evecs = self.solve_all(kpts=kpts)
         for i in range(evalues.shape[1]):
-            ax.plot(x, evalues[:, i], color='blue', alpha=1)
+            ax.plot(x, evalues[:, i], color="blue", alpha=1)
 
         if efermi is not None:
-            plt.axhline(self.get_fermi_level(), linestyle='--', color='gray')
+            plt.axhline(self.get_fermi_level(), linestyle="--", color="gray")
         else:
             try:
-                plt.axhline(self.get_fermi_level(), linestyle='--', color='gray')
+                plt.axhline(self.get_fermi_level(), linestyle="--", color="gray")
             except:
                 pass
-        ax.set_xlabel('k-point')
-        ax.set_ylabel('Energy (eV)')
+        ax.set_xlabel("k-point")
+        ax.set_ylabel("Energy (eV)")
         ax.set_xlim(x[0], x[-1])
         ax.set_xticks(X)
         ax.set_xticklabels(knames)
         for x in X:
-            ax.axvline(x, linewidth=0.6, color='gray')
+            ax.axvline(x, linewidth=0.6, color="gray")
         return ax
 
     def validate(self):
         # make sure all R are 3d.
         for R in self.data.keys():
             if len(R) != 3:
                 raise ValueError("R should be 3d")
```

### Comparing `lawaf-0.1.0/lawaf/wrapper/myTB.py` & `lawaf-0.2.1/lawaf/wrapper/myTB.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os
 import numpy as np
 import copy
 from scipy.linalg import eigh
 from scipy.sparse import csr_matrix
 from scipy.io import netcdf_file
 from collections import defaultdict
-#from tbmodels import Model
+
+# from tbmodels import Model
 from ase.io import read
 from ase.atoms import Atoms
 from TB2J.utils import auto_assign_basis_name
 from TB2J.wannier import parse_ham, parse_xyz
 
 
-class AbstractTB():
+class AbstractTB:
     def __init__(self, R2kfactor, nspin, norb):
         #: :math:`\alpha` used in :math:`H(k)=\sum_R  H(R) \exp( \alpha k \cdot R)`,
         #: Should be :math:`2\pi i` or :math:`-2\pi i`
         self.is_siesta = False
         self.is_orthogonal = True
         self.R2kfactor = R2kfactor
 
@@ -52,15 +53,15 @@
         raise NotImplementedError()
 
     def HSE(self, kpt):
         raise NotImplementedError()
 
     def HS_and_eigen(self, kpts):
         """
-        get Hamiltonian, overlap matrices, eigenvalues, eigen vectors for all kpoints. 
+        get Hamiltonian, overlap matrices, eigenvalues, eigen vectors for all kpoints.
 
         :param:
 
         * kpts: list of k points.
 
         :returns:
 
@@ -92,16 +93,15 @@
         :param ndim: number of dimensions.
         :param nspin: number of spins.
         """
 
         if data is not None:
             self.data = data
         else:
-            self.data = defaultdict(lambda: np.zeros(
-                (nbasis, nbasis), dtype=complex))
+            self.data = defaultdict(lambda: np.zeros((nbasis, nbasis), dtype=complex))
         self._nbasis = nbasis
         self._nspin = nspin
         self._norb = nbasis // nspin
         self._ndim = ndim
         if positions is None:
             self._positions = np.zeros((nbasis, self.ndim))
         else:
@@ -160,36 +160,30 @@
         """
         The hopping parameters, not including any onsite energy.
         """
         data = copy.deepcopy(self.data)
         np.fill_diagonal(data[(0, 0, 0)], 0.0)
         return data
 
-
     @staticmethod
-    def read_from_wannier_dir(path,
-                              prefix,
-                              posfile='POSCAR',
-                              nls=True,
-                              groupby='spin'):
+    def read_from_wannier_dir(path, prefix, posfile="POSCAR", nls=True, groupby="spin"):
         """
-        read tight binding model from a wannier function directory. 
+        read tight binding model from a wannier function directory.
         :param path: path
         :param prefix: prefix to the wannier files, often wannier90, or wannier90_up, or wannier90_dn for vasp.
         """
-        #tbmodel = Model.from_wannier_folder(
+        # tbmodel = Model.from_wannier_folder(
         #    folder=path, prefix=prefix)
-        #m = MyTB.from_tbmodel(tbmodel)
-        nbasis, data = parse_ham(fname=os.path.join(path, prefix + '_hr.dat'))
-        xcart, _, _ = parse_xyz(fname=os.path.join(path, prefix +
-                                                   '_centres.xyz'))
+        # m = MyTB.from_tbmodel(tbmodel)
+        nbasis, data = parse_ham(fname=os.path.join(path, prefix + "_hr.dat"))
+        xcart, _, _ = parse_xyz(fname=os.path.join(path, prefix + "_centres.xyz"))
         atoms = read(os.path.join(path, posfile))
         cell = atoms.get_cell()
         xred = cell.scaled_positions(xcart)
-        if groupby == 'orbital':
+        if groupby == "orbital":
             norb = nbasis // 2
             xtmp = np.copy(xred)
             xred[:norb] = xtmp[::2]
             xred[norb:] = xtmp[1::2]
             for key, val in data.items():
                 dtmp = copy.deepcopy(val)
                 data[key][:norb, :norb] = dtmp[::2, ::2]
@@ -199,56 +193,49 @@
         ind, positions = auto_assign_basis_name(xred, atoms)
         m = MyTB(nbasis=nbasis, data=data, positions=xred)
         nm = m.shift_position(positions)
         nm.set_atoms(atoms)
         return nm
 
     @staticmethod
-    def load_lawaf(path,
-                            prefix,
-                            posfile='POSCAR',
-                            nls=True,
-                            groupby='spin'):
+    def load_lawaf(path, prefix, posfile="POSCAR", nls=True, groupby="spin"):
         from lawaf.scdm.lwf import LWF
+
         lwf = LWF.load_nc(fname=os.path.join(path, f"{prefix}.nc"))
         nbasis = lwf.nwann
         nspin = 1
         positions = lwf.wann_centers
         ndim = lwf.ndim
         H_mnR = defaultdict(lambda: np.zeros((nbasis, nbasis), dtype=complex))
 
         for iR, R in enumerate(lwf.Rlist):
             val = lwf.HwannR[iR]
             if np.linalg.norm(R) < 0.001:
                 H_mnR[R] = val
                 H_mnR[R] -= np.diag(np.diag(val) / 2.0)
             else:
                 H_mnR[R] = lwf.HwannR[iR]
-        m = MyTB(nbasis,
-                 data=H_mnR,
-                 nspin=nspin,
-                 ndim=ndim,
-                 positions=positions)
+        m = MyTB(nbasis, data=H_mnR, nspin=nspin, ndim=ndim, positions=positions)
         m.atoms = read(posfile)
         return m
 
     def gen_ham(self, k, convention=2):
         """
         generate hamiltonian matrix at k point.
         H_k( i, j)=\sum_R H_R(i, j)^phase.
-        There are two conventions,         
+        There are two conventions,
         first:
         phase =e^{ik(R+rj-ri)}. often better used for berry phase.
         second:
         phase= e^{ikR}. We use the first convention here.
 
         :param k: kpoint
-        :param convention: 1 or 2. 
+        :param convention: 1 or 2.
         """
-        Hk = np.zeros((self.nbasis, self.nbasis), dtype='complex')
+        Hk = np.zeros((self.nbasis, self.nbasis), dtype="complex")
         if convention == 2:
             for R, mat in self.data.items():
                 phase = np.exp(self.R2kfactor * np.dot(k, R))
                 H = mat * phase
                 Hk += H + H.conjugate().T
         elif convention == 1:
             for R, mat in self.data.items():
@@ -267,33 +254,34 @@
         H = self.gen_ham(tuple(kpt), convention=convention)
         S = None
         evals, evecs = eigh(H)
         return H, S, evals, evecs
 
     def HS_and_eigen(self, kpts, convention=2):
         """
-        calculate eigens for all kpoints. 
+        calculate eigens for all kpoints.
         :param kpts: list of k points.
         """
         nk = len(kpts)
         hams = np.zeros((nk, self.nbasis, self.nbasis), dtype=complex)
         evals = np.zeros((nk, self.nbasis), dtype=float)
         evecs = np.zeros((nk, self.nbasis, self.nbasis), dtype=complex)
         for ik, k in enumerate(kpts):
             hams[ik], S, evals[ik], evecs[ik] = self.HSE_k(
-                tuple(k), convention=convention)
+                tuple(k), convention=convention
+            )
         return hams, None, evals, evecs
 
     def prepare_phase_rjri(self):
         """
         The matrix P: P(i, j) = r(j)-r(i)
         """
-        #self.rjminusri = np.zeros((self.nbasis, self.nbasis, self.ndim),
+        # self.rjminusri = np.zeros((self.nbasis, self.nbasis, self.ndim),
         #                          dtype=float)
-        #for i in range(self.nbasis):
+        # for i in range(self.nbasis):
         #    for j in range(self.nbasis):
         #        self.rjminusri[i, j] = self.xred[j] - self.xred[i]
         self.rjminusri = self.xred[None, :, :] - self.xred[:, None, :]
 
     def to_sparse(self):
         for key, val in self.data:
             self.data[key] = self._matrix(val)
@@ -351,31 +339,31 @@
         else:
             newR = R
             newmat = mat
         return newR, newmat
 
     def _to_positive_R(self):
         """
-        make all the R positive. 
+        make all the R positive.
         t(i, j, R) = t(j, i, -R).conj() if R is negative.
         """
         new_MyTB = MyTB(self.nbasis, sparse=self.sparse)
         for R, mat in self.data:
             newR, newmat = self._positive_R_mat(R, mat)
             new_MyTB[newR] += newmat
         return new_MyTB
 
     def shift_position(self, rpos):
         """
         shift the positions of basis set to near reference positions.
-        E.g. reduced position 0.8, with refernce 0.0 will goto -0.2. 
-        This can move the wannier functions to near the ions. 
+        E.g. reduced position 0.8, with refernce 0.0 will goto -0.2.
+        This can move the wannier functions to near the ions.
         """
         pos = self.positions
-        shift = np.zeros((self.nbasis, self.ndim), dtype='int')
+        shift = np.zeros((self.nbasis, self.ndim), dtype="int")
         shift[:, :] = np.round(pos - rpos)
         newpos = copy.deepcopy(pos)
         for i in range(self.nbasis):
             newpos[i] = pos[i] - shift[i]
         d = MyTB(self.nbasis, ndim=self.ndim, nspin=self.nspin)
         d._positions = newpos
 
@@ -396,79 +384,71 @@
         return d
 
     def save(self, fname):
         """
         Save model into a netcdf file.
         :param fname: filename.
         """
-        #from netCDF4 import Dataset
+        # from netCDF4 import Dataset
         # root = Dataset(fname, 'w', format="NETCDF4")
-        root = netcdf_file(fname, mode='w')
+        root = netcdf_file(fname, mode="w")
         root.createDimension("nR", self.nR)
         root.createDimension("ndim", self.ndim)
         root.createDimension("nbasis", self.nbasis)
         root.createDimension("nspin", self.nspin)
         root.createDimension("natom", len(self.atoms))
-        R = root.createVariable("R", 'i4', ("nR", "ndim"))
-        data_real = root.createVariable("data_real", 'f8',
-                                        ("nR", "nbasis", "nbasis"))
-        data_imag = root.createVariable("data_imag", 'f8',
-                                        ("nR", "nbasis", "nbasis"))
-        positions = root.createVariable("positions", 'f8', ("nbasis", "ndim"))
+        R = root.createVariable("R", "i4", ("nR", "ndim"))
+        data_real = root.createVariable("data_real", "f8", ("nR", "nbasis", "nbasis"))
+        data_imag = root.createVariable("data_imag", "f8", ("nR", "nbasis", "nbasis"))
+        positions = root.createVariable("positions", "f8", ("nbasis", "ndim"))
 
         if self.atoms is not None:
-            atom_numbers = root.createVariable("atom_numbers", 'i4',
-                                               ("natom", ))
-            atom_xred = root.createVariable("atom_xred", 'f8',
-                                            ("natom", "ndim"))
-            atom_cell = root.createVariable("atom_cell", 'f8',
-                                            ("ndim", "ndim"))
+            atom_numbers = root.createVariable("atom_numbers", "i4", ("natom",))
+            atom_xred = root.createVariable("atom_xred", "f8", ("natom", "ndim"))
+            atom_cell = root.createVariable("atom_cell", "f8", ("ndim", "ndim"))
 
-        atom_cell.unit = 'Angstrom'
+        atom_cell.unit = "Angstrom"
         positions.unit = "1"
-        data_real.unit = 'eV'
-        data_imag.unit = 'eV'
+        data_real.unit = "eV"
+        data_imag.unit = "eV"
 
         R[:] = np.array(self.Rlist)
         d = np.array(tuple(self.data.values()))
         data_real[:] = np.real(d)
         data_imag[:] = np.imag(d)
         positions[:] = np.array(self.positions)
 
         if self.atoms is not None:
             atom_numbers[:] = np.array(self.atoms.get_atomic_numbers())
-            atom_xred[:] = np.array(
-                self.atoms.get_scaled_positions(wrap=False))
+            atom_xred[:] = np.array(self.atoms.get_scaled_positions(wrap=False))
             atom_cell[:] = np.array(self.atoms.get_cell())
         root.close()
 
     @staticmethod
     def load_MyTB(fname):
         """
         Load from a netcdf file.
         :param fname: netcdf filename.
         :Returns: tight binding model.
         """
-        #from netCDF4 import Dataset
-        root = netcdf_file(fname, 'r', mmap=False)
-        nbasis = root.dimensions['nbasis']
-        nspin = root.dimensions['nspin']
-        ndim = root.dimensions['ndim']
-        natom = root.dimensions['natom']
-        Rlist = root.variables['R'][:]
-        mdata_real = root.variables['data_real'][:]
-        mdata_imag = root.variables['data_imag'][:]
-        positions = root.variables['positions'][:]
-
-        atom_numbers = root.variables['atom_numbers'][:]
-        atom_xred = root.variables['atom_xred'][:]
-        atom_cell = root.variables['atom_cell'][:]
-        atoms = Atoms(numbers=atom_numbers,
-                      scaled_positions=atom_xred,
-                      cell=atom_cell)
+        # from netCDF4 import Dataset
+        root = netcdf_file(fname, "r", mmap=False)
+        nbasis = root.dimensions["nbasis"]
+        nspin = root.dimensions["nspin"]
+        ndim = root.dimensions["ndim"]
+        natom = root.dimensions["natom"]
+        Rlist = root.variables["R"][:]
+        mdata_real = root.variables["data_real"][:]
+        mdata_imag = root.variables["data_imag"][:]
+        positions = root.variables["positions"][:]
+
+        atom_numbers = root.variables["atom_numbers"][:]
+        atom_xred = root.variables["atom_xred"][:]
+        atom_cell = root.variables["atom_cell"][:]
+        atoms = Atoms(numbers=atom_numbers, scaled_positions=atom_xred, cell=atom_cell)
         m = MyTB(nbasis, nspin=nspin, ndim=ndim, positions=positions)
         m.atoms = copy.deepcopy(atoms)
         root.close()
         for iR, R in enumerate(Rlist):
             m.data[tuple(R)] = mdata_real[iR] + mdata_imag[iR] * 1j
         return m
 
@@ -486,14 +466,15 @@
     @staticmethod
     def from_tbmodel_hdf5(fname):
         """
         load model from a hdf5 file. It uses the tbmodel parser.
         """
 
         from tbmodels import Model
+
         m = Model.from_hdf5_file(fname)
         ret = MyTB(nbasis=m.size)
         for R, v in m.hop.items():
             ret.data[R] = v
         ret.positions = np.reshape(m.pos, (m.size, m.ndim))
         return ret
 
@@ -509,43 +490,43 @@
         else:
             ret.positions = np.repeat(self.positions, 2, axis=0)
         for R, mat in self.data.items():
             if order == 1:
                 ret.data[R][::2, ::2] = mat
                 ret.data[R][1::2, 1::2] = mat
             elif order == 2:
-                ret.data[R][:self.norb, :self.norb] = mat
-                ret.data[R][self.norb:, self.norb:] = mat
+                ret.data[R][: self.norb, : self.norb] = mat
+                ret.data[R][self.norb :, self.norb :] = mat
         return ret
 
-    #def plot_band(self, kpts, color='green', show=False):
+    # def plot_band(self, kpts, color='green', show=False):
     #    evals, evecs = self.solve_all(kpts)
     #    for i in range(self.nbasis):
     #        plt.plot(evals[:, i], color=color)
     #    if show():
     #        plt.show()
 
     def validate(self):
         # make sure all R are 3d.
         for R in self.data.keys():
             if len(R) != self.ndim:
-                raise ValueError("Dimension of R should be ndim %s" %
-                                 (self.ndim))
+                raise ValueError("Dimension of R should be ndim %s" % (self.ndim))
 
 
 def merge_tbmodels_spin(tbmodel_up, tbmodel_dn):
     """
     Merge a spin up and spin down model to one spinor model.
     """
-    tbmodel = MyTB(nbasis=tbmodel_up.nbasis * 2,
-                   data=None,
-                   positions=np.vstack(
-                       [tbmodel_up.positions, tbmodel_dn.positions]),
-                   sparse=False,
-                   ndim=tbmodel_up.ndim,
-                   nspin=2,
-                   double_site_energy=2.0)
+    tbmodel = MyTB(
+        nbasis=tbmodel_up.nbasis * 2,
+        data=None,
+        positions=np.vstack([tbmodel_up.positions, tbmodel_dn.positions]),
+        sparse=False,
+        ndim=tbmodel_up.ndim,
+        nspin=2,
+        double_site_energy=2.0,
+    )
     norb = tbmodel.norb
     for R in tbmodel_up.data:
         tbmodel.data[R][:norb, :norb] = tbmodel_up.data[R][:, :]
         tbmodel.data[R][norb:, norb:] = tbmodel_dn.data[R][:, :]
     return tbmodel
```

### Comparing `lawaf-0.1.0/lawaf/wrapper/sislwrapper.py` & `lawaf-0.2.1/lawaf/wrapper/sislwrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,254 +2,247 @@
 from scipy.linalg import eigh
 from lawaf.mathutils.linalg import Lowdin
 from ase.atoms import Atoms
 from lawaf.utils.symbol import symbol_number
 from collections import defaultdict
 
 
-class SislWrapper():
+class SislWrapper:
     def __init__(self, sisl_geom, spin, ispin=None, shift_fermi=None):
-        self.shift_fermi=shift_fermi
-        self.spin=spin
+        self.shift_fermi = shift_fermi
+        self.spin = spin
         self.ispin = ispin
-        self.orbs=[]
-        self.orb_dict=defaultdict(lambda:[])
+        self.orbs = []
+        self.orb_dict = defaultdict(lambda: [])
         _atoms = sisl_geom._atoms
-        atomic_numbers=[]
+        atomic_numbers = []
         atom_positions = sisl_geom.xyz
         self.cell = np.array(sisl_geom.sc.cell)
         for ia, a in enumerate(_atoms):
             atomic_numbers.append(a.Z)
-        self.atoms = Atoms(numbers=atomic_numbers,
-                           cell=self.cell,
-                           positions=atom_positions)
-        xred=self.atoms.get_scaled_positions()
-        sdict=list(symbol_number(self.atoms).keys())
+        self.atoms = Atoms(
+            numbers=atomic_numbers, cell=self.cell, positions=atom_positions
+        )
+        xred = self.atoms.get_scaled_positions()
+        sdict = list(symbol_number(self.atoms).keys())
         if self.spin.is_colinear:
             if ispin is None:
                 raise ValueError("For colinear spin, ispin must be given")
         else:
             if ispin is not None:
                 raise ValueError(
                     "For non-colinear spin and unpolarized spin, ispin should be None"
                 )
 
-        self.positions=[]
+        self.positions = []
         if self.spin.is_colinear:
             for ia, a in enumerate(_atoms):
-                symnum=sdict[ia]
-                orb_names=[]
+                symnum = sdict[ia]
+                orb_names = []
                 for x in a.orbitals:
                     name = f"{symnum}|{x.name()}|{ispin}"
                     orb_names.append(name)
                     self.positions.append(xred[ia])
-                self.orbs+=orb_names
-                self.orb_dict[ia]+=orb_names
+                self.orbs += orb_names
+                self.orb_dict[ia] += orb_names
             self.norb = len(self.orbs)
-            self.nbasis=self.norb
+            self.nbasis = self.norb
         elif self.spin.is_spinorbit:
-            for ispin in ['up', 'down']:
+            for ispin in ["up", "down"]:
                 for ia, a in enumerate(_atoms):
-                    symnum=sdict[ia]
-                    orb_names=[]
+                    symnum = sdict[ia]
+                    orb_names = []
                     for x in a.orbitals:
-                        name=f"{symnum}|{x.name()}|{spin}"
+                        name = f"{symnum}|{x.name()}|{spin}"
                         orb_names.append(name)
                         self.positions.append(xred[ia])
-                    self.orbs+=orb_names
-                    self.orb_dict[ia]+=orb_names
-            self.norb=len(self.orbs)/2
-            self.nbasis= len(self.orbs)
+                    self.orbs += orb_names
+                    self.orb_dict[ia] += orb_names
+            self.norb = len(self.orbs) / 2
+            self.nbasis = len(self.orbs)
         else:
             for ia, a in enumerate(_atoms):
-                symnum=sdict[ia]
-                orb_names=[]
+                symnum = sdict[ia]
+                orb_names = []
                 for x in a.orbitals:
-                    name=f"{symnum}|{x.name()}|None"
+                    name = f"{symnum}|{x.name()}|None"
                     orb_names.append(name)
                     self.positions.append(xred[ia])
-                self.orbs+=orb_names
-                self.orb_dict[ia]+=orb_names
-            self.norb=len(self.orbs)
-            self.nbasis= len(self.orbs)
-        self.positions=np.array(self.positions, dtype=float)
-
+                self.orbs += orb_names
+                self.orb_dict[ia] += orb_names
+            self.norb = len(self.orbs)
+            self.nbasis = len(self.orbs)
+        self.positions = np.array(self.positions, dtype=float)
 
     def print_orbs(self):
         print(self.orb_dict)
 
     def solve_all(self, kpts):
-        """ Get eigenvalues and eigenvectors for all kpts. Should be
+        """Get eigenvalues and eigenvectors for all kpts. Should be
         implemented in children."""
         pass
 
     def get_fermi_level(self):
         if self.shift_fermi:
             return self.shift_fermi
         else:
             return 0.0
 
 
 class SislHSWrapper(SislWrapper):
-    def __init__(self,
-                 sisl_hamiltonian,
-                 ispin=None,
-                 shift_fermi=None,
-                 format='dense',
-                 nbands=10):
-
+    def __init__(
+        self, sisl_hamiltonian, ispin=None, shift_fermi=None, format="dense", nbands=10
+    ):
         self.format = format
         self.nbands = nbands
         self.ham = sisl_hamiltonian
         super().__init__(self.ham.geometry, self.ham.spin, ispin, shift_fermi)
 
     def solve(self, k):
         if self.ispin is None:
-            evals, evecs= self.ham.eigh(k=k, eigvals_only=False)
+            evals, evecs = self.ham.eigh(k=k, eigvals_only=False)
         else:
-            evals, evecs = self.ham.eigh(k=k,
-                                         spin=self.ispin,
-                                         eigvals_only=False)
+            evals, evecs = self.ham.eigh(k=k, spin=self.ispin, eigvals_only=False)
         if self.shift_fermi:
             evals += self.shift_fermi
         return evals, evecs
 
-    def Hk(self, k, format='dense'):
+    def Hk(self, k, format="dense"):
         if self.ispin is not None:
             return self.ham.Hk(k, format=format, spin=self.ispin)
         else:
             return self.ham.Hk(k, format=format)
 
     def solve_all(self, kpts, orth=False):
         evals = []
         evecs = []
         for ik, k in enumerate(kpts):
             if orth and self.ham.orthogonal:
-                S = self.ham.Sk(k, format='dense')
+                S = self.ham.Sk(k, format="dense")
                 Smh = Lowdin(S)
-                H = self.Hk(k, format='dense')
+                H = self.Hk(k, format="dense")
                 Horth = Smh.T.conj() @ H @ Smh
                 evalue, evec = eigh(Horth)
             else:
                 evalue, evec = self.solve(k)
             evals.append(evalue)
             evecs.append(evec)
-        return np.array(evals, dtype=float), np.array(evecs,
-                                                      dtype=complex,
-                                                      order='C')
+        return np.array(evals, dtype=float), np.array(evecs, dtype=complex, order="C")
 
     def get_fermi_level(self):
         if self.shift_fermi:
             return self.shift_fermi
         else:
             return 0.0
 
 
-
 class SislWFSXWrapper(SislWrapper):
-    """ Wrapper for retrieving eigenvalues and eigenvectors from siesta WFSX file
+    """Wrapper for retrieving eigenvalues and eigenvectors from siesta WFSX file
 
     Parameters
     ----------
     geom : sisl.Geometry
         the geometry containing information about atomic positions and orbitals
     wfsx_sile: sisl.io.siesta.wfsxSileSiesta
         file reader for WFSX file
-    spin : sisl.physics.Spin 
+    spin : sisl.physics.Spin
         spin object carrying information about spin configurations and spin component.
     ispin : None or int
-        index of spin channel to be considered. Only takes effect for collinear spin calculations (UP: 0, DOWN: 1). 
+        index of spin channel to be considered. Only takes effect for collinear spin calculations (UP: 0, DOWN: 1).
         (default: None)
     shift_fermi: None or float
         energy shift to be applied to all energies. If `None` no shift is applied. (default: None)
     """
+
     def __init__(self, geom, wfsx_sile, spin, ispin=None, shift_fermi=None):
         super().__init__(geom, spin=spin, ispin=ispin, shift_fermi=shift_fermi)
         self.geom = geom
         self.wfsx_sile = wfsx_sile
         self.read_all()
 
     def read_all(self):
-        """ Read all wavefunctions, eigenvalues, and k-points from WFSX file."""
+        """Read all wavefunctions, eigenvalues, and k-points from WFSX file."""
         evals = []
         evecs = []
         wfsx_kpts = []
 
         def change_gauge(k, evec):
-            """ Change the eigenvector gauge """
+            """Change the eigenvector gauge"""
             phase = np.dot(
                 self.geom.xyz[self.geom.o2a(np.arange(self.geom.no)), :],
-                np.dot(k, self.geom.rcell))
+                np.dot(k, self.geom.rcell),
+            )
             if self.spin.has_noncolinear:
                 # for NC/SOC we have a 2x2 spin-box per orbital
                 phase = np.repeat(phase, 2)
             # r -> R gauge tranformation.
             return evec * np.exp(1j * phase).reshape(1, -1)
 
         # Read wavefunctions and eigenvalues
         for wfc in self.wfsx_sile.yield_eigenstate(parent=self.geom):
-            wfsx_kpts.append(wfc.info['k'])
+            wfsx_kpts.append(wfc.info["k"])
             evals.append(wfc.c)
             # To get the same eigvecs as eigh returns we need to transpose the
             # array and change the gauge from 'r' to 'R'
-            evecs.append(change_gauge(wfc.info['k'], wfc.state).T)
+            evecs.append(change_gauge(wfc.info["k"], wfc.state).T)
 
         wfsx_kpts = np.asarray(wfsx_kpts)
 
         # If any k-point occurs more than once in the WaveFuncKPoints block,
         # we discard the duplicates
         is_duplicate = self._is_duplicate(wfsx_kpts)
         self.wfsx_kpts = wfsx_kpts[~is_duplicate]
         self.evals = np.array(evals, dtype=float)[~is_duplicate]
         if self.shift_fermi is not None:
             self.evals += self.shift_fermi
-        self.evecs = np.array(evecs, dtype=np.complex64,
-                              order='C')[~is_duplicate]
+        self.evecs = np.array(evecs, dtype=np.complex64, order="C")[~is_duplicate]
 
     def _is_duplicate(self, array):
         # TODO: Move into utils
         # Find all matches (i,j): array[i] == array[j]
         matches = np.all(np.isclose(array[None, :], array[:, None]), axis=-1)
         # Remove double counting of matches: (i,j) and (j,i)
         # Also, remove matches of elements with themselves: (i,i)
         matches = np.triu(matches, 1)
 
         # Finally determine elements which are duplicates
         return np.any(matches, axis=0)
 
     def find_all(self, kpts):
-        """ Find the correct eigenvectors and eigenvalues and sort them
+        """Find the correct eigenvectors and eigenvalues and sort them
         to match the order in kpts.
 
         Parameters
         ----------
         kpts : list of float (3,) or (nk, 3)
             list of k points
-        
+
         Returns
         -------
         evals : list of float (nk, n)
             list of eigenvalues for every requested k point
         evecs :
             list of eiegnvector for every requested k point
         """
         kpts = np.asarray(kpts)
         sort_idx = np.where(
-            np.all(np.isclose(self.wfsx_kpts[None, :], kpts[:, None]),
-                   axis=-1))[1]
+            np.all(np.isclose(self.wfsx_kpts[None, :], kpts[:, None]), axis=-1)
+        )[1]
         if len(sort_idx) < len(kpts):
             # k-point not found
             raise ValueError(
                 f"{self.__class__.__name__}._read_all unable to find at least one "
                 "required k point in '{self.wfsx_sile.file}'. Please, ensure that "
-                "all k points listed below are included:\n" +
-                "\n".join([str(k) for k in kpts]))
+                "all k points listed below are included:\n"
+                + "\n".join([str(k) for k in kpts])
+            )
         if not np.all(np.isclose(self.wfsx_kpts[sort_idx], kpts)):
             raise ValueError(
                 f"{self.__class__.__name__}._read_all was unable to match k points "
-                "in {self.wfsx_sile.file} against required kpts:" +
-                "\n".join([str(k) for k in kpts]))
+                "in {self.wfsx_sile.file} against required kpts:"
+                + "\n".join([str(k) for k in kpts])
+            )
 
         return self.evals[sort_idx], self.evecs[sort_idx]
 
     # Define alias for find_all to unify in wrapper's interface
     solve_all = find_all
```

### Comparing `lawaf-0.1.0/lawaf/wrapper/utils.py` & `lawaf-0.2.1/lawaf/wrapper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,40 +23,38 @@
 
 
 def read_basis(fname):
     """
     return basis names from file (often named as basis.txt). Return a dict. key: basis name. value: basis index, from 0
     """
     bdict = OrderedDict()
-    if fname.endswith('.win'):
+    if fname.endswith(".win"):
         with open(fname) as myfile:
             inside = False
             iline = 0
             for line in myfile.readlines():
-                if line.strip().startswith('end projections'):
+                if line.strip().startswith("end projections"):
                     inside = False
                 if inside:
-                    a = line.strip().split('#')
-                    assert len(
-                        a) == 2, "The format should be .... # label_of_basis"
+                    a = line.strip().split("#")
+                    assert len(a) == 2, "The format should be .... # label_of_basis"
                     bdict[a[-1].strip()] = iline
                     iline += 1
-                if line.strip().startswith('begin projections'):
+                if line.strip().startswith("begin projections"):
                     inside = True
     else:
         with open(fname) as myfile:
             for iline, line in enumerate(myfile.readlines()):
                 a = line.strip().split()
                 if len(a) != 0:
                     bdict[a[0]] = iline
     return bdict
 
 
-def auto_assign_wannier_to_atom(positions, atoms, max_distance=0.1,
-                                half=False):
+def auto_assign_wannier_to_atom(positions, atoms, max_distance=0.1, half=False):
     """
     assign
     half: only half of orbitals. if half, only the first half is used.
     Returns:
     ind_atoms: a list of same length of n(orb).
     """
     pos = np.array(positions)
@@ -77,18 +75,15 @@
         rpos = atompos[iatom]
         ind_atoms.append(iatom)
         refpos.append(rpos)
         newpos.append(rmin + rpos)
     return ind_atoms, newpos
 
 
-def auto_assign_wannier_to_atom2(positions,
-                                 atoms,
-                                 max_distance=0.1,
-                                 half=False):
+def auto_assign_wannier_to_atom2(positions, atoms, max_distance=0.1, half=False):
     """
     assign
     half: only half of orbitals. if half, only the first half is used.
     Returns:
     ind_atoms: a list of same length of n(orb).
     """
     porbs = positions
@@ -99,50 +94,53 @@
     patoms = atoms.get_scaled_positions()
     shifted_pos = []
     for iorb, porb in enumerate(porbs):
         distances = []
         distance_vecs = []
         for iatom, patom in enumerate(patoms):
             d = porb - patom
-            rd = np.min(
-                np.array([d % 1.0 % 1.0, (1.0 - d) % 1.0 % 1.0]), axis=0)
+            rd = np.min(np.array([d % 1.0 % 1.0, (1.0 - d) % 1.0 % 1.0]), axis=0)
             rdn = np.linalg.norm(rd)
             distance_vecs.append(rd)
             distances.append(rdn)
         iatom = np.argmin(distances)
         ind_atoms.append(iatom)
         shifted_pos.append(distance_vecs[iatom] + patoms[iatom])
         if min(distances) > max_distance:
             print(
                 "Warning: the minimal distance between wannier function No. %s is large. Check if the MLWFs are well localized."
-                % iorb)
+                % iorb
+            )
     if half:
         ind_atoms = np.vstack([ind_atoms, ind_atoms], dtype=int)
         shifted_pos = np.vstack([shifted_pos, shifted_pos], dtype=float)
     return ind_atoms, shifted_pos
 
 
-def auto_assign_basis_name(positions,
-                           atoms,
-                           max_distance=0.1,
-                           write_basis_file='assigned_basis.txt',
-                           half=False):
+def auto_assign_basis_name(
+    positions,
+    atoms,
+    max_distance=0.1,
+    write_basis_file="assigned_basis.txt",
+    half=False,
+):
     ind_atoms, shifted_pos = auto_assign_wannier_to_atom(
-        positions=positions, atoms=atoms, max_distance=max_distance, half=half)
+        positions=positions, atoms=atoms, max_distance=max_distance, half=half
+    )
     basis_dict = {}
     a = defaultdict(int)
     symdict = symbol_number(atoms)
     syms = list(symdict.keys())
     for i, iatom in enumerate(ind_atoms):
         a[iatom] = a[iatom] + 1
-        basis_dict['%s|orb_%d' % (syms[iatom], a[iatom])] = i + 1
+        basis_dict["%s|orb_%d" % (syms[iatom], a[iatom])] = i + 1
     if write_basis_file is not None:
-        with open(write_basis_file, 'w') as myfile:
+        with open(write_basis_file, "w") as myfile:
             for key, val in basis_dict.items():
-                myfile.write('%s  %d \n' % (key, val))
+                myfile.write("%s  %d \n" % (key, val))
     return basis_dict, shifted_pos
 
 
 def shift_positions(p, pref):
     return p - np.round(p - pref)
 
 
@@ -208,23 +206,24 @@
 
 def match_kq_mesh(klist, qlist):
     """
     return a table of (iq, ik): i(k+q)
     """
     nk = len(klist)
     nq = len(qlist)
-    ret = np.zeros((nq, nk), dtype='int')
+    ret = np.zeros((nq, nk), dtype="int")
     for iq, q in enumerate(qlist):
         for ik, k in enumerate(klist):
             ikq, kshift = match_k(k + q, klist)
             ret[iq, ik] = ikq
     return ret
 
 
-
 def kmesh_to_R(kmesh):
     k1, k2, k3 = kmesh
-    Rlist = [(R1, R2, R3) for R1 in range(-k1 // 2 + 1, k1 // 2 + 1)
-             for R2 in range(-k2 // 2 + 1, k2 // 2 + 1)
-             for R3 in range(-k3 // 2 + 1, k3 // 2 + 1)]
+    Rlist = [
+        (R1, R2, R3)
+        for R1 in range(-k1 // 2 + 1, k1 // 2 + 1)
+        for R2 in range(-k2 // 2 + 1, k2 // 2 + 1)
+        for R3 in range(-k3 // 2 + 1, k3 // 2 + 1)
+    ]
     return Rlist
-
```

### Comparing `lawaf-0.1.0/lawaf/wrapper/w90_parser.py` & `lawaf-0.2.1/lawaf/wrapper/w90_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,80 +10,77 @@
     atoms = read(fname)
     symbols = atoms.get_chemical_symbols()
     pos = atoms.get_positions()
     wann_pos = []
     atoms_pos = []
     atoms_symbols = []
     for s, x in zip(symbols, pos):
-        if s == 'X':
+        if s == "X":
             wann_pos.append(x)
         else:
             atoms_symbols.append(s)
             atoms_pos.append(x)
     return np.array(wann_pos), atoms_symbols, np.array(atoms_pos)
 
 
 def remove_comment(line: str):
-    x = re.split('!|#', line)[0]
+    x = re.split("!|#", line)[0]
     return x
 
 
 def parse_win(fname):
     """
     read atomic structure from .win file
     """
     cell = []
     xcart = []
     xred = []
     symbols = []
     with open(fname) as myfile:
         for line in myfile:
             line = remove_comment(line)
-            if re.match('begin\s+unit_cell_cart', line):
-                while (not re.match('end\s+unit_cell_cart', line)):
+            if re.match("begin\s+unit_cell_cart", line):
+                while not re.match("end\s+unit_cell_cart", line):
                     line = remove_comment(next(myfile))
                     ts = line.split()
                     if len(ts) == 3:
                         cell.append([float(x) for x in ts])
-            elif re.match('begin\s+atoms_cart', line):
-                while (not re.match('end\s+atoms_cart', line)):
+            elif re.match("begin\s+atoms_cart", line):
+                while not re.match("end\s+atoms_cart", line):
                     line = remove_comment(next(myfile))
                     ts = line.split()
                     if len(ts) == 4:
                         symbols.append(ts[0])
                         xcart.append([float(x) for x in ts[1:]])
-            elif re.match('begin\s+atoms_frac', line):
-                while (not re.match('end\s+atoms_frac', line)):
+            elif re.match("begin\s+atoms_frac", line):
+                while not re.match("end\s+atoms_frac", line):
                     line = remove_comment(next(myfile))
                     ts = line.split()
                     if len(ts) == 4:
                         symbols.append(ts[0])
                         xred.append([float(x) for x in ts[1:]])
 
     cell = np.array(cell)
     xcart = np.array(xcart)
     if xcart != []:
         atoms = Atoms(symbols=symbols, positions=xcart, cell=cell, pbc=True)
     elif xred != []:
-        atoms = Atoms(symbols=symbols,
-                      scaled_positions=xred,
-                      cell=cell,
-                      pbc=True)
+        atoms = Atoms(symbols=symbols, scaled_positions=xred, cell=cell, pbc=True)
     else:
         raise IOError("Failed to read atomic structure from %s" % fname)
     return atoms
 
 
-def parse_ham(fname='wannier90_hr.dat', cutoff=None):
+def parse_ham(fname="wannier90_hr.dat", cutoff=None):
     """
     wannier90 hr file phaser.
 
     :param cutoff: the energy cutoff.  None | number | list (of Emin, Emax).
     """
-    with open(fname, 'r') as myfile:
+    with open(fname, "r") as myfile:
         lines = myfile.readlines()
     n_wann = int(lines[1].strip())
     n_R = int(lines[2].strip())
 
     # The lines of degeneracy of each R point. 15 per line.
     nline = int(math.ceil(n_R / 15.0))
     dlist = []
@@ -95,26 +92,25 @@
         t = lines[i].strip().split()
         R = tuple(map(int, t[:3]))
         m, n = map(int, t[3:5])
         m = m - 1
         n = n - 1
         H_real, H_imag = map(float, t[5:])
         val = H_real + 1j * H_imag
-        if (m == n and np.linalg.norm(R) < 0.001):
+        if m == n and np.linalg.norm(R) < 0.001:
             H_mnR[R][m, n] = val / 2.0
         elif cutoff is not None:
             if abs(val) > cutoff:
                 H_mnR[R][m, n] = val
         else:
             H_mnR[R][m, n] = val / 2.0
     return n_wann, H_mnR
 
 
-def auto_assign_wannier_to_atom(positions, atoms, max_distance=0.1,
-                                half=False):
+def auto_assign_wannier_to_atom(positions, atoms, max_distance=0.1, half=False):
     """
     assign
     half: only half of orbitals. if half, only the first half is used.
     Returns:
     ind_atoms: a list of same length of n(orb).
     """
     pos = np.array(positions)
@@ -133,8 +129,7 @@
         # ref+residual
         rmin = r[iatom]
         rpos = atompos[iatom]
         ind_atoms.append(iatom)
         refpos.append(rpos)
         newpos.append(rmin + rpos)
     return ind_atoms, newpos
-
```

### Comparing `lawaf-0.1.0/lawaf.egg-info/PKG-INFO` & `lawaf-0.2.1/lawaf.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: lawaf
-Version: 0.1.0
+Version: 0.2.1
 Summary: A library for constructing Lattice and other Wannier functions 
-Author: Xu He
 Author-email: Xu He <mailhexu@gmail.com>
 License: BSD-2
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: scipy>=1.7.0
 Requires-Dist: sisl>=0.9.0
-Requires-Dist: HamiltonIO>=0.1.0
+Requires-Dist: HamiltonIO>=0.1.2
 Requires-Dist: matplotlib>=3.4.0
 Requires-Dist: ase>=3.19
 Requires-Dist: phonopy>=2.11.0
+Requires-Dist: toml
 Provides-Extra: test
 Requires-Dist: pytest>=6.2.0; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pytest>=6.2.0; extra == "dev"
 Requires-Dist: black>=21.6b0; extra == "dev"
 Requires-Dist: pre-commit>=2.13.0; extra == "dev"
 Requires-Dist: sphinx>=4.1.2; extra == "dev"
```

### Comparing `lawaf-0.1.0/pyproject.toml` & `lawaf-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [project]
 name = "lawaf"
-version = "0.1.0"
+version = "0.2.1"
 description = "A library for constructing Lattice and other Wannier functions "
 authors = [
     {name = "Xu He", email = "mailhexu@gmail.com"},
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 license = {text = "BSD-2"}
 dependencies = [
     "numpy>=1.21.0",
     "scipy>=1.7.0",
     "sisl>=0.9.0",
-    "HamiltonIO>=0.1.0",
+    "HamiltonIO>=0.1.2",
     "matplotlib>=3.4.0",
     "ase>=3.19",
     "phonopy>=2.11.0",
+    "toml",
 ]
 	
 
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
```

