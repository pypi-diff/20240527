# Comparing `tmp/sinto-0.8.4.tar.gz` & `tmp/sinto-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/tim/Documents/github/sinto/dist/tmpc69w1pue/sinto-0.8.4.tar", last modified: Mon Aug 15 15:07:12 2022, max compression
+gzip compressed data, was "sinto-0.9.0.tar", last modified: Wed Sep  7 20:39:59 2022, max compression
```

## Comparing `sinto-0.8.4.tar` & `sinto-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2022-08-15 15:07:12.897782 sinto-0.8.4/
--rw-r--r--   0 tim        (501) staff       (20)     1090 2022-08-12 13:33:36.000000 sinto-0.8.4/LICENSE
--rw-r--r--   0 tim        (501) staff       (20)     1536 2022-08-15 15:07:12.897862 sinto-0.8.4/PKG-INFO
--rw-r--r--   0 tim        (501) staff       (20)     1021 2022-08-12 13:33:36.000000 sinto-0.8.4/README.rst
--rw-r--r--   0 tim        (501) staff       (20)       98 2022-08-12 13:33:36.000000 sinto-0.8.4/pyproject.toml
--rw-r--r--   0 tim        (501) staff       (20)      688 2022-08-15 15:07:12.898187 sinto-0.8.4/setup.cfg
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2022-08-15 15:07:12.896644 sinto-0.8.4/sinto/
--rw-r--r--   0 tim        (501) staff       (20)       76 2022-08-12 13:33:36.000000 sinto-0.8.4/sinto/__init__.py
--rw-r--r--   0 tim        (501) staff       (20)     2260 2022-08-12 13:33:36.000000 sinto-0.8.4/sinto/addbarcodes.py
--rw-r--r--   0 tim        (501) staff       (20)     3055 2022-08-15 15:06:02.000000 sinto-0.8.4/sinto/addtags.py
--rw-r--r--   0 tim        (501) staff       (20)    12603 2022-08-12 13:33:36.000000 sinto-0.8.4/sinto/arguments.py
--rw-r--r--   0 tim        (501) staff       (20)     2851 2022-08-12 13:33:36.000000 sinto-0.8.4/sinto/cli.py
--rw-r--r--   0 tim        (501) staff       (20)       70 2022-08-12 13:33:36.000000 sinto-0.8.4/sinto/constants.py
--rw-r--r--   0 tim        (501) staff       (20)     4576 2022-08-15 15:06:02.000000 sinto-0.8.4/sinto/filterbarcodes.py
--rw-r--r--   0 tim        (501) staff       (20)    19085 2022-08-12 13:33:36.000000 sinto-0.8.4/sinto/fragments.py
--rw-r--r--   0 tim        (501) staff       (20)     1869 2022-08-12 13:33:36.000000 sinto-0.8.4/sinto/tagtoname.py
--rw-r--r--   0 tim        (501) staff       (20)     1919 2022-08-12 13:33:36.000000 sinto-0.8.4/sinto/tagtorg.py
--rw-r--r--   0 tim        (501) staff       (20)     1403 2022-08-12 13:33:36.000000 sinto-0.8.4/sinto/tagtotag.py
--rw-r--r--   0 tim        (501) staff       (20)     6108 2022-08-15 15:06:02.000000 sinto-0.8.4/sinto/utils.py
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2022-08-15 15:07:12.897678 sinto-0.8.4/sinto.egg-info/
--rw-r--r--   0 tim        (501) staff       (20)     1536 2022-08-15 15:07:12.000000 sinto-0.8.4/sinto.egg-info/PKG-INFO
--rw-r--r--   0 tim        (501) staff       (20)      438 2022-08-15 15:07:12.000000 sinto-0.8.4/sinto.egg-info/SOURCES.txt
--rw-r--r--   0 tim        (501) staff       (20)        1 2022-08-15 15:07:12.000000 sinto-0.8.4/sinto.egg-info/dependency_links.txt
--rw-r--r--   0 tim        (501) staff       (20)       47 2022-08-15 15:07:12.000000 sinto-0.8.4/sinto.egg-info/entry_points.txt
--rw-r--r--   0 tim        (501) staff       (20)       24 2022-08-15 15:07:12.000000 sinto-0.8.4/sinto.egg-info/requires.txt
--rw-r--r--   0 tim        (501) staff       (20)        6 2022-08-15 15:07:12.000000 sinto-0.8.4/sinto.egg-info/top_level.txt
+drwxr-xr-x   0 stuartt  (100014) satijalab (50000)        0 2022-09-07 20:39:59.468538 sinto-0.9.0/
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)     1090 2021-11-03 21:05:28.000000 sinto-0.9.0/LICENSE
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)     1536 2022-09-07 20:39:59.468538 sinto-0.9.0/PKG-INFO
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)     1021 2022-09-02 14:54:12.000000 sinto-0.9.0/README.rst
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)       98 2021-11-03 21:05:28.000000 sinto-0.9.0/pyproject.toml
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)      688 2022-09-07 20:39:59.468538 sinto-0.9.0/setup.cfg
+drwxr-xr-x   0 stuartt  (100014) satijalab (50000)        0 2022-09-07 20:39:59.468538 sinto-0.9.0/sinto/
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)       76 2021-11-03 21:05:28.000000 sinto-0.9.0/sinto/__init__.py
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)     2260 2021-11-03 21:05:28.000000 sinto-0.9.0/sinto/addbarcodes.py
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)     3055 2022-09-02 14:54:54.000000 sinto-0.9.0/sinto/addtags.py
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)    14584 2022-09-07 20:31:57.000000 sinto-0.9.0/sinto/arguments.py
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)     3954 2022-09-07 20:31:57.000000 sinto-0.9.0/sinto/blocks.py
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)     3239 2022-09-07 20:31:57.000000 sinto-0.9.0/sinto/cli.py
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)       70 2021-11-03 21:05:28.000000 sinto-0.9.0/sinto/constants.py
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)     4576 2022-09-02 14:54:54.000000 sinto-0.9.0/sinto/filterbarcodes.py
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)    19085 2022-09-02 14:54:12.000000 sinto-0.9.0/sinto/fragments.py
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)     1869 2022-05-04 02:02:50.000000 sinto-0.9.0/sinto/tagtoname.py
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)     1919 2021-11-03 21:05:28.000000 sinto-0.9.0/sinto/tagtorg.py
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)     1403 2021-11-03 21:05:28.000000 sinto-0.9.0/sinto/tagtotag.py
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)     6108 2022-09-02 14:54:54.000000 sinto-0.9.0/sinto/utils.py
+drwxr-xr-x   0 stuartt  (100014) satijalab (50000)        0 2022-09-07 20:39:59.468538 sinto-0.9.0/sinto.egg-info/
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)     1536 2022-09-07 20:39:59.000000 sinto-0.9.0/sinto.egg-info/PKG-INFO
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)      454 2022-09-07 20:39:59.000000 sinto-0.9.0/sinto.egg-info/SOURCES.txt
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)        1 2022-09-07 20:39:59.000000 sinto-0.9.0/sinto.egg-info/dependency_links.txt
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)       47 2022-09-07 20:39:59.000000 sinto-0.9.0/sinto.egg-info/entry_points.txt
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)       24 2022-09-07 20:39:59.000000 sinto-0.9.0/sinto.egg-info/requires.txt
+-rw-r--r--   0 stuartt  (100014) satijalab (50000)        6 2022-09-07 20:39:59.000000 sinto-0.9.0/sinto.egg-info/top_level.txt
```

### Comparing `sinto-0.8.4/LICENSE` & `sinto-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sinto-0.8.4/PKG-INFO` & `sinto-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinto
-Version: 0.8.4
+Version: 0.9.0
 Summary: Tools for single-cell data processing
 Home-page: https://timoast.github.io/sinto/
 Author: Tim Stuart
 Author-email: tstuart@nygenome.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/timoast/sinto/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sinto-0.8.4/README.rst` & `sinto-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `sinto-0.8.4/setup.cfg` & `sinto-0.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sinto
-version = 0.8.4
+version = 0.9.0
 url = https://timoast.github.io/sinto/
 project_urls = 
 	Bug Tracker = https://github.com/timoast/sinto/issues
 author = Tim Stuart
 author_email = tstuart@nygenome.org
 description = Tools for single-cell data processing
 long_description = file: README.rst
```

### Comparing `sinto-0.8.4/sinto/addbarcodes.py` & `sinto-0.9.0/sinto/addbarcodes.py`

 * *Files identical despite different names*

### Comparing `sinto-0.8.4/sinto/addtags.py` & `sinto-0.9.0/sinto/addtags.py`

 * *Files identical despite different names*

### Comparing `sinto-0.8.4/sinto/arguments.py` & `sinto-0.9.0/sinto/arguments.py`

 * *Files 15% similar despite different names*

```diff
@@ -343,22 +343,102 @@
     default=-5,
     type=int,
 )
 parser_fragments.add_argument(
     "--collapse_within",
     help="""
     Take cell barcode into account when collapsing duplicate fragments. Setting this
-    flag means that fragments with the same coordinates can be identified provided 
+    flag means that fragments with the same coordinates can be identified provided
     they originate from a different cell barcode.
     """,
     action="store_true",
     default=False,
 )
 parser_fragments.set_defaults(func=cli.run_fragments)
 
+# blocks
+parser_blocks = subparsers.add_parser(
+    "blocks", description="Create scRNA-seq block file from BAM file"
+)
+parser_blocks.add_argument(
+    "-b", "--bam", help="Input bam file (must be indexed)", required=True, type=str
+)
+parser_blocks.add_argument(
+    "--blocks",
+    help="""
+    Name and path for output blocks file. Note that the output is not sorted or compressed.
+    To sort the output file use sort -k 1,1 -k2,2n
+    """,
+    required=True,
+    type=str,
+)
+parser_blocks.add_argument(
+    "-m",
+    "--min_mapq",
+    help="Minimum MAPQ required to retain read (default = 30)",
+    required=False,
+    default=30,
+    type=int,
+)
+parser_blocks.add_argument(
+    "-p",
+    "--nproc",
+    help="Number of processors (default = 1)",
+    required=False,
+    type=int,
+    default=1,
+)
+parser_blocks.add_argument(
+    "-t",
+    "--barcodetag",
+    help='Read tag storing cell barcode information (default = "CB")',
+    required=False,
+    type=str,
+    default="CB",
+)
+parser_blocks.add_argument(
+    "-u",
+    "--umitag",
+    help='Read tag storing UMI barcode information (default = "UB")',
+    required=False,
+    type=str,
+    default="UB",
+)
+parser_blocks.add_argument(
+    "-c",
+    "--cells",
+    help="""
+    Path to file containing cell barcodes to retain, or a
+    comma-separated list of cell barcodes.
+    If None (default), use all cell barocodes present in the BAM file.
+    """,
+    required=False,
+    type=str,
+    default=None,
+)
+parser_blocks.add_argument(
+    "--barcode_regex",
+    help="""
+    Regular expression used to extract cell barcode from read name. If None (default), extract cell barcode from read tag.
+    Use "[^:]*" to match all characters up to the first colon.
+    """,
+    required=False,
+    type=str,
+    default=None,
+)
+parser_blocks.add_argument(
+    "--strand",
+    help="""
+    Include strand information in output file
+    """,
+    action="store_true",
+    default=False
+)
+parser_blocks.set_defaults(func=cli.run_blocks)
+
 # barcodes
 parser_barcode = subparsers.add_parser(
     "barcode", description="Add cell barcode sequences to read names in FASTQ file."
 )
 parser_barcode.add_argument(
     "--barcode_fastq", help="FASTQ file containing cell barcode sequences", required=True, type=str
 )
```

### Comparing `sinto-0.8.4/sinto/cli.py` & `sinto-0.9.0/sinto/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,22 @@
     utils,
     filterbarcodes,
     addtags,
     fragments,
     tagtorg,
     addbarcodes,
     tagtotag,
-    tagtoname
+    tagtoname,
+    blocks
 )
 
 
 @utils.log_info
 def run_filterbarcodes(options):
-    """Wraps the sctools.filterbarcodes function for use on the command line
+    """Wraps the sinto.filterbarcodes function for use on the command line
     """
     filterbarcodes.filterbarcodes(
         cells=options.cells,
         bam=options.bam,
         trim_suffix=options.trim_suffix,
         nproc=options.nproc,
         readname_barcode=options.barcode_regex,
@@ -24,30 +25,30 @@
         outdir=options.outdir,
         sam=options.sam
     )
 
 
 @utils.log_info
 def run_addtags(options):
-    """Wraps the sctools.addtags function for use on the command line
+    """Wraps the sinto.addtags function for use on the command line
     """
     addtags.addtags(
         bam=options.bam,
         tagfile=options.tagfile,
         trim_suffix=options.trim_suffix,
         output=options.output,
         sam=options.sam,
         nproc=options.nproc,
         mode=options.mode,
     )
 
 
 @utils.log_info
 def run_fragments(options):
-    """Wraps the sctools.fragments function for use on the command line
+    """Wraps the sinto.fragments function for use on the command line
     """
     fragments.fragments(
         bam=options.bam,
         fragment_path=options.fragments,
         min_mapq=options.min_mapq,
         nproc=options.nproc,
         cellbarcode=options.barcodetag,
@@ -70,14 +71,28 @@
         tag=options.tag,
         output=options.output,
         out_format=options.outputformat,
     )
 
 
 @utils.log_info
+def run_blocks(options):
+    blocks.blocks(
+        bam=options.bam,
+        block_path=options.blocks,
+        min_mapq=options.min_mapq,
+        nproc=options.nproc,
+        cellbarcode=options.barcodetag,
+        umibarcode=options.umitag,
+        readname_barcode=options.barcode_regex,
+        cells=options.cells,
+        include_strand=options.strand,
+    )
+
+@utils.log_info
 def run_tagtotag(options):
     tagtotag.tagtotag(
         bam=options.bam,
         from_tag=options.from_,
         to_tag=options.to,
         output=options.output,
         delete=options.delete,
```

### Comparing `sinto-0.8.4/sinto/filterbarcodes.py` & `sinto-0.9.0/sinto/filterbarcodes.py`

 * *Files identical despite different names*

### Comparing `sinto-0.8.4/sinto/fragments.py` & `sinto-0.9.0/sinto/fragments.py`

 * *Files identical despite different names*

### Comparing `sinto-0.8.4/sinto/tagtoname.py` & `sinto-0.9.0/sinto/tagtoname.py`

 * *Files identical despite different names*

### Comparing `sinto-0.8.4/sinto/tagtorg.py` & `sinto-0.9.0/sinto/tagtorg.py`

 * *Files identical despite different names*

### Comparing `sinto-0.8.4/sinto/tagtotag.py` & `sinto-0.9.0/sinto/tagtotag.py`

 * *Files identical despite different names*

### Comparing `sinto-0.8.4/sinto/utils.py` & `sinto-0.9.0/sinto/utils.py`

 * *Files identical despite different names*

### Comparing `sinto-0.8.4/sinto.egg-info/PKG-INFO` & `sinto-0.9.0/sinto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinto
-Version: 0.8.4
+Version: 0.9.0
 Summary: Tools for single-cell data processing
 Home-page: https://timoast.github.io/sinto/
 Author: Tim Stuart
 Author-email: tstuart@nygenome.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/timoast/sinto/issues
 Classifier: Programming Language :: Python :: 3
```

