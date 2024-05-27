# Comparing `tmp/klumpy-1.0.5.tar.gz` & `tmp/klumpy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klumpy-1.0.5.tar", last modified: Mon Feb 26 19:28:53 2024, max compression
+gzip compressed data, was "klumpy-1.0.6.tar", last modified: Mon May 27 17:08:57 2024, max compression
```

## Comparing `klumpy-1.0.5.tar` & `klumpy-1.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 giovannimadrigal   (501) staff       (20)        0 2024-02-26 19:28:53.392325 klumpy-1.0.5/
-drwxr-xr-x   0 giovannimadrigal   (501) staff       (20)        0 2024-02-26 19:28:53.387503 klumpy-1.0.5/Klumpy.egg-info/
--rw-r--r--   0 giovannimadrigal   (501) staff       (20)    54931 2024-02-26 19:28:53.000000 klumpy-1.0.5/Klumpy.egg-info/PKG-INFO
--rw-r--r--   0 giovannimadrigal   (501) staff       (20)      613 2024-02-26 19:28:53.000000 klumpy-1.0.5/Klumpy.egg-info/SOURCES.txt
--rw-r--r--   0 giovannimadrigal   (501) staff       (20)        1 2024-02-26 19:28:53.000000 klumpy-1.0.5/Klumpy.egg-info/dependency_links.txt
--rw-r--r--   0 giovannimadrigal   (501) staff       (20)        8 2024-02-26 19:28:53.000000 klumpy-1.0.5/Klumpy.egg-info/requires.txt
--rw-r--r--   0 giovannimadrigal   (501) staff       (20)        7 2024-02-26 19:28:53.000000 klumpy-1.0.5/Klumpy.egg-info/top_level.txt
--rw-r--r--   0 giovannimadrigal   (501) staff       (20)    35148 2024-02-01 01:45:16.000000 klumpy-1.0.5/LICENSE
--rw-r--r--   0 giovannimadrigal   (501) staff       (20)    54931 2024-02-26 19:28:53.392026 klumpy-1.0.5/PKG-INFO
--rw-------   0 giovannimadrigal   (501) staff       (20)    54391 2024-02-14 01:07:47.000000 klumpy-1.0.5/README.md
-drwxr-xr-x   0 giovannimadrigal   (501) staff       (20)        0 2024-02-26 19:28:53.391091 klumpy-1.0.5/klumpy/
--rw-------   0 giovannimadrigal   (501) staff       (20)    24850 2024-01-31 21:12:01.000000 klumpy-1.0.5/klumpy/Classes.py
--rw-------   0 giovannimadrigal   (501) staff       (20)     1237 2024-02-21 15:15:03.000000 klumpy-1.0.5/klumpy/__init__.py
--rw-------   0 giovannimadrigal   (501) staff       (20)    19492 2024-02-21 15:18:35.000000 klumpy-1.0.5/klumpy/__main__.py
--rw-------   0 giovannimadrigal   (501) staff       (20)    90126 2024-02-26 19:25:51.000000 klumpy-1.0.5/klumpy/alignment_plot.py
--rw-------   0 giovannimadrigal   (501) staff       (20)     2638 2024-02-01 00:59:59.000000 klumpy-1.0.5/klumpy/combine_klumps.py
--rw-------   0 giovannimadrigal   (501) staff       (20)     4173 2024-02-01 01:00:06.000000 klumpy-1.0.5/klumpy/find_gaps.py
--rw-------   0 giovannimadrigal   (501) staff       (20)    11432 2024-02-01 01:00:11.000000 klumpy-1.0.5/klumpy/find_klumps.py
--rw-------   0 giovannimadrigal   (501) staff       (20)     8391 2024-02-01 01:00:16.000000 klumpy-1.0.5/klumpy/get_exons.py
--rw-r--r--   0 giovannimadrigal   (501) staff       (20)    53205 2024-02-01 01:00:25.000000 klumpy-1.0.5/klumpy/grouping.py
--rw-------   0 giovannimadrigal   (501) staff       (20)    26309 2024-02-01 01:00:31.000000 klumpy-1.0.5/klumpy/klump_plot.py
--rw-------   0 giovannimadrigal   (501) staff       (20)     2807 2024-02-01 01:00:37.000000 klumpy-1.0.5/klumpy/klump_sizes.py
--rw-------   0 giovannimadrigal   (501) staff       (20)    15783 2024-02-20 22:51:38.000000 klumpy-1.0.5/klumpy/kmerize.py
--rw-------   0 giovannimadrigal   (501) staff       (20)    26529 2024-02-26 19:26:36.000000 klumpy-1.0.5/klumpy/scan_alignments.py
-drwxr-xr-x   0 giovannimadrigal   (501) staff       (20)        0 2024-02-26 19:28:53.391623 klumpy-1.0.5/scripts/
--rw-r--r--   0 giovannimadrigal   (501) staff       (20)       34 2024-02-13 23:02:24.000000 klumpy-1.0.5/scripts/klumpy
--rw-r--r--   0 giovannimadrigal   (501) staff       (20)       38 2024-02-26 19:28:53.392421 klumpy-1.0.5/setup.cfg
--rw-------   0 giovannimadrigal   (501) staff       (20)      820 2024-02-26 19:28:07.000000 klumpy-1.0.5/setup.py
+drwxr-xr-x   0 giovannimadrigal   (501) staff       (20)        0 2024-05-27 17:08:57.450551 klumpy-1.0.6/
+drwxr-xr-x   0 giovannimadrigal   (501) staff       (20)        0 2024-05-27 17:08:57.443014 klumpy-1.0.6/Klumpy.egg-info/
+-rw-r--r--   0 giovannimadrigal   (501) staff       (20)    56196 2024-05-27 17:08:57.000000 klumpy-1.0.6/Klumpy.egg-info/PKG-INFO
+-rw-r--r--   0 giovannimadrigal   (501) staff       (20)      613 2024-05-27 17:08:57.000000 klumpy-1.0.6/Klumpy.egg-info/SOURCES.txt
+-rw-r--r--   0 giovannimadrigal   (501) staff       (20)        1 2024-05-27 17:08:57.000000 klumpy-1.0.6/Klumpy.egg-info/dependency_links.txt
+-rw-r--r--   0 giovannimadrigal   (501) staff       (20)        8 2024-05-27 17:08:57.000000 klumpy-1.0.6/Klumpy.egg-info/requires.txt
+-rw-r--r--   0 giovannimadrigal   (501) staff       (20)        7 2024-05-27 17:08:57.000000 klumpy-1.0.6/Klumpy.egg-info/top_level.txt
+-rw-r--r--   0 giovannimadrigal   (501) staff       (20)    35148 2024-02-01 01:45:16.000000 klumpy-1.0.6/LICENSE
+-rw-r--r--   0 giovannimadrigal   (501) staff       (20)    56196 2024-05-27 17:08:57.450281 klumpy-1.0.6/PKG-INFO
+-rw-------   0 giovannimadrigal   (501) staff       (20)    55656 2024-05-26 22:18:44.000000 klumpy-1.0.6/README.md
+drwxr-xr-x   0 giovannimadrigal   (501) staff       (20)        0 2024-05-27 17:08:57.449055 klumpy-1.0.6/klumpy/
+-rw-------   0 giovannimadrigal   (501) staff       (20)    25519 2024-05-22 13:35:41.000000 klumpy-1.0.6/klumpy/Classes.py
+-rw-------   0 giovannimadrigal   (501) staff       (20)     1281 2024-05-27 16:17:29.000000 klumpy-1.0.6/klumpy/__init__.py
+-rw-------   0 giovannimadrigal   (501) staff       (20)    20461 2024-05-27 15:10:44.000000 klumpy-1.0.6/klumpy/__main__.py
+-rw-------   0 giovannimadrigal   (501) staff       (20)    91263 2024-05-27 15:41:31.000000 klumpy-1.0.6/klumpy/alignment_plot.py
+-rw-------   0 giovannimadrigal   (501) staff       (20)     2642 2024-05-24 21:50:07.000000 klumpy-1.0.6/klumpy/combine_klumps.py
+-rw-------   0 giovannimadrigal   (501) staff       (20)     4169 2024-05-27 15:43:07.000000 klumpy-1.0.6/klumpy/find_gaps.py
+-rw-------   0 giovannimadrigal   (501) staff       (20)    11492 2024-05-27 15:43:37.000000 klumpy-1.0.6/klumpy/find_klumps.py
+-rw-------   0 giovannimadrigal   (501) staff       (20)     8360 2024-05-27 15:43:57.000000 klumpy-1.0.6/klumpy/get_exons.py
+-rw-r--r--   0 giovannimadrigal   (501) staff       (20)    57181 2024-05-27 15:42:26.000000 klumpy-1.0.6/klumpy/grouping.py
+-rw-------   0 giovannimadrigal   (501) staff       (20)    26518 2024-05-24 22:12:41.000000 klumpy-1.0.6/klumpy/klump_plot.py
+-rw-------   0 giovannimadrigal   (501) staff       (20)     2831 2024-05-25 10:14:35.000000 klumpy-1.0.6/klumpy/klump_sizes.py
+-rw-------   0 giovannimadrigal   (501) staff       (20)    15862 2024-05-25 10:21:21.000000 klumpy-1.0.6/klumpy/kmerize.py
+-rw-------   0 giovannimadrigal   (501) staff       (20)    30818 2024-05-27 15:41:54.000000 klumpy-1.0.6/klumpy/scan_alignments.py
+drwxr-xr-x   0 giovannimadrigal   (501) staff       (20)        0 2024-05-27 17:08:57.449774 klumpy-1.0.6/scripts/
+-rw-r--r--   0 giovannimadrigal   (501) staff       (20)       34 2024-02-13 23:02:24.000000 klumpy-1.0.6/scripts/klumpy
+-rw-r--r--   0 giovannimadrigal   (501) staff       (20)       38 2024-05-27 17:08:57.450630 klumpy-1.0.6/setup.cfg
+-rw-------   0 giovannimadrigal   (501) staff       (20)      798 2024-05-27 16:21:52.000000 klumpy-1.0.6/setup.py
```

### Comparing `klumpy-1.0.5/Klumpy.egg-info/PKG-INFO` & `klumpy-1.0.6/Klumpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klumpy
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package to evaluate genome assemblies and detect sequence motifs
 Author: Giovanni Madrigal <gm33@illinois.edu>, Bushra Fazal Minhas <bfazal2@illinois.edu>, Julian Catchen <jcatchen@illinois.edu>
 Author-email: gm33@illinois.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.6.0
@@ -16,14 +16,16 @@
 Initially developed to verify the Antifreeze glycoproteins in the genomes of two icefishes (see [Rivera-Colón, 2023](https://academic.oup.com/mbe/article/40/3/msad029/7035026)), `klumpy` now has expanded to include a suite of tools for assessing whether a particular region in a genome assembly is missassembled by leveraging the original data (i.e., raw reads) used in the assembly process, or it can instead be used to search for a gene of interest in a set of sequences. Complete overview of the software and the methods used in the paper can be viewed at [here](https://bitbucket.org/Gio12/klumpy/src/master/).
 
 # Installation
 ```
 python3 -m pip install klumpy
 ```
 
+**NOTE**: `klumpy` uses `samtools` to parse *.bam* / *.sam* files, so `samtools` should be installed and available in the current path when providing `klumpy` an alignment file. 
+
 # Components
 
 `klumpy` currently is composed of 9 different subprograms, two are which are the primary subprograms, two which can illustrate the results, with the remaining 5 designed to supplement the four other subprograms. Depending on whether you have a gene of interest, as in the case with the Icefishes and AFGPs, you can start the analysis with `find_klumps`. If the aim is to assess the quality of your reference genome, the `scan_alignment` analysis would flag regions that were possibly missassembled.
 
 ```
 # primary subprograms
     find_klumps:                Find query klumps in a set of subject sequences
@@ -120,56 +122,69 @@
         --t_len:                    Minimum length a sequence must be in order to trust its assignment when grouping (default = 2000)
         --t_per:                    Minimum percentage a sequence must be aligned in order to trust its assignment when grouping (default = 30)
         --align_offset:             Maximum number of base pairs apart for two sequences to be considered aligned at the same position (default = 100)
         --min_grp:                  Minimum number of sequences in a group in order to retain the group (default = 2)
         --window_size:              Length (in bp) for the sliding window to be (default = 50000)
         --window_step:              Length (in bp) for the sliding window to slide down to establish the next window (default = 25000) 
         --limit:                    Maximum number of alignments to process in a window (default 10000)
+        --flag_excess_groups:       If set, will report regions with greater than or equal to --num_of_groups parameter regardless if the region was tiled or not
 ```
 With the exception of `--threads`, the main parameters are shared with `alignment_plot`. Here, a sliding window approach is implemented, and at each window, `klumpy`'s grouping algorithm is performed (see *Advanced options* under the `alignment_plot` section). The use of multiple threads (i.e., the `--threads` argument) is only useful if the alignment map contains more than 1 *reference* sequence (parallelization is implemented across reference sequences, not alignment records).
 
 To perform a scan, one can run a command similar to this
 ```
 klumpy scan_alignments --alignment_map input.bam --threads 16
 ```
 Here, we used the default parameters of using sequences with a length of at least 2 Kbp (set by `--min_len`), with the default `--min_percent` value of 50, meaning that sequences where more than a quarter of the sequence are unmapped, are not retained in the scanning process.
 
-The `--num_of_groups` argument sets the minimum number of groups a region must have in order for the region to be flagged as a possible missassembly. If a *.gtf* or *.gff* file is provided to `--annotation`, only regions containing a gene will be processed (useful if you are only interested in annotated regions).
+The `--num_of_groups` argument sets the minimum number of groups a region must have in order to flag a region to be flagged as a possible missassembly if the `--flag_excess_groups` is set. If a *.gtf* or *.gff* file is provided to `--annotation`, only regions containing a gene will be processed (useful if you are only interested in annotated regions).
 
 When running this software, temporary files will be written to disk using the naming scheme *Temp_seq_name.txt*, where the *seq_name* is the name of the reference sequence being scanned. **DO NOT DISGARD THESE FILES**, they will be removed after the data is merged. 
 
 The temporary files contain flagged *windows* that look something like this
 ```
-seq 400000  425000
-seq 750000  775000
-seq 775000  800000
+seq 400000  425000  1
+seq 750000  775000  1
+seq 775000  800000  2
 ```
 
-Where the first column contains the sequence name, the second column the start position of the window, and the third column contains the end position of the window. If an annotation file is provided, the temporary file would contain an additional column
+Where the first column contains the sequence name, the second column the start position of the window, the third column contains the end position of the window, and the fourth columm contains the number of groups found. If an annotation file is provided, the temporary file would contain an additional column
 ```
-seq 400000  425000  geneA,geneB,geneC
-seq 750000  775000  geneX,geneY
-seq 775000  800000  geneY,geneZ
+seq 400000  425000  1   geneA,geneB,geneC
+seq 750000  775000  1   geneX,geneY
+seq 775000  800000  2   geneY,geneZ
 ```
 
-Where the fourth column is added with a comma separated list containing the genes found in the window. 
+Where the fifth column is added with a comma separated list containing the genes found in the window. Lastly, if using the `--flag_excess_groups` option, an additional column containing either a *T* or a *F* will be added between the third and fourth column to indicate whether the region was tiled (*T* or True) or not (*F* or False).
+
+```
+seq 400000  425000  F   1   geneA,geneB,geneC
+seq 750000  775000  F   1   geneX,geneY
+seq 775000  800000  T   2   geneY,geneZ
+```
 
 Once all the reference sequences have been scanned, they are merged into a single file. The output file will contain the same name as in the alignment map, with the added extension of *_Candidate_Regions.tsv*. For example, if the input was called *input.bam*, the output would be *input_Candidate_Regions.tsv*. Using the examples above, the resulting output would like this
 
 ```
 # klumpy scan_alignments --alignment_map input.bam --threads 16
-Region_Num  Reference_Seq   Start   End
-1   seq 400000  425000
-2   seq 750000  800000
+Region_Num  Reference_Seq   Start   End Number_of_Groups
+1   seq 400000  425000  1
+2   seq 750000  800000  1,2
 
 # with annotation file provided
 # klumpy scan_alignments --alignment_map input.bam --threads 16 --annotation input.gtf.gz
-Region_Num  Reference_Seq   Start   End Genes
-1   seq 400000  425000  geneA,geneB,geneC
-2   seq 750000  800000  geneX,geneY,geneZ
+Region_Num  Reference_Seq   Start   End Number_of_Groups    Genes
+1   seq 400000  425000  1 geneA,geneB,geneC
+2   seq 750000  800000  1,2 geneX,geneY,geneZ
+
+# with annotation file provided & flagging regions based on group number
+# klumpy scan_alignments --alignment_map input.bam --threads 16 --annotation input.gtf.gz --flag_excess_groups
+Region_Num  Reference_Seq   Start   End Tiled Number_of_Groups Genes
+1   seq 400000  425000  F, 1 geneA,geneB,geneC
+2   seq 750000  800000  F,T 1,2 geneX,geneY,geneZ
 ```
 
 The first line of the output will contain the line of code provided used to start the analysis, while the second line contains the column headers. Here, *regions* are reported instead of windows since `klumpy` will collapse overlapping windows since they represent the same locus. Th *Reference_Seq* column contains the name of the reference sequence, and the *Start* and *End* columns contain positions of the region (**NOTE** these are 0-based positions). The *Genes* column is optionally added if an annotation file was used in the analysis. If a desired window is of interest, the *_Candidate_Regions.tsv* output can be supplied to `alignment_plot` using the `--candidates` option in combination with the `--region_num` argument to specify which region `klumpy` should plot instead of explicitly using `--reference`, `--leftbound`, and `--rightbound`.
 
 #### Advanced options
 
 The `scan_alignments` subprogram shares the majority of its arguments with `alignment_plot`, which both implement the grouping algorithm. New arguments include `--window_size` and `--window_step`. The software runs a sliding window across each reference sequence in the alignment map (i.e., a *SAM*/*BAM* file), and applies the grouping algorithm at each window. The size of the window is determined by `--window_size` (defaults to 50 Kb) and the sliding distance is set by `--window_step` (default = 25 Kb). Reference sequences that are shorter than `--window_size` are ignored. 
@@ -204,35 +219,35 @@
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue
 ```
 
 The resulting file is written by default in pdf format, but can be changed using the `--format` option, which accepts either *pdf*, *png* or *svg* as a value. The ouput file will have the same name as the file passed to `--klumps_tsv`. For example, the output for *input_klumps.tsv* would be *input_klumps.pdf*. Below is an example of 6 sequences
 
 <p align="center">
-<img src="Images/klump_plot_example1.png" alt="drawing" style="width:800px;height:200px"/>
+<img src="./Images/klump_plot_example1.png" alt="drawing" style="width:600px;height:300px"/>
 </p>
 
 Sequences are sorted by sequence length, with the shortest sequence at the top, and the longest sequence at the bottom. Furthermore, since the number of sequences to plot is unknown, the height of the pdf is extended so that each sequence is equally spaced apart. The klump labels begin with the number of k-mers in the klump, separated by a **-** from the name of the query source.
 
 If using the `--fix_width` flag is implemented, there will be no relative scaling done on the sequences.
 
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue --fix_width
 ```
 <p align="center">
-<img src="Images/klump_plot_example2.png" alt="drawing" style="width:800px;height:200px"/>
+<img src="./Images/klump_plot_example2.png" alt="drawing" style="width:600px;height:300px"/>
 </p>
 
 In the case in which you are interested in a particular locus in a specific sequence, the `--seq_name` flags can be used.
 
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue --seq_name Seq4
 ```
 <p align="center">
-<img src="Images/klump_plot_example3.png" alt="drawing" style="width:800px;height:100px"/>
+<img src="./Images/klump_plot_example3.png" alt="drawing" style="width:600px;height:100px"/>
 </p>
 
 If the sequences contain gaps, the output of `find_gaps` can be used to annotate the figure with the sequence gaps (see `./TestCases/TestCases.md` for an example where we viewed gaps across several *Bombus* reference genomes)
 
 ### Advanced options
 
 The `--klump_colors` and `--color_by_gene` parameters accept a *.tsv* file and uses that to map a color to a specific query source. If the color is unavailable, the program will report back to the user the error and exit. Not every query source needs to be present in the *.tsv* file, as those unlisted sources will be defaulted to a blue color. An example of an acceptable tab-delimited file is shown below
@@ -246,42 +261,42 @@
 Query6  cyan
 ```
 Assuming the file is named *klump_colors.tsv*, the following command illustrates its use
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --fix_width --klump_colors klump_colors.tsv
 ```
 <p align="center">
-<img src="Images/klump_plot_example_colors.png" alt="drawing" style="width:800px;height:200px"/>
+<img src="./Images/klump_plot_example_colors.png" alt="drawing" style="width:600px;height:300px"/>
 </p>
 
 The file supplied to `--color_by_gene` is treated differently, as this argument was designed to work with the results of the `get_exons` subprogram. Sequences obtained with `get_exons` will have the extension *_EN* in the sequence header, where *E* is short for Exon and *N* is for the *N*<sup>th</sup> exon. So if using the above example, all klumps with *query1_E[N]* will be colored blue (*N* being any number).
 
 To view a specific region in a specific sequence in the klumps *.tsv* file, the `--leftbound` and `--rightbound` parameters can be used.
 
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue --seq_name Seq4 --leftbound 5e3 --rightbound 7e3
 ```
 <p align="center">
-<img src="Images/klump_plot_example4.png" alt="drawing" style="width:800px;height:100px"/>
+<img src="./Images/klump_plot_example4.png" alt="drawing" style="width:600px;height:100px"/>
 </p>
 
 Further customization can be performed with the `--tick_count` and `--tick_span` parameters, both of which are only implemented when viewing a single sequence. `--tick_count` specifies the number of tick markers in the drawing, while `--tick_span` will set the length (in base pairs) between tick markers.
 
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue --seq_name Seq4 --tick_count 20
 ```
 <p align="center">
-<img src="Images/klump_plot_example5.png" alt="drawing" style="width:800px;height:100px"/>
+<img src="./Images/klump_plot_example5.png" alt="drawing" style="width:600px;height:100px"/>
 </p>
 
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue --seq_name Seq4 --tick_span 2e3
 ```
 <p align="center">
-<img src="Images/klump_plot_example6.png" alt="drawing" style="width:800px;height:100px"/>
+<img src="./Images/klump_plot_example6.png" alt="drawing" style="width:600px;height:100px"/>
 </p>
 
 # kmerize
 The `kmerize` subprogram performs the `--query` search in the `--subject` sequences implemented by `find_klumps`. A *query_map.gz* file will be generated, but no klump construction will be performed. All parameters available to `kmerize` are those which are also available to `find_klumps` (see `find_klumps` section for details ).
 
 ```
     --subject:                  Subject sequences in FAST[A|Q] format [Required]    
@@ -450,21 +465,21 @@
                       --leftbound 4.47e6 \    # could use 4470000
                       --rightbound 4.55e6 \   # could use 4550000
                       --min_len 1e4 \         # can use 10000
                       --min_percent 50        # could use 0.50
 ```
 The output will resemble something along the lines of what is shown below
 <p align="center">
-<img src="Images/align_plot1.png" width="50%" height="75%">
+<img src="./Images/align_plot1.png" width="50%" height="75%">
 </p>
 
 
 The leftmost postitioned sequence is placed at the top, with the rightmost sequence positioned at the bottom (excluding the reference sequence). The alignments either are a light grey, indicating a forward alignment (in respect to the reference genome), or a shade of yellow, which represent alignments on the reverse strand of the reference genome. Several other features are shown here, notably deletions and clips.
 <p align="center">
-<img src="Images/align_plot1_zoom.png" width="50%" height="100%">
+<img src="./Images/align_plot1_zoom.png" width="50%" height="100%">
 </p>
 
 Zooming in, there are horizontal black lines that separate the blocks of the aligned portions of the sequence. These black lines represent deletions. Data such as Pac-Bio are known to have many small indels. As these may be due to sequencing errors as opposed to real biological indels, viewing these small indels may not benefit the user. By default, the `--deletion_len` argument is set to 100 (*Note* that this is an advanced parameter that). In other words, `klumpy` will draw deletions that are at least 100 bp in length. As insertions do not consume the reference sequence, they are ignored. The light green extensions from the alignment represent soft clips in the alignment, while red lines extending from the alignment would indicate hard clips (not shown in example).
 
 Additional annotation files that can be provided include `--gap_file` (file generated from `find_gaps`) and `--annotation`, which takes a *.gtf* or *.gff* file (can be compresssed) as input. Both these two files will annotate the reference sequence with any features located within region. For further annotation, `--vertical_line_gaps`, `--vertical_line_klumps`, and `--vertical_line_exons` will draw a dashed line above the desired feature in the reference sequence.
 
 Example with `--annotation`.
@@ -476,20 +491,20 @@
                       --min_len 1e4 \         # could use 10000
                       --min_percent 50 \      # could use 0.50
                       --annotation cgun.gtf.gz
 ```
 
 The output will resememble something along the lines of what is shown below
 <p align="center">
-<img src="Images/align_plot2.png" width="50%" height="100%">
+<img src="./Images/align_plot2.png" width="50%" height="100%">
 </p>
 
 Here, each gene is differentiated by its color. For example, gene *g_9529* is red while gene *g_16157* is a lighter blue. Each separate annotation represents an exon, with the first exon in the image for each gene being tagged with the name of the gene. Gene labels alternate in position, where one gene's label is drawn on top of the reference sequence, and the following gene's label will be drawn below the reference sequence. If a third gene is drawn, its label will then be drawn above the reference sequence and the pattern continues.
 <p align="center">
-<img src="Images/align_plot2_zoom.png" width="50%" height="100%">
+<img src="./Images/align_plot2_zoom.png" width="50%" height="100%">
 </p>
 
 Plotting a region where a gap is located, we can see the following
 ```
 klumpy alignment_plot --alignment_map cgun_raw_reads.bam \
                       --reference 24 \
                       --leftbound 13.07e6 \    # could use 13070000
@@ -497,15 +512,15 @@
                       --min_len 1e4 \         # could use 10000
                       --min_percent 50 \      # could use 0.50
                       --annotation cgun.gtf.gz \
                       --gap_file cgun_gaps.tsv \
                       --vertical_line_gaps    # no input needed
 ```
 <p align="center">
-<img src="Images/align_plot3.png", width="50%" height="100%">
+<img src="./Images/align_plot3.png", width="50%" height="100%">
 </p>
 
 Here, it is clear that the gap connecting two contigs is directly below a deletion in several alignments. 
 
 To present an example with klumps, we will annotate one of the *afgp* regions in our assembly & alignments.
 ```
 klumpy alignment_plot --alignment_map cgun_raw_reads.bam \
@@ -518,15 +533,15 @@
                       --gap_file cgun_gaps.tsv \
                       --vertical_line_gaps \# no input needed
                       --klumps_tsv afgp_klumps.tsv
 ```
 
 Here, it is clear that there is a gapless region containing relatively few AFGP loci in the Mackerel Icefish
 <p align="center">
-<img src="Images/klumps_align_example.png" width="50%" height="100%">
+<img src="./Images/klumps_align_example.png" width="50%" height="100%">
 </p>
 
 The `--group_seqs` argument does not accept any input (i.e., just include the parameter in your command) and groups the sequences using `klumpy`'s grouping algorithm (see *Advanced options* for detials)
 
 ## Advanced options
 
 By default, only primary alignments are visualized, with the available options `--secondary` and `--supplementary` that can relax this constraint. To exclude primary alignments, simply use the flag `--no_primary`.
@@ -570,15 +585,15 @@
                       --annotation cgun.gtf.gz \
                       --number \              # no input needed
                       --write_table           # no input needed
 ```
 
 Zoomed in for clarity
 <p align="center">
-<img src="Images/num_zoom.png" width="50%" height="100%">
+<img src="./Images/num_zoom.png" width="50%" height="100%">
 </p>
 
 
 To plot paired-end data, you **must** use the `--paired` flag. The plotting scheme is different for paired-end data, where the pair of sequences are plotted on the same line, and `R1` sequences are plotted in green, and `R2` are colored as blue. 
 
 Illustrating an example with some Restriction-site Associated Sequencing (RAD-Seq) data.
 ```
@@ -588,15 +603,15 @@
                       --rightbound 1.71e5 \   # could use 171000
                       --min_len 100 \         # min length should be set for short reads
                       --min_percent 50 \      # could use 0.50
                       --annotation cgun.gtf.gz \
                       --paired                # no input needed
 ```
 <p align="center">
-<img src="Images/paired_align.png" width="50%" height="100%">
+<img src="./Images/paired_align.png" width="50%" height="100%">
 </p>
 
 Here, the reads are aligned right at an exon of `cdk15`, which is a *cyclin-dependent kinase*.
 
 `--group_seqs` is used to signal to `klumpy` to attempt to group the alignments based on their alignment patterns. Before describing some of the parameters, it must be noted that the grouping algorithm is **only** applied on *primary* alignments and *non-paired-end* data.
 
 The grouping algorithm first starts by trying to group "good" alignments (i.e., alignments without large deletions or clipping). This is based on the assumption that alignments in missassembled regions tend to have features such as clipping and deletions. Most of the grouping-specific featuers are designed to work with these features.
@@ -604,31 +619,31 @@
 First, the `--assume_sep_del` flag is used to *turn off* the assumption that alignments with deletions *should* be grouped together if there is their deletions span the same region in the reference. The `--per_overlap` takes a percentage (e.g., 50 or 0.50), which sets the minimum percentage that alignments need to overlap one another (i.e., both alignments need to overlap each other by `--per_overlap`) to be *considered* a good match (i.e., this alone does not result in the two alignments being grouped together).
 
 The `--t_len` and `--t_per` arguments work similarly to `--min_len` and `--min_percent`. The `--t_len` argument is used to set the "trust" length, which any *sequence* below this length will be ignored when grouping as it is assumed to be untrustworthy. Likewise, any *sequence* with an aligned percentage lower than `--t_per` is also ignored when grouping. The rationale for these parameters is to avoid trying to bin short and poorly aligned sequences that cannot be reliably placed into a single group.
 
 The `--clip_tolerance` argument is used to set the number of clipped base pairs that can be tolerated between two alignments. Below is a simple case.
 
 <p align="center">
-<img src="Images/clip_tolerance.png" width="50%" height="100%">
+<img src="./Images/clip_tolerance.png" width="50%" height="75%">
 </p>
 
 Here, a clip from alignment B is overlapping an aligned portion of alignment A. If `--clip_tolerance` is shorter than the *clip overlap*, the two alignments are considered incompatible. Otherwise, they can still be compatible. 
 
 The `--del_tolerance` is similar to `--clip_tolerance`, except that it evaluates the deletion overlaps.
 
 <p align="center">
-<img src="Images/del_tolerance.png" width="50%" height="100%">
+<img src="./Images/del_tolerance.png" width="50%" height="75%">
 </p>
 
 If the value provided to `--del_tolerance` is shorter than the *deletion overlap*, then the two sequences are considered incompatible.
 
 In `--group_seqs`, alignments that begin at the same position are assumed to represent the same locus, as it is reasonable to assume the two sequences are of the same origin if starting at the same site. Since two alignments may not *exactly* align at the same position, but can be loosely interpretted as aligning to the same position, the `--align_offset` provides some wiggle room.
 
 <p align="center">
-<img src="Images/align_offset.png" width="50%" height="100%">
+<img src="./Images/align_offset.png" width="50%" height="75%">
 </p>
 
 The offset applies both to the left and right side of the aligned portions of an alignment (here, alignment A). For visual purposes, only alignment A is being checked in the illustration, but this evaluation is also applied from the perspective of alignment B.
 
 
 To illustrate a simple case, we will apply the grouping algorithm to a 50 Kb region on chromosome 3 using default parameters
 
@@ -639,15 +654,15 @@
                       --rightbound 10.25e6 \    # could use 4550000
                       --min_len 2.5e4 \         # 25 Kb
                       --min_percent 75 \        # same as 0.75
                       --annotation cgun.gtf.gz \
                       --group_seqs              # no input needed
 ```
 <p align="center">
-<img src="Images/group_align_example1.png" width="50%" height="100%">
+<img src="./Images/group_align_example1.png" width="50%" height="100%">
 </p>
 
 Here, the sequence alignments are colored based on the group they were assigned to. Alignments that are ungrouped are left white. Here, there are two groups. 
 
 To illustrate an unresolved region, we will focus on a region where the algorithm struggles to find 2 or less groups while keeping the parameters the same. Additionally, we will annotate the image with the gaps in the region.
 
 ```
@@ -659,23 +674,23 @@
                       --min_percent 85 \            # same as 0.85
                       --annotation cgun.gtf.gz \
                       --group_seqs \                # no input needed
                       --gap_file cgun_gaps.tsv \
                       --vertical_line_gaps          # no input needed
 ```
 <p align="center">
-<img src="Images/misassemble_example.png" width="50%" height="100%">
+<img src="./Images/misassemble_example.png" width="50%" height="100%">
 </p>
 
 Within this 180 Kb region, 4 contigs are stitched together as indicated by the 3 gaps (stretches of *N*'s). Interestingly, the third contig (~6.99 Mb - 7.65 Mb) was predicted to be composed of three groups, with two of the groups having some overlap with each other. In this example, `klumpy` predicts 12 groups within this region. Although this is likely to not be the true number of groups, the binning of sequences into their respective groups can aid in the reconstruction of problematic loci.
 
 The remaining grouping-based arguments are `--min_grp`, `--write_groups` and `--write_edge_seqs`. The `--min_grp` flag accepts an integer to set as the minimum number of sequences required to form a group. The `--write_groups` flag is set to tell the program to write the groups to group-specific fasta files, which can be used for tasks such as local reassemblies or annotations. If your interests are more on clipped sequences at the ends/edges of the groups, implementing the `--write_edge_seqs` will write out the names of the clipped sequences at the ends/edges of the groups into group-specific *.txt* files. The following image highlights some of the edge sequences from above.
 
 <p align="center">
-<img src="Images/edge_seqs_example.png" width="50%" height="100%">
+<img src="./Images/edge_seqs_example.png" width="50%" height="100%">
 </p>
 
 # get_exons
 
 The purpose of this subprogram is to take a list of genes, and extract out their exonic sequences from a reference assembly. All arguments are required for this program.
 ```
     --fasta:                    Reference genome in fasta format [Required]
```

### Comparing `klumpy-1.0.5/Klumpy.egg-info/SOURCES.txt` & `klumpy-1.0.6/Klumpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `klumpy-1.0.5/LICENSE` & `klumpy-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `klumpy-1.0.5/PKG-INFO` & `klumpy-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klumpy
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package to evaluate genome assemblies and detect sequence motifs
 Author: Giovanni Madrigal <gm33@illinois.edu>, Bushra Fazal Minhas <bfazal2@illinois.edu>, Julian Catchen <jcatchen@illinois.edu>
 Author-email: gm33@illinois.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.6.0
@@ -16,14 +16,16 @@
 Initially developed to verify the Antifreeze glycoproteins in the genomes of two icefishes (see [Rivera-Colón, 2023](https://academic.oup.com/mbe/article/40/3/msad029/7035026)), `klumpy` now has expanded to include a suite of tools for assessing whether a particular region in a genome assembly is missassembled by leveraging the original data (i.e., raw reads) used in the assembly process, or it can instead be used to search for a gene of interest in a set of sequences. Complete overview of the software and the methods used in the paper can be viewed at [here](https://bitbucket.org/Gio12/klumpy/src/master/).
 
 # Installation
 ```
 python3 -m pip install klumpy
 ```
 
+**NOTE**: `klumpy` uses `samtools` to parse *.bam* / *.sam* files, so `samtools` should be installed and available in the current path when providing `klumpy` an alignment file. 
+
 # Components
 
 `klumpy` currently is composed of 9 different subprograms, two are which are the primary subprograms, two which can illustrate the results, with the remaining 5 designed to supplement the four other subprograms. Depending on whether you have a gene of interest, as in the case with the Icefishes and AFGPs, you can start the analysis with `find_klumps`. If the aim is to assess the quality of your reference genome, the `scan_alignment` analysis would flag regions that were possibly missassembled.
 
 ```
 # primary subprograms
     find_klumps:                Find query klumps in a set of subject sequences
@@ -120,56 +122,69 @@
         --t_len:                    Minimum length a sequence must be in order to trust its assignment when grouping (default = 2000)
         --t_per:                    Minimum percentage a sequence must be aligned in order to trust its assignment when grouping (default = 30)
         --align_offset:             Maximum number of base pairs apart for two sequences to be considered aligned at the same position (default = 100)
         --min_grp:                  Minimum number of sequences in a group in order to retain the group (default = 2)
         --window_size:              Length (in bp) for the sliding window to be (default = 50000)
         --window_step:              Length (in bp) for the sliding window to slide down to establish the next window (default = 25000) 
         --limit:                    Maximum number of alignments to process in a window (default 10000)
+        --flag_excess_groups:       If set, will report regions with greater than or equal to --num_of_groups parameter regardless if the region was tiled or not
 ```
 With the exception of `--threads`, the main parameters are shared with `alignment_plot`. Here, a sliding window approach is implemented, and at each window, `klumpy`'s grouping algorithm is performed (see *Advanced options* under the `alignment_plot` section). The use of multiple threads (i.e., the `--threads` argument) is only useful if the alignment map contains more than 1 *reference* sequence (parallelization is implemented across reference sequences, not alignment records).
 
 To perform a scan, one can run a command similar to this
 ```
 klumpy scan_alignments --alignment_map input.bam --threads 16
 ```
 Here, we used the default parameters of using sequences with a length of at least 2 Kbp (set by `--min_len`), with the default `--min_percent` value of 50, meaning that sequences where more than a quarter of the sequence are unmapped, are not retained in the scanning process.
 
-The `--num_of_groups` argument sets the minimum number of groups a region must have in order for the region to be flagged as a possible missassembly. If a *.gtf* or *.gff* file is provided to `--annotation`, only regions containing a gene will be processed (useful if you are only interested in annotated regions).
+The `--num_of_groups` argument sets the minimum number of groups a region must have in order to flag a region to be flagged as a possible missassembly if the `--flag_excess_groups` is set. If a *.gtf* or *.gff* file is provided to `--annotation`, only regions containing a gene will be processed (useful if you are only interested in annotated regions).
 
 When running this software, temporary files will be written to disk using the naming scheme *Temp_seq_name.txt*, where the *seq_name* is the name of the reference sequence being scanned. **DO NOT DISGARD THESE FILES**, they will be removed after the data is merged. 
 
 The temporary files contain flagged *windows* that look something like this
 ```
-seq 400000  425000
-seq 750000  775000
-seq 775000  800000
+seq 400000  425000  1
+seq 750000  775000  1
+seq 775000  800000  2
 ```
 
-Where the first column contains the sequence name, the second column the start position of the window, and the third column contains the end position of the window. If an annotation file is provided, the temporary file would contain an additional column
+Where the first column contains the sequence name, the second column the start position of the window, the third column contains the end position of the window, and the fourth columm contains the number of groups found. If an annotation file is provided, the temporary file would contain an additional column
 ```
-seq 400000  425000  geneA,geneB,geneC
-seq 750000  775000  geneX,geneY
-seq 775000  800000  geneY,geneZ
+seq 400000  425000  1   geneA,geneB,geneC
+seq 750000  775000  1   geneX,geneY
+seq 775000  800000  2   geneY,geneZ
 ```
 
-Where the fourth column is added with a comma separated list containing the genes found in the window. 
+Where the fifth column is added with a comma separated list containing the genes found in the window. Lastly, if using the `--flag_excess_groups` option, an additional column containing either a *T* or a *F* will be added between the third and fourth column to indicate whether the region was tiled (*T* or True) or not (*F* or False).
+
+```
+seq 400000  425000  F   1   geneA,geneB,geneC
+seq 750000  775000  F   1   geneX,geneY
+seq 775000  800000  T   2   geneY,geneZ
+```
 
 Once all the reference sequences have been scanned, they are merged into a single file. The output file will contain the same name as in the alignment map, with the added extension of *_Candidate_Regions.tsv*. For example, if the input was called *input.bam*, the output would be *input_Candidate_Regions.tsv*. Using the examples above, the resulting output would like this
 
 ```
 # klumpy scan_alignments --alignment_map input.bam --threads 16
-Region_Num  Reference_Seq   Start   End
-1   seq 400000  425000
-2   seq 750000  800000
+Region_Num  Reference_Seq   Start   End Number_of_Groups
+1   seq 400000  425000  1
+2   seq 750000  800000  1,2
 
 # with annotation file provided
 # klumpy scan_alignments --alignment_map input.bam --threads 16 --annotation input.gtf.gz
-Region_Num  Reference_Seq   Start   End Genes
-1   seq 400000  425000  geneA,geneB,geneC
-2   seq 750000  800000  geneX,geneY,geneZ
+Region_Num  Reference_Seq   Start   End Number_of_Groups    Genes
+1   seq 400000  425000  1 geneA,geneB,geneC
+2   seq 750000  800000  1,2 geneX,geneY,geneZ
+
+# with annotation file provided & flagging regions based on group number
+# klumpy scan_alignments --alignment_map input.bam --threads 16 --annotation input.gtf.gz --flag_excess_groups
+Region_Num  Reference_Seq   Start   End Tiled Number_of_Groups Genes
+1   seq 400000  425000  F, 1 geneA,geneB,geneC
+2   seq 750000  800000  F,T 1,2 geneX,geneY,geneZ
 ```
 
 The first line of the output will contain the line of code provided used to start the analysis, while the second line contains the column headers. Here, *regions* are reported instead of windows since `klumpy` will collapse overlapping windows since they represent the same locus. Th *Reference_Seq* column contains the name of the reference sequence, and the *Start* and *End* columns contain positions of the region (**NOTE** these are 0-based positions). The *Genes* column is optionally added if an annotation file was used in the analysis. If a desired window is of interest, the *_Candidate_Regions.tsv* output can be supplied to `alignment_plot` using the `--candidates` option in combination with the `--region_num` argument to specify which region `klumpy` should plot instead of explicitly using `--reference`, `--leftbound`, and `--rightbound`.
 
 #### Advanced options
 
 The `scan_alignments` subprogram shares the majority of its arguments with `alignment_plot`, which both implement the grouping algorithm. New arguments include `--window_size` and `--window_step`. The software runs a sliding window across each reference sequence in the alignment map (i.e., a *SAM*/*BAM* file), and applies the grouping algorithm at each window. The size of the window is determined by `--window_size` (defaults to 50 Kb) and the sliding distance is set by `--window_step` (default = 25 Kb). Reference sequences that are shorter than `--window_size` are ignored. 
@@ -204,35 +219,35 @@
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue
 ```
 
 The resulting file is written by default in pdf format, but can be changed using the `--format` option, which accepts either *pdf*, *png* or *svg* as a value. The ouput file will have the same name as the file passed to `--klumps_tsv`. For example, the output for *input_klumps.tsv* would be *input_klumps.pdf*. Below is an example of 6 sequences
 
 <p align="center">
-<img src="Images/klump_plot_example1.png" alt="drawing" style="width:800px;height:200px"/>
+<img src="./Images/klump_plot_example1.png" alt="drawing" style="width:600px;height:300px"/>
 </p>
 
 Sequences are sorted by sequence length, with the shortest sequence at the top, and the longest sequence at the bottom. Furthermore, since the number of sequences to plot is unknown, the height of the pdf is extended so that each sequence is equally spaced apart. The klump labels begin with the number of k-mers in the klump, separated by a **-** from the name of the query source.
 
 If using the `--fix_width` flag is implemented, there will be no relative scaling done on the sequences.
 
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue --fix_width
 ```
 <p align="center">
-<img src="Images/klump_plot_example2.png" alt="drawing" style="width:800px;height:200px"/>
+<img src="./Images/klump_plot_example2.png" alt="drawing" style="width:600px;height:300px"/>
 </p>
 
 In the case in which you are interested in a particular locus in a specific sequence, the `--seq_name` flags can be used.
 
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue --seq_name Seq4
 ```
 <p align="center">
-<img src="Images/klump_plot_example3.png" alt="drawing" style="width:800px;height:100px"/>
+<img src="./Images/klump_plot_example3.png" alt="drawing" style="width:600px;height:100px"/>
 </p>
 
 If the sequences contain gaps, the output of `find_gaps` can be used to annotate the figure with the sequence gaps (see `./TestCases/TestCases.md` for an example where we viewed gaps across several *Bombus* reference genomes)
 
 ### Advanced options
 
 The `--klump_colors` and `--color_by_gene` parameters accept a *.tsv* file and uses that to map a color to a specific query source. If the color is unavailable, the program will report back to the user the error and exit. Not every query source needs to be present in the *.tsv* file, as those unlisted sources will be defaulted to a blue color. An example of an acceptable tab-delimited file is shown below
@@ -246,42 +261,42 @@
 Query6  cyan
 ```
 Assuming the file is named *klump_colors.tsv*, the following command illustrates its use
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --fix_width --klump_colors klump_colors.tsv
 ```
 <p align="center">
-<img src="Images/klump_plot_example_colors.png" alt="drawing" style="width:800px;height:200px"/>
+<img src="./Images/klump_plot_example_colors.png" alt="drawing" style="width:600px;height:300px"/>
 </p>
 
 The file supplied to `--color_by_gene` is treated differently, as this argument was designed to work with the results of the `get_exons` subprogram. Sequences obtained with `get_exons` will have the extension *_EN* in the sequence header, where *E* is short for Exon and *N* is for the *N*<sup>th</sup> exon. So if using the above example, all klumps with *query1_E[N]* will be colored blue (*N* being any number).
 
 To view a specific region in a specific sequence in the klumps *.tsv* file, the `--leftbound` and `--rightbound` parameters can be used.
 
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue --seq_name Seq4 --leftbound 5e3 --rightbound 7e3
 ```
 <p align="center">
-<img src="Images/klump_plot_example4.png" alt="drawing" style="width:800px;height:100px"/>
+<img src="./Images/klump_plot_example4.png" alt="drawing" style="width:600px;height:100px"/>
 </p>
 
 Further customization can be performed with the `--tick_count` and `--tick_span` parameters, both of which are only implemented when viewing a single sequence. `--tick_count` specifies the number of tick markers in the drawing, while `--tick_span` will set the length (in base pairs) between tick markers.
 
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue --seq_name Seq4 --tick_count 20
 ```
 <p align="center">
-<img src="Images/klump_plot_example5.png" alt="drawing" style="width:800px;height:100px"/>
+<img src="./Images/klump_plot_example5.png" alt="drawing" style="width:600px;height:100px"/>
 </p>
 
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue --seq_name Seq4 --tick_span 2e3
 ```
 <p align="center">
-<img src="Images/klump_plot_example6.png" alt="drawing" style="width:800px;height:100px"/>
+<img src="./Images/klump_plot_example6.png" alt="drawing" style="width:600px;height:100px"/>
 </p>
 
 # kmerize
 The `kmerize` subprogram performs the `--query` search in the `--subject` sequences implemented by `find_klumps`. A *query_map.gz* file will be generated, but no klump construction will be performed. All parameters available to `kmerize` are those which are also available to `find_klumps` (see `find_klumps` section for details ).
 
 ```
     --subject:                  Subject sequences in FAST[A|Q] format [Required]    
@@ -450,21 +465,21 @@
                       --leftbound 4.47e6 \    # could use 4470000
                       --rightbound 4.55e6 \   # could use 4550000
                       --min_len 1e4 \         # can use 10000
                       --min_percent 50        # could use 0.50
 ```
 The output will resemble something along the lines of what is shown below
 <p align="center">
-<img src="Images/align_plot1.png" width="50%" height="75%">
+<img src="./Images/align_plot1.png" width="50%" height="75%">
 </p>
 
 
 The leftmost postitioned sequence is placed at the top, with the rightmost sequence positioned at the bottom (excluding the reference sequence). The alignments either are a light grey, indicating a forward alignment (in respect to the reference genome), or a shade of yellow, which represent alignments on the reverse strand of the reference genome. Several other features are shown here, notably deletions and clips.
 <p align="center">
-<img src="Images/align_plot1_zoom.png" width="50%" height="100%">
+<img src="./Images/align_plot1_zoom.png" width="50%" height="100%">
 </p>
 
 Zooming in, there are horizontal black lines that separate the blocks of the aligned portions of the sequence. These black lines represent deletions. Data such as Pac-Bio are known to have many small indels. As these may be due to sequencing errors as opposed to real biological indels, viewing these small indels may not benefit the user. By default, the `--deletion_len` argument is set to 100 (*Note* that this is an advanced parameter that). In other words, `klumpy` will draw deletions that are at least 100 bp in length. As insertions do not consume the reference sequence, they are ignored. The light green extensions from the alignment represent soft clips in the alignment, while red lines extending from the alignment would indicate hard clips (not shown in example).
 
 Additional annotation files that can be provided include `--gap_file` (file generated from `find_gaps`) and `--annotation`, which takes a *.gtf* or *.gff* file (can be compresssed) as input. Both these two files will annotate the reference sequence with any features located within region. For further annotation, `--vertical_line_gaps`, `--vertical_line_klumps`, and `--vertical_line_exons` will draw a dashed line above the desired feature in the reference sequence.
 
 Example with `--annotation`.
@@ -476,20 +491,20 @@
                       --min_len 1e4 \         # could use 10000
                       --min_percent 50 \      # could use 0.50
                       --annotation cgun.gtf.gz
 ```
 
 The output will resememble something along the lines of what is shown below
 <p align="center">
-<img src="Images/align_plot2.png" width="50%" height="100%">
+<img src="./Images/align_plot2.png" width="50%" height="100%">
 </p>
 
 Here, each gene is differentiated by its color. For example, gene *g_9529* is red while gene *g_16157* is a lighter blue. Each separate annotation represents an exon, with the first exon in the image for each gene being tagged with the name of the gene. Gene labels alternate in position, where one gene's label is drawn on top of the reference sequence, and the following gene's label will be drawn below the reference sequence. If a third gene is drawn, its label will then be drawn above the reference sequence and the pattern continues.
 <p align="center">
-<img src="Images/align_plot2_zoom.png" width="50%" height="100%">
+<img src="./Images/align_plot2_zoom.png" width="50%" height="100%">
 </p>
 
 Plotting a region where a gap is located, we can see the following
 ```
 klumpy alignment_plot --alignment_map cgun_raw_reads.bam \
                       --reference 24 \
                       --leftbound 13.07e6 \    # could use 13070000
@@ -497,15 +512,15 @@
                       --min_len 1e4 \         # could use 10000
                       --min_percent 50 \      # could use 0.50
                       --annotation cgun.gtf.gz \
                       --gap_file cgun_gaps.tsv \
                       --vertical_line_gaps    # no input needed
 ```
 <p align="center">
-<img src="Images/align_plot3.png", width="50%" height="100%">
+<img src="./Images/align_plot3.png", width="50%" height="100%">
 </p>
 
 Here, it is clear that the gap connecting two contigs is directly below a deletion in several alignments. 
 
 To present an example with klumps, we will annotate one of the *afgp* regions in our assembly & alignments.
 ```
 klumpy alignment_plot --alignment_map cgun_raw_reads.bam \
@@ -518,15 +533,15 @@
                       --gap_file cgun_gaps.tsv \
                       --vertical_line_gaps \# no input needed
                       --klumps_tsv afgp_klumps.tsv
 ```
 
 Here, it is clear that there is a gapless region containing relatively few AFGP loci in the Mackerel Icefish
 <p align="center">
-<img src="Images/klumps_align_example.png" width="50%" height="100%">
+<img src="./Images/klumps_align_example.png" width="50%" height="100%">
 </p>
 
 The `--group_seqs` argument does not accept any input (i.e., just include the parameter in your command) and groups the sequences using `klumpy`'s grouping algorithm (see *Advanced options* for detials)
 
 ## Advanced options
 
 By default, only primary alignments are visualized, with the available options `--secondary` and `--supplementary` that can relax this constraint. To exclude primary alignments, simply use the flag `--no_primary`.
@@ -570,15 +585,15 @@
                       --annotation cgun.gtf.gz \
                       --number \              # no input needed
                       --write_table           # no input needed
 ```
 
 Zoomed in for clarity
 <p align="center">
-<img src="Images/num_zoom.png" width="50%" height="100%">
+<img src="./Images/num_zoom.png" width="50%" height="100%">
 </p>
 
 
 To plot paired-end data, you **must** use the `--paired` flag. The plotting scheme is different for paired-end data, where the pair of sequences are plotted on the same line, and `R1` sequences are plotted in green, and `R2` are colored as blue. 
 
 Illustrating an example with some Restriction-site Associated Sequencing (RAD-Seq) data.
 ```
@@ -588,15 +603,15 @@
                       --rightbound 1.71e5 \   # could use 171000
                       --min_len 100 \         # min length should be set for short reads
                       --min_percent 50 \      # could use 0.50
                       --annotation cgun.gtf.gz \
                       --paired                # no input needed
 ```
 <p align="center">
-<img src="Images/paired_align.png" width="50%" height="100%">
+<img src="./Images/paired_align.png" width="50%" height="100%">
 </p>
 
 Here, the reads are aligned right at an exon of `cdk15`, which is a *cyclin-dependent kinase*.
 
 `--group_seqs` is used to signal to `klumpy` to attempt to group the alignments based on their alignment patterns. Before describing some of the parameters, it must be noted that the grouping algorithm is **only** applied on *primary* alignments and *non-paired-end* data.
 
 The grouping algorithm first starts by trying to group "good" alignments (i.e., alignments without large deletions or clipping). This is based on the assumption that alignments in missassembled regions tend to have features such as clipping and deletions. Most of the grouping-specific featuers are designed to work with these features.
@@ -604,31 +619,31 @@
 First, the `--assume_sep_del` flag is used to *turn off* the assumption that alignments with deletions *should* be grouped together if there is their deletions span the same region in the reference. The `--per_overlap` takes a percentage (e.g., 50 or 0.50), which sets the minimum percentage that alignments need to overlap one another (i.e., both alignments need to overlap each other by `--per_overlap`) to be *considered* a good match (i.e., this alone does not result in the two alignments being grouped together).
 
 The `--t_len` and `--t_per` arguments work similarly to `--min_len` and `--min_percent`. The `--t_len` argument is used to set the "trust" length, which any *sequence* below this length will be ignored when grouping as it is assumed to be untrustworthy. Likewise, any *sequence* with an aligned percentage lower than `--t_per` is also ignored when grouping. The rationale for these parameters is to avoid trying to bin short and poorly aligned sequences that cannot be reliably placed into a single group.
 
 The `--clip_tolerance` argument is used to set the number of clipped base pairs that can be tolerated between two alignments. Below is a simple case.
 
 <p align="center">
-<img src="Images/clip_tolerance.png" width="50%" height="100%">
+<img src="./Images/clip_tolerance.png" width="50%" height="75%">
 </p>
 
 Here, a clip from alignment B is overlapping an aligned portion of alignment A. If `--clip_tolerance` is shorter than the *clip overlap*, the two alignments are considered incompatible. Otherwise, they can still be compatible. 
 
 The `--del_tolerance` is similar to `--clip_tolerance`, except that it evaluates the deletion overlaps.
 
 <p align="center">
-<img src="Images/del_tolerance.png" width="50%" height="100%">
+<img src="./Images/del_tolerance.png" width="50%" height="75%">
 </p>
 
 If the value provided to `--del_tolerance` is shorter than the *deletion overlap*, then the two sequences are considered incompatible.
 
 In `--group_seqs`, alignments that begin at the same position are assumed to represent the same locus, as it is reasonable to assume the two sequences are of the same origin if starting at the same site. Since two alignments may not *exactly* align at the same position, but can be loosely interpretted as aligning to the same position, the `--align_offset` provides some wiggle room.
 
 <p align="center">
-<img src="Images/align_offset.png" width="50%" height="100%">
+<img src="./Images/align_offset.png" width="50%" height="75%">
 </p>
 
 The offset applies both to the left and right side of the aligned portions of an alignment (here, alignment A). For visual purposes, only alignment A is being checked in the illustration, but this evaluation is also applied from the perspective of alignment B.
 
 
 To illustrate a simple case, we will apply the grouping algorithm to a 50 Kb region on chromosome 3 using default parameters
 
@@ -639,15 +654,15 @@
                       --rightbound 10.25e6 \    # could use 4550000
                       --min_len 2.5e4 \         # 25 Kb
                       --min_percent 75 \        # same as 0.75
                       --annotation cgun.gtf.gz \
                       --group_seqs              # no input needed
 ```
 <p align="center">
-<img src="Images/group_align_example1.png" width="50%" height="100%">
+<img src="./Images/group_align_example1.png" width="50%" height="100%">
 </p>
 
 Here, the sequence alignments are colored based on the group they were assigned to. Alignments that are ungrouped are left white. Here, there are two groups. 
 
 To illustrate an unresolved region, we will focus on a region where the algorithm struggles to find 2 or less groups while keeping the parameters the same. Additionally, we will annotate the image with the gaps in the region.
 
 ```
@@ -659,23 +674,23 @@
                       --min_percent 85 \            # same as 0.85
                       --annotation cgun.gtf.gz \
                       --group_seqs \                # no input needed
                       --gap_file cgun_gaps.tsv \
                       --vertical_line_gaps          # no input needed
 ```
 <p align="center">
-<img src="Images/misassemble_example.png" width="50%" height="100%">
+<img src="./Images/misassemble_example.png" width="50%" height="100%">
 </p>
 
 Within this 180 Kb region, 4 contigs are stitched together as indicated by the 3 gaps (stretches of *N*'s). Interestingly, the third contig (~6.99 Mb - 7.65 Mb) was predicted to be composed of three groups, with two of the groups having some overlap with each other. In this example, `klumpy` predicts 12 groups within this region. Although this is likely to not be the true number of groups, the binning of sequences into their respective groups can aid in the reconstruction of problematic loci.
 
 The remaining grouping-based arguments are `--min_grp`, `--write_groups` and `--write_edge_seqs`. The `--min_grp` flag accepts an integer to set as the minimum number of sequences required to form a group. The `--write_groups` flag is set to tell the program to write the groups to group-specific fasta files, which can be used for tasks such as local reassemblies or annotations. If your interests are more on clipped sequences at the ends/edges of the groups, implementing the `--write_edge_seqs` will write out the names of the clipped sequences at the ends/edges of the groups into group-specific *.txt* files. The following image highlights some of the edge sequences from above.
 
 <p align="center">
-<img src="Images/edge_seqs_example.png" width="50%" height="100%">
+<img src="./Images/edge_seqs_example.png" width="50%" height="100%">
 </p>
 
 # get_exons
 
 The purpose of this subprogram is to take a list of genes, and extract out their exonic sequences from a reference assembly. All arguments are required for this program.
 ```
     --fasta:                    Reference genome in fasta format [Required]
```

### Comparing `klumpy-1.0.5/README.md` & `klumpy-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 Initially developed to verify the Antifreeze glycoproteins in the genomes of two icefishes (see [Rivera-Colón, 2023](https://academic.oup.com/mbe/article/40/3/msad029/7035026)), `klumpy` now has expanded to include a suite of tools for assessing whether a particular region in a genome assembly is missassembled by leveraging the original data (i.e., raw reads) used in the assembly process, or it can instead be used to search for a gene of interest in a set of sequences. Complete overview of the software and the methods used in the paper can be viewed at [here](https://bitbucket.org/Gio12/klumpy/src/master/).
 
 # Installation
 ```
 python3 -m pip install klumpy
 ```
 
+**NOTE**: `klumpy` uses `samtools` to parse *.bam* / *.sam* files, so `samtools` should be installed and available in the current path when providing `klumpy` an alignment file. 
+
 # Components
 
 `klumpy` currently is composed of 9 different subprograms, two are which are the primary subprograms, two which can illustrate the results, with the remaining 5 designed to supplement the four other subprograms. Depending on whether you have a gene of interest, as in the case with the Icefishes and AFGPs, you can start the analysis with `find_klumps`. If the aim is to assess the quality of your reference genome, the `scan_alignment` analysis would flag regions that were possibly missassembled.
 
 ```
 # primary subprograms
     find_klumps:                Find query klumps in a set of subject sequences
@@ -107,56 +109,69 @@
         --t_len:                    Minimum length a sequence must be in order to trust its assignment when grouping (default = 2000)
         --t_per:                    Minimum percentage a sequence must be aligned in order to trust its assignment when grouping (default = 30)
         --align_offset:             Maximum number of base pairs apart for two sequences to be considered aligned at the same position (default = 100)
         --min_grp:                  Minimum number of sequences in a group in order to retain the group (default = 2)
         --window_size:              Length (in bp) for the sliding window to be (default = 50000)
         --window_step:              Length (in bp) for the sliding window to slide down to establish the next window (default = 25000) 
         --limit:                    Maximum number of alignments to process in a window (default 10000)
+        --flag_excess_groups:       If set, will report regions with greater than or equal to --num_of_groups parameter regardless if the region was tiled or not
 ```
 With the exception of `--threads`, the main parameters are shared with `alignment_plot`. Here, a sliding window approach is implemented, and at each window, `klumpy`'s grouping algorithm is performed (see *Advanced options* under the `alignment_plot` section). The use of multiple threads (i.e., the `--threads` argument) is only useful if the alignment map contains more than 1 *reference* sequence (parallelization is implemented across reference sequences, not alignment records).
 
 To perform a scan, one can run a command similar to this
 ```
 klumpy scan_alignments --alignment_map input.bam --threads 16
 ```
 Here, we used the default parameters of using sequences with a length of at least 2 Kbp (set by `--min_len`), with the default `--min_percent` value of 50, meaning that sequences where more than a quarter of the sequence are unmapped, are not retained in the scanning process.
 
-The `--num_of_groups` argument sets the minimum number of groups a region must have in order for the region to be flagged as a possible missassembly. If a *.gtf* or *.gff* file is provided to `--annotation`, only regions containing a gene will be processed (useful if you are only interested in annotated regions).
+The `--num_of_groups` argument sets the minimum number of groups a region must have in order to flag a region to be flagged as a possible missassembly if the `--flag_excess_groups` is set. If a *.gtf* or *.gff* file is provided to `--annotation`, only regions containing a gene will be processed (useful if you are only interested in annotated regions).
 
 When running this software, temporary files will be written to disk using the naming scheme *Temp_seq_name.txt*, where the *seq_name* is the name of the reference sequence being scanned. **DO NOT DISGARD THESE FILES**, they will be removed after the data is merged. 
 
 The temporary files contain flagged *windows* that look something like this
 ```
-seq 400000  425000
-seq 750000  775000
-seq 775000  800000
+seq 400000  425000  1
+seq 750000  775000  1
+seq 775000  800000  2
 ```
 
-Where the first column contains the sequence name, the second column the start position of the window, and the third column contains the end position of the window. If an annotation file is provided, the temporary file would contain an additional column
+Where the first column contains the sequence name, the second column the start position of the window, the third column contains the end position of the window, and the fourth columm contains the number of groups found. If an annotation file is provided, the temporary file would contain an additional column
 ```
-seq 400000  425000  geneA,geneB,geneC
-seq 750000  775000  geneX,geneY
-seq 775000  800000  geneY,geneZ
+seq 400000  425000  1   geneA,geneB,geneC
+seq 750000  775000  1   geneX,geneY
+seq 775000  800000  2   geneY,geneZ
 ```
 
-Where the fourth column is added with a comma separated list containing the genes found in the window. 
+Where the fifth column is added with a comma separated list containing the genes found in the window. Lastly, if using the `--flag_excess_groups` option, an additional column containing either a *T* or a *F* will be added between the third and fourth column to indicate whether the region was tiled (*T* or True) or not (*F* or False).
+
+```
+seq 400000  425000  F   1   geneA,geneB,geneC
+seq 750000  775000  F   1   geneX,geneY
+seq 775000  800000  T   2   geneY,geneZ
+```
 
 Once all the reference sequences have been scanned, they are merged into a single file. The output file will contain the same name as in the alignment map, with the added extension of *_Candidate_Regions.tsv*. For example, if the input was called *input.bam*, the output would be *input_Candidate_Regions.tsv*. Using the examples above, the resulting output would like this
 
 ```
 # klumpy scan_alignments --alignment_map input.bam --threads 16
-Region_Num  Reference_Seq   Start   End
-1   seq 400000  425000
-2   seq 750000  800000
+Region_Num  Reference_Seq   Start   End Number_of_Groups
+1   seq 400000  425000  1
+2   seq 750000  800000  1,2
 
 # with annotation file provided
 # klumpy scan_alignments --alignment_map input.bam --threads 16 --annotation input.gtf.gz
-Region_Num  Reference_Seq   Start   End Genes
-1   seq 400000  425000  geneA,geneB,geneC
-2   seq 750000  800000  geneX,geneY,geneZ
+Region_Num  Reference_Seq   Start   End Number_of_Groups    Genes
+1   seq 400000  425000  1 geneA,geneB,geneC
+2   seq 750000  800000  1,2 geneX,geneY,geneZ
+
+# with annotation file provided & flagging regions based on group number
+# klumpy scan_alignments --alignment_map input.bam --threads 16 --annotation input.gtf.gz --flag_excess_groups
+Region_Num  Reference_Seq   Start   End Tiled Number_of_Groups Genes
+1   seq 400000  425000  F, 1 geneA,geneB,geneC
+2   seq 750000  800000  F,T 1,2 geneX,geneY,geneZ
 ```
 
 The first line of the output will contain the line of code provided used to start the analysis, while the second line contains the column headers. Here, *regions* are reported instead of windows since `klumpy` will collapse overlapping windows since they represent the same locus. Th *Reference_Seq* column contains the name of the reference sequence, and the *Start* and *End* columns contain positions of the region (**NOTE** these are 0-based positions). The *Genes* column is optionally added if an annotation file was used in the analysis. If a desired window is of interest, the *_Candidate_Regions.tsv* output can be supplied to `alignment_plot` using the `--candidates` option in combination with the `--region_num` argument to specify which region `klumpy` should plot instead of explicitly using `--reference`, `--leftbound`, and `--rightbound`.
 
 #### Advanced options
 
 The `scan_alignments` subprogram shares the majority of its arguments with `alignment_plot`, which both implement the grouping algorithm. New arguments include `--window_size` and `--window_step`. The software runs a sliding window across each reference sequence in the alignment map (i.e., a *SAM*/*BAM* file), and applies the grouping algorithm at each window. The size of the window is determined by `--window_size` (defaults to 50 Kb) and the sliding distance is set by `--window_step` (default = 25 Kb). Reference sequences that are shorter than `--window_size` are ignored. 
@@ -191,35 +206,35 @@
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue
 ```
 
 The resulting file is written by default in pdf format, but can be changed using the `--format` option, which accepts either *pdf*, *png* or *svg* as a value. The ouput file will have the same name as the file passed to `--klumps_tsv`. For example, the output for *input_klumps.tsv* would be *input_klumps.pdf*. Below is an example of 6 sequences
 
 <p align="center">
-<img src="Images/klump_plot_example1.png" alt="drawing" style="width:800px;height:200px"/>
+<img src="./Images/klump_plot_example1.png" alt="drawing" style="width:600px;height:300px"/>
 </p>
 
 Sequences are sorted by sequence length, with the shortest sequence at the top, and the longest sequence at the bottom. Furthermore, since the number of sequences to plot is unknown, the height of the pdf is extended so that each sequence is equally spaced apart. The klump labels begin with the number of k-mers in the klump, separated by a **-** from the name of the query source.
 
 If using the `--fix_width` flag is implemented, there will be no relative scaling done on the sequences.
 
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue --fix_width
 ```
 <p align="center">
-<img src="Images/klump_plot_example2.png" alt="drawing" style="width:800px;height:200px"/>
+<img src="./Images/klump_plot_example2.png" alt="drawing" style="width:600px;height:300px"/>
 </p>
 
 In the case in which you are interested in a particular locus in a specific sequence, the `--seq_name` flags can be used.
 
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue --seq_name Seq4
 ```
 <p align="center">
-<img src="Images/klump_plot_example3.png" alt="drawing" style="width:800px;height:100px"/>
+<img src="./Images/klump_plot_example3.png" alt="drawing" style="width:600px;height:100px"/>
 </p>
 
 If the sequences contain gaps, the output of `find_gaps` can be used to annotate the figure with the sequence gaps (see `./TestCases/TestCases.md` for an example where we viewed gaps across several *Bombus* reference genomes)
 
 ### Advanced options
 
 The `--klump_colors` and `--color_by_gene` parameters accept a *.tsv* file and uses that to map a color to a specific query source. If the color is unavailable, the program will report back to the user the error and exit. Not every query source needs to be present in the *.tsv* file, as those unlisted sources will be defaulted to a blue color. An example of an acceptable tab-delimited file is shown below
@@ -233,42 +248,42 @@
 Query6  cyan
 ```
 Assuming the file is named *klump_colors.tsv*, the following command illustrates its use
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --fix_width --klump_colors klump_colors.tsv
 ```
 <p align="center">
-<img src="Images/klump_plot_example_colors.png" alt="drawing" style="width:800px;height:200px"/>
+<img src="./Images/klump_plot_example_colors.png" alt="drawing" style="width:600px;height:300px"/>
 </p>
 
 The file supplied to `--color_by_gene` is treated differently, as this argument was designed to work with the results of the `get_exons` subprogram. Sequences obtained with `get_exons` will have the extension *_EN* in the sequence header, where *E* is short for Exon and *N* is for the *N*<sup>th</sup> exon. So if using the above example, all klumps with *query1_E[N]* will be colored blue (*N* being any number).
 
 To view a specific region in a specific sequence in the klumps *.tsv* file, the `--leftbound` and `--rightbound` parameters can be used.
 
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue --seq_name Seq4 --leftbound 5e3 --rightbound 7e3
 ```
 <p align="center">
-<img src="Images/klump_plot_example4.png" alt="drawing" style="width:800px;height:100px"/>
+<img src="./Images/klump_plot_example4.png" alt="drawing" style="width:600px;height:100px"/>
 </p>
 
 Further customization can be performed with the `--tick_count` and `--tick_span` parameters, both of which are only implemented when viewing a single sequence. `--tick_count` specifies the number of tick markers in the drawing, while `--tick_span` will set the length (in base pairs) between tick markers.
 
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue --seq_name Seq4 --tick_count 20
 ```
 <p align="center">
-<img src="Images/klump_plot_example5.png" alt="drawing" style="width:800px;height:100px"/>
+<img src="./Images/klump_plot_example5.png" alt="drawing" style="width:600px;height:100px"/>
 </p>
 
 ```
 klumpy klump_plot --klumps_tsv input_klumps.tsv --color blue --seq_name Seq4 --tick_span 2e3
 ```
 <p align="center">
-<img src="Images/klump_plot_example6.png" alt="drawing" style="width:800px;height:100px"/>
+<img src="./Images/klump_plot_example6.png" alt="drawing" style="width:600px;height:100px"/>
 </p>
 
 # kmerize
 The `kmerize` subprogram performs the `--query` search in the `--subject` sequences implemented by `find_klumps`. A *query_map.gz* file will be generated, but no klump construction will be performed. All parameters available to `kmerize` are those which are also available to `find_klumps` (see `find_klumps` section for details ).
 
 ```
     --subject:                  Subject sequences in FAST[A|Q] format [Required]    
@@ -437,21 +452,21 @@
                       --leftbound 4.47e6 \    # could use 4470000
                       --rightbound 4.55e6 \   # could use 4550000
                       --min_len 1e4 \         # can use 10000
                       --min_percent 50        # could use 0.50
 ```
 The output will resemble something along the lines of what is shown below
 <p align="center">
-<img src="Images/align_plot1.png" width="50%" height="75%">
+<img src="./Images/align_plot1.png" width="50%" height="75%">
 </p>
 
 
 The leftmost postitioned sequence is placed at the top, with the rightmost sequence positioned at the bottom (excluding the reference sequence). The alignments either are a light grey, indicating a forward alignment (in respect to the reference genome), or a shade of yellow, which represent alignments on the reverse strand of the reference genome. Several other features are shown here, notably deletions and clips.
 <p align="center">
-<img src="Images/align_plot1_zoom.png" width="50%" height="100%">
+<img src="./Images/align_plot1_zoom.png" width="50%" height="100%">
 </p>
 
 Zooming in, there are horizontal black lines that separate the blocks of the aligned portions of the sequence. These black lines represent deletions. Data such as Pac-Bio are known to have many small indels. As these may be due to sequencing errors as opposed to real biological indels, viewing these small indels may not benefit the user. By default, the `--deletion_len` argument is set to 100 (*Note* that this is an advanced parameter that). In other words, `klumpy` will draw deletions that are at least 100 bp in length. As insertions do not consume the reference sequence, they are ignored. The light green extensions from the alignment represent soft clips in the alignment, while red lines extending from the alignment would indicate hard clips (not shown in example).
 
 Additional annotation files that can be provided include `--gap_file` (file generated from `find_gaps`) and `--annotation`, which takes a *.gtf* or *.gff* file (can be compresssed) as input. Both these two files will annotate the reference sequence with any features located within region. For further annotation, `--vertical_line_gaps`, `--vertical_line_klumps`, and `--vertical_line_exons` will draw a dashed line above the desired feature in the reference sequence.
 
 Example with `--annotation`.
@@ -463,20 +478,20 @@
                       --min_len 1e4 \         # could use 10000
                       --min_percent 50 \      # could use 0.50
                       --annotation cgun.gtf.gz
 ```
 
 The output will resememble something along the lines of what is shown below
 <p align="center">
-<img src="Images/align_plot2.png" width="50%" height="100%">
+<img src="./Images/align_plot2.png" width="50%" height="100%">
 </p>
 
 Here, each gene is differentiated by its color. For example, gene *g_9529* is red while gene *g_16157* is a lighter blue. Each separate annotation represents an exon, with the first exon in the image for each gene being tagged with the name of the gene. Gene labels alternate in position, where one gene's label is drawn on top of the reference sequence, and the following gene's label will be drawn below the reference sequence. If a third gene is drawn, its label will then be drawn above the reference sequence and the pattern continues.
 <p align="center">
-<img src="Images/align_plot2_zoom.png" width="50%" height="100%">
+<img src="./Images/align_plot2_zoom.png" width="50%" height="100%">
 </p>
 
 Plotting a region where a gap is located, we can see the following
 ```
 klumpy alignment_plot --alignment_map cgun_raw_reads.bam \
                       --reference 24 \
                       --leftbound 13.07e6 \    # could use 13070000
@@ -484,15 +499,15 @@
                       --min_len 1e4 \         # could use 10000
                       --min_percent 50 \      # could use 0.50
                       --annotation cgun.gtf.gz \
                       --gap_file cgun_gaps.tsv \
                       --vertical_line_gaps    # no input needed
 ```
 <p align="center">
-<img src="Images/align_plot3.png", width="50%" height="100%">
+<img src="./Images/align_plot3.png", width="50%" height="100%">
 </p>
 
 Here, it is clear that the gap connecting two contigs is directly below a deletion in several alignments. 
 
 To present an example with klumps, we will annotate one of the *afgp* regions in our assembly & alignments.
 ```
 klumpy alignment_plot --alignment_map cgun_raw_reads.bam \
@@ -505,15 +520,15 @@
                       --gap_file cgun_gaps.tsv \
                       --vertical_line_gaps \# no input needed
                       --klumps_tsv afgp_klumps.tsv
 ```
 
 Here, it is clear that there is a gapless region containing relatively few AFGP loci in the Mackerel Icefish
 <p align="center">
-<img src="Images/klumps_align_example.png" width="50%" height="100%">
+<img src="./Images/klumps_align_example.png" width="50%" height="100%">
 </p>
 
 The `--group_seqs` argument does not accept any input (i.e., just include the parameter in your command) and groups the sequences using `klumpy`'s grouping algorithm (see *Advanced options* for detials)
 
 ## Advanced options
 
 By default, only primary alignments are visualized, with the available options `--secondary` and `--supplementary` that can relax this constraint. To exclude primary alignments, simply use the flag `--no_primary`.
@@ -557,15 +572,15 @@
                       --annotation cgun.gtf.gz \
                       --number \              # no input needed
                       --write_table           # no input needed
 ```
 
 Zoomed in for clarity
 <p align="center">
-<img src="Images/num_zoom.png" width="50%" height="100%">
+<img src="./Images/num_zoom.png" width="50%" height="100%">
 </p>
 
 
 To plot paired-end data, you **must** use the `--paired` flag. The plotting scheme is different for paired-end data, where the pair of sequences are plotted on the same line, and `R1` sequences are plotted in green, and `R2` are colored as blue. 
 
 Illustrating an example with some Restriction-site Associated Sequencing (RAD-Seq) data.
 ```
@@ -575,15 +590,15 @@
                       --rightbound 1.71e5 \   # could use 171000
                       --min_len 100 \         # min length should be set for short reads
                       --min_percent 50 \      # could use 0.50
                       --annotation cgun.gtf.gz \
                       --paired                # no input needed
 ```
 <p align="center">
-<img src="Images/paired_align.png" width="50%" height="100%">
+<img src="./Images/paired_align.png" width="50%" height="100%">
 </p>
 
 Here, the reads are aligned right at an exon of `cdk15`, which is a *cyclin-dependent kinase*.
 
 `--group_seqs` is used to signal to `klumpy` to attempt to group the alignments based on their alignment patterns. Before describing some of the parameters, it must be noted that the grouping algorithm is **only** applied on *primary* alignments and *non-paired-end* data.
 
 The grouping algorithm first starts by trying to group "good" alignments (i.e., alignments without large deletions or clipping). This is based on the assumption that alignments in missassembled regions tend to have features such as clipping and deletions. Most of the grouping-specific featuers are designed to work with these features.
@@ -591,31 +606,31 @@
 First, the `--assume_sep_del` flag is used to *turn off* the assumption that alignments with deletions *should* be grouped together if there is their deletions span the same region in the reference. The `--per_overlap` takes a percentage (e.g., 50 or 0.50), which sets the minimum percentage that alignments need to overlap one another (i.e., both alignments need to overlap each other by `--per_overlap`) to be *considered* a good match (i.e., this alone does not result in the two alignments being grouped together).
 
 The `--t_len` and `--t_per` arguments work similarly to `--min_len` and `--min_percent`. The `--t_len` argument is used to set the "trust" length, which any *sequence* below this length will be ignored when grouping as it is assumed to be untrustworthy. Likewise, any *sequence* with an aligned percentage lower than `--t_per` is also ignored when grouping. The rationale for these parameters is to avoid trying to bin short and poorly aligned sequences that cannot be reliably placed into a single group.
 
 The `--clip_tolerance` argument is used to set the number of clipped base pairs that can be tolerated between two alignments. Below is a simple case.
 
 <p align="center">
-<img src="Images/clip_tolerance.png" width="50%" height="100%">
+<img src="./Images/clip_tolerance.png" width="50%" height="75%">
 </p>
 
 Here, a clip from alignment B is overlapping an aligned portion of alignment A. If `--clip_tolerance` is shorter than the *clip overlap*, the two alignments are considered incompatible. Otherwise, they can still be compatible. 
 
 The `--del_tolerance` is similar to `--clip_tolerance`, except that it evaluates the deletion overlaps.
 
 <p align="center">
-<img src="Images/del_tolerance.png" width="50%" height="100%">
+<img src="./Images/del_tolerance.png" width="50%" height="75%">
 </p>
 
 If the value provided to `--del_tolerance` is shorter than the *deletion overlap*, then the two sequences are considered incompatible.
 
 In `--group_seqs`, alignments that begin at the same position are assumed to represent the same locus, as it is reasonable to assume the two sequences are of the same origin if starting at the same site. Since two alignments may not *exactly* align at the same position, but can be loosely interpretted as aligning to the same position, the `--align_offset` provides some wiggle room.
 
 <p align="center">
-<img src="Images/align_offset.png" width="50%" height="100%">
+<img src="./Images/align_offset.png" width="50%" height="75%">
 </p>
 
 The offset applies both to the left and right side of the aligned portions of an alignment (here, alignment A). For visual purposes, only alignment A is being checked in the illustration, but this evaluation is also applied from the perspective of alignment B.
 
 
 To illustrate a simple case, we will apply the grouping algorithm to a 50 Kb region on chromosome 3 using default parameters
 
@@ -626,15 +641,15 @@
                       --rightbound 10.25e6 \    # could use 4550000
                       --min_len 2.5e4 \         # 25 Kb
                       --min_percent 75 \        # same as 0.75
                       --annotation cgun.gtf.gz \
                       --group_seqs              # no input needed
 ```
 <p align="center">
-<img src="Images/group_align_example1.png" width="50%" height="100%">
+<img src="./Images/group_align_example1.png" width="50%" height="100%">
 </p>
 
 Here, the sequence alignments are colored based on the group they were assigned to. Alignments that are ungrouped are left white. Here, there are two groups. 
 
 To illustrate an unresolved region, we will focus on a region where the algorithm struggles to find 2 or less groups while keeping the parameters the same. Additionally, we will annotate the image with the gaps in the region.
 
 ```
@@ -646,23 +661,23 @@
                       --min_percent 85 \            # same as 0.85
                       --annotation cgun.gtf.gz \
                       --group_seqs \                # no input needed
                       --gap_file cgun_gaps.tsv \
                       --vertical_line_gaps          # no input needed
 ```
 <p align="center">
-<img src="Images/misassemble_example.png" width="50%" height="100%">
+<img src="./Images/misassemble_example.png" width="50%" height="100%">
 </p>
 
 Within this 180 Kb region, 4 contigs are stitched together as indicated by the 3 gaps (stretches of *N*'s). Interestingly, the third contig (~6.99 Mb - 7.65 Mb) was predicted to be composed of three groups, with two of the groups having some overlap with each other. In this example, `klumpy` predicts 12 groups within this region. Although this is likely to not be the true number of groups, the binning of sequences into their respective groups can aid in the reconstruction of problematic loci.
 
 The remaining grouping-based arguments are `--min_grp`, `--write_groups` and `--write_edge_seqs`. The `--min_grp` flag accepts an integer to set as the minimum number of sequences required to form a group. The `--write_groups` flag is set to tell the program to write the groups to group-specific fasta files, which can be used for tasks such as local reassemblies or annotations. If your interests are more on clipped sequences at the ends/edges of the groups, implementing the `--write_edge_seqs` will write out the names of the clipped sequences at the ends/edges of the groups into group-specific *.txt* files. The following image highlights some of the edge sequences from above.
 
 <p align="center">
-<img src="Images/edge_seqs_example.png" width="50%" height="100%">
+<img src="./Images/edge_seqs_example.png" width="50%" height="100%">
 </p>
 
 # get_exons
 
 The purpose of this subprogram is to take a list of genes, and extract out their exonic sequences from a reference assembly. All arguments are required for this program.
 ```
     --fasta:                    Reference genome in fasta format [Required]
```

### Comparing `klumpy-1.0.5/klumpy/Classes.py` & `klumpy-1.0.6/klumpy/Classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,17 +47,17 @@
 
         return seq_rc
 
     # construct record
     __slots__ = "seq_name", "seq", "seq_rc", "seq_length"
 
     def __init__(self, seq_name : str, seq: str):
-        self.seq_name = seq_name
-        self.seq = seq.upper()
-        self.seq_rc = Seq_Record.reverse_complement(seq) # will automatically create R.C.
+        self.seq_name   = seq_name
+        self.seq        = seq.upper()
+        self.seq_rc     = Seq_Record.reverse_complement(seq) # will automatically create R.C.
         self.seq_length = len(seq)
 
 
     #use seq ID and assume short read
     def check_if_paired_end(self):
         if self.seq_length > 160:
             return False, None
@@ -74,64 +74,64 @@
         elif len(seq_name.split(" ")) == 2:
             casava_info = seq_name.split(" ")[-1]
             if len(casava_info.split(":")) == 4:
                 seq_info = casava_info.split(":")
                 if seq_info[0] in ["1", "2"]:
                     # following casava 1.8 format
                     if seq_info[1].upper() in ["Y", "N"]:
-                        paired = True
+                        paired   = True
                         pair_num = int(seq_info[0])
                     else:
-                        paired = False
+                        paired   = False
                         pair_num = None
             else:
-                paired = False
+                paired   = False
                 pair_num = None
             return paired, pair_num
         #error prone to conventional naming schemes
         else:
             return False, None
 
 # store klump details
 class Klump:
     def __init__(self, klump_name: str, start_pos: str, end_pos: str, query_source: str, klump_size: str, direction: str):
-        self.klump_name = klump_name
-        self.start_pos = int(start_pos)
-        self.end_pos = int(end_pos)
+        self.klump_name   = klump_name
+        self.start_pos    = int(start_pos)
+        self.end_pos      = int(end_pos)
         self.query_source = query_source
-        self.klump_size = int(klump_size)
-        self.direction = direction
-        self.pair_info = False
-        self.pair_num = None
+        self.klump_size   = int(klump_size)
+        self.direction    = direction
+        self.pair_info    = False
+        self.pair_num     = None
     
     # for paired data
     def add_pair_num(self, pair_num: int):
         self.pair_info = True
-        self.pair_num = pair_num
+        self.pair_num  = pair_num
 
 
 # for summarizing klumps
 class KLUMPS:
     def __init__(self, seq_name: str):
-        self.seq_name = seq_name
-        self.klumps = []
+        self.seq_name   = seq_name
+        self.klumps     = []
         self.all_klumps = {}
 
     def add_klumps(self, klump: Klump):
         self.klumps.append(klump)
 
     # to keep details in one place
     def create_all_klumps(self):
         for klump in self.klumps:
-            klump_name = klump.klump_name
-            start_pos = int(klump.start_pos)
-            end_pos = int(klump.end_pos)
+            klump_name   = klump.klump_name
+            start_pos    = int(klump.start_pos)
+            end_pos      = int(klump.end_pos)
             query_source = klump.query_source
-            size = int(klump.klump_size)
-            direction = klump.direction
+            size         = int(klump.klump_size)
+            direction    = klump.direction
             self.all_klumps[klump_name] = [
                 start_pos, end_pos, query_source, size, direction]
 
     def largest_klump(self):
         max_size = 0
         for klump in self.klumps:
             klump_size = klump.klump_size
@@ -160,109 +160,109 @@
     def queries(self):
         queries_list = list()
         for q in self.all_klumps.values():
             source = [s for s in q[2]]
             if source not in queries_list:
                 queries_list.append(source)
         # flatten list
-        flattened = [query for source in queries_list for query in source]
+        flattened         = [query for source in queries_list for query in source]
         self.queries_list = flattened
         return self.queries_list
 
     def which_directions(self):
         self.directions = set()
         for k in self.all_klumps.values():
             # get directions
             self.directions.add(k[4])
         return self.directions
 
     def both_strands(self):
         strand_directions = ""
         for q in self.all_klumps.values():
             strand_directions += q[4]
-        if "F" in strand_directions and "R" in strand_directions:
+        if 'F' in strand_directions and 'R' in strand_directions:
             return True
         else:
             return False
 
     def distances(self):
       # get distances b/t klumps
         if len(self.all_klumps) == 1:
             self.dist = [0]
         else:
             self.dist = []
             initial = True
             for vals in self.all_klumps.values():
                 # for initial ends
                 if initial is True:
-                    end = vals[1]
+                    end     = vals[1]
                     initial = False
                 else:
                     start = vals[0]
                     self.dist.append(abs(start - end))
                     # set new end
                     end = vals[1]
         return self.dist
 
 class SAM_FLAG:
     def __init__(self, flag: int):
-        self.primary = False
-        self.secondary = False
+        self.primary       = False
+        self.secondary     = False
         self.supplementary = False
-        self.fwd_seq = False
-        self.rev_seq = False
+        self.fwd_seq       = False
+        self.rev_seq       = False
         if (flag & 256) == 256:
             self.secondary = True
         elif (flag & 2048) == 2048:
             self.supplementary = True
         else:
             self.primary = True
 
 # class for blocks of the alignment when deletions are present
 class algn_blocks:
     def __init__(self):
-        self.blocks = {}
-        self.block_del = {} # large gaps separating block
-        self.MiniDels = {} # gaps within block
+        self.blocks         = {}
+        self.block_del      = {} # large gaps separating block
+        self.MiniDels       = {} # gaps within block
         self.aligned_length = 0
-        self.covered_len = 0
-        self.del_pos = None # used to hold positions of each deletion
+        self.covered_len    = 0
+        self.del_pos        = None # used to hold positions of each deletion
 
     def add_entry(self, block_num: int, block: list, deletion_len: str, del_cnt: int):
         block_id = f"block{block_num}"
         # avoid putting gap cnt at beginning and end of block
-        self.blocks[block_id] = block # gaps within block
+        self.blocks[block_id]    = block # gaps within block
         self.block_del[block_id] = int(deletion_len)
-        self.MiniDels[block_id] = del_cnt
+        self.MiniDels[block_id]  = del_cnt
 
     # for clips, start block after clip
     def adjust_start(self):
-        first_block = self.blocks["block0"]
-        clipped_site = first_block[0]
+        first_block           = self.blocks["block0"]
+        clipped_site          = first_block[0]
         self.blocks["block0"] = first_block[1:] # get all but 1st element
         return clipped_site
         
 
     # for clips, adjust for last clipping
     def adjust_end(self, adjust_end: int):
-        last_block = list(self.blocks.keys())[-1]
-        block = self.blocks[last_block]
+        last_block              = list(self.blocks.keys())[-1]
+        block                   = self.blocks[last_block]
         self.blocks[last_block] = sum(block) - adjust_end
 
     # to find overlapping alignments
     def covered_region(self, clipped_start: int, clipped_end: int):
         for block, values in self.blocks.items():
             # add deletion from within blocks
             del_cnt = self.MiniDels[block]
             # last block is type int, others are lists
             if type(values) == list:
-                self.blocks[block] = sum(values) + del_cnt
+                self.blocks[block]   = sum(values) + del_cnt
                 self.aligned_length += sum(values) + del_cnt
             else:
-                self.blocks[block] = values + del_cnt
+                self.blocks[block]   = values + del_cnt
                 self.aligned_length += values + del_cnt
         for value in self.block_del.values():
             self.aligned_length += value
         self.covered_len = self.aligned_length + clipped_start + \
                             clipped_end
 
     def get_ending_blocks(self):
@@ -281,58 +281,58 @@
                 "clipping_start", "adjust_start", "clipping_end", "adjust_end", "percent_aligned", \
                 "seq_len", "IsPrimary", "map_num", "aligned_length", "pair_num", "seq_color", "seq", "group_num"
      
     def __init__(self, seq_name: str, position: int, flag: int, chromosome: str, 
                  segment: bool, align_blocks : dict, clipping_start: str, adjust_start: int, 
                  clipping_end: str, adjust_end: int, percent_aligned: float, seq_len: int, 
                  IsPrimary: bool, map_num=None):
-        self.seq_name = seq_name
-        self.position = int(position)
-        self.flag = int(flag)
-        self.chromosome = chromosome
-        self.segment = segment # for hard clips
-        self.align_blocks = align_blocks #aligned len (includes soft clips)
-        self.aligned_length = align_blocks.aligned_length
-        self.clipping_start = clipping_start
-        self.adjust_start = adjust_start
-        self.clipping_end = clipping_end
-        self.adjust_end = adjust_end
+        self.seq_name        = seq_name
+        self.position        = int(position)
+        self.flag            = int(flag)
+        self.chromosome      = chromosome
+        self.segment         = segment # for hard clips
+        self.align_blocks    = align_blocks # aligned len (includes soft clips)
+        self.aligned_length  = align_blocks.aligned_length
+        self.clipping_start  = clipping_start
+        self.adjust_start    = adjust_start
+        self.clipping_end    = clipping_end
+        self.adjust_end      = adjust_end
         self.percent_aligned = float(percent_aligned)
-        self.seq_len = seq_len
-        self.IsPrimary = IsPrimary
-        self.map_num = map_num #  used to figure out if a particular alignment 
-                               #  overlaps with another
-        self.pair_num = 0 # modify after initialization
-        self.seq_color = ""
-        self.seq = ""
-        self.group_num = None
+        self.seq_len         = seq_len
+        self.IsPrimary       = IsPrimary
+        self.map_num         = map_num #  used to figure out if a particular alignment 
+                                       #  overlaps with another
+        self.pair_num        = 0 # modify after initialization
+        self.seq_color       = ""
+        self.seq             = ""
+        self.group_num       = None
 
 class Feature_Color:
     __slots__ = "red", "green", "blue", "alpha", "name"
 
     def __init__(self, red: float, green: float, blue: float, alpha = 1, name = None):
-        self.red = red
+        self.red   = red
         self.green = green
-        self.blue = blue
+        self.blue  = blue
         self.alpha = alpha
-        self.name = name
+        self.name  = name
 
 # will serve as a parent class for classes with start & end position members
 class Positions:
     def __init__(self, start_pos: int, end_pos: int):
         self.start_pos = int(start_pos)
-        self.end_pos = int(end_pos)
+        self.end_pos   = int(end_pos)
 
 class EXON(Positions):
     __slots__ = "start_pos", "end_pos", "direction", "gene_color", "gene_name"
     def __init__(self, start_pos: int, end_pos: int, direction: str, gene_color: Feature_Color):
         super().__init__(start_pos, end_pos)
-        self.direction = direction
+        self.direction  = direction
         self.gene_color = gene_color
-        self.gene_name = None
+        self.gene_name  = None
     
     def add_gene_name(self, gene_name: str):
         self.gene_name = gene_name
 
 class GENE(Positions):
     def __init__(self, start_pos: int, end_pos: int, gene_name: str):
         super().__init__(start_pos, end_pos)
@@ -341,54 +341,56 @@
 class GAP(Positions):
     pass
 
 class Kmer:
     __slots__ = "pos", "query", "direction"
 
     def __init__(self, pos: int, query: str, direction: str):
-        self.pos = int(pos)
-        self.query = query
+        self.pos       = int(pos)
+        self.query     = query
         self.direction = direction
 
 class STRUCTURE:
 
     __slots__ = "num_blocks", "num_del", "del_lengths", "align_pos", "align_end", "clipping_start", \
                 "clipping_end", "clip_start_len", "clip_end_len", "covered_regions", "deletion_regions", \
                 "clip_start", "clip_end", "seq_len", "percent_align", "num_align_bp", "seq_name", \
                 "align_num", "clipfree", "trustworthy"
     
     def __init__(self, num_blocks: int, num_del: int, del_lengths: list, align_pos: int, 
                  align_end: int, clipping_start: str, clipping_end: str, clip_start_len: int, 
                  clip_end_len: int, covered_regions: list, deletion_regions: list, 
                  clip_start: int, clip_end: int, seq_len: int, percent_align: float, 
                  num_align_bp: int, seq_name: str, align_num: int):
-        self.num_blocks = num_blocks
-        self.num_del = num_del
-        self.del_lengths = del_lengths
-        self.align_pos = align_pos
-        self.align_end = align_end
-        self.clipping_start = clipping_start
-        self.clipping_end = clipping_end
-        self.clip_start_len = clip_start_len
-        self.clip_end_len = clip_end_len
-        self.covered_regions = covered_regions # struct [[int, int], [int, int], ..]
+        self.num_blocks       = num_blocks
+        self.num_del          = num_del
+        self.del_lengths      = del_lengths
+        self.align_pos        = align_pos
+        self.align_end        = align_end
+        self.clipping_start   = clipping_start
+        self.clipping_end     = clipping_end
+        self.clip_start_len   = clip_start_len
+        self.clip_end_len     = clip_end_len
+        self.covered_regions  = covered_regions # struct [[int, int], [int, int], ..]
         self.deletion_regions = deletion_regions
-        self.clip_start = clip_start
-        self.clip_end = clip_end
-        self.seq_len = seq_len
-        self.percent_align = percent_align
-        self.num_align_bp = num_align_bp
-        self.seq_name = seq_name
-        self.align_num = align_num
+        self.clip_start       = clip_start
+        self.clip_end         = clip_end
+        self.seq_len          = seq_len
+        self.percent_align    = percent_align
+        self.num_align_bp     = num_align_bp
+        self.seq_name         = seq_name
+        self.align_num        = align_num
         # members to be checked upon evaluation
-        self.clipfree = True
-        self.trustworthy = True
+        self.clipfree         = True
+        self.trustworthy      = True
 
-    def evaluate(self, min_len: int, t_per: float):
-        if self.clipping_start or self.clipping_end:
+    def evaluate(self, min_len: int, t_per: float, clip_tolerance: int):
+        if (self.clip_start_len <= clip_tolerance) and (self.clip_end_len <= clip_tolerance):
+            self.clipfree = True
+        else:
             self.clipfree = False
         if self.seq_len < min_len or self.percent_align < t_per:
             self.trustworthy = False
 
 class Del_Window(Positions):
     def __init__(self, start_pos: int, end_pos: int, seq: str):
         super().__init__(start_pos, end_pos)
@@ -401,51 +403,51 @@
 # compatibility score
 class C_Score:
     __slots__ = "incompatible", "groupable", "likely", "reasonable", "unlikely", \
                 "possible", "evidence", "POE"
 
     def __init__(self):
         self.incompatible = False
-        self.groupable = False
-        self.likely = False
-        self.reasonable = False
-        self.unlikely = False
-        self.possible = False
-        self.evidence = 0
-        self.POE = []
+        self.groupable    = False
+        self.likely       = False
+        self.reasonable   = False
+        self.unlikely     = False
+        self.possible     = False
+        self.evidence     = 0
+        self.POE          = []
 
     def __str__(self):
         s = f"Incompatibility = {self.incompatible}, Groupable = {self.groupable}, " + \
             f"Likely = {self.likely}, Reasonable = {self.reasonable}, Unlikely = {self.unlikely}, " + \
             f"Possible = {self.possible}"
         return s 
     
 # to retain gene identifiers in GTF/GFF files
 class GeneRecord:
     def __init__(self):
-        self.gene_name = None # GTF ids
-        self.gene_id = None
-        self.id = None # GFF ids
-        self.prot_id = None
-        self.parent = None # to trace back to ID
-        self.name = None # may be the same as ID in some cases
-        self.other_ids = set() # store other ids for the record
-        self.visited = list() # to know if a new record has been encountered
-        self.exon_list = list()
+        self.gene_name  = None # GTF ids
+        self.gene_id    = None
+        self.id         = None # GFF ids
+        self.prot_id    = None
+        self.parent     = None # to trace back to ID
+        self.name       = None # may be the same as ID in some cases
+        self.other_ids  = set() # store other ids for the record
+        self.visited    = list() # to know if a new record has been encountered
+        self.exon_list  = list()
         self.prev_added = set() # just in case exon already added
-        self.retain = list() # to store entries not added to visited
-        self.ref = None # used for get exons to remember which ref seq
+        self.retain     = list() # to store entries not added to visited
+        self.ref        = None # used for get exons to remember which ref seq
 
     def prune_id(gene_id: str):
         # remove extra information from gene attributes subfield 
         # not a optimal approach as it keeps reconstructing a str obj
 
         for s in ["gene", "exon", "rna", "transcript"]:
             if gene_id.lower().startswith(s):
-                s_len = len(s)
+                s_len   = len(s)
                 prunned = False
                 for e in ['-', ':', '_']:
                     if gene_id.lower().startswith(f"{s}{e}"):
                         gene_id = gene_id[s_len:]
                         prunned = True
                         break
                 if not prunned:
@@ -469,23 +471,23 @@
     # process the attributes field
     def parse_attributes(self, entry_info: str):
 
         info_map = {}
 
         # make a dict of the of the info
         for field in entry_info.split(';'):
-            field = field.strip()
+            field    = field.strip()
             key_vals = field.split(' ')
             if len(key_vals) == 1: # not space separated
                 key_vals = field.split('=') # assume = delimited
             try:
                 id_key = key_vals[0].lower()
                  # remove quotes & spaces
-                id_val = key_vals[1].replace('"', '').replace(' ', '')
-                id_val = GeneRecord.prune_id(id_val)
+                id_val           = key_vals[1].replace('"', '').replace(' ', '')
+                id_val           = GeneRecord.prune_id(id_val)
                 info_map[id_key] = id_val
             except:
                 # if last field is empty
                 continue
 
         # add whatever ids we obtained
         if "gene_id" in info_map:
@@ -566,35 +568,35 @@
             self.visited.append(entry_type)
 
         return False
     
         # reset object
     def clear(self):
         self.gene_name = None
-        self.gene_id = None
-        self.id = None
-        self.prot_id = None
-        self.parent = None
-        self.name = None
+        self.gene_id   = None
+        self.id        = None
+        self.prot_id   = None
+        self.parent    = None
+        self.name      = None
         self.other_ids.clear()
         self.visited.clear()
         self.exon_list.clear()
         self.prev_added.clear()
-        self.ref = None
+        self.ref       = None
 
         # move prev entries haven't added during update check
         self.visited = self.retain[::] # this should construct a new copy
         self.retain.clear()
      
     def add_exon(self, left: int, right: int, direction: str, gene_color: Feature_Color, line: str):
         
         # some safety checks
         if left > right:
             right, left = left, right
-        assert left >= 0, f"Encountered an entry where left ({left}) is less than 0. Offending line:\n{line}"
+        assert left  >= 0, f"Encountered an entry where left ({left}) is less than 0. Offending line:\n{line}"
         assert right >= 0, f"Encountered an entry where right ({right}) is less than 0. Offending line:\n{line}"
         assert direction in ['+', '-'], f"Encountered an entry where direction ({direction}) cannot be determined. Offending line:\n{line}"
         
         # avoid dup entries
         if (left, right, direction) not in self.prev_added:
             self.exon_list.append(EXON(left, right, direction, gene_color))
             self.prev_added.add((left, right, direction)) # assuming positions will always be dup
@@ -609,16 +611,16 @@
     def get_ref(self):
         return self.ref if self.ref != None else ''
     
     # a function for get_exons to see if id in any in the current ids
     def in_record(self, genes: list):
         # put all ids together
         all_ids = set()
-        ids_ = [self.gene_id, self.gene_name, self.id, self.prot_id, self.parent,
-                self.name]
+        ids_    = [self.gene_id, self.gene_name, self.id, 
+                   self.prot_id, self.parent, self.name]
         
         # non-Nones
         for i in ids_:
             if i != None:
                 all_ids.add(i)
         
         # add just in case
```

### Comparing `klumpy-1.0.5/klumpy/__init__.py` & `klumpy-1.0.6/klumpy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Klumpy. If not, see <http://www.gnu.org/licenses/>.
 #
 
-from .alignment_plot import Alignment_Plot
-from .combine_klumps import Combine_Klumps
-from .find_gaps import Find_Gaps
-from .find_klumps import Find_Klumps
-from .get_exons import Get_Exons
-from .klump_plot import Klump_Plot
-from .kmerize import Kmerize
-from .klump_sizes import Klump_Sizes
-from .scan_alignments import Scan_Alignments
+from  .alignment_plot  import Alignment_Plot
+from  .combine_klumps  import Combine_Klumps
+from  .find_gaps       import Find_Gaps
+from  .find_klumps     import Find_Klumps
+from  .get_exons       import Get_Exons
+from  .klump_plot      import Klump_Plot
+from  .kmerize         import Kmerize
+from  .klump_sizes     import Klump_Sizes
+from  .scan_alignments import Scan_Alignments
 import pkg_resources
 
 try:
     __version__ = pkg_resources.get_distribution('klumpy').version
 except Exception:
-    __version__ = "1.0.4"
+    __version__ = "1.0.6"
```

### Comparing `klumpy-1.0.5/klumpy/__main__.py` & `klumpy-1.0.6/klumpy/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,15 +59,14 @@
         --limit:                    Number of subject sequences to load into memory at once (default 10000)        
 
         
 Options for `scan_alignment`:
     --alignment_map:            A sorted and indexed SAM/BAM file [Required]
     --min_len:                  Minimum length a sequence must be to retain an alignment in the grouping analysis (default = 2000)
     --min_percent:              Minimum percent a sequence must be aligned for the alignment to be retained in the grouping analysis (default = 50)
-    --num_of_groups:            Number of groups at a window to flag the window (default = 3)
     --threads:                  Number of threads (default = 1)
     --annotation:               Gene annotations in GTF/GFF3 format [Optional]
 
     Advanced options:
         --deletion_len:             Minimum length of deletion to draw and split alignment into blocks (default = 100)
         --assume_sep_del:           If set, remove the assumption that overlapping alignments with deletions can be automatically grouped if compatible
         --clip_tolerance:           Number of clipped base pairs to tolerate when comparing two alignments for compatibility (default = 400)
@@ -76,16 +75,18 @@
         --t_len:                    Minimum length a sequence must be in order to trust its assignment when grouping (default = 2000)
         --t_per:                    Minimum percentage a sequence must be aligned in order to trust its assignment when grouping (default = 30)
         --align_offset:             Maximum number of base pairs apart for two sequences to be considered aligned at the same position (default = 100)
         --min_grp:                  Minimum number of sequences in a group in order to retain the group (default = 10)
         --window_size:              Length (in bp) for the sliding window to be (default = 50000)
         --window_step:              Length (in bp) for the sliding window to slide down to establish the next window (default = 25000) 
         --limit:                    Maximum number of alignments to process in a window (default 10000)
+        --num_of_groups:            Number of groups at a window to flag the window (default = 3)
+        --flag_excess_groups:       If set, will report regions with --num_of_groups Groups or more regardless if the region was tiled or not (default = False)
+
 
-        
 Options for `alignment_plot`:
     --alignment_map:            A sorted and indexed SAM/BAM file [Required]
     --reference:                Name of reference sequence
     --leftbound:                Leftmost Position in the reference genome (default = 0)
     --rightbound:               Rightmost Position in the reference genome (default = 50000)
     --region_num:               Region Number in a *_Candidate_Regions.tsv file generated by `scan_alignments` (default = 1)
     --candidates:               A *_Candidate_Regions.tsv file generated from `scan_alignments`
@@ -121,15 +122,15 @@
         --no_subsample:             If set, will not randomly subsample alignments when the number of alignments is greater than --limit
         --supplementary:            If set, supplementary alignments will be kept if they pass all other filters
         --secondary:                If set, secondary alignments will be kept if they pass all other filters
         --write_groups:             If set, the sequences for each group will be written out in fasta format (one file per group)
         --write_seqs:               If set, the sequences that were plotted will be written in fasta format
         --write_edge_seqs:          If set, sequences with clipped alignments at the edges/ends of their groups will have their names written to a list
         --assume_sep_del:           If set, remove the assumption that overlapping alignments with deletions can be automatically grouped if compatible
-        --clip_tolerance:           Number of clipped base pairs to tolerate when comparing two alignments for compatibility (default = 400)
+        --clip_tolerance:           Number of clipped base pairs to tolerate when comparing two alignments for compatibility (default = 150)
         --del_tolerance:            Length (in bp) covered by a deletion to be tolerated when comparing two alignments for compatibility (default = 50)
         --limit:                    Maximum number of alignments to process in a group analysis and draw (default 10000)
         --per_overlap:              Minimum percent two sequences need to overlap one another in order to confidently consider them compatible
         --t_len:                    Minimum length a sequence must be in order to trust its assignment when grouping (default = 2000)
         --t_per:                    Minimum percentage a sequence must be aligned in order to trust its assignment when grouping (default = 30)
         --align_offset:             Maximum number of base pairs apart for two sequences to be considered aligned at the same position (default = 100)
         --min_grp:                  Minimum number of sequences in a group in order to retain the group (default = 10)
@@ -184,86 +185,86 @@
     --ksize:                    Length of k-mer (must be an integer greater than 0) (default = 17)
 '''
 
 def get_arguments():
     """get the arguments"""
 
     parser = argparse.ArgumentParser(description="Klumpy: A bioinformatic tool for untangling collapsed genomes", prog="klumpy")
-    parser.add_argument("analysis", choices = ["alignment_plot", "combine_klumps", "find_gaps", "find_klumps", "get_exons", "kmerize", "klump_plot", "klump_sizes", "scan_alignments"])
-    parser.add_argument("--align_offset", default=100, type=int)
-    parser.add_argument("--alignment_map", default=None, type=str)
-    parser.add_argument("--annotation", default=None, type=str)
-    parser.add_argument("--assume_sep_del", action="store_false")    
-    parser.add_argument("--candidates", default=None, type=str)
-    parser.add_argument("--clip_tolerance", default=400, type=int)
-    parser.add_argument("--color", default="blue", type=str)
-    parser.add_argument("--color_by_gene", action="store_true")
-    parser.add_argument("--del_tolerance", default=50, type=float)
-    parser.add_argument("--deletion_len", default=100, type=float)
-    parser.add_argument("--fasta", default=None, type=str)
-    parser.add_argument("--fix_width", action="store_true")
-    parser.add_argument("--format", default="pdf", type=str, choices=["pdf", "png", "svg"])
-    parser.add_argument("--gap_file", default=None, type=str)
-    parser.add_argument("--genes", default=None, nargs='*')
-    parser.add_argument("--group_seqs", action="store_true")
-    parser.add_argument("--height", default=2000, type=int)
-    parser.add_argument("--klump_count", default=1, type=int)
-    parser.add_argument("--klump_colors", default=None, type=str)
-    parser.add_argument("--klumps_tsv", default=None, type=str)
-    parser.add_argument("--klumps_tsv_list", default=None, nargs='*')
-    parser.add_argument("--ksize", default=17, type=int)
-    parser.add_argument("--leftbound", default=1, type=float)
-    parser.add_argument("--limit", default=10000, type=int)
-    parser.add_argument("--list_colors", action="store_true")
-    parser.add_argument("--max_percent", default=100.0, type=float)
-    parser.add_argument("--min_grp", default=10, type=int)
-    parser.add_argument("--min_klump_size",default=1, type=int)
-    parser.add_argument("--min_kmers",default=1, type=int)
-    parser.add_argument("--min_len", default=2000, type=float)
-    parser.add_argument("--min_percent", default=0.50, type=float)
-    parser.add_argument("--no_primary", action="store_true")
-    parser.add_argument("--no_subsample", action="store_true")
-    parser.add_argument("--num_of_groups", default=2, type=int)
-    parser.add_argument("--number", action="store_true")
-    parser.add_argument("--output", default=None, type=str)
-    parser.add_argument("--paired", action="store_true") 
-    parser.add_argument("--per_overlap", default=0.50, type=float)
-    parser.add_argument("--plotting_list", default=None, type=str)
-    parser.add_argument("--query", default=None, type=str)
-    parser.add_argument("--query_count",default=1, type=int)
-    parser.add_argument("--query_map", default=None, type=str)
-    parser.add_argument("--range", default=1000, type=int)
-    parser.add_argument("--reference", default=None, type=str)
-    parser.add_argument("--region_num", default=1, type=int)
-    parser.add_argument("--rightbound", default=50000, type=float)
-    parser.add_argument("--secondary", action="store_true")
-    parser.add_argument("--seq_name", default=None, type=str)
-    parser.add_argument("--subject", default=None, type=str)
-    parser.add_argument("--supplementary", action="store_true")
-    parser.add_argument("--t_len", default=2000, type=float)
-    parser.add_argument("--t_per", default=0.30, type=float)
-    parser.add_argument("--tick_count", default=None, type=int)
-    parser.add_argument("--tick_span", default=None, type=float)
-    parser.add_argument("--threads", default=1, type=int)
-    parser.add_argument("--vertical_line_exons", action="store_true")
-    parser.add_argument("--vertical_line_gaps", action="store_true")
+    parser.add_argument("analysis",               choices = ["alignment_plot", "combine_klumps", "find_gaps", "find_klumps", "get_exons", "kmerize", "klump_plot", "klump_sizes", "scan_alignments"])
+    parser.add_argument("--align_offset",         default=250,  type=int)
+    parser.add_argument("--alignment_map",        default=None, type=str)
+    parser.add_argument("--annotation",           default=None, type=str)
+    parser.add_argument("--assume_sep_del",       action="store_false")    
+    parser.add_argument("--candidates",           default=None,   type=str)
+    parser.add_argument("--clip_tolerance",       default=250,    type=int)
+    parser.add_argument("--color",                default="blue", type=str)
+    parser.add_argument("--color_by_gene",        action="store_true")
+    parser.add_argument("--del_tolerance",        default=50,   type=float)
+    parser.add_argument("--deletion_len",         default=100,  type=float)
+    parser.add_argument("--fasta",                default=None, type=str)
+    parser.add_argument("--flag_excess_groups",   action="store_true")
+    parser.add_argument("--fix_width",            action="store_true")
+    parser.add_argument("--format",               default="pdf", type=str, choices=["pdf", "png", "svg"])
+    parser.add_argument("--gap_file",             default=None,  type=str)
+    parser.add_argument("--genes",                default=None,  nargs='*')
+    parser.add_argument("--group_seqs",           action="store_true")
+    parser.add_argument("--height",               default=2000,  type=int)
+    parser.add_argument("--klump_count",          default=1,     type=int)
+    parser.add_argument("--klump_colors",         default=None,  type=str)
+    parser.add_argument("--klumps_tsv",           default=None,  type=str)
+    parser.add_argument("--klumps_tsv_list",      default=None,  nargs='*')
+    parser.add_argument("--ksize",                default=17,    type=int)
+    parser.add_argument("--leftbound",            default=1,     type=float)
+    parser.add_argument("--limit",                default=10000,  type=int)
+    parser.add_argument("--list_colors",          action="store_true")
+    parser.add_argument("--max_percent",          default=100.0, type=float)
+    parser.add_argument("--min_grp",              default=10,    type=int)
+    parser.add_argument("--min_klump_size",       default=1,     type=int)
+    parser.add_argument("--min_kmers",            default=1,     type=int)
+    parser.add_argument("--min_len",              default=2000,  type=float)
+    parser.add_argument("--min_percent",          default=0.50,  type=float)
+    parser.add_argument("--no_primary",           action="store_true")
+    parser.add_argument("--no_subsample",         action="store_true")
+    parser.add_argument("--num_of_groups",        default=3,    type=int)
+    parser.add_argument("--number",               action="store_true")
+    parser.add_argument("--output",               default=None, type=str)
+    parser.add_argument("--paired",               action="store_true") 
+    parser.add_argument("--per_overlap",          default=0.50, type=float)
+    parser.add_argument("--plotting_list",        default=None, type=str)
+    parser.add_argument("--query",                default=None, type=str)
+    parser.add_argument("--query_count",          default=1,    type=int)
+    parser.add_argument("--query_map",            default=None, type=str)
+    parser.add_argument("--range",                default=1000, type=int)
+    parser.add_argument("--reference",            default=None, type=str)
+    parser.add_argument("--region_num",           default=1,    type=int)
+    parser.add_argument("--rightbound",           default=50000, type=float)
+    parser.add_argument("--secondary",            action="store_true")
+    parser.add_argument("--seq_name",             default=None, type=str)
+    parser.add_argument("--subject",              default=None, type=str)
+    parser.add_argument("--supplementary",        action="store_true")
+    parser.add_argument("--t_len",                default=2000, type=float)
+    parser.add_argument("--t_per",                default=0.30, type=float)
+    parser.add_argument("--tick_count",           default=None, type=int)
+    parser.add_argument("--tick_span",            default=None, type=float)
+    parser.add_argument("--threads",              default=1,    type=int)
+    parser.add_argument("--vertical_line_exons",  action="store_true")
+    parser.add_argument("--vertical_line_gaps",   action="store_true")
     parser.add_argument("--vertical_line_klumps", action="store_true")
-    parser.add_argument("--view_span", default=1000000, type=float)
-    parser.add_argument("--width", default=2000, type=int)
-    parser.add_argument("--window_size",  default=50000, type=float)
-    parser.add_argument("--window_step",  default=25000, type=float)
-    parser.add_argument("--write_edge_seqs", action="store_true")
-    parser.add_argument("--write_groups", action="store_true")
-    parser.add_argument("--write_seqs", action="store_true")
-    parser.add_argument("--write_table", action="store_true")
+    parser.add_argument("--view_span",            default=1000000, type=float)
+    parser.add_argument("--width",                default=2000,    type=int)
+    parser.add_argument("--window_size",          default=50000,   type=float)
+    parser.add_argument("--window_step",          default=25000,   type=float)
+    parser.add_argument("--write_edge_seqs",      action="store_true")
+    parser.add_argument("--write_groups",         action="store_true")
+    parser.add_argument("--write_seqs",           action="store_true")
+    parser.add_argument("--write_table",          action="store_true")
 
     # change usage
     parser.format_usage = lambda : Usage
-    parser.format_help = parser.format_usage
-
+    parser.format_help  = parser.format_usage
 
     # parse the arguements and return the entire collection of inputs
     args = parser.parse_args()
 
     return args
   
 def main():
```

### Comparing `klumpy-1.0.5/klumpy/alignment_plot.py` & `klumpy-1.0.6/klumpy/alignment_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,43 +19,43 @@
 
 import math
 import cairo
 import sys
 import gzip
 import os
 import random
-from collections import defaultdict
-from typing import List
-from .Classes import SAM, SAM_FLAG, GAP, Feature_Color, Klump, GeneRecord, algn_blocks, Label_Position
-from .grouping import Group_Seqs, within_window
+from   collections import defaultdict
+from   typing      import List
+from  .Classes     import SAM, SAM_FLAG, GAP, Feature_Color, Klump, GeneRecord, algn_blocks, Label_Position
+from  .grouping    import Group_Seqs, within_window
 
 ########## safety/validating functions #############
 
 def check_tick_params(tick_count: int, tick_span: float, leftbound: int, rightbound: int):
     """a function to verify that the tick counts are legal or need some modification"""
 
     # do some assertions
     if tick_count != None:
         assert type(tick_count) == int, "--tick_count requires an integer"
-        assert tick_count >= 0, "--tick_count cannot be negative"
+        assert tick_count >= 0,         "--tick_count cannot be negative"
         if tick_span != None:
             assert type(tick_span) == float, "--tick_span requires a number [float or int]"
-            assert tick_span > 0, "--tick_span must be greater than 0"
+            assert tick_span > 0,            "--tick_span must be greater than 0"
             tick_span = int(tick_span)
             last_tick = leftbound + (tick_count * tick_span)
             if last_tick > rightbound:
                 msg = f"--rightbound set to {rightbound}." + \
-                    f"Setting --tick_count to {tick_count} and --tick_span to {tick_span} places last tick at {last_tick}"
+                      f"Setting --tick_count to {tick_count} and --tick_span to {tick_span} places last tick at {last_tick}"
                 sys.exit(msg)
         else:
             # estimate tick_span
             tick_span = (rightbound - leftbound) // (tick_count + 1) # do not include rightbound pos
     elif tick_span != None:
         assert type(tick_span) == float, "--tick_span requires a number [float or int]"
-        assert tick_span > 0, "--tick_span must be greater than 0"
+        assert tick_span > 0,            "--tick_span must be greater than 0"
         tick_span = int(tick_span)
         assert leftbound + tick_span < rightbound, f"--tick_span {tick_span} + --leftbound {leftbound} is greater than --rightbound {rightbound}"
         tick_count = ((rightbound - leftbound) // (tick_span)) # - 1  # TODO this minus 1 may need to be re-implemented in the future
     else:
         tick_count, tick_span = None, None
 
     # if passed all checks, return validated values
@@ -78,29 +78,29 @@
     
     fmsg = var + " must be a number"
     imsg = var + " cannot be a negative integer"
 
     try:
         val = int(val)
         assert type(val) == int, fmsg
-        assert 0 <= val, imsg
+        assert 0 <= val,         imsg
     except:
         sys.exit(fmsg)
 
     return val
 
 def check_args(args):
     """determine if params are acceptable"""
 
     assert type(args.list_colors) is bool, "--list_colors does not take any positional values"
     if args.list_colors:
         get_color(True, False, 0)
 
     warning_color = "\033[93m"
-    end_color = "\033[0m"
+    end_color     = "\033[0m"
 
     # check if alignment file exists and samtools is in path
     if args.alignment_map == None:
         msg = "--alignment_map SAM/BAM file is required for alignment_plot"
         sys.exit(msg)
     if os.path.isfile(args.alignment_map):
         in_path = os.popen("which samtools").read()
@@ -116,61 +116,61 @@
             sys.exit(msg) 
     else:
         msg = f"Could not find {args.alignment_map}"
         sys.exit(msg)
 
     # check if a reference or candidates file was provided
     if args.reference == None:
-        assert args.candidates != None, "No --candidates or --reference argument provided"
+        assert args.candidates != None,          "No --candidates or --reference argument provided"
         assert os.path.isfile(args.candidates), f"Could not locate {args.candidates}"
-        assert type(args.region_num) == int, "--region_num must be an integer"
+        assert type(args.region_num) == int,     "--region_num must be an integer"
         # assign values
-        ref, l, r = parse_candidates(args.candidates, args.region_num)
-        args.reference = ref
-        args.leftbound = l
+        ref, l, r       = parse_candidates(args.candidates, args.region_num)
+        args.reference  = ref
+        args.leftbound  = l
         args.rightbound = r
     
     # no else b/c it is not none by now
     
     # check inputs for non-scan pipeline
     # make sure bounds are reasonable
     # adjusts for extending past reference seq
     # this will also cause an error if leftbound is greater than ref len
     assert args.leftbound >= 0, "Leftbound cannot be a negative number" 
     args.rightbound = \
         adjust_rightbound(args.reference, args.rightbound, args.alignment_map)
     assert args.rightbound > args.leftbound, "Rightbound must be greater than leftbound"
-    assert args.view_span >= 0, "The view offset used when calling samtools must be greater or equal to 0"
-    assert args.height > 0, "Figure height must be greater than 0"
-    assert args.width > 0, "Figure width must be greater than 0"
-    assert args.min_len > 0, "--min_len must be greater than 0"
+    assert args.view_span >= 0,              "The view offset used when calling samtools must be greater or equal to 0"
+    assert args.height    > 0,               "Figure height must be greater than 0"
+    assert args.width     > 0,               "Figure width must be greater than 0"
+    assert args.min_len   > 0,               "--min_len must be greater than 0"
 
     # convert params to ints
-    args.leftbound = int(args.leftbound)
-    args.min_len = int(args.min_len)
-    args.deletion_len = int(args.deletion_len)
+    args.leftbound                  = int(args.leftbound)
+    args.min_len                    = int(args.min_len)
+    args.deletion_len               = int(args.deletion_len)
     args.tick_count, args.tick_span = \
         check_tick_params(args.tick_count, args.tick_span, args.leftbound, args.rightbound)
 
     # ensure one type of alignment is to be retained
     if args.no_primary:
         if args.secondary == False and args.supplementary == False:
             msg = "Error. Filtering out primary, secondary, and supplementary alignments\n" + \
-                "Please ensure 1 type of alignment is to be retained"
+                  "Please ensure 1 type of alignment is to be retained"
             sys.exit(msg)
 
     # other params to verify
     assert type(args.deletion_len) is int, "--deletion_len must be an integer"
     if args.plotting_list != None:
         assert os.path.isfile(args.plotting_list), f"Could not find {args.plotting_list}"
 
     #check gtf/gff3 file 
     if args.annotation != None:
         if os.path.isfile(args.annotation):
-            if (args.annotation.endswith(".gtf.gz")) or (args.annotation.endswith(".gtf")):
+            if (args.annotation.endswith(".gtf.gz"))   or (args.annotation.endswith(".gtf")):
                 pass
             elif (args.annotation.endswith(".gff.gz")) or (args.annotation.endswith(".gff")) or \
                 (args.annotation.endswith(".gff3.gz")) or (args.annotation.endswith(".gff3")):
                 pass
             else:
                 msg = f"No .gtf, .gtf.gz, .gff, .gff.gz, .gff3, or .gff3.gz file extension detected in {args.annotation}" + \
                     "\nAssuming proper input"
@@ -202,62 +202,62 @@
                 args.vertical_line_gaps = False
     else:
         args.vertical_line_gaps = False
 
     if args.klumps_tsv != None:
         assert os.path.isfile(args.klumps_tsv), f"Could not find {args.klumps_tsv}"
         assert type(args.min_klump_size) is int, "--min_klump_size must be an integer"
-        assert args.min_klump_size >= 0, "--min_klump_size must be greater or equal to 0"
+        assert args.min_klump_size >= 0,         "--min_klump_size must be greater or equal to 0"
         #check if drawing vertical dashes at klumps
         assert type(args.vertical_line_klumps) is bool, "--vertical_line_klumps does not take any positional values"
         if args.vertical_line_klumps:
             if args.klumps_tsv == None:
                 msg = "WARNING: Drawing vertical lines at klumps requires klumps tsv file for klump locations"
                 print(f"{warning_color}{msg}{end_color}")
         if args.klump_colors != None:
             assert os.path.isfile(args.klump_colors), f"Could not find {args.klump_colors}"
-            assert type(args.color_by_gene) == bool, "--color_by_gene does not take any arguments"
+            assert type(args.color_by_gene) == bool,   "--color_by_gene does not take any arguments"
     else:
         args.vertical_line_klumps = False   
 
     # check for currently available colors and set as default
     args.color = get_color(False, False, 0, args.color)
 
     # check other boolean params
     assert type(args.supplementary) is bool, "--supplementary does not taken any positional values"
-    assert type(args.secondary) is bool, "--secondary does not take any positional values"
-    assert type(args.number) is bool, "--number does not take any positional values"
-    assert type(args.write_table) is bool, "--write_table does not take any positional values"
-    assert type(args.paired) is bool, "--paired does not take any positional values"
-    assert type(args.group_seqs) is bool, "--group_seqs does not take any positional values"
-    assert type(args.no_subsample) is bool, "--no_subsample does not take any positional values"
+    assert type(args.secondary)     is bool, "--secondary does not take any positional values"
+    assert type(args.number)        is bool, "--number does not take any positional values"
+    assert type(args.write_table)   is bool, "--write_table does not take any positional values"
+    assert type(args.paired)        is bool, "--paired does not take any positional values"
+    assert type(args.group_seqs)    is bool, "--group_seqs does not take any positional values"
+    assert type(args.no_subsample)  is bool, "--no_subsample does not take any positional values"
 
     #check for percentages
-    msg = "Minimum mapping"
+    msg              = "Minimum mapping"
     args.min_percent = percent_check(args.min_percent, msg)
-    msg = "Maximum mapping"
+    msg              = "Maximum mapping"
     args.max_percent = percent_check(args.max_percent, msg)
     assert args.min_percent <= args.max_percent, "--min_percent cannot be higher than --max_percent"
    
     # currently only supports non-paired end
     if args.group_seqs:
-        msg = "Minimum percent for trusting a sequence when grouping"
-        args.t_per = percent_check(args.t_per, msg)
-        msg = "Minimum percent for confidently grouping two sequences"
-        args.per_overlap = percent_check(args.per_overlap, msg)
-        args.align_offset = group_assert(args.align_offset, "Alignment Offset")
+        msg                 = "Minimum percent for trusting a sequence when grouping"
+        args.t_per          = percent_check(args.t_per, msg)
+        msg                 = "Minimum percent for confidently grouping two sequences"
+        args.per_overlap    = percent_check(args.per_overlap, msg)
+        args.align_offset   = group_assert(args.align_offset, "Alignment Offset")
         args.clip_tolerance = group_assert(args.clip_tolerance, "Clip tolerance")
-        args.del_tolerance = group_assert(args.del_tolerance, "Deletion tolerance")
-        args.t_len = group_assert(args.t_len, "Trustworthy length")
-        args.min_grp = group_assert(args.min_grp, "Minimum group")
-        assert type(args.assume_sep_del) is bool, "--assume_sep_del does not take any positional values"
-        assert type(args.write_groups) is bool, "--write_groups does not take any positional values"
-        assert type(args.write_seqs) is bool, "--write_seqs does not take any positional values"
+        args.del_tolerance  = group_assert(args.del_tolerance, "Deletion tolerance")
+        args.t_len          = group_assert(args.t_len, "Trustworthy length")
+        args.min_grp        = group_assert(args.min_grp, "Minimum group")
+        assert type(args.assume_sep_del)  is bool, "--assume_sep_del does not take any positional values"
+        assert type(args.write_groups)    is bool, "--write_groups does not take any positional values"
+        assert type(args.write_seqs)      is bool, "--write_seqs does not take any positional values"
         assert type(args.write_edge_seqs) is bool, "--write_edge_seqs does not take any positional values"
-        assert args.limit >= 0, "--limit must be >= 0"
+        assert args.limit                    >= 0, "--limit must be >= 0"
 
         msg = f"WARNING: Grouping Sequences currently only uses primary alignments. " 
         if args.supplementary == args.secondary == True:
             msg = msg + "Excluding supplementary and secondary alignments"
             print(f"{warning_color}{msg}{end_color}")
             args.supplementary = False
             args.secondary = False
@@ -293,24 +293,24 @@
 ######### parsing functions ############
 
 def parse_candidates(candidates_tsv: str, region_num: int):
     """parse a candidates file for a region & return the positions of the window"""
 
     fh = gzip.open(candidates_tsv, "rt") if candidates_tsv.endswith(".gz") else open(candidates_tsv, 'r')
 
-    reference = None
+    reference  = None
     region_num = str(region_num) # a single conversion
 
     for line in fh:
         if line[0] == '#' or line.startswith("Region_Num\t"):
             continue
         fields = line.strip().split('\t')
         if fields[0] == region_num: # found the region
-            reference = fields[1]
-            leftbound = int(fields[2]) + 1
+            reference  = fields[1]
+            leftbound  = int(fields[2]) + 1
             rightbound = int(fields[3]) # will keep this as is and assume it is inclusive
             break
 
     fh.close()
 
     if reference == None:
         msg = f"Could not locate region number: {region_num}"
@@ -318,23 +318,23 @@
     else:
         return reference, leftbound, rightbound 
 
 def parse_klumps_out(klump_file: str, min_len: int, klump_size: int, paired_end: bool):
     """get klump info per sequence"""
 
     warning_color = "\033[93m"
-    end_color = "\033[0m"
+    end_color     = "\033[0m"
 
     #determine if parsing to returning None's
     if klump_file == None:
         return None, None
     
     fh = gzip.open(klump_file, "rt") if klump_file.endswith(".gz") else open(klump_file, 'r')
 
-    seq_klumps = {}
+    seq_klumps  = {}
     seq_lengths = {}
 
     for line in fh:
         if line.startswith(f"Sequence\t"):
             continue
         fields = line.strip().split("\t")
         #plotting only min_len seqs and klumps
@@ -391,36 +391,37 @@
     # import once
     if grouping or write_seqs:
         from .Classes import Seq_Record
 
     # samtools does not return alignments where the clip is within the region
     # so I will look ~500 Mb from the region of interest in both directions
     # in theory, MOST cases should be able to cover this region
-    left_search = leftbound - view_len
+    left_search  = leftbound - view_len
+    right_search = rightbound + view_len
+
     if left_search < 0:
         left_search = 0
-    right_search = rightbound + view_len
 
     cmd = f"samtools view {align_map} " + '"' + f"{ref}:{left_search}-{right_search}" + '"'
-    fh = os.popen(cmd, 'r')
+    fh  = os.popen(cmd, 'r')
 
     for line in fh:
         if line.startswith('@'):
             continue
         fields = line.strip('\n').split('\t')
         #check if even considering the sequence
         if plotting_list != None:
             if r'{}'.format(fields[0]) not in plotting_list:
                 continue
         # index fields for passing filters
-        seq_name = fields[0]
-        seq_flag = int(fields[1])
-        seq_cigar = fields[5]
+        seq_name          = fields[0]
+        seq_flag          = int(fields[1])
+        seq_cigar         = fields[5]
         leftmost_position = int(fields[3]) + 1 # SAM/BAM is 0-based
-        paired = False #assume not paired-end
+        paired            = False #assume not paired-end
         #get seq length if not in seq_lengths
         if seq_name not in seq_lengths:
             seq_lengths[seq_name] = estimate_seq_length(seq_cigar)
         # skip short seqs
         sequence_length = seq_lengths[seq_name]
         if sequence_length < min_len:
             continue
@@ -440,17 +441,17 @@
             #remove non-proper alignments
             if (seq_flag & 3) != 3:
                 continue
             # check pair num
             if (seq_flag & 1) == 1:
                 if (seq_flag & 64) == 64:
                     pair_num = 1
-                    paired = True
+                    paired   = True
                 elif (seq_flag & 128) == 128:
-                    paired = True
+                    paired   = True
                     pair_num = 2
                 else:
                     pair_num = 0
             else:
                 pair_num = 0
         algn_len, clipping_start, adjust_start, clipping_end, \
              adjust_end, align_blocks = \
@@ -466,18 +467,15 @@
             clipped_end = sequence_length - adjust_end
         percent_aligned = (clipped_end - clipped_start)/sequence_length
         #filter by align %
         if percent_aligned < percent or percent_aligned > max_per:
             continue
         in_window = within_window(leftmost_position, align_blocks, leftbound, rightbound, clipped_start)
         if in_window:
-                if algn_len == sequence_length:
-                    segment = False
-                else:
-                    segment = True
+                segment    = (algn_len != sequence_length)
                 #create sam object
                 sam_record = SAM(seq_name, leftmost_position, seq_flag,
                                      ref, segment, align_blocks, clipping_start,
                                      adjust_start, clipping_end, adjust_end, 
                                      percent_aligned, sequence_length, sam_flag.primary)
                 # add pair num info if paired
                 if paired:
@@ -501,39 +499,41 @@
     if num_alignments == 0:
         sys.exit(f"No matching records found within alignment file. Please check {align_map}.")
 
     #rescale?
         
     if num_alignments > limit:
         warning_color = "\033[93m"
-        end_color = "\033[0m"
+        end_color     = "\033[0m"
+
         if no_subsample == False: 
             msg = f"WARNING: {num_alignments} sequence alignments found. Randomly subsampling to --limit size of {limit}.\n" + \
-                "To turn off random subsampling, add --no_subsample to command"
+                    "To turn off random subsampling, add --no_subsample to command"
             alignments = dict(random.sample(alignments.items(), limit))
         else:
-            msg = f"WARNING: {num_alignments} sequence alignments found. Rescaling image dimensions..."
+            msg           = f"WARNING: {num_alignments} sequence alignments found. Rescaling image dimensions..."
             figure_height = limit
-            figure_width = limit
+            figure_width  = limit
+
         print(f"{warning_color}{msg}{end_color}")
 
     # add a map_num for each alignment
     for seq, algnments in alignments.items():
         for num, algn in enumerate(algnments):
             algn.map_num = f"{seq}-alignment-{num}"
 
     # returning only the seq lengths for seqs in alignments
-    seq_lengths = {seq: seq_lengths[seq] for seq in list(alignments.keys())}
+    seq_lengths     = {seq: seq_lengths[seq] for seq in list(alignments.keys())}
 
     # add ref
     seq_lengths[ref] = int(rightbound - leftbound)
     
     # print info
     num_rec = len(alignments)
-    ending = "record"
+    ending  = "record"
     if num_rec > 1:
         ending += 's'
 
     print(f"A total of {num_rec} alignment {ending} will be drawn")
     
     return alignments, figure_height, figure_width, seq_lengths
 
@@ -541,41 +541,38 @@
     """get the exons within the region based on the annotation coordinates"""
 
     print(f"Parsing {os.path.basename(annotation_file)}")
 
     fh = gzip.open(annotation_file, "rt") if annotation_file.endswith(".gz") else open(annotation_file, 'r')
 
     # CDS & exon records will be treated as exon records
-    genes_found = list()
-    num_genes = 0
-
-    exons = {}
-    gene_record = GeneRecord() # start off empty
-
-    # construct once
-    process_records = ["gene", "mRNA", "cds", "exon"]
+    genes_found     = list()
+    num_genes       = 0
+    exons           = {}
+    gene_record     = GeneRecord() # start off empty
+    process_records = ["gene", "mRNA", "cds", "exon"] # construct once
 
     for line in fh:
         if line[0] == '#':
             continue
         fields = line.strip('\n').split('\t')
         if fields[0] == chrom:
             record_type = fields[2].lower()
             if record_type in process_records:
                 if gene_record.update(record_type):
                     exons, genes_found = \
                         gene_record.incorporate(leftbound, rightbound, exons, genes_found)
                     num_genes = len(genes_found)
                 gene_record.parse_attributes(fields[8])
                 if record_type in ["cds", "exon"]:
-                    left = int(fields[3])
-                    right = int(fields[4])
+                    left      = int(fields[3])
+                    right     = int(fields[4])
                     direction = fields[6]
                     # may consider moving this step to the class
-                    num = num_genes % 6
+                    num        = num_genes % 6
                     gene_color = get_color(False, True, num)
                     # duplicates are not added
                     gene_record.add_exon(left, right, direction, gene_color, line)
             
     # get last bit
     if not gene_record.empty():
         exons, genes_found = gene_record.incorporate(leftbound, rightbound, exons, genes_found)
@@ -601,20 +598,20 @@
     for line in fh:
         fields = line.strip().split('\t')
         if fields[0] == ref:
             #0-based positions
             if leftbound <= int(fields[1]) <= rightbound or \
                 leftbound <= int(fields[2]) <= rightbound:
                 start_pos = int(fields[1])
-                end_pos = int(fields[2])
+                end_pos   = int(fields[2])
                 #just in case gap crosses boundaries                    
                 if start_pos <= leftbound:
                     start_pos = leftbound
                 if end_pos >= rightbound:
-                    end_pos = rightbound
+                    end_pos   = rightbound
                 gaps.append(GAP(start_pos, end_pos))
 
     fh.close()
 
     return gaps
 
 def parse_cigar(cigar: str, deletion_len: int):
@@ -626,58 +623,57 @@
                     'I': 0,
                     'S':0,
                     '=':0,
                     'X':0}
         return operators
 
     # deletions will shift sequences
-    align_blocks = algn_blocks()
-    block = []
-
-    current_cnt = ""
-    Op = [] #operators found for entire cigar
-    block_num = 0
+    align_blocks  = algn_blocks()
+    block         = []
+    current_cnt   = ''
+    Op            = [] #operators found for entire cigar
+    block_num     = 0
     estimated_len = 0
-    del_cnt = 0 # for total covered length
-    del_pos = {} # positions of deletions, needed to shift klumps
-    hclip_start = 0
-    hclip_end = 0
-    pos = 0
-    operators = create_op()
+    del_cnt       = 0 # for total covered length
+    del_pos       = {} # positions of deletions, needed to shift klumps
+    hclip_start   = 0
+    hclip_end     = 0
+    pos           = 0
+    operators     = create_op()
 
     for char in cigar:
         if char.isdigit():
             current_cnt += char
         elif char in operators:
-            pos += int(current_cnt)
+            pos             += int(current_cnt)
             operators[char] += int(current_cnt)
             Op.append(char)
             if char != 'I': # insertions do not consume ref
                 block.append(int(current_cnt))
-            current_cnt = ""
+            current_cnt = ''
         else:
-            current_cnt = int(current_cnt)
+            current_cnt       = int(current_cnt)
             if current_cnt >= deletion_len and char == 'D':
                 estimated_len += sum(list(operators.values()))
-                del_pos[pos] = current_cnt # document deletion pos
-                operators = create_op()
+                del_pos[pos]   = current_cnt # document deletion pos
+                operators      = create_op()
                 align_blocks.add_entry(block_num, block, current_cnt, del_cnt)
-                block_num += 1
-                block = []
-                del_cnt = 0
-                pos += int(current_cnt)
+                block_num     += 1
+                block          = []
+                del_cnt        = 0
+                pos           += int(current_cnt)
             elif char == 'D':
-                del_pos[pos] = current_cnt
-                del_cnt += current_cnt
-                pos += current_cnt
+                del_pos[pos]   = current_cnt
+                del_cnt       += current_cnt
+                pos           += current_cnt
             elif char == 'H':
                 if len(Op) == 0:
                     hclip_start = current_cnt
                 else:
-                    hclip_end = current_cnt
+                    hclip_end   = current_cnt
             Op.append(char)
             current_cnt = ""
     
     # last block
     estimated_len += sum(list(operators.values()))
     align_blocks.add_entry(block_num, block, 0, del_cnt)
     del current_cnt
@@ -754,15 +750,15 @@
     """return a dictionary where the key is the source and the value is the color"""
 
     fh = gzip.open(klump_colors, "rt") if klump_colors.endswith(".gz") else open(klump_colors, 'r')
 
     klump_colors = {}
 
     for line in fh:
-        fields = line.strip('\n').split('\t')
+        fields                  = line.strip('\n').split('\t')
         klump_colors[fields[0]] = get_color(False, False, 0, fields[1])
 
     fh.close()
 
     return klump_colors
 
 ########## analytical functions #############
@@ -773,58 +769,54 @@
     overlaps = defaultdict(dict)
 
     for seq_name, alignmnts in list(alignments.items()):
         mappings = {}
         for algn in alignmnts:
             algn_length = algn.aligned_length
             if len(mappings) == 0:
-                mappings[algn.map_num] = (
-                    algn.position, algn.position + algn_length)
+                mappings[algn.map_num]           = (algn.position, algn.position + algn_length)
                 overlaps[seq_name][algn.map_num] = False
             else:
                 for mapped, positions in list(mappings.items()):
                     # first scenario (position inside mapped region)
                     #        |------------|
                     #      |-----------|
                     if positions[0] <= algn.position <= positions[1]:
-                        overlaps[seq_name][mapped] = True
+                        overlaps[seq_name][mapped]       = True
                         overlaps[seq_name][algn.map_num] = True
-                        mappings[algn.map_num] = (
-                            algn.position, algn.position + algn_length)
+                        mappings[algn.map_num]           = (algn.position, algn.position + algn_length)
                     # second scenario (will catch only ones coming from the left)
                     #    |--------|
                     #      |-----------|
                     elif algn.position <= positions[0] <= algn.position + algn_length <= positions[1]:
-                        overlaps[seq_name][mapped] = True
+                        overlaps[seq_name][mapped]       = True
                         overlaps[seq_name][algn.map_num] = True
-                        mappings[algn.map_num] = (
-                            algn.position, algn.position + algn_length)
+                        mappings[algn.map_num]           = (algn.position, algn.position + algn_length)
                     # no overlap for the query
                     else:
                         overlaps[seq_name][algn.map_num] = False
-                        mappings[algn.map_num] = (
-                            algn.position, algn.position + algn_length)
+                        mappings[algn.map_num]           = (algn.position, algn.position + algn_length)
 
     return overlaps
 
 def estimate_seq_length(cigar: str):
     """Estimate seq length using cigar"""
 
-    operators = {'M', 'I', 'S', '=', 'X', 'H'}
-    current_cnt = ""
+    operators     = {'M', 'I', 'S', '=', 'X', 'H'}
+    current_cnt   = ''
     estimated_len = 0
 
     for char in cigar:
         if char.isdigit():
             current_cnt += char
         elif char in operators:
             estimated_len += int(current_cnt)
-            current_cnt = ""
+            current_cnt = ''
         else:
-            current_cnt = ""
+            current_cnt = ''
 
     return estimated_len
 
 def scale_image_width(alignments: dict, leftmost: int, rightbound: int):
     """determine width to contain all seqs"""
 
     rightmost = 0
@@ -854,42 +846,41 @@
 
     # the left most alignment will start 1% off the leftside of the img
     if seq_name in alignments:
         if leftmost_pos == position:
             return figure_width * 0.01
         else:
             # scale to leftmost
-            allocated_pos = image_width / image_area
+            allocated_pos     = image_width / image_area
             adjusted_position = position - leftmost_pos
-            adjusted_x = (figure_width * 0.01) + (allocated_pos*adjusted_position)
+            adjusted_x        = (figure_width * 0.01) + (allocated_pos*adjusted_position)
             return adjusted_x
     else:
         allocated_pos = image_width / image_area
-        adjusted_x = (figure_width * 0.01) + (allocated_pos*(leftbound - leftmost_pos))
+        adjusted_x    = (figure_width * 0.01) + (allocated_pos*(leftbound - leftmost_pos))
         return adjusted_x
 
 def create_seq_sizes(figure_height: int, num_seqs: int):
     """adjust seq sizes based on number of alignments and figure length"""
 
-    offset = figure_height * 0.01
-    top = figure_height * 0.99
-    ref_area = figure_height * 0.02 #proportion
+    offset       = figure_height * 0.01
+    top          = figure_height * 0.99
+    ref_area     = figure_height * 0.02 #proportion
     section_area = top - (figure_height * 0.1)
-    sections = section_area/num_seqs
-
-    bottom = figure_height * 0.905
+    sections     = section_area/num_seqs
+    bottom       = figure_height * 0.905
 
     return offset, ref_area, sections, bottom
 
 def set_up_plt(figure_height: float, alignments: dict, ref: str, leftbound: int, enumerating: bool):
     """set up plt height and y positions"""
     
-    y_positions = {} #y axis
-    positions = [] #for leftmost position (i.e., x axis)
-    leftmost_aligns = {} #leftmost for each seq
+    y_positions     = {} # y axis
+    positions       = [] # for leftmost position (i.e., x axis)
+    leftmost_aligns = {} # leftmost for each seq
 
     for seq, algns in alignments.items():
         for algn in algns: 
             if algn.clipping_start in ['S','H']:
                 position = algn.position - algn.adjust_start
             else:
                 position = algn.position
@@ -903,16 +894,15 @@
     leftmost_pos = min(positions)
 
     #if leftbound is left of leftmost seq
     if leftmost_pos > leftbound:
         leftmost_pos = leftbound
 
     #leftmost seq will be plotted at the top
-    sorted_algns = dict(sorted(leftmost_aligns.items(), key=lambda seq: seq[1]))
-
+    sorted_algns  = dict(sorted(leftmost_aligns.items(), key=lambda seq: seq[1]))
     reversed_seqs = list(sorted_algns.keys())[::-1]
 
     #if enumerating
     if enumerating:
         enumeration_dict = {seq: i for i, seq in enumerate(list(sorted_algns.keys()))}
     else:
         enumeration_dict = None
@@ -923,32 +913,35 @@
         = create_seq_sizes(figure_height, num_seqs)
     
     #check to avoid plotting sequences too wide for current plotting method
     if sections >= ref_area:
         print(f"The number of alignments ({num_seqs}) may not look well for the figure.")
         print("Adjusting...")
         adjusted_length = (figure_height - (2*offset))
-        original_len = figure_height + 0
-        original_ref = ref_area + 0
+        original_len    = figure_height + 0
+        original_ref    = ref_area + 0
         adjusted_length = original_len - (2*offset)
-        figure_height = original_ref
+        figure_height   = original_ref
+        
         for _ in range(num_seqs):
             figure_height += sections
         offset, ref_area, sections, bottom \
             = create_seq_sizes(figure_height, num_seqs)
+        
         if original_ref >= 3 * ref_area:
-            original_ref = original_ref * 0.5
+            original_ref      = original_ref * 0.5
             bottom_adjustment = 0.25
-            len_adjustment = 0.9
+            len_adjustment    = 0.9
         else:
             bottom_adjustment = 0.15
-            len_adjustment = 0.925
-        ref_area = original_ref
-        sections = ref_area - (ref_area * (0.01 * num_seqs))
-        bottom = figure_height - (figure_height * bottom_adjustment)
+            len_adjustment    = 0.925
+
+        ref_area        = original_ref
+        sections        = ref_area - (ref_area * (0.01 * num_seqs))
+        bottom          = figure_height - (figure_height * bottom_adjustment)
         adjusted_length = figure_height * len_adjustment
  
     else:
         adjusted_length = (figure_height - (2*offset))
 
     #order going from bottom to top
     for i, seq in enumerate(reversed_seqs):
@@ -980,15 +973,15 @@
     with open(f"Results_{record_nt}_records_{ref}_{leftbound}-{rightbound}.tsv", 'w') as out:
         out.write(header + '\n')
         for seq_id in seqs:
             seq_len = seq_lengths[seq_id]
             seq_alignments = alignments[seq_id]
             for algn in seq_alignments:
                 percentage = round(algn.percent_aligned * 100, 2)
-                outLine = f"{seq_id}\t{seq_len}\t{algn.chromosome}\t{algn.flag}\t{algn.position}\t{percentage}\t{algn.clipping_start}\t{algn.clipping_end}"
+                outLine    = f"{seq_id}\t{seq_len}\t{algn.chromosome}\t{algn.flag}\t{algn.position}\t{percentage}\t{algn.clipping_start}\t{algn.clipping_end}"
                 if enumerating:
                     outLine += f"\t{enumeration_dict[seq_id]}"
                 if grouping:
                     outLine += f"\t{algn.group_num}"
                 out.write(outLine + '\n')
 
 def get_color(list_colors: bool, grouping: bool, group_num: int, color = "blue"):
@@ -1029,16 +1022,16 @@
             options = ",".join([opt for opt in colors.keys()])
             sys.exit(f"{color} currently not available. Current options are: {options}")
         else:
             colr = colors[color]
             return Feature_Color(colr[0], colr[1], colr[2], 1, color)
     else:
         colors_list = list(colors.keys())
-        color = colors_list[group_num]
-        colr = colors[color]
+        color       = colors_list[group_num]
+        colr        = colors[color]
         return Feature_Color(colr[0], colr[1], colr[2], 1.0, color)
 
 def algn_color(flag: str):
     """determine the color of the sequence"""
 
     samflag = int(flag)
 
@@ -1057,30 +1050,26 @@
       
     return seq_color
 
 def adjust_rightbound(ref: str, rightbound: int, alignment_map: str):
     """if rightbound is beyond length of reference, adjust rightbound"""
 
     # just another check to verify that the ref is indeed in the aligment map
-    ref_found = False
-
-    cmd = f"samtools view -H {alignment_map}"
-    fh = os.popen(cmd, 'r')
-
-    ref_field = f"SN:{ref}"
-
-    # convert to int
-    rightbound = int(rightbound)
+    ref_found  = False
+    cmd        = f"samtools view -H {alignment_map}"
+    fh         = os.popen(cmd, 'r')
+    ref_field  = f"SN:{ref}"
+    rightbound = int(rightbound) # convert from float to int
 
     for line in fh:
         if line.startswith("@SQ"):
             fields = line.strip('\n').split('\t')
             if fields[1] == ref_field:
                 ref_found = True
-                ref_len = int(fields[2].split(':')[1])
+                ref_len   = int(fields[2].split(':')[1])
                 if rightbound > ref_len:
                     print(f"Rightbound exceeds {ref}'s length. Setting rightbound to the end of {ref}")
                     rightbound = ref_len
                 break
     
     fh.close()
 
@@ -1101,22 +1090,22 @@
     if clip_start != None:
         block_start = clip_start
     else:
         block_start = 0
 
     # objects to check logic of loop
     klump_start_set = False
-    klump_end_set = False
-    klumps_list = []
-    added_len = 0
+    klump_end_set   = False
+    klumps_list     = []
+    added_len       = 0
 
     # get in case of a split & reversing
     # adding 0 to avoid using copy module
     k_start = klump_start + 0.0
-    k_end = klump_end + 0.0
+    k_end   = klump_end + 0.0
 
     # add mini deletions to positions
     for pos, dlen in del_pos.items():
         if pos <= k_start and dlen < deletion_len:
             klump_start += dlen
         if pos <= k_end and dlen < deletion_len:
             klump_end += dlen
@@ -1124,63 +1113,62 @@
     # stop once we shifted over to the new positions
     for block, block_len in align_blocks.items():
         block_len = align_blocks[block]
         block_end = block_start + block_len
         if block_start <= klump_start <= block_end:
             klump_start_set = True
         if block_start <= klump_end <= block_end:
-            klump_end_set = True
+            klump_end_set   = True
         if klump_start_set:
             if klump_end_set:
                 if block_start <= klump_start <= klump_end <= block_end:
                     klumps_list.append([klump_start, klump_end])
                     return klumps_list
             elif block_start <= klump_start <= block_end:
                 klumps_list.append([klump_start, block_end])
                 added_len += (block_end - klump_start)
             elif klump_start < block_start:
                 klumps_list.append([block_start, block_end])
                 added_len += (block_end - block_start)
         if klump_end_set:
             klumps_list.append([block_start, klump_end - added_len])
         deletion_len = block_del[block]
-        block_start = block_end + deletion_len
+        block_start  = block_end + deletion_len
         if not klump_start_set:
             klump_start += deletion_len
         if not klump_end_set:
             klump_end += deletion_len
 
     return klumps_list
 
 def find_overlap_labels(labels_list: list):
     """find overlapping labels based on their dimensions"""
 
     # each sub list will be an overlapping group
     overlaps_group = [[]]
-
-    first = True
-    prev_start = None
-    prev_end = None
+    first          = True
+    prev_start     = None
+    prev_end       = None
 
     for label_arr in labels_list:
         start = label_arr[0]
-        end = label_arr[1]
+        end   = label_arr[1]
         if first:
             first = False
             overlaps_group[0].append(label_arr)
         else:
             if (prev_start <= start <= prev_end) or \
                 (prev_start <= end <= prev_end):
                 # add to current subgroup
                 overlaps_group[-1].append(label_arr)
             else:
                 # new subgroup
                 overlaps_group.append([label_arr])
         prev_start = start
-        prev_end = end
+        prev_end   = end
 
     return overlaps_group
 
 def find_coordinates(x1: float, y1: float, width: float, height: float, direction: str):
     """given the position where the label will be drawn, return the coordinates of each corner"""
 
     # first, we need to get the first two points
@@ -1204,16 +1192,16 @@
     if direction == 'F':
         rad = math.radians(45)
     elif direction == 'R':
         rad = math.radians(-45)
 
     cos_angle = math.cos(rad)
     sin_angle = math.sin(rad)
-    center_x = x1 + (width * 0.5 * cos_angle)   
-    center_y = y1 - (width * 0.5 * sin_angle)
+    center_x  = x1 + (width * 0.5 * cos_angle)   
+    center_y  = y1 - (width * 0.5 * sin_angle)
 
     # get corners
     # x1 = center_x + (height / 2) * cos_angle - (width / 2) * sin_angle
     # y1 = center_y + (height / 2) * sin_angle + (width / 2) * cos_angle
 
     x2 = center_x - (height / 2) * cos_angle - (width / 2) * sin_angle
     y2 = center_y - (height / 2) * sin_angle + (width / 2) * cos_angle
@@ -1240,15 +1228,15 @@
     # helper functions to project points onto the axes
     # MDP = Make Dot Product
     def MDP(corner1: tuple, corner2: tuple):
         return (corner1[0] * corner2[0]) + (corner1[1] * corner2[1])
     
     # coords will contain all cordinates of the rectange in a single tuple
     def project_rect(axis: tuple, label_pos: Label_Position):
-        t = label_pos.make_tuple() # get tuple
+        t      = label_pos.make_tuple() # get tuple
         min_pt = min(MDP(t[0], axis), MDP(t[1], axis), MDP(t[2], axis), MDP(t[3], axis))
         max_pt = max(MDP(t[0], axis), MDP(t[1], axis), MDP(t[2], axis), MDP(t[3], axis))
         return (min_pt, max_pt)
     
     # create the axes
     label1_tup = label1_pos.make_tuple()
     label2_tup = label2_pos.make_tuple()
@@ -1269,35 +1257,35 @@
 
 def adjust_klump_labels(klump_labels: dict, exon_positions: list, direction: str):
     """shift the klump labels to avoid overlap with exon lables"""
 
     adjusted_positions = {} # {label : (label_position, width, height)}
 
     for klump_name, label_dim in klump_labels.items():
-        x_start = label_dim[0]
-        label_width = label_dim[1]
-        y_start = label_dim[2]
+        x_start      = label_dim[0]
+        label_width  = label_dim[1]
+        y_start      = label_dim[2]
         label_height = label_dim[3]
-        label = label_dim[4]
-        label_pos = find_coordinates(x_start, y_start, label_width, label_height, direction)
+        label        = label_dim[4]
+        label_pos    = find_coordinates(x_start, y_start, label_width, label_height, direction)
         # make sure it has not move onto other adjusted labels
         for label2_tuple in adjusted_positions.values():
             label2_pos = label2_tuple[0]
             while (overlapping_labels(label_pos, label2_pos)):
                 label_pos.shift_right(1) # shift 1 pixel to the right
         # if the label was shifted, we need to move it above any overlapping
         # exon labels
         for exon_loc in exon_positions:
             # x -> start, end
             # y -> bottom, top
-            exon_start = exon_loc[0]
-            exon_end = exon_loc[1]
+            exon_start  = exon_loc[0]
+            exon_end    = exon_loc[1]
             exon_bottom = exon_loc[2]
-            exon_top = exon_loc[3]
-            exon_pos = Label_Position(exon_start, exon_bottom, exon_end, exon_bottom,
+            exon_top    = exon_loc[3]
+            exon_pos    = Label_Position(exon_start, exon_bottom, exon_end, exon_bottom,
                                       exon_end, exon_top, exon_start, exon_top)
             if overlapping_labels(label_pos, exon_pos):
                 if direction == 'F':
                     if exon_top < exon_bottom:
                         y_start = exon_top - 2
                     else:   
                         y_start = exon_bottom - 2
@@ -1316,119 +1304,118 @@
 ########## plotting functions #############
 
 def plot_seq(cairo_context, alignment: SAM, allocated_positions: float, seq_height: float,
               x_pos: float, overlap: bool, ref: str, leftbound: int, rightbound: int, section: float):
     """ plot sequence to scale to the longest sequence"""
 
     #get params
-    align_blocks = alignment.align_blocks.blocks
-    block_del = alignment.align_blocks.block_del
-    covered_len = alignment.align_blocks.covered_len
-    ending_blocks = alignment.align_blocks.get_ending_blocks()
-    seq_id = alignment.seq_name
+    align_blocks   = alignment.align_blocks.blocks
+    block_del      = alignment.align_blocks.block_del
+    covered_len    = alignment.align_blocks.covered_len
+    ending_blocks  = alignment.align_blocks.get_ending_blocks()
+    seq_id         = alignment.seq_name
     clipping_start = alignment.clipping_start
-    adjust_start = alignment.adjust_start
-    clipping_end = alignment.clipping_end
-    adjust_end = alignment.adjust_end
-    seq_color = alignment.seq_color
+    adjust_start   = alignment.adjust_start
+    clipping_end   = alignment.clipping_end
+    adjust_end     = alignment.adjust_end
+    seq_color      = alignment.seq_color
 
     # for clipping
-    clipping_colors = {'S': [0,1,0], #green
-                           'H': [1,0,0], #red
-                           None: [0,0,0]} #black
+    clipping_colors = {'S':   [0,1,0], #green
+                       'H':   [1,0,0], #red
+                        None: [0,0,0]} #black
+    
     if len(ending_blocks) == 1:
         first_block = ending_blocks[0]
-        last_block = first_block
+        last_block  = first_block
     else:
         first_block = ending_blocks[0]
-        last_block = ending_blocks[1]
+        last_block  = ending_blocks[1]
 
     # make adjustments 0
     if adjust_start == None:
         adjust_start = 0
     if adjust_end == None:
-        adjust_end = 0
+        adjust_end   = 0
 
     # starting positions
     x1 = x_pos  # offset from left by x position
     y1 = seq_height  # y / vertical offset
     y2 = y1
     x2 = x_pos + (allocated_positions * covered_len)
     
     #check for clipping
     if clipping_start != None:
         clip_color = clipping_colors[clipping_start]
         clip_color.append(seq_color.alpha)
-        clip_x_s = x_pos + (allocated_positions * adjust_start) # go right after clip
+        clip_x_s   = x_pos + (allocated_positions * adjust_start) # go right after clip
         draw_borders(cairo_context, x_pos, clip_x_s, y1, clip_color, section)
     if clipping_end != None:
         clip_color = clipping_colors[clipping_end] 
         clip_color.append(seq_color.alpha)
-        clip_x_e = x2 - (allocated_positions * adjust_end) # go left of clip
+        clip_x_e   = x2 - (allocated_positions * adjust_end) # go left of clip
         draw_borders(cairo_context, x2, clip_x_e, y1, clip_color, section)
         x2 = clip_x_e # replace to new end
 
     # draw the actual aligned portions & gaps
     for block, block_len in align_blocks.items():
         if clipping_start == None and clipping_end == None and len(align_blocks) == 1:
              # determine new x
             adjusted_start = x1
-            adjusted_end = x2
+            adjusted_end   = x2
         else:
             if block == first_block:
                 adjusted_start = x_pos + (allocated_positions * adjust_start)
-                adjusted_end = adjusted_start + (allocated_positions * block_len)
+                adjusted_end   = adjusted_start + (allocated_positions * block_len)
             elif block == last_block:
                 adjusted_end = x2
             else:
                 adjusted_end = adjusted_start + (allocated_positions * block_len)
        
         # if forward: grey else orangy-yellow, if overlapping, alpha 0.5 else 1
         if overlap:
             seq_color.alpha = 0.5
         if seq_id == ref:
             section = section * 1.25
 
         adjusted_height = section * 0.45
-        top = y1 - adjusted_height
-        bottom = y1 + adjusted_height
+        top             = y1 - adjusted_height
+        bottom          = y1 + adjusted_height
         cairo_context.move_to(adjusted_start, bottom) 
         cairo_context.line_to(adjusted_end, bottom)
         cairo_context.line_to(adjusted_end, top)
         cairo_context.line_to(adjusted_start, top)
         cairo_context.close_path()
         cairo_context.set_source_rgba(seq_color.red, seq_color.green, seq_color.blue, seq_color.alpha)
         cairo_context.fill_preserve()
         cairo_context.set_source_rgb(0, 0, 0)
         cairo_context.set_line_width((section * 0.05))
         cairo_context.stroke()
         
         # for plotting the deletions
         if block != last_block:
             del_start = adjusted_end
-            del_end = del_start + (allocated_positions * block_del[block])
+            del_end   = del_start + (allocated_positions * block_del[block])
             cairo_context.move_to(del_start, y1)
             cairo_context.line_to(del_end, y2)
             cairo_context.set_line_width(section * 0.25)
             cairo_context.set_source_rgba(0, 0, 0, seq_color.alpha) #black
             cairo_context.stroke()
             adjusted_start = del_end
 
     # add sequence name if not written
     if seq_id == ref:
         x, y = 50, seq_height - (seq_height * 0.05)
 
         cairo_context.set_source_rgb(0, 0, 0)
         cairo_context.set_font_size(0.75 * section) #used to be 75
-        cairo_context.select_font_face(
-            "Arial", cairo.FONT_SLANT_NORMAL, cairo.FONT_WEIGHT_NORMAL
-        )
+        cairo_context.select_font_face("Arial", cairo.FONT_SLANT_NORMAL, cairo.FONT_WEIGHT_NORMAL)
         cairo_context.move_to(x, y)
-        left = "{:,}".format(leftbound)
-        right = "{:,}".format(rightbound)
+        left   = "{:,}".format(leftbound)
+        right  = "{:,}".format(rightbound)
         seq_id = f"{seq_id}: {left}-{right}"
         cairo_context.show_text(seq_id)
         cairo_context.stroke()
         return top, bottom
     else:
         return -1, -1
 
@@ -1445,43 +1432,43 @@
     cairo_context.set_line_width((section * 0.05))
     cairo_context.stroke()
 
 def create_ticks(seq_length: int):
     """Find the appropriate marker lengths for tick marks"""
 
     marker_sets = {
-        1e3: ["bp", 100],
-        5e3: ["K", 1000],
+        1e3:   ["bp", 100],
+        5e3:   ["K", 1000],
         7.5e3: ["K", 1500],
-        1e4: ["K", 2000],
+        1e4:   ["K", 2000],
         2.5e4: ["K", 5000],
-        5e4: ["K", 10000],
-        9e4: ["K", 15000],
-        1e5: ["K", 20000],
-        5e5: ["K", 25000],
-        9e5: ["K", 30000],
-        1e6: ["M", 50000],
-        5e6: ["M", 70000],
-        9e6: ["M", 100000],
-        1e7: ["M", 150000],
-        3e7: ["M", 200000],
-        5e7: ["M", 500000],
-        7e7: ["M", 700000],
-        9e7: ["M", 900000],
-        1e8: ["M", 1000000],
-        5e8: ["M", 1500000],
-        9e8: ["M", 3000000],
-        1e9: ["M", 5000000],
+        5e4:   ["K", 10000],
+        9e4:   ["K", 15000],
+        1e5:   ["K", 20000],
+        5e5:   ["K", 25000],
+        9e5:   ["K", 30000],
+        1e6:   ["M", 50000],
+        5e6:   ["M", 70000],
+        9e6:   ["M", 100000],
+        1e7:   ["M", 150000],
+        3e7:   ["M", 200000],
+        5e7:   ["M", 500000],
+        7e7:   ["M", 700000],
+        9e7:   ["M", 900000],
+        1e8:   ["M", 1000000],
+        5e8:   ["M", 1500000],
+        9e8:   ["M", 3000000],
+        1e9:   ["M", 5000000],
               }
 
     multiplier = None
 
     for marker_length in marker_sets.keys():
         if seq_length <= marker_length:
-            fields = marker_sets[marker_length]
+            fields     = marker_sets[marker_length]
             multiplier = fields[1]
             break
 
     # multiplier will be used to show increments in bp length
     if multiplier != None:
         tick_ct = math.floor(seq_length/multiplier)
     else:
@@ -1514,21 +1501,21 @@
             marker = "bp"
         elif 1e3 <= marker_num < 1e6:
             marker_num = marker_num/1e3
             marker = "K"
         elif marker_num >= 1e6:
             marker_num = marker_num/1e6
             marker = "M" 
-        marker_num = round(marker_num, 2)
+        marker_num   = round(marker_num, 2)
         marker_label = f"{marker_num}{marker}"
-        marker_pos = x_pos + (allocated_pos * i)
+        marker_pos   = x_pos + (allocated_pos * i)
          # marker labels
         cairo_context.set_source_rgba(0, 0, 0, 1)
         cairo_context.set_font_size((section * 0.40))
-        e = cairo_context.text_extents(marker_label)
+        e          = cairo_context.text_extents(marker_label)
         label_xpos = marker_pos - (e.width / 2) # put it half way
         cairo_context.move_to(label_xpos, label_ypos) 
         cairo_context.show_text(marker_label)
         cairo_context.stroke()
         # now draw tick up to the top of the text
         top = label_ypos - e.height
         cairo_context.move_to(marker_pos, mark_ypos1)
@@ -1565,36 +1552,36 @@
                 rightbound: int, section: float, klmp_color: Feature_Color, klump_colors: dict, 
                 deletion_len: int, color_by_gene: bool, top_positions: list, bottom_positions: list,
                 chrom_top_pos: float, chrom_bottom_pos: float, ylabel_pos: float, plt_height=None):
     """plot the klumps"""
 
     # fill in instead of making "klump"
 
-    seq_name = alignment.seq_name
-    align_blocks = alignment.align_blocks.blocks
-    del_pos = alignment.align_blocks.del_pos
-    covered_len = alignment.align_blocks.covered_len
-    block_del = alignment.align_blocks.block_del
-    flag = alignment.flag
+    seq_name       = alignment.seq_name
+    align_blocks   = alignment.align_blocks.blocks
+    del_pos        = alignment.align_blocks.del_pos
+    covered_len    = alignment.align_blocks.covered_len
+    block_del      = alignment.align_blocks.block_del
+    flag           = alignment.flag
     clipping_start = alignment.clipping_start
-    adjust_start = alignment.adjust_start
-    clipping_end = alignment.clipping_end
-    adjust_end = alignment.adjust_end
-    seq_len = alignment.seq_len
+    adjust_start   = alignment.adjust_start
+    clipping_end   = alignment.clipping_end
+    adjust_end     = alignment.adjust_end
+    seq_len        = alignment.seq_len
 
     # labels will alternate
     directions = ['F', 'R']
-    i = 0
+    i          = 0
 
     # will store x positions after drawing to
     # be the starting positions for the labels
     # before adjusting
-    top_labels = {}
+    top_labels    = {}
     bottom_labels = {}
-    midpoint_pos = {} # store klump midpoint & klump color to connect line to label
+    midpoint_pos  = {} # store klump midpoint & klump color to connect line to label
 
     #remove tag if briding image
     for klump in seq_klumps[seq_name]:
         if klump.query_source == "None":
             continue
         # check if setting color to a new param
         if klump_colors != None:
@@ -1607,26 +1594,26 @@
         if klump.pair_info:
             #check that klumps are with correct sequence
             if klump.pair_num != alignment.pair_num:
                     continue     
         #to avoid plotting klumps not in region of interest
         if seq_name != ref:
             if clipping_start == None:
-                left_pos = 0
+                left_pos     = 0
                 adjust_start = 0 # used when adjusting to x pos
             else:
                 left_pos = adjust_start
             if clipping_end == None:
                 right_pos = covered_len
             else:
                 right_pos = covered_len - adjust_end
             # reverse klumps
             if (flag & 16) == 16:
                 klump.start_pos = seq_len - klump.start_pos
-                klump.end_pos = seq_len - klump.end_pos
+                klump.end_pos   = seq_len - klump.end_pos
                 # the end is now the start, and the start is now the end
                 klump.start_pos, klump.end_pos = klump.end_pos, klump.start_pos
             # if out of range
             if left_pos <= klump.start_pos <= right_pos:
                 if left_pos <= klump.end_pos <= right_pos:
                     pass
                 else:
@@ -1634,26 +1621,26 @@
             else:
                 continue
             klumps_list = \
                 adjust_klumps(adjust_start, klump.start_pos, klump.end_pos, 
                                 align_blocks, block_del, del_pos, deletion_len)
             for klumps in klumps_list:
                 klmp_start = klumps[0] 
-                klmp_end = klumps[1]
+                klmp_end   = klumps[1]
                 # re-check if out of range after klumps are adjusted
                 if left_pos <= klmp_start <= right_pos:
                     if left_pos <= klmp_end <= right_pos:
                         pass
                     else:
                         continue
                 else:
                     continue
                 if clipping_start == 'H':
                     klmp_start = klmp_start - adjust_start
-                    klmp_end = klmp_end - adjust_start
+                    klmp_end   = klmp_end - adjust_start
                 # make height of seq
                 fill_height = section * 0.425
                 # added to fig
                 _ = fill_in_matches(cairo_context, y_coordinate, x_pos,
                             allocated_positions, klmp_start, klmp_end,
                             overlap, fill_height, klmp_color)
 
@@ -1665,176 +1652,181 @@
                 else:
                     continue
             else:
                 continue       
             #adjust by shifting leftbound             
             if (flag & 16) == 16:
                 start_pos = (covered_len - klump.start_pos) - leftbound
-                end_pos = (covered_len - klump.end_pos) - leftbound
+                end_pos   = (covered_len - klump.end_pos) - leftbound
             else:
                 start_pos = klump.start_pos - leftbound
-                end_pos = klump.end_pos - leftbound
+                end_pos   = klump.end_pos - leftbound
             fill_height = section * 0.5315 # color up to borders
         # not a split klump
             k_midpoint = fill_in_matches(cairo_context, y_coordinate, x_pos,
                             allocated_positions, start_pos, end_pos,
                             overlap, fill_height, klmp_color)
             #check if vertical line for klumps
             if plt_height != None:
                 if start_pos > end_pos:
                     vertical_start, vertical_end = end_pos, start_pos
                 else:
                     vertical_start, vertical_end = start_pos, end_pos
                 #make adjustments
                 vertical_start = x_pos + (vertical_start * allocated_positions)
-                vertical_end =  x_pos + (vertical_end * allocated_positions)
+                vertical_end   =  x_pos + (vertical_end * allocated_positions)
                 draw_vertical_line(cairo_context, vertical_start, vertical_end,
                                     y_coordinate, plt_height, klmp_color, fill_height)
             # set the dimensions prior to adjusting positions
             cairo_context.select_font_face("Arial", cairo.FONT_SLANT_NORMAL, cairo.FONT_WEIGHT_NORMAL)
             cairo_context.set_source_rgb(0, 0, 0)  # black
             cairo_context.set_font_size((section * 0.20))
             # create label
             klump_size = klump.klump_size
-            query = klump.query_source
-            label = f"{klump_size}-{query}"
-            label_dim = cairo_context.text_extents(label)
+            query      = klump.query_source
+            label      = f"{klump_size}-{query}"
+            label_dim  = cairo_context.text_extents(label)
             # get the mid point of the text if i were not rotated
-            start_pos = x_pos + (start_pos * allocated_positions)
-            end_pos = x_pos + (end_pos * allocated_positions)
+            start_pos      = x_pos + (start_pos * allocated_positions)
+            end_pos        = x_pos + (end_pos * allocated_positions)
             klump_midpoint = (end_pos + start_pos) / 2
-            direction = directions[i % 2]
+            direction      = directions[i % 2]
             i += 1
             if direction == 'F':
                 y_pos = chrom_top_pos - 2
                 # y_pos = yLabel - (section * 0.75)
                 top_labels[klump.klump_name] = (klump_midpoint, label_dim.width, y_pos, label_dim.height, label)
             elif direction == 'R':
                 y_pos = ylabel_pos + 2
                 # y_pos = yLabel + (section * 0.75)
                 bottom_labels[klump.klump_name] = (klump_midpoint, label_dim.width, y_pos, label_dim.height, label)
             midpoint_pos[klump.klump_name] = (k_midpoint, klmp_color) # store the midpoint for later
       
     # if ref, we may plot labels
     if seq_name == ref:
         # adjust the labels to prevent overlaps
-        adjusted_tops = adjust_klump_labels(top_labels, top_positions, 'F')
+        adjusted_tops    = adjust_klump_labels(top_labels, top_positions, 'F')
         adjusted_bottoms = adjust_klump_labels(bottom_labels, bottom_positions, 'R')
  
         # now to plot the labels and the lines
         # if they are empty, no elements will be returned
 
         for klump_name, label_dim in adjusted_tops.items():
-            x1, y1 = label_dim[0].x1, label_dim[0].y1
-            label = label_dim[3]
+            x1, y1                 = label_dim[0].x1, label_dim[0].y1
+            label                  = label_dim[3]
             k_midpoint, klmp_color = midpoint_pos[klump_name]
             plot_label(cairo_context, x1, y1, math.radians(-45), label, k_midpoint, chrom_top_pos, klmp_color)
+        
         for klump_name, label_dim in adjusted_bottoms.items():
-            x1, y1 = label_dim[0].x1, label_dim[0].y1
-            label = label_dim[3]
+            x1, y1                 = label_dim[0].x1, label_dim[0].y1
+            label                  = label_dim[3]
             k_midpoint, klmp_color = midpoint_pos[klump_name]
             plot_label(cairo_context, x1, y1, math.radians(45), label, k_midpoint, chrom_bottom_pos, klmp_color)
             
 
 def plot_exons(cairo_context, y_coordinate: float, exons: dict, allocated_positions: float,
                chrom_top: float, chrom_bottom: float, x_pos: float, leftbound: int, section: float, 
                ylabel_pos: float, plot_height: float, pdf_height: float):
     """plot the exons onto the reference"""
 
     # will be used to avoid plotting the same gene twice
-    current_gene = None
-    prev_color = None # as a safety measure
-    label_height = -float("inf")
+    current_gene  = None
+    prev_color    = None # as a safety measure
+    label_height  = -float("inf")
     bottom_labels = [] # will be used to know where labels start/end
-    top_labels = []
-    i = 0 # used to assign direction
-    directions = ['+', '-']
+    top_labels    = []
+    i             = 0 # used to assign direction
+    directions    = ['+', '-']
 
     cairo_context.select_font_face("Arial", cairo.FONT_SLANT_NORMAL,
                                    cairo.FONT_WEIGHT_NORMAL)
     cairo_context.set_font_size((section * 0.25))
 
     # sort exons
     exons = dict(sorted(exons.items(), key = lambda exon: exon[1].start_pos))
 
     # plot ONLY the annotations onto the chrom
     for exon in exons.values():
         #adjust by shifting
         start_pos = exon.start_pos - leftbound
-        end_pos = exon.end_pos - leftbound
+        end_pos   = exon.end_pos - leftbound
         # direction = exon.direction
         fill_in_annotation(cairo_context, y_coordinate, x_pos,
-                        allocated_positions, start_pos, end_pos,
-                         section, "exon", None, exon.gene_color)
+                           allocated_positions, start_pos, end_pos,
+                           section, "exon", None, exon.gene_color)
         
         # check for vertical lines
         if plot_height != None:
             fill_height = section * 0.515
-            start = x_pos + (start_pos * allocated_positions)
-            end = x_pos + (end_pos * allocated_positions)
+            start       = x_pos + (start_pos * allocated_positions)
+            end         = x_pos + (end_pos * allocated_positions)
             draw_vertical_line(cairo_context, start, end, y_coordinate, plot_height, exon.gene_color, fill_height)
 
         # plot label based on direction
         if (current_gene != exon.gene_name) and (prev_color != exon.gene_color.name):
             current_gene = exon.gene_name
-            prev_color = exon.gene_color.name
+            prev_color   = exon.gene_color.name
         else:
             continue
-        t_dim = cairo_context.text_extents(current_gene)   
+
+        t_dim        = cairo_context.text_extents(current_gene)   
         label_height = max(label_height, t_dim.height)
-        direction = directions[i % 2]
+        direction    = directions[i % 2]
+
         if direction == '-':
             start = x_pos + (start_pos * allocated_positions) # dash at start of label
-            end = start + t_dim.width
+            end   = start + t_dim.width
             bottom_labels.append([start, end, exon.gene_name, exon.gene_color])
         elif direction == '+':
-            end = x_pos + (start_pos * allocated_positions) # dash at end of label
+            end   = x_pos + (start_pos * allocated_positions) # dash at end of label
             start = end - t_dim.width
             top_labels.append([start, end, exon.gene_name, exon.gene_color])
         i += 1
 
     # now to find the overlapping text
     overlap_groups_bottom = find_overlap_labels(bottom_labels)
-    overlap_groups_top = find_overlap_labels(top_labels)
+    overlap_groups_top    = find_overlap_labels(top_labels)
 
     # used for klump labels
-    top_positions = []
+    top_positions    = []
     bottom_positions = []
 
     # now to draw the labels
 
     for i, labels_list in enumerate([overlap_groups_top, overlap_groups_bottom]):
         direction = directions[i]
         for label_sub_list in labels_list:
             if direction == '-':
                 ybottom = ylabel_pos # + t_dim.height + 2
                 label_sub_list.reverse() # only reverse if drawing on bottom
             elif direction == '+':
                 ybottom = chrom_top - 1
             for j, sub_list in enumerate(label_sub_list, start = 1):
                 x_position = sub_list[0] # will shift to prevent dash line overlap
+                
                 if direction == '+':
-                    y_position = ybottom - (label_height * j)
-                    top_y = y_position
-                    bottom_y = chrom_top - 1
+                    y_position  = ybottom - (label_height * j)
+                    top_y       = y_position
+                    bottom_y    = chrom_top - 1
                     x_position -= 1
-                    dash_xpos = sub_list[1]
+                    dash_xpos   = sub_list[1]
                 elif direction == '-':
-                    y_position = ybottom + (label_height * j)
-                    top_y = chrom_bottom + ((section * 0.025))
-                    bottom_y = y_position - label_height + ((section * 0.05))
+                    y_position  = ybottom + (label_height * j)
+                    top_y       = chrom_bottom + ((section * 0.025))
+                    bottom_y    = y_position - label_height + ((section * 0.05))
                     x_position += 1
-                    dash_xpos = sub_list[0]
+                    dash_xpos   = sub_list[0]
+
                 label = sub_list[2]
                 cairo_context.move_to(x_position, y_position)
                 cairo_context.set_source_rgb(0, 0, 0)
                 cairo_context.show_text(label)
                 cairo_context.stroke()
-                label_dim = cairo_context.text_extents(label)
-                x_end = x_position + label_dim.width
+                label_dim   = cairo_context.text_extents(label)
+                x_end       = x_position + label_dim.width
                 y_top_label = y_position - label_dim.height
                 if direction == '+':
                     top_positions.append((x_position, x_end, y_position, y_top_label))
                 elif direction == '-':
                     bottom_positions.append((x_position, x_end, y_position, y_top_label))
                 # now for the line
                 # print(direction, top_y, bottom_y, y_position - label_height)
@@ -1853,18 +1845,18 @@
     """plot the genes onto the reference"""
 
     # fill in where the gaps are located
 
     for gap in gaps:
         #adjust by shifting leftbound
         start_pos = gap.start_pos - leftbound
-        end_pos = gap.end_pos - leftbound
+        end_pos   = gap.end_pos - leftbound
         fill_in_annotation(cairo_context, y_coordinate, x_pos,
-                        allocated_positions, start_pos, end_pos,
-                         section, "gap", plt_height)
+                           allocated_positions, start_pos, end_pos,
+                            section, "gap", plt_height)
 
 def fill_in_matches(cairo_context, y: float, x_pos: float, allocated_pos: float, 
                     klump_start: float, klump_end: float, overlap: bool, \
                     fill_height: float, klmp_color: Feature_Color):
     """fill in seq with klump positions"""
 
     # checking for overlap (default is alpha = 1)
@@ -1872,15 +1864,15 @@
         klmp_color.alpha = 0.5
     # in case of reverse aligned
     if klump_start > klump_end:
         klump_start, klump_end = klump_end, klump_start
 
     #make adjustments
     klump_start = x_pos + (klump_start * allocated_pos)
-    klump_end =  x_pos + (klump_end * allocated_pos)
+    klump_end   = x_pos + (klump_end * allocated_pos)
 
     #plot
     cairo_context.move_to(klump_start, y - fill_height)
     cairo_context.line_to(klump_end, y - fill_height)
     cairo_context.line_to(klump_end, y + fill_height)
     cairo_context.line_to(klump_start, y + fill_height)
     cairo_context.close_path()
@@ -1901,15 +1893,15 @@
     elif an_type == "gap":
         color = Feature_Color(0,0,0,0.5)
     #fill height
     fhght = section * 0.5315
 
     #adjust positions
     start_pos = x_pos + (start_pos * allocated_pos)
-    end_pos = x_pos + (end_pos * allocated_pos)
+    end_pos   = x_pos + (end_pos * allocated_pos)
 
     #plt
     cairo_context.move_to(start_pos, y - fhght)
     cairo_context.line_to(end_pos, y - fhght)
     cairo_context.line_to(end_pos, y + fhght)
     cairo_context.line_to(start_pos, y + fhght)
     cairo_context.close_path()
@@ -1936,20 +1928,18 @@
 def enumerate_seqs(cairo_context, ypos: float, xpos: float, section: float, seq_num: int):
     """enumerate sequences onto the figure"""
 
     # set the dimensions of the text & then place
     num_label = str(seq_num)
     cairo_context.set_source_rgb(0, 0, 0)
     cairo_context.set_font_size(0.75 * section)
-    cairo_context.select_font_face(
-        "Arial", cairo.FONT_SLANT_NORMAL, cairo.FONT_WEIGHT_NORMAL
-    )
+    cairo_context.select_font_face("Arial", cairo.FONT_SLANT_NORMAL, cairo.FONT_WEIGHT_NORMAL)
     label_dim = cairo_context.text_extents(num_label)
-    x = xpos - (label_dim.width * 1.2) # by 1/5th of the text label
-    y = ypos + (label_dim.height * 0.75)
+    x         = xpos - (label_dim.width * 1.2) # by 1/5th of the text label
+    y         = ypos + (label_dim.height * 0.75)
     cairo_context.move_to(x, y)
     cairo_context.show_text(num_label)
     cairo_context.stroke()
 
 def plot_sequences(alignments: dict, seq_lengths: dict, seq_klumps: dict, ref: str,
                    leftbound: int, rightbound: int, overlaps: dict, annotation: str,
                    vertical_line_exons: bool, gap_file: str, figure_height: int, figure_width: int, 
@@ -1964,15 +1954,15 @@
     # set up the plot given the number of sequences and their aligment positions
     section, y_positions, leftmost_pos, \
         ref_area, figure_height, enumeration_dict = \
              set_up_plt(figure_height, alignments, ref, leftbound, enumerating)
     
     # below functions take dimensions as an int, so will do a conversion to be safe
     figure_height = int(figure_height)
-    figure_width = int(figure_width)
+    figure_width  = int(figure_width)
     
     # determine what format to draw to when creating the image surface
     if outformat == "pdf":
        ims = cairo.PDFSurface(f"Alignment_{ref}_{leftbound}-{rightbound}.pdf",
                                figure_width, figure_height)
     elif outformat == "png":
         ims = cairo.ImageSurface(cairo.FORMAT_ARGB32, figure_width, figure_height)
@@ -1987,15 +1977,15 @@
         
     cairo_context = cairo.Context(ims)
 
     # offset by starting positions on both sides
     image_width = figure_width - (2*(figure_width * 0.025)) 
 
     # get x positions
-    image_area = scale_image_width(alignments, leftmost_pos, rightbound)
+    image_area  = scale_image_width(alignments, leftmost_pos, rightbound)
     x_positions = defaultdict(dict) 
     for seq, alignment_list in alignments.items():
         for algn in alignment_list:
             x_positions[seq][algn.map_num] = adjust_x(
                 image_width, seq, alignments, leftmost_pos, leftbound, algn.position,\
                      image_area, figure_width, algn.clipping_start, algn.adjust_start)
 
@@ -2146,15 +2136,15 @@
             klump_info = True
         else:
             klump_info = False
             seq_klumps = {}
         alignments = \
             Group_Seqs(alignments, leftbound, rightbound, ref, align_offset, clip_tolerance,
                         del_tolerance, per_overlap, klump_info, seq_klumps, t_len, t_per, 
-                        group_dels, write_groups, min_grp, write_edge_seqs, limit, False, 0)
+                        group_dels, write_groups, min_grp, write_edge_seqs, limit, False)
     # find if there are overlaps for coloration
     overlaps = identify_overlaps(alignments)
     # plot
     plot_sequences(alignments, seq_lengths, seq_klumps, ref, leftbound, 
                    rightbound, overlaps, annotation, vertical_line_exons, gap_file,
                    figure_height, figure_width, write_table, enumerating, klmp_color, 
                    klump_colors, color_by_gene,  vertical_line_gaps, vertical_line_klumps,
```

### Comparing `klumpy-1.0.5/klumpy/combine_klumps.py` & `klumpy-1.0.6/klumpy/combine_klumps.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,12 +65,12 @@
                         line = line.replace('\n',"\tNA\n")
                     combined.write(line)
             input_tsv.close()
             
 def Combine_Klumps(args):
     """Start Combining"""
 
-    list_of_tsvs, output = check_args(args)
+    list_of_tsvs, output     = check_args(args)
 
     kept_header, column_cnts = longest_header(list_of_tsvs)
 
     combine_tsvs(list_of_tsvs, output, kept_header, column_cnts)
```

### Comparing `klumpy-1.0.5/klumpy/find_gaps.py` & `klumpy-1.0.6/klumpy/find_gaps.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 # along with Klumpy. If not, see <http://www.gnu.org/licenses/>.
 #
 
 
 import gzip
 import sys
 import os
-from collections import defaultdict
-from .Classes import Seq_Record
+from   collections import defaultdict
+from  .Classes     import Seq_Record
 
 def check_args(args):
     """verify that there is a file to parse"""
 
     if args.fasta == None:
         msg = "--fasta file required for find_gaps"
         sys.exit(msg)
@@ -43,15 +43,15 @@
     # Read a gzipped file without any intervention.
     if fasta_file.endswith(".gz"):
         fh = gzip.open(fasta_file, 'rt')
     else:
         fh = open(fasta_file, "r")
 
     seq = ""
-    id = None
+    id  = None
 
     for line in fh:
         # skip empty or commented lines
         if len(line) == 0 or line.startswith('#'):
             continue
         line = line.strip()
         if line[0] == '>':
@@ -77,34 +77,33 @@
 
 def get_gaps(records: list, fasta_file: str):
     """get gaps from inputted sequences"""
 
     seq_gaps = defaultdict(list)
 
     # initialize some trackers
-    start = float("inf")
-    end = -float("inf")
+    start   = float("inf")
+    end     = -float("inf")
     gap_cnt = 0
 
     for seq_record in records:
         # will make 1-index for users
         for pos, nuc in enumerate(seq_record.seq, start = 1):
             if nuc.upper() != "N":
                 if start != float("inf"):
                     gap = (start, end)
                     seq_gaps[seq_record.seq_name].append(gap)
                     gap_cnt += 1
-                    # gaps = []
-                    start = float("inf")
-                    end = -float("inf")
+                    start    = float("inf")
+                    end      = -float("inf")
                 else:
                     continue
             elif nuc.upper() == "N":
                 start = min(pos, start) # will stay as first num
-                end = max(pos, end)
+                end   = max(pos, end)
                 #if it is the last position
                 # should never happen but still check
                 if pos == seq_record.seq_length:
                     gap = (start, end)
                     seq_gaps[seq_record.seq_name].append(gap)
                     gap_cnt += 1
 
@@ -120,30 +119,30 @@
 
     if '.gz' in fasta_file:
         filename = os.path.basename(fasta_file).split(".")[:-2]
     else:
         filename = os.path.basename(fasta_file).split(".")[:-1]
 
     filename = ".".join([text for text in filename])
-    outfile = f"{filename}_gaps.tsv"
+    outfile  = f"{filename}_gaps.tsv"
 
     with open(outfile, "w") as out:
         out.write(f"Chrom\tStart\tEnd\n")
         for seq_id, gaps in seq_gaps.items():
             for gap in gaps:
                 out.write(f"{seq_id}\t{gap[0]}\t{gap[1]}\n")
     
 def Find_Gaps(args):
     """Find the gaps in the provided fasta file"""
 
     # get arguments
     fasta_file = check_args(args)
 
     #get sequences
-    records = load_fasta_file(fasta_file)
+    records   = load_fasta_file(fasta_file)
 
     #get gaps
-    seq_gaps = get_gaps(records, fasta_file)
+    seq_gaps  = get_gaps(records, fasta_file)
 
     #write output
     write_output(seq_gaps, fasta_file)
```

### Comparing `klumpy-1.0.5/klumpy/find_klumps.py` & `klumpy-1.0.6/klumpy/find_klumps.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # along with Klumpy. If not, see <http://www.gnu.org/licenses/>.
 #
 
 
 import sys
 import os
 import gzip
-from .Classes import Klump, KLUMPS, Kmer
+from  .Classes import Klump, KLUMPS, Kmer
 
 def check_params(args):
     """check params to prevent downstream errors"""
 
     # first, check if we are starting from fast[a|q] records
     if (args.subject != None) and (args.query != None) and (args.query_map == None):
         # run kmerize
@@ -34,18 +34,18 @@
         # assign outname to kmerize output
         args.query_map = "query_map.gz"
     # the above analysis should finish first
     if args.query_map != None:
         assert os.path.isfile(args.query_map), f"Could not find {args.query_map}"
         # check min_kmers param
         assert type(args.min_kmers) is int, "--min_kmers values must be an integer"
-        assert args.min_kmers >= 0, "--min_kmers cannot be a negative integer"
+        assert args.min_kmers >= 0,         "--min_kmers cannot be a negative integer"
         # check base pair param:
         assert type(args.range) is int, "--range values must be an integer"
-        assert args.range > 0, "--range values must be greater than 0"
+        assert args.range > 0,          "--range values must be greater than 0"
         # check query ct and klump_ct
         assert type(args.query_count) is int, "--query_count must be an integer"
         assert type(args.klump_count) is int, "--klump_count must be an integer"
     else:
         msg = "find_klumps must be either provided the --coords file (generated from kmerize) or\n" + \
             "--subject and --query files in fast[a|q] format"
         sys.exit(msg)
@@ -68,25 +68,25 @@
 
     if '.gz' in filename and filename.count('.') > 1:
         filename = filename.split(".")[:-2]
     elif filename.count('.') >= 1:
         filename = filename.split(".")[:-1]
 
     filename = ".".join([text for text in filename])
-    output = f"{str(filename)}{extension}"
+    output   = f"{str(filename)}{extension}"
 
     return output
 
 def get_distributions(input: str):
     """parse the file for kmer distribution"""
 
     # create dict to store the data
     dict_of_seqs = {}
-    seq_lengths = {}
-    ksize = None
+    seq_lengths  = {}
+    ksize        = None
 
     if input.endswith(".gz"):
         cfile = gzip.open(input, "rt")
     else:
         cfile = open(input, 'r')
 
     for line in cfile:
@@ -97,15 +97,15 @@
                 except:
                     m = "ERROR: Could not parse k-size line\n" + \
                         "Offending line --> " + line
                     sys.exit(m)
             # move on regardless if it's true or not
             continue
         list_of_coords = list()
-        line = line.strip()
+        line           = line.strip()
         if line.count(':') == 1:
             seq_name = line.split(':')[0].split('[')[0][:-1]
             seq_lengths[seq_name] = \
                         int(line.split(":")[0].split("[")[1].replace("]",""))
             data = line.split(':')[1].split(',')
         else:
             seq_header = line.split(':')[:-1]
@@ -146,31 +146,31 @@
                 # check if kmers are the same direction & from the same source
                 if kmer.direction == direction and current_src == kmer.query:
                     res[-1].append(kmer)
                 else:
                     res.append([kmer])
             else:
                 res.append([kmer])
-            direction = kmer.direction
-            last = kmer.pos
+            direction   = kmer.direction
+            last        = kmer.pos
             current_src = kmer.query
         coord_dict[seq] = res
 
     # if queryID present, assign as klump ID
     full_seq_klumps = {}
 
     for seq, full_list in coord_dict.items():
         klump_cnt = 1
         seq_klump = KLUMPS(seq)
         for klumps in full_list:
             if len(klumps) < min_kmers:
                 continue
             direction = klumps[0].direction
             first_pos = klumps[0].pos
-            last_pos = klumps[-1].pos
+            last_pos  = klumps[-1].pos
             # use coordinates and source of kmers for klump name
             queries = set()
             for kmer in klumps:
                 queries.add(kmer.query)
             klmp = Klump(f"Klump{klump_cnt}", first_pos,
                          last_pos, queries, len(klumps), direction)
             seq_klump.add_klumps(klmp)
@@ -198,15 +198,15 @@
 def sort_klump_info(klump_info: dict):
     """sort klump dictionary prior to writing"""
 
     num_klumps = len(klump_info)
     if num_klumps == 1:
         return klump_info
     else:
-        fwd_klmps = {}
+        fwd_klmps  = {}
         rvsd_klmps = {}
         for klmp, klmp_info in klump_info.items():
             if klmp_info[4] == 'F':
                 fwd_klmps[klmp] = klmp_info
             elif klmp_info[4] == 'R':
                 rvsd_klmps[klmp] = klmp_info
         for klmp in reversed(list(rvsd_klmps.keys())):
@@ -263,19 +263,19 @@
                     out_header = out_header.replace("\n", "\tPair_Num\n")
                     printing_lines[0] = printing_lines[0].replace("Direction","Direction\tPair_Num")
                 out.write(command)
                 out.write(out_header)
                 header_written = True
             #initially captured during parsing,
             #hence, using original name
-            seq_length = seq_lengths[org_name]
+            seq_length  = seq_lengths[org_name]
             sorted_info = sort_klump_info(klumps_info)
             for klump, klmp_info in sorted_info.items():
                 start = klmp_info[0] + 1
-                end = klmp_info[1] + ksize # 1-based so no need to subtract 1
+                end   = klmp_info[1] + ksize # 1-based so no need to subtract 1
                 queries = klmp_info[2]
                 if len(queries) == 1:
                     query = list(queries)[0]
                 else:
                     query = ", ".join(q for q in queries)
                 size = klmp_info[3]
                 direction = klmp_info[4]
@@ -300,15 +300,15 @@
     seq_klumps_dict = find_klumps(
         dict_of_seqs, bp_range, min_kmers, query_ct, klump_ct)
     
     #write results
     if output != None:
         printing_lines = write_threshold_met(seq_klumps_dict, output, seq_lengths, ksize)
     else:
-        output = make_output_name(input, "_klumps.tsv", args.subject)
+        output         = make_output_name(input, "_klumps.tsv", args.subject)
         printing_lines = write_threshold_met(seq_klumps_dict, output, seq_lengths, ksize)
     
     #print results
     print()
     for line in printing_lines:
         print(line)
```

### Comparing `klumpy-1.0.5/klumpy/get_exons.py` & `klumpy-1.0.6/klumpy/get_exons.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 #
 
 
 import sys
 import os
 import gzip
 import textwrap
-from .Classes import EXON, Seq_Record, GeneRecord
+from  .Classes import EXON, Seq_Record, GeneRecord
 
 def determine_annotation_type(annotation: str):
     """determine whether the annotation file is a gtf or gff3 file"""
     
     # just a list of conditionals to check file extension
-    if (annotation.endswith(".gtf.gz")) or (annotation.endswith(".gtf")):
+    if (annotation.endswith(".gtf.gz"))   or (annotation.endswith(".gtf")):
         pass
     elif (annotation.endswith(".gff.gz")) or (annotation.endswith(".gff")) or \
         (annotation.endswith(".gff3.gz")) or (annotation.endswith(".gff3")):
         pass
     else:
         msg = f"No .gtf, .gtf.gz, .gff, .gff.gz, .gff3, or .gff3.gz file extension detected in {annotation}" + \
                     "\nAssuming proper input"
@@ -74,21 +74,19 @@
     """get the exons from the genes list"""
 
     if annotation.endswith(".gz"):
         fh = gzip.open(annotation, "rt")
     else:
         fh = open(annotation, 'r')
 
-    ref_seqs = {} # store reference & gene names
-    found_gene = False
+    ref_seqs       = {} # store reference & gene names
+    found_gene     = False
     gene_container = {} # this will handle duplicate genes in annotation
-    gene_record = GeneRecord()
-
-    # determine which fields to look for
-    rec_types = ["gene", "mrna", "exon", "cds"]
+    gene_record    = GeneRecord()
+    rec_types      = ["gene", "mrna", "exon", "cds"] # determine which fields to look for
 
     for line in fh:
         if line[0] == '#':
             continue
         fields = line.strip('\n').split('\t')
         rec_type = fields[2].lower()
         if rec_type in rec_types:
@@ -107,15 +105,15 @@
                     # now add the exons
                     for ex in gene_record.exon_list:
                         gene_container[gene][-1].append(ex)
                 gene_record.clear()
             gene_record.parse_attributes(fields[8])
             if rec_type in ["exon", "cds"]:
                 gene_record.store_ref(fields[0]) # store for later
-                left_pos = int(fields[3])
+                left_pos  = int(fields[3])
                 right_pos = int(fields[4])
                 direction = fields[6]           # color won't be used
                 gene_record.add_exon(left_pos, right_pos, direction, 0, line)
 
     # check last record
     if not gene_record.empty():
         found_gene, gene = gene_record.in_record(genes)
@@ -142,26 +140,23 @@
     return gene_container, ref_seqs
 
 def write_to_fasta(seq: str, gene_container: dict, gene_set: set, ofh):
     """write a set of genes to the fasta output file handle"""
 
     for gene_name in gene_set: # for each gene in set
         exon_lists = gene_container[gene_name] # get list of lists
-        if len(exon_lists) == 1:
-            duplicated = False
-        else:
-            duplicated = True
+        duplicated = (len(exon_lists) != 1)
         for i, exon_list in enumerate(exon_lists, start = 1): # for each sub list in list
             for j, exon in enumerate(exon_list, start = 1): # for each exon obj in subj list
                 start = exon.start_pos - 1 # gtf/gff are 1-based files
-                end = exon.end_pos # indexing is already excluding last pos
+                end   = exon.end_pos # indexing is already excluding last pos
                 if end > len(seq) - 1: # safety measurement
                     end = len(seq) - 1
                 direction = exon.direction
-                exon_seq = seq[start:end]
+                exon_seq  = seq[start:end]
                 if direction == '-':
                     exon_seq = Seq_Record.reverse_complement(exon_seq)
                 exon_seq = textwrap.fill(exon_seq, width = 80)
                 if duplicated:
                     header_name = f">{gene_name}_{i}_E{j}\n"
                 else:
                     header_name = f">{gene_name}_E{j}\n"
@@ -181,41 +176,41 @@
     # Read a gzipped file without any intervention.
     #
     if fasta.endswith(".gz"):
         fh = gzip.open(fasta, "rt")
     else:
         fh = open(fasta, 'r')
 
-    seq = ""
-    id = None
+    seq   = ''
+    id    = None
     found = False
-    ofh = None # only write if an exon found
+    ofh   = None # only write if an exon found
 
     for line in fh:
         # skip empty or commented lines
         if len(line) == 0 or line.startswith('#'):
             continue
         line = line.strip('\n')
         if line.startswith(">"):
             # for the 1st record
             if seq == "":
                 id = line[1:].split(" ")[0]
                 if id in ref_seqs:
                     found = True
             elif found:
                 # write exons to fasta
-                ofh = write_to_fasta(seq, gene_container, ref_seqs[id], ofh)
+                ofh   = write_to_fasta(seq, gene_container, ref_seqs[id], ofh)
                 found = False
-                seq = ""
+                seq   = ''
             id = line[1:].split(" ")[0]
             if id in ref_seqs:
                 found = True
             else:
                 found = False
-                seq = "" # just for safe measures
+                seq   = '' # just for safe measures
         elif found:
             seq += line.upper()
 
     # for last seq
     if id in ref_seqs and len(seq) > 0:
         ofh = write_to_fasta(seq, gene_container, ref_seqs[id], ofh)
```

### Comparing `klumpy-1.0.5/klumpy/grouping.py` & `klumpy-1.0.6/klumpy/grouping.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 
 # this code will not be run as a pipeline
 # but instead, will be called by scan_alignments &
 # alignment_plot to perform the grouping algorithm
 
 import os, random
-from .Classes import STRUCTURE, Del_Window, C_Score, Feature_Color, algn_blocks
-from typing import List
+from .Classes    import STRUCTURE, Del_Window, C_Score, Feature_Color, algn_blocks
+from typing      import List
 from collections import defaultdict
-from . import alignment_plot
+from .           import alignment_plot
 
 
 def clear_dict(map_dict: dict):
     """currently a temporary fix to remove possible circular references"""
 
     for v in map_dict.values():
         v.clear()
@@ -42,18 +42,18 @@
     """determine if the two sequences are incompatible due to covered regions overlapping deletions"""
 
     for cov_blck in s1_struct.covered_regions:
         cov_blk_start = cov_blck[0]
         cov_blk_end = cov_blck[1]
         for del_blck in s2_struct.deletion_regions:
             del_start = del_blck[0]
-            del_end = del_blck[1]
+            del_end   = del_blck[1]
             # buffers of tolerance
             del_start_b = del_start + del_tol
-            del_end_b = del_end - del_tol
+            del_end_b   = del_end - del_tol
             if del_start_b < cov_blk_start < del_end_b:
                 return True
             elif del_start_b < cov_blk_end < del_end_b:
                 return True
             # now do check for deletions being within the covered blocks
             del_len = del_end_b - del_start_b
             if cov_blk_start < del_start_b < del_end_b < cov_blk_end:
@@ -72,15 +72,15 @@
         s2_blks = s2_struct.covered_regions
     else:
         s1_blks = s2_struct.covered_regions
         s2_blks = s1_struct.covered_regions
 
     for blk1 in s1_blks:
         blk1_start = blk1[0]
-        blk1_end = blk1[1]
+        blk1_end   = blk1[1]
         for blk2 in s2_blks:
             blk2_start = blk2[0]
             blk2_end = blk2[1]
             if blk1_end < blk2_start:
                 continue
             if blk1_start < blk2_start:
                 start = blk2_start
@@ -93,51 +93,51 @@
             tot_cov += (end - start)
 
     return tot_cov
 
 def Within_Range(pos1: int, pos2: int, offset: int):
     """check if two positions are close enough to be considered the 'same' """
 
-    pos1_left = pos1 - offset
+    pos1_left  = pos1 - offset
     pos1_right = pos1 + offset
-    pos2_left = pos2 - offset
+    pos2_left  = pos2 - offset
     pos2_right = pos2 + offset
 
     if pos1_left <= pos2 <= pos1_right:
         return True
     elif pos2_left <= pos1 <= pos2_right:
         return True
     
     return False
 
 def check_clip_status(s1_struct: STRUCTURE, s2_struct: STRUCTURE, clip_tolerance : int):
     """check if the clipping tolerance is acceptable"""
 
     # straight forward
-    if s1_struct.clipfree and s2_struct.clipfree:
+    if (s1_struct.clipfree) and (s2_struct.clipfree):
         return True
     
     # same overall struct
     if s1_struct.num_blocks == s2_struct.num_blocks:
         # if seq 2 is contained within seq 1
         if s1_struct.align_pos <= s2_struct.align_pos <= s2_struct.align_end <= s1_struct.align_end: 
             if s2_struct.clipfree:
                 return True
             # only the beginning of the alignment is clipped
-            elif s2_struct.clipping_start and s2_struct.clipping_end == False:
+            elif (s2_struct.clipping_start) and (s2_struct.clipping_end == False):
                 clip_pos = s2_struct.clip_start
                 # if clip is entirely in seq 1
                 if clip_pos > s1_struct.align_pos:
                     clip_len = s2_struct.clip_start_len
                 else:
                     clip_len = s2_struct.align_pos - s1_struct.align_pos    
                 if clip_len <= clip_tolerance:
                     return True
             # only the end of the alignment is clipped
-            elif s2_struct.clipping_start == False and s2_struct.clipping_end:
+            elif (s2_struct.clipping_start == False) and (s2_struct.clipping_end):
                 clip_pos = s2_struct.clip_end
                 if clip_pos > s1_struct.align_end:
                     clip_len = s1_struct.align_end - s2_struct.align_end
                 else:
                     clip_len = s2_struct.clip_end_len
                 if clip_len <= clip_tolerance:
                     return True
@@ -156,25 +156,25 @@
                 if clip_len_s <= clip_tolerance and clip_len_e <= clip_tolerance:
                     return True
         # seq 1 is, instead, within seq 2
         elif s2_struct.align_pos <= s1_struct.align_pos <= s1_struct.align_end <= s2_struct.align_end:
             if s1_struct.clipfree:
                 return True
             # only the beginning of the alignment is clipped
-            elif s1_struct.clipping_start and s1_struct.clipping_end == False:
+            elif (s1_struct.clipping_start) and (s1_struct.clipping_end == False):
                 clip_pos = s1_struct.clip_start
                 # if clip is entirely in seq 1
                 if clip_pos > s2_struct.align_pos:
                     clip_len = s1_struct.clip_start_len
                 else:
                     clip_len = s1_struct.align_pos - s2_struct.align_pos    
                 if clip_len <= clip_tolerance:
                     return True
             # only the end of the alignment is clipped
-            elif s1_struct.clipping_start == False and s1_struct.clipping_end:
+            elif (s1_struct.clipping_start == False) and (s1_struct.clipping_end):
                 clip_pos = s1_struct.clip_end
                 if clip_pos > s2_struct.align_end:
                     clip_len = s2_struct.align_end - s1_struct.align_end
                 else:
                     clip_len = s1_struct.clip_end_len
                 if clip_len <= clip_tolerance:
                     return True
@@ -186,15 +186,15 @@
                     clip_len_s = s1_struct.clip_start_len
                 else:
                     clip_len_s = s1_struct.align_pos - s2_struct.align_pos
                 if clip_pos_e > s2_struct.align_end:
                     clip_len_e = s2_struct.align_end - s1_struct.align_end
                 else:
                     clip_len_e = s1_struct.align_end
-                if clip_len_s <= clip_tolerance and clip_len_e <= clip_tolerance:
+                if (clip_len_s <= clip_tolerance) and (clip_len_e <= clip_tolerance):
                     return True
         # seq 2 overlaps at the beginning
         elif s1_struct.align_pos <= s2_struct.align_pos <= s1_struct.align_end:
             clip_pos = s2_struct.clip_start
             if clip_pos < s1_struct.align_pos:
                 clip_len = s2_struct.align_pos - s1_struct.align_pos
             else:
@@ -244,29 +244,29 @@
         overlap = True
     if s1_struct.align_pos <= s2_struct.align_end <= s1_struct.align_end:
         overlap = True
     elif s2_struct.align_pos <= s1_struct.align_end <= s2_struct.align_end:
         overlap = True
 
     if overlap:
-        if s1_struct.clipfree and s2_struct.clipfree:
+        if (s1_struct.clipfree) and (s2_struct.clipfree):
             return overlap
         else:
 
             num_passes = 0
             
             # calc & overlap between the two
-            cov_bases = calc_overlap(s1_struct, s2_struct)
+            cov_bases       = calc_overlap(s1_struct, s2_struct)
             s1_prop_aligned = (cov_bases / s1_struct.num_align_bp) * 100
             s2_prop_aligned = (cov_bases / s2_struct.num_align_bp) * 100
 
-            if s1_prop_aligned >= min_per and s2_prop_aligned >= min_per:
+            if (s1_prop_aligned >= min_per) and (s2_prop_aligned >= min_per):
                 num_passes += 1
             # both are clipped at the beginning
-            if s1_struct.clipping_start and s2_struct.clipping_start:
+            if (s1_struct.clipping_start) and (s2_struct.clipping_start):
                 if s1_struct.align_pos < s2_struct.align_pos:
                     if s1_struct.align_pos < s2_struct.clip_start:
                         clip_dist = s2_struct.clip_start_len
                         if clip_dist <= clip_tolerance:
                             num_passes += 1
                     else:
                         clip_dist = s2_struct.align_pos - s1_struct.align_pos
@@ -310,15 +310,15 @@
                     if clip_dist <= clip_tolerance:
                         num_passes += 1
                 elif s1_struct.align_pos < s2_struct.clip_start < s1_struct.align_end:
                     clip_dist = s1_struct.align_end - s2_struct.clip_start
                     if clip_dist <= clip_tolerance:
                         num_passes += 1
             # now for the clipping ends
-            if s1_struct.clipping_end and s2_struct.clipping_end:
+            if (s1_struct.clipping_end) and (s2_struct.clipping_end):
                 if s2_struct.align_end < s1_struct.align_end:
                     if s2_struct.clip_end < s1_struct.align_end:
                         clip_dist = s2_struct.clip_end_len
                         if clip_dist <= clip_tolerance:
                             num_passes += 1
                     else:
                         clip_dist = s1_struct.align_end - s2_struct.align_end
@@ -365,38 +365,38 @@
                         num_passes += 1
             if num_passes < 2:
                 overlap = False
 
     return overlap
 
 
-def make_group_rep(align_structs: dict, seqs: list):
+def make_group_rep(align_structs: dict, seqs: set):
     """create a representing alignment using the aligned blocks for the seqs"""
 
     # first, lets sort by first position of covered regions
     sorted_seqs = [s for s, _ in sorted(align_structs.items(), key = lambda item:item[1].covered_regions[0][0]) if s in seqs]
 
     # initialize with first alignment (is this really better than using copy.deepcopy?)
-    first_blk = align_structs[sorted_seqs[0]].covered_regions[0][0] + 0 # add 0 to make copy
+    first_blk  = align_structs[sorted_seqs[0]].covered_regions[0][0] + 0 # add 0 to make copy
     second_blk = align_structs[sorted_seqs[0]].covered_regions[0][1] + 0 
     group_blks = [[first_blk, second_blk]]
 
     if len(seqs) < 2:
         return group_blks # only 1 seq
 
     for seq in sorted_seqs[1:]:
         seq_struct = align_structs[seq]
         for blk in seq_struct.covered_regions:
             blk_start = blk[0]
-            blk_end = blk[1]
-            added = False
+            blk_end   = blk[1]
+            added     = False
             # now to add the current blk to the group blocks
             for i, rep_blk in enumerate(group_blks):
                 rep_start = rep_blk[0]
-                rep_end = rep_blk[1]
+                rep_end   = rep_blk[1]
                 if rep_start <= blk_start <= blk_end <= rep_end:
                     added = True
                     break # end rep_blk loop
                 elif rep_start <= blk_start <= rep_end <= blk_end:
                     rep_blk[1] = blk_end
                     added = True
                     break # break to move onto next seq block
@@ -478,27 +478,55 @@
             
     return False
 
 def extend_to_rep(seq1_struct: STRUCTURE, rep_seq: list, clip_tolerance: int, align_offset: int):
     """if the sequence can be added to the ends of the represented group"""
 
     last_blk_num = len(rep_seq) - 1
-
-    tot_blocks = len(rep_seq)
+    tot_blocks   = len(rep_seq)
 
     for i, blk in enumerate(rep_seq):
         blk_start = blk[0] - align_offset
-        blk_end = blk[1] + align_offset
-        okayed = False
-        if i == 0 or tot_blocks == 1:
-            if seq1_struct.align_pos <= blk_start <= seq1_struct.align_end <= blk_end:
+        blk_end   = blk[1] + align_offset
+        if (tot_blocks == 1):
+            if ((seq1_struct.align_pos <= blk_start <= seq1_struct.align_end <= blk_end) and seq1_struct.clip_end_len <= clip_tolerance) or \
+                (seq1_struct.align_pos <= blk_start <= blk_end <= seq1_struct.align_end) or \
+                ((blk_start <= seq1_struct.align_pos <= blk_end <= seq1_struct.align_end) and seq1_struct.clip_start_len <= clip_tolerance):
+                return True
+            if (seq1_struct.clip_start_len > 0):
+                if (blk_start < seq1_struct.align_pos - seq1_struct.clip_start_len):
+                    if (seq1_struct.clip_start_len > clip_tolerance):
+                        return False
+                    else:
+                        return True
+                elif (blk_start < seq1_struct.align_pos):
+                    if (seq1_struct.align_pos - blk_start < clip_tolerance):
+                        return True
+                    else:
+                        return False
+            if (seq1_struct.clip_end_len > 0):
+                if (blk_start <= seq1_struct.align_end <= blk_end):
+                    if (seq1_struct.align_end + seq1_struct.clip_end_len < blk_end):
+                        if (seq1_struct.clip_end_len <= clip_tolerance):
+                            return True
+                        else:
+                            return False
+                    elif (blk_end - seq1_struct.align_pos <= clip_tolerance):
+                        return True
+                    else:
+                        return False
+        if i == 0:
+            okayed = False
+            if seq1_struct.align_pos <= blk_start <= seq1_struct.align_end <= blk_end or \
+               seq1_struct.align_pos <= blk_start <= blk_end <= seq1_struct.align_end:
                 okayed = True
         if not okayed:
-            if i == last_blk_num or tot_blocks == 1:
-                if blk_start <= seq1_struct.align_pos <= blk_end <= seq1_struct.align_end:
+            if i == last_blk_num:
+                if (blk_start <= seq1_struct.align_pos <= blk_end <= seq1_struct.align_end) and \
+                    (((blk_start - seq1_struct.align_pos) <= clip_tolerance) or seq1_struct.clip_start_len < clip_tolerance):
                     okayed = True
             else:
                 continue
         if okayed:
             passed = False
             if i == 0 or tot_blocks == 1:
                 if seq1_struct.clipping_end:
@@ -541,15 +569,15 @@
         if s2_struct.align_end <= s1_struct.align_pos <= s1_struct.align_end <= s2_struct.clip_end:
             cscore.incompatible = True
             return cscore
 
     # it is possible that they can be grouped
     # need to gather evidence
     cscore.possible = True
-    
+
     # do they overlap at all
     if s1_struct.align_pos <= s2_struct.align_pos <= s1_struct.align_end:
         cscore.evidence += 1
         # cscore.POE.append("s1 align_pos <= s2 align_pos <= s1 align_end")
     elif s2_struct.align_pos <= s1_struct.align_pos <= s2_struct.align_end:
         cscore.evidence += 1
         # cscore.POE.append("s2 align_pos <= s1 align_pos <= s2 align_end")
@@ -560,19 +588,26 @@
     elif s2_struct.align_pos <= s1_struct.align_end <= s2_struct.align_end:
         cscore.evidence += 1
         # cscore.POE.append("s2 align_pos <= s1 align_end <= s2 align_end")
     # no evidence so they align at separate parts of the assembly
     if cscore.evidence == 0:
         return cscore # these two cannot be bridged on their own
     
+    # alternatively, if evidence is 2 and they both are in agreement
+    # with the reference, they are compatible
+    if (s1_struct.num_blocks == 1) and (s1_struct.clipfree) and (s2_struct.num_blocks == 1) and (s2_struct.clipfree):
+        if (cscore.evidence  == 2):
+            cscore.groupable = True
+            return cscore
+    
     # are there any deletions overlapping the sequences
-    if s1_struct.num_blocks > 1 or s2_struct.num_blocks > 1:
+    if (s1_struct.num_blocks > 1) or (s2_struct.num_blocks > 1):
         # check if they can be grouped
         for del_wind in del_windows:
-            if s1_struct.seq_name in del_wind.seqs and s2_struct.seq_name in del_wind.seqs:
+            if (s1_struct.seq_name in del_wind.seqs) and (s2_struct.seq_name in del_wind.seqs):
                 cscore.groupable = True
                 return cscore
           
         #check if start & end positions of blocks match
         for blk1 in s1_struct.covered_regions:
             blk1_start = blk1[0]
             blk1_end = blk1[1]
@@ -593,20 +628,20 @@
             return cscore
         incomp = check_blocks(s2_struct, s1_struct, del_tol)
         if incomp:
             cscore.incompatible = True
             return cscore
     
     # calc & overlap between the two
-    cov_bases = calc_overlap(s1_struct, s2_struct)
+    cov_bases       = calc_overlap(s1_struct, s2_struct)
     s1_prop_aligned = (cov_bases / s1_struct.num_align_bp) * 100
     s2_prop_aligned = (cov_bases / s2_struct.num_align_bp) * 100
 
     # check if they can grouped
-    if s1_prop_aligned >= percent_overlap and s2_prop_aligned >= percent_overlap:
+    if (s1_prop_aligned >= percent_overlap) and (s2_prop_aligned >= percent_overlap):
         cscore.evidence += 1
         # cscore.POE.append("s1_prop_aligned >= per overlap and s2_prop_aligned >= per overlap")
         acceptable = check_clip_status(s1_struct, s2_struct, clip_tolerance)
         if acceptable:
             cscore.groupable = True
             return cscore 
 
@@ -638,30 +673,30 @@
                 cscore.groupable = True
                 # cscore.POE.append("sum(s1 del_lengths) == sum(s2 del_lengths)")
                 return cscore
 
     # do they have the same number of blocks
     if s1_struct.num_blocks == s2_struct.num_blocks:
         # check for clear compatibilitiy
-        if s1_struct.num_blocks == 1 and s2_struct.num_blocks == 1:
+        if (s1_struct.num_blocks == 1) and (s2_struct.num_blocks == 1):
             acceptable = check_clip_status(s1_struct, s2_struct, clip_tolerance)
             if acceptable:
                 cscore.evidence += 1
                 # cscore.POE.append("check_clip_status(s1, s2, clip_tolerance) - acceptable")
 
     # do they have the same clipping patterns
     if s1_struct.clipping_start == s2_struct.clipping_start:
         cscore.evidence += 1
         # cscore.POE.append("s1 clipping_start == s2 clipping_start")
     if s1_struct.clipping_end == s2_struct.clipping_end:
         cscore.evidence += 1
         # cscore.POE.append("s1 clipping_end == s2 clipping_end")
 
     # use klump info if present
-    if klump_info and len(s1_klumps) > 0 and len(s2_klumps) > 0:
+    if klump_info and (len(s1_klumps) > 0) and (len(s2_klumps) > 0):
         s1_sources = set()
         s2_sources = set()
         for k in s1_klumps:
             s1_sources.add(k.query_source)
         for k in s2_klumps:
             s2_sources.add(k.query_source)
         s1_diff = s1_sources.difference(s2_sources)
@@ -676,32 +711,32 @@
         cscore.reasonable = True
     else:
         cscore.unlikely = True
     
     return cscore
 
 def can_be_grouped(align_structs: dict, seq: str, del_tol: int, clip_tolerance: int, per_overlap: float, 
-                   seq_list: list, bck_trace: list = []):
+                   seq_set: set, bck_trace: list = []):
     """looks for incompatibilities and overlap of seq 1 in reference to seq 2"""
     
     compatible = True
-    overlap = False
+    overlap    = False
 
     s1_struct = align_structs[seq]
 
     # a check for clipping issues at certain stages
     if bck_trace:
         if not s1_struct.clipfree:
-            if s1_struct.clip_start_len > clip_tolerance or s1_struct.clip_end_len > clip_tolerance:
+            if (s1_struct.clip_start_len > clip_tolerance) or (s1_struct.clip_end_len > clip_tolerance):
                 for bck_seq in bck_trace:
                     acceptable = check_clip_status(s1_struct, align_structs[bck_seq], clip_tolerance)
                     if not acceptable:
                         return acceptable, overlap
 
-    for seq2 in seq_list:
+    for seq2 in seq_set:
         # this happens when trying to group seqs that need grouping
         if seq == seq2:
             continue
         s2_struct = align_structs[seq2]
         if not s2_struct.trustworthy:
             continue
         incompatible = check_blocks(s1_struct, s2_struct, del_tol)
@@ -712,15 +747,15 @@
             overlap = True 
 
     return compatible, overlap
 
 def Group_Seqs(alignments: dict, leftbound: int, rightbound: int, ref: str, align_offset: int, 
                clip_tolerance: int, del_tol: int, per_overlap: float, klump_info: bool, 
                seq_klumps: dict, t_len: int, t_per: float, group_dels: bool, write_groups: bool,
-               min_grp: int, write_edge_seqs: bool, limit: int, scan: bool, num_of_groups: int):
+               min_grp: int, write_edge_seqs: bool, limit: int, scan: bool):
     """group sequences by alignment patterns"""
 
     if not scan:
         print("Grouping sequences..")
 
     coverage = len(alignments)
 
@@ -729,85 +764,79 @@
             print(f"Randomly subsampling {limit} alignment records for grouping analysis")
         alignments = dict(random.sample(alignments.items(), limit))
 
     # keep track of the structure of each alignment
     align_structs = {}
 
     # keep track of the alignment positions for each sequence
-    align_starts = {}
+    align_starts  = {}
 
-    left_flank = leftbound # default
+    left_flank  = leftbound # default
     right_flank = rightbound
 
-    del_windows = []
+    del_windows  = []
     clipped_seqs = []
-    good_aligns = set()
-    align_num = 0
+    good_aligns  = set()
+    align_num    = 0
 
     # fill out using alignments
     for seq, aligns in alignments.items():
         if seq == ref:
             continue
         # only using primary alignments
         for align in aligns:
             if align.IsPrimary: # only groups primary alignments
                 clip_start_len = align.adjust_start
                 clipping_start = align.clipping_start
-                clip_end_len = align.adjust_end
-                clipping_end = align.clipping_end
-                align_pos = align.position
-                align_len = align.aligned_length
-                align_blocks = align.align_blocks.blocks
-                del_blocks = align.align_blocks.block_del
-                align_end = align_pos + align_len - 1
-                per_align = align.percent_aligned
+                clip_end_len   = align.adjust_end
+                clipping_end   = align.clipping_end
+                align_pos      = align.position
+                align_len      = align.aligned_length
+                align_blocks   = align.align_blocks.blocks
+                del_blocks     = align.align_blocks.block_del
+                align_end      = align_pos + align_len - 1
+                per_align      = align.percent_aligned
                 # check for blocks out of chrom bound
                 if clipping_start == None:
-                    clip_start = align_pos # range will not produce a value
+                    clip_start     = align_pos # range will not produce a value
                     clip_start_len = 0
                     clipping_start = False
                 else:
                     clip_start = align_pos - clip_start_len
                     clipping_start = True
                 if clipping_end == None:
-                    clip_end = align_end
+                    clip_end     = align_end
                     clip_end_len = 0
                     clipping_end = False
                 else:
-                    clip_end = align_end + clip_end_len
+                    clip_end     = align_end + clip_end_len
                     clipping_end = True
                 # do a check here so I don't have to put several checks if already added
                 if clipping_start or clipping_end:
                     clipped_seqs.append(seq)
-                    clipped = True
-                else:
-                    clipped = False       
                 # keep record of alignment structure
-                covered_regions = []
+                covered_regions  = []
                 deletion_regions = []
-                seq_len = align.seq_len
-                num_blocks = len(align_blocks)
-                del_lengths = list(del_blocks.values())
-                del_lengths = del_lengths[:-1] # last block always has 0 deletions
-                num_dels = len(del_lengths)
-                # will first attempt to combine good alignments
-                if num_dels == 0 and not clipped:
-                    good_aligns.add(seq)
-                num_align_bp = 0
+                seq_len          = align.seq_len
+                num_blocks       = len(align_blocks)
+                del_lengths      = list(del_blocks.values())
+                del_lengths      = del_lengths[:-1] # last block always has 0 deletions
+                num_dels         = len(del_lengths)
+                num_align_bp     = 0
                 blk_start = align_pos
                 for blk in align_blocks:
                     blk_len = align_blocks[blk]
                     del_len = del_blocks[blk]
                     blk_end = blk_start + blk_len
-                    num_align_bp += blk_len
                     blk_tup = [blk_start, blk_end]
+                    num_align_bp += blk_len
                     covered_regions.append(blk_tup)
                     del_start = blk_end + 1
-                    del_end = del_start + del_len   
-                    del_tup = [del_start, del_end]
+                    del_end   = del_start + del_len   
+                    del_tup   = [del_start, del_end]
                     if del_start != del_end:
                         if len(del_windows) == 0:
                             first_wind = Del_Window(del_start, del_end, seq)
                             del_windows.append(first_wind)
                         else:
                             added = False
                             for del_win in del_windows:
@@ -830,32 +859,34 @@
                 deletion_regions = deletion_regions[:-1] # remove last 0 length block
                 struct = \
                     STRUCTURE(num_blocks, num_dels, del_lengths, align_pos, 
                               align_end, clipping_start, clipping_end,
                               clip_start_len, clip_end_len, covered_regions,
                               deletion_regions, clip_start, clip_end,
                               seq_len, per_align, num_align_bp, seq, align_num)
-                struct.evaluate(t_len, t_per)
+                struct.evaluate(t_len, t_per, clip_tolerance)
+                if (struct.num_del == 0) and (struct.clipfree):
+                    good_aligns.add(seq)
                 align_structs[seq] = struct
-                align_starts[seq] = clip_start
+                align_starts[seq]  = clip_start
                 if clip_start < left_flank:
                     left_flank = clip_start
                 if clip_end > right_flank:
                     right_flank = clip_end
                 align_num += 1
 
     # sort from left to right and start from leftmost alignment
     sorted_good_aligns = []
 
     for s in dict(sorted(align_starts.items(), key = lambda x : x[1])).keys():
         if s in good_aligns:
             sorted_good_aligns.append(s)
  
-    group_sets = defaultdict(list)
-    has_group = set()
+    group_sets        = defaultdict(list)
+    has_group         = set()
     compatibility_map = {}
     good_aligns.clear()
 
     # first, try to tile across with the "good" alignments and assume the reference
     # is correct. In other words, can we find a path across the region?
 
     ns = len(sorted_good_aligns)
@@ -863,94 +894,113 @@
     for i, seq in enumerate(sorted_good_aligns):
         seq1_struct = align_structs[seq]
         if seq not in compatibility_map:
             compatibility_map[seq] = {}
             seq1_klumps = seq_klumps.get(seq, []) # default to empty list
         if i + 1 == ns:
             break
+        j = i
         for seq2 in sorted_good_aligns[i+1:]:
+            j += 1
             if seq2 in compatibility_map[seq]:
                 continue
             if seq2 not in compatibility_map:
                 compatibility_map[seq2] = {}
             seq2_struct = align_structs[seq2]
             if not seq2_struct.trustworthy:
                 continue
             seq2_klumps = seq_klumps.get(seq2, [])
-            cscore = compare_alignments(seq1_struct, seq2_struct, klump_info, seq1_klumps, seq2_klumps, 
-                                        del_tol, del_windows, align_offset, per_overlap, clip_tolerance)
+            cscore      = compare_alignments(seq1_struct, seq2_struct, klump_info, seq1_klumps, seq2_klumps, 
+                                             del_tol, del_windows, align_offset, per_overlap, clip_tolerance)
             if cscore.groupable:
                 group_sets[seq].append(seq2)
                 has_group.add(seq)
                 has_group.add(seq2)
             compatibility_map[seq][seq2] = compatibility_map[seq2][seq] = cscore
 
-    group_map = {}
-    grp_cnt = 0
-    grp_backtrace = defaultdict(list)
+    group_map     = {}
+    grp_cnt       = 0
+    grp_backtrace = defaultdict(set)
 
     for i, seq in enumerate(sorted_good_aligns):
         if seq not in has_group:
             continue
         if seq not in group_map:
-            grp_cnt += 1
+            grp_cnt       += 1
             group_map[seq] = grp_cnt
-            grp_backtrace[grp_cnt].append(seq)
-        else:
-            continue
-        grp_num = group_map[seq]
+            grp_backtrace[grp_cnt].add(seq)
+        # else:
+        #     continue
+        grp_num         = group_map[seq]
         compatible_seqs = group_sets[seq]
         if i + 1 == ns:
             break
+        j = i
         for seq2 in sorted_good_aligns[i+1:]:
+            j += 1
             if seq2 in group_map:
                 continue
-            compatible, overlap = \
-                can_be_grouped(align_structs, seq2, del_tol, clip_tolerance, 
-                               per_overlap, compatible_seqs, grp_backtrace[grp_num])
+            # if already considered groupable
+            if (compatibility_map[seq][seq2].groupable):
+                compatible, overlap = True, True
+            else:
+                compatible, overlap = \
+                    can_be_grouped(align_structs, seq2, del_tol, clip_tolerance, 
+                                   per_overlap, compatible_seqs, grp_backtrace[grp_num])
             if compatible:
                 if overlap:
                     if seq2 not in group_map:
                         group_map[seq2] = grp_num
-                        grp_backtrace[grp_num].append(seq2)
+                        grp_backtrace[grp_num].add(seq2)
                 # check the updated groups
                 else:
-                    align_num = align_structs[seq2].align_num
-                    for seq3 in reversed(sorted_good_aligns[:align_num - 1]):
+                    j -= 1
+                    while (j != i):
+                        seq3 = sorted_good_aligns[j]
                         if seq3 in grp_backtrace[grp_num]:
                             if seq3 in compatibility_map[seq2]:
                                 cscore = compatibility_map[seq2][seq3]
-                                if cscore.groupable and seq2 not in group_map:
+                                if (cscore.groupable) and (seq2 not in group_map):
                                     group_map[seq2] = grp_num
-                                    grp_backtrace[grp_num].append(seq2)
+                                    grp_backtrace[grp_num].add(seq2)
+                                    break
+                        j -= 1
+                    # align_num = align_structs[seq2].align_num
+                    # for seq3 in reversed(sorted_good_aligns[:align_num - 1]):
+                    #     if seq3 in grp_backtrace[grp_num]:
+                    #         if seq3 in compatibility_map[seq2]:
+                    #             cscore = compatibility_map[seq2][seq3]
+                    #             if cscore.groupable and seq2 not in group_map:
+                    #                 group_map[seq2] = grp_num
+                    #                 grp_backtrace[grp_num].append(seq2)
 
     # no longer needed
     sorted_good_aligns.clear()
     clear_dict(group_sets)
+    
+    rep_seqs = {}
+    for grp_id, seqs in grp_backtrace.items():
+        rep_seqs[grp_id] = make_group_rep(align_structs, seqs)
 
     # now this is where we attempt to go through and add different seqs
     # ideally at each stage, the seqs needing grouping will grow smaller
     # and smaller
 
-    rep_seqs = {}
-    for grp_id, seqs in grp_backtrace.items():
-        rep_seqs[grp_id] = make_group_rep(align_structs, seqs)
-
     for seq in align_starts.keys():
         if seq in group_map:
             continue
         if not align_structs[seq].trustworthy:
             continue
         seq1_struct = align_structs[seq]
         for grp_num, seq_rep in rep_seqs.items():
             # NOTE: true will only occur if the seq is within the rep
             compatible = covered_by_rep(seq1_struct, seq_rep, del_tol, clip_tolerance, align_offset)
             if compatible:
                 group_map[seq] = grp_num
-                grp_backtrace[grp_num].append(seq)
+                grp_backtrace[grp_num].add(seq)
                 break
 
     # next, group by deletion windows if there are any
     grp_num = len(grp_backtrace)
     del_seqs = []
     marked = set()
     for del_wind in del_windows:
@@ -975,16 +1025,16 @@
             # skip comparing twice
             if seq2 in compatibility_map[seq]:
                 continue
             if seq2 not in compatibility_map:
                 compatibility_map[seq2] = {}
             seq2_struct = align_structs[seq2]
             seq2_klumps = seq_klumps.get(seq2, [])
-            cscore = compare_alignments(seq1_struct, seq2_struct, klump_info, seq1_klumps, seq2_klumps, 
-                                        del_tol, del_windows, align_offset, per_overlap, clip_tolerance)
+            cscore      = compare_alignments(seq1_struct, seq2_struct, klump_info, seq1_klumps, seq2_klumps, 
+                                             del_tol, del_windows, align_offset, per_overlap, clip_tolerance)
             if cscore.groupable:
                 has_group.add(seq)
                 has_group.add(seq2)
             compatibility_map[seq][seq2] = compatibility_map[seq2][seq] = cscore
             
     del_seqs.clear()
 
@@ -996,109 +1046,145 @@
     # before it was del_seqs?
     for seq, cscore_dict in compatibility_map.items():
         if seq not in group_map:
             grp_cnt = len(grp_backtrace) + 1
             group_map[seq] = grp_cnt
         grp_num = group_map[seq]
         if seq not in grp_backtrace[grp_num]:
-            grp_backtrace[grp_num].append(seq)
+            grp_backtrace[grp_num].add(seq)
         for seq2, cscore in cscore_dict.items():
             if seq2 in group_map:
                 continue
             if cscore.groupable or cscore.likely:
                 if seq2 not in group_map:
                     group_map[seq2] = grp_num
                     has_group.add(seq2)
                     if seq2 not in grp_backtrace[grp_num]:
-                        grp_backtrace[grp_num].append(seq2)
+                        grp_backtrace[grp_num].add(seq2)
             # assume alignments with deletions represent the same locus
             elif group_dels:
                 compatible, overlap = \
                     can_be_grouped(align_structs, seq2, del_tol, clip_tolerance,
                                    per_overlap, grp_backtrace[grp_num])
                 if compatible and overlap:
                     if seq2 not in group_map:
                         group_map[seq2] = grp_num
                         has_group.add(seq2)
                         if seq2 not in grp_backtrace[grp_num]:
-                            grp_backtrace[grp_num].append(seq2)
+                            grp_backtrace[grp_num].add(seq2)
     
     clear_dict(compatibility_map)
 
     # create new rep alignments
     for grp_id, seqs in grp_backtrace.items():
-        if grp_id not in rep_seqs and len(seqs) >= min_grp:
-            rep_seqs[grp_id] = make_group_rep(align_structs, seqs)
+        rep_seqs[grp_id] = make_group_rep(align_structs, seqs)
+        # if (grp_id not in rep_seqs) and (len(seqs) >= min_grp):
 
     # # now to added clipped seqs under the assumption that if they start at the same position, they are of the same locus
     clip_dict = defaultdict(list)
     
+    in_set = set()
     for i, seq in enumerate(clipped_seqs):
         if seq in group_map:
             continue
         seq1_struct = align_structs[seq]
-        if (not seq1_struct.trustworthy) or (i + 1 >= len(clipped_seqs)):
+        if (not seq1_struct.trustworthy):
+            continue
+        if (i + 1 >= len(clipped_seqs)):
+            # only clipped seq in the set of alignments
+            if (len(clipped_seqs) == 1):
+                clip_dict[seq] = []
+                break
             continue
         for seq2 in clipped_seqs[i+1:]:
             seq2_struct = align_structs[seq2]
             if (not seq2_struct.trustworthy) or (seq2 in group_map):
                 continue
             if Within_Range(seq1_struct.align_pos, seq2_struct.align_pos, align_offset) or \
                 Within_Range(seq1_struct.align_end, seq2_struct.align_end, align_offset):
                 clip_dict[seq].append(seq2)
+                clip_dict[seq2].append(seq)
+                in_set.add(seq)
+                in_set.add(seq2)
+        if (seq not in clip_dict):
+            clip_dict[seq] = [] # will be a stand alone
+            in_set.add(seq)
+
+    # others will remain as a set of size 1
+    for seq in clipped_seqs:
+        if (seq not in in_set):
+            clip_dict[seq] = []
+    
+    in_set.clear()
+
+    # now we create a new dict and sort by the size of the clipping
+    sorted_clips = {}
+    for seq, seq_list in clip_dict.items():
+        cur_max = align_structs[seq].clip_start_len + align_structs[seq].clip_end_len
+        for s in seq_list:
+            s_struct = align_structs[s]
+            if (s_struct.clip_start_len + s_struct.clip_end_len) > cur_max:
+                cur_max = s_struct.clip_start_len + s_struct.clip_end_len
+        sorted_clips[seq] = cur_max
+    
+    sorted_clip_list = []
+    for s in dict(sorted(sorted_clips.items(), key = lambda x : x[1])).keys():
+        sorted_clip_list.append(s)
 
-    # # remove enteries of below the min group threshold
-    clip_dict_filtered = {k:v for k,v in clip_dict.items() if len(v) >= min_grp}
 
     # now to add the group map          
     # first, will attempt to add to trailing ends
     # of current groups
 
-    for seq_name, seq_list in clip_dict_filtered.items():
+    for seq_name in sorted_clip_list:
+        seq_list = clip_dict[seq_name]
         if seq_name not in group_map:
             compatible = False
             seq1_struct = align_structs[seq_name]
             for group_num, sequence_rep in rep_seqs.items():
                 compatible = \
                       extend_to_rep(seq1_struct, sequence_rep,
                                     clip_tolerance, align_offset)
                 if compatible:
                     group_map[seq_name] = group_num
                     break
             # if it remained false the entire time
             if not compatible:
-                new_grp_num = len(grp_backtrace) + 1
+                new_grp_num         = len(grp_backtrace) + 1
                 group_map[seq_name] = new_grp_num
             # now use the group number for seq
             # to assign the other clipped sequences
             # that are within its alignment range
             seq_grp_num = group_map[seq_name]
-            grp_backtrace[seq_grp_num].append(seq_name)
+            grp_backtrace[seq_grp_num].add(seq_name)
             for s in seq_list:
                 if s not in group_map:
                     group_map[s] = seq_grp_num
-                    grp_backtrace[seq_grp_num].append(s)
-
+                    grp_backtrace[seq_grp_num].add(s)
+            # now to recreate the new rep sequence
+            if compatible:
+                rep_seqs[seq_grp_num] = make_group_rep(align_structs, grp_backtrace[seq_grp_num])
 
     # last bit of filtering
-    grp_cnt = 0
+    grp_cnt   = 0
     to_remove = []
+    rep_seqs.clear()
     for grp_id, seqs in grp_backtrace.items():
         if len(seqs) < min_grp:
             for seq in seqs:
                 del group_map[seq]
             to_remove.append(grp_id)
         else:
             grp_cnt += 1
+            rep_seqs[grp_cnt] = make_group_rep(align_structs, seqs)
         
     # remove from back trace
     for grp_id in to_remove:
         del grp_backtrace[grp_id]
 
-
     # if not scanning, then plot the results & maybe write output
     if not scan:
 
         msg = f"Found {grp_cnt} group"
 
         if grp_cnt == 1:
             print(msg)
@@ -1133,26 +1219,26 @@
                                 line = f">{seq}\n{a.seq}\n"
                                 fh.write(line)
                                 break
         
         # create a dict of seqs with clips per group 
         # since we are already going through the alignments
         if write_edge_seqs:
-            clip_dict = defaultdict(list)
+            clip_dict  = defaultdict(list)
             final_grps = defaultdict(list)
                             
         # change color of alignments based on group number
         for seq, aligns in alignments.items():
             if seq == ref:
                 continue
             elif seq not in group_map:
                 for align in aligns:
                     align.seq_color = Feature_Color(1, 1, 1) # white is reserved for background & off switch
             else:
-                grp = group_map[seq]
+                grp    = group_map[seq]
                 aligns = alignments[seq]
                 for align in aligns:
                     if align.IsPrimary:
                         align.seq_color = alignment_plot.get_color(False, True, grp)
                         align.group_num = grp
                         # add seqs to write
                         if write_edge_seqs:
@@ -1199,33 +1285,24 @@
                 # remove any empty files
                 if not wrote:
                     os.remove(f"Group_{grp}_Informative_Seqs.txt")
 
         # colors have changed
         return alignments
     else:
-        clear_dict(rep_seqs) # won't need these anymore
         group_map.clear()
-        if grp_cnt >= num_of_groups:
-            tiled = False
-            for seqs in grp_backtrace.values():
-                rep_sequence = make_group_rep(align_structs, seqs)
-                for blk in rep_sequence:
-                    if blk[0] <= leftbound <= rightbound <= blk[1]:
-                        tiled = True
-                        break
-                if tiled:
-                    break
-            clear_dict(grp_backtrace)
-            align_structs.clear()
-            return not tiled # inverse, so true -> false, and false -> true
-        else:
-            clear_dict(grp_backtrace)
-            align_structs.clear()
-            return False
+        for rep_sequence in rep_seqs.values():
+            for blk in rep_sequence:
+                if blk[0] <= leftbound <= rightbound <= blk[1]:
+                    return grp_cnt
+        clear_dict(grp_backtrace)
+        align_structs.clear()
+        # none were able to be tiled
+        return (grp_cnt * -1)
+
         
 def within_window(seq_pos: int, align_blocks: algn_blocks, start: int, end: int, clipped_start: int):
     """determine if the sequence is within the current and next window"""
 
     # current window
     if start <= seq_pos <= end:
         return True
```

### Comparing `klumpy-1.0.5/klumpy/klump_plot.py` & `klumpy-1.0.6/klumpy/klump_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,27 +45,29 @@
             if len(line.strip().split("\t")) != 3:
                 sys.exit(f"Check if {args.gap_file} is a three column file")
             else:
                 break
     
     if args.klump_colors != None:
         assert os.path.isfile(args.klump_colors), f"Could not find {args.klump_colors}"
-        assert type(args.color_by_gene) == bool, "--color_by_gene does not take any arguments"
+        assert type(args.color_by_gene) == bool,   "--color_by_gene does not take any arguments"
     
     # if a reference, leftbound, and rightbound are applied
     update_bounds = False
     if args.seq_name != None:
         # check if leftbound & rightbound are provided in args
         if (("--leftbound" in sys.argv) == False) or (("--rightbound" in sys.argv) == False):
             # set to default for now, but will update later
-            args.leftbound = 1
+            args.leftbound  = 1
             args.rightbound = 50000
             update_bounds = True
+        
         assert args.rightbound > args.leftbound, "--rightbound must be greater than --leftbound"
-        assert args.leftbound >= 0, "--leftbound must be greater than or equal to 0"
+        assert args.leftbound >= 0,              "--leftbound must be greater than or equal to 0"
+        
         # only check now if we can
         if update_bounds == False:
             args.tick_count, args.tick_span = \
                 check_tick_params(args.tick_count, args.tick_span, args.leftbound, args.rightbound)
 
     # return args
     return args.klumps_tsv, args.color, args.fix_width, args.gap_file, args.klump_colors, \
@@ -74,15 +76,15 @@
 
 ######### parsing functions ############
 
 def parse_klumps_out(klump_file: str, SEQ_NAME: str, leftbound: int, rightbound: int, update_bounds: bool,
                      tick_count: int, tick_span: int):
     """get klump info per sequence or if specified, a particular locus"""
 
-    seq_klumps = {}
+    seq_klumps  = {}
     seq_lengths = {}
 
     fh = gzip.open(klump_file, "rt") if klump_file.endswith(".gz") else open(klump_file, 'r')
 
     for line in fh:
         if line[0] == '#':
             continue
@@ -121,17 +123,17 @@
                 continue
             if klmp.start_pos > rightbound:
                 continue
             # adjust to section
             if klmp.start_pos < leftbound:
                 klmp.start_pos = leftbound
             if klmp.end_pos > rightbound:
-                klmp.end_pos = rightbound
+                klmp.end_pos   = rightbound
             klmp.start_pos = int(klmp.start_pos - leftbound)
-            klmp.end_pos = int(klmp.end_pos - leftbound)
+            klmp.end_pos   = int(klmp.end_pos - leftbound)
         if seq not in seq_klumps:
             seq_klumps[seq] = [klmp]
         else:
             seq_klumps[seq].append(klmp)
     
     fh.close()
 
@@ -161,31 +163,32 @@
 
     fh = gzip.open(gap_file, "rt") if gap_file.endswith(".gz") else open(gap_file, 'r')
 
     for line in fh:
         fields = line.strip().split('\t')
         if fields[0] in seq_klumps:
             if SEQ_NAME == None:
-                seq = fields[0]
+                seq       = fields[0]
                 start_pos = int(fields[1])
-                end_pos = int(fields[2])
+                end_pos   = int(fields[2])
                 if seq not in gaps:
                     gaps[seq] = []
                 gaps[seq].append(GAP(start_pos, end_pos))
             else:   
                 #0-based positions
                 if leftbound <= int(fields[1]) <= rightbound or \
                     leftbound <= int(fields[2]) <= rightbound:
                     start_pos = int(fields[1])
-                    end_pos = int(fields[2])
+                    end_pos   = int(fields[2])
+
                     #just in case gap crosses boundaries                    
                     if start_pos < leftbound:
                         start_pos = leftbound
                     if end_pos > rightbound:
-                        end_pos = rightbound
+                        end_pos   = rightbound
                     if SEQ_NAME not in gaps:
                         gaps[SEQ_NAME] = []
                     gaps[SEQ_NAME].append(GAP(start_pos, end_pos))
 
     fh.close()
 
     return gaps
@@ -198,51 +201,50 @@
 
     # if img width is fixed, return
     if fix_width:
         return 150
 
     # adjust
     max_seq_length = max(list(seq_lengths.values()))
-    seq_length = seq_lengths[seq_name]
+    seq_length     = seq_lengths[seq_name]
 
     # longest seq starts in normal position
     if max_seq_length == seq_length:
         return 150
     else:
         # attempt to align the middles of each seq
         # idea:
         #       |-----|
         #    |-----------|
 
-        longer_half = max_seq_length/2
-        shorter_half = seq_length/2
+        longer_half   = max_seq_length/2
+        shorter_half  = seq_length/2
         allocated_pos = image_width / max_seq_length
 
         # find relative position of the longer seq
         adjusted_longer_half = 150 + (allocated_pos * longer_half)
         # make adjustment for seq
         adjusted_x = adjusted_longer_half - (shorter_half * allocated_pos)
         return adjusted_x
 
 
 def create_y_positions(seq_lengths: dict):
     """adjust pdf height for # of seqs"""
 
     # how many pixel are allocated per sequence
-    seq_space = 275
-    offset = 200
-
+    seq_space     = 275
+    offset        = 200
     figure_height = (len(seq_lengths)*seq_space) + offset
+    y_positions   = {}
 
-    y_positions = {}
     # reverse order to have longest seq at top
     sorted_seq_lengths = dict(sorted(seq_lengths.items(), key=lambda seq: seq[1], reverse=True))
 
     for i, seq in enumerate(sorted_seq_lengths):
-        y_pos = figure_height - offset - (i * seq_space)
+        y_pos            = figure_height - offset - (i * seq_space)
         y_positions[seq] = y_pos
 
     return figure_height, y_positions
 
 # TODO prevent overlapping between klump labels
 # def adjust_klump_labels(klumps_labels: dict, direction: str):
 #     """establish label positions to avoid overlapping labels"""
@@ -276,15 +278,15 @@
 ########## plotting functions #############
 
 
 def plot_seq(cairo_context, seq_lengths: dict, seq_id: str, allocated_positions: float,
               seq_height: float, x_pos: float, SEQ_NAME: str, leftbound: int, rightbound: int):
     """ plot sequence to scale to the longest sequence"""
     
-    sequence_id = seq_id
+    sequence_id   = seq_id
     allocated_pos = allocated_positions[seq_id]
 
     # starting positions
     x1 = x_pos  # offset from left by x position
     y1 = seq_height  # y / vertical offset
 
     # determine new x
@@ -382,15 +384,15 @@
         label_ypos = y_coordinate - 35 # 80
     elif orientation == "bottom":
         mark_ypos1 = y_coordinate + 13
         mark_ypos2 = y_coordinate + 23
         label_ypos = y_coordinate + 46 # this is the bottom of the text label
 
     if SEQ_NAME != None:
-        adjust = True
+        adjust  = True
         org_len = seq_len
         seq_len = rightbound - leftbound
     else:
         adjust = False
     
     # manual adjustment of ticks only when plotting a specific site
     if SEQ_NAME != None and tick_count != None:
@@ -519,38 +521,38 @@
                     color = klump_colors.get(ksource, org_color) # default to current color
                 fill_in_matches(cairo_context, y_coordinate, x_pos,
                                 allocated_pos, klump.start_pos, klump.end_pos, color)
 
                 # get direction to see if klump is on forward or reverse (currently alternating)
                 # create label & get dimensions
                 klump_size = klump.klump_size
-                query = klump.query_source
-                label = f"{klump_size}-{query}"
+                query      = klump.query_source
+                label      = f"{klump_size}-{query}"
                 # label_dim = cairo_context.text_extents(label)
                 # get the mid point of the text if i were not rotated
-                start_pos = x_pos + (klump.start_pos * allocated_pos)
-                end_pos = x_pos + (klump.end_pos * allocated_pos)
-                klump_midpoint = (end_pos + start_pos) / 2
+                start_pos                   = x_pos + (klump.start_pos * allocated_pos)
+                end_pos                     = x_pos + (klump.end_pos * allocated_pos)
+                klump_midpoint              = (end_pos + start_pos) / 2
                 midpoints[klump.klump_name] = (label, klump_midpoint)
 
     sorted_labels = [k for k,v in sorted(midpoints.items(), key = lambda item: item[1][1])]
 
     for i, k in enumerate(sorted_labels):
         direction = directions[i % 2]
         if direction == 'F':
             yLabel = y_coordinate + 42 # prev 30
-            angle = -45
+            angle  = -45
         elif direction == 'R':
             yLabel = y_coordinate + 90 # 105
-            angle = 45
+            angle  = 45
         # convert to radians
-        theta = math.radians(angle)
-        k_tuple = midpoints[k]
+        theta          = math.radians(angle)
+        k_tuple        = midpoints[k]
         klump_midpoint = k_tuple[1]
-        label = k_tuple[0]
+        label          = k_tuple[0]
         # create labels
         plot_label(cairo_context, yLabel, theta, label, klump_midpoint)
 
 
 def fill_in_matches(cairo_context, y: float, x_pos: float, allocated_pos: float, 
                     klump_start: int, klump_end: int, color):
     """fill in seq with klump positions"""
@@ -580,15 +582,15 @@
 
     y1 = y - 13 # starting on top of the seq
     y2 = y - 100 # move upwards by 160 pixels
 
     # adjust
     for gap in gaps_list:
         start_pos = x_pos + (gap.start_pos * allocated_pos)
-        end_pos = x_pos + (gap.end_pos * allocated_pos)
+        end_pos   = x_pos + (gap.end_pos   * allocated_pos)
         # mid point between start & end
         dash_start = start_pos + ((end_pos - start_pos)/2)
         cairo_context.set_line_width(end_pos - start_pos)
         cairo_context.set_dash([15.0, 5.0])
         cairo_context.move_to(dash_start, y1)
         cairo_context.line_to(dash_start, y2)
         cairo_context.set_source_rgb(0, 0, 0) # solid black to stand out
@@ -607,30 +609,30 @@
         ims = cairo.PDFSurface(output_name, figure_width, figure_height)
     elif outformat == "png":
         ims = cairo.ImageSurface(cairo.FORMAT_ARGB32, figure_width, figure_height)
     elif outformat == "svg":
         ims = cairo.SVGSurface(output_name, figure_width, figure_height)
 
     cairo_context = cairo.Context(ims)
-
-    image_width = figure_width - 400  # offset by starting positions on both sides
+    image_width   = figure_width - 400  # offset by starting positions on both sides
 
     # change length if needed
     if SEQ_NAME != None:
-        org_len = seq_lengths[SEQ_NAME]
+        org_len               = seq_lengths[SEQ_NAME]
         seq_lengths[SEQ_NAME] = rightbound - leftbound
 
     # get x positions
     x_positions = {}
     for seq in seq_lengths.keys():
         x_positions[seq] = adjust_x(image_width, seq, seq_lengths, fix_width)
 
     # create allocated posititions for sites
     max_seq_length = max(list(seq_lengths.values()))
-    allocated_pos = {}
+    allocated_pos  = {}
+
     for seq_id, seq_len in seq_lengths.items():
         # if img is fixed
         if fix_width:
             allocated_pos[seq_id] = \
                 ((image_width/max_seq_length) * max_seq_length) / seq_len
         else:
             # adjust
@@ -641,15 +643,15 @@
     for seq, seq_len in seq_lengths.items():
         plot_seq(cairo_context, seq_lengths, seq, allocated_pos, y_positions[seq],
                       x_positions[seq], SEQ_NAME, leftbound, rightbound)
         if SEQ_NAME == None:
             orientation = "top"
         else:
             orientation = "bottom"
-            seq_len = org_len
+            seq_len     = org_len
         draw_ticks(cairo_context, y_positions[seq], seq_len, image_width,
                     orientation, x_positions[seq], fix_width, max_seq_length,
                     SEQ_NAME, leftbound, rightbound, tick_count, tick_span)
         plot_klumps(cairo_context, y_positions[seq],
                     seq, allocated_pos, seq_klumps, x_positions[seq],
                     color, klump_colors, color_by_gene)
         # if gaps provided
@@ -693,15 +695,16 @@
 
     # check if using klump specific colors
     if klump_colors != None:
         klump_colors = parse_klump_color_list(klump_colors)
 
     # run the entire script
     if SEQ_NAME == None:
-        extension = str(klump_file).split(".")[-1]
+        extension   = str(klump_file).split(".")[-1]
         output_name = os.path.basename(klump_file).replace(extension, outformat)
     else:
         output_name = f"{SEQ_NAME}_{leftbound}-{rightbound}_klump_plot.{outformat}"
+        
     plot_seq_klumps(seq_lengths, seq_klumps, output_name, color, fix_width,
                     gaps, klump_colors, color_by_gene, SEQ_NAME, leftbound, rightbound,
                     outformat, tick_count, tick_span)
```

### Comparing `klumpy-1.0.5/klumpy/klump_sizes.py` & `klumpy-1.0.6/klumpy/klump_sizes.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 # along with Klumpy. If not, see <http://www.gnu.org/licenses/>.
 #
 
 
 import gzip
 import os
 import sys
-from .Classes import Seq_Record
+from  .Classes import Seq_Record
 
 def check_args(args):
     """verify that the arguments are legal and able to be used"""
 
     if args.fasta == None:
         msg = "No fasta input. Use --fasta"
         sys.exit(msg)
     assert os.path.isfile(args.fasta), f"Could not find {args.fasta}"
-    assert args.ksize > 0, "--ksize must be greater than 0"
+    assert args.ksize > 0,              "--ksize must be greater than 0"
 
     return args.fasta, args.ksize
 
 ########################
 ### Parsing functions ###
 ########################
 
@@ -46,34 +46,34 @@
 
     #
     # Read a gzipped file without any intervention.
     #
     if fasta_file.endswith(".gz"):
         fh = gzip.open(fasta_file, 'rt')
     else:
-        fh = open(fasta_file, "r")
+        fh = open(fasta_file, 'r')
 
-    seq = ""
-    id = None
+    seq = ''
+    id  = None
 
     for line in fh:
         # skip empty or commented lines
         if len(line) == 0 or line.startswith('#'):
             continue
         line = line.strip()
-        if line.startswith(">"):
+        if line.startswith('>'):
             # for the 1st record
-            if seq == "":
+            if seq == '':
                 id = line[1:].split(" ")[0]
                 continue
             else:
                 if len(seq) >= ksize:
                     records.append(Seq_Record(id, seq))
-                seq = ""
-                id = line[1:].split(" ")[0]
+                seq = ''
+                id  = line[1:].split(' ')[0]
         else:
             seq += line.upper()
 
     # for the last record
     if len(seq) >= ksize:
         records.append(Seq_Record(id, seq))
 
@@ -87,22 +87,22 @@
 ########################
 
 
 def print_to_console(records: list, ksize: int):
     """for each fasta record, print the kmer"""
 
     for record in records:
-        seq_id = record.seq_name
+        seq_id    = record.seq_name
         num_kmers = record.seq_length - ksize + 1
         print(f"{seq_id} length {record.seq_length}: Klump size of {num_kmers} k-mers")
 
 
 def Klump_Sizes(args):
     """Main entry point to this small subprogram"""
     # get arguments
 
     fasta, ksize = check_args(args)
 
     # load sequences
-    records = load_fasta_file(fasta, ksize)
+    records      = load_fasta_file(fasta, ksize)
 
     print_to_console(records, ksize)
```

### Comparing `klumpy-1.0.5/klumpy/kmerize.py` & `klumpy-1.0.6/klumpy/kmerize.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,39 +17,39 @@
 # along with Klumpy. If not, see <http://www.gnu.org/licenses/>.
 #
 
 
 import sys
 import gzip
 import os
-from collections import defaultdict
-from datetime import datetime
 import concurrent.futures
-from .Classes import Seq_Record
+from   collections import defaultdict
+from   datetime import datetime
+from  .Classes import Seq_Record
 
 def check_params(args):
     """do some assertions and checking for Nones"""
 
     warning_color = "\033[93m"
-    end_color = "\033[0m"
+    end_color     = "\033[0m"
 
     if args.subject == None:
         msg = "--subject is required for kmerize"
         sys.exit(msg)
     assert os.path.isfile(args.subject), f"Could not find {args.subject}"
     if args.query == None:
         msg = "--query is required for kmerize"
         sys.exit(msg)
     assert os.path.isfile(args.query), f"Could not find {args.query}"
      # check limit
     assert type(args.ksize) is int, "Ksize must be an integer"
-    assert args.ksize > 0, "Ksize must be greater than 0"
+    assert args.ksize > 0,          "Ksize must be greater than 0"
     # check limit
     assert type(args.limit) is int, "Limit value must be an integer"
-    assert args.limit > 0, "Limit must be greater than 0"
+    assert args.limit > 0,          "Limit must be greater than 0"
     #check thread number is appropriate
     assert type(args.threads) is int, "Threads value must be an integer"
     # check threads
     assert args.threads > 0, "--threads must be greater than 0"
     if args.threads > os.cpu_count():
         msg = f"Detected only {os.cpu_count()} threads. Reducing --threads count"
         print(f"{warning_color}{msg}{end_color}")
@@ -64,33 +64,29 @@
 ########################
 
 
 def load_fasta_file(fasta_file: str, limit: int, query_records: list, ksize: int, output_fh, 
                     record_cnt: int, hits: int, seq_cnt: int, query: bool, thread_num: int):
     """read fasta file in limited chunks"""
 
-    records = []
-
     #set up params
-    seq = ""
-    id = None
+    records = []
+    seq     = ''
+    id      = None
 
     # did the user explicitly add a limit?
-    if "--limit" not in sys.argv:
-        limit_checked = False
-    else:
-        limit_checked = True
+    limit_checked = ("--limit" in sys.argv)
 
     #
     # Read a gzipped file without any intervention.
     #
     if fasta_file.endswith(".gz"):
-        fh = gzip.open(fasta_file, 'rt')
+        fh = gzip.open(fasta_file, "rt")
     else:
-        fh = open(fasta_file, "r")
+        fh = open(fasta_file, 'r')
  
    #minus 1 to get last record
     for line in fh:
         # skip empty or commented lines
         if len(line) == 0 or line.startswith('#'):
             continue
         line = line.strip()
@@ -102,33 +98,33 @@
             else:
                 seq_len = len(seq)
                 # working with a genome or just records?
                 if (seq_len >= 1000000) and (limit_checked == False) and (limit > 3):
                     msg = "Detected sequneces of >= 1 MB. Reducing number of subject records " + \
                         "read into memory to 3 at a time"
                     print(msg)
-                    limit = 3
+                    limit         = 3
                     limit_checked = True
-                    thread_num = min(thread_num, 3) 
+                    thread_num    = min(thread_num, 3) 
                 if seq_len >= ksize:
                     records.append(Seq_Record(id, seq))
                 else:
                     print(f"Excluded {id} due to sequence length ({len(seq)}bp)")   
-                seq = ""
-                id = line[1:]
+                seq = ''
+                id  = line[1:]
                 if len(records) == limit:
                     record_cnt += len(records)
                     if record_cnt > 1:
                         s = "sequences"
                     else:
                         s = "sequence"
                     print(f"Loaded {record_cnt} {s} from {os.path.basename(fasta_file)}", end = "\r")
                     seq_cnt, matches = kmer_pipeline(records, query_records, ksize, 
                                                      output_fh, seq_cnt, thread_num)
-                    hits += matches
+                    hits   += matches
                     records = []
                 else:
                     pass
         else:
             seq += line.upper()
 
     # for the last record
@@ -139,19 +135,21 @@
     #process remaining seqs
     record_cnt = record_cnt + len(records)
     if record_cnt > 1:
         s = "sequences"
     else:
         s = "sequence"
     print(f"Loaded {record_cnt} {s} from {os.path.basename(fasta_file)}", end = "\r")
+    
     #need to return query before pipeline begins
     if query:
         return records
+    
     seq_cnt, matches = kmer_pipeline(records, query_records, ksize, output_fh, seq_cnt, thread_num)
-    hits += matches
+    hits            += matches
 
     return hits
 
     
 def load_fastq_file(fastq_file: str, limit: int, query_records: list, ksize: int, output_fh, 
                     record_cnt: int, hits: int, seq_cnt: int, query: bool, thread_num: int):
     """load fastq file in limited chunks as dict"""
@@ -160,66 +158,64 @@
     #set up variables
     records = [] #for multiple records
 
     #create file handle
     if fastq_file.endswith(".gz"):
         fh = gzip.open(fastq_file, "rt")
     else:
-        fh = open(fastq_file, "r")
+        fh = open(fastq_file, 'r')
 
     # assume legal fastq file
-    line_num = 0
-    seq_header = ""
+    line_num   = 0
+    seq_header = 'r'
     
     # same limit check as fasta function
-    if "--limit" not in sys.argv:
-        limit_checked = False
-    else:
-        limit_checked = True
+    limit_checked = ("--limit" in sys.argv)
 
     #begin reading
     for line in fh:
         if len(records) == limit:
             record_cnt += len(records)
             print(f"Loaded {record_cnt} sequences from {os.path.basename(fastq_file)}", end = "\r")
             seq_cnt, matches = kmer_pipeline(records, query_records,
                                              ksize, output_fh, seq_cnt,
                                              thread_num)
-            hits += matches
+            hits   += matches
             records = []
         #currently assumes fastq has no oddities
         if len(line) == 0:
             sys.exit(f"Please remove empty lines in {os.path.basename(fastq_file)}")
         line_num += 1
-        line = line.strip()
+        line      = line.strip()
         if line_num % 4 == 1 and line.startswith("@"):
             seq_header = line[1:]
         #4 lines = 1 record
         elif line_num % 4 == 2:
             seq_len = len(line)
             # same safety check here
             if (seq_len >= 1000000) and (limit_checked == False) and (limit > 3):
                 msg = "Detected sequneces of >= 1 MB. Reducing number of subject records " + \
                         "read into memory to 3 at a time"
                 print(msg)
-                limit = 3
+                limit         = 3
                 limit_checked = True
-                thread_num = min(thread_num, 3)  
+                thread_num    = min(thread_num, 3)  
             if seq_len >= ksize:
                 records.append(Seq_Record(seq_header, line))
             else:
                 print(f"Excluded {seq_header} due to a sequence length of ({seq_len}bp)")  
 
     fh.close()
 
     record_cnt += len(records)
     print(f"Loaded {record_cnt} sequences from {os.path.basename(fastq_file)}", end = "\r")
     #need to return query before pipeline begins
     if query:
         return records
+    
     seq_cnt, matches = kmer_pipeline(records, query_records,
                                      ksize, output_fh, seq_cnt,
                                      thread_num)
     hits += matches
     
     return hits
 
@@ -256,15 +252,15 @@
 
     file = os.path.basename(file)
 
     fasta_ext = ["fa", "fasta", "fna", "faa"]
     fastq_ext = ["fastq", "fq"]
 
     # in case format could not be determined
-    message = f"Could not determine file type for {os.path.basename(file)} using its file extension"
+    message   = f"Could not determine file type for {os.path.basename(file)} using its file extension"
 
     if file.endswith(".gz"):
         file_ext = file.split(".")[-2]
     else:
         file_ext = file.split(".")[-1]
     
     if file_ext in fasta_ext:
@@ -277,18 +273,18 @@
 def parse_query(query_records: list, ksize: int):
     """create query kmers"""
 
     #dict to separate different queries & orientations
     query_kmers = defaultdict(list)
 
     for record in query_records:
-        query_id = record.seq_name
-        query_seq = record.seq
-        query_seq_rc = record.seq_rc
-        seq_length = record.seq_length
+        query_id                     = record.seq_name
+        query_seq                    = record.seq
+        query_seq_rc                 = record.seq_rc
+        seq_length                   = record.seq_length
         query_kmers[f"{query_id}_F"] = build_kmers(query_seq, ksize, seq_length)
         #reverse kmer list for reverse kmers to have sorted output at the end
         query_kmers[f"{query_id}_R"] = build_kmers(query_seq_rc, ksize, seq_length)
 
     return query_kmers
 
 ##############################
@@ -309,15 +305,15 @@
 ### Kmer functions ###
 ########################
 
 
 def build_kmers(sequence: str, ksize: int, seq_length: int):
     """return a list of kmer objects or a set of kmers depending if it is query or subject"""
 
-    kmers = set()
+    kmers   = set()
     n_kmers = seq_length - ksize + 1
 
     for pos in range(n_kmers):
         kmer = sequence[pos:pos + ksize]
         kmers.add(kmer)
     
     # return the hash set of unique k-mers
@@ -337,27 +333,28 @@
             shared_kmers = query_kmers.intersection(subj_kmers)
 
             # if none shared, else
             if len(shared_kmers) == 0:
                 continue
             else:
                 orientation = query_id[-1:]
-                query_name = query_id[:-2]
+                query_name  = query_id[:-2]
                 #modify for easier parsing downstream
-                query_name = query_name.split(" ")[0].replace(":",";")
-                n_kmers = record.seq_length - ksize + 1
+                query_name  = query_name.split(" ")[0].replace(":",";")
+                n_kmers     = record.seq_length - ksize + 1
+
                 for pos in range(n_kmers):
                     kmer = record.seq[pos:pos + ksize]
                     if kmer in shared_kmers:
                         kmer_info += f"{pos} " + \
                                      f"{orientation} {query_name},"
 
-        if kmer_info != "":
+        if kmer_info != '':
             #check if paired end to keep info
-            seq_name = record.seq_name.split(" ")[0] #get rid of extra info
+            seq_name         = record.seq_name.split(" ")[0] #get rid of extra info
             paired, pair_num = record.check_if_paired_end()
             if paired:
                 seq_name = f"{seq_name}_PAIRED{pair_num}"
             # [:-1] to exclude last comma
             kmer_line = f"{seq_name} [{record.seq_length}]: {kmer_info[:-1]}\n"
             kmer_results.append(kmer_line)
 
@@ -370,16 +367,15 @@
 
 
 def kmer_pipeline(subject_records: list, query_records: list, ksize: int, output_fh, seq_cnt: int, thread_num: int):
     """function to run the pipeline on processing_seq_cnt of seq records"""
 
     # parse query
     query_kmers = parse_query(query_records, ksize)
-
-    matches = 0
+    matches     = 0
 
     if thread_num == 1:
         print() #spaceing b/t loaded print
         for record in subject_records:
             print(f"Processing sequence #{seq_cnt}", end='\r')
             seq_cnt += 1
             kmer_info = find_shared_kmers(query_kmers, [record], ksize)
@@ -392,15 +388,15 @@
         with concurrent.futures.ThreadPoolExecutor() as executor:
             # split records based on thread number
             thread_jobs = [executor.submit(find_shared_kmers, query_kmers,
                                             subject_records[i::thread_num],
                                             ksize) for i in range(thread_num)]
             # get results
             for thread_job in concurrent.futures.as_completed(thread_jobs):
-                results = thread_job.result()
+                results     = thread_job.result()
                 results_cnt = len(results)
                 if results_cnt != 0:
                     matches += results_cnt
                     for result in results:
                         output_fh.write(result)
                     output_fh.flush()
 
@@ -424,15 +420,15 @@
 
     # load query sequences
     query_records = load_query_records(query_file)
     print() #spacing b/t '\r' prints
 
     # create the coordinates file
     output_fh = create_file_handle(output)
-    command = "# klumpy " + \
+    command   = "# klumpy " + \
          " ".join("\"" + arg + "\"" if " " in arg else arg for arg in sys.argv[1:]) + '\n'
     output_fh.write(command)
     output_fh.write(f"# k-size: {ksize}\n")
     output_fh.write(f"# Starting time: {starting_time}\n")
     results_format = "# Sequence [Sequence Length]: " + \
                     "Kmer Position_in_Seq Orientation_in_Seq Query_Source\n"
     output_fh.write(results_format)
```

### Comparing `klumpy-1.0.5/klumpy/scan_alignments.py` & `klumpy-1.0.6/klumpy/scan_alignments.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,51 +19,52 @@
 
 import sys
 import gc
 import os
 import copy
 import multiprocessing
 import gzip
-from .Classes import SAM, SAM_FLAG, GENE, GeneRecord
+from  .Classes        import SAM, SAM_FLAG, GENE, GeneRecord
 from  .alignment_plot import estimate_seq_length, parse_cigar, group_assert, percent_check
-from .grouping import Group_Seqs, within_window
+from  .grouping       import Group_Seqs, within_window
+
 
 def clear_dict(map_dict: dict):
     """currently a temporary fix to remove possible circular references"""
 
     for v in map_dict.values():
         v.clear()
     map_dict.clear()
     map_dict = None # deallocate pointer
 
 ######### parsing functions ############
 
 def parse_sam_header(align_map: str, window_size: int, num_of_threads: int):
     """get the lengths of each ref seq in order to establish scanning scheme"""
 
-    ref_seqs = {} # will sort to run largest chroms 1st
+    ref_seqs      = {} # will sort to run largest chroms 1st
     ref_seqs_list = [] # for preserving initial order when writing
-    threads_list = [[] for _ in range(num_of_threads)]
+    threads_list  = [[] for _ in range(num_of_threads)]
 
     # just get the header
     cmd = f"samtools view -H {align_map}"
-    fh = os.popen(cmd, 'r')
+    fh  = os.popen(cmd, 'r')
 
     skip_cnt = 0
     total_bp = 0
 
     for line in fh:
         if line.startswith("@SQ"):
             # expected format:
             # @SQ\tSN:Seq_Name\tLN:Seq_Len
-            fields = line.strip('\n').split('\t')
+            fields   = line.strip('\n').split('\t')
             seq_name = fields[1]
             seq_name = seq_name.replace("SN:", '')
-            seq_len = fields[2]
-            seq_len = int(seq_len.replace("LN:", ''))
+            seq_len  = fields[2]
+            seq_len  = int(seq_len.replace("LN:", ''))
             if seq_len < window_size:
                 skip_cnt += 1
                 continue
             ref_seqs[seq_name] = seq_len
             total_bp += seq_len
             ref_seqs_list.append(seq_name)
     
@@ -118,15 +119,15 @@
     assert args.window_step > 0, "--window_step must be greater than 0"
     args.window_size = int(args.window_size)
     args.window_step = int(args.window_step)
 
     # if a gtf/gff3 is supplied, only report windows where a gene is found   
     if args.annotation != None:
         if os.path.isfile(args.annotation):
-            if (args.annotation.endswith(".gtf.gz")) or (args.annotation.endswith(".gtf")):
+            if (args.annotation.endswith(".gtf.gz"))   or (args.annotation.endswith(".gtf")):
                 pass
             elif (args.annotation.endswith(".gff.gz")) or (args.annotation.endswith(".gff")) or \
                 (args.annotation.endswith(".gff3.gz")) or (args.annotation.endswith(".gff3")):
                 pass
             else:
                 msg = f"No .gtf, .gtf.gz, .gff, .gff.gz, .gff3, or .gff3.gz file extension detected in {args.annotation}" + \
                     "\nAssuming proper input"
@@ -134,27 +135,29 @@
         else:
             sys.exit(f"Could not find {args.annotation}")
 
     # convert min_len to int
     args.min_len = int(args.min_len)
 
     # other params to verify
-    args.deletion_len = group_assert(args.deletion_len, "Deletion length")
-    args.align_offset = group_assert(args.align_offset, "Alignment Offset")
-    args.min_len = group_assert(args.min_len, "Minimum length")
+    args.deletion_len   = group_assert(args.deletion_len, "Deletion length")
+    args.align_offset   = group_assert(args.align_offset, "Alignment Offset")
+    args.min_len        = group_assert(args.min_len, "Minimum length")
     args.clip_tolerance = group_assert(args.clip_tolerance, "Clip tolerance")
-    args.del_tolerance = group_assert(args.del_tolerance, "Deletion tolerance")
-    args.t_len = group_assert(args.t_len, "Trustworthy length")
-    args.min_grp = group_assert(args.min_grp, "Minimum group")
-    assert args.limit >= 0, "--limit must be >= 0"
+    args.del_tolerance  = group_assert(args.del_tolerance, "Deletion tolerance")
+    args.t_len          = group_assert(args.t_len, "Trustworthy length")
+    args.min_grp        = group_assert(args.min_grp, "Minimum group")
+    args.num_of_groups  = group_assert(args.num_of_groups, "Number of groups")
+    assert args.limit  >= 0, "--limit must be >= 0"
     
     # check other boolean params
-    assert type(args.supplementary) is bool, "--supplementary does not taken any positional values"
-    assert type(args.secondary) is bool, "--secondary does not take any positional values"
-    assert type(args.assume_sep_del) is bool, "--assume_sep_del does not take any positional values"
+    assert type(args.supplementary)      is bool, "--supplementary does not taken any positional values"
+    assert type(args.secondary)          is bool, "--secondary does not take any positional values"
+    assert type(args.assume_sep_del)     is bool, "--assume_sep_del does not take any positional values"
+    assert type(args.flag_excess_groups) is bool, "--flag_excess_groups does not take any positional values"
 
     #check for percentages
     msg = "Minimum mapping"
     args.min_percent = percent_check(args.min_percent, msg)
     msg = "Minimum percent for trusting a sequence when grouping"
     args.t_per = percent_check(args.t_per, msg)
     msg = "Minimum percent for confidently grouping two sequences"
@@ -185,27 +188,28 @@
         msg = f"Detected only {os.cpu_count()} threads. Reducing --threads count"
         print(f"{warning_color}{msg}{end_color}")
         args.threads = os.cpu_count()
 
     return args.alignment_map, args.annotation, args.min_len, args.min_percent, \
            args.deletion_len, args.align_offset, args.clip_tolerance, args.t_len, args.t_per, \
            args.per_overlap, args.del_tolerance, args.assume_sep_del, args.min_grp, \
-           args.window_size, args.window_step, args.num_of_groups, args.threads, args.limit
+           args.window_size, args.window_step, args.num_of_groups, args.threads, args.limit, \
+           args.flag_excess_groups
 
 def get_genes(annotation: str, ref_lists: list):
     """return a dictionary of genes that will be used to only report windows of interest"""
 
     print(f"Parsing {annotation}")
 
     # check which fields will be sought for
 
     genome_genes = {}
     # will use a set to avoid duplciates
-    rec_types = ["gene", "mrna"]
-    visited = set()
+    rec_types    = ["gene", "mrna"]
+    visited      = set()
 
     # collapse the lists of lists to a single "list"
     ref_seqs = set()
     for ref_list in ref_lists:
         for ref_tuple in ref_list:
             ref_seqs.add(ref_tuple[0])
 
@@ -222,16 +226,16 @@
         chr = fields[0]
         # only keep genes for seqs being scanned
         if chr not in ref_seqs:
             continue
         if fields[2].lower() in rec_types:
             chr = fields[0]
             # ignoring direction for window scanning
-            start = int(fields[3])
-            end = int(fields[4])
+            start     = int(fields[3])
+            end       = int(fields[4])
             direction = fields[6]
             if (start, end, direction) in visited:
                 continue
             visited.add((start, end, direction))
             gene_record.parse_attributes(fields[8])
             gene_name = gene_record.get_gene_name()
             gene = GENE(start, end, gene_name)
@@ -269,91 +273,106 @@
         
     return genes
 
 def process_window(alignments: dict, window_start: int, window_end: int, ref: str, 
                    align_offset: int, clip_tolerance: int, del_tol: int, per_overlap: float,
                    t_len: int, t_per: float, group_dels: bool, min_grp: int, 
                    num_of_groups: int, using_genes: bool, chr_genes: list, 
-                   limit: int, outfh):
+                   limit: int, flag_excess_groups: bool, outfh):
     """will determine if the current window will be written to output"""
 
     # assume we will group the sequences
     will_group = True
 
     if using_genes: # if only reporting regions with genes
         if chr_genes != None:
             genes = genes_in_window(window_start, window_end, chr_genes)
             if len(genes) == 0:
                 will_group = False # no genes here
         else:
             will_group = False # no genes in this ref seq
     
     if will_group: # okay-ed to group
-        missassembled = Group_Seqs(alignments, window_start, window_end, ref, align_offset,
+        group_count = Group_Seqs(alignments, window_start, window_end, ref, align_offset,
                                    clip_tolerance, del_tol, per_overlap, False,
                                    {}, t_len, t_per, group_dels, False, min_grp, False,
-                                   limit, True, num_of_groups)
-        if missassembled: # true is no tiling was created
-            endl = '\n'
+                                   limit, True)
+ 
+        # not able to be tiled or if reporting regions with >N groups
+        if (group_count < 0 or (flag_excess_groups and abs(group_count) >= num_of_groups)):
+            group_count = abs(group_count)
+            endl  = '\n'
+            
             if using_genes:
                 # add genes to outline
-                endl = '\t' + ','.join(genes) + '\n'
+                endl = '\t' + ','.join(genes) + '\n' 
+
+            if (flag_excess_groups):
+                tiled = 'F' if (group_count < 0) else 'T'
+                outline = f"{ref}\t{window_start}\t{window_end}\t{tiled}\t{group_count}{endl}"
+            else:
+                outline = f"{ref}\t{window_start}\t{window_end}\t{group_count}{endl}"
+
             # assume file handle is open
             try:
-                outfh.write(f"{ref}\t{window_start}\t{window_end}{endl}")
+                outfh.write(outline)
                 outfh.flush() 
             except:
                 # open file
                 outfh = open(f"Temp_{ref}.txt", 'w')
-                outfh.write(f"{ref}\t{window_start}\t{window_end}{endl}")
+                outfh.write(outline)
                 outfh.flush() 
 
     # return it just in case
     return outfh
 
 def scan_align_map(align_map: str, ref_list: list, window_size: int, window_step: int,
                    min_len: int, min_percent: float, limit: int, deletion_len: int,
                    min_grp: int, num_of_groups: int, align_offset: int, clip_tolerance: int, 
                    del_tol: int, per_overlap: float, t_len: int, t_per: int, group_dels: bool,
-                   using_genes: bool, ref_genes: dict):
+                   using_genes: bool, flag_excess_groups: bool, ref_genes: dict):
     """go through the alignment bam and look for regions that may be missassembled"""
 
     for ref_tuple in ref_list:
-        ref = ref_tuple[0]
+        ref     = ref_tuple[0]
         ref_len = ref_tuple[1]
         # delete previous temps if they are still present
         if os.path.isfile(f"Temp_{ref}.txt"):
             os.remove(f"Temp_{ref}.txt")
         if using_genes:
             chr_genes = ref_genes[ref] # get the genes once
         else:
             chr_genes = None
-        outfh = None # only open file if missassembled region found
-        tmp = None # will be used to hold next window sam records
-        window_start = 0
-        window_end = window_size + 0
-        cmd = f"samtools view {align_map} " + f'"{ref}' + '"'
-        alignments = {}
+        
+        # set up the parameters
+        outfh            = None # only open file if missassembled region found
+        tmp              = None # will be used to hold next window sam records
+        window_start     = 0
+        window_end       = window_size + 0
+        cmd              = f"samtools view {align_map} " + f'"{ref}' + '"'
+        alignments       = {}
         next_window_seqs = list()
         fh = os.popen(cmd, 'r')
 
         # now go in and slide through the alignments
         for line in fh:
+            if window_start == 4800000:
+                fff = copy.deepcopy(alignments)
             if line.startswith('@'):
                 continue
             fields = line.strip('\n').split('\t')
             seq_name = fields[0]
             seq_flag = int(fields[1])
             sam_flag = SAM_FLAG(seq_flag)
             # only primary seqs are used for grouping
             if not sam_flag.primary:
                 continue
-            seq_cigar = fields[5]
+            seq_cigar    = fields[5]
             leftmost_pos = int(fields[3])
-            seq_length = estimate_seq_length(seq_cigar)
+            seq_length   = estimate_seq_length(seq_cigar)
             # filtering for unreliable alignments is still applied
             if seq_length < min_len:
                 continue
             align_len, clipping_start, adjust_start, clipping_end, \
                 adjust_end, align_blocks = parse_cigar(seq_cigar, deletion_len)
             if adjust_start == None:
                 clipped_start = 0
@@ -373,93 +392,120 @@
             sam_record = SAM(seq_name, leftmost_pos, seq_flag, ref, segment,
                             align_blocks, clipping_start, adjust_start,
                             clipping_end, adjust_end, percent_aligned, seq_length,
                             sam_flag.primary)
 
             # determine if in current & next window
             next_start = window_start + window_step
-            next_end = window_end + window_step
+            next_end   = window_end   + window_step
             in_current = within_window(leftmost_pos, align_blocks, window_start,
                                        window_end, clipped_start)
-            in_next = within_window(leftmost_pos, align_blocks, next_start, 
-                                    next_end, clipped_start)
-
+            in_next    = within_window(leftmost_pos, align_blocks, next_start, 
+                                       next_end, clipped_start)
             if in_current and in_next:
                 # keeping in list to make grouping functions combatible
                 # with scanning pipeline
                 alignments[seq_name] = [sam_record] # keeping in list
                 next_window_seqs.append(seq_name)
             elif in_current:
                 alignments[seq_name] = [sam_record]
             elif in_next and not in_current:
+ 
                 # now do the grouping here
                 if len(alignments) >= min_grp and len(alignments) > 0:
-                    # save next windows in a temp dict b/c limit can be trigged, and remove
-                    # next window alignments
-                    tmp = {s:v for s,v in alignments.items() if s in next_window_seqs}
                     outfh = process_window(alignments, window_start, window_end, ref, align_offset,
                                            clip_tolerance, del_tol, per_overlap, t_len, t_per,
                                            group_dels, min_grp, num_of_groups, using_genes, chr_genes,
-                                           limit, outfh)
+                                           limit, flag_excess_groups, outfh)
  
-                    # after processing window, move on
+                # save next windows in a temp dict b/c limit can be trigged, and remove
+                # next window alignments
+                if len(next_window_seqs) > 0:                
+                    tmp        = {s:v for s,v in alignments.items() if s in next_window_seqs} 
                     alignments = copy.deepcopy(tmp)
                     clear_dict(tmp)
-                    alignments[seq_name] = [sam_record]
-                    window_start += window_step
-                    window_end += window_step
                     next_window_seqs.clear()
-                    # just in case
-                    next_s = window_start + window_step
-                    next_e = window_end + window_step
-                    for seq in alignments:
-                        sr = alignments[seq][0]
-                        if sr.adjust_start == None:
-                            clipped_start = 0
-                        else:
-                            clipped_start = sr.adjust_start
-                        if within_window(sr.position, sr.align_blocks, next_s, next_e, clipped_start):
-                            next_window_seqs.append(seq)
+                else:
+                    clear_dict(alignments)
+                
+                # start refilling the alignments again
+                alignments[seq_name] = [sam_record]
+                window_start += window_step
+                window_end   += window_step
+
+                next_s = window_start + window_step
+                next_e = window_end   + window_step
+                for seq in alignments:
+                    sr = alignments[seq][0]
+                    if sr.adjust_start == None:
+                        clipped_start = 0
+                    else:
+                        clipped_start = sr.adjust_start
+                    if within_window(sr.position, sr.align_blocks, next_s, next_e, clipped_start):
+                        next_window_seqs.append(seq)
+
             elif not in_current and not in_next:
+                
                 if len(alignments) >= min_grp and len(alignments) > 0:
+                    # process current alignments
                     outfh = process_window(alignments, window_start, window_end, ref, align_offset,
                                            clip_tolerance, del_tol, per_overlap, t_len, t_per,
                                            group_dels, min_grp, num_of_groups, using_genes, chr_genes,
-                                           limit, outfh)
-
+                                           limit, flag_excess_groups, outfh)
                 # clear current containers just in case
-                clear_dict(alignments)
-                next_window_seqs.clear()
+                if (len(next_window_seqs) > 0):
+                    start_tmp = next_start
+                    end_tmp   = next_end
+                    alignments = {k:v for k, v in alignments.items() if k in next_window_seqs}
+                    next_window_seqs.clear()
+                else:
+                    start_tmp = None
+                    end_tmp   = None
+                    clear_dict(alignments)
                 # slide over to the next window
                 while (in_current == False):
                     attempts = 0
                     window_start += window_step
                     window_end += window_step
                     in_current = within_window(leftmost_pos, align_blocks, window_start,
                                        window_end, clipped_start)
                     # should not happen, but just in case, start over and move forward
                     if window_start > ref_len:
                         if attempts == 1:
                             break
                         window_start = 0
-                        window_end = 0 + window_step
-                        attempts += 1
+                        window_end   = 0 + window_size
+                        attempts    += 1
+                # check if we are at a different window
+                if len(alignments) >= min_grp and len(alignments) > 0 and start_tmp != window_start:
+                    outfh = process_window(alignments, start_tmp, end_tmp, ref, align_offset,
+                                           clip_tolerance, del_tol, per_overlap, t_len, t_per,
+                                           group_dels, min_grp, num_of_groups, using_genes, chr_genes,
+                                           limit, flag_excess_groups, outfh)
+                elif (len(alignments) < min_grp) and (start_tmp != window_start):
+                    clear_dict(alignments)
                 alignments[seq_name] = [sam_record]
                 next_start = window_start + window_step
-                next_end = window_end + window_step
+                next_end   = window_end + window_step
                 # still on the same record
-                if within_window(leftmost_pos, align_blocks, next_start, next_end, clipped_start):
-                    next_window_seqs.append(seq_name)
+                for seq in alignments:
+                        sr = alignments[seq][0]
+                        if sr.adjust_start == None:
+                            clipped_start = 0
+                        else:
+                            clipped_start = sr.adjust_start
+                        if within_window(sr.position, sr.align_blocks, next_s, next_e, clipped_start):
+                            next_window_seqs.append(seq)
         fh.close()
         # check for last remaining seqs (a just in case situation)
         if len(alignments) >= min_grp and len(alignments) > 0:
             outfh = process_window(alignments, window_start, window_end, ref, align_offset,
                                            clip_tolerance, del_tol, per_overlap, t_len, t_per,
                                            group_dels, min_grp, num_of_groups, using_genes, chr_genes,
-                                           limit, outfh)
+                                           limit, flag_excess_groups, outfh)
 
         # remove any remaining data
         clear_dict(alignments)
         next_window_seqs.clear()
         if tmp != None:
             clear_dict(tmp) # dict created
 
@@ -479,34 +525,74 @@
     next_genes = next_window[2].split(',')
     for gene in next_genes:
         if gene not in current_genes:
             current_genes.append(gene)
 
     return ','.join(current_genes)
 
-def combine_scan_results(ref_seqs: list, align_map: str, window_step: int, using_genes: bool):
+
+def combine_columns(current_window: list, next_window: list, using_genes: bool, flag_excess_groups: bool):
+    """combine the tile, number of groups, and gene (if present) columns"""
+
+    new_window = [current_window[0], current_window[1]]
+
+
+    if (flag_excess_groups):
+        # add tile column
+        new_window.append(current_window[2] + ',' + next_window[2])
+
+        # add number of groups column
+        new_window.append(current_window[3] + ',' + next_window[3])
+
+        if (using_genes):
+            current_genes = current_window[4].split(',')
+            next_genes    = next_window[4].split(',')
+            for gene in next_genes:
+                if gene not in current_genes:
+                    current_genes.append(gene)
+            new_window.append(','.join(current_genes))
+    else:
+        # repeated code - TODO
+        new_window.append(current_window[2] + ',' + next_window[2])
+
+        if (using_genes):
+            current_genes = current_window[3].split(',')
+            next_genes    = next_window[3].split(',')
+            for gene in next_genes:
+                if gene not in current_genes:
+                    current_genes.append(gene)
+            new_window.append(','.join(current_genes))
+
+    
+    return new_window
+
+
+def combine_scan_results(ref_seqs: list, align_map: str, window_step: int, using_genes: bool, flag_excess_groups: bool):
     """combine the Temp results into a single file"""
 
     printed = False
 
     # create output file
     align_map_name = os.path.basename(align_map)
     if align_map_name.endswith(".gz"):
         ext_cnt = 2
     else:
         ext_cnt = 1
     outname = '.'.join(align_map_name.split('.')[:-ext_cnt])
     outname = outname + "_Candidate_Regions.tsv"
-    outfh = open(outname, 'w')
+    outfh   = open(outname, 'w')
     # write command & header
     # store arguments to tsv file
     command = "# klumpy " + \
          " ".join("\"" + arg + "\"" if " " in arg else arg for arg in sys.argv[1:]) + '\n'
     outfh.write(command)
-    header = "Region_Number\tReference_Seq\tStart\tEnd"
+    if (flag_excess_groups):
+        header = "Region_Number\tReference_Seq\tStart\tEnd\tTiled\tNumber_of_Groups"
+    else:
+        header = "Region_Number\tReference_Seq\tStart\tEnd\tNumber_of_Groups"
     if using_genes:
         header = header + "\tGenes"
     outfh.write(header + '\n')
 
     region_cnt = 0 # used to track number of regions
     ref_count = 0 # used to track number of ref seqs
 
@@ -526,24 +612,27 @@
                         current_start = int(current_window[0])
                         current_end = int(current_window[1])
                         next_window = line.strip('\n').split('\t')[1:]
                         next_start = int(next_window[0])
                         next_end = int(next_window[1])
                         if current_start + window_step == next_start:
                             current_window[1] = next_end
-                            if using_genes:
-                                current_window[2] = merge_genes(current_window, next_window)
+                            current_window = combine_columns(current_window, next_window, using_genes, flag_excess_groups)
+                            # if using_genes:
+                            #     current_window[2] = merge_genes(current_window, next_window)
                         elif current_end + window_step == next_end:
                             current_window[1] = next_end
-                            if using_genes:
-                                current_window[2] = merge_genes(current_window, next_window)
+                            current_window = combine_columns(current_window, next_window, using_genes, flag_excess_groups)
+                            # if using_genes:
+                            #     current_window[2] = merge_genes(current_window, next_window)
                         elif current_end >= next_start:
                             current_window[1] = next_end
-                            if using_genes:
-                                current_window[2] = merge_genes(current_window, next_window)
+                            current_window = combine_columns(current_window, next_window, using_genes, flag_excess_groups)
+                            # if using_genes:
+                            #     current_window[2] = merge_genes(current_window, next_window)
                         else:
                             # write to outfh
                             region_cnt += 1
                             outline = f"{region_cnt}\t{seq}\t" + '\t'.join([str(v) for v  in current_window]) + '\n'
                             outfh.write(outline)
                             outfh.flush()
                             current_window = next_window                
@@ -560,16 +649,16 @@
 
 def Scan_Alignments(args):
     """Scan through a SAM/BAM file and find possible misassemblied regions"""
 
     # get arguments
     align_map, annotation, min_len, percent, deletion_len, align_offset, \
     clip_tolerance, t_len, t_per, per_overlap, del_tolerance, group_dels, \
-    min_grp, window_size, window_step, num_of_groups, num_of_threads, limit \
-        = check_args(args)
+    min_grp, window_size, window_step, num_of_groups, num_of_threads, limit, \
+    flag_excess_groups    = check_args(args)
 
      # first, get the ref IDs to only analyze seqs >= window size
     ref_seqs, ref_seqs_list = parse_sam_header(align_map, window_size, num_of_threads)
 
     # check if we are using a gtf file
     if annotation != None:
         genome_genes = get_genes(annotation, ref_seqs)
@@ -577,15 +666,16 @@
     else:
         genome_genes = {}
         using_genes = False
 
     # put args into a list that will serve as an agruements list
     scan_args = [align_map, window_size, window_step, min_len, percent, limit,
                 deletion_len, min_grp, num_of_groups, align_offset, clip_tolerance,
-                del_tolerance, per_overlap, t_len, t_per, group_dels, using_genes]
+                del_tolerance, per_overlap, t_len, t_per, group_dels, using_genes, 
+                flag_excess_groups]
     
     # if not multi-processing
     if num_of_threads == 1:
         ref_list = ref_seqs[0]
         ref_genes = {}
         if using_genes:
             tmp = []
@@ -619,9 +709,9 @@
             processes.append(proc)
         for proc in processes:
             proc.join()
         processes.clear()
 
     
     # now clean up
-    combine_scan_results(ref_seqs_list, align_map, window_step, using_genes)
+    combine_scan_results(ref_seqs_list, align_map, window_step, using_genes, flag_excess_groups)
```

### Comparing `klumpy-1.0.5/setup.py` & `klumpy-1.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", 'r') as fh:
     description = fh.read()
 
-setup(name="klumpy", version="1.0.5", packages=find_packages(),
-      python_requires=">=3.6.0", install_requires=["pycairo"],
+setup(name="klumpy",
+      version="1.0.6",
+      packages=find_packages(),
+      python_requires=">=3.6.0", 
+      install_requires=["pycairo"],
       description="A package to evaluate genome assemblies and detect sequence motifs",
-      long_description=description, long_description_content_type="text/markdown",
-      author_email="gm33@illinois.edu", classifiers=["Programming Language :: Python :: 3","Operating System :: POSIX",
-                                                     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"],
+      long_description=description,
+      long_description_content_type="text/markdown",
+      author_email="gm33@illinois.edu",
+      classifiers=["Programming Language :: Python :: 3","Operating System :: POSIX", "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"],
       author="Giovanni Madrigal <gm33@illinois.edu>, Bushra Fazal Minhas <bfazal2@illinois.edu>, Julian Catchen <jcatchen@illinois.edu>",
       scripts=["scripts/klumpy"])
```

