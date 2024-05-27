# Comparing `tmp/sage_lib-0.1.5.3.tar.gz` & `tmp/sage_lib-0.1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sage_lib-0.1.5.3.tar", last modified: Tue May 21 16:03:15 2024, max compression
+gzip compressed data, was "sage_lib-0.1.5.4.tar", last modified: Mon May 27 11:21:32 2024, max compression
```

## Comparing `sage_lib-0.1.5.3.tar` & `sage_lib-0.1.5.4.tar`

### file list

```diff
@@ -1,100 +1,102 @@
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.126714 sage_lib-0.1.5.3/
--rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-21 16:03:15.126521 sage_lib-0.1.5.3/PKG-INFO
--rw-rw-r--   0 dimitry    (501) staff       (20)        7 2023-11-24 15:31:44.000000 sage_lib-0.1.5.3/README.md
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.103764 sage_lib-0.1.5.3/sage_lib/
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.108462 sage_lib-0.1.5.3/sage_lib/IO/
--rw-rw-r--   0 dimitry    (501) staff       (20)     5213 2023-11-26 10:15:10.000000 sage_lib-0.1.5.3/sage_lib/IO/BashScriptManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4088 2023-11-26 10:15:54.000000 sage_lib-0.1.5.3/sage_lib/IO/BinaryDataHandler.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3145 2023-11-26 10:15:38.000000 sage_lib-0.1.5.3/sage_lib/IO/ChargeFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6402 2023-11-30 08:47:00.000000 sage_lib-0.1.5.3/sage_lib/IO/DOSManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     9400 2023-11-30 16:58:50.000000 sage_lib-0.1.5.3/sage_lib/IO/EigenvalueFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      559 2023-11-26 11:22:04.000000 sage_lib-0.1.5.3/sage_lib/IO/ForceFieldManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     8862 2023-11-30 09:14:10.000000 sage_lib-0.1.5.3/sage_lib/IO/KPointsManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    17982 2024-05-14 11:48:21.000000 sage_lib-0.1.5.3/sage_lib/IO/OutFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5292 2023-11-26 10:15:38.000000 sage_lib-0.1.5.3/sage_lib/IO/PROFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     8151 2023-11-26 10:16:36.000000 sage_lib-0.1.5.3/sage_lib/IO/PotentialManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2756 2023-11-26 10:15:40.000000 sage_lib-0.1.5.3/sage_lib/IO/WaveFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/IO/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.110196 sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/
--rw-rw-r--   0 dimitry    (501) staff       (20)      609 2024-01-17 11:45:45.000000 sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/InputClassic.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24368 2024-01-17 11:45:39.000000 sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/InputDFT.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1168 2024-01-17 11:45:21.000000 sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/InputFile.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      873 2023-11-26 10:17:02.000000 sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/InputFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.112903 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/
--rw-rw-r--   0 dimitry    (501) staff       (20)     2622 2024-01-17 11:44:29.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPosition.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5789 2024-05-21 15:53:34.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5924 2023-12-29 02:33:08.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24115 2024-05-21 15:51:02.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPositionManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    47828 2024-04-29 15:23:19.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      666 2024-01-30 15:22:44.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    31224 2024-05-02 06:40:23.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/PeriodicSystem.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    10187 2024-01-25 08:34:17.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/plot.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.115824 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/
--rw-rw-r--   0 dimitry    (501) staff       (20)     5733 2023-12-12 15:25:04.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4702 2023-12-18 08:26:38.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3458 2023-11-28 08:43:18.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
--rw-r--r--   0 dimitry    (501) staff       (20)     8851 2024-05-21 15:56:27.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6036 2024-01-17 16:13:47.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
--rw-r--r--   0 dimitry    (501) staff       (20)    12680 2024-05-21 15:56:28.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/LAMMPS.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     7960 2024-04-03 12:15:20.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5328 2024-05-16 15:26:28.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2583 2023-11-28 07:46:02.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12012 2024-04-29 15:28:10.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5409 2024-01-17 14:07:15.000000 sage_lib-0.1.5.3/sage_lib/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.116618 sage_lib-0.1.5.3/sage_lib/descriptor/
--rw-rw-r--   0 dimitry    (501) staff       (20)    22605 2024-01-30 14:35:03.000000 sage_lib-0.1.5.3/sage_lib/descriptor/MBTR.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12332 2024-01-26 13:40:44.000000 sage_lib-0.1.5.3/sage_lib/descriptor/MDTR_rev.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/descriptor/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.117736 sage_lib-0.1.5.3/sage_lib/ensemble/
--rw-rw-r--   0 dimitry    (501) staff       (20)      723 2023-11-30 08:05:18.000000 sage_lib-0.1.5.3/sage_lib/ensemble/DFTEnsemble.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1943 2023-11-30 08:04:04.000000 sage_lib-0.1.5.3/sage_lib/ensemble/FFEnsembleManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/ensemble/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    60980 2024-05-21 15:52:17.000000 sage_lib-0.1.5.3/sage_lib/main.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.118744 sage_lib-0.1.5.3/sage_lib/master/
--rw-rw-r--   0 dimitry    (501) staff       (20)    56879 2024-05-16 12:31:55.000000 sage_lib-0.1.5.3/sage_lib/master/AtomicProperties.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12849 2024-05-16 15:37:20.000000 sage_lib-0.1.5.3/sage_lib/master/FileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/master/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.119626 sage_lib-0.1.5.3/sage_lib/miscellaneous/
--rw-rw-r--   0 dimitry    (501) staff       (20)     7176 2024-01-17 14:09:09.000000 sage_lib-0.1.5.3/sage_lib/miscellaneous/BandPathGenerator.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24192 2024-03-27 14:48:16.000000 sage_lib-0.1.5.3/sage_lib/miscellaneous/MD_tools.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/miscellaneous/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    22279 2024-01-31 09:07:23.000000 sage_lib-0.1.5.3/sage_lib/miscellaneous/periodic_kdtree.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.120429 sage_lib-0.1.5.3/sage_lib/partition/
--rw-rw-r--   0 dimitry    (501) staff       (20)    18091 2024-03-31 12:51:40.000000 sage_lib-0.1.5.3/sage_lib/partition/Partition.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    28251 2024-05-16 15:06:54.000000 sage_lib-0.1.5.3/sage_lib/partition/PartitionManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/partition/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.124933 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/
--rw-rw-r--   0 dimitry    (501) staff       (20)     7189 2024-02-23 12:29:06.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2503 2023-11-26 11:03:08.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/BandStructure_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24419 2024-04-30 06:33:56.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Blender_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    11799 2024-04-15 15:59:15.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Config_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    11764 2024-01-30 14:29:29.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/CrystalDefect_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      614 2023-11-26 10:15:36.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Crystal_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2714 2024-02-28 10:50:31.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Dataset_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    14023 2024-02-28 09:01:31.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Filter_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    35233 2024-05-02 11:31:03.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/MolecularDynamic_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    13519 2024-03-15 18:00:18.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/MoleculeCluster_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3669 2024-01-17 14:10:13.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Molecule_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4199 2024-04-02 14:56:25.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/PositionEditor_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    11331 2024-01-17 14:16:35.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5375 2023-11-26 12:34:42.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/SurfaceStates_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6358 2024-02-23 08:00:39.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/VacuumStates_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/partition/partition_builder/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.126001 sage_lib-0.1.5.3/sage_lib/single_run/
--rw-rw-r--   0 dimitry    (501) staff       (20)     6596 2023-11-24 15:31:44.000000 sage_lib-0.1.5.3/sage_lib/single_run/FF_Gap.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1803 2024-01-17 15:01:44.000000 sage_lib-0.1.5.3/sage_lib/single_run/SingleRun.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    13356 2024-03-12 14:35:36.000000 sage_lib-0.1.5.3/sage_lib/single_run/SingleRunDFT.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3098 2024-01-17 14:12:18.000000 sage_lib-0.1.5.3/sage_lib/single_run/SingleRunManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.3/sage_lib/single_run/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-21 16:03:15.126166 sage_lib-0.1.5.3/sage_lib.egg-info/
--rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-21 16:03:15.000000 sage_lib-0.1.5.3/sage_lib.egg-info/PKG-INFO
--rw-rw-r--   0 dimitry    (501) staff       (20)     3797 2024-05-21 16:03:15.000000 sage_lib-0.1.5.3/sage_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)        1 2024-05-21 16:03:15.000000 sage_lib-0.1.5.3/sage_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)       44 2024-05-21 16:03:15.000000 sage_lib-0.1.5.3/sage_lib.egg-info/entry_points.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)       23 2024-05-21 16:03:15.000000 sage_lib-0.1.5.3/sage_lib.egg-info/requires.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)        9 2024-05-21 16:03:15.000000 sage_lib-0.1.5.3/sage_lib.egg-info/top_level.txt
--rw-r--r--   0 dimitry    (501) staff       (20)       38 2024-05-21 16:03:15.126761 sage_lib-0.1.5.3/setup.cfg
--rw-rw-r--   0 dimitry    (501) staff       (20)      394 2024-05-21 16:00:25.000000 sage_lib-0.1.5.3/setup.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.648360 sage_lib-0.1.5.4/
+-rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-27 11:21:32.648155 sage_lib-0.1.5.4/PKG-INFO
+-rw-rw-r--   0 dimitry    (501) staff       (20)        7 2023-11-24 15:31:44.000000 sage_lib-0.1.5.4/README.md
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.626533 sage_lib-0.1.5.4/sage_lib/
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.630271 sage_lib-0.1.5.4/sage_lib/IO/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5213 2023-11-26 10:15:10.000000 sage_lib-0.1.5.4/sage_lib/IO/BashScriptManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4088 2023-11-26 10:15:54.000000 sage_lib-0.1.5.4/sage_lib/IO/BinaryDataHandler.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3145 2023-11-26 10:15:38.000000 sage_lib-0.1.5.4/sage_lib/IO/ChargeFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6402 2023-11-30 08:47:00.000000 sage_lib-0.1.5.4/sage_lib/IO/DOSManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     9400 2023-11-30 16:58:50.000000 sage_lib-0.1.5.4/sage_lib/IO/EigenvalueFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      559 2023-11-26 11:22:04.000000 sage_lib-0.1.5.4/sage_lib/IO/ForceFieldManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     8862 2023-11-30 09:14:10.000000 sage_lib-0.1.5.4/sage_lib/IO/KPointsManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    17982 2024-05-14 11:48:21.000000 sage_lib-0.1.5.4/sage_lib/IO/OutFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5292 2023-11-26 10:15:38.000000 sage_lib-0.1.5.4/sage_lib/IO/PROFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     8151 2023-11-26 10:16:36.000000 sage_lib-0.1.5.4/sage_lib/IO/PotentialManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2756 2023-11-26 10:15:40.000000 sage_lib-0.1.5.4/sage_lib/IO/WaveFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/IO/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.631574 sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/
+-rw-rw-r--   0 dimitry    (501) staff       (20)      609 2024-01-17 11:45:45.000000 sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/InputClassic.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24368 2024-01-17 11:45:39.000000 sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/InputDFT.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1168 2024-01-17 11:45:21.000000 sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/InputFile.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      873 2023-11-26 10:17:02.000000 sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/InputFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.634356 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2622 2024-01-17 11:44:29.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPosition.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5789 2024-05-21 15:53:34.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6242 2024-05-24 12:11:00.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24117 2024-05-27 10:02:52.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPositionManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    47824 2024-05-27 11:11:25.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      666 2024-01-30 15:22:44.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    32829 2024-05-22 08:19:10.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/PeriodicSystem.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    10187 2024-01-25 08:34:17.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/plot.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.637608 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5733 2023-12-12 15:25:04.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4702 2023-12-18 08:26:38.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3458 2023-11-28 08:43:18.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
+-rw-r--r--   0 dimitry    (501) staff       (20)     8851 2024-05-21 15:56:27.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6036 2024-01-17 16:13:47.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
+-rw-r--r--   0 dimitry    (501) staff       (20)    12682 2024-05-22 08:19:13.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/LAMMPS.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7960 2024-04-03 12:15:20.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5328 2024-05-16 15:26:28.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2583 2023-11-28 07:46:02.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12012 2024-04-29 15:28:10.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5409 2024-01-17 14:07:15.000000 sage_lib-0.1.5.4/sage_lib/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.638464 sage_lib-0.1.5.4/sage_lib/descriptor/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    22605 2024-01-30 14:35:03.000000 sage_lib-0.1.5.4/sage_lib/descriptor/MBTR.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12332 2024-01-26 13:40:44.000000 sage_lib-0.1.5.4/sage_lib/descriptor/MDTR_rev.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/descriptor/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.639216 sage_lib-0.1.5.4/sage_lib/ensemble/
+-rw-rw-r--   0 dimitry    (501) staff       (20)      723 2023-11-30 08:05:18.000000 sage_lib-0.1.5.4/sage_lib/ensemble/DFTEnsemble.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1943 2023-11-30 08:04:04.000000 sage_lib-0.1.5.4/sage_lib/ensemble/FFEnsembleManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/ensemble/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    63292 2024-05-24 08:50:37.000000 sage_lib-0.1.5.4/sage_lib/main.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    60371 2024-05-26 18:50:36.000000 sage_lib-0.1.5.4/sage_lib/main2.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    63292 2024-05-24 08:50:37.000000 sage_lib-0.1.5.4/sage_lib/main_rev.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.640139 sage_lib-0.1.5.4/sage_lib/master/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    56879 2024-05-16 12:31:55.000000 sage_lib-0.1.5.4/sage_lib/master/AtomicProperties.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12849 2024-05-16 15:37:20.000000 sage_lib-0.1.5.4/sage_lib/master/FileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/master/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.640993 sage_lib-0.1.5.4/sage_lib/miscellaneous/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7176 2024-01-17 14:09:09.000000 sage_lib-0.1.5.4/sage_lib/miscellaneous/BandPathGenerator.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24192 2024-03-27 14:48:16.000000 sage_lib-0.1.5.4/sage_lib/miscellaneous/MD_tools.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/miscellaneous/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    22279 2024-01-31 09:07:23.000000 sage_lib-0.1.5.4/sage_lib/miscellaneous/periodic_kdtree.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.641775 sage_lib-0.1.5.4/sage_lib/partition/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    18094 2024-05-22 09:47:50.000000 sage_lib-0.1.5.4/sage_lib/partition/Partition.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    28251 2024-05-27 11:12:35.000000 sage_lib-0.1.5.4/sage_lib/partition/PartitionManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/partition/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.646734 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7189 2024-02-23 12:29:06.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2503 2023-11-26 11:03:08.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/BandStructure_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24419 2024-04-30 06:33:56.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Blender_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    11799 2024-04-15 15:59:15.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Config_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    23321 2024-05-27 11:18:25.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/CrystalDefect_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      614 2023-11-26 10:15:36.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Crystal_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2714 2024-02-28 10:50:31.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Dataset_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    14023 2024-02-28 09:01:31.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Filter_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    35233 2024-05-02 11:31:03.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/MolecularDynamic_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    15646 2024-05-24 14:03:21.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/MoleculeCluster_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3669 2024-01-17 14:10:13.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Molecule_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4199 2024-04-02 14:56:25.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/PositionEditor_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    11331 2024-01-17 14:16:35.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5375 2023-11-26 12:34:42.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/SurfaceStates_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6358 2024-02-23 08:00:39.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/VacuumStates_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/partition/partition_builder/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.647808 sage_lib-0.1.5.4/sage_lib/single_run/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6596 2023-11-24 15:31:44.000000 sage_lib-0.1.5.4/sage_lib/single_run/FF_Gap.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1803 2024-01-17 15:01:44.000000 sage_lib-0.1.5.4/sage_lib/single_run/SingleRun.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    13356 2024-03-12 14:35:36.000000 sage_lib-0.1.5.4/sage_lib/single_run/SingleRunDFT.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3098 2024-01-17 14:12:18.000000 sage_lib-0.1.5.4/sage_lib/single_run/SingleRunManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.4/sage_lib/single_run/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-27 11:21:32.647945 sage_lib-0.1.5.4/sage_lib.egg-info/
+-rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-27 11:21:32.000000 sage_lib-0.1.5.4/sage_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3836 2024-05-27 11:21:32.000000 sage_lib-0.1.5.4/sage_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)        1 2024-05-27 11:21:32.000000 sage_lib-0.1.5.4/sage_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)       44 2024-05-27 11:21:32.000000 sage_lib-0.1.5.4/sage_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)       23 2024-05-27 11:21:32.000000 sage_lib-0.1.5.4/sage_lib.egg-info/requires.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)        9 2024-05-27 11:21:32.000000 sage_lib-0.1.5.4/sage_lib.egg-info/top_level.txt
+-rw-r--r--   0 dimitry    (501) staff       (20)       38 2024-05-27 11:21:32.648406 sage_lib-0.1.5.4/setup.cfg
+-rw-rw-r--   0 dimitry    (501) staff       (20)      394 2024-05-27 11:19:11.000000 sage_lib-0.1.5.4/setup.py
```

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/BashScriptManager.py` & `sage_lib-0.1.5.4/sage_lib/IO/BashScriptManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/BinaryDataHandler.py` & `sage_lib-0.1.5.4/sage_lib/IO/BinaryDataHandler.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/ChargeFileManager.py` & `sage_lib-0.1.5.4/sage_lib/IO/ChargeFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/DOSManager.py` & `sage_lib-0.1.5.4/sage_lib/IO/DOSManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/EigenvalueFileManager.py` & `sage_lib-0.1.5.4/sage_lib/IO/EigenvalueFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/ForceFieldManager.py` & `sage_lib-0.1.5.4/sage_lib/IO/ForceFieldManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/KPointsManager.py` & `sage_lib-0.1.5.4/sage_lib/IO/KPointsManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/OutFileManager.py` & `sage_lib-0.1.5.4/sage_lib/IO/OutFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/PROFileManager.py` & `sage_lib-0.1.5.4/sage_lib/IO/PROFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/PotentialManager.py` & `sage_lib-0.1.5.4/sage_lib/IO/PotentialManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/WaveFileManager.py` & `sage_lib-0.1.5.4/sage_lib/IO/WaveFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/InputClassic.py` & `sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/InputClassic.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/InputDFT.py` & `sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/InputDFT.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/InputFile.py` & `sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/InputFile.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/input_handling_tools/InputFileManager.py` & `sage_lib-0.1.5.4/sage_lib/IO/input_handling_tools/InputFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPosition.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPosition.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         Args:
             file_location (str, optional): The location of a file containing molecular data.
             name (str, optional): The name of the molecule.
 
         The class also accepts additional keyword arguments (**kwargs) for future extensions.
         """
 
+        self._atomic_compounds = { f'{a}':  {'atomLabels': [f'{a}' ],   'atomPositions': [[0, 0, 0]]} for a in self.atomic_numbers }
+
         self._diatomic_compounds = {
             'H2':  {'atomLabels': ['H', 'H'],   'atomPositions': [[0, 0, 0], [0, 0,  .62]]},
             'O2':  {'atomLabels': ['O', 'O'],   'atomPositions': [[0, 0, 0], [0, 0, 1.32]]},
             'N2':  {'atomLabels': ['N', 'N'],   'atomPositions': [[0, 0, 0], [0, 0, 1.42]]},
             'F2':  {'atomLabels': ['F', 'F'],   'atomPositions': [[0, 0, 0], [0, 0, 1.14]]},
             'Cl2': {'atomLabels': ['Cl', 'Cl'], 'atomPositions': [[0, 0, 0], [0, 0, 2.04]]},
             'Br2': {'atomLabels': ['Br', 'Br'], 'atomPositions': [[0, 0, 0], [0, 0, 2.40]]},
@@ -99,14 +101,19 @@
         Builds a molecule based on the given name.
 
         Args:
             name (str): The name of the molecule to be built.
 
         This method looks up the molecule's structure from predefined compounds and constructs it.
         """
+
+        if name in self.atomic_compounds:
+            atomLabels = self.atomic_compounds[name]['atomLabels']
+            atomPositions = self.atomic_compounds[name]['atomPositions']
+
         if name in self.diatomic_compounds:
             atomLabels = self.diatomic_compounds[name]['atomLabels']
             atomPositions = self.diatomic_compounds[name]['atomPositions']
 
         if name in self.triatomic_compounds:
             atomLabels = self.triatomic_compounds[name]['atomLabels']
             atomPositions = self.triatomic_compounds[name]['atomPositions']
```

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPositionManager.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPositionManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -576,14 +576,16 @@
         if metric == 'metric':
             self._graph_representation = MBTR.find_related_atoms_groups(self.similarity_matrix, threshold=0.82)
         elif metric == 'kdtree':
             self._graph_representation = self.get_molecular_graph(sigma=1.0, metric='kdtree')
 
         return self._graph_representation
 
+
+
         '''
     def calculate_rms_displacement_in_angstrom(atomic_mass_amu, temperature, frequency_au=1.0):
         """
         Calculate the root-mean-square displacement of an atom in a harmonic potential in Ångströms.
 
         Parameters:
         atomic_mass_amu (float): Atomic mass of the element in atomic mass units (amu).
```

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,15 +501,15 @@
         save substantial amounts of time by putting them in a
         PeriodicCKDTree and using query_ball_tree.
         """
         return self.kdtree.query_ball_point(x, r, p=2., eps=0)
 
     def find_n_closest_neighbors(self, r, n:int, kdtree:bool=True, eps:int=0, p:int=2, distance_upper_bound:float=np.inf):
         if kdtree:
-            return self.kdtree.query(x=r, k=n, eps=eps, p=p, distance_upper_bound=distance_upper_bound.inf)
+            return self.kdtree.query(x=r, k=n, eps=eps, p=p, distance_upper_bound=distance_upper_bound)
         else:
             return self.find_n_closest_neighbors_distance(r, n)
 
     def find_n_closest_neighbors_distance(self, r, n):
         """Find the n closest neighbors to a given atom."""
         #distance_matrix = self.distanceamtrix
         #distances = distance_matrix[atom_index]
```

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/PeriodicSystem.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/PeriodicSystem.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         Additional inherited attributes from AtomPositionManager.
     """
     
     def __init__(self, file_location:str=None, name:str=None, **kwargs):
         super().__init__(name=name, file_location=file_location)
         self._reciprocalLatticeVectors = None # [b1, b2, b3]
         self._latticeVectors = None # [a1,a2,a3]
+        self._triclinic_box = None
         self._latticeVectors_inv = None # [a1,a2,a3]
 
         self._symmetryEquivPositions = None
         self._atomCoordinateType = None  # str cartedian direct
         self._latticeParameters = None # [] latticeParameters
         self._latticeAngles = None  # [alpha, beta, gamma]
         self._cellVolumen = None  # float
@@ -256,14 +257,53 @@
         elif self._latticeVectors is not None:
             self._latticeParameters = np.linalg.norm(self.latticeVectors, axis=1)
             return self._latticeParameters
         else:
             return None
 
     @property
+    def triclinic_box(self):   
+        if '_latticeVectors' not in self.__dict__ or '_latticeParameters' not in self.__dict__:
+            raise AttributeError("Attributes _latticeParameters and _latticeParameters must be initialized before accessing latticeParameters.")
+        elif self._latticeVectors is not None:
+            self._triclinic_box = self.latticeVectors_2_triclinic_box(self.latticeVectors)
+            return self._triclinic_box
+        else:
+            return None
+
+    def latticeVectors_2_triclinic_box(self, lattice_vectors: np.ndarray) -> list:
+        """
+        Transforms VASP lattice vectors to LAMMPS triclinic box bounds.
+
+        Parameters:
+            lattice_vectors (np.ndarray): 3x3 matrix representing the lattice vectors for VASP.
+        
+        Returns:
+            list: List representing the box bounds in LAMMPS.
+                  It includes (xlo, xhi), (ylo, yhi), (zlo, zhi), xy, xz, yz.
+        """
+        if lattice_vectors.shape != (3, 3):
+            raise ValueError("lattice_vectors must be a 3x3 matrix")
+        
+        # Extracting lattice vectors
+        a1, a2, a3 = lattice_vectors
+        
+        # Calculating box bounds
+        xlo, xhi = 0.0, np.linalg.norm(a1)
+        xy = np.dot(a1, a2) / xhi
+
+        ylo, yhi = 0.0, np.sqrt(np.linalg.norm(a2)**2 - xy**2)
+
+        xz = np.dot(a1, a3) / xhi
+        yz = (np.dot(a2, a3) - xy * xz) / yhi
+        zlo, zhi = 0.0, np.sqrt(np.linalg.norm(a3)**2 - xz**2 - yz**2)
+        
+        return [(xlo, xhi), (ylo, yhi), (zlo, zhi), xy, xz, yz]
+
+    @property
     def cellVolumen(self):
         if '_cellVolumen' not in self.__dict__ or '_cellVolumen' not in self.__dict__:
             raise AttributeError("Attributes _cellVolumen and _cellVolumen must be initialized before accessing cellVolumen.")
         elif not self._cellVolumen is None: 
             return  self._cellVolumen 
         elif self.latticeParameters is not None or self.latticeAngles is not None:
             a, b, c = self.latticeParameters
```

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/plot.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/plot.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/DUMP.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/LAMMPS.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/LAMMPS.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         # Calculating box bounds
         xlo, xhi = 0.0, a1[0]
         ylo, yhi = 0.0, a2[1]
         zlo, zhi = 0.0, a3[2]
         
         return [(xlo, xhi), (ylo, yhi), (zlo, zhi)]
 
-    def read_DUMP(self, file_location: str = None, lines: list = None, verbose: bool = False) -> dict:
+    def read_LAMMPS(self, file_location: str = None, lines: list = None, verbose: bool = False) -> dict:
         """
         Reads a single timestep configuration from a LAMMPS dump file.
 
         Parameters:
             file_location (str, optional): Location of the dump file. Defaults to instance file location if None.
             lines (list, optional): List of lines from the dump file. If None, reads from file.
             verbose (bool, optional): If True, prints additional information. Defaults to False.
```

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py` & `sage_lib-0.1.5.4/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/__init__.py` & `sage_lib-0.1.5.4/sage_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/descriptor/MBTR.py` & `sage_lib-0.1.5.4/sage_lib/descriptor/MBTR.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/descriptor/MDTR_rev.py` & `sage_lib-0.1.5.4/sage_lib/descriptor/MDTR_rev.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/ensemble/DFTEnsemble.py` & `sage_lib-0.1.5.4/sage_lib/ensemble/DFTEnsemble.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/ensemble/FFEnsembleManager.py` & `sage_lib-0.1.5.4/sage_lib/ensemble/FFEnsembleManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/main.py` & `sage_lib-0.1.5.4/sage_lib/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 from sage_lib.partition.Partition import Partition 
 from sage_lib.IO.structure_handling_tools.AtomPosition import AtomPosition 
 from sage_lib.IO.EigenvalueFileManager import EigenvalueFileManager 
 from sage_lib.IO.DOSManager import DOSManager 
 
 from sage_lib.IO.OutFileManager import OutFileManager 
 
-def generate_defects(path:str, source:str=None, forces_tag:str=None, energy_tag:str=None, subfolders:bool=False, output_path:str=None, 
-                    verbose:bool=False, conteiner_index:int=None,
-                    species:list=None, new_species:list=None, defect:str=None):
+def generate_defects(path:str, source:str=None, forces_tag:str=None, energy_tag:str=None, subfolders:bool=False, conteiner_index:int=None, output_path:str=None, output_source:str=None, verbose:bool=False,  
+                    species:list=None, new_species:list=None, defect:str=None, 
+                    distribution:str=None, fill:bool=None, atom_groups:list=None, group_numbers:list=None, repetitions:bool=None,
+                    iterations:int=None):
     """
     Generate configurations with vacancies for computational chemistry simulations.
 
     Parameters:
     - path (str): Path to the directory containing input files.
     - source (str, optional): Type of source files, default is 'VASP'.
     - subfolders (bool, optional): Flag to include subdirectories in the search.
@@ -22,19 +23,28 @@
     Uses the Partition class from the sage_lib to read, process, and generate
     DFT (Density Functional Theory) variants with vacancies.
     """
     # Initialize a Partition object with the given path
     PT = Partition(path)
     # Read files and generate DFT variants with vacancies
     PT.read_files(file_location=path, source=source, energy_tag=energy_tag, forces_tag=forces_tag, subfolders=subfolders, verbose=verbose)
-    
-    PT.generate_variants('DEFECTS', values= [ {'defect':defect, 'species':species, 'new_species':new_species} ] )
 
+    #PT.generate_variants('DEFECTS', values= [ {'defect':defect, 'species':species, 'new_species':new_species} ] )
+    
+    values = {  'iterations': iterations, 
+                'repetitions': repetitions,
+                'distribution':distribution, 
+                'fill':fill, 
+                'atom_groups':atom_groups, 
+                'group_numbers':group_numbers}
+                
+    PT.generate_configurational_space(values=values, verbose=verbose) 
+    
     # Export the generated files back to the specified path
-    PT.export_files(file_location=path, source=source, label=None, verbose=verbose)
+    PT.export_files(file_location=output_path, source=output_source, label='enumerate', verbose=verbose)
 
 def generate_disassemble_surface(path, steps=5, final_distance=5.0, atoms_to_remove=None, subfolders=False, verbose=False):
     """
     Generate configurations for disassembling the surface.
 
     Parameters:
     - path (str): Path to the VASP files directory.
@@ -629,14 +639,34 @@
     parser.add_argument('--output_path', type=str, default='.', help='Path for exporting VASP partition and scripts')
     parser.add_argument('--output_source', type=str, choices=structure_list, help='Source for exporting partition and scripts')
 
     parser.add_argument('--verbose', default=False, action='store_true', help='Display additional information')
     parser.add_argument('--subfolders', default=False, action='store_true', help='Read from all subfolders under the specified path')    
     parser.add_argument('--conteiner_index', type=int, help='')    
 
+def parse_dynamic_groups(args):
+    atom_groups = [None] * 10  # Suponiendo hasta 10 grupos
+    group_numbers = [None] * 10
+
+    for key, value in vars(args).items():
+        if key.startswith('g') and not key.startswith('gn') and value is not None:
+            index = int(key[1:]) - 1  # Obtener el índice del grupo
+            atom_groups[index] = value
+            continue
+
+        if key.startswith('gn') and value is not None:
+            index = int(key[2:]) - 1  # Obtener el índice del número del grupo
+            group_numbers[index] = value
+            continue
+    
+    # Eliminar valores None
+    atom_groups = [group for group in atom_groups if group is not None]
+    group_numbers = [num for num in group_numbers if num is not None]
+
+    return atom_groups, group_numbers
 
 def main():
     """
     Main function to handle command line arguments and execute respective functions.
     This tool is designed for theoretical calculations in quantum mechanics and molecular dynamics,
     providing various sub-commands for different types of calculations and manipulations.
     """
@@ -647,14 +677,24 @@
     
     # =========== Sub-command to generate vacancy directory ===========
     parser_defects = subparsers.add_parser('defect', help='Generate configurations for defects in materials.')
     add_arguments(parser_defects)
     parser_defects.add_argument('--defect', choices=['substitution'], type=str, help='')
     parser_defects.add_argument('--species', nargs='+', help=' .')
     parser_defects.add_argument('--new_species', nargs='+', help=' .')
+    parser_defects.add_argument('--distribution', type=str, choices=['uniform', 'distance', 'distance-1', 'random'], help=' .')
+    parser_defects.add_argument('--fill', default=False, action='store_true', help=' .')
+    parser_defects.add_argument('--repetitions', default=1, type=int, help=' .')
+    parser_defects.add_argument('--iterations', default=1, type=int, help=' .')
+
+    for i in range(1, 10):  # Assuming up to 10 groups
+        parser_defects.add_argument(f'--g{i}', nargs='+', help=f'List of atom indices for group {i}')
+
+    for i in range(1, 10):  # Assuming up to 10 groups
+        parser_defects.add_argument(f'--gn{i}', type=int, help=f'Number of atoms in group {i}')
 
     # =========== Sub-command to generate configurations for disassembling the surface ===========
     parser_disassemble = subparsers.add_parser('disassemble', help='Generate configurations for disassembling surfaces or layers in a material.')
     add_arguments(parser_disassemble)
     parser_disassemble.add_argument('--steps', type=int, default=5, help='Number of steps in the disassembly process (default: 5)')
     parser_disassemble.add_argument('--final_distance', type=float, default=5.0, help='Final distance between layers or atoms after disassembly (default: 5.0)')
     parser_disassemble.add_argument('--atoms_to_remove', type=int, help='Number of atoms to remove during disassembly.')
@@ -664,16 +704,18 @@
     add_arguments(parser_dimer)
     parser_dimer.add_argument('--labels', nargs='+', help='List of atom labels to include in the dimer search. This option allows the specification of which types of atoms are to be considered for forming dimers.')
     parser_dimer.add_argument('--steps', type=int, default=10, help='Number of iterative steps in the dimer search. This parameter determines the resolution of the search process, with a higher number of steps providing finer detail in exploring dimer configurations (default: 10).')
     parser_dimer.add_argument('--vacuum', type=float, default=6.0, help='Specifies the vacuum distance (in Ångströms) around the dimer structure. This distance is used to define the amount of empty space surrounding the dimer in simulations, important for accurate electronic structure calculations (default: 6.0 Å).')
     parser_dimer.add_argument('--d0', type=float, default=None, help='Initial distance between the two atoms in a dimer (in Ångströms). If not specified, a default value based on atomic properties will be used. This parameter sets the starting point for the search process.')
     parser_dimer.add_argument('--df', type=float, default=None, help='Final distance between the two atoms in a dimer (in Ångströms). This value defines the end point of the distance range to be explored during the dimer search. If not specified, a reasonable default based on the atomic properties will be used.')
 
+
+
     # =========== Sub-comando para generar script ===========
-    parser_config = subparsers.add_parser('config', help='Read Position data from "path", read Configurtion data from "config_path" and export to "output_path".')
+    parser_config = subparsers.add_parser(' config', help='Read Position data from "path", read Configurtion data from "config_path" and export to "output_path".')
     add_arguments(parser_config)
     parser_config.add_argument('--config_path', type=str, required=True, help='')
     parser_config.add_argument('--config_source', type=str, required=True, help='')
 
     # =========== Sub-comando para generar BAND files ===========
     parser_bands = subparsers.add_parser('bands', help='Configure parameters for generating band calculation files from VASP data.')
     add_arguments(parser_bands)
@@ -804,18 +846,21 @@
     parser_blender.add_argument('--camera', type=str, nargs='+', default=['x', 'y', 'z'], choices=['x', '-x', 'y', '-y', 'z', '-z'], required=False, help='')
     parser_blender.add_argument('--repeat', type=int, nargs=3, default=[0,0,0], required=False, help='')
     
     args = parser.parse_args()
 
     # Handle execution based on the specified sub-command
     if args.command == 'defect':
+        atom_groups, group_numbers = parse_dynamic_groups(args)
         generate_defects(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, conteiner_index=args.conteiner_index,
-            verbose=args.verbose, output_path=args.output_path, 
-            defect=args.defect, species=args.species, new_species=args.new_species)
-
+            output_path=args.output_path, output_source=args.output_source,
+            verbose=args.verbose,
+            defect=args.defect, species=args.species, new_species=args.new_species, 
+            atom_groups=atom_groups, group_numbers=group_numbers, fill=args.fill, repetitions=args.repetitions, iterations=args.iterations, distribution=args.distribution)
+ 
     elif args.command == 'disassemble':
         generate_disassemble_surface(args.path, steps=args.steps, final_distance=args.final_distance, atoms_to_remove=args.atoms_to_remove, subfolders=args.subfolders, verbose=args.verbose)
     
     elif args.command == 'dimer':
         generate_dimers(path=args.path,     source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, 
                         subfolders=args.subfolders, conteiner_index=args.conteiner_index,
                         labels=args.labels, steps=args.steps, initial_distance=args.d0, final_distance=args.df, vacuum_tolerance=args.vacuum,
```

### Comparing `sage_lib-0.1.5.3/sage_lib/master/AtomicProperties.py` & `sage_lib-0.1.5.4/sage_lib/master/AtomicProperties.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/master/FileManager.py` & `sage_lib-0.1.5.4/sage_lib/master/FileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/miscellaneous/BandPathGenerator.py` & `sage_lib-0.1.5.4/sage_lib/miscellaneous/BandPathGenerator.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/miscellaneous/MD_tools.py` & `sage_lib-0.1.5.4/sage_lib/miscellaneous/MD_tools.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/miscellaneous/periodic_kdtree.py` & `sage_lib-0.1.5.4/sage_lib/miscellaneous/periodic_kdtree.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/partition/Partition.py` & `sage_lib-0.1.5.4/sage_lib/partition/Partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,17 +224,17 @@
                 containers += self.handleDefect(container, values, container_index, file_location)
                 directories[container_index] = 'Vacancy'
 
             elif parameter.upper() == 'BAND_STRUCTURE':
                 containers += self.handleBandStruture(container, values, container_index, file_location)
                 directories[container_index] = 'band_structure'
 
-            elif parameter.upper() == 'RATTLE':
-                containers += self.handleRattle(container, values, container_index, file_location)
-                directories[container_index] = 'rattle'
+            #elif parameter.upper() == 'RATTLE':
+            #    containers += self.handleRattle(container, values, container_index, file_location)
+            #    directories[container_index] = 'rattle'
 
             elif parameter.upper() == 'COMPRESS':
                 containers += self.handleCompress(container, values, container_index, file_location)
                 directories[container_index] = 'compress'
 
             elif parameter.upper() == 'CHANGE_ATOM_ID':
                 containers += self.handleAtomIDChange(container, values, container_index, file_location)
```

### Comparing `sage_lib-0.1.5.3/sage_lib/partition/PartitionManager.py` & `sage_lib-0.1.5.4/sage_lib/partition/PartitionManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py` & `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/BandStructure_builder.py` & `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/BandStructure_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Blender_builder.py` & `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Blender_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Config_builder.py` & `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Config_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Crystal_builder.py` & `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Crystal_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Dataset_builder.py` & `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Dataset_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Filter_builder.py` & `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Filter_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/MolecularDynamic_builder.py` & `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/MolecularDynamic_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/MoleculeCluster_builder.py` & `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/MoleculeCluster_builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -66,14 +66,50 @@
         """
         super().__init__(name=name, file_location=file_location)
 
         self._molecule_template = {}
         self._density = None
         self._cluster_lattice_vectors = None
 
+    @staticmethod
+    def generate_points_in_sphere(radius, num_points, distribution:str='uniform'):
+        """
+        Generates a uniform distribution of points inside a sphere.
+
+        Parameters:
+            radius (float): The radius of the sphere.
+            num_points (int): The number of points to generate.
+
+        Returns:
+            np.ndarray: An array of shape (num_points, 3) containing the generated points.
+        """
+        points = []
+
+        for _ in range(num_points):
+            # Generate a random point in spherical coordinates
+            phi = np.random.uniform(0, 2 * np.pi)  # azimuthal angle
+            costheta = np.random.uniform(-1, 1)  # cosine of polar angle
+            u = np.random.uniform(0, 1)  # random number for radius
+
+            theta = np.arccos(costheta)  # polar angle
+
+            if distribution == 'uniform':
+                r = radius * (u ** (1/3))  # cubic root to ensure uniform distribution
+            elif distribution == 'center':
+                r = radius   # cubic root to ensure center distribution
+
+            # Convert spherical coordinates to Cartesian coordinates
+            x = r * np.sin(theta) * np.cos(phi)
+            y = r * np.sin(theta) * np.sin(phi)
+            z = r * np.cos(theta)
+
+            points.append([x, y, z])
+
+        return np.array(points)
+
     def get_cluster_volume(self, shape:str='box', cluster_lattice_vectors:np.array=None ):
         """
         Calculates the volume of the molecular cluster based on its shape and lattice vectors.
 
         Parameters:
             shape (str): The shape of the cluster, default is 'box'.
             cluster_lattice_vectors (np.array): The lattice vectors defining the cluster boundaries.
@@ -81,16 +117,19 @@
         Returns:
             float: The volume of the cluster in cubic angstroms.
         """
         cluster_lattice_vectors = cluster_lattice_vectors if cluster_lattice_vectors is not None else self.cluster_lattice_vectors 
         
         if shape.lower() == 'box':
             return np.abs(np.linalg.det(cluster_lattice_vectors)) * 10**-24
+        elif shape.lower() == 'sphere':
+            return np.pi * 3/4 * cluster_lattice_vectors[0]**3 * 10**-24
+        
         else:
-            print('Undefine shape')
+            print(f'Undefine shape : {shape}')
 
         return volume
 
     def get_molecules_number_for_target_density(self, density:float=1.0, cluster_volume:float=None, molecules:dict={'H2O':1.0} ) -> dict:
         """
         Calculates the number of molecules needed to achieve a target density in the cluster.
 
@@ -143,14 +182,22 @@
         iteration = 0
 
         molecule_copy = copy.deepcopy(molecule) 
         while True:
             if shape.lower() == 'box':
                 if distribution.lower() == 'random':
                     displacement = translation + molecule_copy.generate_uniform_translation_from_fractional(latticeVectors=cluster_lattice_vectors )
+
+            elif shape.lower() == 'sphere':
+                if distribution.lower() == 'random':
+                    displacement = translation + self.generate_points_in_sphere(radius=cluster_lattice_vectors[0], num_points=1, distribution='uniform')
+                if distribution.lower() == 'center':
+                    displacement = translation + self.generate_points_in_sphere(radius=cluster_lattice_vectors[0], num_points=1, distribution='center')
+
+
             atomPositions = np.dot(molecule.atomPositions, molecule.generate_random_rotation_matrix().T) + displacement
             molecule_copy.set_atomPositions(new_atomPositions=atomPositions) 
             molecule_copy.latticeVectors = container.AtomPositionManager.latticeVectors
         
             if np.sum( container.AtomPositionManager.count_neighbors( molecule_copy, r=tolerance) ) == 0:   
                 container.AtomPositionManager.add_atom( atomLabels=molecule_copy.atomLabelsList, atomPosition=molecule_copy.atomPositions, atomicConstraints=molecule_copy.atomicConstraints )
                 return True
@@ -187,76 +234,79 @@
             for mn in range(molecule_number):
                 if verbosity: print(f'adding solvent: {int(mn/molecule_number*100)} %')
                 if not self.add_molecule( container=container, molecule=self.molecule_template[molecule_name], translation=translation, tolerance=tolerance,
                                         shape=shape, cluster_lattice_vectors=cluster_lattice_vectors, distribution=distribution, max_iteration=max_iteration ):
                     print('Can not set cluster, try lower density. ')
                     break
         
-    def handleCLUSTER(self, values:dict):
+    def handleCLUSTER(self, values:dict, containers:list=None):
         """
         Handles the creation and management of a molecular cluster within a specified container.
 
         Parameters:
             container (object): The container in which the cluster is built.
             values (list): A list of parameters defining the cluster properties.
             container_index (int): The index of the container.
             file_location (str, optional): The file location for storing cluster data.
 
         Returns:
             list: A list of containers with the created clusters.
         """
         #sub_directories, containers = [], []
         
-        containers = []
-        for container_index, container in enumerate(self.containers):
+        containers_new = []
+        containers = containers if isinstance(containers, list) else self.containers
+
+        for container_index, container in enumerate(containers):
             for v_key, v_item in values.items():
-                if isinstance(v_item['seed'], float): np.random.seed(int(v_item['seed'])) 
+
+                if 'seed' in v_item and isinstance(v_item['seed'], float): np.random.seed(int(v_item['seed'])) 
 
                 if v_key.upper() == 'ADD_SOLVENT':
                     # Copy and update container for each set of k-point values
                     container_copy = self.copy_and_update_container(container, f'/solvent/', '')
                     
                     for s in v_item['solvent']:
                         molecule = AtomPosition()
                         molecule.build(s)
                         self.add_molecule_template(s, molecule)
                     
-                    if v_item['slab']:
+                    if 'slab' in v_item and v_item['slab']:
                         vacuum_box, vacuum_start = container_copy.AtomPositionManager.get_vacuum_box(tolerance=v_item['vacuum_tolerance']) 
                         shape = 'box'
                         distribution = 'random'
                     else:
                         shape = v_item['shape']
                         if shape.upper() == 'BOX':
                             shape = 'box'
                             vacuum_box, vacuum_start = np.array([[v_item['size'][0],0,0],[0,v_item['size'][1],0],[0,0,v_item['size'][2]]], dtype=np.float64), v_item['translation']
                         elif shape.upper() == 'SPHERE':
                             shape = 'sphere'
-                            vacuum_box, vacuum_start = float(v_item['size'][0]), v_item['translation']
+                            vacuum_box, vacuum_start = [float(v_item['size'][0])], v_item['translation']
                         elif shape.upper() == 'PARALLELEPIPED':
                             shape = 'box'
                             vacuum_box, vacuum_start = np.array([
                                                             [v_item['size'][0],v_item['size'][1],v_item['size'][2]],
                                                             [v_item['size'][3],v_item['size'][4],v_item['size'][5]],
                                                             [v_item['size'][6],v_item['size'][7],v_item['size'][8]]], 
                                                         dtype=np.float64), v_item['translation']
                         elif shape.upper() == 'CELL':
                             shape = 'box'
                             vacuum_box, vacuum_start = np.array(container_copy.AtomPositionManager.get_cell() ,dtype=np.float64), np.array([0,0,0] ,dtype=np.float64)
 
-                        distribution = 'random'
+                        distribution = values.get('distribution', 'random')
 
                     tolerance = v_item['colition_tolerance']
                     density = v_item['density']
 
                     self.add_solvent(container=container_copy, shape=shape, cluster_lattice_vectors=vacuum_box, 
                                 translation=vacuum_start, distribution=distribution, density=density, tolerance=tolerance)
 
                     if v_item['wrap']:
                         container_copy.AtomPositionManager.pack_to_unit_cell()
 
-                    containers.append(container_copy)
+                    containers_new.append(container_copy)
 
-        self.containers = containers
+        self.containers = containers_new
 
-        return containers
+        return containers_new
```

### Comparing `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/Molecule_builder.py` & `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/Molecule_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/PositionEditor_builder.py` & `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/PositionEditor_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py` & `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/SurfaceStates_builder.py` & `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/SurfaceStates_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/partition/partition_builder/VacuumStates_builder.py` & `sage_lib-0.1.5.4/sage_lib/partition/partition_builder/VacuumStates_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/single_run/FF_Gap.py` & `sage_lib-0.1.5.4/sage_lib/single_run/FF_Gap.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/single_run/SingleRun.py` & `sage_lib-0.1.5.4/sage_lib/single_run/SingleRun.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/single_run/SingleRunDFT.py` & `sage_lib-0.1.5.4/sage_lib/single_run/SingleRunDFT.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib/single_run/SingleRunManager.py` & `sage_lib-0.1.5.4/sage_lib/single_run/SingleRunManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.3/sage_lib.egg-info/SOURCES.txt` & `sage_lib-0.1.5.4/sage_lib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 README.md
 setup.py
 sage_lib/__init__.py
 sage_lib/main.py
+sage_lib/main2.py
+sage_lib/main_rev.py
 sage_lib.egg-info/PKG-INFO
 sage_lib.egg-info/SOURCES.txt
 sage_lib.egg-info/dependency_links.txt
 sage_lib.egg-info/entry_points.txt
 sage_lib.egg-info/requires.txt
 sage_lib.egg-info/top_level.txt
 sage_lib/IO/BashScriptManager.py
```

