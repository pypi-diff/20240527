# Comparing `tmp/conifer-1.4b1.tar.gz` & `tmp/conifer-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conifer-1.4b1.tar", last modified: Thu Nov 23 13:14:49 2023, max compression
+gzip compressed data, was "conifer-1.5.tar", last modified: Mon May 27 15:26:17 2024, max compression
```

## Comparing `conifer-1.4b1.tar` & `conifer-1.5.tar`

### file list

```diff
@@ -1,142 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.386176 conifer-1.4b1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.366176 conifer-1.4b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.370176 conifer-1.4b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-11-23 13:14:38.000000 conifer-1.4b1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-23 13:14:38.000000 conifer-1.4b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-23 13:14:38.000000 conifer-1.4b1/Jenkinsfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-23 13:14:38.000000 conifer-1.4b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-11-23 13:14:38.000000 conifer-1.4b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5943 2023-11-23 13:14:49.386176 conifer-1.4b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2023-11-23 13:14:38.000000 conifer-1.4b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.370176 conifer-1.4b1/conifer/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.374176 conifer-1.4b1/conifer/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.374176 conifer-1.4b1/conifer/backends/boards/
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/boards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/boards/boards.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.366176 conifer-1.4b1/conifer/backends/boards/configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.374176 conifer-1.4b1/conifer/backends/boards/configs/alveo/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/boards/configs/alveo/xilinx_u200_gen3x16_xdma_2_202110_1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.374176 conifer-1.4b1/conifer/backends/boards/configs/zynq/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/boards/configs/zynq/kr260.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/boards/configs/zynq/kv260.json
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/boards/configs/zynq/pynq_z2.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/boards/configs/zynq/ultra96v2.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/boards/configs/zynq/zcu102.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/boards/configs/zynq/zcu104.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.374176 conifer-1.4b1/conifer/backends/boards/src/
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/boards/src/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/boards/src/build_bit.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.374176 conifer-1.4b1/conifer/backends/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/cpp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.374176 conifer-1.4b1/conifer/backends/cpp/include/
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/cpp/include/conifer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.374176 conifer-1.4b1/conifer/backends/cpp/template/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/cpp/template/bridge.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/cpp/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.374176 conifer-1.4b1/conifer/backends/fpu/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/fpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/fpu/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.378176 conifer-1.4b1/conifer/backends/fpu/src/
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/fpu/src/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      647 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/fpu/src/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/fpu/src/build_hls.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/fpu/src/changes.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/fpu/src/fpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/fpu/src/fpu.h
--rw-r--r--   0 runner    (1001) docker     (127)    16002 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/fpu/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.378176 conifer-1.4b1/conifer/backends/vhdl/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.378176 conifer-1.4b1/conifer/backends/vhdl/firmware/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/firmware/AddReduce.vhd
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/firmware/BDT.vhd
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/firmware/BDTTestbench.vhd
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/firmware/BDTTop.vhd
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/firmware/Constants.vhd
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/firmware/SimulationInput.vhd
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/firmware/SimulationOutput.vhd
--rw-r--r--   0 runner    (1001) docker     (127)      810 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/firmware/TestUtil.vhd
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/firmware/Tree.vhd
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/firmware/Types.vhd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.378176 conifer-1.4b1/conifer/backends/vhdl/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/scripts/ghdl_compile.sh
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/scripts/modelsim_compile.sh
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/scripts/synth.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/scripts/xsim_compile.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/simulators.py
--rw-r--r--   0 runner    (1001) docker     (127)    11150 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/vhdl/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.378176 conifer-1.4b1/conifer/backends/xilinxhls/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/xilinxhls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.378176 conifer-1.4b1/conifer/backends/xilinxhls/firmware/
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/xilinxhls/firmware/BDT_rolled.h
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/xilinxhls/firmware/BDT_unrolled.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.382176 conifer-1.4b1/conifer/backends/xilinxhls/hls-template/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/xilinxhls/hls-template/bridge.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/xilinxhls/hls-template/build_hls.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.382176 conifer-1.4b1/conifer/backends/xilinxhls/hls-template/firmware/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/xilinxhls/hls-template/firmware/BDT_rolled.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/xilinxhls/hls-template/firmware/BDT_unrolled.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      969 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/xilinxhls/hls-template/firmware/myproject.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/xilinxhls/hls-template/firmware/myproject.h
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/xilinxhls/hls-template/myproject_test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/xilinxhls/hls-template/vivado_synth.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/xilinxhls/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    28251 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/backends/xilinxhls/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.382176 conifer-1.4b1/conifer/converters/
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/converters/onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/converters/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/converters/tf_df.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/converters/tmva.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/converters/xgboost.py
--rw-r--r--   0 runner    (1001) docker     (127)    15029 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.382176 conifer-1.4b1/conifer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/utils/fixed_point.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/utils/fixed_point_conversions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.386176 conifer-1.4b1/conifer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5943 2023-11-23 13:14:49.000000 conifer-1.4b1/conifer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2023-11-23 13:14:49.000000 conifer-1.4b1/conifer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 13:14:49.000000 conifer-1.4b1/conifer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-23 13:14:49.000000 conifer-1.4b1/conifer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-23 13:14:49.000000 conifer-1.4b1/conifer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    28385 2023-11-23 13:14:38.000000 conifer-1.4b1/conifer_v1.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.370176 conifer-1.4b1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.382176 conifer-1.4b1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2023-11-23 13:14:38.000000 conifer-1.4b1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2023-11-23 13:14:38.000000 conifer-1.4b1/docs/source/fpu.rst
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-11-23 13:14:38.000000 conifer-1.4b1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.386176 conifer-1.4b1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2023-11-23 13:14:38.000000 conifer-1.4b1/examples/build_fpu_alveo.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2023-11-23 13:14:38.000000 conifer-1.4b1/examples/build_fpu_pynq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2023-11-23 13:14:38.000000 conifer-1.4b1/examples/hls_accelerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2023-11-23 13:14:38.000000 conifer-1.4b1/examples/model_saving_loading.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2023-11-23 13:14:38.000000 conifer-1.4b1/examples/pruned_xgboost_to_hls.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-11-23 13:14:38.000000 conifer-1.4b1/examples/sklearn_RandomForest.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-11-23 13:14:38.000000 conifer-1.4b1/examples/sklearn_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-11-23 13:14:38.000000 conifer-1.4b1/examples/sklearn_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2023-11-23 13:14:38.000000 conifer-1.4b1/examples/sklearn_to_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-11-23 13:14:38.000000 conifer-1.4b1/examples/sklearn_to_fpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-11-23 13:14:38.000000 conifer-1.4b1/examples/sklearn_to_hls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-11-23 13:14:38.000000 conifer-1.4b1/examples/sklearn_to_vhdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-11-23 13:14:38.000000 conifer-1.4b1/examples/tf_df_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2023-11-23 13:14:38.000000 conifer-1.4b1/examples/tf_df_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-11-23 13:14:38.000000 conifer-1.4b1/examples/xgboost_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-11-23 13:14:38.000000 conifer-1.4b1/examples/xgboost_to_hls.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-23 13:14:38.000000 conifer-1.4b1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-23 13:14:49.386176 conifer-1.4b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      720 2023-11-23 13:14:38.000000 conifer-1.4b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 13:14:49.386176 conifer-1.4b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-23 13:14:38.000000 conifer-1.4b1/tests/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-11-23 13:14:38.000000 conifer-1.4b1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2023-11-23 13:14:38.000000 conifer-1.4b1/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2023-11-23 13:14:38.000000 conifer-1.4b1/tests/test_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2023-11-23 13:14:38.000000 conifer-1.4b1/tests/test_onnx_to_hls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2023-11-23 13:14:38.000000 conifer-1.4b1/tests/test_save_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2023-11-23 13:14:38.000000 conifer-1.4b1/tests/test_skl_to_hls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2023-11-23 13:14:38.000000 conifer-1.4b1/tests/test_tf_df.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2023-11-23 13:14:38.000000 conifer-1.4b1/tests/test_xgb_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2023-11-23 13:14:38.000000 conifer-1.4b1/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.832729 conifer-1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.808729 conifer-1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.812729 conifer-1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-27 15:26:08.000000 conifer-1.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-27 15:26:08.000000 conifer-1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-27 15:26:08.000000 conifer-1.5/Jenkinsfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 15:26:08.000000 conifer-1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 15:26:08.000000 conifer-1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-27 15:26:17.832729 conifer-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-27 15:26:08.000000 conifer-1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.812729 conifer-1.5/conifer/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-27 15:26:08.000000 conifer-1.5/conifer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.812729 conifer-1.5/conifer/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.816729 conifer-1.5/conifer/backends/boards/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/boards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/boards/boards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.808729 conifer-1.5/conifer/backends/boards/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.816729 conifer-1.5/conifer/backends/boards/configs/alveo/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/boards/configs/alveo/xilinx_u200_gen3x16_xdma_2_202110_1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.816729 conifer-1.5/conifer/backends/boards/configs/zynq/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/boards/configs/zynq/kr260.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/boards/configs/zynq/kv260.json
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/boards/configs/zynq/pynq_z2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/boards/configs/zynq/ultra96v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/boards/configs/zynq/zcu102.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/boards/configs/zynq/zcu104.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.816729 conifer-1.5/conifer/backends/boards/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/boards/src/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/boards/src/build_bit.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.816729 conifer-1.5/conifer/backends/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/cpp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.816729 conifer-1.5/conifer/backends/cpp/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/cpp/include/conifer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.816729 conifer-1.5/conifer/backends/cpp/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/cpp/template/bridge.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/cpp/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.816729 conifer-1.5/conifer/backends/fpu/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/fpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/fpu/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.820729 conifer-1.5/conifer/backends/fpu/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/fpu/src/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/fpu/src/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/fpu/src/build_hls.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/fpu/src/changes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/fpu/src/fpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/fpu/src/fpu.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16002 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/fpu/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.820729 conifer-1.5/conifer/backends/vhdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.820729 conifer-1.5/conifer/backends/vhdl/firmware/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/firmware/AddReduce.vhd
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/firmware/BDT.vhd
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/firmware/BDTTestbench.vhd
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/firmware/BDTTop.vhd
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/firmware/Constants.vhd
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/firmware/SimulationInput.vhd
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/firmware/SimulationOutput.vhd
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/firmware/TestUtil.vhd
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/firmware/Tree.vhd
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/firmware/Types.vhd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.820729 conifer-1.5/conifer/backends/vhdl/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/scripts/ghdl_compile.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/scripts/modelsim_compile.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/scripts/synth.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/scripts/xsim_compile.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/simulators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/vhdl/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.824729 conifer-1.5/conifer/backends/xilinxhls/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/xilinxhls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.824729 conifer-1.5/conifer/backends/xilinxhls/firmware/
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/xilinxhls/firmware/BDT_rolled.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/xilinxhls/firmware/BDT_unrolled.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.824729 conifer-1.5/conifer/backends/xilinxhls/hls-template/
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/xilinxhls/hls-template/bridge.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/xilinxhls/hls-template/build_hls.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.824729 conifer-1.5/conifer/backends/xilinxhls/hls-template/firmware/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/xilinxhls/hls-template/firmware/BDT_rolled.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/xilinxhls/hls-template/firmware/BDT_unrolled.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/xilinxhls/hls-template/firmware/myproject.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/xilinxhls/hls-template/firmware/myproject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/xilinxhls/hls-template/myproject_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/xilinxhls/hls-template/vivado_synth.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/xilinxhls/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-05-27 15:26:08.000000 conifer-1.5/conifer/backends/xilinxhls/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.824729 conifer-1.5/conifer/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-27 15:26:08.000000 conifer-1.5/conifer/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-27 15:26:08.000000 conifer-1.5/conifer/converters/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-27 15:26:08.000000 conifer-1.5/conifer/converters/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-27 15:26:08.000000 conifer-1.5/conifer/converters/tmva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-27 15:26:08.000000 conifer-1.5/conifer/converters/xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-27 15:26:08.000000 conifer-1.5/conifer/converters/ydf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-27 15:26:08.000000 conifer-1.5/conifer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.824729 conifer-1.5/conifer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-27 15:26:08.000000 conifer-1.5/conifer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-27 15:26:08.000000 conifer-1.5/conifer/utils/fixed_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-27 15:26:08.000000 conifer-1.5/conifer/utils/fixed_point_conversions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-27 15:26:08.000000 conifer-1.5/conifer/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.832729 conifer-1.5/conifer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-27 15:26:17.000000 conifer-1.5/conifer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-27 15:26:17.000000 conifer-1.5/conifer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:26:17.000000 conifer-1.5/conifer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 15:26:17.000000 conifer-1.5/conifer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 15:26:17.000000 conifer-1.5/conifer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    28385 2024-05-27 15:26:08.000000 conifer-1.5/conifer_v1.png
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-27 15:26:08.000000 conifer-1.5/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.808729 conifer-1.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.828729 conifer-1.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-27 15:26:08.000000 conifer-1.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-27 15:26:08.000000 conifer-1.5/docs/source/fpu.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-27 15:26:08.000000 conifer-1.5/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.828729 conifer-1.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-27 15:26:08.000000 conifer-1.5/examples/build_fpu_alveo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-27 15:26:08.000000 conifer-1.5/examples/build_fpu_pynq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-27 15:26:08.000000 conifer-1.5/examples/hls_accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-27 15:26:08.000000 conifer-1.5/examples/model_saving_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-27 15:26:08.000000 conifer-1.5/examples/pruned_xgboost_to_hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-27 15:26:08.000000 conifer-1.5/examples/sklearn_RandomForest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-27 15:26:08.000000 conifer-1.5/examples/sklearn_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-27 15:26:08.000000 conifer-1.5/examples/sklearn_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-27 15:26:08.000000 conifer-1.5/examples/sklearn_to_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-27 15:26:08.000000 conifer-1.5/examples/sklearn_to_fpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-27 15:26:08.000000 conifer-1.5/examples/sklearn_to_hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-27 15:26:08.000000 conifer-1.5/examples/sklearn_to_vhdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-27 15:26:08.000000 conifer-1.5/examples/xgboost_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-27 15:26:08.000000 conifer-1.5/examples/xgboost_to_hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-27 15:26:08.000000 conifer-1.5/examples/ydf_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-27 15:26:08.000000 conifer-1.5/examples/ydf_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-27 15:26:08.000000 conifer-1.5/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:26:17.832729 conifer-1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-27 15:26:08.000000 conifer-1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:17.832729 conifer-1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:26:08.000000 conifer-1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 15:26:08.000000 conifer-1.5/tests/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-27 15:26:08.000000 conifer-1.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-27 15:26:08.000000 conifer-1.5/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-27 15:26:08.000000 conifer-1.5/tests/test_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-27 15:26:08.000000 conifer-1.5/tests/test_onnx_to_hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-27 15:26:08.000000 conifer-1.5/tests/test_save_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-27 15:26:08.000000 conifer-1.5/tests/test_skl_to_hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-27 15:26:08.000000 conifer-1.5/tests/test_xgb_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-27 15:26:08.000000 conifer-1.5/tests/test_ydf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-27 15:26:08.000000 conifer-1.5/tests/util.py
```

### Comparing `conifer-1.4b1/.github/workflows/python-publish.yml` & `conifer-1.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/Jenkinsfile` & `conifer-1.5/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/LICENSE` & `conifer-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/PKG-INFO` & `conifer-1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: conifer
-Version: 1.4b1
-Summary: BDT Inference for FPGAs
-Home-page: https://github.com/thesps/conifer
-Author: Sioni Summers
-Author-email: sioni@cern.ch
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: pybind11
-Requires-Dist: packaging
-
 <img src="https://github.com/thesps/conifer/raw/master/conifer_v1.png" width="250" alt="conifer">
 
 Conifer translates trained Boosted Decision Trees to FPGA firmware for extreme low latency inference. 
 
 # Installation
 Conifer is on the Python Package Index, so install it like:
 ```
@@ -114,9 +99,25 @@
 # X = np.zeros(16, dtype='int32')
 # fpu.predict(X)
 ```
 
 
 </details>
 
+# Development
+1. Clone the github repository: `git clone https://github.com/thesps/conifer`
+1. Install the dependencies listed in the *Installation* section. For instance:
+    - Clone nlohmann json: `git clone https://github.com/nlohmann/json`
+    - Clone Arbitrary Precision: `git clone https://github.com/Xilinx/HLS_arbitrary_Precision_Types`
+    - Set the env variables `JSON_ROOT` and `XILINX_AP_INCLUDE` as the `include` directory in them respectively e.g.
+    ```shell
+    export XILINX_AP_INCLUDE=$(pwd)/HLS_arbitrary_Precision_Types/include
+    export JSON_ROOT=$(pwd)/json/include
+    ```
+1. Go into the Conifer project directory: `cd conifer`
+1. Install the python development dependencies: `pip install -r dev_requirements.txt`
+1. Run an example: `export PYTHONPATH="$(pwd):${PYTHONPATH}" && python examples/sklearn_to_cpp.py`
+1. Run a single unit test: `pytest tests/test_multiclass.py`
+1. Run all the unit tests: `pytest`
+
 # License
 Apart from the source code and binaries of the Forest Processing Unit (FPU), `conifer` is licensed under *Apache v2*. The FPU source code and binaries are licensed under the [*CERN-OHL-P v2*](https://cern.ch/cern-ohl) or later.
```

### Comparing `conifer-1.4b1/README.md` & `conifer-1.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: conifer
+Version: 1.5
+Summary: BDT Inference for FPGAs
+Home-page: https://github.com/thesps/conifer
+Author: Sioni Summers
+Author-email: sioni@cern.ch
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pybind11
+Requires-Dist: packaging
+
 <img src="https://github.com/thesps/conifer/raw/master/conifer_v1.png" width="250" alt="conifer">
 
 Conifer translates trained Boosted Decision Trees to FPGA firmware for extreme low latency inference. 
 
 # Installation
 Conifer is on the Python Package Index, so install it like:
 ```
@@ -99,9 +114,25 @@
 # X = np.zeros(16, dtype='int32')
 # fpu.predict(X)
 ```
 
 
 </details>
 
+# Development
+1. Clone the github repository: `git clone https://github.com/thesps/conifer`
+1. Install the dependencies listed in the *Installation* section. For instance:
+    - Clone nlohmann json: `git clone https://github.com/nlohmann/json`
+    - Clone Arbitrary Precision: `git clone https://github.com/Xilinx/HLS_arbitrary_Precision_Types`
+    - Set the env variables `JSON_ROOT` and `XILINX_AP_INCLUDE` as the `include` directory in them respectively e.g.
+    ```shell
+    export XILINX_AP_INCLUDE=$(pwd)/HLS_arbitrary_Precision_Types/include
+    export JSON_ROOT=$(pwd)/json/include
+    ```
+1. Go into the Conifer project directory: `cd conifer`
+1. Install the python development dependencies: `pip install -r dev_requirements.txt`
+1. Run an example: `export PYTHONPATH="$(pwd):${PYTHONPATH}" && python examples/sklearn_to_cpp.py`
+1. Run a single unit test: `pytest tests/test_multiclass.py`
+1. Run all the unit tests: `pytest`
+
 # License
 Apart from the source code and binaries of the Forest Processing Unit (FPU), `conifer` is licensed under *Apache v2*. The FPU source code and binaries are licensed under the [*CERN-OHL-P v2*](https://cern.ch/cern-ohl) or later.
```

### Comparing `conifer-1.4b1/conifer/backends/__init__.py` & `conifer-1.5/conifer/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/boards/__init__.py` & `conifer-1.5/conifer/backends/boards/__init__.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/boards/boards.py` & `conifer-1.5/conifer/backends/boards/boards.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/boards/src/LICENSE` & `conifer-1.5/conifer/backends/boards/src/LICENSE`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/boards/src/build_bit.tcl` & `conifer-1.5/conifer/backends/boards/src/build_bit.tcl`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/common.py` & `conifer-1.5/conifer/backends/common.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/cpp/include/conifer.h` & `conifer-1.5/conifer/backends/cpp/include/conifer.h`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/cpp/writer.py` & `conifer-1.5/conifer/backends/cpp/writer.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/fpu/runtime.py` & `conifer-1.5/conifer/backends/fpu/runtime.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/fpu/src/LICENSE` & `conifer-1.5/conifer/backends/fpu/src/LICENSE`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/fpu/src/README.md` & `conifer-1.5/conifer/backends/fpu/src/README.md`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/fpu/src/build_hls.tcl` & `conifer-1.5/conifer/backends/fpu/src/build_hls.tcl`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/fpu/src/fpu.cpp` & `conifer-1.5/conifer/backends/fpu/src/fpu.cpp`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/fpu/src/fpu.h` & `conifer-1.5/conifer/backends/fpu/src/fpu.h`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/fpu/writer.py` & `conifer-1.5/conifer/backends/fpu/writer.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/vhdl/firmware/AddReduce.vhd` & `conifer-1.5/conifer/backends/vhdl/firmware/AddReduce.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/vhdl/firmware/BDT.vhd` & `conifer-1.5/conifer/backends/vhdl/firmware/BDT.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/vhdl/firmware/BDTTestbench.vhd` & `conifer-1.5/conifer/backends/vhdl/firmware/BDTTestbench.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/vhdl/firmware/BDTTop.vhd` & `conifer-1.5/conifer/backends/vhdl/firmware/BDTTop.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/vhdl/firmware/SimulationInput.vhd` & `conifer-1.5/conifer/backends/vhdl/firmware/SimulationInput.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/vhdl/firmware/SimulationOutput.vhd` & `conifer-1.5/conifer/backends/vhdl/firmware/SimulationOutput.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/vhdl/firmware/TestUtil.vhd` & `conifer-1.5/conifer/backends/vhdl/firmware/TestUtil.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/vhdl/firmware/Tree.vhd` & `conifer-1.5/conifer/backends/vhdl/firmware/Tree.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/vhdl/firmware/Types.vhd` & `conifer-1.5/conifer/backends/vhdl/firmware/Types.vhd`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/vhdl/scripts/ghdl_compile.sh` & `conifer-1.5/conifer/backends/vhdl/scripts/ghdl_compile.sh`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/vhdl/scripts/modelsim_compile.sh` & `conifer-1.5/conifer/backends/vhdl/scripts/modelsim_compile.sh`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/vhdl/simulators.py` & `conifer-1.5/conifer/backends/vhdl/simulators.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/vhdl/writer.py` & `conifer-1.5/conifer/backends/vhdl/writer.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/xilinxhls/firmware/BDT_rolled.h` & `conifer-1.5/conifer/backends/xilinxhls/firmware/BDT_rolled.h`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/xilinxhls/hls-template/bridge.cpp` & `conifer-1.5/conifer/backends/xilinxhls/hls-template/bridge.cpp`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/xilinxhls/hls-template/build_hls.tcl` & `conifer-1.5/conifer/backends/xilinxhls/hls-template/build_hls.tcl`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     open_solution -reset "solution1"
 } else {
     open_solution "solution1"
 }
 
 open_solution -reset "solution1" -flow_target ${flow_target}
 set_part ${part}
-create_clock -period 5 -name default
+create_clock -period ${clock_period} -name default
 
 config_interface -m_axi_addr64=${m_axi_addr64}
 
 if {$opt(csim)} {
     csim_design
 }
```

### Comparing `conifer-1.4b1/conifer/backends/xilinxhls/hls-template/firmware/myproject.cpp` & `conifer-1.5/conifer/backends/xilinxhls/hls-template/firmware/myproject.cpp`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/xilinxhls/hls-template/myproject_test.cpp` & `conifer-1.5/conifer/backends/xilinxhls/hls-template/myproject_test.cpp`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/xilinxhls/runtime.py` & `conifer-1.5/conifer/backends/xilinxhls/runtime.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/backends/xilinxhls/writer.py` & `conifer-1.5/conifer/backends/xilinxhls/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             fin = open(f'{filedir}/hls-template/firmware/BDT_unrolled.cpp', 'r')
             fout = open(f'{cfg.output_dir}/firmware/BDT.cpp', 'w')
             for line in fin.readlines():
                 if '// conifer insert tree_scores' in line:
                     newline = ''
                     for it, trees in enumerate(self.trees):
                         for ic, tree in enumerate(trees):
-                            newline += f'  scores[{it}][{ic}] = tree_{it}_{ic}.decision_function(x);\n'
+                            newline += f'  scores[{ic}][{it}] = tree_{ic}_{it}.decision_function(x);\n'
                 else:
                     newline = line
                 fout.write(newline)
         else:
             copyfile(f'{filedir}/hls-template/firmware/BDT_rolled.cpp',
                      f'{cfg.output_dir}/firmware/BDT.cpp')
 
@@ -223,15 +223,15 @@
         fout.write("// The trees\n")
         # loop over trees
         for itree, trees in enumerate(self.trees):
             # loop over classes
             for iclass, tree in enumerate(trees):
                 fout.write(f'static const BDT::Tree<{itree*nc+iclass}, {tree.n_nodes()}, {tree.n_leaves()}')
                 fout.write(f', input_arr_t, score_t, threshold_t>')
-                fout.write(f' tree_{itree}_{iclass} = {{\n')
+                fout.write(f' tree_{iclass}_{itree} = {{\n')
                 # loop over fields
                 for ifield, field in enumerate(tree_fields):
                     newline = '    {'
                     newline += ','.join(map(str, getattr(tree, field)))
                     newline += '}'
                     if ifield < len(tree_fields) - 1:
                         newline += ','
```

### Comparing `conifer-1.4b1/conifer/converters/__init__.py` & `conifer-1.5/conifer/converters/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 logger = logging.getLogger(__name__)
 
 _converter_map = {}
 import importlib
-for module in ['sklearn', 'tmva', 'xgboost', 'onnx', 'tf_df']:
+for module in ['sklearn', 'tmva', 'xgboost', 'onnx', 'ydf']:
   try:
     the_module = importlib.import_module(f'conifer.converters.{module}')
     _converter_map[module] = the_module
   except ImportError:
     logger.warn(f'Could not import conifer {module} converter')
 
 from conifer.model import make_model
@@ -38,11 +38,11 @@
   return make_model(ensembleDict, config)
 
 def convert_from_onnx(model, config=None):
   '''Convert a BDT from an ONNX model and configuration'''
   ensembleDict = onnx.convert(model)
   return make_model(ensembleDict, config)
 
-def convert_from_tf_df(model, config=None):
-  '''Convert a BDT from an TF-DF model and configuration'''
-  ensembleDict = tf_df.convert(model)
+def convert_from_ydf(model, config=None):
+  '''Convert a BDT from an Yggdrasil Decision Forests model and configuration'''
+  ensembleDict = ydf.convert(model)
   return make_model(ensembleDict, config)
```

### Comparing `conifer-1.4b1/conifer/converters/onnx.py` & `conifer-1.5/conifer/converters/onnx.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/converters/sklearn.py` & `conifer-1.5/conifer/converters/sklearn.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/converters/tmva.py` & `conifer-1.5/conifer/converters/tmva.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/converters/xgboost.py` & `conifer-1.5/conifer/converters/xgboost.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/model.py` & `conifer-1.5/conifer/model.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/utils/fixed_point.py` & `conifer-1.5/conifer/utils/fixed_point.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/utils/fixed_point_conversions.cpp` & `conifer-1.5/conifer/utils/fixed_point_conversions.cpp`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer/utils/misc.py` & `conifer-1.5/conifer/utils/misc.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/conifer.egg-info/PKG-INFO` & `conifer-1.5/conifer.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conifer
-Version: 1.4b1
+Version: 1.5
 Summary: BDT Inference for FPGAs
 Home-page: https://github.com/thesps/conifer
 Author: Sioni Summers
 Author-email: sioni@cern.ch
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -114,9 +114,25 @@
 # X = np.zeros(16, dtype='int32')
 # fpu.predict(X)
 ```
 
 
 </details>
 
+# Development
+1. Clone the github repository: `git clone https://github.com/thesps/conifer`
+1. Install the dependencies listed in the *Installation* section. For instance:
+    - Clone nlohmann json: `git clone https://github.com/nlohmann/json`
+    - Clone Arbitrary Precision: `git clone https://github.com/Xilinx/HLS_arbitrary_Precision_Types`
+    - Set the env variables `JSON_ROOT` and `XILINX_AP_INCLUDE` as the `include` directory in them respectively e.g.
+    ```shell
+    export XILINX_AP_INCLUDE=$(pwd)/HLS_arbitrary_Precision_Types/include
+    export JSON_ROOT=$(pwd)/json/include
+    ```
+1. Go into the Conifer project directory: `cd conifer`
+1. Install the python development dependencies: `pip install -r dev_requirements.txt`
+1. Run an example: `export PYTHONPATH="$(pwd):${PYTHONPATH}" && python examples/sklearn_to_cpp.py`
+1. Run a single unit test: `pytest tests/test_multiclass.py`
+1. Run all the unit tests: `pytest`
+
 # License
 Apart from the source code and binaries of the Forest Processing Unit (FPU), `conifer` is licensed under *Apache v2*. The FPU source code and binaries are licensed under the [*CERN-OHL-P v2*](https://cern.ch/cern-ohl) or later.
```

### Comparing `conifer-1.4b1/conifer.egg-info/SOURCES.txt` & `conifer-1.5/conifer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 Jenkinsfile
 LICENSE
 MANIFEST.in
 README.md
 conifer_v1.png
+dev_requirements.txt
 pytest.ini
 setup.py
 .github/workflows/python-publish.yml
 conifer/__init__.py
 conifer/model.py
 conifer.egg-info/PKG-INFO
 conifer.egg-info/SOURCES.txt
@@ -69,17 +70,17 @@
 conifer/backends/xilinxhls/hls-template/firmware/BDT_rolled.cpp
 conifer/backends/xilinxhls/hls-template/firmware/BDT_unrolled.cpp
 conifer/backends/xilinxhls/hls-template/firmware/myproject.cpp
 conifer/backends/xilinxhls/hls-template/firmware/myproject.h
 conifer/converters/__init__.py
 conifer/converters/onnx.py
 conifer/converters/sklearn.py
-conifer/converters/tf_df.py
 conifer/converters/tmva.py
 conifer/converters/xgboost.py
+conifer/converters/ydf.py
 conifer/utils/__init__.py
 conifer/utils/fixed_point.py
 conifer/utils/fixed_point_conversions.cpp
 conifer/utils/misc.py
 docs/source/conf.py
 docs/source/fpu.rst
 docs/source/index.rst
@@ -91,21 +92,22 @@
 examples/sklearn_RandomForest.py
 examples/sklearn_multiclass.py
 examples/sklearn_regression.py
 examples/sklearn_to_cpp.py
 examples/sklearn_to_fpu.py
 examples/sklearn_to_hls.py
 examples/sklearn_to_vhdl.py
-examples/tf_df_binary.py
-examples/tf_df_multiclass.py
 examples/xgboost_multiclass.py
 examples/xgboost_to_hls.py
+examples/ydf_binary.py
+examples/ydf_multiclass.py
+tests/__init__.py
 tests/cleanup.sh
 tests/conftest.py
 tests/test_backends.py
 tests/test_multiclass.py
 tests/test_onnx_to_hls.py
 tests/test_save_load.py
 tests/test_skl_to_hls.py
-tests/test_tf_df.py
 tests/test_xgb_converter.py
+tests/test_ydf.py
 tests/util.py
```

### Comparing `conifer-1.4b1/conifer_v1.png` & `conifer-1.5/conifer_v1.png`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/docs/source/conf.py` & `conifer-1.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/docs/source/fpu.rst` & `conifer-1.5/docs/source/fpu.rst`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/examples/build_fpu_alveo.py` & `conifer-1.5/examples/build_fpu_alveo.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/examples/build_fpu_pynq.py` & `conifer-1.5/examples/build_fpu_pynq.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/examples/hls_accelerator.py` & `conifer-1.5/examples/hls_accelerator.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/examples/model_saving_loading.py` & `conifer-1.5/examples/model_saving_loading.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/examples/pruned_xgboost_to_hls.py` & `conifer-1.5/examples/pruned_xgboost_to_hls.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/examples/sklearn_RandomForest.py` & `conifer-1.5/examples/sklearn_RandomForest.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/examples/sklearn_multiclass.py` & `conifer-1.5/examples/sklearn_multiclass.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/examples/sklearn_regression.py` & `conifer-1.5/examples/sklearn_regression.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/examples/sklearn_to_cpp.py` & `conifer-1.5/examples/sklearn_to_cpp.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/examples/sklearn_to_fpu.py` & `conifer-1.5/examples/sklearn_to_fpu.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/examples/sklearn_to_hls.py` & `conifer-1.5/examples/sklearn_to_hls.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/examples/sklearn_to_vhdl.py` & `conifer-1.5/examples/sklearn_to_vhdl.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/examples/tf_df_binary.py` & `conifer-1.5/examples/ydf_multiclass.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,56 @@
-# Example BDT creation with TensorFlow Decision Forests (https://www.tensorflow.org/decision_forests)
-
-import numpy as np
-import tensorflow_decision_forests as tfdf
-from sklearn.datasets import make_hastie_10_2
-import conifer
-import datetime
-import logging
-import sys
-
-logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
-
-# Create dataset
-X, y = make_hastie_10_2(random_state=0)
-
-# Train a BDT
-model = tfdf.keras.GradientBoostedTreesModel(
-    num_trees=1, max_depth=2, verbose=0, apply_link_function=False)
-model.fit(x=X, y=y)
-
-stamp = int(datetime.datetime.now().timestamp())
-# Create a conifer config
-cpp_cfg = conifer.backends.cpp.auto_config()
-#cpp_cfg["Precision"] = "float"
-# Set the output directory to something unique
-cpp_cfg['OutputDir'] = 'prj_cpp_{}'.format(stamp)
-
-# Create and compile the model
-cpp_model = conifer.converters.convert_from_tf_df(model, cpp_cfg)
-cpp_model.compile()
-
-# Create a conifer config
-hls_cfg = conifer.backends.xilinxhls.auto_config()
-#hls_cfg["Precision"] = "float"
-# Set the output directory to something unique
-hls_cfg['OutputDir'] = 'prj_hls_{}'.format(stamp)
-
-# Create and compile the model
-hls_model = conifer.converters.convert_from_tf_df(model, hls_cfg)
-hls_model.compile()
-
-# Run the C++ and get the output
-y_cpp = cpp_model.decision_function(X)
-y_hls = hls_model.decision_function(X)
-y_skl = model.predict(X, verbose=0)[:, 0]
-
-if np.array_equal(y_hls, y_cpp):
-    print(f'HLS and CPP predictions agree 100% ({len(y_cpp)}/{len(y_cpp)})')
-else:
-    abs_diff = np.abs(y_hls - y_cpp)
-    rel_diff = abs_diff / np.abs(y_hls)
-    print(
-        f'HLS and CPP predictions disagree. Biggest absolute difference: {abs_diff.max():.4f}, biggest relative difference: {rel_diff.max():.4f}')
+"""Example of BDT creation with Yggdrasil Decision Forests (https://ydf.readthedocs.io)."""
+
+import datetime
+import logging
+import sys
+
+import numpy as np
+import ydf
+from sklearn.datasets import load_iris
+import conifer
+
+logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
+
+# Create dataset
+iris = load_iris()
+X, y = iris.data, iris.target
+
+# Train a BDT
+model = ydf.GradientBoostedTreesLearner(
+    num_trees=100, max_depth=6, apply_link_function=False, label="y"
+).train({"x": X, "y": y})
+
+stamp = int(datetime.datetime.now().timestamp())
+# Create a conifer config
+cpp_cfg = conifer.backends.cpp.auto_config()
+# cpp_cfg["Precision"] = "float"
+# Set the output directory to something unique
+cpp_cfg["OutputDir"] = "prj_cpp_{}".format(stamp)
+
+# Create and compile the model
+cpp_model = conifer.converters.convert_from_ydf(model, cpp_cfg)
+cpp_model.compile()
+
+# Create a conifer config
+hls_cfg = conifer.backends.xilinxhls.auto_config()
+# hls_cfg["Precision"] = "float"
+# Set the output directory to something unique
+hls_cfg["OutputDir"] = "prj_hls_{}".format(stamp)
+
+# Create and compile the model
+hls_model = conifer.converters.convert_from_ydf(model, hls_cfg)
+hls_model.compile()
+
+# Run the C++ and get the output
+y_cpp = cpp_model.decision_function(X)
+y_hls = hls_model.decision_function(X)
+y_skl = model.predict({"x": X})
+
+if np.array_equal(y_hls, y_cpp):
+    print(f"HLS and CPP predictions agree 100% ({len(y_cpp)}/{len(y_cpp)})")
+else:
+    abs_diff = np.abs(y_hls - y_cpp)
+    rel_diff = abs_diff / np.abs(y_hls)
+    print(
+        f"HLS and CPP predictions disagree. Biggest absolute difference: {abs_diff.max():.4f}, biggest relative difference: {rel_diff.max():.4f}"
+    )
```

### Comparing `conifer-1.4b1/examples/tf_df_multiclass.py` & `conifer-1.5/examples/ydf_binary.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,58 @@
-# Example BDT creation with TensorFlow Decision Forests (https://www.tensorflow.org/decision_forests)
-
-import numpy as np
-import tensorflow_decision_forests as tfdf
-from sklearn.datasets import load_iris
-import conifer
-import datetime
-import logging
-import sys
-
-logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
-
-# Create dataset
-iris = load_iris()
-X, y = iris.data, iris.target
-
-# Train a BDT
-model = tfdf.keras.GradientBoostedTreesModel(
-    num_trees=100, max_depth=6, verbose=0)
-model.fit(x=X, y=y)
-
-stamp = int(datetime.datetime.now().timestamp())
-# Create a conifer config
-cpp_cfg = conifer.backends.cpp.auto_config()
-#cpp_cfg["Precision"] = "float"
-# Set the output directory to something unique
-cpp_cfg['OutputDir'] = 'prj_cpp_{}'.format(stamp)
-
-# Create and compile the model
-cpp_model = conifer.converters.convert_from_tf_df(model, cpp_cfg)
-cpp_model.compile()
-
-# Create a conifer config
-hls_cfg = conifer.backends.xilinxhls.auto_config()
-#hls_cfg["Precision"] = "float"
-# Set the output directory to something unique
-hls_cfg['OutputDir'] = 'prj_hls_{}'.format(stamp)
-
-# Create and compile the model
-hls_model = conifer.converters.convert_from_tf_df(model, hls_cfg)
-hls_model.compile()
-
-# Run the C++ and get the output
-y_cpp = cpp_model.decision_function(X)
-y_hls = hls_model.decision_function(X)
-y_skl = model.predict(X, verbose=0)
-
-if np.array_equal(y_hls, y_cpp):
-    print(f'HLS and CPP predictions agree 100% ({len(y_cpp)}/{len(y_cpp)})')
-else:
-    abs_diff = np.abs(y_hls - y_cpp)
-    rel_diff = abs_diff / np.abs(y_hls)
-    print(
-        f'HLS and CPP predictions disagree. Biggest absolute difference: {abs_diff.max():.4f}, biggest relative difference: {rel_diff.max():.4f}')
+"""Example of BDT creation with Yggdrasil Decision Forests (https://ydf.readthedocs.io)."""
+
+import datetime
+import logging
+import sys
+
+import numpy as np
+import ydf
+from sklearn.datasets import make_hastie_10_2
+import conifer
+
+logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
+
+# Create dataset
+X, y = make_hastie_10_2(random_state=0)
+y = y == 1  # Converts Hastie's labels from {-1, 1} to {False, True}.
+
+# Train a Gradient Boosted Decision Trees model using YDF.
+model = ydf.GradientBoostedTreesLearner(
+    num_trees=1,
+    max_depth=2,
+    apply_link_function=False,
+    label="y",
+).train({"x": X, "y": y})
+
+# Create a Conifer configuration.
+stamp = int(datetime.datetime.now().timestamp())
+cpp_cfg = conifer.backends.cpp.auto_config()
+# cpp_cfg["Precision"] = "float"  # Optional float precision.
+cpp_cfg["OutputDir"] = "prj_cpp_{}".format(stamp)
+
+# Convert the YDF model to a C++ Conifer model.
+cpp_model = conifer.converters.convert_from_ydf(model, cpp_cfg)
+cpp_model.compile()
+
+# Create a conifer config
+hls_cfg = conifer.backends.xilinxhls.auto_config()
+# hls_cfg["Precision"] = "float"  # Optional float precision.
+hls_cfg["OutputDir"] = "prj_hls_{}".format(stamp)
+
+# Convert the YDF model to a HLS Conifer model.
+hls_model = conifer.converters.convert_from_ydf(model, hls_cfg)
+hls_model.compile()
+
+# Compare the predictions of YDF, C++ Conifer, and HLS Conifer model.
+y_cpp = cpp_model.decision_function(X)
+y_hls = hls_model.decision_function(X)
+y_ydf = model.predict({"x": X})
+
+
+if np.array_equal(y_hls, y_cpp):
+    print(f"HLS and CPP predictions agree 100% ({len(y_cpp)}/{len(y_cpp)})")
+else:
+    abs_diff = np.abs(y_hls - y_cpp)
+    rel_diff = abs_diff / np.abs(y_hls)
+    print(
+        f"HLS and CPP predictions disagree. Biggest absolute difference: {abs_diff.max():.4f}, biggest relative difference: {rel_diff.max():.4f}"
+    )
```

### Comparing `conifer-1.4b1/examples/xgboost_multiclass.py` & `conifer-1.5/examples/xgboost_multiclass.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/examples/xgboost_to_hls.py` & `conifer-1.5/examples/xgboost_to_hls.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/setup.py` & `conifer-1.5/setup.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/tests/test_backends.py` & `conifer-1.5/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/tests/test_multiclass.py` & `conifer-1.5/tests/test_multiclass.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from sklearn.datasets import load_iris
 from sklearn.ensemble import GradientBoostingClassifier
 import datetime
 import onnxmltools
 import onnx
 import numpy as np
 import conifer
-import util
+from tests import util
 import pytest
 
 iris = load_iris()
 X, y = iris.data, iris.target
 
 def train_model():
     clf = GradientBoostingClassifier(n_estimators=20, learning_rate=1.0,
```

### Comparing `conifer-1.4b1/tests/test_onnx_to_hls.py` & `conifer-1.5/tests/test_onnx_to_hls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-import util
+from tests import util
 import onnxmltools
 import onnx
 
 @pytest.fixture
 def train_onnx():
     # Example BDT creation from: https://scikit-learn.org/stable/modules/ensemble.html
     from sklearn.datasets import make_hastie_10_2
```

### Comparing `conifer-1.4b1/tests/test_save_load.py` & `conifer-1.5/tests/test_save_load.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import util
+from tests import util
 import numpy as np
 import conifer
 import json
 
 '''
 Test conifer's model saving and loading functionality by loading some models and checking the predictions
 match the original.
```

### Comparing `conifer-1.4b1/tests/test_xgb_converter.py` & `conifer-1.5/tests/test_xgb_converter.py`

 * *Files identical despite different names*

### Comparing `conifer-1.4b1/tests/util.py` & `conifer-1.5/tests/util.py`

 * *Files identical despite different names*

