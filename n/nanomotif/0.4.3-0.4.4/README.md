# Comparing `tmp/nanomotif-0.4.3.tar.gz` & `tmp/nanomotif-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomotif-0.4.3.tar", last modified: Tue May 21 09:42:41 2024, max compression
+gzip compressed data, was "nanomotif-0.4.4.tar", last modified: Mon May 27 13:18:00 2024, max compression
```

## Comparing `nanomotif-0.4.3.tar` & `nanomotif-0.4.4.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:41.719247 nanomotif-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-21 09:42:37.000000 nanomotif-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-21 09:42:41.719247 nanomotif-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-21 09:42:37.000000 nanomotif-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:41.683247 nanomotif-0.4.3/nanomotif/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11213 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/bin_consensus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:41.683247 nanomotif-0.4.3/nanomotif/binnary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/binnary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/binnary/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/binnary/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/binnary/detect_contamination.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/binnary/include_contigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/binnary/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/binnary/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/binnary/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14301 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/dataload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:41.683247 nanomotif-0.4.3/nanomotif/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/datasets/geobacillus-contig-bin.tsv
--rw-r--r--   0 runner    (1001) docker     (127)   176247 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
--rw-r--r--   0 runner    (1001) docker     (127) 26479844 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/datasets/geobacillus-plasmids.pileup.bed
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    28633 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    20030 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:41.715247 nanomotif-0.4.3/nanomotif/mtase_linker/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/mtase_linker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/mtase_linker/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/mtase_linker/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/old_search_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/scoremotifs.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)    20090 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/seq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-21 09:42:37.000000 nanomotif-0.4.3/nanomotif/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:41.719247 nanomotif-0.4.3/nanomotif.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-21 09:42:41.000000 nanomotif-0.4.3/nanomotif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-21 09:42:41.000000 nanomotif-0.4.3/nanomotif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:42:41.000000 nanomotif-0.4.3/nanomotif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 09:42:41.000000 nanomotif-0.4.3/nanomotif.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:42:41.000000 nanomotif-0.4.3/nanomotif.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-21 09:42:41.000000 nanomotif-0.4.3/nanomotif.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 09:42:41.000000 nanomotif-0.4.3/nanomotif.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:42:41.719247 nanomotif-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-21 09:42:37.000000 nanomotif-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:41.719247 nanomotif-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:41.719247 nanomotif-0.4.3/tests/binnary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_cli_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_data_processing_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_detect_contamination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_generate_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_include_contigs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/binnary/test_write_bins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/test_candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/test_dataload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/test_motif_find.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:42:37.000000 nanomotif-0.4.3/tests/test_motif_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:00.877487 nanomotif-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-27 13:17:48.000000 nanomotif-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-27 13:18:00.877487 nanomotif-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-27 13:17:48.000000 nanomotif-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:00.837487 nanomotif-0.4.4/nanomotif/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11200 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/bin_consensus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:00.841487 nanomotif-0.4.4/nanomotif/binnary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/binnary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/binnary/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/binnary/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/binnary/detect_contamination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/binnary/include_contigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/binnary/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/binnary/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/binnary/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14370 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/dataload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:00.841487 nanomotif-0.4.4/nanomotif/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/datasets/geobacillus-contig-bin.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   176247 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
+-rw-r--r--   0 runner    (1001) docker     (127) 26479844 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/datasets/geobacillus-plasmids.pileup.bed
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28633 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20007 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:00.873487 nanomotif-0.4.4/nanomotif/mtase_linker/
+-rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/mtase_linker/MTase_linker.smk
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/mtase_linker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/mtase_linker/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/mtase_linker/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/mtase_linker/setup.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/old_search_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/scoremotifs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20090 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:00.877487 nanomotif-0.4.4/nanomotif.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-27 13:18:00.000000 nanomotif-0.4.4/nanomotif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-27 13:18:00.000000 nanomotif-0.4.4/nanomotif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:18:00.000000 nanomotif-0.4.4/nanomotif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 13:18:00.000000 nanomotif-0.4.4/nanomotif.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:18:00.000000 nanomotif-0.4.4/nanomotif.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-27 13:18:00.000000 nanomotif-0.4.4/nanomotif.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 13:18:00.000000 nanomotif-0.4.4/nanomotif.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 13:18:00.877487 nanomotif-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-27 13:17:49.000000 nanomotif-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:00.873487 nanomotif-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:00.877487 nanomotif-0.4.4/tests/binnary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_cli_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_data_processing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_detect_contamination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_generate_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_include_contigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_write_bins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/test_candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/test_dataload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/test_motif_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/test_motif_score.py
```

### Comparing `nanomotif-0.4.3/LICENSE` & `nanomotif-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/PKG-INFO` & `nanomotif-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomotif
-Version: 0.4.3
+Version: 0.4.4
 Summary: Identifying methlyation motifs in nanopore data
 Author: AAU_DarkScience
 Author-email: shei@bio.aau.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
@@ -107,15 +107,15 @@
 
 ```
 nanomotif include_contigs --motifs_scored MOTIFS_SCORED.tsv --bin_motifs BIN_MOTIFS.tsv --contig_bins CONTIG_BINS.tsv --run_detect_contamination -t THREADS --out OUT
 ```
 
 If decontamination should not be performed, the `include_contigs` can be run without the `--run_detect_contamination` flag or without the `--contamination_file` flag.
 
-#### Associating MTases and RM-systems to motifs
+#### MTase-linker
 This module tries to link methylation motifs to their corresponding MTase and, when present, their entire RM system. 
 
 The MTase-Linker module has additional dependencies that are not automatically installed with Nanomotif. Therefore, before using this module, you must manually install these dependencies using the `MTase-linker install` command.
 The `MTase-linker` module requires that conda is available on your system.
 
 ```
 nanomotif MTase-linker install
@@ -132,14 +132,16 @@
 ```
 
 Running the nanomotif MTase-linker run command will generate two primary output files: mtase_assignment_table.tsv and nanomotif_assignment_table.tsv. The first file lists all predicted MTase genes in the genome along with their predicted methylation characteristics and whether the module was able to unambiguously assign any detected motifs to the MTase (`linked` = (True/False)).
 The second file includes data from the bin-motifs.tsv of the nanomotif output with two additional columns `linked` and `candidate_genes`. The `linked` variable is a boolean indicator if the motif could be unambiguously linked to a MTase in the bin/genome (TRUE/FALSE). If True the gene_id of the MTase is provided in `candidate_gene`. If False, the `candidate_gene` variable lists feasible candidate facilitators of the modification based on motif type and modification type predictions.
 
 ## Citation
 
+Please cite our preprint if you use Nanomotif for your research:
+
 Nanomotif: Identification and Exploitation of DNA Methylation Motifs in Metagenomes using Oxford Nanopore Sequencing
 Søren Heidelbach, Sebastian Mølvang Dall, Jeppe Støtt Bøjer, Jacob Nissen, Lucas Nicolaas Ludovic van der Maas, Mantas Sereika, Rasmus Kirkegaard, Sabrina Just Kousgaard, Ole Thorlacius-Ussing, Sheila I Jensen, Katja Hose, Thomas Dyhre Nielsen, Mads Albertsen. Preprint at *bioRxiv* https://doi.org/10.1101/2024.04.29.591623 (2024)
 
 ## License
 
 Nanomotif is released under the [MIT License](https://github.com/your-username/nanomotif/blob/main/LICENSE). Feel free to use, modify, and distribute the package in accordance with the terms of the license.
```

### Comparing `nanomotif-0.4.3/README.md` & `nanomotif-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 ```
 nanomotif include_contigs --motifs_scored MOTIFS_SCORED.tsv --bin_motifs BIN_MOTIFS.tsv --contig_bins CONTIG_BINS.tsv --run_detect_contamination -t THREADS --out OUT
 ```
 
 If decontamination should not be performed, the `include_contigs` can be run without the `--run_detect_contamination` flag or without the `--contamination_file` flag.
 
-#### Associating MTases and RM-systems to motifs
+#### MTase-linker
 This module tries to link methylation motifs to their corresponding MTase and, when present, their entire RM system. 
 
 The MTase-Linker module has additional dependencies that are not automatically installed with Nanomotif. Therefore, before using this module, you must manually install these dependencies using the `MTase-linker install` command.
 The `MTase-linker` module requires that conda is available on your system.
 
 ```
 nanomotif MTase-linker install
@@ -111,14 +111,16 @@
 ```
 
 Running the nanomotif MTase-linker run command will generate two primary output files: mtase_assignment_table.tsv and nanomotif_assignment_table.tsv. The first file lists all predicted MTase genes in the genome along with their predicted methylation characteristics and whether the module was able to unambiguously assign any detected motifs to the MTase (`linked` = (True/False)).
 The second file includes data from the bin-motifs.tsv of the nanomotif output with two additional columns `linked` and `candidate_genes`. The `linked` variable is a boolean indicator if the motif could be unambiguously linked to a MTase in the bin/genome (TRUE/FALSE). If True the gene_id of the MTase is provided in `candidate_gene`. If False, the `candidate_gene` variable lists feasible candidate facilitators of the modification based on motif type and modification type predictions.
 
 ## Citation
 
+Please cite our preprint if you use Nanomotif for your research:
+
 Nanomotif: Identification and Exploitation of DNA Methylation Motifs in Metagenomes using Oxford Nanopore Sequencing
 Søren Heidelbach, Sebastian Mølvang Dall, Jeppe Støtt Bøjer, Jacob Nissen, Lucas Nicolaas Ludovic van der Maas, Mantas Sereika, Rasmus Kirkegaard, Sabrina Just Kousgaard, Ole Thorlacius-Ussing, Sheila I Jensen, Katja Hose, Thomas Dyhre Nielsen, Mads Albertsen. Preprint at *bioRxiv* https://doi.org/10.1101/2024.04.29.591623 (2024)
 
 ## License
 
 Nanomotif is released under the [MIT License](https://github.com/your-username/nanomotif/blob/main/LICENSE). Feel free to use, modify, and distribute the package in accordance with the terms of the license.
```

### Comparing `nanomotif-0.4.3/nanomotif/argparser.py` & `nanomotif-0.4.4/nanomotif/argparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,29 +167,29 @@
     )
 
     parser_mtase_linker_run = mtase_linker_subparsers.add_parser(
         'run', 
         help="Run the MTase-linker workflow"
     )
     parser_mtase_linker_run.add_argument("-t", "--threads", type=int, default=1, help="Number of threads to use. Default is 1")
-    parser_mtase_linker_run.add_argument("--forceall", type=bool, default=False, help="Forcerun workflow regardless of already created output (default = False)")
-    parser_mtase_linker_run.add_argument("--dryrun", type=bool, default=False, help="Dry-run the workflow. Default is False")
+    parser_mtase_linker_run.add_argument("--forceall", type=bool, default=False, help="Flag for snakemake. Forcerun workflow regardless of already created output (default = False)")
+    parser_mtase_linker_run.add_argument("--dryrun", type=bool, default=False, help="Flag for snakemake. Dry-run the workflow. Default is False")
     parser_mtase_linker_run.add_argument("--assembly", type=str, required=True, help="Path to assembly file.")
     parser_mtase_linker_run.add_argument("--contig_bin", type=str, required=True, help="tsv file specifying which bin contigs belong.")
     parser_mtase_linker_run.add_argument("--bin_motifs", type=str, required=True, help="bin-motifs.tsv output from nanomotif.")
-    parser_mtase_linker_run.add_argument("-d", "--dependency_dir", type=str, default=os.path.join(os.getcwd(), "ML_dependencies"), help="Same as for installation. Path to directory of the ML_dependencies directory created during installation of the MTase-linker module. Default is cwd/ML_dependencies")
-    parser_mtase_linker_run.add_argument("-o", "--outputdir", type=str, default=os.path.join(os.getcwd(), "mtase_linker"), help="Output directory. Default is cwd")
+    parser_mtase_linker_run.add_argument("-d", "--dependency_dir", type=str, default=os.path.join(os.getcwd(), "ML_dependencies"), help="Path to the ML_dependencies directory created during installation of the MTase-linker module. Default is cwd/ML_dependencies")
+    parser_mtase_linker_run.add_argument("-o", "--out", type=str, default=os.path.join(os.getcwd(), "mtase_linker"), help="Path to output directory. Default is cwd")
     parser_mtase_linker_run.add_argument("--identity", type=str, default=80, help="Identity threshold for motif prediction. Default is 80")
     parser_mtase_linker_run.add_argument("--qcovs", type=str, default=80, help="Query coverage for motif prediction. Default is 80")
 
     parser_mtase_linker_install = mtase_linker_subparsers.add_parser(
         'install', 
         help="Install additional dependencies for MTase-linker"
     )
-    parser_mtase_linker_install.add_argument("-d", "--dependency_dir", type=str, default=os.getcwd(), help="Path to the directory, where dependencies should be installed. A folder named ML_dependencies will be generated. Default is cwd.")
+    parser_mtase_linker_install.add_argument("-d", "--dependency_dir", type=str, default=os.getcwd(), help="Path to installation location of dependencies. A folder named ML_dependencies will be generated. Default is cwd.")
     
 
 
     ###########################################################################
     # Check installation
     parser_check_installation = subparsers.add_parser('check_installation', parents=[parser_optional, parser_shared_find_motifs], add_help=False, help="Performs small test run to verify that the installation is correct.")
```

### Comparing `nanomotif-0.4.3/nanomotif/bin_consensus.py` & `nanomotif-0.4.4/nanomotif/bin_consensus.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/binnary/analysis.py` & `nanomotif-0.4.4/nanomotif/binnary/analysis.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/binnary/data_processing.py` & `nanomotif-0.4.4/nanomotif/binnary/data_processing.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/binnary/detect_contamination.py` & `nanomotif-0.4.4/nanomotif/binnary/detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/binnary/include_contigs.py` & `nanomotif-0.4.4/nanomotif/binnary/include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/binnary/logging.py` & `nanomotif-0.4.4/nanomotif/binnary/logging.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/binnary/scoring.py` & `nanomotif-0.4.4/nanomotif/binnary/scoring.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/binnary/utils.py` & `nanomotif-0.4.4/nanomotif/binnary/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/candidate.py` & `nanomotif-0.4.4/nanomotif/candidate.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         return str_equal and pos_equal
     def sub_motif_of(self, other_motif):
         """
         Check if a motif is in another motif.
         """
         assert isinstance(other_motif, Motif)
         # Strip for redundant posititons (flanking .)
+        if self.identical(other_motif):
+            return False
         self_stripped = self.new_stripped_motif()
         other_stripped = other_motif.new_stripped_motif()
 
         if self_stripped.length() < other_stripped.length():
             return False
 
         # Split into list of bases
@@ -128,15 +130,15 @@
         """
         motif_split = self.split()
         isolated = False
         for pos in range(len(motif_split)):
             if motif_split[pos] == ".":
                 continue
             index_start = max(pos - isolation_size, 0)
-            index_end = min(pos + isolation_size, len(motif_split) - 1)
+            index_end = min(pos + isolation_size + 1, len(motif_split) - 1)
             # If all surrounding positions are ".", it is isolated
             if set(motif_split[index_start:pos] + motif_split[pos+1:index_end]) == set(["."]):
                 isolated = True
         return isolated
         
 
     def length(self) -> int:
```

### Comparing `nanomotif-0.4.3/nanomotif/constants.py` & `nanomotif-0.4.4/nanomotif/constants.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/dataload.py` & `nanomotif-0.4.4/nanomotif/dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/datasets/geobacillus-plasmids.assembly.fasta` & `nanomotif-0.4.4/nanomotif/datasets/geobacillus-plasmids.assembly.fasta`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/datasets/geobacillus-plasmids.pileup.bed` & `nanomotif-0.4.4/nanomotif/datasets/geobacillus-plasmids.pileup.bed`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/datasets.py` & `nanomotif-0.4.4/nanomotif/datasets.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/evaluate.py` & `nanomotif-0.4.4/nanomotif/evaluate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/feature.py` & `nanomotif-0.4.4/nanomotif/feature.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/main.py` & `nanomotif-0.4.4/nanomotif/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,14 @@
         )
     motifs = pl.DataFrame(motifs)
     if motifs is None:
         log.info("No motifs found")
         return
 
     log.info("Writing motifs")
-    pl.show_versions()
     def format_motif_df(df):
         if "model" in df.columns:
             n_mod = [x._alpha for x in df["model"]]
             n_nomod = [x._beta for x in df["model"]]
         motif_iupac = [nm.seq.regex_to_iupac(x) for x in df["motif"]]
         motif_type = [nm.utils.motif_type(x) for x in motif_iupac]
```

### Comparing `nanomotif-0.4.3/nanomotif/model.py` & `nanomotif-0.4.4/nanomotif/model.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/mtase_linker/command.py` & `nanomotif-0.4.4/nanomotif/mtase_linker/command.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/mtase_linker/dependencies.py` & `nanomotif-0.4.4/nanomotif/mtase_linker/dependencies.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/old_search_method.py` & `nanomotif-0.4.4/nanomotif/old_search_method.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/parallel.py` & `nanomotif-0.4.4/nanomotif/parallel.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/postprocess.py` & `nanomotif-0.4.4/nanomotif/postprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import nanomotif as nm
 import polars as pl
 import numpy as np
 from polars import col
 import logging as log
 
 def remove_noisy_motifs(motif_df):
+    """
+    Remove motifs that have isolated bases
+    """
     motif_df_clean = []
     for contig, df in motif_df.groupby("contig"):
         motif_strings = df.get_column("motif").to_list()
         positions = df.get_column("mod_position").to_list()
         motifs = [nm.candidate.Motif(motif_string, pos) for motif_string, pos in zip(motif_strings, positions)]
         clean_motifs = []
         for motif in motifs:
```

### Comparing `nanomotif-0.4.3/nanomotif/scoremotifs.py` & `nanomotif-0.4.4/nanomotif/scoremotifs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/seq.py` & `nanomotif-0.4.4/nanomotif/seq.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif/utils.py` & `nanomotif-0.4.4/nanomotif/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/nanomotif.egg-info/PKG-INFO` & `nanomotif-0.4.4/nanomotif.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomotif
-Version: 0.4.3
+Version: 0.4.4
 Summary: Identifying methlyation motifs in nanopore data
 Author: AAU_DarkScience
 Author-email: shei@bio.aau.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
@@ -107,15 +107,15 @@
 
 ```
 nanomotif include_contigs --motifs_scored MOTIFS_SCORED.tsv --bin_motifs BIN_MOTIFS.tsv --contig_bins CONTIG_BINS.tsv --run_detect_contamination -t THREADS --out OUT
 ```
 
 If decontamination should not be performed, the `include_contigs` can be run without the `--run_detect_contamination` flag or without the `--contamination_file` flag.
 
-#### Associating MTases and RM-systems to motifs
+#### MTase-linker
 This module tries to link methylation motifs to their corresponding MTase and, when present, their entire RM system. 
 
 The MTase-Linker module has additional dependencies that are not automatically installed with Nanomotif. Therefore, before using this module, you must manually install these dependencies using the `MTase-linker install` command.
 The `MTase-linker` module requires that conda is available on your system.
 
 ```
 nanomotif MTase-linker install
@@ -132,14 +132,16 @@
 ```
 
 Running the nanomotif MTase-linker run command will generate two primary output files: mtase_assignment_table.tsv and nanomotif_assignment_table.tsv. The first file lists all predicted MTase genes in the genome along with their predicted methylation characteristics and whether the module was able to unambiguously assign any detected motifs to the MTase (`linked` = (True/False)).
 The second file includes data from the bin-motifs.tsv of the nanomotif output with two additional columns `linked` and `candidate_genes`. The `linked` variable is a boolean indicator if the motif could be unambiguously linked to a MTase in the bin/genome (TRUE/FALSE). If True the gene_id of the MTase is provided in `candidate_gene`. If False, the `candidate_gene` variable lists feasible candidate facilitators of the modification based on motif type and modification type predictions.
 
 ## Citation
 
+Please cite our preprint if you use Nanomotif for your research:
+
 Nanomotif: Identification and Exploitation of DNA Methylation Motifs in Metagenomes using Oxford Nanopore Sequencing
 Søren Heidelbach, Sebastian Mølvang Dall, Jeppe Støtt Bøjer, Jacob Nissen, Lucas Nicolaas Ludovic van der Maas, Mantas Sereika, Rasmus Kirkegaard, Sabrina Just Kousgaard, Ole Thorlacius-Ussing, Sheila I Jensen, Katja Hose, Thomas Dyhre Nielsen, Mads Albertsen. Preprint at *bioRxiv* https://doi.org/10.1101/2024.04.29.591623 (2024)
 
 ## License
 
 Nanomotif is released under the [MIT License](https://github.com/your-username/nanomotif/blob/main/LICENSE). Feel free to use, modify, and distribute the package in accordance with the terms of the license.
```

### Comparing `nanomotif-0.4.3/nanomotif.egg-info/SOURCES.txt` & `nanomotif-0.4.4/nanomotif.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -35,17 +35,19 @@
 nanomotif/binnary/include_contigs.py
 nanomotif/binnary/logging.py
 nanomotif/binnary/scoring.py
 nanomotif/binnary/utils.py
 nanomotif/datasets/geobacillus-contig-bin.tsv
 nanomotif/datasets/geobacillus-plasmids.assembly.fasta
 nanomotif/datasets/geobacillus-plasmids.pileup.bed
+nanomotif/mtase_linker/MTase_linker.smk
 nanomotif/mtase_linker/__init__.py
 nanomotif/mtase_linker/command.py
 nanomotif/mtase_linker/dependencies.py
+nanomotif/mtase_linker/setup.smk
 tests/__init__.py
 tests/test_candidate.py
 tests/test_dataload.py
 tests/test_motif_find.py
 tests/test_motif_score.py
 tests/binnary/__init__.py
 tests/binnary/conftest.py
```

### Comparing `nanomotif-0.4.3/setup.py` & `nanomotif-0.4.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     author='AAU_DarkScience',
     author_email='shei@bio.aau.com',
     license='MIT',
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     include_package_data=True,
-    package_data={'nanomotif': ['datasets/*'], 'snakemake':['.smk']},
+    package_data={'nanomotif': ['datasets/*'], '':['*.smk']},
     zip_safe=False,
     install_requires=[
         "wheel",
         "requests",
         "numpy>=1.24.4",
         "pandas>=2.0.2",
         "polars>=0.19",
```

### Comparing `nanomotif-0.4.3/tests/binnary/conftest.py` & `nanomotif-0.4.4/tests/binnary/conftest.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/tests/binnary/test_arg_parser.py` & `nanomotif-0.4.4/tests/binnary/test_arg_parser.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/tests/binnary/test_cli_commands.py` & `nanomotif-0.4.4/tests/binnary/test_cli_commands.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/tests/binnary/test_data_processing_functions.py` & `nanomotif-0.4.4/tests/binnary/test_data_processing_functions.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/tests/binnary/test_detect_contamination.py` & `nanomotif-0.4.4/tests/binnary/test_detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/tests/binnary/test_generate_output.py` & `nanomotif-0.4.4/tests/binnary/test_generate_output.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/tests/binnary/test_include_contigs.py` & `nanomotif-0.4.4/tests/binnary/test_include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/tests/binnary/test_scoring.py` & `nanomotif-0.4.4/tests/binnary/test_scoring.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/tests/binnary/test_utils.py` & `nanomotif-0.4.4/tests/binnary/test_utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/tests/binnary/test_write_bins.py` & `nanomotif-0.4.4/tests/binnary/test_write_bins.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/tests/test_candidate.py` & `nanomotif-0.4.4/tests/test_candidate.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         motif_strip = motif.new_stripped_motif()
         motif_strip_reverse = motif_strip.reverse_compliment()
         assert motif_strip_reverse == Motif("CG..AT", 5)
     
     def test_sub_motif_of(self):
         motif1 = Motif("ATCG", 2)
         motif2 = Motif("ATCG", 2)
-        assert motif1.sub_motif_of(motif2) == True
+        assert motif1.sub_motif_of(motif2) == False
 
         motif1 = Motif("ATCG", 0)
         motif2 = Motif("AT", 0)
         assert motif1.sub_motif_of(motif2) == True
 
         motif1 = Motif("A[TCG]CG", 0)
         motif2 = Motif("A.C", 0)
```

### Comparing `nanomotif-0.4.3/tests/test_dataload.py` & `nanomotif-0.4.4/tests/test_dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.3/tests/test_motif_find.py` & `nanomotif-0.4.4/tests/test_motif_find.py`

 * *Files identical despite different names*

