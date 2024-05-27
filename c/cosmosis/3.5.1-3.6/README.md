# Comparing `tmp/cosmosis-3.5.1.tar.gz` & `tmp/cosmosis-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmosis-3.5.1.tar", last modified: Tue Jan  9 10:00:41 2024, max compression
+gzip compressed data, was "cosmosis-3.6.tar", last modified: Mon May 27 11:19:08 2024, max compression
```

## Comparing `cosmosis-3.5.1.tar` & `cosmosis-3.6.tar`

### file list

```diff
@@ -1,290 +1,292 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.286813 cosmosis-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-01-09 10:00:38.000000 cosmosis-3.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-01-09 10:00:38.000000 cosmosis-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-01-09 10:00:41.286813 cosmosis-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-09 10:00:38.000000 cosmosis-3.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.246813 cosmosis-3.5.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-01-09 10:00:38.000000 cosmosis-3.5.1/bin/cosmosis
--rwxr-xr-x   0 runner    (1001) docker     (127)      122 2024-01-09 10:00:38.000000 cosmosis-3.5.1/bin/cosmosis-campaign
--rwxr-xr-x   0 runner    (1001) docker     (127)      792 2024-01-09 10:00:38.000000 cosmosis-3.5.1/bin/cosmosis-configure
--rwxr-xr-x   0 runner    (1001) docker     (127)     1434 2024-01-09 10:00:38.000000 cosmosis-3.5.1/bin/cosmosis-extract
--rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-01-09 10:00:38.000000 cosmosis-3.5.1/bin/cosmosis-postprocess
--rwxr-xr-x   0 runner    (1001) docker     (127)     1527 2024-01-09 10:00:38.000000 cosmosis-3.5.1/bin/cosmosis-sample-fisher
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.246813 cosmosis-3.5.1/cosmosis/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21426 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/campaign.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.250813 cosmosis-3.5.1/cosmosis/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/config/compilers.mk
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/config/subdirs.mk
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.254813 cosmosis-3.5.1/cosmosis/datablock/
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51706 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/c_datablock.cc
--rw-r--r--   0 runner    (1001) docker     (127)    22811 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/c_datablock.h
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/clamp.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/cosmosis_constants.fh
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/cosmosis_constants.h
--rw-r--r--   0 runner    (1001) docker     (127)    34029 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/cosmosis_modules.F90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.254813 cosmosis-3.5.1/cosmosis/datablock/cosmosis_py/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/cosmosis_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52767 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/cosmosis_py/block.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/cosmosis_py/dbt_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/cosmosis_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/cosmosis_py/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/cosmosis_py/section_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/cosmosis_section_names.F90
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/cosmosis_types.F90
--rw-r--r--   0 runner    (1001) docker     (127)    28871 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/cosmosis_wrappers.F90
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/datablock.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/datablock.hh
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/datablock_logging.cc
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/datablock_logging.h
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/datablock_status.h
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/datablock_types.h
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/entry.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/entry.hh
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/exceptions.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/generate_sections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/handler.c
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/ndarray.hh
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/section.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/section.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/section_names.h
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/datablock/section_names.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/gaussian_likelihood.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22952 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.254813 cosmosis-3.5.1/cosmosis/output/
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/output/astropy_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/output/cosmomc_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/output/fits_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/output/in_memory_output.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/output/null_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/output/output_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/output/text_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/output/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.258813 cosmosis-3.5.1/cosmosis/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/plotting/chain_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/plotting/grid_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/plotting/kde.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/plotting/plot_demo_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/plotting/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/plotting/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5502 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.258813 cosmosis-3.5.1/cosmosis/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/postprocessing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16175 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/postprocessing/cosmology_theory_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/postprocessing/density.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/postprocessing/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/postprocessing/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/postprocessing/latex.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/postprocessing/lazy_pylab.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/postprocessing/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/postprocessing/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    50319 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/postprocessing/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/postprocessing/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/postprocessing/postprocess_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/postprocessing/reruns.py
--rw-r--r--   0 runner    (1001) docker     (127)    33609 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/postprocessing/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/postprocessing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.262813 cosmosis-3.5.1/cosmosis/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    13893 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/declare.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.262813 cosmosis-3.5.1/cosmosis/runtime/julia_modules/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/julia_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/julia_modules/julia.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/memmon.py
--rw-r--r--   0 runner    (1001) docker     (127)    17170 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/mpi_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    58624 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    21210 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/prior.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/process_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.262813 cosmosis-3.5.1/cosmosis/samplers/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.262813 cosmosis-3.5.1/cosmosis/samplers/abc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/abc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7126 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/abc/abc_sampler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6698 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/abc/abc_sampler_mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.266813 cosmosis-3.5.1/cosmosis/samplers/apriori/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/apriori/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2766 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/apriori/apriori_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.266813 cosmosis-3.5.1/cosmosis/samplers/dynesty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/dynesty/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3707 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/dynesty/dynesty_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.266813 cosmosis-3.5.1/cosmosis/samplers/emcee/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/emcee/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7516 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/emcee/emcee_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.266813 cosmosis-3.5.1/cosmosis/samplers/fisher/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/fisher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/fisher/fisher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6642 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/fisher/fisher_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.266813 cosmosis-3.5.1/cosmosis/samplers/grid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/grid/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4745 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/grid/grid_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.266813 cosmosis-3.5.1/cosmosis/samplers/gridmax/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/gridmax/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4370 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/gridmax/gridmax_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/hints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.266813 cosmosis-3.5.1/cosmosis/samplers/importance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/importance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/importance/importance_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.266813 cosmosis-3.5.1/cosmosis/samplers/kombine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/kombine/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4932 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/kombine/kombine_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.266813 cosmosis-3.5.1/cosmosis/samplers/list/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/list/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5094 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/list/list_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.266813 cosmosis-3.5.1/cosmosis/samplers/maxlike/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/maxlike/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4666 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/maxlike/maxlike_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.266813 cosmosis-3.5.1/cosmosis/samplers/metropolis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/metropolis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/metropolis/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/metropolis/metropolis_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.270813 cosmosis-3.5.1/cosmosis/samplers/metropolis/proposal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/metropolis/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/metropolis/proposal/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.270813 cosmosis-3.5.1/cosmosis/samplers/minuit/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/minuit/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/minuit/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7323 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/minuit/minuit_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/minuit/minuit_wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.270813 cosmosis-3.5.1/cosmosis/samplers/multinest/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/multinest/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/multinest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.270813 cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/README
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/cwrapper.f90
--rw-r--r--   0 runner    (1001) docker     (127)    42915 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90
--rw-r--r--   0 runner    (1001) docker     (127)   107766 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/nested.f90
--rw-r--r--   0 runner    (1001) docker     (127)    22010 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/posterior.f90
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/priors.f90
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/utils.f90
--rw-r--r--   0 runner    (1001) docker     (127)    28039 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/utils1.f90
--rw-r--r--   0 runner    (1001) docker     (127)    86938 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.274813 cosmosis-3.5.1/cosmosis/samplers/nautilus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/nautilus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/nautilus/nautilus_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.274813 cosmosis-3.5.1/cosmosis/samplers/pmaxlike/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/pmaxlike/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4151 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.274813 cosmosis-3.5.1/cosmosis/samplers/pmc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/pmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/pmc/pmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/pmc/pmc_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.274813 cosmosis-3.5.1/cosmosis/samplers/poco/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/poco/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3703 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/poco/poco_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.274813 cosmosis-3.5.1/cosmosis/samplers/polychord/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12986 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.278813 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/README
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/abort.F90
--rw-r--r--   0 runner    (1001) docker     (127)    18110 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/array_utils.f90
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/c_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/calculate.f90
--rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90
--rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/clustering.f90
--rw-r--r--   0 runner    (1001) docker     (127)    13421 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/feedback.f90
--rw-r--r--   0 runner    (1001) docker     (127)    26147 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/generate.F90
--rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/ini.f90
--rw-r--r--   0 runner    (1001) docker     (127)    20999 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/interfaces.F90
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/interfaces.h
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/interfaces.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    24257 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90
--rw-r--r--   0 runner    (1001) docker     (127)    20674 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/params.f90
--rw-r--r--   0 runner    (1001) docker     (127)    19675 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/priors.f90
--rw-r--r--   0 runner    (1001) docker     (127)    18291 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/random_utils.F90
--rw-r--r--   0 runner    (1001) docker     (127)    44750 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/read_write.f90
--rw-r--r--   0 runner    (1001) docker     (127)    47427 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/run_time_info.f90
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/settings.f90
--rw-r--r--   0 runner    (1001) docker     (127)    29353 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/utils.F90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.278813 cosmosis-3.5.1/cosmosis/samplers/pymc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/pymc/pymc_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.278813 cosmosis-3.5.1/cosmosis/samplers/snake/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/snake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/snake/snake.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2017 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/snake/snake_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.278813 cosmosis-3.5.1/cosmosis/samplers/star/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/star/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4468 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/star/star_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.278813 cosmosis-3.5.1/cosmosis/samplers/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3221 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/test/test_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.278813 cosmosis-3.5.1/cosmosis/samplers/zeus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/zeus/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11554 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/samplers/zeus/zeus_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.282813 cosmosis-3.5.1/cosmosis/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/campaign.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/example-priors.ini
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/example-values.ini
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/example.ini
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/example_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/example_module2.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/example_module3.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/example_module4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.286813 cosmosis-3.5.1/cosmosis/test/libtest/
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/libtest/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/libtest/c_datablock_complex_array_test.c
--rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/libtest/c_datablock_double_array_test.c
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/libtest/c_datablock_int_array_test.c
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c
--rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/libtest/c_datablock_test.c
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/libtest/cosmosis_test.F90
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/libtest/cosmosis_tests.supp
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/libtest/datablock_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/libtest/entry_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/libtest/ndarray_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/libtest/section_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)    28088 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/libtest/test_c_datablock_scalars.h
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/libtest/test_c_datablock_scalars.template
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/test_campaign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/test_chaining.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/test_polychord.py
--rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/test_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/test_text_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-09 10:00:38.000000 cosmosis-3.5.1/cosmosis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 10:00:41.286813 cosmosis-3.5.1/cosmosis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-01-09 10:00:41.000000 cosmosis-3.5.1/cosmosis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9220 2024-01-09 10:00:41.000000 cosmosis-3.5.1/cosmosis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 10:00:41.000000 cosmosis-3.5.1/cosmosis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-09 10:00:41.000000 cosmosis-3.5.1/cosmosis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-09 10:00:41.000000 cosmosis-3.5.1/cosmosis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-09 10:00:38.000000 cosmosis-3.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 10:00:41.286813 cosmosis-3.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-01-09 10:00:38.000000 cosmosis-3.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.974270 cosmosis-3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-27 11:19:03.000000 cosmosis-3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-27 11:19:03.000000 cosmosis-3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-27 11:19:08.974270 cosmosis-3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 11:19:03.000000 cosmosis-3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.930270 cosmosis-3.6/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-27 11:19:03.000000 cosmosis-3.6/bin/cosmosis
+-rwxr-xr-x   0 runner    (1001) docker     (127)      122 2024-05-27 11:19:03.000000 cosmosis-3.6/bin/cosmosis-campaign
+-rwxr-xr-x   0 runner    (1001) docker     (127)      792 2024-05-27 11:19:03.000000 cosmosis-3.6/bin/cosmosis-configure
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1434 2024-05-27 11:19:03.000000 cosmosis-3.6/bin/cosmosis-extract
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-27 11:19:03.000000 cosmosis-3.6/bin/cosmosis-postprocess
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1527 2024-05-27 11:19:03.000000 cosmosis-3.6/bin/cosmosis-sample-fisher
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.934270 cosmosis-3.6/cosmosis/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26386 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/campaign.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.934270 cosmosis-3.6/cosmosis/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/config/compilers.mk
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/config/subdirs.mk
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.938270 cosmosis-3.6/cosmosis/datablock/
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51706 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/c_datablock.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    22811 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/c_datablock.h
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/clamp.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_constants.fh
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34029 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_modules.F90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.942270 cosmosis-3.6/cosmosis/datablock/cosmosis_py/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52767 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_py/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_py/dbt_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_py/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_py/section_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_section_names.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_types.F90
+-rw-r--r--   0 runner    (1001) docker     (127)    28871 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/cosmosis_wrappers.F90
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/datablock.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/datablock.hh
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/datablock_logging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/datablock_logging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/datablock_status.h
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/datablock_types.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/entry.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/entry.hh
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/exceptions.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/generate_sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/handler.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/ndarray.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/section.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/section.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/section_names.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/datablock/section_names.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/gaussian_likelihood.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22952 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.942270 cosmosis-3.6/cosmosis/output/
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/astropy_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/cosmomc_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/fits_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/in_memory_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/null_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/output_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/text_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/output/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.942270 cosmosis-3.6/cosmosis/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/plotting/chain_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/plotting/grid_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/plotting/kde.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/plotting/plot_demo_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/plotting/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/plotting/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5502 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.946270 cosmosis-3.6/cosmosis/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16175 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/cosmology_theory_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/latex.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/lazy_pylab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50319 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/postprocess_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/reruns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33609 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/postprocessing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/declare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/runtime/julia_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/julia_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/julia_modules/julia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/memmon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17170 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/mpi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58652 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21210 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/prior.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/process_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/samplers/abc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/abc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7126 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/abc/abc_sampler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6698 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/abc/abc_sampler_mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/samplers/apriori/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/apriori/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2766 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/apriori/apriori_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/samplers/dynesty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/dynesty/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3707 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/dynesty/dynesty_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/samplers/emcee/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/emcee/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7516 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/emcee/emcee_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/samplers/fisher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/fisher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/fisher/fisher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6642 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/fisher/fisher_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/samplers/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/grid/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4745 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/grid/grid_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.950270 cosmosis-3.6/cosmosis/samplers/gridmax/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/gridmax/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4370 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/gridmax/gridmax_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/hints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.954270 cosmosis-3.6/cosmosis/samplers/importance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/importance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/importance/importance_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.954270 cosmosis-3.6/cosmosis/samplers/kombine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/kombine/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4932 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/kombine/kombine_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.954270 cosmosis-3.6/cosmosis/samplers/list/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/list/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5094 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/list/list_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.954270 cosmosis-3.6/cosmosis/samplers/maxlike/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/maxlike/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4666 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/maxlike/maxlike_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.954270 cosmosis-3.6/cosmosis/samplers/metropolis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/metropolis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/metropolis/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/metropolis/metropolis_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.954270 cosmosis-3.6/cosmosis/samplers/metropolis/proposal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/metropolis/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/metropolis/proposal/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.954270 cosmosis-3.6/cosmosis/samplers/minuit/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/minuit/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/minuit/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7323 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/minuit/minuit_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/minuit/minuit_wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.954270 cosmosis-3.6/cosmosis/samplers/multinest/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.958270 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/README
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/cwrapper.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    42915 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90
+-rw-r--r--   0 runner    (1001) docker     (127)   107766 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/nested.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    22010 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/posterior.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/priors.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/utils.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    28039 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/utils1.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    86938 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.958270 cosmosis-3.6/cosmosis/samplers/nautilus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/nautilus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/nautilus/nautilus_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.958270 cosmosis-3.6/cosmosis/samplers/pmaxlike/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/pmaxlike/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4151 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.958270 cosmosis-3.6/cosmosis/samplers/pmc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/pmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/pmc/pmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/pmc/pmc_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.958270 cosmosis-3.6/cosmosis/samplers/poco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/poco/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3703 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/poco/poco_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.958270 cosmosis-3.6/cosmosis/samplers/polychord/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12986 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.966270 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/README
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/abort.F90
+-rw-r--r--   0 runner    (1001) docker     (127)    18110 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/array_utils.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/c_interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/calculate.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/clustering.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    13421 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/feedback.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    26147 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/generate.F90
+-rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/ini.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    20999 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/interfaces.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/interfaces.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/interfaces.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24257 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90
+-rw-r--r--   0 runner    (1001) docker     (127)    20674 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/params.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    19675 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/priors.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    18291 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/random_utils.F90
+-rw-r--r--   0 runner    (1001) docker     (127)    44750 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/read_write.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    47427 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/run_time_info.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/settings.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    29353 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/utils.F90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.966270 cosmosis-3.6/cosmosis/samplers/pymc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/pymc/pymc_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.966270 cosmosis-3.6/cosmosis/samplers/snake/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/snake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/snake/snake.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2017 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/snake/snake_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.966270 cosmosis-3.6/cosmosis/samplers/star/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/star/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4468 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/star/star_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.966270 cosmosis-3.6/cosmosis/samplers/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3221 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/test/test_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.966270 cosmosis-3.6/cosmosis/samplers/zeus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/zeus/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11554 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/samplers/zeus/zeus_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.970270 cosmosis-3.6/cosmosis/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/bad-campaign.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/campaign.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/example-priors.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/example-values.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/example.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/example_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/example_module2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/example_module3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/example_module4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/included.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.974270 cosmosis-3.6/cosmosis/test/libtest/
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/c_datablock_complex_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/c_datablock_double_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/c_datablock_int_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/c_datablock_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/cosmosis_test.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/cosmosis_tests.supp
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/datablock_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/entry_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/ndarray_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/section_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    28088 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/test_c_datablock_scalars.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/libtest/test_c_datablock_scalars.template
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_polychord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_text_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 11:19:03.000000 cosmosis-3.6/cosmosis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:19:08.974270 cosmosis-3.6/cosmosis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-27 11:19:08.000000 cosmosis-3.6/cosmosis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-05-27 11:19:08.000000 cosmosis-3.6/cosmosis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:19:08.000000 cosmosis-3.6/cosmosis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-27 11:19:08.000000 cosmosis-3.6/cosmosis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-27 11:19:08.000000 cosmosis-3.6/cosmosis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-27 11:19:03.000000 cosmosis-3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 11:19:08.974270 cosmosis-3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-27 11:19:03.000000 cosmosis-3.6/setup.py
```

### Comparing `cosmosis-3.5.1/LICENSE` & `cosmosis-3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/MANIFEST.in` & `cosmosis-3.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/PKG-INFO` & `cosmosis-3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmosis
-Version: 3.5.1
+Version: 3.6
 Summary: The CosmoSIS parameter estimation library.
 Home-page: https://github.com/joezuntz/cosmosis
 Author: Joe Zuntz
 Author-email: joezuntz@googlemail.com
 License-File: LICENSE
 Requires-Dist: pyyaml
 Requires-Dist: emcee
```

### Comparing `cosmosis-3.5.1/bin/cosmosis-configure` & `cosmosis-3.6/bin/cosmosis-configure`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/bin/cosmosis-extract` & `cosmosis-3.6/bin/cosmosis-extract`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/bin/cosmosis-sample-fisher` & `cosmosis-3.6/bin/cosmosis-sample-fisher`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/__init__.py` & `cosmosis-3.6/cosmosis/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/campaign.py` & `cosmosis-3.6/cosmosis/campaign.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,50 @@
 from .main import run_cosmosis
 from .runtime.utils import underline
 import time
 import os
 import yaml
 import sys
 import warnings
+import subprocess
 import contextlib
 
+class UniqueKeyLoader(yaml.SafeLoader):
+    """
+    This is a YAML loader that raises an error if there are duplicate keys.
+
+    It is based on the discussion here:
+    https://gist.github.com/pypt/94d747fe5180851196eb
+    """
+    def construct_mapping(self, node, deep=False):
+        mapping = set()
+        for key_node, _ in node.value:
+            key = self.construct_object(key_node, deep=deep)
+            if key in mapping:
+                raise ValueError(f"Duplicate {key} key found in YAML.")
+            mapping.add(key)
+        return super().construct_mapping(node, deep)
+
+def load_yaml(stream):
+    """
+    Load YAML markup from a stream, with a check for duplicate keys.
+
+    Parameters
+    ----------
+    stream : file
+        The open file-like object to load from
+
+    Returns
+    -------
+    data : object
+        The dict or list loaded from the YAML file
+    """
+    return yaml.load(stream, Loader=UniqueKeyLoader)
+
+
 def pipeline_after(params, after_module, modules):
     """
     Insert item(s) in the pipeline after the given module.
 
     Parameters
     ----------
     params : Inifile
@@ -338,15 +372,15 @@
 
     if params.has_section("multinest"):
         params.set("multinest", "multinest_outfile_root", os.path.join(output_dir, f"{name}.multinest"))
     if params.has_section("polychord"):
         params.set("polychord", "polychord_outfile_root", f"{name}.polychord")
         params.set("polychord", "base_dir", output_dir)
 
-def build_run(name, run_info, runs, components, output_dir, output_name="{name}"):
+def build_run(name, run_info, runs, components, output_dir, submission_info, output_name="{name}"):
     """
     Generate a dictionary specifying a CosmoSIS run from a run_info dictioary.
 
     Parameters
     ----------
     name : str
         The name of the run
@@ -362,98 +396,136 @@
         - env : a dictionary of environment variables to set (optional)
     runs : dict
         A dictionary of previously built runs
     components : dict
         A dictionary of previously built components
     output_dir : str
         The output directory to use
+    submission_info : dict
+        A dictionary of submission information
     output_name : str
         The format string to use to generate the output file name, using {name}
         for the run name.
 
     Returns
     -------
     """
     run = run_info.copy()
-    env_vars = run_info.get("env", {})
-    run["env"] = env_vars
 
-
-    # We set the environment both now, when reading the ini files,
-    # so that any variable expansion is done, and also later when running
-    with temporary_environment(env_vars):
-        if "base" in run_info:
-            params = Inifile(run_info["base"], print_include_messages=False)
-        elif "parent" in run_info:
-            try:
-                parent = runs[run_info["parent"]]
-            except KeyError:
-                warnings.warn(f"Run {name} specifies parent {run_info['parent']} but there is no run with that name yet")
-                return None
-            params = Inifile(parent["params"], print_include_messages=False)
-        else:
-            warnings.warn(f"Run {name} specifies neither 'parent' nor 'base' so is invalid")
+    # We want to delay expanding environment variables so that child runs
+    # have a chance to override them. So we set no_expand_vars=True on all of these
+    if "base" in run_info:
+        params = Inifile(run_info["base"], print_include_messages=False, no_expand_vars=True)
+    elif "parent" in run_info:
+        try:
+            parent = runs[run_info["parent"]]
+        except KeyError:
+            warnings.warn(f"Run {name} specifies parent {run_info['parent']} but there is no run with that name yet")
             return None
+        params = Inifile(parent["params"], print_include_messages=False, no_expand_vars=True)
+    else:
+        warnings.warn(f"Run {name} specifies neither 'parent' nor 'base' so is invalid")
+        return None
+    
+    # Build environment variables
+    # These are inherited from the parent run, if there is one,
+    # and then updated with any specific to this run, which can overwrite.
+    # env vars are only applied right at the end when all runs are collected
+    if "parent" in run_info:
+        env_vars = parent["env"].copy()
+    else:
+        env_vars = {}
+    env_vars.update(run_info.get("env", {}))
+    run["env"] = env_vars
 
-        # Build values file, which is mandatory
-        if "parent" in run_info:
-            values = Inifile(parent["values"], print_include_messages=False)
-        else:
-            values_file = params.get('pipeline', 'values')
-            values = Inifile(values_file, print_include_messages=False)
-
-        # Build optional priors file
-        if "parent" in run_info:
-            priors = Inifile(parent["priors"], print_include_messages=False)
-        elif "priors" in params.options("pipeline"):
-            priors_file = params.get('pipeline', 'priors')
-            priors = Inifile(priors_file, print_include_messages=False)
-        else:
-            priors = Inifile(None)
-        
-
+    # Build values file, which is mandatory
+    if "parent" in run_info:
+        values = Inifile(parent["values"], print_include_messages=False, no_expand_vars=True)
+    else:
+        values_file = params.get('pipeline', 'values')
+        values = Inifile(values_file, print_include_messages=False, no_expand_vars=True)
 
-        # Make a list of all the modifications to be applied
-        # to the different bits of this pipeline
+    # Build optional priors file
+    if "parent" in run_info:
+        priors = Inifile(parent["priors"], print_include_messages=False, no_expand_vars=True)
+    elif "priors" in params.options("pipeline"):
+        priors_file = params.get('pipeline', 'priors')
+        priors = Inifile(priors_file, print_include_messages=False, no_expand_vars=True)
+    else:
+        priors = Inifile(None, no_expand_vars=True)
 
-        param_updates = []
-        value_updates = []
-        prior_updates = []
-        pipeline_updates = []
-
-        # First from any generic components specified
-        for component in run_info.get("components", []):
-            component_info = components[component]
-            param_updates.extend(component_info.get("params", []))
-            value_updates.extend(component_info.get("values", []))
-            prior_updates.extend(component_info.get("priors", []))
-            pipeline_updates.extend(component_info.get("pipeline", []))
-
-        # And then for anything specific to this pipeline
-        param_updates.extend(run_info.get("params", []))
-        value_updates.extend(run_info.get("values", []))
-        prior_updates.extend(run_info.get("priors", []))
-        pipeline_updates.extend(run_info.get("pipeline", []))
-
-        # Now apply all the steps
-        apply_updates(params, param_updates, is_params=True)
-        apply_updates(values, value_updates)
-        apply_updates(priors, prior_updates)
-        apply_pipeline_updates(params, pipeline_updates)
+    # Make a list of all the modifications to be applied
+    # to the different bits of this pipeline
 
-        output_name = run_info.get("output_name", output_name)
-        set_output_dir(params, name, output_dir, output_name)
+    param_updates = []
+    value_updates = []
+    prior_updates = []
+    pipeline_updates = []
+
+    # First from any generic components specified
+    for component in run_info.get("components", []):
+        component_info = components[component]
+        param_updates.extend(component_info.get("params", []))
+        value_updates.extend(component_info.get("values", []))
+        prior_updates.extend(component_info.get("priors", []))
+        pipeline_updates.extend(component_info.get("pipeline", []))
+
+    # And then for anything specific to this pipeline
+    param_updates.extend(run_info.get("params", []))
+    value_updates.extend(run_info.get("values", []))
+    prior_updates.extend(run_info.get("priors", []))
+    pipeline_updates.extend(run_info.get("pipeline", []))
+
+    # Now apply all the steps
+    apply_updates(params, param_updates, is_params=True)
+    apply_updates(values, value_updates)
+    apply_updates(priors, prior_updates)
+    apply_pipeline_updates(params, pipeline_updates)
+
+    output_name = run_info.get("output_name", output_name)
+    set_output_dir(params, name, output_dir, output_name)
+
+    # Finally, set the submission information
+    submission_info = submission_info.copy()
+    submission_info["output_dir"] = output_dir
+    submission_info.update(run_info.get("submission", {}))
+    run["submission"] = submission_info
 
     run["params"] = params
     run["values"] = values
     run["priors"] = priors
 
     return run
 
 
+def expand_environment_variables(runs):
+    """
+    For each run, expand any environment variables in the all three parameter files.
+
+    Environment variables are only supported in values, not in keys or sections.
+
+    Parameters
+    ----------
+    runs : dict
+        A dictionary of runs, keyed by name
+    """
+    for run in runs.values():
+        # This sets environment varibles for the duration of the with block
+        with temporary_environment(run["env"]):
+
+            # We apply this to all the different ini files
+            for ini in [run["params"], run["values"], run["priors"]]:
+                for section in ini.sections():
+                    # Now we can expand all the actual options
+                    for option in ini.options(section):
+                        value = ini.get(section, option)
+                        new_value = os.path.expandvars(value)
+                        if new_value != value:
+                            ini.set(section, option, new_value)
+
 def parse_yaml_run_file(run_config):
     """
     Parse a yaml file (or process a previously parsed file)
     containing a list of runs to perform.
 
     The file should have the following format:
 
@@ -485,59 +557,82 @@
         - <list of updates to apply to the parameters file>
         values:
         - <list of updates to apply to the values file>
         priors:
         - <list of updates to apply to the priors file>
         pipeline:
         - <list of updates to apply to the pipeline>
-            
+
+    submission:
+        submit: a command to submit runs from batch files (default sbatch)
+        cancel: a command to cancel runs from batch files (default scancel)
+        template: a template for the batch file (default is a SLURM one suitable for NERSC)
+        # remaining variables are passed to the template and can be overridden in specific runs
+        time: Wall time for the job, e.g. 00:30:00
+        nodes: Number of nodes, e.g. 1
+        tasks: Number of tasks in total, e.g. 1
+        cores_per_task: Number of cores (threads) per task, e.g. 1
+        queue: Queue to submit to, e.g. regular
+
                 
     Parameters
     ----------
     run_config : str or dict
         The name of the file to parse, or a previously loaded configuration
 
     Returns
     -------
     runs : dict
         A dictionary of runs, keyed by name
+    
+    components : dict
+        A dictionary of components, keyed by name
     """
     if isinstance(run_config, dict):
         info = run_config
     else:
         with open(run_config, 'r') as f:
-            info = yaml.safe_load(f)
+            info = load_yaml(f)
     
     output_dir = info.get("output_dir", ".")
     output_name = info.get("output_name", "{name}")
 
     include = info.get("include", [])
     if isinstance(include, str):
         include = [include]
 
     # Can include another run file, which we deal with
     # recursively.  
     runs = {}
+    components = {}
     for include_file in include:
-        runs.update(parse_yaml_run_file(include_file))
+        inc_runs, inc_comps = parse_yaml_run_file(include_file)
+        components.update(inc_comps)
+        runs.update(inc_runs)
 
     # But we override the output directory
     # of any imported runs with the one we have here   
     for name, run in runs.items():
         set_output_dir(run["params"], name, output_dir, output_name)
     
     # deal with re-usable components
-    components = info.get("components", {})
+    components.update(info.get("components", {}))
+
+    submission_info = info.get("submission", {})
 
     # Build the parameter, value, and prior objects for this run
     for run_dict in info["runs"]:
         name = run_dict["name"]
-        runs[name] = build_run(name, run_dict, runs, components, output_dir, output_name)
+        runs[name] = build_run(name, run_dict, runs, components, output_dir, submission_info, output_name)
+
+    # Only now do we expand environment variables in the runs.  This gives the child runs
+    # a chance to override the environment variables of their parents.
+    expand_environment_variables(runs)
 
-    return runs
+    return runs, components
 
 
 def show_run(run):
     """
     Print a complete description of the run to the screen
 
     Parameters
@@ -664,31 +759,65 @@
         if mpi:
             with MPIPool() as pool:
                 return run_cosmosis(params, values=values, priors=priors, pool=pool)
         else:
             return run_cosmosis(params, values=values, priors=priors)
 
 
+def submit_run(run_file, run):
+    """
+    Subnmit a CosmoSIS run using a batch system such as SLURM.
+    """
+
+    submission_info = run["submission"]
+    template = submission_info["template"]
+    keys = submission_info.copy()
+    name = run["name"]
+    keys["job_name"] = name
+    output_dir = keys["output_dir"]
+
+    # We use the campaign program to actually run the jobs
+    keys["command"]  = f"cosmosis-campaign {run_file} --run {name} --mpi"
+
+    # choose where the jobs stdout / stderr should go
+    os.makedirs(os.path.join(output_dir, "logs"), exist_ok=True)
+    keys["log"] = os.path.join(output_dir, "logs", f"{name}.log")
+
+    # fill in the template
+    sub_script = template.format(**keys).lstrip()
+
+    # write the submission file to a batch subdir
+    os.makedirs(os.path.join(output_dir, "batch"), exist_ok=True)
+    sub_file = os.path.join(output_dir, "batch", f"{name}.sub")
+    with open(sub_file, "w") as f:
+        f.write(sub_script)
+
+    # Actually submit the job using slurm or similar
+    submit = submission_info.get("submit", "sbatch")
+    subprocess.check_call(f"{submit} {sub_file}", shell=True)
+    print(f"Submitted {sub_file}\nJob output in", keys["log"])
+
 
 
 import argparse
 parser = argparse.ArgumentParser(description="Manage and launch CosmoSIS runs")
 parser.add_argument("run_config", help="The yaml file containing the runs to perform")
 group = parser.add_mutually_exclusive_group(required=True)
 group.add_argument("--list", "-l", action="store_true", help="List all available runs")
 group.add_argument("--cat", "-c",  type=str, help="Show a single run")
 group.add_argument("--status", "-s", default="_unset", nargs="*", help="Show the status of a single run, or all runs if called with no argument")
 group.add_argument("--run", "-r",  help="Run the named run")
-group.add_argument("--test", "-t",  help="Launch the named run")
+group.add_argument("--test", "-t",  help="Test the named run")
+group.add_argument("--submit", "-x",  help="Submit the named run to a batch system")
 parser.add_argument("--mpi", action="store_true", help="Use MPI to launch the runs")
 
 
 
 def main(args):
-    runs = parse_yaml_run_file(args.run_config)
+    runs, _ = parse_yaml_run_file(args.run_config)
 
     if args.mpi and not args.run:
         raise ValueError("MPI can only be used when running a single run")
 
     status_set = args.status != "_unset"
 
     # The various command line options, which are mutually exclusive.
@@ -700,14 +829,16 @@
         show_run(runs[args.cat])
     elif args.test:
         perform_test_run(runs[args.test])
     elif status_set:
         show_run_status(runs, args.status)
     elif args.run:
         launch_run(runs[args.run], mpi=args.mpi)
+    elif args.submit:
+        submit_run(args.run_config, runs[args.submit])
 
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
     main(args)
```

### Comparing `cosmosis-3.5.1/cosmosis/config/compilers.mk` & `cosmosis-3.6/cosmosis/config/compilers.mk`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/configure.py` & `cosmosis-3.6/cosmosis/configure.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/constants.py` & `cosmosis-3.6/cosmosis/constants.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/Makefile` & `cosmosis-3.6/cosmosis/datablock/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/c_datablock.cc` & `cosmosis-3.6/cosmosis/datablock/c_datablock.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/c_datablock.h` & `cosmosis-3.6/cosmosis/datablock/c_datablock.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/clamp.hh` & `cosmosis-3.6/cosmosis/datablock/clamp.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/cosmosis_constants.fh` & `cosmosis-3.6/cosmosis/datablock/cosmosis_constants.fh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/cosmosis_constants.h` & `cosmosis-3.6/cosmosis/datablock/cosmosis_constants.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/cosmosis_modules.F90` & `cosmosis-3.6/cosmosis/datablock/cosmosis_modules.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/cosmosis_py/block.py` & `cosmosis-3.6/cosmosis/datablock/cosmosis_py/block.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/cosmosis_py/errors.py` & `cosmosis-3.6/cosmosis/datablock/cosmosis_py/errors.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/cosmosis_py/lib.py` & `cosmosis-3.6/cosmosis/datablock/cosmosis_py/lib.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/cosmosis_py/section_names.py` & `cosmosis-3.6/cosmosis/datablock/cosmosis_py/section_names.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/cosmosis_section_names.F90` & `cosmosis-3.6/cosmosis/datablock/cosmosis_section_names.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/cosmosis_wrappers.F90` & `cosmosis-3.6/cosmosis/datablock/cosmosis_wrappers.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/datablock.cc` & `cosmosis-3.6/cosmosis/datablock/datablock.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/datablock.hh` & `cosmosis-3.6/cosmosis/datablock/datablock.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/datablock_logging.cc` & `cosmosis-3.6/cosmosis/datablock/datablock_logging.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/datablock_logging.h` & `cosmosis-3.6/cosmosis/datablock/datablock_logging.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/datablock_status.h` & `cosmosis-3.6/cosmosis/datablock/datablock_status.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/entry.cc` & `cosmosis-3.6/cosmosis/datablock/entry.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/entry.hh` & `cosmosis-3.6/cosmosis/datablock/entry.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/generate_sections.py` & `cosmosis-3.6/cosmosis/datablock/generate_sections.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/handler.c` & `cosmosis-3.6/cosmosis/datablock/handler.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/ndarray.hh` & `cosmosis-3.6/cosmosis/datablock/ndarray.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/section.cc` & `cosmosis-3.6/cosmosis/datablock/section.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/section.hh` & `cosmosis-3.6/cosmosis/datablock/section.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/section_names.h` & `cosmosis-3.6/cosmosis/datablock/section_names.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/datablock/section_names.txt` & `cosmosis-3.6/cosmosis/datablock/section_names.txt`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/gaussian_likelihood.py` & `cosmosis-3.6/cosmosis/gaussian_likelihood.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/main.py` & `cosmosis-3.6/cosmosis/main.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/output/__init__.py` & `cosmosis-3.6/cosmosis/output/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/output/astropy_output.py` & `cosmosis-3.6/cosmosis/output/astropy_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/output/cosmomc_output.py` & `cosmosis-3.6/cosmosis/output/cosmomc_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/output/fits_output.py` & `cosmosis-3.6/cosmosis/output/fits_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/output/in_memory_output.py` & `cosmosis-3.6/cosmosis/output/in_memory_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/output/null_output.py` & `cosmosis-3.6/cosmosis/output/null_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/output/output_base.py` & `cosmosis-3.6/cosmosis/output/output_base.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/output/text_output.py` & `cosmosis-3.6/cosmosis/output/text_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/output/utils.py` & `cosmosis-3.6/cosmosis/output/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/plotting/chain_plots.py` & `cosmosis-3.6/cosmosis/plotting/chain_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/plotting/grid_plots.py` & `cosmosis-3.6/cosmosis/plotting/grid_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/plotting/kde.py` & `cosmosis-3.6/cosmosis/plotting/kde.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/plotting/plotter.py` & `cosmosis-3.6/cosmosis/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/postprocess.py` & `cosmosis-3.6/cosmosis/postprocess.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/postprocessing/__init__.py` & `cosmosis-3.6/cosmosis/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/postprocessing/cosmology_theory_plots.py` & `cosmosis-3.6/cosmosis/postprocessing/cosmology_theory_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/postprocessing/density.py` & `cosmosis-3.6/cosmosis/postprocessing/density.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/postprocessing/elements.py` & `cosmosis-3.6/cosmosis/postprocessing/elements.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/postprocessing/inputs.py` & `cosmosis-3.6/cosmosis/postprocessing/inputs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/postprocessing/latex.ini` & `cosmosis-3.6/cosmosis/postprocessing/latex.ini`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/postprocessing/lazy_pylab.py` & `cosmosis-3.6/cosmosis/postprocessing/lazy_pylab.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/postprocessing/main.py` & `cosmosis-3.6/cosmosis/postprocessing/main.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/postprocessing/outputs.py` & `cosmosis-3.6/cosmosis/postprocessing/outputs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/postprocessing/plots.py` & `cosmosis-3.6/cosmosis/postprocessing/plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/postprocessing/postprocess.py` & `cosmosis-3.6/cosmosis/postprocessing/postprocess.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/postprocessing/postprocess_base.py` & `cosmosis-3.6/cosmosis/postprocessing/postprocess_base.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/postprocessing/reruns.py` & `cosmosis-3.6/cosmosis/postprocessing/reruns.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/postprocessing/statistics.py` & `cosmosis-3.6/cosmosis/postprocessing/statistics.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/postprocessing/utils.py` & `cosmosis-3.6/cosmosis/postprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/runtime/analytics.py` & `cosmosis-3.6/cosmosis/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/runtime/attribution.py` & `cosmosis-3.6/cosmosis/runtime/attribution.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/runtime/config.py` & `cosmosis-3.6/cosmosis/runtime/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 
     Note that the caller of the `read()` method may set a
     `no_expand_includes` attribute on this object, to cause any %include
     lines to *not* actually be actioned (they will be regarded as
     comments, but still delineate sections).
     """
 
-    def __init__(self, defaults=None, print_include_messages=True):
+    def __init__(self, defaults=None, print_include_messages=True, no_expand_vars=False):
+        self.no_expand_vars = no_expand_vars
         configparser.ConfigParser.__init__(self,
                                    defaults=defaults,
                                    dict_type=collections.OrderedDict,
                                    strict=False,
                                    inline_comment_prefixes=(';', '#'),
                                    )
         self.print_include_messages = print_include_messages
@@ -48,15 +49,15 @@
         To do so we first read the file into a StringIO object, dealing
         with the %include directives as we go, then pass that to the
         parent method.
         """
         s = io.StringIO()
         for line in fp:
             # check for include directives
-            if not getattr(self, 'no_expand_vars', False):
+            if not self.no_expand_vars:
                 line = os.path.expandvars(line)
 
             if line.lower().startswith('%include'):
                 _, filename = line.split()
                 filename = filename.strip('"').strip("'")
 
                 if self.print_include_messages:
@@ -91,30 +92,31 @@
 
     The values are all stored as strings, with methods provided to locate
     and interpret them as integers, floating-point numbers, booleans, or
     arrays of integers or floating-point numbers.
 
     """
 
-    def __init__(self, filename, defaults=None, override=None, print_include_messages=True):
+    def __init__(self, filename, defaults=None, override=None, print_include_messages=True, no_expand_vars=False):
         u"""Read in a configuration from `filename`.
 
         The `defaults` will be applied if a parameter is not specified in
         the file (or %included descendants), and the `override`s will be
         imposed on the regardless of whether those parameters have
         assigned values or not.
 
         Where supplied, `defaults` and `override` should be dictionary
         mappings of `(section, name) -> value`.
 
         """
 
         IncludingConfigParser.__init__(self,
                                        defaults=defaults,
-                                       print_include_messages=print_include_messages)
+                                       print_include_messages=print_include_messages,
+                                       no_expand_vars=no_expand_vars)
 
         # if we are pased a dict, convert it to an inifile
         if isinstance(filename, dict):
             for section, values in filename.items():
                 self.add_section(section)
                 for key, value in values.items():
                     self.set(section, key, str(value))
```

### Comparing `cosmosis-3.5.1/cosmosis/runtime/declare.py` & `cosmosis-3.6/cosmosis/runtime/declare.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/runtime/julia_modules/julia.py` & `cosmosis-3.6/cosmosis/runtime/julia_modules/julia.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/runtime/logs.py` & `cosmosis-3.6/cosmosis/runtime/logs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/runtime/memmon.py` & `cosmosis-3.6/cosmosis/runtime/memmon.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/runtime/module.py` & `cosmosis-3.6/cosmosis/runtime/module.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/runtime/mpi_pool.py` & `cosmosis-3.6/cosmosis/runtime/mpi_pool.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/runtime/parameter.py` & `cosmosis-3.6/cosmosis/runtime/parameter.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/runtime/pipeline.py` & `cosmosis-3.6/cosmosis/runtime/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,14 +389,15 @@
             ]
         else:
             self.modules = []
 
 
         self.shortcut_module=0
         self.shortcut_data=None
+        self.timings = None
 
         if self.modules:
             if shortcut is not None:
                 try:
                     index = module_list.index(shortcut)
                 except ValueError:
                     raise ValueError("You tried to set a shortcut in "
```

### Comparing `cosmosis-3.5.1/cosmosis/runtime/prior.py` & `cosmosis-3.6/cosmosis/runtime/prior.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/runtime/process_pool.py` & `cosmosis-3.6/cosmosis/runtime/process_pool.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/__init__.py` & `cosmosis-3.6/cosmosis/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/abc/abc_sampler.py` & `cosmosis-3.6/cosmosis/samplers/abc/abc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/abc/abc_sampler_mpi.py` & `cosmosis-3.6/cosmosis/samplers/abc/abc_sampler_mpi.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/apriori/apriori_sampler.py` & `cosmosis-3.6/cosmosis/samplers/apriori/apriori_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/dynesty/dynesty_sampler.py` & `cosmosis-3.6/cosmosis/samplers/dynesty/dynesty_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/emcee/emcee_sampler.py` & `cosmosis-3.6/cosmosis/samplers/emcee/emcee_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/fisher/fisher.py` & `cosmosis-3.6/cosmosis/samplers/fisher/fisher.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/fisher/fisher_sampler.py` & `cosmosis-3.6/cosmosis/samplers/fisher/fisher_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/grid/grid_sampler.py` & `cosmosis-3.6/cosmosis/samplers/grid/grid_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/gridmax/gridmax_sampler.py` & `cosmosis-3.6/cosmosis/samplers/gridmax/gridmax_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/hints.py` & `cosmosis-3.6/cosmosis/samplers/hints.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/importance/importance_sampler.py` & `cosmosis-3.6/cosmosis/samplers/importance/importance_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/kombine/kombine_sampler.py` & `cosmosis-3.6/cosmosis/samplers/kombine/kombine_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/list/list_sampler.py` & `cosmosis-3.6/cosmosis/samplers/list/list_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/maxlike/maxlike_sampler.py` & `cosmosis-3.6/cosmosis/samplers/maxlike/maxlike_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/metropolis/metropolis.py` & `cosmosis-3.6/cosmosis/samplers/metropolis/metropolis.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/metropolis/metropolis_sampler.py` & `cosmosis-3.6/cosmosis/samplers/metropolis/metropolis_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py` & `cosmosis-3.6/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/metropolis/proposal/standard.py` & `cosmosis-3.6/cosmosis/samplers/metropolis/proposal/standard.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/minuit/Makefile` & `cosmosis-3.6/cosmosis/samplers/minuit/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/minuit/minuit_sampler.py` & `cosmosis-3.6/cosmosis/samplers/minuit/minuit_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/minuit/minuit_wrapper.cpp` & `cosmosis-3.6/cosmosis/samplers/minuit/minuit_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_sampler.py` & `cosmosis-3.6/cosmosis/samplers/multinest/multinest_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/LICENCE` & `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/LICENCE`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/Makefile` & `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/README` & `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/README`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/cwrapper.f90` & `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/cwrapper.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90` & `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/nested.f90` & `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/nested.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/posterior.f90` & `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/posterior.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/priors.f90` & `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/priors.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/utils.f90` & `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/utils.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/utils1.f90` & `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/utils1.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90` & `cosmosis-3.6/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/nautilus/nautilus_sampler.py` & `cosmosis-3.6/cosmosis/samplers/nautilus/nautilus_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py` & `cosmosis-3.6/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/pmc/pmc.py` & `cosmosis-3.6/cosmosis/samplers/pmc/pmc.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/pmc/pmc_sampler.py` & `cosmosis-3.6/cosmosis/samplers/pmc/pmc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/poco/poco_sampler.py` & `cosmosis-3.6/cosmosis/samplers/poco/poco_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_sampler.py` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/LICENCE` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/LICENCE`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/Makefile` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/README` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/README`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/abort.F90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/abort.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/array_utils.f90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/array_utils.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/c_interface.cpp` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/c_interface.cpp`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/calculate.f90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/calculate.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/clustering.f90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/clustering.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/feedback.f90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/feedback.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/generate.F90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/generate.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/ini.f90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/ini.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/interfaces.F90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/interfaces.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/interfaces.h` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/interfaces.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/interfaces.hpp` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/interfaces.hpp`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/params.f90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/params.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/priors.f90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/priors.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/random_utils.F90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/random_utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/read_write.f90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/read_write.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/run_time_info.f90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/run_time_info.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/settings.f90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/settings.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/polychord/polychord_src/utils.F90` & `cosmosis-3.6/cosmosis/samplers/polychord/polychord_src/utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/pymc/pymc_sampler.py` & `cosmosis-3.6/cosmosis/samplers/pymc/pymc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/sampler.py` & `cosmosis-3.6/cosmosis/samplers/sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/snake/snake.py` & `cosmosis-3.6/cosmosis/samplers/snake/snake.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/snake/snake_sampler.py` & `cosmosis-3.6/cosmosis/samplers/snake/snake_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/star/star_sampler.py` & `cosmosis-3.6/cosmosis/samplers/star/star_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/test/test_sampler.py` & `cosmosis-3.6/cosmosis/samplers/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/samplers/zeus/zeus_sampler.py` & `cosmosis-3.6/cosmosis/samplers/zeus/zeus_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/example_module2.py` & `cosmosis-3.6/cosmosis/test/example_module2.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/libtest/Makefile` & `cosmosis-3.6/cosmosis/test/libtest/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/libtest/c_datablock_complex_array_test.c` & `cosmosis-3.6/cosmosis/test/libtest/c_datablock_complex_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/libtest/c_datablock_double_array_test.c` & `cosmosis-3.6/cosmosis/test/libtest/c_datablock_double_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/libtest/c_datablock_int_array_test.c` & `cosmosis-3.6/cosmosis/test/libtest/c_datablock_int_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c` & `cosmosis-3.6/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c` & `cosmosis-3.6/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c` & `cosmosis-3.6/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/libtest/c_datablock_test.c` & `cosmosis-3.6/cosmosis/test/libtest/c_datablock_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/libtest/cosmosis_test.F90` & `cosmosis-3.6/cosmosis/test/libtest/cosmosis_test.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/libtest/datablock_test.cc` & `cosmosis-3.6/cosmosis/test/libtest/datablock_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/libtest/entry_test.cc` & `cosmosis-3.6/cosmosis/test/libtest/entry_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/libtest/ndarray_test.cc` & `cosmosis-3.6/cosmosis/test/libtest/ndarray_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/libtest/section_test.cc` & `cosmosis-3.6/cosmosis/test/libtest/section_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/libtest/test_c_datablock_scalars.h` & `cosmosis-3.6/cosmosis/test/libtest/test_c_datablock_scalars.h`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/libtest/test_c_datablock_scalars.template` & `cosmosis-3.6/cosmosis/test/libtest/test_c_datablock_scalars.template`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/test_block.py` & `cosmosis-3.6/cosmosis/test/test_block.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/test_chaining.py` & `cosmosis-3.6/cosmosis/test/test_chaining.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/test_gaussian.py` & `cosmosis-3.6/cosmosis/test/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/test_lib.py` & `cosmosis-3.6/cosmosis/test/test_lib.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/test_modules.py` & `cosmosis-3.6/cosmosis/test/test_modules.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/test_parameters.py` & `cosmosis-3.6/cosmosis/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/test_pipeline.py` & `cosmosis-3.6/cosmosis/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/test_polychord.py` & `cosmosis-3.6/cosmosis/test/test_polychord.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/test_samplers.py` & `cosmosis-3.6/cosmosis/test/test_samplers.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/test_text_output.py` & `cosmosis-3.6/cosmosis/test/test_text_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/test/test_utils.py` & `cosmosis-3.6/cosmosis/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis/utils.py` & `cosmosis-3.6/cosmosis/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-3.5.1/cosmosis.egg-info/PKG-INFO` & `cosmosis-3.6/cosmosis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmosis
-Version: 3.5.1
+Version: 3.6
 Summary: The CosmoSIS parameter estimation library.
 Home-page: https://github.com/joezuntz/cosmosis
 Author: Joe Zuntz
 Author-email: joezuntz@googlemail.com
 License-File: LICENSE
 Requires-Dist: pyyaml
 Requires-Dist: emcee
```

### Comparing `cosmosis-3.5.1/cosmosis.egg-info/SOURCES.txt` & `cosmosis-3.6/cosmosis.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -204,22 +204,24 @@
 cosmosis/samplers/star/__init__.py
 cosmosis/samplers/star/star_sampler.py
 cosmosis/samplers/test/__init__.py
 cosmosis/samplers/test/test_sampler.py
 cosmosis/samplers/zeus/__init__.py
 cosmosis/samplers/zeus/zeus_sampler.py
 cosmosis/test/__init__.py
+cosmosis/test/bad-campaign.yml
 cosmosis/test/campaign.yml
 cosmosis/test/example-priors.ini
 cosmosis/test/example-values.ini
 cosmosis/test/example.ini
 cosmosis/test/example_module.py
 cosmosis/test/example_module2.py
 cosmosis/test/example_module3.py
 cosmosis/test/example_module4.py
+cosmosis/test/included.yml
 cosmosis/test/test_block.py
 cosmosis/test/test_campaign.py
 cosmosis/test/test_chaining.py
 cosmosis/test/test_gaussian.py
 cosmosis/test/test_lib.py
 cosmosis/test/test_modules.py
 cosmosis/test/test_parameters.py
```

### Comparing `cosmosis-3.5.1/setup.py` & `cosmosis-3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,16 @@
     "test/libtest/entry_test.cc",
     "test/libtest/ndarray_test.cc",
     "test/libtest/section_test.cc",
     "test/libtest/test_c_datablock_scalars.h",
     "test/libtest/test_c_datablock_scalars.template",
     "test/libtest/Makefile",
     "test/campaign.yml",
+    "test/included.yml",
+    "test/bad-campaign.yml",
     "test/example-priors.ini",
     "test/example-values.ini",
     "test/example.ini",
 
 ]
 
 other_files = ["postprocessing/latex.ini"]
```

