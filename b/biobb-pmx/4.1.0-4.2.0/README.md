# Comparing `tmp/biobb_pmx-4.1.0.tar.gz` & `tmp/biobb_pmx-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_pmx-4.1.0.tar", last modified: Sun Sep 17 22:13:34 2023, max compression
+gzip compressed data, was "biobb_pmx-4.2.0.tar", last modified: Mon May 27 15:35:40 2024, max compression
```

## Comparing `biobb_pmx-4.1.0.tar` & `biobb_pmx-4.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-17 22:13:34.351025 biobb_pmx-4.1.0/
--rwxr-xr-x   0 pau        (501) staff       (20)    11358 2021-06-11 09:55:35.000000 biobb_pmx-4.1.0/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)     6081 2023-09-17 22:13:34.350717 biobb_pmx-4.1.0/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     5165 2023-09-17 22:11:37.000000 biobb_pmx-4.1.0/README.md
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-17 22:13:34.337921 biobb_pmx-4.1.0/biobb_pmx/
--rw-r--r--   0 pau        (501) staff       (20)       64 2023-09-17 21:56:49.000000 biobb_pmx-4.1.0/biobb_pmx/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-17 22:13:34.349674 biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/
--rwxr-xr-x   0 pau        (501) staff       (20)      140 2023-06-30 14:28:12.000000 biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)     1836 2023-09-17 21:35:55.000000 biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/common.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13168 2023-06-30 14:17:30.000000 biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/pmxanalyse.py
--rwxr-xr-x   0 pau        (501) staff       (20)    18149 2023-06-30 14:17:30.000000 biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/pmxatom_mapping.py
--rwxr-xr-x   0 pau        (501) staff       (20)     9994 2023-06-30 14:17:30.000000 biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/pmxcreate_top.py
--rwxr-xr-x   0 pau        (501) staff       (20)    10654 2023-07-07 08:35:58.000000 biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/pmxgentop.py
--rwxr-xr-x   0 pau        (501) staff       (20)    16722 2023-06-30 14:17:30.000000 biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/pmxligand_hybrid.py
--rwxr-xr-x   0 pau        (501) staff       (20)     6993 2023-06-30 14:30:03.000000 biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/pmxmerge_ff.py
--rwxr-xr-x   0 pau        (501) staff       (20)    10031 2023-06-30 14:17:30.000000 biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/pmxmutate.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-17 22:13:34.350365 biobb_pmx-4.1.0/biobb_pmx/test/
--rwxr-xr-x   0 pau        (501) staff       (20)        0 2021-06-11 09:55:35.000000 biobb_pmx-4.1.0/biobb_pmx/test/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-17 22:13:34.340720 biobb_pmx-4.1.0/biobb_pmx.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     6081 2023-09-17 22:13:34.000000 biobb_pmx-4.1.0/biobb_pmx.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)      579 2023-09-17 22:13:34.000000 biobb_pmx-4.1.0/biobb_pmx.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-09-17 22:13:34.000000 biobb_pmx-4.1.0/biobb_pmx.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)      380 2023-09-17 22:13:34.000000 biobb_pmx-4.1.0/biobb_pmx.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)       37 2023-09-17 22:13:34.000000 biobb_pmx-4.1.0/biobb_pmx.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)       10 2023-09-17 22:13:34.000000 biobb_pmx-4.1.0/biobb_pmx.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)       38 2023-09-17 22:13:34.351119 biobb_pmx-4.1.0/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     1770 2023-09-17 22:10:29.000000 biobb_pmx-4.1.0/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-27 15:35:40.685871 biobb_pmx-4.2.0/
+-rwxr-xr-x   0 pau        (501) staff       (20)    11358 2021-06-11 09:55:35.000000 biobb_pmx-4.2.0/LICENSE
+-rw-r--r--   0 pau        (501) staff       (20)     6621 2024-05-27 15:35:40.685352 biobb_pmx-4.2.0/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     5705 2024-05-24 11:12:34.000000 biobb_pmx-4.2.0/README.md
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-27 15:35:40.674403 biobb_pmx-4.2.0/biobb_pmx/
+-rw-r--r--   0 pau        (501) staff       (20)       88 2024-05-24 11:12:01.000000 biobb_pmx-4.2.0/biobb_pmx/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-27 15:35:40.684017 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/
+-rwxr-xr-x   0 pau        (501) staff       (20)      329 2024-05-21 10:57:48.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)     1836 2023-09-17 21:35:55.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/common.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    13304 2024-05-24 08:55:34.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxanalyse.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    18207 2024-05-24 08:55:53.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxatom_mapping.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    10070 2024-05-24 08:56:05.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxcreate_top.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    10712 2024-05-24 08:56:14.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxgentop.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    16799 2024-05-24 08:56:23.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxligand_hybrid.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     7028 2024-05-24 08:56:31.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxmerge_ff.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    10077 2024-05-24 08:57:02.000000 biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxmutate.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-27 15:35:40.684872 biobb_pmx-4.2.0/biobb_pmx/test/
+-rwxr-xr-x   0 pau        (501) staff       (20)        0 2021-06-11 09:55:35.000000 biobb_pmx-4.2.0/biobb_pmx/test/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-27 15:35:40.677329 biobb_pmx-4.2.0/biobb_pmx.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     6621 2024-05-27 15:35:40.000000 biobb_pmx-4.2.0/biobb_pmx.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)      579 2024-05-27 15:35:40.000000 biobb_pmx-4.2.0/biobb_pmx.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2024-05-27 15:35:40.000000 biobb_pmx-4.2.0/biobb_pmx.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)      380 2024-05-27 15:35:40.000000 biobb_pmx-4.2.0/biobb_pmx.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)       37 2024-05-27 15:35:40.000000 biobb_pmx-4.2.0/biobb_pmx.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)       10 2024-05-27 15:35:40.000000 biobb_pmx-4.2.0/biobb_pmx.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)       38 2024-05-27 15:35:40.686184 biobb_pmx-4.2.0/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     1770 2024-05-24 11:10:09.000000 biobb_pmx-4.2.0/setup.py
```

### Comparing `biobb_pmx-4.1.0/LICENSE` & `biobb_pmx-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_pmx-4.1.0/PKG-INFO` & `biobb_pmx-4.2.0/biobb_pmx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: biobb_pmx
-Version: 4.1.0
+Name: biobb-pmx
+Version: 4.2.0
 Summary: Biobb_pmx is the Biobb module collection to perform PMX (http://pmx.mpibpc.mpg.de) executions.
 Home-page: https://github.com/bioexcel/biobb_pmx
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
-Project-URL: Documentation, http://biobb_pmx.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-pmx.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pmx?label=Version)](https://GitHub.com/bioexcel/biobb_pmx/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pmx.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pmx/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pmx?label=Conda)](https://anaconda.org/bioconda/biobb_pmx)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pmx?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pmx)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pmx?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pmx:4.1.0--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pmx)
 [![](https://img.shields.io/pypi/pyversions/biobb-pmx.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pmx/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pmx)
 
 [![](https://readthedocs.org/projects/biobb-pmx/badge/?version=latest&label=Docs)](https://biobb-pmx.readthedocs.io/en/latest/?badge=latest)
@@ -40,86 +40,93 @@
 
 [![](https://docs.bioexcel.eu/biobb_pmx/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_pmx/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_pmx/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_pmx/coverage/)
 [![](https://docs.bioexcel.eu/biobb_pmx/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_pmx/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_pmx?label=Last%20Commit)](https://github.com/bioexcel/biobb_pmx/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_pmx.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_pmx/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 
 # biobb_pmx
 
 ### Introduction
 Biobb_pmx is the Biobb module collection to perform PMX (http://pmx.mpibpc.mpg.de) executions.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_pmx.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-pmx.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2023.3
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
-        pip install "biobb_pmx>=4.1.0"
+        pip install "biobb_pmx>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pmx>=4.1.0"
+        conda install -c bioconda "biobb_pmx>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pmx.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pmx:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_pmx:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pmx:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_pmx:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pmx.sif https://depot.galaxyproject.org/singularity/biobb_pmx:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_pmx.sif https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_pmx.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-pmx.readthedocs.io/en/latest/command_line.html).
 
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2022 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2022[Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_pmx-4.1.0/README.md` & `biobb_pmx-4.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pmx?label=Version)](https://GitHub.com/bioexcel/biobb_pmx/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pmx.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pmx/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pmx?label=Conda)](https://anaconda.org/bioconda/biobb_pmx)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pmx?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pmx)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pmx?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pmx:4.1.0--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pmx)
 [![](https://img.shields.io/pypi/pyversions/biobb-pmx.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pmx/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pmx)
 
 [![](https://readthedocs.org/projects/biobb-pmx/badge/?version=latest&label=Docs)](https://biobb-pmx.readthedocs.io/en/latest/?badge=latest)
@@ -18,86 +18,93 @@
 
 [![](https://docs.bioexcel.eu/biobb_pmx/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_pmx/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_pmx/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_pmx/coverage/)
 [![](https://docs.bioexcel.eu/biobb_pmx/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_pmx/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_pmx?label=Last%20Commit)](https://github.com/bioexcel/biobb_pmx/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_pmx.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_pmx/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 
 # biobb_pmx
 
 ### Introduction
 Biobb_pmx is the Biobb module collection to perform PMX (http://pmx.mpibpc.mpg.de) executions.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_pmx.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-pmx.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2023.3
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
-        pip install "biobb_pmx>=4.1.0"
+        pip install "biobb_pmx>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pmx>=4.1.0"
+        conda install -c bioconda "biobb_pmx>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pmx.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pmx:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_pmx:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pmx:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_pmx:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pmx.sif https://depot.galaxyproject.org/singularity/biobb_pmx:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_pmx.sif https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_pmx.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-pmx.readthedocs.io/en/latest/command_line.html).
 
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2022 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2022[Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/common.py` & `biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/common.py`

 * *Files identical despite different names*

### Comparing `biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/pmxanalyse.py` & `biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxanalyse.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Pmxanalyse(BiobbObject):
     """
     | biobb_pmx Pmxanalyse
     | Wrapper class for the `PMX analyse <https://github.com/deGrootLab/pmx>`_ module.
+    | Analyze the work values from the dgdl.xvg files of the A and B states to calculate the free energy difference between two states.
 
     Args:
         input_a_xvg_zip_path (str): Path the zip file containing the dgdl.xvg files of the A state. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/xvg_A.zip>`_. Accepted formats: zip (edam:format_3987).
         input_b_xvg_zip_path (str): Path the zip file containing the dgdl.xvg files of the B state. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/xvg_B.zip>`_. Accepted formats: zip (edam:format_3987).
         output_result_path (str): Path to the TXT results file. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/ref_result.txt>`_. Accepted formats: txt (edam:format_2330).
         output_work_plot_path (str): Path to the PNG plot results file. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/ref_plot.png>`_. Accepted formats: png (edam:format_3603).
         properties (dic):
```

### Comparing `biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/pmxatom_mapping.py` & `biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxatom_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Pmxatom_mapping(BiobbObject):
     """
     | biobb_pmx Pmxatom_mapping
     | Wrapper class for the `PMX atom_mapping <https://github.com/deGrootLab/pmx>`_ module.
+    | Perform atom mapping between two ligand structures.
 
     Args:
         input_structure1_path (str): Path to the input ligand structure file 1. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/ligand.pdb>`_. Accepted formats: pdb (edam:format_1476).
         input_structure2_path (str): Path to the input ligand structure file 2. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/ligand.pdb>`_. Accepted formats: pdb (edam:format_1476).
         output_pairs1_path (str): Path to the output pairs for the ligand structure 1. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/ref_mapping_pairs.dat>`_. Accepted formats: dat (edam:format_1637), txt (edam:format_2330).
         output_pairs2_path (str): Path to the output pairs for the ligand structure 2. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/ref_mapping_pairs.dat>`_. Accepted formats: dat (edam:format_1637), txt (edam:format_2330).
         output_log_path (str): Path to the log file. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/atom_mapping.log>`_. Accepted formats: log (edam:format_2330), txt (edam:format_2330), out (edam:format_2330).
```

### Comparing `biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/pmxcreate_top.py` & `biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxcreate_top.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Pmxcreate_top(BiobbObject):
     """
     | biobb_pmx Pmxcreate_top
     | Wrapper class for the `PMX create_top <https://github.com/deGrootLab/pmx>`_ module.
+    | Create a complete ligand topology file from two input topology files.
 
     Args:
         input_topology1_path (str): Path to the input topology file 1. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/ligand.itp>`_. Accepted formats: itp (edam:format_3883).
         input_topology2_path (str): Path to the input topology file 2. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/ligand.itp>`_. Accepted formats: itp (edam:format_3883).
         output_topology_path (str): Path to the complete ligand topology file. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/ligand_top.zip>`_. Accepted formats: zip (edam:format_3987).
 
         properties (dic):
```

### Comparing `biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/pmxgentop.py` & `biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxgentop.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Pmxgentop(BiobbObject):
     """
     | biobb_pmx Pmxgentop
     | Wrapper class for the `PMX gentop <https://github.com/deGrootLab/pmx>`_ module.
+    | Generate a topology file for a morphing simulation.
 
     Args:
         input_top_zip_path (str): Path the input GROMACS topology TOP and ITP files in zip format. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/topology.zip>`_. Accepted formats: zip (edam:format_3987).
         output_top_zip_path (str): Path the output TOP topology in zip format. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/ref_output_topology.zip>`_. Accepted formats: zip (edam:format_3987).
         properties (dic):
             * **force_field** (*str*) - ("amber99sb-star-ildn-mut") Force field to use. If **input_top_zip_path** is a top file, it's not necessary to specify the forcefield, as it will be determined automatically. If **input_top_zip_path** is an itp file, then it's needed.
             * **split** (*bool*) - (False) Write separate topologies for the vdW and charge transformations.
```

### Comparing `biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/pmxligand_hybrid.py` & `biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxligand_hybrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Pmxligand_hybrid(BiobbObject):
     """
     | biobb_pmx Pmxligand_hybrid
     | Wrapper class for the `PMX ligand_hybrid <https://github.com/deGrootLab/pmx>`_ module.
+    | Create a hybrid topology and structure based on two ligand structures.
 
     Args:
         input_structure1_path (str): Path to the input ligand structure file 1. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/ligand.pdb>`_. Accepted formats: pdb (edam:format_1476).
         input_structure2_path (str): Path to the input ligand structure file 2. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/ligand.pdb>`_. Accepted formats: pdb (edam:format_1476).
         input_topology1_path (str): Path to the input ligand topology file 1. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/ligand.itp>`_. Accepted formats: itp (edam:format_3883).
         input_topology2_path (str): Path to the input ligand topology file 2. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/ligand.itp>`_. Accepted formats: itp (edam:format_3883).
         input_pairs_path (str) (Optional): Path to the input atom pair mapping. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/ref_mapping_pairs.dat>`_. Accepted formats: dat (edam:format_1637), txt (edam:format_2330).
```

### Comparing `biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/pmxmerge_ff.py` & `biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxmerge_ff.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Pmxmerge_ff(BiobbObject):
     """
     | biobb_pmx Pmxmerge_ff
     | Wrapper class for the `PMX merge_ff <https://github.com/deGrootLab/pmx>`_ module.
+    | Merge ligand topology files.
 
     Args:
         input_topology_path (str): Path to the input ligand topologies as a zip file containing a list of itp files. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/ligand_itps.zip>`_. Accepted formats: zip (edam:format_3987).
         output_topology_path (str): Path to the merged ligand topology file. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/ligand.itp>`_. Accepted formats: itp (edam:format_3883).
 
         properties (dic):
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
```

### Comparing `biobb_pmx-4.1.0/biobb_pmx/pmxbiobb/pmxmutate.py` & `biobb_pmx-4.2.0/biobb_pmx/pmxbiobb/pmxmutate.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Pmxmutate(BiobbObject):
     """
     | biobb_pmx Pmxmutate
     | Wrapper class for the `PMX mutate <https://github.com/deGrootLab/pmx>`_ module.
+    | Mutate residues in a protein structure.
 
     Args:
         input_structure_path (str): Path to the input structure file. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/frame99.pdb>`_. Accepted formats: pdb (edam:format_1476), gro (edam:format_2033).
         output_structure_path (str): Path to the output structure file. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/ref_output_structure.pdb>`_. Accepted formats: pdb (edam:format_1476), gro (edam:format_2033).
         input_b_structure_path (str) (Optional): Path to the mutated input structure file. File type: input. Accepted formats: pdb (edam:format_1476), gro (edam:format_2033).
         properties (dic):
             * **mutation_list** (*str*) - ("2Ala") Mutation list in the format "Chain:Resnum MUT_AA_Code" or "Chain:Resnum MUT_NA_Code"  (no spaces between the elements) separated by commas. If no chain is provided as chain code all the chains in the pdb file will be mutated. ie: "A:15CYS". Possible MUT_AA_Code: 'ALA', 'ARG', 'ASN', 'ASP', 'ASPH', 'ASPP', 'ASH', 'CYS', 'CYS2', 'CYN', 'CYX', 'CYM', 'CYSH', 'GLU', 'GLUH', 'GLUP', 'GLH', 'GLN', 'GLY', 'HIS', 'HIE', 'HISE', 'HSE', 'HIP', 'HSP', 'HISH', 'HID', 'HSD', 'ILE', 'LEU', 'LYS', 'LYSH', 'LYP', 'LYN', 'LSN', 'MET', 'PHE', 'PRO', 'SER', 'SP1', 'SP2', 'THR', 'TRP', 'TYR', 'VAL'. Possible MUT_NA_Codes: 'A', 'T', 'C', 'G', 'U'.
```

### Comparing `biobb_pmx-4.1.0/biobb_pmx.egg-info/PKG-INFO` & `biobb_pmx-4.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: biobb-pmx
-Version: 4.1.0
+Name: biobb_pmx
+Version: 4.2.0
 Summary: Biobb_pmx is the Biobb module collection to perform PMX (http://pmx.mpibpc.mpg.de) executions.
 Home-page: https://github.com/bioexcel/biobb_pmx
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
-Project-URL: Documentation, http://biobb_pmx.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-pmx.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pmx?label=Version)](https://GitHub.com/bioexcel/biobb_pmx/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pmx.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pmx/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pmx?label=Conda)](https://anaconda.org/bioconda/biobb_pmx)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pmx?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pmx)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pmx?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pmx:4.1.0--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pmx)
 [![](https://img.shields.io/pypi/pyversions/biobb-pmx.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pmx/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pmx)
 
 [![](https://readthedocs.org/projects/biobb-pmx/badge/?version=latest&label=Docs)](https://biobb-pmx.readthedocs.io/en/latest/?badge=latest)
@@ -40,86 +40,93 @@
 
 [![](https://docs.bioexcel.eu/biobb_pmx/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_pmx/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_pmx/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_pmx/coverage/)
 [![](https://docs.bioexcel.eu/biobb_pmx/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_pmx/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_pmx?label=Last%20Commit)](https://github.com/bioexcel/biobb_pmx/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_pmx.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_pmx/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 
 # biobb_pmx
 
 ### Introduction
 Biobb_pmx is the Biobb module collection to perform PMX (http://pmx.mpibpc.mpg.de) executions.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_pmx.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-pmx.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2023.3
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
-        pip install "biobb_pmx>=4.1.0"
+        pip install "biobb_pmx>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pmx>=4.1.0"
+        conda install -c bioconda "biobb_pmx>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pmx.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pmx:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_pmx:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pmx:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_pmx:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pmx.sif https://depot.galaxyproject.org/singularity/biobb_pmx:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_pmx.sif https://depot.galaxyproject.org/singularity/biobb_pmx:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_pmx.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-pmx.readthedocs.io/en/latest/command_line.html).
 
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2022 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2022[Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_pmx-4.1.0/biobb_pmx.egg-info/SOURCES.txt` & `biobb_pmx-4.2.0/biobb_pmx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_pmx-4.1.0/setup.py` & `biobb_pmx-4.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_pmx",
-    version="4.1.0",
+    version="4.2.0",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="Biobb_pmx is the Biobb module collection to perform PMX (http://pmx.mpibpc.mpg.de) executions.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_pmx",
     project_urls={
-        "Documentation": "http://biobb_pmx.readthedocs.io/en/latest/",
+        "Documentation": "http://biobb-pmx.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs']),
-    install_requires=['biobb_common==4.1.0', 'pmx-biobb==4.1.3'],
+    install_requires=['biobb_common==4.2.0', 'pmx-biobb==4.1.3'],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
             "pmxanalyse = biobb_pmx.pmxbiobb.pmxanalyse:main",
             "pmxgentop = biobb_pmx.pmxbiobb.pmxgentop:main",
             "pmxmutate = biobb_pmx.pmxbiobb.pmxmutate:main",
             "pmxatom_mapping = biobb_pmx.pmxbiobb.pmxatom_mapping:main",
```

