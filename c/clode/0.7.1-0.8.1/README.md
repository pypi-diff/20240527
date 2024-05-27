# Comparing `tmp/clode-0.7.1.tar.gz` & `tmp/clode-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clode-0.7.1.tar", last modified: Wed Mar  6 22:55:05 2024, max compression
+gzip compressed data, was "clode-0.8.1.tar", last modified: Mon May 27 16:03:43 2024, max compression
```

## Comparing `clode-0.7.1.tar` & `clode-0.8.1.tar`

### file list

```diff
@@ -1,227 +1,234 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.136681 clode-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-06 22:53:28.000000 clode-0.7.1/.bazeliskrc
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-06 22:53:28.000000 clode-0.7.1/.bazelversion
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-06 22:53:28.000000 clode-0.7.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.096681 clode-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.104681 clode-0.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-06 22:53:28.000000 clode-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-06 22:53:28.000000 clode-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.104681 clode-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-03-06 22:53:28.000000 clode-0.7.1/.github/workflows/bazel_build_linux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-06 22:53:28.000000 clode-0.7.1/.github/workflows/bazel_build_windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-06 22:53:28.000000 clode-0.7.1/.github/workflows/bazel_test_mac.yml
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-06 22:53:28.000000 clode-0.7.1/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-03-06 22:53:28.000000 clode-0.7.1/.github/workflows/deploy_mkdocs_pages.yml
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-06 22:53:28.000000 clode-0.7.1/.github/workflows/draft_pdf.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-03-06 22:53:28.000000 clode-0.7.1/.github/workflows/scorecards.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-03-06 22:53:28.000000 clode-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 22:53:28.000000 clode-0.7.1/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-06 22:53:28.000000 clode-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-03-06 22:53:28.000000 clode-0.7.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-03-06 22:55:05.136681 clode-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-06 22:53:28.000000 clode-0.7.1/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-06 22:53:28.000000 clode-0.7.1/WORKSPACE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.104681 clode-0.7.1/bazel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/clode_http_archive.bzl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.108681 clode-0.7.1/bazel/external/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/external/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/external/fmtlib.BUILD
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/external/opencl_windows.BUILD
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/external/pybind11.BUILD
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/external/python.BUILD
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/external/spdlog.BUILD
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/external_deps.bzl
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/get_python_libs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.108681 clode-0.7.1/bazel/python/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/python/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/python/BUILD.tpl
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/python/python.bzl
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/python/python_native.bzl
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/python/variety.tpl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.108681 clode-0.7.1/bazel/remote_config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/remote_config/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/remote_config/common.bzl
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/repositories.bzl
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/repository_locations.bzl
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-06 22:53:28.000000 clode-0.7.1/bazel/repository_locations_utils.bzl
--rw-r--r--   0 runner    (1001) docker     (127)    17104 2024-03-06 22:53:28.000000 clode-0.7.1/bazelisk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.108681 clode-0.7.1/clode/
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-06 22:53:28.000000 clode-0.7.1/clode/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-03-06 22:53:28.000000 clode-0.7.1/clode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.112681 clode-0.7.1/clode/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/CLODE.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/CLODE.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/CLODEfeatures.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/CLODEfeatures.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/CLODEpython.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7347 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/CLODEtrajectory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/CLODEtrajectory.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.116681 clode-0.7.1/clode/cpp/OpenCL/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/OpenCL/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)   299120 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/OpenCL/cl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)   326155 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/OpenCL/cl2.hpp
--rw-r--r--   0 runner    (1001) docker     (127)   396729 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/OpenCL/opencl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18229 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/OpenCLResource.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/OpenCLResource.hpp
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/clODE_random.cl
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/clODE_struct_defs.cl
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/clODE_utilities.cl
--rw-r--r--   0 runner    (1001) docker     (127)    13003 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/clode_cpp_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/features.cl
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/initializeObserver.cl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.116681 clode-0.7.1/clode/cpp/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/logging/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/logging/MatlabSink.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/logging/PythonSink.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.116681 clode-0.7.1/clode/cpp/observers/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/observers/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/observers/observer_basic.clh
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/observers/observer_basic_allVar.clh
--rw-r--r--   0 runner    (1001) docker     (127)     9845 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/observers/observer_local_maximum.clh
--rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/observers/observer_neighborhood_1.clh
--rw-r--r--   0 runner    (1001) docker     (127)    13466 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/observers/observer_neighborhood_2.clh
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/observers/observer_template.clh
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/observers/observer_threshold_1.clh
--rw-r--r--   0 runner    (1001) docker     (127)    17012 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/observers/observer_threshold_2.clh
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/observers.cl
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/odedriver.cl
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/realtype.cl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.120681 clode-0.7.1/clode/cpp/steppers/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/steppers/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/steppers/adaptive_bs23.clh
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/steppers/adaptive_dp45.clh
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/steppers/adaptive_explicit_step.clh
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/steppers/adaptive_he12.clh
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/steppers/adaptive_rkck.clh
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/steppers/fixed_explicit_Euler.clh
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/steppers/fixed_explicit_RK4.clh
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/steppers/fixed_explicit_Trapezoidal.clh
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/steppers/fixed_explicit_step.clh
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/steppers/fixed_explicit_stochastic_Euler.clh
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/steppers.cl
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/trajectory.cl
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-06 22:53:28.000000 clode-0.7.1/clode/cpp/transient.cl
--rw-r--r--   0 runner    (1001) docker     (127)    13199 2024-03-06 22:53:28.000000 clode-0.7.1/clode/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    35186 2024-03-06 22:53:28.000000 clode-0.7.1/clode/function_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-03-06 22:53:28.000000 clode-0.7.1/clode/opencl_builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 22:53:28.000000 clode-0.7.1/clode/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-03-06 22:53:28.000000 clode-0.7.1/clode/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-03-06 22:53:28.000000 clode-0.7.1/clode/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-03-06 22:53:28.000000 clode-0.7.1/clode/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-03-06 22:53:28.000000 clode-0.7.1/clode/xpp_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.136681 clode-0.7.1/clode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-03-06 22:55:05.000000 clode-0.7.1/clode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-03-06 22:55:05.000000 clode-0.7.1/clode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 22:55:05.000000 clode-0.7.1/clode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-06 22:55:05.000000 clode-0.7.1/clode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.124681 clode-0.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-06 22:53:28.000000 clode-0.7.1/docs/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-06 22:53:28.000000 clode-0.7.1/docs/Ornstein-Uhlenbeck_process.md
--rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-03-06 22:53:28.000000 clode-0.7.1/docs/Ornstein-Uhlenbeck_process.png
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-03-06 22:53:28.000000 clode-0.7.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-06 22:53:28.000000 clode-0.7.1/docs/api_reference.md
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-06 22:53:28.000000 clode-0.7.1/docs/fast_and_slow_variables.md
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-03-06 22:53:28.000000 clode-0.7.1/docs/feature_extraction.md
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-03-06 22:53:28.000000 clode-0.7.1/docs/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-03-06 22:53:28.000000 clode-0.7.1/docs/init_runtime.md
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-03-06 22:53:28.000000 clode-0.7.1/docs/install.md
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-06 22:53:28.000000 clode-0.7.1/docs/logging_levels.md
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-03-06 22:53:28.000000 clode-0.7.1/docs/matlab.md
--rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-03-06 22:53:28.000000 clode-0.7.1/docs/pycon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-03-06 22:53:28.000000 clode-0.7.1/docs/querying_opencl.md
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-03-06 22:53:28.000000 clode-0.7.1/docs/specifying_odes.md
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-03-06 22:53:28.000000 clode-0.7.1/docs/spike_counting.md
--rw-r--r--   0 runner    (1001) docker     (127)    49954 2024-03-06 22:53:28.000000 clode-0.7.1/docs/spike_counting.png
--rw-r--r--   0 runner    (1001) docker     (127)    72190 2024-03-06 22:53:28.000000 clode-0.7.1/docs/spike_counting_trajectories.png
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-06 22:53:28.000000 clode-0.7.1/docs/trajectory_simulation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-06 22:53:28.000000 clode-0.7.1/docs/xpp_files.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.124681 clode-0.7.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-03-06 22:53:28.000000 clode-0.7.1/examples/Ornstein_Uhlenbeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-06 22:53:28.000000 clode-0.7.1/examples/chay_keizer.cl
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-03-06 22:53:28.000000 clode-0.7.1/examples/dump_device_performance.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-06 22:53:28.000000 clode-0.7.1/examples/dump_opencl_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-06 22:53:28.000000 clode-0.7.1/examples/fast_and_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-03-06 22:53:28.000000 clode-0.7.1/examples/spike_counting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.128681 clode-0.7.1/matlab/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/Chart.m
--rw-r--r--   0 runner    (1001) docker     (127)    13590 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/GridSimulation.m
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/InitialValueProblem.m
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    17034 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/clODE.m
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/clODEfeatures.m
--rw-r--r--   0 runner    (1001) docker     (127)    16052 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/clODEfeaturesmex.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/clODEmex.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/clODEmexHelpers.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/clODEtrajectory.m
--rw-r--r--   0 runner    (1001) docker     (127)    14263 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/clODEtrajectorymex.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/clickTrajectory.m
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/compileCLODEmex.m
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/cppclass.m
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/functionSignatures.json
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/generate_pointset.m
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/gridKeyPress.m
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/gridfigure.m
--rw-r--r--   0 runner    (1001) docker     (127)    91317 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/gridtool.m
--rw-r--r--   0 runner    (1001) docker     (127)    84265 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/gridtool_old.m
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/matlabLogging.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/plot_twopar.m
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/queryOpenCL.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-06 22:53:28.000000 clode-0.7.1/matlab/trajectoryfigure.m
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-06 22:53:28.000000 clode-0.7.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-06 22:53:28.000000 clode-0.7.1/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.128681 clode-0.7.1/paper/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-06 22:53:28.000000 clode-0.7.1/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-03-06 22:53:28.000000 clode-0.7.1/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-03-06 22:53:28.000000 clode-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-06 22:53:28.000000 clode-0.7.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-06 22:53:28.000000 clode-0.7.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.132681 clode-0.7.1/samples/
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-03-06 22:53:28.000000 clode-0.7.1/samples/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-06 22:53:28.000000 clode-0.7.1/samples/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-06 22:53:28.000000 clode-0.7.1/samples/lacto_more_vars.cl
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-06 22:53:28.000000 clode-0.7.1/samples/lactotroph.cl
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-06 22:53:28.000000 clode-0.7.1/samples/lactotroph.ode
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-06 22:53:28.000000 clode-0.7.1/samples/lactotroph_noise.cl
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-06 22:53:28.000000 clode-0.7.1/samples/lactotroph_noise.ode
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-06 22:53:28.000000 clode-0.7.1/samples/listOpenCL.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-06 22:53:28.000000 clode-0.7.1/samples/plot_twopar.m
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-03-06 22:53:28.000000 clode-0.7.1/samples/run_twopar.m
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-03-06 22:53:28.000000 clode-0.7.1/samples/test.cl
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-06 22:53:28.000000 clode-0.7.1/samples/testCLODE.m
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-03-06 22:53:28.000000 clode-0.7.1/samples/testCLODEfeatures.m
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-06 22:53:28.000000 clode-0.7.1/samples/testCLODEmex.m
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-06 22:53:28.000000 clode-0.7.1/samples/testCLODEtrajectory.m
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-03-06 22:53:28.000000 clode-0.7.1/samples/testFeatures.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-03-06 22:53:28.000000 clode-0.7.1/samples/testFeatures_morevars.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-03-06 22:53:28.000000 clode-0.7.1/samples/testTrajectory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-03-06 22:53:28.000000 clode-0.7.1/samples/testTransient.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-03-06 22:53:28.000000 clode-0.7.1/samples/test_outputs_cpp.md
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-06 22:53:28.000000 clode-0.7.1/samples/windowsCompileListOpenCL.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 22:55:05.136681 clode-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-03-06 22:53:28.000000 clode-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.136681 clode-0.7.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 22:53:28.000000 clode-0.7.1/test/BUILD
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 22:53:28.000000 clode-0.7.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-06 22:53:28.000000 clode-0.7.1/test/lorenz.cl
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-06 22:53:28.000000 clode-0.7.1/test/ornl_thompson_a1.cl
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-03-06 22:53:28.000000 clode-0.7.1/test/test.cl
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-03-06 22:53:28.000000 clode-0.7.1/test/test_convert_python_to_opencl.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-06 22:53:28.000000 clode-0.7.1/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-03-06 22:53:28.000000 clode-0.7.1/test/test_observers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-03-06 22:53:28.000000 clode-0.7.1/test/test_opencl_builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-03-06 22:53:28.000000 clode-0.7.1/test/test_ornl_thompson_a1.py
--rw-r--r--   0 runner    (1001) docker     (127)    16908 2024-03-06 22:53:28.000000 clode-0.7.1/test/test_pituitary.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-06 22:53:28.000000 clode-0.7.1/test/test_print_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-06 22:53:28.000000 clode-0.7.1/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-03-06 22:53:28.000000 clode-0.7.1/test/test_vdp.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-06 22:53:28.000000 clode-0.7.1/test/test_vdp_long.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-06 22:53:28.000000 clode-0.7.1/test/test_xpp_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-06 22:53:28.000000 clode-0.7.1/test/van_der_pol_oscillator.cl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:55:05.136681 clode-0.7.1/test/xpp/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-06 22:53:28.000000 clode-0.7.1/test/xpp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-06 22:53:28.000000 clode-0.7.1/test/xpp/van_der_pol_oscillator.xpp
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-06 22:53:28.000000 clode-0.7.1/test/xpp/van_der_pol_oscillator_reference.cl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.599550 clode-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 16:02:10.000000 clode-0.8.1/.bazeliskrc
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 16:02:10.000000 clode-0.8.1/.bazelversion
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-27 16:02:10.000000 clode-0.8.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.555550 clode-0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.563550 clode-0.8.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-27 16:02:10.000000 clode-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-27 16:02:10.000000 clode-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.563550 clode-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-27 16:02:10.000000 clode-0.8.1/.github/workflows/bazel_build_linux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-27 16:02:10.000000 clode-0.8.1/.github/workflows/bazel_build_windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-27 16:02:10.000000 clode-0.8.1/.github/workflows/bazel_test_mac.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-27 16:02:10.000000 clode-0.8.1/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-27 16:02:10.000000 clode-0.8.1/.github/workflows/deploy_mkdocs_pages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-27 16:02:10.000000 clode-0.8.1/.github/workflows/draft_pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-27 16:02:10.000000 clode-0.8.1/.github/workflows/scorecards.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-27 16:02:10.000000 clode-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:02:10.000000 clode-0.8.1/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-27 16:02:10.000000 clode-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-27 16:02:10.000000 clode-0.8.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-27 16:03:43.595550 clode-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-27 16:02:10.000000 clode-0.8.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-27 16:02:10.000000 clode-0.8.1/WORKSPACE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.563550 clode-0.8.1/bazel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/clode_http_archive.bzl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.567550 clode-0.8.1/bazel/external/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/external/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/external/fmtlib.BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/external/opencl_windows.BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/external/pybind11.BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/external/python.BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/external/spdlog.BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/external_deps.bzl
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/get_python_libs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.567550 clode-0.8.1/bazel/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/python/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/python/BUILD.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/python/python.bzl
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/python/python_native.bzl
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/python/variety.tpl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.567550 clode-0.8.1/bazel/remote_config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/remote_config/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/remote_config/common.bzl
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/repositories.bzl
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/repository_locations.bzl
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-27 16:02:10.000000 clode-0.8.1/bazel/repository_locations_utils.bzl
+-rw-r--r--   0 runner    (1001) docker     (127)    17104 2024-05-27 16:02:10.000000 clode-0.8.1/bazelisk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.567550 clode-0.8.1/clode/
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-27 16:02:10.000000 clode-0.8.1/clode/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-27 16:02:10.000000 clode-0.8.1/clode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.575550 clode-0.8.1/clode/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/CLODE.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/CLODE.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/CLODEfeatures.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/CLODEfeatures.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17554 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/CLODEpython.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/CLODEtrajectory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/CLODEtrajectory.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.575550 clode-0.8.1/clode/cpp/OpenCL/
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/OpenCL/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)   299120 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/OpenCL/cl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   326155 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/OpenCL/cl2.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   396729 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/OpenCL/opencl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19264 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/OpenCLResource.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/OpenCLResource.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/clODE_random.cl
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/clODE_struct_defs.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/clODE_utilities.cl
+-rw-r--r--   0 runner    (1001) docker     (127)    13391 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/clode_cpp_wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/features.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/initializeObserver.cl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.575550 clode-0.8.1/clode/cpp/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/logging/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/logging/MatlabSink.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/logging/PythonSink.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.579550 clode-0.8.1/clode/cpp/observers/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/observers/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/observers/observer_basic.clh
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/observers/observer_basic_allVar.clh
+-rw-r--r--   0 runner    (1001) docker     (127)    12372 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/observers/observer_local_maximum.clh
+-rw-r--r--   0 runner    (1001) docker     (127)    14221 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/observers/observer_neighborhood_1.clh
+-rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/observers/observer_neighborhood_2.clh
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/observers/observer_template.clh
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/observers/observer_threshold_1.clh
+-rw-r--r--   0 runner    (1001) docker     (127)    18858 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/observers/observer_threshold_2.clh
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/observers.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/odedriver.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/realtype.cl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.579550 clode-0.8.1/clode/cpp/steppers/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/steppers/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/steppers/adaptive_bs23.clh
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/steppers/adaptive_dp45.clh
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/steppers/adaptive_explicit_step.clh
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/steppers/adaptive_he12.clh
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/steppers/adaptive_rkck.clh
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/steppers/fixed_explicit_Euler.clh
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/steppers/fixed_explicit_RK4.clh
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/steppers/fixed_explicit_Trapezoidal.clh
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/steppers/fixed_explicit_step.clh
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/steppers/fixed_explicit_stochastic_Euler.clh
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/steppers.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/trajectory.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-27 16:02:10.000000 clode-0.8.1/clode/cpp/transient.cl
+-rw-r--r--   0 runner    (1001) docker     (127)    21023 2024-05-27 16:02:10.000000 clode-0.8.1/clode/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35257 2024-05-27 16:02:10.000000 clode-0.8.1/clode/function_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-27 16:02:10.000000 clode-0.8.1/clode/opencl_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:02:10.000000 clode-0.8.1/clode/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-27 16:02:10.000000 clode-0.8.1/clode/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26336 2024-05-27 16:02:10.000000 clode-0.8.1/clode/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11095 2024-05-27 16:02:10.000000 clode-0.8.1/clode/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-05-27 16:02:10.000000 clode-0.8.1/clode/xpp_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.595550 clode-0.8.1/clode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-27 16:03:43.000000 clode-0.8.1/clode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-27 16:03:43.000000 clode-0.8.1/clode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:03:43.000000 clode-0.8.1/clode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 16:03:43.000000 clode-0.8.1/clode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.583550 clode-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-27 16:02:10.000000 clode-0.8.1/docs/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-27 16:02:10.000000 clode-0.8.1/docs/Ornstein-Uhlenbeck_process.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-05-27 16:02:10.000000 clode-0.8.1/docs/Ornstein-Uhlenbeck_process.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-27 16:02:10.000000 clode-0.8.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-27 16:02:10.000000 clode-0.8.1/docs/api_reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-27 16:02:10.000000 clode-0.8.1/docs/fast_and_slow_variables.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-27 16:02:10.000000 clode-0.8.1/docs/feature_extraction.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-27 16:02:10.000000 clode-0.8.1/docs/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-27 16:02:10.000000 clode-0.8.1/docs/init_runtime.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-27 16:02:10.000000 clode-0.8.1/docs/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-27 16:02:10.000000 clode-0.8.1/docs/logging_levels.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-27 16:02:10.000000 clode-0.8.1/docs/matlab.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-27 16:02:10.000000 clode-0.8.1/docs/observers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-05-27 16:02:10.000000 clode-0.8.1/docs/pycon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-27 16:02:10.000000 clode-0.8.1/docs/querying_opencl.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-27 16:02:10.000000 clode-0.8.1/docs/specifying_odes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-27 16:02:10.000000 clode-0.8.1/docs/spike_counting.md
+-rw-r--r--   0 runner    (1001) docker     (127)    49954 2024-05-27 16:02:10.000000 clode-0.8.1/docs/spike_counting.png
+-rw-r--r--   0 runner    (1001) docker     (127)    72190 2024-05-27 16:02:10.000000 clode-0.8.1/docs/spike_counting_trajectories.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-27 16:02:10.000000 clode-0.8.1/docs/trajectory_simulation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-27 16:02:10.000000 clode-0.8.1/docs/xpp_files.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.587550 clode-0.8.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-27 16:02:10.000000 clode-0.8.1/examples/Ornstein_Uhlenbeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-27 16:02:10.000000 clode-0.8.1/examples/chay_keizer.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-27 16:02:10.000000 clode-0.8.1/examples/dump_device_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-27 16:02:10.000000 clode-0.8.1/examples/dump_opencl_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-27 16:02:10.000000 clode-0.8.1/examples/fast_and_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-27 16:02:10.000000 clode-0.8.1/examples/find_steady_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-27 16:02:10.000000 clode-0.8.1/examples/observe_sine_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-27 16:02:10.000000 clode-0.8.1/examples/phase_response_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-27 16:02:10.000000 clode-0.8.1/examples/spike_counting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-27 16:02:10.000000 clode-0.8.1/examples/visualize_events_localmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-27 16:02:10.000000 clode-0.8.1/examples/visualize_events_nhood2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-05-27 16:02:10.000000 clode-0.8.1/examples/visualize_events_threshold2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.591550 clode-0.8.1/matlab/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/Chart.m
+-rw-r--r--   0 runner    (1001) docker     (127)    13590 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/GridSimulation.m
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/InitialValueProblem.m
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17036 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/clODE.m
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/clODEfeatures.m
+-rw-r--r--   0 runner    (1001) docker     (127)    16057 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/clODEfeaturesmex.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12413 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/clODEmex.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/clODEmexHelpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/clODEtrajectory.m
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/clODEtrajectorymex.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/clickTrajectory.m
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/compileCLODEmex.m
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/cppclass.m
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/functionSignatures.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/generate_pointset.m
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/gridKeyPress.m
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/gridfigure.m
+-rw-r--r--   0 runner    (1001) docker     (127)    91319 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/gridtool.m
+-rw-r--r--   0 runner    (1001) docker     (127)    84265 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/gridtool_old.m
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/matlabLogging.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/plot_twopar.m
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/queryOpenCL.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-27 16:02:10.000000 clode-0.8.1/matlab/trajectoryfigure.m
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-27 16:02:10.000000 clode-0.8.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 16:02:10.000000 clode-0.8.1/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.591550 clode-0.8.1/paper/
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-27 16:02:10.000000 clode-0.8.1/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-27 16:02:10.000000 clode-0.8.1/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-27 16:02:10.000000 clode-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-27 16:02:10.000000 clode-0.8.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-27 16:02:10.000000 clode-0.8.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.591550 clode-0.8.1/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-27 16:02:10.000000 clode-0.8.1/samples/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-27 16:02:10.000000 clode-0.8.1/samples/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-27 16:02:10.000000 clode-0.8.1/samples/lactotroph.cl
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-27 16:02:10.000000 clode-0.8.1/samples/lactotroph.ode
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-27 16:02:10.000000 clode-0.8.1/samples/lactotroph_noise.cl
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-27 16:02:10.000000 clode-0.8.1/samples/lactotroph_noise.ode
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-27 16:02:10.000000 clode-0.8.1/samples/listOpenCL.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-27 16:02:10.000000 clode-0.8.1/samples/plot_twopar.m
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-27 16:02:10.000000 clode-0.8.1/samples/run_twopar.m
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-27 16:02:10.000000 clode-0.8.1/samples/test.cl
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-27 16:02:10.000000 clode-0.8.1/samples/testCLODE.m
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-27 16:02:10.000000 clode-0.8.1/samples/testCLODEfeatures.m
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-27 16:02:10.000000 clode-0.8.1/samples/testCLODEmex.m
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-27 16:02:10.000000 clode-0.8.1/samples/testCLODEtrajectory.m
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-05-27 16:02:10.000000 clode-0.8.1/samples/testFeatures.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-27 16:02:10.000000 clode-0.8.1/samples/testTrajectory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-27 16:02:10.000000 clode-0.8.1/samples/testTransient.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-05-27 16:02:10.000000 clode-0.8.1/samples/test_outputs_cpp.md
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-27 16:02:10.000000 clode-0.8.1/samples/windowsCompileListOpenCL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:03:43.599550 clode-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-05-27 16:02:10.000000 clode-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.595550 clode-0.8.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:02:10.000000 clode-0.8.1/test/BUILD
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:02:10.000000 clode-0.8.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-27 16:02:10.000000 clode-0.8.1/test/lorenz.cl
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-27 16:02:10.000000 clode-0.8.1/test/ornl_thompson_a1.cl
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-27 16:02:10.000000 clode-0.8.1/test/test_clODE_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-27 16:02:10.000000 clode-0.8.1/test/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-27 16:02:10.000000 clode-0.8.1/test/test_function_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-27 16:02:10.000000 clode-0.8.1/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-05-27 16:02:10.000000 clode-0.8.1/test/test_observers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-27 16:02:10.000000 clode-0.8.1/test/test_opencl_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-27 16:02:10.000000 clode-0.8.1/test/test_ornl_thompson_a1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-27 16:02:10.000000 clode-0.8.1/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-27 16:02:10.000000 clode-0.8.1/test/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:02:10.000000 clode-0.8.1/test/test_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-27 16:02:10.000000 clode-0.8.1/test/test_vdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-27 16:02:10.000000 clode-0.8.1/test/test_vdp_long.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-27 16:02:10.000000 clode-0.8.1/test/test_xpp_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-27 16:02:10.000000 clode-0.8.1/test/tests.md
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-27 16:02:10.000000 clode-0.8.1/test/van_der_pol_oscillator.cl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:03:43.595550 clode-0.8.1/test/xpp/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-27 16:02:10.000000 clode-0.8.1/test/xpp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-27 16:02:10.000000 clode-0.8.1/test/xpp/van_der_pol_oscillator.xpp
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-27 16:02:10.000000 clode-0.8.1/test/xpp/van_der_pol_oscillator_reference.cl
```

### Comparing `clode-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md` & `clode-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md` & `clode-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/.github/workflows/bazel_build_linux.yml` & `clode-0.8.1/.github/workflows/bazel_build_linux.yml`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/.github/workflows/bazel_build_windows.yml` & `clode-0.8.1/.github/workflows/bazel_build_windows.yml`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/.github/workflows/bazel_test_mac.yml` & `clode-0.8.1/.github/workflows/bazel_test_mac.yml`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/.github/workflows/dependency-review.yml` & `clode-0.8.1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/.github/workflows/deploy_mkdocs_pages.yml` & `clode-0.8.1/.github/workflows/deploy_mkdocs_pages.yml`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/.github/workflows/draft_pdf.yml` & `clode-0.8.1/.github/workflows/draft_pdf.yml`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 jobs:
   paper:
     runs-on: ubuntu-latest
     name: Paper Draft
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
       - name: Build draft PDF
         uses: openjournals/openjournals-draft-action@master
         with:
           journal: joss
           # This should be the path to the paper within your repo.
           paper-path: paper/paper.md
       - name: Upload
-        uses: actions/upload-artifact@v1
+        uses: actions/upload-artifact@v4
         with:
           name: paper
           # This is the output path where Pandoc will write the compiled
           # PDF. Note, this should be the same directory as the input
           # paper.md
           path: paper/paper.pdf
```

### Comparing `clode-0.7.1/.github/workflows/scorecards.yml` & `clode-0.8.1/.github/workflows/scorecards.yml`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/.gitignore` & `clode-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/Makefile` & `clode-0.8.1/Makefile`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/PKG-INFO` & `clode-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clode
-Version: 0.7.1
+Version: 0.8.1
 Summary: A Python package for solving ordinary differential equations on the GPU using OpenCL
 Author-email: Patrick Fletcher <patrick.allen.fletcher@gmail.com>
 Maintainer-email: Patrick Fletcher <patrick.allen.fletcher@gmail.com>, Wolf Byttner <wolf@byttner.org>
 Project-URL: Documentation, https://patrickfletcher.github.io/clODE/
 Project-URL: Repository, https://github.com/patrickfletcher/clODE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `clode-0.7.1/WORKSPACE` & `clode-0.8.1/WORKSPACE`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/bazel/clode_http_archive.bzl` & `clode-0.8.1/bazel/clode_http_archive.bzl`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/bazel/external/python.BUILD` & `clode-0.8.1/bazel/external/python.BUILD`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/bazel/external_deps.bzl` & `clode-0.8.1/bazel/external_deps.bzl`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/bazel/get_python_libs.py` & `clode-0.8.1/bazel/get_python_libs.py`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/bazel/python/BUILD.tpl` & `clode-0.8.1/bazel/python/BUILD.tpl`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/bazel/python/python.bzl` & `clode-0.8.1/bazel/python/python.bzl`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/bazel/python/variety.tpl` & `clode-0.8.1/bazel/python/variety.tpl`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/bazel/remote_config/common.bzl` & `clode-0.8.1/bazel/remote_config/common.bzl`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/bazel/repositories.bzl` & `clode-0.8.1/bazel/repositories.bzl`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/bazel/repository_locations.bzl` & `clode-0.8.1/bazel/repository_locations.bzl`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/bazel/repository_locations_utils.bzl` & `clode-0.8.1/bazel/repository_locations_utils.bzl`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/bazelisk.py` & `clode-0.8.1/bazelisk.py`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/clode/BUILD` & `clode-0.8.1/clode/BUILD`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/clode/__init__.py` & `clode-0.8.1/clode/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# This is the package public interface (expose objects for "from clode import X")
+# - keep only main simulation items here?
+# - keep CL-related things in runtime?
+from clode.cpp.clode_cpp_wrapper import ObserverParams, ProblemInfo, SolverParams
 from clode.features import FeatureSimulator, Observer, ObserverOutput
 from clode.function_converter import (
     OpenCLConverter,
     OpenCLRhsEquation,
     convert_str_to_opencl,
 )
 
@@ -31,14 +35,15 @@
     exp10,
     expm1,
     fabs,
     fdim,
     floor,
     fmod,
     gamma,
+    heaviside,
     hypot,
     ilogb,
     ldexp,
     lgamma,
     log,
     log1p,
     log2,
@@ -59,40 +64,58 @@
     tanh,
     tanpi,
     trunc,
 )
 from clode.runtime import (
     CLDeviceType,
     CLVendor,
+    DeviceInfo,
     LogLevel,
-    ProblemInfo,
-    SolverParams,
+    PlatformInfo,
     get_log_level,
     initialize_runtime,
     print_opencl,
     query_opencl,
     set_log_level,
     set_log_pattern,
 )
 from clode.solver import Simulator, Stepper
-from clode.trajectory import TrajectorySimulator
+from clode.trajectory import TrajectoryOutput, TrajectorySimulator
 from clode.xpp_parser import convert_xpp_file, format_opencl_rhs, read_ode_parameters
 
-__version__ = "0.7.1"
+__version__ = "0.8.1"
 
 __all__ = [
-    "TrajectorySimulator",
-    "Simulator",
+    "CLDeviceType",
+    "CLVendor",
+    "DeviceInfo",
+    "PlatformInfo",
+    "initialize_runtime",
+    "print_opencl",
+    "query_opencl",
+    "LogLevel",
+    "get_log_level",
+    "set_log_level",
+    "set_log_pattern",
+    "ProblemInfo",
+    "SolverParams",
     "Stepper",
+    "Simulator",
     "FeatureSimulator",
     "Observer",
+    "ObserverParams",
     "ObserverOutput",
+    "TrajectorySimulator",
+    "TrajectoryOutput",
     "OpenCLConverter",
     "OpenCLRhsEquation",
     "convert_str_to_opencl",
+    "convert_xpp_file",
+    "format_opencl_rhs",
+    "read_ode_parameters",
     "acos",
     "acosh",
     "acospi",
     "asin",
     "asinh",
     "asinpi",
     "atan",
@@ -114,14 +137,15 @@
     "expm1",
     "fabs",
     "fdim",
     "floor",
     "fmod",
     "gamma",
     "hypot",
+    "heaviside",
     "ilogb",
     "ldexp",
     "lgamma",
     "log",
     "log1p",
     "log2",
     "log10",
@@ -137,22 +161,8 @@
     "sinh",
     "sinpi",
     "sqrt",
     "tan",
     "tanh",
     "tanpi",
     "trunc",
-    "CLDeviceType",
-    "CLVendor",
-    "LogLevel",
-    "ProblemInfo",
-    "SolverParams",
-    "get_log_level",
-    "initialize_runtime",
-    "print_opencl",
-    "query_opencl",
-    "set_log_level",
-    "set_log_pattern",
-    "convert_xpp_file",
-    "format_opencl_rhs",
-    "read_ode_parameters",
 ]
```

### Comparing `clode-0.7.1/clode/cpp/BUILD` & `clode-0.8.1/clode/cpp/BUILD`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/clode/cpp/CLODE.cpp` & `clode-0.8.1/clode/cpp/CLODE.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -8,324 +8,287 @@
 #include <random>
 #include <stdexcept>
 
 #include "spdlog/spdlog.h"
 
 CLODE::CLODE(ProblemInfo prob, std::string stepper, bool clSinglePrecision, OpenCLResource opencl, const std::string clodeRoot)
 {
-	getStepperDefineMap(stepperDefineMap, availableSteppers); //from steppers.cl
-	setNewProblem(prob);
+	getStepperDefineMap(stepperDefineMap, availableSteppers); // from steppers.cl
+	setProblemInfo(prob);
 	setStepper(stepper);
 	setPrecision(clSinglePrecision);
-    setClodeRoot(clodeRoot);
+	setClodeRoot(clodeRoot);
 	setOpenCL(opencl);
 
 	clprogramstring = read_file(clodeRoot + "transient.cl");
 	spdlog::debug("constructor clODE");
 }
 
 CLODE::CLODE(ProblemInfo prob, std::string stepper, bool clSinglePrecision, unsigned int platformID, unsigned int deviceID, const std::string clodeRoot)
 {
-	getStepperDefineMap(stepperDefineMap, availableSteppers); //from steppers.cl
-	setNewProblem(prob);
+	getStepperDefineMap(stepperDefineMap, availableSteppers); // from steppers.cl
+	setProblemInfo(prob);
 	setStepper(stepper);
 	setPrecision(clSinglePrecision);
-    setClodeRoot(clodeRoot);
+	setClodeRoot(clodeRoot);
 	setOpenCL(platformID, deviceID);
 
 	clprogramstring = read_file(clodeRoot + "transient.cl");
 	spdlog::debug("constructor clODE");
 }
 
 CLODE::~CLODE()
 {
 }
 
-void CLODE::setNewProblem(ProblemInfo newProb)
-{ //TODO: not equality check for ProblemInfo struct, error checking: at least one variable!
-	prob=newProb;
+void CLODE::setProblemInfo(ProblemInfo newProb)
+{ // TODO: not equality check for ProblemInfo struct, error checking: at least one variable!
+	prob = newProb;
 	clRHSfilename = newProb.clRHSfilename;
 	ODEsystemsource = read_file(clRHSfilename);
 	nVar = newProb.nVar;
-	nPar = newProb.nPar; 
+	nPar = newProb.nPar;
 	nAux = newProb.nAux;
 	nWiener = newProb.nWiener;
 
 	// Some OpenCL implementations don't support zero-length arrays in OpenCL programs
 	// nPar = nPar>0?nPar:1;
 	// nAux = nAux>0?nAux:1;
 	// nWiener = nWiener>0?nWiener:1;
 
-	clInitialized = false;
 	spdlog::debug("set new problem");
 }
 
 void CLODE::setStepper(std::string newStepper)
 {
 	// if (newStepper!=stepper)
 	// {
-	auto loc = stepperDefineMap.find(newStepper); //from steppers.cl
-	if ( loc != stepperDefineMap.end() )
+	auto loc = stepperDefineMap.find(newStepper); // from steppers.cl
+	if (loc != stepperDefineMap.end())
 	{
 		stepper = newStepper;
-		clInitialized = false;
 	}
 	else
 	{
-		spdlog::warn("Unknown stepper: {}. Stepper method unchanged",newStepper.c_str());
+		spdlog::warn("Unknown stepper: {}. Stepper method unchanged", newStepper.c_str());
 	}
-	spdlog::debug("set stepper");	
+	spdlog::debug("set stepper");
 	// }
 }
 
 void CLODE::setPrecision(bool newPrecision)
 {
 	// if (newPrecision != clSinglePrecision)
 	// {
 	clSinglePrecision = newPrecision;
 	realSize = newPrecision ? sizeof(cl_float) : sizeof(cl_double);
-	clInitialized = false;
 	spdlog::debug("set precision");
 	// }
 }
 
 void CLODE::setOpenCL(OpenCLResource newOpencl)
-{//TODO: not equality check for OpenCLResource class
+{ // TODO: not equality check for OpenCLResource class
 	//~ if (newOpencl!=opencl) {
 	opencl = newOpencl;
-	clInitialized = false;
 	//~ }
 	spdlog::debug("set OpenCL");
 }
 
 void CLODE::setOpenCL(unsigned int platformID, unsigned int deviceID)
-{//TODO: not equality check for OpenCLResource class
+{ // TODO: not equality check for OpenCLResource class
 	//~ if (newOpencl!=opencl) {
 	opencl = OpenCLResource(platformID, deviceID);
-	clInitialized = false;
 	//~ }
 	spdlog::debug("set OpenCL");
 }
 
 void CLODE::setClodeRoot(const std::string newClodeRoot)
 {
-    clodeRoot = newClodeRoot;
+	clodeRoot = newClodeRoot;
 }
 
-
 void CLODE::setCLbuildOpts(std::string extraBuildOpts)
 {
-	
+
 	if (!clSinglePrecision && !opencl.getDoubleSupport())
-	{ //TODO: make this an error?
+	{ // TODO: make this an error?
 		clSinglePrecision = true;
 		spdlog::warn("device selected does not support double precision. Using single precision");
 	}
 
 	buildOptions = "";
 
-	//specify precision
+	// specify precision
 	if (clSinglePrecision)
 		buildOptions += " -DCLODE_SINGLE_PRECISION";
 	else
 		buildOptions += " -DCLODE_DOUBLE_PRECISION";
 
-	//specify stepper
+	// specify stepper
 	buildOptions += " -D" + stepperDefineMap.at(stepper);
 
-	//specify problem dimensions
-	buildOptions += " -DN_PAR=" + std::to_string((long long)nPar); //for older c++ compilers the to_string(int) overload of the STL isn't present
+	// specify problem dimensions
+	buildOptions += " -DN_PAR=" + std::to_string((long long)nPar); // for older c++ compilers the to_string(int) overload of the STL isn't present
 	buildOptions += " -DN_VAR=" + std::to_string((long long)nVar);
 	buildOptions += " -DN_AUX=" + std::to_string((long long)nAux);
 	buildOptions += " -DN_WIENER=" + std::to_string((long long)nWiener);
 
-	//include folder for CLODE
+	// include folder for CLODE
 	buildOptions += " -I" + clodeRoot;
 
-    spdlog::debug("OpenCL build options {}", buildOptions);
-
 	buildOptions += extraBuildOpts;
-}
 
+	spdlog::debug("OpenCL build options {}", buildOptions);
+}
 
-//build creates build option defined constants based on selected options, adds the ODEsystem source to clprogramstring then builds for selected OpenCL resource
+// build creates build option defined constants based on selected options, adds the ODEsystem source to clprogramstring then builds for selected OpenCL resource
 void CLODE::buildProgram(std::string extraBuildOpts)
 {
 	setCLbuildOpts(extraBuildOpts);
 
 	opencl.buildProgramFromString(clprogramstring + ODEsystemsource, buildOptions);
 
-    spdlog::debug(clprogramstring + ODEsystemsource);
-    spdlog::debug(buildOptions);
-	spdlog::debug("buildProgram");
+	spdlog::trace(clprogramstring + ODEsystemsource);
+	spdlog::debug("CLODE buildProgram finished");
 }
 
 // build program and create kernel objects. requires host variables to be set
 void CLODE::buildCL()
 {
+	spdlog::info("Running CLODE buildCL");
 	buildProgram();
 
-	//set up the kernel
+	// set up the kernel
 	try
-	{ 
+	{
 		cl_transient = cl::Kernel(opencl.getProgram(), "transient", &opencl.error);
 	}
 	catch (cl::Error &er)
 	{
-		spdlog::error("CLODE::initializeTransientKernel():{}({})", er.what(), CLErrorString(er.err()).c_str());
+		spdlog::error("CLODE::buildCL(): create kernels{}({})", er.what(), CLErrorString(er.err()).c_str());
 		throw er;
 	}
-	clInitialized = false;
-	spdlog::debug("buildCL");
-}
-
-//initialize everything: build the program, create the kernels, and set all needed problem data.
-void CLODE::initialize(std::vector<cl_double> newTspan, std::vector<cl_double> newX0, std::vector<cl_double> newPars, SolverParams<cl_double> newSp)
-{
-	clInitialized = false;
-
-	setTspan(newTspan);
-	setProblemData(newX0, newPars); //will call setNpts
-	setSolverParams(newSp);
-
-	clInitialized = true;
-	spdlog::debug("initialize clODE");
+	spdlog::debug("Created kernel");
 }
 
-//initialize new set of trajectories (nPts may change)
-void CLODE::setProblemData(std::vector<cl_double> newX0, std::vector<cl_double> newPars)
-{	//check if newX0 and newPars are valid, and update nPts if needed:
-	if (newX0.size() % nVar != 0)
-	{
-		spdlog::info("Invalid initial condition vector: not a multiple of nVar={}", nVar);
-		spdlog::info("...Initial conditions were not updated!");
-		return;
-	}
-
-	if (newPars.size() % nPar != 0)
-	{
-		spdlog::info("Invalid parameter vector: not a multiple of nPar={}", nPar);
-		spdlog::info("...Parameters were not updated!");
-		return;
-	}
-
-	// now check if newX0 and newPars represent same number of sets
-	cl_int nPtsX0 = newX0.size() / nVar;
-	cl_int nPtsPars = newPars.size() / nPar;
-	// spdlog::info("Computed nPts: {} {}", nPtsX0, nPtsPars);
-	if (nPtsX0 != nPtsPars)
-	{
-		spdlog::info("Initial contition and parameter vector dimensions don't match");
-		spdlog::info("...Expected {} sets of each, recieved {} for x0 and {} for pars", nPts, nPtsX0, nPtsPars);
-		spdlog::info("...Problem data was not updated!");
-		return;
-	}
-
-	//set nPts
-	setNpts(nPtsX0);
-
-	//set things that depend on nPts
-	setX0(newX0);
-	setPars(newPars);
-	spdlog::debug("set problem data");
-}
-
-//resize all the nPts dependent variables, only if nPts changed
+// resize all the nPts dependent variables, only if nPts changed
 void CLODE::setNpts(cl_int newNpts)
-{	//unlikely that any of these should ever exceed memory limits...
+{
 	size_t largestAlloc = std::max(nVar, std::max(nPar, nAux)) * nPts * realSize;
 	// spdlog::info("Computed largestAlloc: {}", largestAlloc);
 
 	if (largestAlloc > opencl.getMaxMemAllocSize())
 	{
 		throw std::invalid_argument("nPts*nVar, nPts*nPar, or nPts*nAux is too large");
 	}
 
-	if (!clInitialized || newNpts != nPts)
+	if (newNpts != nPts)
 	{
 		nPts = newNpts;
 
 		x0elements = nVar * nPts;
 		parselements = nPar * nPts;
+
 		RNGelements = nRNGstate * nPts;
+		// cl::Buffer doesn't like zero-sized arrays:
+		// RNGelements = nWiener > 0 ? nWiener * nRNGstate * nPts : 1;
 
-		//resize host variables
+		// resize host variables
 		x0.resize(x0elements);
 		pars.resize(parselements);
-		xf.resize(x0elements);
+
 		RNGstate.resize(RNGelements);
+
 		dt.resize(nPts);
+		std::fill(dt.begin(), dt.end(), sp.dt);
 
-		//new device variables
+		xf.resize(x0elements);
+		// new device variables
 		try
 		{
+			// must be populated with valid data prior to simulation
 			d_x0 = cl::Buffer(opencl.getContext(), CL_MEM_READ_WRITE, realSize * x0elements, NULL, &opencl.error);
 			d_pars = cl::Buffer(opencl.getContext(), CL_MEM_READ_ONLY, realSize * parselements, NULL, &opencl.error);
-			d_xf = cl::Buffer(opencl.getContext(), CL_MEM_READ_WRITE, realSize * x0elements, NULL, &opencl.error);
+
 			d_RNGstate = cl::Buffer(opencl.getContext(), CL_MEM_READ_WRITE, sizeof(cl_ulong) * RNGelements, NULL, &opencl.error);
+
+			// resize and fill dt buffer
 			d_dt = cl::Buffer(opencl.getContext(), CL_MEM_READ_WRITE, realSize * nPts, NULL, &opencl.error);
+			if (clSinglePrecision) {
+				std::vector<cl_float> dtF(dt.begin(), dt.end());
+				opencl.error = copy(opencl.getQueue(), dtF.begin(), dtF.end(), d_dt);
+			}
+			else
+				opencl.error = copy(opencl.getQueue(), dt.begin(), dt.end(), d_dt);
+
+			// output of simulation
+			d_xf = cl::Buffer(opencl.getContext(), CL_MEM_READ_WRITE, realSize * x0elements, NULL, &opencl.error);
 		}
 		catch (cl::Error &er)
 		{
 			spdlog::error("CLODE::setNpts:{}({})", er.what(), CLErrorString(er.err()).c_str());
 			throw er;
 		}
 
-		//seed RNG must occur after device variable d_RNGstate is resized
+		// seed RNG must occur after device variable d_RNGstate is resized
 		seedRNG();
-		spdlog::debug("set nPts");
+		spdlog::debug("set nPts={}", nPts);
 	}
 }
 
-void CLODE::setTspan(std::vector<cl_double> newTspan)
-{
-	try
+// initialize new set of trajectories (nPts may change)
+void CLODE::setProblemData(std::vector<cl_double> newX0, std::vector<cl_double> newPars)
+{ // check if newX0 and newPars are valid, and update nPts if needed:
+	if (newX0.size() % nVar != 0)
 	{
-		if (!clInitialized)
-			d_tspan = cl::Buffer(opencl.getContext(), CL_MEM_READ_ONLY, realSize * 2, NULL, &opencl.error);
-
-		tspan = newTspan;
+		spdlog::info("Invalid initial condition vector: not a multiple of nVar={}", nVar);
+		spdlog::info("...Initial conditions were not updated!");
+		return;
+	}
 
-		if (clSinglePrecision)
-		{ //downcast to float if desired
-			std::vector<cl_float> tspanF(tspan.begin(), tspan.end());
-			opencl.error = copy(opencl.getQueue(), tspanF.begin(), tspanF.end(), d_tspan);
-		}
-		else
-		{
-			opencl.error = copy(opencl.getQueue(), tspan.begin(), tspan.end(), d_tspan);
-		}
+	if (newPars.size() % nPar != 0)
+	{
+		spdlog::info("Invalid parameter vector: not a multiple of nPar={}", nPar);
+		spdlog::info("...Parameters were not updated!");
+		return;
 	}
-	catch (cl::Error &er)
+
+	// now check if newX0 and newPars represent same number of sets
+	cl_int nPtsX0 = newX0.size() / nVar;
+	cl_int nPtsPars = newPars.size() / nPar;
+	// spdlog::info("Computed nPts: {} {}", nPtsX0, nPtsPars);
+	if (nPtsX0 != nPtsPars)
 	{
-		spdlog::error("CLODE::setTspan:{}({})", er.what(), CLErrorString(er.err()).c_str());
-		throw er;
+		spdlog::info("Initial contition and parameter vector dimensions don't match");
+		spdlog::info("...Expected {} sets of each, recieved {} for x0 and {} for pars", nPts, nPtsX0, nPtsPars);
+		spdlog::info("...Problem data was not updated!");
+		return;
 	}
-	spdlog::debug("set tspan");
-}
 
-void CLODE::shiftTspan()
-{
-	std::vector<cl_double> newTspan({tspan[1], tspan[1] + (tspan[1] - tspan[0])});
-	setTspan(newTspan);
-	spdlog::debug("shift tspan");
+	// set nPts
+	setNpts(nPtsX0);
+
+	// set things that depend on nPts
+	setX0(newX0);
+	setPars(newPars);
+	spdlog::debug("set problem data");
 }
 
-//set new x0. Cannot update nPts
+// set new x0. Cannot update nPts
 void CLODE::setX0(std::vector<cl_double> newX0)
 {
 	if (newX0.size() == (size_t)nPts * nVar)
 	{
 		x0 = newX0;
 
-		//sync to device
+		// sync to device
 		try
 		{
 			if (clSinglePrecision)
-			{ //downcast to float if desired
+			{ // downcast to float if desired
 				std::vector<cl_float> x0F(x0.begin(), x0.end());
 				opencl.error = copy(opencl.getQueue(), x0F.begin(), x0F.end(), d_x0);
 			}
 			else
 			{
 				opencl.error = copy(opencl.getQueue(), x0.begin(), x0.end(), d_x0);
 			}
@@ -341,41 +304,26 @@
 	{
 		// spdlog::info("Invalid initial condition vector: Expected {}*{} elements, recieved {}}", nPts, nVar, newX0.size());
 		spdlog::info("...Initial conditions were not updated!");
 		//~ throw std::invalid_argument("Initial Condition vector has incorrect size.");
 	}
 }
 
-void CLODE::shiftX0()
-{
-	//device to device transfer of Xf to X0
-	try
-	{
-		opencl.error = opencl.getQueue().enqueueCopyBuffer(d_xf, d_x0, 0, 0, realSize * x0elements);
-	}
-	catch (cl::Error &er)
-	{
-		spdlog::error("CLODE::shiftX0:{}({})", er.what(), CLErrorString(er.err()).c_str());
-		throw er;
-	}
-	spdlog::debug("shift X0");
-}
-
-//set new Pars. Cannot update nPts
+// set new Pars. Cannot update nPts
 void CLODE::setPars(std::vector<cl_double> newPars)
 {
 	if (newPars.size() == (size_t)nPts * nPar)
 	{
 		pars = newPars;
 
-		//sync to device
+		// sync to device
 		try
 		{
 			if (clSinglePrecision)
-			{ //downcast to float if desired
+			{ // downcast to float if desired
 				std::vector<cl_float> parsF(pars.begin(), pars.end());
 				opencl.error = copy(opencl.getQueue(), parsF.begin(), parsF.end(), d_pars);
 			}
 			else
 			{
 				opencl.error = copy(opencl.getQueue(), pars.begin(), pars.end(), d_pars);
 			}
@@ -391,72 +339,90 @@
 	{
 		spdlog::info("Invalid parameter vector: Expected {}*{} elements, recieved {}", nPts, nPar, newPars.size());
 		spdlog::info("...Parameters were not updated!");
 		//~ throw std::invalid_argument("Parameter vector has incorrect size.");
 	}
 }
 
-void CLODE::setSolverParams(SolverParams<cl_double> newSp)
-{//TODO: equality operator for SolverParams struct
+void CLODE::setTspan(std::vector<cl_double> newTspan)
+{
 	try
 	{
-		if (!clInitialized)
+		tspan = newTspan;
+		d_tspan = cl::Buffer(opencl.getContext(), CL_MEM_READ_ONLY, realSize * 2, NULL, &opencl.error);
+
+		if (clSinglePrecision)
+		{ // downcast to float if desired
+			std::vector<cl_float> tspanF(tspan.begin(), tspan.end());
+			opencl.error = copy(opencl.getQueue(), tspanF.begin(), tspanF.end(), d_tspan);
+		}
+		else
 		{
-			if (clSinglePrecision)
-				d_sp = cl::Buffer(opencl.getContext(), CL_MEM_READ_ONLY, sizeof(SolverParams<cl_float>), NULL, &opencl.error);
-			else
-				d_sp = cl::Buffer(opencl.getContext(), CL_MEM_READ_ONLY, sizeof(SolverParams<cl_double>), NULL, &opencl.error);	
+			opencl.error = copy(opencl.getQueue(), tspan.begin(), tspan.end(), d_tspan);
 		}
-	
+	}
+	catch (cl::Error &er)
+	{
+		spdlog::error("CLODE::setTspan:{}({})", er.what(), CLErrorString(er.err()).c_str());
+		throw er;
+	}
+	spdlog::debug("set tspan");
+}
+
+void CLODE::setSolverParams(SolverParams<cl_double> newSp)
+{ // TODO: equality operator for SolverParams struct
+	try
+	{
 		sp = newSp;
-		std::fill(dt.begin(), dt.end(), sp.dt);
-		
+		// std::fill(dt.begin(), dt.end(), sp.dt);
+
 		if (clSinglePrecision)
-		{ //downcast to float if desired
+		{ // downcast to float if desired
 			SolverParams<cl_float> spF = solverParamsToFloat(sp);
+			d_sp = cl::Buffer(opencl.getContext(), CL_MEM_READ_ONLY, sizeof(SolverParams<cl_float>), NULL, &opencl.error);
 			opencl.error = opencl.getQueue().enqueueWriteBuffer(d_sp, CL_TRUE, 0, sizeof(spF), &spF);
-			std::vector<cl_float> dtF(dt.begin(), dt.end());
-			opencl.error = copy(opencl.getQueue(), dtF.begin(), dtF.end(), d_dt);
+			// std::vector<cl_float> dtF(dt.begin(), dt.end());
+			// opencl.error = copy(opencl.getQueue(), dtF.begin(), dtF.end(), d_dt);
 			// opencl.error = opencl.getQueue().enqueueFillBuffer(d_dt, spF.dt, 0, sizeof(spF.dt));
 		}
 		else
 		{
+			d_sp = cl::Buffer(opencl.getContext(), CL_MEM_READ_ONLY, sizeof(SolverParams<cl_double>), NULL, &opencl.error);
 			opencl.error = opencl.getQueue().enqueueWriteBuffer(d_sp, CL_TRUE, 0, sizeof(sp), &sp);
-			opencl.error = copy(opencl.getQueue(), dt.begin(), dt.end(), d_dt);
+			// opencl.error = copy(opencl.getQueue(), dt.begin(), dt.end(), d_dt);
 			// opencl.error = opencl.getQueue().enqueueFillBuffer(d_dt, sp.dt, 0, sizeof(sp.dt));
 		}
-		
 	}
 	catch (cl::Error &er)
 	{
 		spdlog::error("CLODE::setSolverParams:{}({})", er.what(), CLErrorString(er.err()).c_str());
 		throw er;
 	}
 	spdlog::debug("set SolverParams");
 }
 
-//TODO: define an assignment/type cast operator in the struct?
+// TODO: define an assignment/type cast operator in the struct?
 SolverParams<cl_float> CLODE::solverParamsToFloat(SolverParams<cl_double> sp)
 {
 	SolverParams<cl_float> spF;
 	spF.dt = sp.dt;
 	spF.dtmax = sp.dtmax;
 	spF.abstol = sp.abstol;
 	spF.reltol = sp.reltol;
 	spF.max_steps = sp.max_steps;
 	spF.max_store = sp.max_store;
 	spF.nout = sp.nout;
 
 	return spF;
 }
 
-//populate the RNGstate vector on the device. nPts must be set
+// populate the RNGstate vector on the device. nPts must be set
 void CLODE::seedRNG()
 {
-	//TODO: what is correct method??? here, using MT to get (nRNGstate x nPts) 64bit words
+	// TODO: what is correct method??? here, using MT to get (nRNGstate x nPts) 64bit words
 
 	std::random_device rd;
 	std::mt19937_64 gen(rd());
 	std::uniform_int_distribution<cl_ulong> dis;
 
 	for (int i = 0; i < nRNGstate * nPts; ++i)
 	{
@@ -472,15 +438,15 @@
 	{
 		spdlog::error("CLODE::seedRNG:{}({})", er.what(), CLErrorString(er.err()).c_str());
 		throw er;
 	}
 	spdlog::debug("set random RNG seed");
 }
 
-//populate the RNGstate vector on the device. nPts must be set
+// populate the RNGstate vector on the device. nPts must be set
 void CLODE::seedRNG(cl_int mySeed)
 {
 
 	for (int i = 0; i < nRNGstate * nPts; ++i)
 	{
 		RNGstate[i] = mySeed + i;
 	}
@@ -493,94 +459,100 @@
 	{
 		spdlog::error("CLODE::seedRNG(int mySeed):{}({})", er.what(), CLErrorString(er.err()).c_str());
 		throw er;
 	}
 	spdlog::debug("set fixed RNG seed");
 }
 
-//Simulation routine
+// Simulation routine
 void CLODE::transient()
 {
+	try
+	{
+		// kernel args
+		int ix = 0;
+		cl_transient.setArg(ix++, d_tspan);
+		cl_transient.setArg(ix++, d_x0);
+		cl_transient.setArg(ix++, d_pars);
+		cl_transient.setArg(ix++, d_sp);
+		cl_transient.setArg(ix++, d_xf);
+		cl_transient.setArg(ix++, d_RNGstate);
+		cl_transient.setArg(ix++, d_dt);
+
+		// execute the kernel
+		opencl.error = opencl.getQueue().enqueueNDRangeKernel(cl_transient, cl::NullRange, cl::NDRange(nPts));
+		opencl.getQueue().finish();
+	}
+	catch (cl::Error &er)
+	{
+		spdlog::error("CLODE::transient:{}({})", er.what(), CLErrorString(er.err()).c_str());
+		throw er;
+	}
+	spdlog::info("run transient");
+}
+
+void CLODE::shiftTspan()
+{
+	std::vector<cl_double> newTspan({tspan[1], tspan[1] + (tspan[1] - tspan[0])});
+	setTspan(newTspan);
+	spdlog::debug("shift tspan");
+}
 
-	if (clInitialized)
+void CLODE::shiftX0()
+{
+	// device to device transfer of Xf to X0
+	try
 	{
-		try
-		{
-			//kernel args
-			int ix=0;
-			cl_transient.setArg(ix++, d_tspan);
-			cl_transient.setArg(ix++, d_x0);
-			cl_transient.setArg(ix++, d_pars);
-			cl_transient.setArg(ix++, d_sp);
-			cl_transient.setArg(ix++, d_xf);
-			cl_transient.setArg(ix++, d_RNGstate);
-			cl_transient.setArg(ix++, d_dt);
-
-			//execute the kernel
-			opencl.error = opencl.getQueue().enqueueNDRangeKernel(cl_transient, cl::NullRange, cl::NDRange(nPts));
-			opencl.getQueue().finish();
-		}
-		catch (cl::Error &er)
-		{
-			spdlog::error("CLODE::transient:{}({})", er.what(), CLErrorString(er.err()).c_str());
-			throw er;
-		}
-		spdlog::info("run transient");
+		opencl.error = opencl.getQueue().enqueueCopyBuffer(d_xf, d_x0, 0, 0, realSize * x0elements);
 	}
-	else
+	catch (cl::Error &er)
 	{
-		spdlog::info("CLODE has not been initialized");
+		spdlog::error("CLODE::shiftX0:{}({})", er.what(), CLErrorString(er.err()).c_str());
+		throw er;
 	}
+	spdlog::debug("shift X0");
 }
 
-std::vector<cl_double> CLODE::getX0()
+const std::vector<cl_double> CLODE::getX0()
 {
 
 	if (clSinglePrecision)
-	{ //cast back to double
+	{ // cast back to double
 		std::vector<cl_float> x0F(x0elements);
 		opencl.error = copy(opencl.getQueue(), d_x0, x0F.begin(), x0F.end());
 		x0.assign(x0F.begin(), x0F.end());
 	}
 	else
 	{
 		opencl.error = copy(opencl.getQueue(), d_x0, x0.begin(), x0.end());
 	}
 
 	return x0;
 }
 
-std::vector<cl_double> CLODE::getXf()
+const std::vector<cl_double> CLODE::getXf()
 {
 
 	if (clSinglePrecision)
-	{ //cast back to double
+	{ // cast back to double
 		std::vector<cl_float> xfF(x0elements);
 		opencl.error = copy(opencl.getQueue(), d_xf, xfF.begin(), xfF.end());
 		xf.assign(xfF.begin(), xfF.end());
 	}
 	else
 	{
 		opencl.error = copy(opencl.getQueue(), d_xf, xf.begin(), xf.end());
 	}
 
 	return xf;
 }
 
-
-std::string CLODE::getProgramString() 
-{
-	setCLbuildOpts();
-	return buildOptions+clprogramstring+ODEsystemsource; 
-}
-
-
 void CLODE::printStatus()
 {
-	opencl.print();
+	// opencl.print();
 	spdlog::info("------------------");
 	spdlog::info("   {}", clRHSfilename.c_str());
 	spdlog::info("   nVar={}", nVar);
 	spdlog::info("   nPar={}", nPar);
 	spdlog::info("   nAux={}", nAux);
 	spdlog::info("   nWiener={}", nWiener);
 	spdlog::info("Using {} precision.", (clSinglePrecision ? "single" : "double"));
```

### Comparing `clode-0.7.1/clode/cpp/CLODE.hpp` & `clode-0.8.1/clode/cpp/CLODE.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -81,127 +81,109 @@
 
     void setAuxNames(std::vector<std::string> auxNamesIn)
     {
         this->auxNames = auxNamesIn;
         this->nAux = auxNamesIn.size();
     }
 
-    std::vector<std::string> getVarNames()
-    {
-        return this->varNames;
-    }
-
-    std::vector<std::string> getParNames()
-    {
-        return this->parNames;
-    }
-
-    std::vector<std::string> getAuxNames()
-    {
-        return this->auxNames;
-    }
+    std::vector<std::string> getVarNames() { return this->varNames; }
+    std::vector<std::string> getParNames() { return this->parNames; }
+    std::vector<std::string> getAuxNames() { return this->auxNames; }
 };
 
 class CLODE
 {
 
 protected:
-    //Problem details
+    // Problem details
     ProblemInfo prob;
     std::string clRHSfilename;
     cl_int nVar, nPar, nAux, nWiener;
-    cl_int nPts = 1;
+    cl_int nPts = 0;
 
-    //Stepper specification
+    // Stepper specification
     std::string stepper;
     std::vector<std::string> availableSteppers;
     std::map<std::string, std::string> stepperDefineMap;
 
     bool clSinglePrecision;
     size_t realSize;
 
-    //Compute device(s)
+    // Compute device(s)
     OpenCLResource opencl;
     std::string clodeRoot;
 
-    cl_int nRNGstate = 2; //TODO: different RNGs could be selected like steppers...?
+    cl_int nRNGstate = 2; // TODO: different RNGs could be selected like steppers...?
 
     SolverParams<cl_double> sp;
     std::vector<cl_double> tspan, x0, pars, xf, dt;
     size_t x0elements, parselements, RNGelements;
 
     std::vector<cl_ulong> RNGstate;
 
-    //Device variables
-    cl::Buffer d_tspan, d_x0, d_pars, d_sp, d_xf, d_RNGstate, d_dt;
+    // Device variables
+    cl::Buffer d_tspan, d_sp, d_pars, d_x0, d_xf, d_RNGstate, d_dt;
 
-    //kernel object
+    // kernel object
     std::string clprogramstring, buildOptions, ODEsystemsource;
     cl::Kernel cl_transient;
 
-    //flag to indicate whether kernel can be executed
-    bool clInitialized = false;
-
-    
+    void setClodeRoot(const std::string clodeRoot);
     void setCLbuildOpts(std::string extraBuildOpts = "");
+    void buildProgram(std::string extraBuildOpts = ""); // build the program object (inherited by subclasses)
+    void setNpts(cl_int newNpts);                       // resizes the nPts-dependent input variables - can't be called alone as it doesn't populate the arrays with data
     std::string getStepperDefine();
     SolverParams<cl_float> solverParamsToFloat(SolverParams<cl_double> sp);
 
     //~private:
     //~ CLODE( const CLODE& other ); // non construction-copyable
     //~ CLODE& operator=( const CLODE& ); // non copyable
 
-
 public:
-    //for now, require all arguments. TODO: convenience constructors?
+    // for now, require all arguments. TODO: convenience constructors?
     CLODE(ProblemInfo prob, std::string stepper, bool clSinglePrecision, OpenCLResource opencl, const std::string clodeRoot);
     CLODE(ProblemInfo prob, std::string stepper, bool clSinglePrecision, unsigned int platformID, unsigned int deviceID, const std::string clodeRoot);
     virtual ~CLODE();
 
-    //Set functions: trigger rebuild etc
-    void setNewProblem(ProblemInfo prob);               //requires rebuild: pars/vars. Opencl context OK
-    void setStepper(std::string newStepper);            //requires rebuild: Host + Device data OK
-    void setPrecision(bool clSinglePrecision);          //requires rebuild: all device vars. Opencl context OK
-    void setOpenCL(OpenCLResource opencl);              //requires rebuild: all device vars. Host problem data OK
+    // Setters that trigger need to rebuild CL program
+    void setProblemInfo(ProblemInfo prob);     // Opencl context OK
+    void setStepper(std::string newStepper);   // Host + Device data OK
+    void setPrecision(bool clSinglePrecision); // reset all device vars. Opencl context OK
+    void setOpenCL(OpenCLResource opencl);     // reset all device vars. Host problem data OK
     void setOpenCL(unsigned int platformID, unsigned int deviceID);
-    void setClodeRoot(const std::string clodeRoot);
 
-    void buildProgram(std::string extraBuildOpts = ""); //build the program object (inherited by subclasses)
     virtual void buildCL(); // build program and create kernel objects - overloaded by subclasses to include any extra kernels
 
-    // set all problem data needed to run
-    virtual void initialize(std::vector<cl_double> newTspan, std::vector<cl_double> newX0, std::vector<cl_double> newPars, SolverParams<cl_double> newSp);
-	bool isInitialized() { return clInitialized; };
-
-    void setNpts(cl_int newNpts); //resizes the nPts-dependent input variables
-    void setProblemData(std::vector<cl_double> newX0, std::vector<cl_double> newPars); //set both pars and X0 to change nPts
+    // no need to rebuild CL program
+    void setProblemData(std::vector<cl_double> newX0, std::vector<cl_double> newPars); // set both pars and X0 to change nPts
     void setTspan(std::vector<cl_double> newTspan);
-    void setX0(std::vector<cl_double> newX0);     //no change in nPts: newX0 must match nPts
-    void setPars(std::vector<cl_double> newPars); //no change in nPts: newPars must match nPts
+    void setX0(std::vector<cl_double> newX0);     // no change in nPts: newX0 must match nPts
+    void setPars(std::vector<cl_double> newPars); // no change in nPts: newPars must match nPts
     void setSolverParams(SolverParams<cl_double> newSp);
 
     void seedRNG();
-    void seedRNG(cl_int mySeed); //overload for setting reproducible seeds
+    void seedRNG(cl_int mySeed); // overload for setting reproducible seeds
 
-    //simulation routine. TODO: overloads?
-    void transient(); //integrate forward using stored tspan, x0, pars, and solver pars
+    // simulation routine. TODO: overloads?
+    void transient(); // integrate forward using stored tspan, x0, pars, and solver pars
     // void transient(std::vector<cl_double> newTspan); //integrate forward using stored x0, pars, and solver pars
     // void transient(std::vector<cl_double> newTspan, std::vector<cl_double> newX0); //integrate forward using stored pars, and solver pars
     // void transient(std::vector<cl_double> newTspan, std::vector<cl_double> newX0, std::vector<cl_double> newPars); //integrate forward using stored solver pars
     // void transient(std::vector<cl_double> newTspan, std::vector<cl_double> newX0, std::vector<cl_double> newPars, SolverParams<cl_double> newSp);
 
-    void shiftTspan(); //t0 <- tf, tf<-(tf + tf-t0)
-    void shiftX0();    //d_x0 <- d_xf (device to device transfer)
-
-    std::vector<cl_double> getTspan() { return tspan; };
-    std::vector<cl_double> getX0();
-    std::vector<cl_double> getXf();
-    std::string getProgramString();
-    std::vector<std::string> getAvailableSteppers() { return availableSteppers; };
-
-    void printStatus();
+    void shiftTspan(); // t0 <- tf, tf<-(tf + tf-t0)
+    void shiftX0();    // d_x0 <- d_xf (device to device transfer)
 
     // Getters
     const ProblemInfo getProblemInfo() const { return prob; };
+    const std::vector<cl_double> getTspan() const { return tspan; };
+    const SolverParams<cl_double> getSolverParams() const { return sp; };
+    const std::vector<cl_double> getPars() const { return pars; };
+    const std::vector<cl_double> getX0();
+    const std::vector<cl_double> getXf();
+    const std::vector<std::string> getAvailableSteppers() const { return availableSteppers; };
+
+    const std::string getProgramString() const { return buildOptions + clprogramstring + ODEsystemsource; };
+    void printStatus();
 };
 
-#endif //CLODE_HPP_
+#endif // CLODE_HPP_
```

### Comparing `clode-0.7.1/clode/cpp/CLODEfeatures.cpp` & `clode-0.8.1/clode/cpp/CLODEfeatures.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -2,173 +2,130 @@
 
 #include <algorithm> //std::max
 #include <cmath>
 #include <stdexcept>
 
 #include "spdlog/spdlog.h"
 
-CLODEfeatures::CLODEfeatures(ProblemInfo prob, std::string stepper, std::string observer, bool clSinglePrecision, OpenCLResource opencl, const std::string clodeRoot)
+CLODEfeatures::CLODEfeatures(ProblemInfo prob, std::string stepper, std::string observer, ObserverParams<cl_double> op, bool clSinglePrecision, OpenCLResource opencl, const std::string clodeRoot)
 	: CLODE(prob, stepper, clSinglePrecision, opencl, clodeRoot), observer(observer)
 {
-	// default fVarIx and eVarIx to allow first query of observer define map (exposes availableObservers, fNames)
-	op.fVarIx=0;
-	op.eVarIx=0;
+	setObserverParams(op);
 	updateObserverDefineMap();
 
 	clprogramstring += read_file(clodeRoot + "initializeObserver.cl");
 	clprogramstring += read_file(clodeRoot + "features.cl");
 	spdlog::debug("constructor clODEfeatures");
 }
 
-CLODEfeatures::CLODEfeatures(ProblemInfo prob, std::string stepper, std::string observer, bool clSinglePrecision,  unsigned int platformID, unsigned int deviceID, const std::string clodeRoot)
+CLODEfeatures::CLODEfeatures(ProblemInfo prob, std::string stepper, std::string observer, ObserverParams<cl_double> op, bool clSinglePrecision, unsigned int platformID, unsigned int deviceID, const std::string clodeRoot)
 	: CLODE(prob, stepper, clSinglePrecision, platformID, deviceID, clodeRoot), observer(observer)
 {
-	// default fVarIx and eVarIx to allow first query of observer define map
-	op.fVarIx=0;
-	op.eVarIx=0;
+	setObserverParams(op);
 	updateObserverDefineMap();
 
 	clprogramstring += read_file(clodeRoot + "initializeObserver.cl");
 	clprogramstring += read_file(clodeRoot + "features.cl");
 	spdlog::debug("constructor clODEfeatures");
 }
 
 CLODEfeatures::~CLODEfeatures() {}
 
 // build program and create kernel objects - requires host variables to be set (specifically observerBuildOpts)
 void CLODEfeatures::buildCL()
 {
-	observerBuildOpts=" -D" + observerDefineMap.at(observer).define;
+	spdlog::info("Running CLODEFeatures buildCL");
+	observerBuildOpts = " -D" + observerDefineMap.at(observer).define;
+	observerBuildOpts += " -DN_STORE_EVENTS=" + std::to_string((long long)op.maxEventTimestamps);
 	buildProgram(observerBuildOpts);
 
-	//set up the kernels
+	// set up the kernels
 	try
 	{
 		cl_transient = cl::Kernel(opencl.getProgram(), "transient", &opencl.error);
 		cl_initializeObserver = cl::Kernel(opencl.getProgram(), "initializeObserver", &opencl.error);
 		cl_features = cl::Kernel(opencl.getProgram(), "features", &opencl.error);
 
 		// size_t preferred_multiple;
 		// cl::Device dev;
 		// opencl.getProgram().getInfo(CL_PROGRAM_DEVICES,&dev);
 		// cl_features.getWorkGroupInfo(dev,CL_KERNEL_PREFERRED_WORK_GROUP_SIZE_MULTIPLE,&preferred_multiple);
 		// spdlog::info("Preferred work size multiple (features): {}",preferred_multiple);
 	}
 	catch (cl::Error &er)
 	{
-		spdlog::error("CLODEfeatures::initializeFeaturesKernel:{}({})", er.what(), CLErrorString(er.err()).c_str());
+		spdlog::error("CLODEfeatures::buildCL(): create kernels{}({})", er.what(), CLErrorString(er.err()).c_str());
 		throw er;
 	}
-	spdlog::debug("initialize features kernel");
-
-	clInitialized = false;
-	spdlog::debug("Using observer: {}",observer.c_str());
-}
-
-
-const std::string CLODEfeatures::getProgramString()
-{
-	observerBuildOpts=" -D" + observerDefineMap.at(observer).define;
-	setCLbuildOpts(observerBuildOpts);
-	return buildOptions+clprogramstring+ODEsystemsource; 
-}
-
-// void CLODEfeatures::initialize(std::vector<cl_double> newTspan, std::vector<cl_double> newX0, std::vector<cl_double> newPars, SolverParams<cl_double> newSp) {
-//     throw std::runtime_error("CLODEfeatures requires the newOp parameter!");
-// }
-
-//initialize everything
-void CLODEfeatures::initialize(std::vector<cl_double> newTspan, std::vector<cl_double> newX0, std::vector<cl_double> newPars, SolverParams<cl_double> newSp, ObserverParams<cl_double> newOp)
-{
-	clInitialized = false;
-
-	//at the time of initialize, make sure observerDataSize and nFeatures are up to date (for d_F, d_odata)
-	updateObserverDefineMap();
-
-	setTspan(newTspan);
-	setProblemData(newX0, newPars); //will set nPts
-	resizeFeaturesVariables(); //set up d_F and d_odata too, which depend on nPts
-	setSolverParams(newSp);
-	setObserverParams(newOp);
-
-	doObserverInitialization = true;
-	clInitialized = true;
-	spdlog::debug("initialize clODEfeatures.");
+	spdlog::debug("created features kernels");
+	spdlog::debug("Using observer: {}", observer.c_str());
 }
 
 void CLODEfeatures::setObserver(std::string newObserver)
 {
-	auto loc = observerDefineMap.find(newObserver); //from steppers.cl
-	if ( loc != observerDefineMap.end() )
+	auto loc = observerDefineMap.find(newObserver); // from steppers.cl
+	if (loc != observerDefineMap.end())
 	{
 		observer = newObserver;
 		updateObserverDefineMap();
-		clInitialized = false;
 	}
 	else
 	{
-		spdlog::warn("unknown observer: {}. Observer method unchanged",newObserver.c_str());
+		spdlog::warn("unknown observer: {}. Observer method unchanged", newObserver.c_str());
 	}
 	spdlog::debug("set observer");
 }
 
-
 void CLODEfeatures::setObserverParams(ObserverParams<cl_double> newOp)
 {
 	try
 	{
-		if (!clInitialized)
-		{
-			if (clSinglePrecision)
-				d_op = cl::Buffer(opencl.getContext(), CL_MEM_READ_ONLY, sizeof(ObserverParams<cl_float>), NULL, &opencl.error);
-			else
-				d_op = cl::Buffer(opencl.getContext(), CL_MEM_READ_ONLY, sizeof(ObserverParams<cl_double>), NULL, &opencl.error);
-		}
-
-		op = newOp; 
+		op = newOp;
 
 		if (clSinglePrecision)
-		{ //downcast to float if desired
+		{ // downcast to float if desired
 			ObserverParams<cl_float> opF = observerParamsToFloat(newOp);
+			d_op = cl::Buffer(opencl.getContext(), CL_MEM_READ_ONLY, sizeof(ObserverParams<cl_float>), NULL, &opencl.error);
 			opencl.error = opencl.getQueue().enqueueWriteBuffer(d_op, CL_TRUE, 0, sizeof(opF), &opF);
 		}
 		else
 		{
+			d_op = cl::Buffer(opencl.getContext(), CL_MEM_READ_ONLY, sizeof(ObserverParams<cl_double>), NULL, &opencl.error);
 			opencl.error = opencl.getQueue().enqueueWriteBuffer(d_op, CL_TRUE, 0, sizeof(op), &newOp);
 		}
 
-		//if op.fVarIx or op.eVarIx change, observer's fNames may change (doesn't need rebuild though)
+		// if op.fVarIx or op.eVarIx change, observer's fNames may change (doesn't need rebuild though)
 		updateObserverDefineMap();
 	}
 	catch (cl::Error &er)
 	{
 		spdlog::error("CLODEfeatures::setObserverParams:{}({})", er.what(), CLErrorString(er.err()).c_str());
 		throw er;
 	}
 	spdlog::debug("set observer params");
 }
 
-
 // updates the defineMap to reflect changes in problem, precision, observerParams
 void CLODEfeatures::updateObserverDefineMap()
 {
-	getObserverDefineMap(prob, op.fVarIx, op.eVarIx, observerDefineMap, availableObserverNames);
-	observerBuildOpts=" -D" + observerDefineMap.at(observer).define;
+	getObserverDefineMap(prob, op.fVarIx, op.eVarIx, op.maxEventTimestamps, observerDefineMap, availableObserverNames);
+	observerBuildOpts = " -D" + observerDefineMap.at(observer).define;
+	observerBuildOpts += " -DN_STORE_EVENTS=" + std::to_string((long long)op.maxEventTimestamps);
 	if (clSinglePrecision)
-		observerDataSize=observerDefineMap.at(observer).observerDataSizeFloat;
+		observerDataSize = observerDefineMap.at(observer).observerDataSizeFloat;
 	else
-		observerDataSize=observerDefineMap.at(observer).observerDataSizeDouble;
+		observerDataSize = observerDefineMap.at(observer).observerDataSizeDouble;
 	// spdlog::debug("observerDataSize = {}",observerDataSize);
 	// observerDataSize = observerDataSize + observerDataSize % realSize; //align to a multiple of realsize. is this necessary?
 
-	nFeatures=(int)observerDefineMap.at(observer).featureNames.size();
-	featureNames=observerDefineMap.at(observer).featureNames;
+	nFeatures = (int)observerDefineMap.at(observer).featureNames.size();
+	featureNames = observerDefineMap.at(observer).featureNames;
 }
 
-//TODO: define an assignment/type cast operator in the struct?
+// TODO: define an assignment/type cast operator in the struct?
 ObserverParams<cl_float> CLODEfeatures::observerParamsToFloat(ObserverParams<cl_double> op)
 {
 	ObserverParams<cl_float> opF;
 
 	opF.eVarIx = op.eVarIx;
 	opF.fVarIx = op.fVarIx;
 	opF.maxEventCount = op.maxEventCount;
@@ -191,141 +148,124 @@
 	if (largestAlloc > opencl.getMaxMemAllocSize())
 	{
 		int maxNpts = floor(opencl.getMaxMemAllocSize() / (cl_ulong)std::max(nFeatures * realSize, observerDataSize));
 		spdlog::info("nPts is too large, requested memory size exceeds selected device's limit. Maximum nPts appears to be {} ", maxNpts);
 		throw std::invalid_argument("nPts is too large");
 	}
 
-	//resize device variables if nPts changed, or if not yet initialized
-	if (!clInitialized || Felements != currentFelements)
+	// resize device variables if nPts changed
+	if (Felements != currentFelements)
 	{
 
 		Felements = currentFelements;
 		F.resize(currentFelements);
 
-		//resize device variables
+		// resize device variables
 		try
 		{
 			d_odata = cl::Buffer(opencl.getContext(), CL_MEM_READ_WRITE, observerDataSize * nPts, NULL, &opencl.error);
 			d_F = cl::Buffer(opencl.getContext(), CL_MEM_WRITE_ONLY, realSize * currentFelements, NULL, &opencl.error);
 		}
 		catch (cl::Error &er)
 		{
 			spdlog::error("CLODEfeatures::resizeFeaturesVariables:{}({})", er.what(), CLErrorString(er.err()).c_str());
 			throw er;
 		}
-		spdlog::debug("resize F, d_F, d_odata with: nPts={}, nF={}",nPts,nFeatures);
+		spdlog::debug("resize F, d_F, d_odata with: nPts={}, nF={}", nPts, nFeatures);
+
+		observerInitialized = false;
 	}
-	
 }
 
-//Simulation routines
-
-//
+// Simulation routines
 void CLODEfeatures::initializeObserver()
 {
+	// spdlog::info("do init={}",observerInitialized?"false":"true");
+	// resize output variables - will only occur if nPts has changed
+	resizeFeaturesVariables();
 
-	if (clInitialized)
+	try
 	{
-		// spdlog::info("do init={}",doObserverInitialization?"true":"false");
-		//resize output variables - will only occur if nPts has changed
-		resizeFeaturesVariables();
-
-		try
-		{
-			//kernel arguments
-			int ix = 0;
-			cl_initializeObserver.setArg(ix++, d_tspan);
-			cl_initializeObserver.setArg(ix++, d_x0);
-			cl_initializeObserver.setArg(ix++, d_pars);
-			cl_initializeObserver.setArg(ix++, d_sp);
-			cl_initializeObserver.setArg(ix++, d_RNGstate);
-			cl_initializeObserver.setArg(ix++, d_dt);
-			cl_initializeObserver.setArg(ix++, d_odata);
-			cl_initializeObserver.setArg(ix++, d_op);
-
-			//execute the kernel
-			opencl.error = opencl.getQueue().enqueueNDRangeKernel(cl_initializeObserver, cl::NullRange, cl::NDRange(nPts));
-			// spdlog::info("Enqueue error code: {}",CLErrorString(opencl.error).c_str());
-			opencl.error = opencl.getQueue().finish();
-			// spdlog::info("Finish Queue error code: {}",CLErrorString(opencl.error).c_str());
-			doObserverInitialization = false;
-		}
-		catch (cl::Error &er)
-		{
-			spdlog::error("CLODEfeatures::initializeObserver:{}({})", er.what(), CLErrorString(er.err()).c_str());
-			throw er;
-		}
-		spdlog::debug("run initializeObserver");
+		// kernel arguments
+		int ix = 0;
+		cl_initializeObserver.setArg(ix++, d_tspan);
+		cl_initializeObserver.setArg(ix++, d_x0);
+		cl_initializeObserver.setArg(ix++, d_pars);
+		cl_initializeObserver.setArg(ix++, d_sp);
+		cl_initializeObserver.setArg(ix++, d_RNGstate);
+		cl_initializeObserver.setArg(ix++, d_dt);
+		cl_initializeObserver.setArg(ix++, d_odata);
+		cl_initializeObserver.setArg(ix++, d_op);
+
+		// execute the kernel
+		opencl.error = opencl.getQueue().enqueueNDRangeKernel(cl_initializeObserver, cl::NullRange, cl::NDRange(nPts));
+		// spdlog::info("Enqueue error code: {}",CLErrorString(opencl.error).c_str());
+		opencl.error = opencl.getQueue().finish();
+		// spdlog::info("Finish Queue error code: {}",CLErrorString(opencl.error).c_str());
 	}
-	else
+	catch (cl::Error &er)
 	{
-		spdlog::info("CLODE has not been initialized");
+		spdlog::error("CLODEfeatures::initializeObserver:{}({})", er.what(), CLErrorString(er.err()).c_str());
+		throw er;
 	}
+	observerInitialized = true;
+	spdlog::debug("run initializeObserver");
 }
 
-//overload to allow manual re-initialization of observer data at any time.
-void CLODEfeatures::features(bool newDoObserverInitFlag)
+// overload to allow manual re-initialization of observer data at any time.
+void CLODEfeatures::features(bool reinitialize_observer)
 {
-	doObserverInitialization = newDoObserverInitFlag;
+	observerInitialized = !reinitialize_observer;
 
 	features();
 }
 
 void CLODEfeatures::features()
 {
+	// spdlog::info("do init={}",observerInitialized?"false":"true");
+	// resize output variables - will only occur if nPts has changed
+	resizeFeaturesVariables();
 
-	if (clInitialized)
-	{
-		// spdlog::info("do init={}",doObserverInitialization?"true":"false");
-		//resize output variables - will only occur if nPts has changed
-		resizeFeaturesVariables();
+	if (!observerInitialized)
+		initializeObserver();
 
-		if (doObserverInitialization)
-			initializeObserver();
-
-		try
-		{
-			//kernel arguments
-			int ix = 0;
-			cl_features.setArg(ix++, d_tspan);
-			cl_features.setArg(ix++, d_x0);
-			cl_features.setArg(ix++, d_pars);
-			cl_features.setArg(ix++, d_sp);
-			cl_features.setArg(ix++, d_xf);
-			cl_features.setArg(ix++, d_RNGstate);
-			cl_features.setArg(ix++, d_dt);
-			cl_features.setArg(ix++, d_odata);
-			cl_features.setArg(ix++, d_op);
-			cl_features.setArg(ix++, d_F);
-
-			//execute the kernel
-			opencl.error = opencl.getQueue().enqueueNDRangeKernel(cl_features, cl::NullRange, cl::NDRange(nPts));
-			// spdlog::info("Enqueue error code: {}",CLErrorString(opencl.error).c_str());
-			opencl.error = opencl.getQueue().finish();
-			// spdlog::info("Finish Queue error code: {}",CLErrorString(opencl.error).c_str());
-		}
-		catch (cl::Error &er)
-		{
-			spdlog::error("CLODEfeatures::features:{}({})", er.what(), CLErrorString(er.err()).c_str());
-			throw er;
-		}
-		spdlog::debug("run features");
+	try
+	{
+		// kernel arguments
+		int ix = 0;
+		cl_features.setArg(ix++, d_tspan);
+		cl_features.setArg(ix++, d_x0);
+		cl_features.setArg(ix++, d_pars);
+		cl_features.setArg(ix++, d_sp);
+		cl_features.setArg(ix++, d_xf);
+		cl_features.setArg(ix++, d_RNGstate);
+		cl_features.setArg(ix++, d_dt);
+		cl_features.setArg(ix++, d_odata);
+		cl_features.setArg(ix++, d_op);
+		cl_features.setArg(ix++, d_F);
+
+		// execute the kernel
+		opencl.error = opencl.getQueue().enqueueNDRangeKernel(cl_features, cl::NullRange, cl::NDRange(nPts));
+		// spdlog::info("Enqueue error code: {}",CLErrorString(opencl.error).c_str());
+		opencl.error = opencl.getQueue().finish();
+		// spdlog::info("Finish Queue error code: {}",CLErrorString(opencl.error).c_str());
 	}
-	else
+	catch (cl::Error &er)
 	{
-		spdlog::info("CLODE has not been initialized");
+		spdlog::error("CLODEfeatures::features:{}({})", er.what(), CLErrorString(er.err()).c_str());
+		throw er;
 	}
+	spdlog::debug("run features");
 }
 
 const std::vector<cl_double> CLODEfeatures::getF()
 {
 
 	if (clSinglePrecision)
-	{ //cast back to double
+	{ // cast back to double
 		std::vector<cl_float> FF(Felements);
 		opencl.error = copy(opencl.getQueue(), d_F, FF.begin(), FF.end());
 		F.assign(FF.begin(), FF.end());
 	}
 	else
 	{
 		opencl.error = copy(opencl.getQueue(), d_F, F.begin(), F.end());
```

### Comparing `clode-0.7.1/clode/cpp/CLODEfeatures.hpp` & `clode-0.8.1/clode/cpp/CLODEfeatures.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -23,60 +23,56 @@
 class CLODEfeatures : public CLODE
 {
 
 protected:
     std::string observer;
     size_t ObserverParamsSize;
 
-    std::map<std::string, ObserverInfo> observerDefineMap;
+    std::map<std::string, struct ObserverInfo> observerDefineMap;
     std::vector<std::string> featureNames;
     std::vector<std::string> availableObserverNames;
 
     int nFeatures;
     size_t observerDataSize;
     std::vector<cl_double> F;
     ObserverParams<cl_double> op;
     size_t Felements;
-    bool doObserverInitialization = true;
+    bool observerInitialized = false;
 
     cl::Buffer d_odata, d_op, d_F;
     cl::Kernel cl_initializeObserver;
     cl::Kernel cl_features;
 
     std::string observerBuildOpts;
     std::string observerName;
 
     ObserverParams<cl_float> observerParamsToFloat(ObserverParams<cl_double> op);
-
     std::string getObserverBuildOpts();
     void updateObserverDefineMap(); // update host variables representing feature detector: nFeatures, featureNames, observerDataSize
-    void resizeFeaturesVariables(); //d_odata and d_F depend on nPts. nPts change invalidates d_odata
+    void resizeFeaturesVariables(); // d_odata and d_F depend on nPts. nPts change invalidates d_odata
 
 public:
-    CLODEfeatures(ProblemInfo prob, std::string stepper, std::string observer, bool clSinglePrecision, OpenCLResource opencl, const std::string clodeRoot);
-    CLODEfeatures(ProblemInfo prob, std::string stepper, std::string observer, bool clSinglePrecision, unsigned int platformID, unsigned int deviceID, const std::string clodeRoot);
+    CLODEfeatures(ProblemInfo prob, std::string stepper, std::string observer, ObserverParams<cl_double> op, bool clSinglePrecision, OpenCLResource opencl, const std::string clodeRoot);
+    CLODEfeatures(ProblemInfo prob, std::string stepper, std::string observer, ObserverParams<cl_double> op, bool clSinglePrecision, unsigned int platformID, unsigned int deviceID, const std::string clodeRoot);
     virtual ~CLODEfeatures();
 
-    //build program, set all problem data needed to run
-    using CLODE::initialize;
-    virtual void initialize(std::vector<cl_double> newTspan, std::vector<cl_double> newX0, std::vector<cl_double> newPars, SolverParams<cl_double> newSp, ObserverParams<cl_double> newOp);
-
-    void setObserverParams(ObserverParams<cl_double> newOp);
-    void setObserver(std::string newObserver); //requires rebuild: program, kernel, kernel args. Host + Device data OK
+    void buildCL() override; // build program and create kernel objects
 
-    virtual void buildCL(); // build program and create kernel objects
+    void setObserverParams(ObserverParams<cl_double> newOp); // requires rebuild: maxEventTimestamps in ObserverData... TODO: ideally decouple this!
+    void setObserver(std::string newObserver);               // requires rebuild: program, kernel, kernel args. Host + Device data OK
 
-    //simulation routine.
-    void initializeObserver();                 //initialize Observer struct: possibly integrate forward an interval of duration (tf-t0), rewinds to t0
-    void features();                           //integrate forward using stored tspan, x0, pars, and solver pars
-    void features(bool newDoObserverInitFlag); //allow manually forcing re-init of observer data
+    // simulation routine.
+    void initializeObserver();                 // initialize Observer struct: possibly integrate forward an interval of duration (tf-t0), rewinds to t0
+    void features();                           // integrate forward using stored tspan, x0, pars, and solver pars
+    void features(bool reinitialize_observer); // allow manually forcing re-init of observer data
+    bool isObserverInitialized() { return observerInitialized; };
 
-    //Get functions
+    // Get functions
+    const ObserverParams<cl_double> getObserverParams() const { return op; };
     const std::string getObserverName() const { return observerName; }
-    const std::string getProgramString();
     const std::vector<cl_double> getF();
     const int getNFeatures() const { return nFeatures; };
-    const std::vector<std::string> getFeatureNames() const { return featureNames;};
-    const std::vector<std::string> getAvailableObservers() const { return availableObserverNames;};
+    const std::vector<std::string> getFeatureNames() const { return featureNames; };
+    const std::vector<std::string> getAvailableObservers() const { return availableObserverNames; };
 };
 
-#endif //CLODE_FEATURES_HPP_
+#endif // CLODE_FEATURES_HPP_
```

### Comparing `clode-0.7.1/clode/cpp/CLODEpython.cpp` & `clode-0.8.1/clode/cpp/CLODEpython.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -17,84 +17,90 @@
 #include "spdlog/spdlog.h"
 
 namespace py = pybind11;
 
 template <typename... Args>
 using overload_cast_ = py::detail::overload_cast_impl<Args...>;
 
-std::string vector_to_string(const std::vector<std::string> &vec){
+std::string vector_to_string(const std::vector<std::string> &vec)
+{
     std::string out = "[";
-    for (const std::string &s : vec){
+    for (const std::string &s : vec)
+    {
         out += s + ", ";
     }
     out += "]";
     return out;
 }
 
-PYBIND11_MODULE(clode_cpp_wrapper, m) {
+PYBIND11_MODULE(clode_cpp_wrapper, m)
+{
 
     m.doc() = "CLODE C++/Python interface"; // optional module docstring
 
-
     // logging
     /****************************************************/
 
     py::enum_<spdlog::level::level_enum>(m, "LogLevel")
         .value("trace", spdlog::level::trace)
         .value("debug", spdlog::level::debug)
         .value("info", spdlog::level::info)
         .value("warn", spdlog::level::warn)
         .value("err", spdlog::level::err)
         .value("critical", spdlog::level::critical)
         .value("off", spdlog::level::off)
         .export_values();
 
-    struct LoggerSingleton {
+    struct LoggerSingleton
+    {
         std::shared_ptr<PythonSink_mt> sink;
         std::shared_ptr<spdlog::logger> python_logger;
-        LoggerSingleton() {
+        LoggerSingleton()
+        {
             spdlog::set_level(spdlog::level::info);
             sink = std::make_shared<PythonSink_mt>();
             python_logger = std::make_shared<spdlog::logger>("python", sink);
             spdlog::set_default_logger(python_logger);
         }
 
-        static LoggerSingleton& instance()
+        static LoggerSingleton &instance()
         {
             static LoggerSingleton just_one;
             return just_one;
         }
 
-        void set_log_level(spdlog::level::level_enum level){
+        void set_log_level(spdlog::level::level_enum level)
+        {
             python_logger->set_level(level);
         };
 
-        void set_log_pattern(std::string &pattern){
+        void set_log_pattern(std::string &pattern)
+        {
             python_logger->set_pattern(pattern);
         };
 
-        spdlog::level::level_enum get_log_level() {
+        spdlog::level::level_enum get_log_level()
+        {
             return python_logger->level();
         };
     };
 
     py::class_<LoggerSingleton>(m, "LoggerSingleton")
         .def("set_log_level", &LoggerSingleton::set_log_level)
         .def("set_log_pattern", &LoggerSingleton::set_log_pattern)
         .def("get_log_level", &LoggerSingleton::get_log_level);
 
     m.def("get_logger",
-        &LoggerSingleton::instance,
-        py::return_value_policy::reference,
-        "Get logger singleton instance");
-
+          &LoggerSingleton::instance,
+          py::return_value_policy::reference,
+          "Get logger singleton instance");
 
     // OpenCL runtime
     /****************************************************/
-    
+
     py::enum_<cl_vendor>(m, "CLVendor")
         .value("VENDOR_ANY", VENDOR_ANY)
         .value("VENDOR_NVIDIA", VENDOR_NVIDIA)
         .value("VENDOR_AMD", VENDOR_AMD)
         .value("VENDOR_INTEL", VENDOR_INTEL)
         .export_values();
 
@@ -130,236 +136,244 @@
         .def_readwrite("max_clock", &deviceInfo::maxClock)
         .def_readwrite("max_work_group_size", &deviceInfo::maxWorkGroupSize)
         .def_readwrite("device_memory_size", &deviceInfo::deviceMemSize)
         .def_readwrite("max_memory_alloc_size", &deviceInfo::maxMemAllocSize)
         .def_readwrite("extensions", &deviceInfo::extensions)
         .def_readwrite("double_support", &deviceInfo::doubleSupport)
         .def_readwrite("device_available", &deviceInfo::deviceAvailable)
-        .def("__repr__", [](const deviceInfo &d) {
-            return "<device_info(name=" + d.name +
-                   ", vendor=" + d.vendor +
-                   ", version=" + d.version +
-                   ", device_type=" + d.devTypeStr +
-                   ", compute_units=" + std::to_string(d.computeUnits) +
-                   ", max_clock=" + std::to_string(d.maxClock) +
-                   ", max_work_group_size=" + std::to_string(d.maxWorkGroupSize) +
-                   ", device_memory_size=" + std::to_string(d.deviceMemSize) +
-                   ", max_memory_alloc_size=" + std::to_string(d.maxMemAllocSize) +
-                   ", extensions=" + d.extensions +
-                   ", double_support=" + std::to_string(d.doubleSupport) +
-                   ", device_available=" + std::to_string(d.deviceAvailable) +
-                   ")>";
-        }, "Device info string representation");
+        .def(
+            "__repr__", [](const deviceInfo &d)
+            { return "<device_info(name=" + d.name +
+                     ", vendor=" + d.vendor +
+                     ", version=" + d.version +
+                     ", device_type=" + d.devTypeStr +
+                     ", compute_units=" + std::to_string(d.computeUnits) +
+                     ", max_clock=" + std::to_string(d.maxClock) +
+                     ", max_work_group_size=" + std::to_string(d.maxWorkGroupSize) +
+                     ", device_memory_size=" + std::to_string(d.deviceMemSize) +
+                     ", max_memory_alloc_size=" + std::to_string(d.maxMemAllocSize) +
+                     ", extensions=" + d.extensions +
+                     ", double_support=" + std::to_string(d.doubleSupport) +
+                     ", device_available=" + std::to_string(d.deviceAvailable) +
+                     ")>"; },
+            "Device info string representation");
 
     py::class_<platformInfo>(m, "PlatformInfo")
         .def_readwrite("name", &platformInfo::name)
         .def_readwrite("vendor", &platformInfo::vendor)
         .def_readwrite("version", &platformInfo::version)
         .def_readwrite("device_info", &platformInfo::device_info)
         .def_readwrite("device_count", &platformInfo::nDevices)
-        .def("__repr__", [](const platformInfo &p) {
-            return "<platform_info(name=" + p.name +
-                   ", vendor=" + p.vendor +
-                   ", version=" + p.version +
-                   ", device_count=" + std::to_string(p.nDevices) +
-                   ")>";
-        }, "Platform info string representation");
+        .def(
+            "__repr__", [](const platformInfo &p)
+            { return "<platform_info(name=" + p.name +
+                     ", vendor=" + p.vendor +
+                     ", version=" + p.version +
+                     ", device_count=" + std::to_string(p.nDevices) +
+                     ")>"; },
+            "Platform info string representation");
 
     m.def("query_opencl", &queryOpenCL, "Query OpenCL devices");
-    m.def("print_opencl", overload_cast_<>()(&printOpenCL), "Print OpenCL devices");
-
+    m.def("_print_opencl", overload_cast_<>()(&printOpenCL), "Print OpenCL devices");
 
-    // core clODE solver 
+    // core clODE solver
     /****************************************************/
 
     py::class_<ProblemInfo>(m, "ProblemInfo")
-            .def(py::init<const std::string &,
-                 const std::vector<std::string> &,
-                 const std::vector<std::string> &,
-                 const std::vector<std::string> &,
-                 int>(),
-                 py::arg("src_file"),
-                 py::arg("vars"),
-                 py::arg("pars"),
-                 py::arg("aux") = std::vector<std::string>(),
-                 py::arg("num_noise") = 1)
-                 .def(py::init<>())
-                 .def_readwrite("src_file", &ProblemInfo::clRHSfilename)
-                 .def_readwrite("num_noise", &ProblemInfo::nWiener)
-                 .def_property("vars", &ProblemInfo::getVarNames, &ProblemInfo::setVarNames)
-                 .def_property("pars", &ProblemInfo::getParNames, &ProblemInfo::setParNames)
-                 .def_property("aux", &ProblemInfo::getAuxNames, &ProblemInfo::setAuxNames)
-                 .def("__repr__", [](const ProblemInfo &p) {
-                     return "<problem_info(src_file=" + p.clRHSfilename +
-                           ", vars=" + vector_to_string(p.varNames) +
-                           ", pars=" + vector_to_string(p.parNames) +
-                           ", aux=" + vector_to_string(p.auxNames) +
-                           ", num_noise=" + std::to_string(p.nWiener) +
-                           ")>";
-                 }, "clode Problem info string representation");
+        .def(py::init<const std::string &,
+                      const std::vector<std::string> &,
+                      const std::vector<std::string> &,
+                      const std::vector<std::string> &,
+                      int>(),
+             py::arg("src_file"),
+             py::arg("vars"),
+             py::arg("pars"),
+             py::arg("aux") = std::vector<std::string>(),
+             py::arg("num_noise") = 1)
+        .def(py::init<>())
+        .def_readwrite("src_file", &ProblemInfo::clRHSfilename)
+        .def_readwrite("num_var", &ProblemInfo::nVar)
+        .def_readwrite("num_par", &ProblemInfo::nPar)
+        .def_readwrite("num_aux", &ProblemInfo::nAux)
+        .def_readwrite("num_noise", &ProblemInfo::nWiener)
+        .def_property("vars", &ProblemInfo::getVarNames, &ProblemInfo::setVarNames)
+        .def_property("pars", &ProblemInfo::getParNames, &ProblemInfo::setParNames)
+        .def_property("aux", &ProblemInfo::getAuxNames, &ProblemInfo::setAuxNames)
+        .def(
+            "__repr__", [](const ProblemInfo &p)
+            { return "<problem_info(src_file=" + p.clRHSfilename +
+                     ", vars=" + vector_to_string(p.varNames) +
+                     ", pars=" + vector_to_string(p.parNames) +
+                     ", aux=" + vector_to_string(p.auxNames) +
+                     ", num_noise=" + std::to_string(p.nWiener) +
+                     ")>"; },
+            "clode Problem info string representation");
 
     py::class_<SolverParams<double>>(m, "SolverParams")
-    .def(py::init<double,
-                double,
-                double,
-                double,
-                int,
-                int,
-                int>(),
-                py::arg("dt") = 0.1,
-                py::arg("dtmax") = 0.5,
-                py::arg("abstol") = 1e-6,
-                py::arg("reltol") = 1e-3,
-                py::arg("max_steps") = 1000000,
-                py::arg("max_store") = 1000000,
-                py::arg("nout") = 1
-    ).def_readwrite("dt", &SolverParams<double>::dt)
-    .def_readwrite("dtmax", &SolverParams<double>::dtmax)
-    .def_readwrite("abstol", &SolverParams<double>::abstol)
-    .def_readwrite("reltol", &SolverParams<double>::reltol)
-    .def_readwrite("max_steps", &SolverParams<double>::max_steps)
-    .def_readwrite("max_store", &SolverParams<double>::max_store)
-    .def_readwrite("nout", &SolverParams<double>::nout)
-    .def("__repr__", [](const SolverParams<double> &s) {
-        return "<solver_params(dt=" + std::to_string(s.dt) +
-               ", dtmax=" + std::to_string(s.dtmax) +
-               ", abstol=" + std::to_string(s.abstol) +
-               ", reltol=" + std::to_string(s.reltol) +
-               ", max_steps=" + std::to_string(s.max_steps) +
-               ", max_store=" + std::to_string(s.max_store) +
-               ", nout=" + std::to_string(s.nout) +
-               ")>";
-    }, "Solver params string representation");
-    
-    py::class_<CLODE>(m, "SimulatorBase")
-            .def(py::init<ProblemInfo &,
-                    std::string &,
-                    bool,
-                    OpenCLResource &,
-                    std::string &>(),
-                    	py::arg("problem_info"),
-                    	py::arg("stepper"),
-                    	py::arg("cl_single_precision"),
-                    	py::arg("opencl_resource"),
-                    	py::arg("clode_root"))
-            .def("initialize", static_cast<void (CLODE::*)
-                    (std::vector<double>,
-                     std::vector<double>,
-                     std::vector<double>,
-                     SolverParams<double>)>
-            (&CLODE::initialize), "Initialize CLODE", py::arg("tspan"), py::arg("x0"), py::arg("pars"), py::arg("solver_params"))
-            .def("seed_rng", static_cast<void (CLODE::*)(int)>(&CLODE::seedRNG), "Seed RNG", py::arg("seed"))
-            .def("seed_rng", static_cast<void (CLODE::*)()>(&CLODE::seedRNG), "Seed RNG")
-            .def("build_cl", &CLODE::buildCL)
-            .def("set_tspan", static_cast<void (CLODE::*)(std::vector<double>)>(&CLODE::setTspan))
-            .def("set_problem_data", static_cast<void (CLODE::*)(std::vector<double>, std::vector<double>)>(&CLODE::setProblemData))
-            .def("set_x0", static_cast<void (CLODE::*)(std::vector<double>)>(&CLODE::setX0))
-            .def("set_pars", static_cast<void (CLODE::*)(std::vector<double>)>(&CLODE::setPars))
-            .def("set_solver_params", static_cast<void (CLODE::*)(SolverParams<double>)>(&CLODE::setSolverParams))
-            .def("transient", &CLODE::transient)
-            .def("shift_tspan", &CLODE::shiftTspan)
-            .def("shift_x0", &CLODE::shiftX0)
-            .def("get_tspan", &CLODE::getTspan)
-            .def("get_x0", &CLODE::getX0)
-            .def("get_xf", &CLODE::getXf)
-            .def("get_available_steppers", &CLODE::getAvailableSteppers)
-            .def("get_problem_info", &CLODE::getProblemInfo)
-            .def("get_program_string", &CLODE::getProgramString)
-            .def("print_status", &CLODE::printStatus)
-            .def("is_initialized", &CLODE::isInitialized);
+        .def(py::init<double,
+                      double,
+                      double,
+                      double,
+                      unsigned int,
+                      unsigned int,
+                      unsigned int>(),
+             py::arg("dt") = 0.1,
+             py::arg("dtmax") = 0.5,
+             py::arg("abstol") = 1e-6,
+             py::arg("reltol") = 1e-3,
+             py::arg("max_steps") = 1000000,
+             py::arg("max_store") = 1000000,
+             py::arg("nout") = 1)
+        .def_readwrite("dt", &SolverParams<double>::dt)
+        .def_readwrite("dtmax", &SolverParams<double>::dtmax)
+        .def_readwrite("abstol", &SolverParams<double>::abstol)
+        .def_readwrite("reltol", &SolverParams<double>::reltol)
+        .def_readwrite("max_steps", &SolverParams<double>::max_steps)
+        .def_readwrite("max_store", &SolverParams<double>::max_store)
+        .def_readwrite("nout", &SolverParams<double>::nout)
+        .def(
+            "__repr__", [](const SolverParams<double> &s)
+            { return "<solver_params(dt=" + std::to_string(s.dt) +
+                     ", dtmax=" + std::to_string(s.dtmax) +
+                     ", abstol=" + std::to_string(s.abstol) +
+                     ", reltol=" + std::to_string(s.reltol) +
+                     ", max_steps=" + std::to_string(s.max_steps) +
+                     ", max_store=" + std::to_string(s.max_store) +
+                     ", nout=" + std::to_string(s.nout) +
+                     ")>"; },
+            "Solver params string representation");
 
+    py::class_<CLODE>(m, "SimulatorBase")
+        .def(py::init<ProblemInfo &,
+                      std::string &,
+                      bool,
+                      OpenCLResource &,
+                      std::string &>(),
+             py::arg("problem_info"),
+             py::arg("stepper"),
+             py::arg("cl_single_precision"),
+             py::arg("opencl_resource"),
+             py::arg("clode_root"))
+        .def("set_problem_info", static_cast<void (CLODE::*)(ProblemInfo)>(&CLODE::setProblemInfo))
+        .def("set_stepper", static_cast<void (CLODE::*)(std::string)>(&CLODE::setStepper))
+        .def("set_precision", static_cast<void (CLODE::*)(bool)>(&CLODE::setPrecision))
+        .def("set_opencl", static_cast<void (CLODE::*)(OpenCLResource opencl)>(&CLODE::setOpenCL))
+        .def("set_opencl", static_cast<void (CLODE::*)(unsigned int platformID, unsigned int deviceID)>(&CLODE::setOpenCL))
+        .def("build_cl", &CLODE::buildCL)
+        .def("set_problem_data", static_cast<void (CLODE::*)(std::vector<double>, std::vector<double>)>(&CLODE::setProblemData))
+        .def("set_tspan", static_cast<void (CLODE::*)(std::vector<double>)>(&CLODE::setTspan))
+        .def("set_x0", static_cast<void (CLODE::*)(std::vector<double>)>(&CLODE::setX0))
+        .def("set_pars", static_cast<void (CLODE::*)(std::vector<double>)>(&CLODE::setPars))
+        .def("set_solver_params", static_cast<void (CLODE::*)(SolverParams<double>)>(&CLODE::setSolverParams))
+        .def("seed_rng", static_cast<void (CLODE::*)()>(&CLODE::seedRNG), "Seed RNG")
+        .def("seed_rng", static_cast<void (CLODE::*)(int)>(&CLODE::seedRNG), "Seed RNG", py::arg("seed"))
+        .def("transient", &CLODE::transient)
+        .def("shift_tspan", &CLODE::shiftTspan)
+        .def("shift_x0", &CLODE::shiftX0)
+        .def("get_problem_info", &CLODE::getProblemInfo)
+        .def("get_tspan", &CLODE::getTspan)
+        .def("get_solver_params", &CLODE::getSolverParams)
+        .def("get_pars", &CLODE::getPars)
+        .def("get_x0", &CLODE::getX0)
+        .def("get_xf", &CLODE::getXf)
+        .def("get_available_steppers", &CLODE::getAvailableSteppers)
+        .def("get_program_string", &CLODE::getProgramString)
+        .def("print_status", &CLODE::printStatus);
 
-    // clODE features specialization 
+    // clODE features specialization
     /****************************************************/
 
     py::class_<ObserverParams<double>>(m, "ObserverParams")
-    .def(py::init<int,
-            int,
-            int,
-            double,
-            double,
-            double,
-            double,
-            double,
-            double,
-            double,
-            double>
-            ()
-    ).def_readwrite("e_var_ix", &ObserverParams<double>::eVarIx)
-    .def_readwrite("f_var_ix", &ObserverParams<double>::fVarIx)
-    .def_readwrite("maxEventCount", &ObserverParams<double>::maxEventCount)
-    .def("__repr__", [](const ObserverParams<double> &p) {
-        return "<observer_params(e_var_ix=" + std::to_string(p.eVarIx) +
-               ", f_var_ix=" + std::to_string(p.fVarIx) +
-               ", maxEventCount=" + std::to_string(p.maxEventCount) +
-               ", minXamp=" + std::to_string(p.minXamp) +
-               ", minIMI=" + std::to_string(p.minIMI) +
-               ", nHoodRadius=" + std::to_string(p.nHoodRadius) +
-               ", xUpThresh=" + std::to_string(p.xUpThresh) +
-               ", xDownThresh=" + std::to_string(p.xDownThresh) +
-               ", dxUpThresh=" + std::to_string(p.dxUpThresh) +
-               ", dxDownThresh=" + std::to_string(p.dxDownThresh) +
-               ", eps_dx=" + std::to_string(p.eps_dx) +
-               ")>";
-    });
+        .def(py::init<unsigned int,
+                      unsigned int,
+                      unsigned int,
+                      unsigned int,
+                      double,
+                      double,
+                      double,
+                      double,
+                      double,
+                      double,
+                      double,
+                      double>(),
+             py::arg("e_var_ix") = 0,
+             py::arg("f_var_ix") = 0,
+             py::arg("max_event_count") = 100,
+             py::arg("max_event_timestamps") = 0,
+             py::arg("min_amp") = 0.,
+             py::arg("min_imi") = 0.,
+             py::arg("nhood_radius") = 0.05,
+             py::arg("x_up_threshold") = 0.2,
+             py::arg("x_down_threshold") = 0.2,
+             py::arg("dx_up_threshold") = 0.,
+             py::arg("dx_down_threshold") = 0.,
+             py::arg("eps_dx") = 0.)
+        .def_readwrite("e_var_ix", &ObserverParams<double>::eVarIx)
+        .def_readwrite("f_var_ix", &ObserverParams<double>::fVarIx)
+        .def_readwrite("max_event_count", &ObserverParams<double>::maxEventCount)
+        .def_readwrite("max_event_timestamps", &ObserverParams<double>::maxEventTimestamps)
+        .def_readwrite("min_amp", &ObserverParams<double>::minXamp)
+        .def_readwrite("min_imi", &ObserverParams<double>::minIMI)
+        .def_readwrite("nhood_radius", &ObserverParams<double>::nHoodRadius)
+        .def_readwrite("x_up_threshold", &ObserverParams<double>::xUpThresh)
+        .def_readwrite("x_down_threshold", &ObserverParams<double>::xDownThresh)
+        .def_readwrite("dx_up_threshold", &ObserverParams<double>::dxUpThresh)
+        .def_readwrite("dx_down_threshold", &ObserverParams<double>::dxDownThresh)
+        .def_readwrite("eps_dx", &ObserverParams<double>::eps_dx)
+        .def("__repr__", [](const ObserverParams<double> &p)
+             { return "<observer_params(e_var_ix=" + std::to_string(p.eVarIx) +
+                      ", f_var_ix=" + std::to_string(p.fVarIx) +
+                      ", max_event_count=" + std::to_string(p.maxEventCount) +
+                      ", max_event_timestamps=" + std::to_string(p.maxEventTimestamps) +
+                      ", min_amp=" + std::to_string(p.minXamp) +
+                      ", min_imi=" + std::to_string(p.minIMI) +
+                      ", nhood_radius=" + std::to_string(p.nHoodRadius) +
+                      ", x_up_threshold=" + std::to_string(p.xUpThresh) +
+                      ", x_down_threshold=" + std::to_string(p.xDownThresh) +
+                      ", dx_up_threshold=" + std::to_string(p.dxUpThresh) +
+                      ", dx_down_threshold=" + std::to_string(p.dxDownThresh) +
+                      ", eps_dx=" + std::to_string(p.eps_dx) +
+                      ")>"; });
 
     py::class_<CLODEfeatures, CLODE>(m, "FeatureSimulatorBase")
-            .def(py::init<ProblemInfo &,
-                          std::string &,
-                          std::string &,
-                          bool,
-                          OpenCLResource &,
-                          std::string &>())
-            .def("initialize", static_cast<void (CLODEfeatures::*)
-                    (std::vector<double>,
-                     std::vector<double>,
-                     std::vector<double>,
-                     SolverParams<double>)>
-                     (&CLODEfeatures::initialize), "Initialize FeatureSimulatorBase")
-            .def("initialize", static_cast<void (CLODEfeatures::*)
-                                                    (std::vector<double>,
-                                                    std::vector<double>,
-                                                    std::vector<double>,
-                                                    SolverParams<double>,
-                                                    ObserverParams<double>)>
-                                                    (&CLODEfeatures::initialize), "Initialize FeatureSimulatorBase")
-            .def("build_cl", &CLODEfeatures::buildCL)
-            .def("features", static_cast<void (CLODEfeatures::*)(bool)>(&CLODEfeatures::features)) //CLODEfeatures specializations
-            .def("features", static_cast<void (CLODEfeatures::*)()>(&CLODEfeatures::features))
-            .def("set_observer_params", static_cast<void (CLODEfeatures::*)(ObserverParams<double>)>(&CLODEfeatures::setObserverParams))
-            .def("get_observer_name", &CLODEfeatures::getObserverName)
-            .def("get_n_features", &CLODEfeatures::getNFeatures)
-            .def("get_feature_names", &CLODEfeatures::getFeatureNames)
-            .def("get_f", &CLODEfeatures::getF)
-            .def("get_available_observers", &CLODEfeatures::getAvailableObservers)
-            .def("__repr__", [](const CLODEfeatures &c) {
-                return "<CLODEfeatures (observer="
-                + c.getObserverName()
-                + ", n_features="
-                + std::to_string(c.getNFeatures())
-                + ")>";
-            }, "CLODEfeatures string representation");
-
+        .def(py::init<ProblemInfo &,
+                      std::string &,
+                      std::string &,
+                      ObserverParams<double>,
+                      bool,
+                      OpenCLResource &,
+                      std::string &>())
+        .def("build_cl", &CLODEfeatures::buildCL)
+        .def("set_observer_params", static_cast<void (CLODEfeatures::*)(ObserverParams<double>)>(&CLODEfeatures::setObserverParams))
+        .def("set_observer", static_cast<void (CLODEfeatures::*)(std::string)>(&CLODEfeatures::setObserver))
+        .def("initialize_observer", &CLODEfeatures::initializeObserver)
+        .def("is_observer_initialized", &CLODEfeatures::isObserverInitialized)
+        .def("features", static_cast<void (CLODEfeatures::*)(bool)>(&CLODEfeatures::features))
+        .def("features", static_cast<void (CLODEfeatures::*)()>(&CLODEfeatures::features))
+        .def("get_observer_params", &CLODEfeatures::getObserverParams)
+        .def("get_observer_name", &CLODEfeatures::getObserverName)
+        .def("get_f", &CLODEfeatures::getF)
+        .def("get_n_features", &CLODEfeatures::getNFeatures)
+        .def("get_feature_names", &CLODEfeatures::getFeatureNames)
+        .def("get_available_observers", &CLODEfeatures::getAvailableObservers)
+        .def(
+            "__repr__", [](const CLODEfeatures &c)
+            { return "<CLODEfeatures (observer=" + c.getObserverName() + ", n_features=" + std::to_string(c.getNFeatures()) + ")>"; },
+            "CLODEfeatures string representation");
 
     // clODE trajectory specialization
     /****************************************************/
 
     py::class_<CLODEtrajectory, CLODE>(m, "TrajectorySimulatorBase")
-            .def(py::init<ProblemInfo &,
-                    std::string &,
-                    bool,
-                    OpenCLResource &,
-                    std::string &>())
-            .def("initialize", static_cast<void (CLODEtrajectory::*)
-                    (std::vector<double>,
-                     std::vector<double>,
-                     std::vector<double>,
-                     SolverParams<double>)>
-            (&CLODEtrajectory::initialize), "Initialize TrajectorySimulatorBase")
-            .def("build_cl", &CLODEtrajectory::buildCL)
-            .def("trajectory", &CLODEtrajectory::trajectory)    //CLODEtrajectory specializations
-            .def("get_t", &CLODEtrajectory::getT)
-            .def("get_x", &CLODEtrajectory::getX)
-            .def("get_dx", &CLODEtrajectory::getDx)
-            .def("get_aux", &CLODEtrajectory::getAux)
-            .def("get_n_stored", &CLODEtrajectory::getNstored);
+        .def(py::init<ProblemInfo &,
+                      std::string &,
+                      bool,
+                      OpenCLResource &,
+                      std::string &>())
+        .def("build_cl", &CLODEtrajectory::buildCL)
+        .def("trajectory", &CLODEtrajectory::trajectory) // CLODEtrajectory specializations
+        .def("get_t", &CLODEtrajectory::getT)
+        .def("get_x", &CLODEtrajectory::getX)
+        .def("get_dx", &CLODEtrajectory::getDx)
+        .def("get_aux", &CLODEtrajectory::getAux)
+        .def("get_n_stored", &CLODEtrajectory::getNstored);
 }
```

### Comparing `clode-0.7.1/clode/cpp/CLODEtrajectory.cpp` & `clode-0.8.1/clode/cpp/CLODEtrajectory.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -5,114 +5,83 @@
 #include <stdexcept>
 
 #include "spdlog/spdlog.h"
 
 CLODEtrajectory::CLODEtrajectory(ProblemInfo prob, std::string stepper, bool clSinglePrecision, OpenCLResource opencl, const std::string clodeRoot)
 	: CLODE(prob, stepper, clSinglePrecision, opencl, clodeRoot), nStoreMax(0)
 {
-
-	//printf("CLODE has been specialized: CLODEtrajectory");
-
 	clprogramstring += read_file(clodeRoot + "trajectory.cl");
 	spdlog::debug("constructor clODEtrajectory");
 }
 
 CLODEtrajectory::CLODEtrajectory(ProblemInfo prob, std::string stepper, bool clSinglePrecision, unsigned int platformID, unsigned int deviceID, const std::string clodeRoot)
 	: CLODE(prob, stepper, clSinglePrecision, platformID, deviceID, clodeRoot), nStoreMax(0)
 {
-
-	//printf("CLODE has been specialized: CLODEtrajectory");
-
 	clprogramstring += read_file(clodeRoot + "trajectory.cl");
 	spdlog::debug("constructor clODEtrajectory");
 }
 
 CLODEtrajectory::~CLODEtrajectory() {}
 
-
 // build program and create kernel objects. requires host variables to be set
 void CLODEtrajectory::buildCL()
 {
+	spdlog::info("Running CLODEtrajectory buildCL");
 	buildProgram();
 
-	//set up the kernels
+	// set up the kernels
 	try
 	{
 		cl_transient = cl::Kernel(opencl.getProgram(), "transient", &opencl.error);
 		cl_trajectory = cl::Kernel(opencl.getProgram(), "trajectory", &opencl.error);
 	}
 	catch (cl::Error &er)
 	{
-		spdlog::error("CLODEtrajectory::initializeTrajectoryKernel():{}({})", er.what(), CLErrorString(er.err()).c_str());
+		spdlog::error("CLODEtrajectory::buildCL() create kernels:{}({})", er.what(), CLErrorString(er.err()).c_str());
 		throw er;
 	}
-	clInitialized = false;
-	spdlog::debug("initialize trajectory kernel");
-}
-
-//initialize everything
-void CLODEtrajectory::initialize(std::vector<cl_double> newTspan, std::vector<cl_double> newX0, std::vector<cl_double> newPars, SolverParams<cl_double> newSp)
-{
-
-	clInitialized = false;
-
-	setTspan(newTspan);
-	setProblemData(newX0, newPars); //will set nPts
-	setSolverParams(newSp);
-	//set up output variables, depends on sp.max_store, nPts, nVar, nAux
-	resizeTrajectoryVariables(); 
-
-	clInitialized = true;
-	spdlog::debug("initialize clODEtrajectory");
+	spdlog::debug("Created trajectory kernels");
 }
 
 void CLODEtrajectory::resizeTrajectoryVariables()
 {
+	int currentStoreAlloc = sp.max_store; // TODO: time chunking for long trajectories
 
-	int currentStoreAlloc = sp.max_store; //TODO: always alloc sp.max_store? or try to compute something?
-	//catch any changes to tspan, dt, or nout:
-	// int currentStoreAlloc=(tspan[1]-tspan[0])/(sp.dt*sp.nout)+1;
-	// currentStoreAlloc=std::min(currentStoreAlloc, sp.max_store);
-	//~ if (currentStoreAlloc > sp.max_store) {
-	//~ currentStoreAlloc=sp.max_store;
-	//~ printf("Warning: (tspan[1]-tspan[0])/(dt*nout)+1 > max_store. Reducing storage to max_store={} timepoints. ",sp.max_store);
-	//~ }
-
-	//check largest desired memory chunk against device's maximum allowable variable size
+	// check largest desired memory chunk against device's maximum allowable variable size
 	size_t largestAlloc = std::max(1 /*t*/, std::max(nVar /*x, dx*/, nAux /*aux*/)) * nPts * currentStoreAlloc * realSize;
 
 	if (largestAlloc > opencl.getMaxMemAllocSize())
 	{
 		int estimatedMaxStoreAlloc = std::floor(opencl.getMaxMemAllocSize() / (std::max(1, std::max(nVar, nAux)) * nPts * realSize));
-        spdlog::error("Storage requested exceeds device maximum variable size. Reason: {}. Try reducing storage to <{} time points, or reducing nPts. ", nAux > nVar ? "aux vars" : "state vars", estimatedMaxStoreAlloc);
+		spdlog::error("Storage requested exceeds device maximum variable size. Reason: {}. Try reducing storage to <{} time points, or reducing nPts. ", nAux > nVar ? "aux vars" : "state vars", estimatedMaxStoreAlloc);
 		throw std::invalid_argument("nPts*nStoreMax*nVar*realSize or nPts*nStoreMax*nAux*realSize is too big");
 	}
 
 	size_t currentTelements = currentStoreAlloc * nPts;
 
-	//only resize device variables if size changed, or if not yet initialized
-	if (!clInitialized || nStoreMax != currentStoreAlloc || telements != currentTelements)
+	// only resize device variables if size changed
+	if (nStoreMax != currentStoreAlloc || telements != currentTelements)
 	{
 
 		nStoreMax = currentStoreAlloc;
 		telements = currentTelements;
 		xelements = nVar * currentTelements;
 		// cl::Buffer doesn't like zero-sized arrays:
-		auxelements = nAux>0 ? nAux * currentTelements : 1;
+		auxelements = nAux > 0 ? nAux * currentTelements : 1;
 
 		t.resize(telements);
 		x.resize(xelements);
 		dx.resize(xelements);
 		aux.resize(auxelements);
 		nStored.resize(nPts);
 
-		//resize device variables
+		// resize device variables
 		try
 		{
-			//trajectory
+			// trajectory
 			d_t = cl::Buffer(opencl.getContext(), CL_MEM_WRITE_ONLY, realSize * telements, NULL, &opencl.error);
 			d_x = cl::Buffer(opencl.getContext(), CL_MEM_WRITE_ONLY, realSize * xelements, NULL, &opencl.error);
 			d_dx = cl::Buffer(opencl.getContext(), CL_MEM_WRITE_ONLY, realSize * xelements, NULL, &opencl.error);
 			d_aux = cl::Buffer(opencl.getContext(), CL_MEM_WRITE_ONLY, realSize * auxelements, NULL, &opencl.error);
 			d_nStored = cl::Buffer(opencl.getContext(), CL_MEM_WRITE_ONLY, sizeof(int) * nPts, NULL, &opencl.error);
 		}
 		catch (cl::Error &er)
@@ -120,61 +89,54 @@
 			spdlog::error("CLODEtrajectory::resizeTrajectoryVariables():{}({})", er.what(), CLErrorString(er.err()).c_str());
 			throw er;
 		}
 		spdlog::debug("resize d_t, d_x, d_dx, d_aux, d_nStored");
 	}
 }
 
-//Simulation routine
+// Simulation routine
 void CLODEtrajectory::trajectory()
 {
-	if (clInitialized)
-	{
-		//resize output variables - will only occur if nPts or nSteps has changed [~4ms overhead on Tornado]
-		resizeTrajectoryVariables();
+	// resize output variables - will only occur if nPts or nSteps has changed [~4ms overhead on Tornado]
+	resizeTrajectoryVariables();
 
-		try
-		{
-			//kernel arguments
-			int ix = 0;
-			cl_trajectory.setArg(ix++, d_tspan);
-			cl_trajectory.setArg(ix++, d_x0);
-			cl_trajectory.setArg(ix++, d_pars);
-			cl_trajectory.setArg(ix++, d_sp);
-			cl_trajectory.setArg(ix++, d_xf);
-			cl_trajectory.setArg(ix++, d_RNGstate);
-			cl_trajectory.setArg(ix++, d_dt);
-			cl_trajectory.setArg(ix++, d_t);
-			cl_trajectory.setArg(ix++, d_x);
-			cl_trajectory.setArg(ix++, d_dx);
-			cl_trajectory.setArg(ix++, d_aux);
-			cl_trajectory.setArg(ix++, d_nStored);
-
-			//execute the kernel
-			opencl.error = opencl.getQueue().enqueueNDRangeKernel(cl_trajectory, cl::NullRange, cl::NDRange(nPts));
-			opencl.getQueue().finish();
-		}
-		catch (cl::Error &er)
-		{
-			spdlog::error("CLODEtrajectory::trajectory():{}({})", er.what(), CLErrorString(er.err()).c_str());
-			throw er;
-		}
-		spdlog::debug("run trajectory");
+	try
+	{
+		// kernel arguments
+		int ix = 0;
+		cl_trajectory.setArg(ix++, d_tspan);
+		cl_trajectory.setArg(ix++, d_x0);
+		cl_trajectory.setArg(ix++, d_pars);
+		cl_trajectory.setArg(ix++, d_sp);
+		cl_trajectory.setArg(ix++, d_xf);
+		cl_trajectory.setArg(ix++, d_RNGstate);
+		cl_trajectory.setArg(ix++, d_dt);
+		cl_trajectory.setArg(ix++, d_t);
+		cl_trajectory.setArg(ix++, d_x);
+		cl_trajectory.setArg(ix++, d_dx);
+		cl_trajectory.setArg(ix++, d_aux);
+		cl_trajectory.setArg(ix++, d_nStored);
+
+		// execute the kernel
+		opencl.error = opencl.getQueue().enqueueNDRangeKernel(cl_trajectory, cl::NullRange, cl::NDRange(nPts));
+		opencl.getQueue().finish();
 	}
-	else
+	catch (cl::Error &er)
 	{
-		printf("CLODE has not been initialized");
+		spdlog::error("CLODEtrajectory::trajectory():{}({})", er.what(), CLErrorString(er.err()).c_str());
+		throw er;
 	}
+	spdlog::debug("run trajectory");
 }
 
 std::vector<cl_double> CLODEtrajectory::getT()
 {
 
 	if (clSinglePrecision)
-	{ //cast back to double
+	{ // cast back to double
 		std::vector<cl_float> tF(telements);
 		opencl.error = copy(opencl.getQueue(), d_t, tF.begin(), tF.end());
 		t.assign(tF.begin(), tF.end());
 	}
 	else
 	{
 		opencl.error = copy(opencl.getQueue(), d_t, t.begin(), t.end());
@@ -183,15 +145,15 @@
 	return t;
 }
 
 std::vector<cl_double> CLODEtrajectory::getX()
 {
 
 	if (clSinglePrecision)
-	{ //cast back to double
+	{ // cast back to double
 		std::vector<cl_float> xF(xelements);
 		opencl.error = copy(opencl.getQueue(), d_x, xF.begin(), xF.end());
 		x.assign(xF.begin(), xF.end());
 	}
 	else
 	{
 		opencl.error = copy(opencl.getQueue(), d_x, x.begin(), x.end());
@@ -200,29 +162,29 @@
 	return x;
 }
 
 std::vector<cl_double> CLODEtrajectory::getDx()
 {
 
 	if (clSinglePrecision)
-	{ //cast back to double
+	{ // cast back to double
 		std::vector<cl_float> dxF(xelements);
 		opencl.error = copy(opencl.getQueue(), d_dx, dxF.begin(), dxF.end());
 		dx.assign(dxF.begin(), dxF.end());
 	}
 	else
 	{
 		opencl.error = copy(opencl.getQueue(), d_dx, dx.begin(), dx.end());
 	}
 
 	return dx;
 }
 
 std::vector<cl_double> CLODEtrajectory::getAux()
-{ //cast back to double
+{ // cast back to double
 
 	if (clSinglePrecision)
 	{
 		std::vector<cl_float> auxF(auxelements);
 		opencl.error = copy(opencl.getQueue(), d_aux, auxF.begin(), auxF.end());
 		aux.assign(auxF.begin(), auxF.end());
 	}
```

### Comparing `clode-0.7.1/clode/cpp/CLODEtrajectory.hpp` & `clode-0.8.1/clode/cpp/CLODEtrajectory.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -20,37 +20,34 @@
 
 class CLODEtrajectory : public CLODE
 {
 
 protected:
     cl_int nStoreMax;
     std::vector<cl_int> nStored;
-    std::vector<cl_double> t, x, dx, aux; //new result vectors
+    std::vector<cl_double> t, x, dx, aux; // new result vectors
     size_t telements, xelements, auxelements;
 
     cl::Buffer d_t, d_x, d_dx, d_aux, d_nStored;
     cl::Kernel cl_trajectory;
 
-    void resizeTrajectoryVariables(); //creates trajectory output global variables, called just before launching trajectory kernel
+    void resizeTrajectoryVariables(); // creates trajectory output global variables, called just before launching trajectory kernel
 
 public:
-    CLODEtrajectory(ProblemInfo prob, std::string stepper, bool clSinglePrecision, OpenCLResource opencl, const std::string clodeRoot); //will construct the base class with same arguments
+    CLODEtrajectory(ProblemInfo prob, std::string stepper, bool clSinglePrecision, OpenCLResource opencl, const std::string clodeRoot); // will construct the base class with same arguments
     CLODEtrajectory(ProblemInfo prob, std::string stepper, bool clSinglePrecision, unsigned int platformID, unsigned int deviceID, const std::string clodeRoot);
     virtual ~CLODEtrajectory();
 
-    virtual void buildCL(); // build program and create kernel objects
+    void buildCL() override; // build program and create kernel objects
 
-    //build program, set all problem data needed to run
-    virtual void initialize(std::vector<cl_double> newTspan, std::vector<cl_double> newX0, std::vector<cl_double> newPars, SolverParams<cl_double> newSp);
+    // simulation routine. TODO: overloads?
+    void trajectory(); // integrate forward an interval of duration (tf-t0)
 
-    //simulation routine. TODO: overloads?
-    void trajectory(); //integrate forward an interval of duration (tf-t0)
-
-    //Get functions
+    // Get functions
     std::vector<cl_double> getT();
     std::vector<cl_double> getX();
     std::vector<cl_double> getDx();
     std::vector<cl_double> getAux();
     std::vector<cl_int> getNstored();
 };
 
-#endif //CLODE_HPP_
+#endif // CLODE_HPP_
```

### Comparing `clode-0.7.1/clode/cpp/OpenCL/BUILD` & `clode-0.8.1/clode/cpp/OpenCL/BUILD`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/clode/cpp/OpenCL/cl.hpp` & `clode-0.8.1/clode/cpp/OpenCL/cl.hpp`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/clode/cpp/OpenCL/cl2.hpp` & `clode-0.8.1/clode/cpp/OpenCL/cl2.hpp`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/clode/cpp/OpenCL/opencl.hpp` & `clode-0.8.1/clode/cpp/OpenCL/opencl.hpp`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/clode/cpp/OpenCLResource.cpp` & `clode-0.8.1/clode/cpp/OpenCLResource.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 /*
  * OpenCLResource.cpp
  *
  *  Copyright 2017 Patrick Fletcher <patrick.fletcher@nih.gov>
- * 
+ *
  */
 
 #include "OpenCLResource.hpp"
 
 #include <stdexcept>
 #include <fstream>
 #include <filesystem>
 
 #include "spdlog/spdlog.h"
 
-/******************************** 
+/********************************
  * OpenCLResource Member Functions
  ********************************/
 
 OpenCLResource::OpenCLResource()
 {
     getPlatformAndDevices(CL_DEVICE_TYPE_DEFAULT, VENDOR_ANY);
     initializeOpenCL();
@@ -50,15 +50,15 @@
     getPlatformAndDevices(type, vendor);
     initializeOpenCL();
 }
 
 OpenCLResource::OpenCLResource(int argc, char **argv)
 {
 
-    //modified from openCLUtilities to include accelerators as a devicetype
+    // modified from openCLUtilities to include accelerators as a devicetype
     cl_deviceType type = CL_DEVICE_TYPE_ALL;
     cl_vendor vendor = VENDOR_ANY;
     int nValidArgs = 0;
 
     for (int i = 1; i < argc; i++)
     {
         if (strcmp(argv[i], "--device") == 0)
@@ -121,20 +121,20 @@
 OpenCLResource::OpenCLResource(unsigned int platformID, std::vector<unsigned int> deviceIDs)
 {
 
     getPlatformAndDevices(platformID, deviceIDs);
     initializeOpenCL();
 };
 
-//modified from openCLUtilities
-//TODO: check various possibilities on default? eg: any Accel, any non-intel GPU, intel GPU, any CPU
+// modified from openCLUtilities
+// TODO: check various possibilities on default? eg: any Accel, any non-intel GPU, intel GPU, any CPU
 void OpenCLResource::getPlatformAndDevices(cl_deviceType type, cl_vendor vendor)
 {
 
-    //query all platform and device info, store as a vector of structs
+    // query all platform and device info, store as a vector of structs
     //~ std::vector<platformInfo> pinfo=queryOpenCL();
 
     // Get available platforms
     std::vector<cl::Platform> platforms;
     cl::Platform::get(&platforms);
 
     if (platforms.size() == 0)
@@ -165,41 +165,41 @@
         {
             if (platforms[i].getInfo<CL_PLATFORM_VENDOR>().find(vendorStr) != std::string::npos)
             {
                 tempPlatforms.push_back(platforms[i]);
             }
         }
 
-        platforms = tempPlatforms; //keep only the platforms with correct vendor
+        platforms = tempPlatforms; // keep only the platforms with correct vendor
     }
 
     std::vector<cl::Device> tempDevices;
     for (unsigned int i = 0; i < platforms.size(); i++)
     {
         try
         {
             platforms[i].getDevices(type, &tempDevices);
-            //TODO: apply extra device filters (eg. extensionSupported,enoughMem,...) here?
+            // TODO: apply extra device filters (eg. extensionSupported,enoughMem,...) here?
             tempID = i;
             break;
         }
         catch (cl::Error &e)
         {
             continue;
         }
     }
 
     if (tempID == -1)
         throw cl::Error(1, "No compatible OpenCL platform found");
 
-    //we found a platform with compatible device(s) to use
+    // we found a platform with compatible device(s) to use
     platform = platforms[tempID];
     devices = tempDevices;
 
-    //get info for the selected plaform and device(s)
+    // get info for the selected plaform and device(s)
     platform_info = getPlatformInfo(platform, devices);
 }
 
 void OpenCLResource::getPlatformAndDevices(unsigned int platformID, std::vector<unsigned int> deviceIDs)
 {
 
     std::vector<cl::Platform> platforms;
@@ -230,22 +230,21 @@
         }
         else
         {
             throw std::out_of_range("Specified deviceID exceeds the number devices on the selected platform");
         }
     }
 
-    //get info for the selected plaform and device(s)
+    // get info for the selected plaform and device(s)
     platform_info = getPlatformInfo(platform, devices);
 }
 
-//create the OpenCL context from the device list, and a queue for each device
+// create the OpenCL context from the device list, and a queue for each device
 void OpenCLResource::initializeOpenCL()
 {
-
     try
     {
         context = cl::Context(devices);
         for (unsigned int i = 0; i < devices.size(); ++i)
             queues.push_back(cl::CommandQueue(context, devices[i]));
     }
     catch (cl::Error &er)
@@ -253,72 +252,81 @@
         spdlog::error("{}({})", er.what(), CLErrorString(er.err()).c_str());
         throw er;
     }
 
     spdlog::debug("OpenCLResource Created");
 }
 
-//attempt to build OpenCL program given as a string, build options empty if not supplied.
+// attempt to build OpenCL program given as a string, build options empty if not supplied.
 void OpenCLResource::buildProgramFromString(std::string sourceStr, std::string buildOptions)
 {
-
+    spdlog::debug("Building program from string");
+    spdlog::trace(sourceStr.c_str());
+    spdlog::debug(buildOptions.c_str());
     cl::Program::Sources source(1, std::make_pair(sourceStr.c_str(), sourceStr.length()));
     std::string buildLog;
     cl_int builderror;
     try
     {
         program = cl::Program(context, source, &error);
-        spdlog::debug("Program Object creation error code: {}",CLErrorString(error).c_str());
+        spdlog::debug("Program Object creation error code: {}", CLErrorString(error).c_str());
 
         builderror = program.build(devices, buildOptions.c_str());
-        spdlog::debug("Program Object build error code: {}",CLErrorString(builderror).c_str());
+        spdlog::debug("Program Object build error code: {}", CLErrorString(builderror).c_str());
 
         std::string kernelnames;
-        program.getInfo(CL_PROGRAM_KERNEL_NAMES,&kernelnames);
+        program.getInfo(CL_PROGRAM_KERNEL_NAMES, &kernelnames);
         spdlog::debug("Kernels built:   {}", kernelnames.c_str());
     }
     catch (cl::Error &er)
     {
         spdlog::error("{}({})", er.what(), CLErrorString(er.err()).c_str());
         if (er.err() == CL_BUILD_PROGRAM_FAILURE)
         {
             // spdlog::info("{}",sourceStr.c_str());
             for (unsigned int i = 0; i < devices.size(); ++i)
             {
                 program.getBuildInfo(devices[i], CL_PROGRAM_BUILD_LOG, &buildLog);
                 spdlog::error("OpenCL build log, Device {}:", i);
                 spdlog::error("{}", buildLog.c_str());
-                //spdlog::error(std::__fs::filesystem::current_path().c_str());
+                // spdlog::error(std::__fs::filesystem::current_path().c_str());
             }
         }
         throw er;
     }
 }
 
 void OpenCLResource::buildProgramFromSource(std::string filename, std::string buildOptions)
 {
-
+    spdlog::debug("Building program from source file");
+    spdlog::trace(filename.c_str());
+    spdlog::debug(buildOptions.c_str());
     std::string sourceStr = read_file(filename);
     buildProgramFromString(sourceStr, buildOptions);
 }
 
-//prints the selected platform and devices information (queried on the fly)
+// void OpenCLResource::writeProgramBinary()
+// {
+//     write_file("cl_program.ptx", program.getInfo<CL_PROGRAM_BINARIES>()[0]); // save binary (ptx file)
+// }
+
+// prints the selected platform and devices information (queried on the fly)
 void OpenCLResource::print()
 {
     std::string tmp;
     spdlog::info("Selected platform and device: ");
     spdlog::info("Platform  --------------------");
     printPlatformInfo(platform_info);
 }
 
-/******************************** 
+/********************************
  * Other functions
  ********************************/
 
-//get info of all devices on all platforms
+// get info of all devices on all platforms
 std::vector<platformInfo> queryOpenCL()
 {
 
     std::vector<cl::Platform> platforms;
     cl::Platform::get(&platforms);
     if (platforms.size() == 0)
         throw cl::Error(1, "No OpenCL platforms were found");
@@ -329,43 +337,43 @@
     {
         pinfo.push_back(getPlatformInfo(platforms[i]));
     }
 
     return pinfo;
 }
 
-//get info of a given cl::Platform and its devices (optionally only devices of a given type, default is CL_DEVICE_TYPE_ALL)
+// get info of a given cl::Platform and its devices (optionally only devices of a given type, default is CL_DEVICE_TYPE_ALL)
 platformInfo getPlatformInfo(cl::Platform platform, std::vector<cl::Device> devices)
 {
 
     platformInfo pinfo;
     platform.getInfo(CL_PLATFORM_NAME, &pinfo.name);
     platform.getInfo(CL_PLATFORM_VENDOR, &pinfo.vendor);
     platform.getInfo(CL_PLATFORM_VERSION, &pinfo.version);
 
     if (devices.size() == 0)
-    { //get all the devices
+    { // get all the devices
         platform.getDevices(CL_DEVICE_TYPE_ALL, &devices);
     }
 
     pinfo.nDevices = (unsigned int)devices.size();
 
     for (unsigned int j = 0; j < pinfo.nDevices; j++)
         pinfo.device_info.push_back(getDeviceInfo(devices[j]));
 
     return pinfo;
 }
 
-//get info for given cl::Device
+// get info for given cl::Device
 deviceInfo getDeviceInfo(cl::Device device)
 {
 
     deviceInfo dinfo;
 
-    //Get device info for this compute resource
+    // Get device info for this compute resource
     device.getInfo(CL_DEVICE_NAME, &dinfo.name);
     device.getInfo(CL_DEVICE_VENDOR, &dinfo.vendor);
     device.getInfo(CL_DEVICE_VERSION, &dinfo.version);
     device.getInfo(CL_DEVICE_TYPE, &dinfo.devType);
     switch (dinfo.devType)
     {
     case CL_DEVICE_TYPE_CPU:
@@ -393,58 +401,70 @@
 
     device.getInfo(CL_DEVICE_EXTENSIONS, &dinfo.extensions);
     device.getInfo(CL_DEVICE_AVAILABLE, &dinfo.deviceAvailable);
 
     return dinfo;
 }
 
-//print information about all platforms and devices found
+// TODO: kernel info
+
+// /* cl_kernel_work_group_info */
+// #define CL_KERNEL_WORK_GROUP_SIZE                   0x11B0
+// #define CL_KERNEL_COMPILE_WORK_GROUP_SIZE           0x11B1
+// #define CL_KERNEL_LOCAL_MEM_SIZE                    0x11B2
+// #define CL_KERNEL_PREFERRED_WORK_GROUP_SIZE_MULTIPLE 0x11B3
+// #define CL_KERNEL_PRIVATE_MEM_SIZE                  0x11B4
+// #ifdef CL_VERSION_1_2
+// #define CL_KERNEL_GLOBAL_WORK_SIZE                  0x11B5
+// #endif
+
+// print information about all platforms and devices found
 void printOpenCL()
 {
 
     spdlog::info("Querying OpenCL platforms...");
     std::vector<platformInfo> pinfo = queryOpenCL();
     printOpenCL(pinfo);
 }
 
-//print information about all platforms and devices found, given pre-queried array of platformInfo structs
+// print information about all platforms and devices found, given pre-queried array of platformInfo structs
 void printOpenCL(std::vector<platformInfo> pinfo)
 {
 
     spdlog::info("Number of platforms found: {}", (unsigned int)pinfo.size());
     for (unsigned int i = 0; i < pinfo.size(); ++i)
     {
         spdlog::info("- Platform {} ------------------------------", i);
         printPlatformInfo(pinfo[i]);
     }
     spdlog::info("");
 }
 
-//print information about a platform and its devices given pre-queried info in platformInfo struct
+// print information about a platform and its devices given pre-queried info in platformInfo struct
 void printPlatformInfo(platformInfo pinfo)
 {
     spdlog::info("Name:    {}", pinfo.name.c_str());
     spdlog::info("Vendor:  {}", pinfo.vendor.c_str());
     spdlog::info("Version: {}", pinfo.version.c_str());
 
     for (unsigned int j = 0; j < pinfo.nDevices; j++)
     {
         spdlog::info("- Device {} ------------", j);
         printDeviceInfo(pinfo.device_info[j]);
     }
 }
 
-//print info about a specific cl::Device
+// print info about a specific cl::Device
 void printDeviceInfo(cl::Device device)
 {
     deviceInfo dinfo = getDeviceInfo(device);
     printDeviceInfo(dinfo);
 }
 
-//print info about a specific cl::Device given pre-queried info in deviceInfo struct
+// print info about a specific cl::Device given pre-queried info in deviceInfo struct
 void printDeviceInfo(deviceInfo dinfo)
 {
     spdlog::info("  Name:   {}", dinfo.name.c_str());
     spdlog::info("  Type:   {}", dinfo.devTypeStr.c_str());
     spdlog::info("  Vendor: {}", dinfo.vendor.c_str());
     spdlog::info("  Version: {}", dinfo.version.c_str());
     spdlog::info("  Compute units (CUs): {}", dinfo.computeUnits);
@@ -562,12 +582,17 @@
 {
     std::ifstream sourceFile(filename.c_str());
     if (sourceFile.fail())
     {
         spdlog::error("Cannot find file {}", filename.c_str());
         throw cl::Error(1, "Failed to open OpenCL source file");
     }
-    std::string sourceStr(std::istreambuf_iterator<char>(sourceFile), (std::istreambuf_iterator<char>())); //second arg is "end of stream" iterator
+    std::string sourceStr(std::istreambuf_iterator<char>(sourceFile), (std::istreambuf_iterator<char>()));
     sourceFile.close();
-    // spdlog::info(sourceStr.c_str());
     return sourceStr;
 }
+
+// void write_file(const std::string& filename, const std::string& content="") {
+// 	std::ofstream file(filename, std::ios::out);
+// 	file.write(content.c_str(), content.length());
+// 	file.close();
+// }
```

### Comparing `clode-0.7.1/clode/cpp/OpenCLResource.hpp` & `clode-0.8.1/clode/cpp/OpenCLResource.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 //
-// Created by Patrick Fletcher 2017 
+// Created by Patrick Fletcher 2017
 // - Inspired by openCLUtilities (https://www.eriksmistad.no/opencl-utilities/)
 //
 
+// also consider: https://github.com/ProjectPhysX/OpenCL-Wrapper
 
 #ifndef OPENCL_RESOURCE_HPP_
 #define OPENCL_RESOURCE_HPP_
 
 #define CL_HPP_ENABLE_EXCEPTIONS
 #define CL_HPP_MINIMUM_OPENCL_VERSION 120
 #define CL_HPP_TARGET_OPENCL_VERSION 120
 #define CL_HPP_CL_1_2_DEFAULT_BUILD
 #define CL_HPP_ENABLE_PROGRAM_CONSTRUCTION_FROM_ARRAY_COMPATIBILITY
 
 #include "OpenCL/cl2.hpp"
-
 // we should be using opencl.hpp from here: https://github.com/KhronosGroup/OpenCL-CLHPP
 // e.g., see https://github.com/KhronosGroup/OpenCL-SDK/tree/main/external
 // - works as a drop-in replacement
 
 #include <string>
 #include <vector>
 
@@ -28,24 +28,25 @@
 {
 	VENDOR_ANY = 0,
 	VENDOR_NVIDIA,
 	VENDOR_AMD,
 	VENDOR_INTEL
 };
 
-enum e_cl_device_type {
+enum e_cl_device_type
+{
 	DEVICE_TYPE_ALL = CL_DEVICE_TYPE_ALL,
 	DEVICE_TYPE_CPU = CL_DEVICE_TYPE_CPU,
 	DEVICE_TYPE_GPU = CL_DEVICE_TYPE_GPU,
 	DEVICE_TYPE_ACCELERATOR = CL_DEVICE_TYPE_ACCELERATOR,
 	DEVICE_TYPE_DEFAULT = CL_DEVICE_TYPE_DEFAULT,
 	DEVICE_TYPE_CUSTOM = CL_DEVICE_TYPE_CUSTOM
 };
 
-//struct to hold a reduced set of information about a device
+// struct to hold a reduced set of information about a device
 typedef struct deviceInfo
 {
 	std::string name;
 	std::string vendor;
 	std::string version;
 	cl_device_type devType;
 	std::string devTypeStr;
@@ -73,80 +74,74 @@
 {
 
 	cl::Platform platform;
 	platformInfo platform_info;
 	cl::Context context;
 	cl::Program program;
 
-	//the following vectors will all contain one entry per device in the context
+	// the following vectors will all contain one entry per device in the context
 	std::vector<cl::Device> devices;
-	std::vector<cl::CommandQueue> queues; //could have many queues per device...
+	std::vector<cl::CommandQueue> queues; // could have many queues per device...
 
-	//TODO: figure out how to use events... one per queue? one per context? for syncing & barriers, out-of-order queues etc..
-	//cl::Event event;
+	// TODO: figure out how to use events... one per queue? one per context? for syncing & barriers, out-of-order queues etc..
+	// cl::Event event;
 
-	//helper functions to get the desired platform and device(s), and create the context and command queues
+	// helper functions to get the desired platform and device(s), and create the context and command queues
 	void getPlatformAndDevices(cl_deviceType type = CL_DEVICE_TYPE_ALL, cl_vendor vendor = VENDOR_ANY);
-	void getPlatformAndDevices(unsigned int platformID, std::vector<unsigned int> deviceID); //cl_device_type collides with int... function signature ambiguous
+	void getPlatformAndDevices(unsigned int platformID, std::vector<unsigned int> deviceID); // cl_device_type collides with int... function signature ambiguous
 	void initializeOpenCL();
 
 public:
-	//constructors
-
-	//optionally specify device type and/or vendor using enum defined above.
-
-	//~ OpenCLResource(cl_deviceType type = CL_DEVICE_TYPE_DEFAULT, cl_vendor vendor = VENDOR_ANY);
-	OpenCLResource();					//cl_deviceType type = CL_DEVICE_TYPE_DEFAULT, cl_vendor vendor = VENDOR_ANY
-	OpenCLResource(cl_deviceType type); //cl_vendor vendor = VENDOR_ANY
-	OpenCLResource(cl_vendor vendor);   //cl_deviceType type = CL_DEVICE_TYPE_DEFAULT
+	// constructors
+	OpenCLResource();					// cl_deviceType type = CL_DEVICE_TYPE_DEFAULT, cl_vendor vendor = VENDOR_ANY
+	OpenCLResource(cl_deviceType type); // cl_vendor vendor = VENDOR_ANY
+	OpenCLResource(cl_vendor vendor);	// cl_deviceType type = CL_DEVICE_TYPE_DEFAULT
 	OpenCLResource(cl_deviceType type, cl_vendor vendor);
 	OpenCLResource(e_cl_device_type type, cl_vendor vendor);
 
-	//command line constructor, expects "--device gpu/cpu/accel" and/or "--vendor amd/intel/nvidia".  Defaults as above
+	// command line constructor, expects "--device gpu/cpu/accel" and/or "--vendor amd/intel/nvidia".  Defaults as above
 	OpenCLResource(int argc, char **argv);
-    //OpenCLResource(const std::vector<std::string> &);
-
-	OpenCLResource(unsigned int platformID, unsigned int deviceID);				 //specify the platform and optionally device by integer ID
-	OpenCLResource(unsigned int platformID, std::vector<unsigned int> deviceID); //specify the platform and optionally device by integer IDs. default uses all available devices on that platform.
-
-    ~OpenCLResource() {}
+	OpenCLResource(unsigned int platformID, unsigned int deviceID);				 // specify the platform and optionally device by integer ID
+	OpenCLResource(unsigned int platformID, std::vector<unsigned int> deviceID); // specify the platform and optionally device by integer IDs. default uses all available devices on that platform.
 
-	cl_int error; //use this for error checking in host program
+	cl_int error; // use this for error checking in host program
 
-	cl::Program getProgram() { return program; };								  //get this program, needed for creating kernel objects
-	cl::Context getContext() { return context; };								  //get this context, needed for creating memory objects
-	cl::CommandQueue getQueue(cl_uint deviceID = 0) { return queues[deviceID]; }; //get the command queue associated with device=deviceID from the list of devices available in the context
+	cl::Program getProgram() { return program; };								  // get this program, needed for creating kernel objects
+	cl::Context getContext() { return context; };								  // get this context, needed for creating memory objects
+	cl::CommandQueue getQueue(cl_uint deviceID = 0) { return queues[deviceID]; }; // get the command queue associated with device=deviceID from the list of devices available in the context
 
 	bool getDoubleSupport(cl_uint deviceID = 0) { return platform_info.device_info[deviceID].doubleSupport; };
 	cl_ulong getMaxMemAllocSize(cl_uint deviceID = 0) { return platform_info.device_info[deviceID].maxMemAllocSize; };
 	std::string getDeviceCLVersion(cl_uint deviceID = 0) { return platform_info.device_info[deviceID].version; };
 	cl_device_type getDeviceType(cl_uint deviceID = 0) { return platform_info.device_info[deviceID].devType; };
 
 	void buildProgramFromString(std::string clProgramString, std::string buildOptions = "");
 	void buildProgramFromSource(std::string filename, std::string buildOptions = "");
 
-	//TODO: add support for binary/offline compilation etc - from openCLUtilities
+	// TODO: add support for binary/offline compilation etc - from openCLUtilities
+	// void writeProgramBinary();
 
-	//prints the platform and device info related to this context
+	// prints the platform and device info related to this context
 	void print();
 };
 
-//basic functions to scan opencl platforms and devices of the system and print the results
-//TODO: query more/all platform and device properties
-//TODO: switch for verbosity of printOpenCL routines: name only, basics, all
-//TODO: other overloads for print opencl/platform/device? eg filters for vendor/type/...
+// basic functions to scan opencl platforms and devices of the system and print the results
+// TODO: query more/all platform and device properties
+// TODO: switch for verbosity of printOpenCL routines: name only, basics, all
+// TODO: other overloads for print opencl/platform/device? eg filters for vendor/type/...
 std::vector<platformInfo> queryOpenCL();
 platformInfo getPlatformInfo(cl::Platform platform, std::vector<cl::Device> devices = std::vector<cl::Device>());
 platformInfo getPlatformInfo(cl::Platform platform, cl::Device device);
 deviceInfo getDeviceInfo(cl::Device device);
 void printOpenCL();
 void printOpenCL(std::vector<platformInfo>);
 void printPlatformInfo(platformInfo pi);
 void printDeviceInfo(deviceInfo di);
 
-//convert OpenCL error enum to human readable string
+// convert OpenCL error enum to human readable string
 std::string CLErrorString(cl_int cl_error);
 
-//read file contents into a string
+// read file contents into a string
 std::string read_file(std::string filename);
+// void write_file(const std::string& filename, const std::string& content="");
 
 #endif // OPENCL_RESOURCE_HPP_
```

### Comparing `clode-0.7.1/clode/cpp/clODE_random.cl` & `clode-0.8.1/clode/cpp/clODE_random.cl`

 * *Files 14% similar despite different names*

```diff
@@ -10,107 +10,103 @@
 // seed with i=get_global_id[0]? or better to pass in more random seed?
 //=>make a rand_init kernel: hash global_id to create RNGstate array.
 // return final state back to a global array to continue stream if desired?
 
 //TODO: not clear how to make host code aware of rngstatetype. Only use 64bit int methods?
 // -> template rngData struct on realtype, rngstatetype. Pass N_RNGSTATE as compiler define to OpenCL? Store array of structs (not just rngData.state)
 
+
 #define XORSHIRO128_PLUS
 //~ #define XORSHIFT128_PLUS
 
-//Wrappers with fixed function signatures. Conditional compilation could be used to select the backend "next" function
 
 #ifdef XORSHIRO128_PLUS
 
-//TODO: this can be set as compiler flag to enable different RNG algorithms
 #define N_RNGSTATE (2)
-
 typedef ulong rngstatetype;
 #define RNGNORM RCONST(5.421010862427522e-20)
-// #if defined(CLODE_SINGLE_PRECISION)
-// 	#define RNGNORM (5.4210109e-20f) // 1.0/(2^64 - 1) single precision
-// #elif defined(CLODE_DOUBLE_PRECISION)
-// 	#define RNGNORM (5.421010862427522e-20) // 1.0/(2^64 - 1) double precision
-// #endif
 
 static inline ulong rotl(const ulong x, int k)
 {
 	return (x << k) | (x >> (64 - k));
 }
 
-ulong next(__private rngstatetype s[])
+static inline ulong next(__private rngstatetype s[])
 {
 	const ulong s0 = s[0];
 	ulong s1 = s[1];
 	const ulong result = s0 + s1;
 
 	s1 ^= s0;
 	s[0] = rotl(s0, 55) ^ s1 ^ (s1 << 14); // a, b
 	s[1] = rotl(s1, 36);				   // c
 
 	return result;
 }
 
-#endif
+#endif //XORSHIRO128_PLUS
+
+
 
 #ifdef XORSHIFT128_PLUS
 
 #define N_RNGSTATE (2)
-
 typedef ulong rngstatetype;
 #define RNGNORM RCONST(5.421010862427522e-20)
 
-ulong next(ulong s[])
+static inline ulong next(ulong s[])
 {
 	ulong s1 = s[0];
 	const ulong s0 = s[1];
 	const ulong result = s0 + s1;
 	s[0] = s0;
 	s1 ^= s1 << 23;							 // a
 	s[1] = s1 ^ s0 ^ (s1 >> 18) ^ (s0 >> 5); // b, c
 	return result;
 }
 
-#endif
+#endif //XORSHIFT128_PLUS
+
+
+// ---- Utilities ------
 
 //hold the RNG's state and other data in a struct
-typedef struct rngData
+struct rngData
 {
 	rngstatetype state[N_RNGSTATE];
 	bool randnUselast;
 	realtype randnLast;
-} rngData;
+};
 
 //return uniform pseudorandom number in [0,1)
-inline realtype rand(__private rngstatetype *state)
+static inline realtype rand(__private rngstatetype *state)
 {
 	rngstatetype result = next(state);
 	return result * RNGNORM;
 };
 
 //return normally distributed pseudorandom number N(0,1)
-//polar method, generates two at a time requiring  external storage of useLast switch and y2.... ugly! but no access to work-item private static vars..
-inline realtype randn(__private rngData *rd)
+static inline realtype randn(__private struct rngData *rd)
 {
 
 	realtype x1, x2, w, y1;
 
 	if (rd->randnUselast)
 	{
 		y1 = rd->randnLast;
 		rd->randnUselast = 0;
 	}
 	else
 	{
 		do
 		{
-			x1 = RCONST(2.0) * rand(rd->state) - RCONST(1.0);
-			x2 = RCONST(2.0) * rand(rd->state) - RCONST(1.0);
+			x1 = RCONST(2.0) * rand(rd->state) - ONE;
+			x2 = RCONST(2.0) * rand(rd->state) - ONE;
 			w = x1 * x1 + x2 * x2;
-		} while (w >= RCONST(1.0));
+		} while (w >= ONE);
 
 		w = sqrt((-RCONST(2.0) * log(w)) / w);
 		y1 = x1 * w;
 		rd->randnLast = x2 * w;
 		rd->randnUselast = 1;
 	}
```

### Comparing `clode-0.7.1/clode/cpp/clode_cpp_wrapper.pyi` & `clode-0.8.1/clode/cpp/clode_cpp_wrapper.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 CLODE C++/Python interface
 """
 from __future__ import annotations
 import typing
-__all__ = ['CLDeviceType', 'CLVendor', 'DEVICE_TYPE_ACCELERATOR', 'DEVICE_TYPE_ALL', 'DEVICE_TYPE_CPU', 'DEVICE_TYPE_CUSTOM', 'DEVICE_TYPE_DEFAULT', 'DEVICE_TYPE_GPU', 'DeviceInfo', 'FeatureSimulatorBase', 'LogLevel', 'LoggerSingleton', 'ObserverParams', 'OpenCLResource', 'PlatformInfo', 'ProblemInfo', 'SimulatorBase', 'SolverParams', 'TrajectorySimulatorBase', 'VENDOR_AMD', 'VENDOR_ANY', 'VENDOR_INTEL', 'VENDOR_NVIDIA', 'critical', 'debug', 'err', 'get_logger', 'info', 'off', 'print_opencl', 'query_opencl', 'trace', 'warn']
+__all__ = ['CLDeviceType', 'CLVendor', 'DEVICE_TYPE_ACCELERATOR', 'DEVICE_TYPE_ALL', 'DEVICE_TYPE_CPU', 'DEVICE_TYPE_CUSTOM', 'DEVICE_TYPE_DEFAULT', 'DEVICE_TYPE_GPU', 'DeviceInfo', 'FeatureSimulatorBase', 'LogLevel', 'LoggerSingleton', 'ObserverParams', 'OpenCLResource', 'PlatformInfo', 'ProblemInfo', 'SimulatorBase', 'SolverParams', 'TrajectorySimulatorBase', 'VENDOR_AMD', 'VENDOR_ANY', 'VENDOR_INTEL', 'VENDOR_NVIDIA', 'critical', 'debug', 'err', 'get_logger', 'info', 'off', 'query_opencl', 'trace', 'warn']
 class CLDeviceType:
     """
     Members:
     
       DEVICE_TYPE_ALL
     
       DEVICE_TYPE_CPU
@@ -17,20 +17,20 @@
       DEVICE_TYPE_ACCELERATOR
     
       DEVICE_TYPE_DEFAULT
     
       DEVICE_TYPE_CUSTOM
     """
     DEVICE_TYPE_ACCELERATOR: typing.ClassVar[CLDeviceType]  # value = <CLDeviceType.DEVICE_TYPE_ACCELERATOR: 8>
-    DEVICE_TYPE_ALL: typing.ClassVar[CLDeviceType]  # value = <CLDeviceType.DEVICE_TYPE_ALL: 4294967295>
+    DEVICE_TYPE_ALL: typing.ClassVar[CLDeviceType]  # value = <CLDeviceType.DEVICE_TYPE_ALL: -1>
     DEVICE_TYPE_CPU: typing.ClassVar[CLDeviceType]  # value = <CLDeviceType.DEVICE_TYPE_CPU: 2>
     DEVICE_TYPE_CUSTOM: typing.ClassVar[CLDeviceType]  # value = <CLDeviceType.DEVICE_TYPE_CUSTOM: 16>
     DEVICE_TYPE_DEFAULT: typing.ClassVar[CLDeviceType]  # value = <CLDeviceType.DEVICE_TYPE_DEFAULT: 1>
     DEVICE_TYPE_GPU: typing.ClassVar[CLDeviceType]  # value = <CLDeviceType.DEVICE_TYPE_GPU: 4>
-    __members__: typing.ClassVar[dict[str, CLDeviceType]]  # value = {'DEVICE_TYPE_ALL': <CLDeviceType.DEVICE_TYPE_ALL: 4294967295>, 'DEVICE_TYPE_CPU': <CLDeviceType.DEVICE_TYPE_CPU: 2>, 'DEVICE_TYPE_GPU': <CLDeviceType.DEVICE_TYPE_GPU: 4>, 'DEVICE_TYPE_ACCELERATOR': <CLDeviceType.DEVICE_TYPE_ACCELERATOR: 8>, 'DEVICE_TYPE_DEFAULT': <CLDeviceType.DEVICE_TYPE_DEFAULT: 1>, 'DEVICE_TYPE_CUSTOM': <CLDeviceType.DEVICE_TYPE_CUSTOM: 16>}
+    __members__: typing.ClassVar[dict[str, CLDeviceType]]  # value = {'DEVICE_TYPE_ALL': <CLDeviceType.DEVICE_TYPE_ALL: -1>, 'DEVICE_TYPE_CPU': <CLDeviceType.DEVICE_TYPE_CPU: 2>, 'DEVICE_TYPE_GPU': <CLDeviceType.DEVICE_TYPE_GPU: 4>, 'DEVICE_TYPE_ACCELERATOR': <CLDeviceType.DEVICE_TYPE_ACCELERATOR: 8>, 'DEVICE_TYPE_DEFAULT': <CLDeviceType.DEVICE_TYPE_DEFAULT: 1>, 'DEVICE_TYPE_CUSTOM': <CLDeviceType.DEVICE_TYPE_CUSTOM: 16>}
     def __eq__(self, other: typing.Any) -> bool:
         ...
     def __getstate__(self) -> int:
         ...
     def __hash__(self) -> int:
         ...
     def __index__(self) -> int:
@@ -111,15 +111,15 @@
     vendor: str
     version: str
     def __repr__(self) -> str:
         """
         Device info string representation
         """
 class FeatureSimulatorBase(SimulatorBase):
-    def __init__(self, arg0: ProblemInfo, arg1: str, arg2: str, arg3: bool, arg4: OpenCLResource, arg5: str) -> None:
+    def __init__(self, arg0: ProblemInfo, arg1: str, arg2: str, arg3: ObserverParams, arg4: bool, arg5: OpenCLResource, arg6: str) -> None:
         ...
     def __repr__(self) -> str:
         """
         CLODEfeatures string representation
         """
     def build_cl(self) -> None:
         ...
@@ -135,24 +135,22 @@
         ...
     def get_feature_names(self) -> list[str]:
         ...
     def get_n_features(self) -> int:
         ...
     def get_observer_name(self) -> str:
         ...
-    @typing.overload
-    def initialize(self, arg0: list[float], arg1: list[float], arg2: list[float], arg3: SolverParams) -> None:
-        """
-        Initialize FeatureSimulatorBase
-        """
-    @typing.overload
-    def initialize(self, arg0: list[float], arg1: list[float], arg2: list[float], arg3: SolverParams, arg4: ObserverParams) -> None:
-        """
-        Initialize FeatureSimulatorBase
-        """
+    def get_observer_params(self) -> ObserverParams:
+        ...
+    def initialize_observer(self) -> None:
+        ...
+    def is_observer_initialized(self) -> bool:
+        ...
+    def set_observer(self, arg0: str) -> None:
+        ...
     def set_observer_params(self, arg0: ObserverParams) -> None:
         ...
 class LogLevel:
     """
     Members:
     
       trace
@@ -207,18 +205,27 @@
     def get_log_level(self) -> LogLevel:
         ...
     def set_log_level(self, arg0: LogLevel) -> None:
         ...
     def set_log_pattern(self, arg0: str) -> None:
         ...
 class ObserverParams:
+    dx_down_threshold: float
+    dx_up_threshold: float
     e_var_ix: int
+    eps_dx: float
     f_var_ix: int
-    maxEventCount: int
-    def __init__(self, arg0: int, arg1: int, arg2: int, arg3: float, arg4: float, arg5: float, arg6: float, arg7: float, arg8: float, arg9: float, arg10: float) -> None:
+    max_event_count: int
+    max_event_timestamps: int
+    min_amp: float
+    min_imi: float
+    nhood_radius: float
+    x_down_threshold: float
+    x_up_threshold: float
+    def __init__(self, e_var_ix: int = 0, f_var_ix: int = 0, max_event_count: int = 100, max_event_timestamps: int = 0, min_amp: float = 0.0, min_imi: float = 0.0, nhood_radius: float = 0.05, x_up_threshold: float = 0.2, x_down_threshold: float = 0.2, dx_up_threshold: float = 0.0, dx_down_threshold: float = 0.0, eps_dx: float = 0.0) -> None:
         ...
     def __repr__(self) -> str:
         ...
 class OpenCLResource:
     @typing.overload
     def __init__(self) -> None:
         ...
@@ -264,15 +271,18 @@
     version: str
     def __repr__(self) -> str:
         """
         Platform info string representation
         """
 class ProblemInfo:
     aux: list[str]
+    num_aux: int
     num_noise: int
+    num_par: int
+    num_var: int
     pars: list[str]
     src_file: str
     vars: list[str]
     @typing.overload
     def __init__(self, src_file: str, vars: list[str], pars: list[str], aux: list[str] = [], num_noise: int = 1) -> None:
         ...
     @typing.overload
@@ -285,46 +295,58 @@
 class SimulatorBase:
     def __init__(self, problem_info: ProblemInfo, stepper: str, cl_single_precision: bool, opencl_resource: OpenCLResource, clode_root: str) -> None:
         ...
     def build_cl(self) -> None:
         ...
     def get_available_steppers(self) -> list[str]:
         ...
+    def get_pars(self) -> list[float]:
+        ...
     def get_problem_info(self) -> ProblemInfo:
         ...
     def get_program_string(self) -> str:
         ...
+    def get_solver_params(self) -> SolverParams:
+        ...
     def get_tspan(self) -> list[float]:
         ...
     def get_x0(self) -> list[float]:
         ...
     def get_xf(self) -> list[float]:
         ...
-    def initialize(self, tspan: list[float], x0: list[float], pars: list[float], solver_params: SolverParams) -> None:
-        """
-        Initialize CLODE
-        """
     def print_status(self) -> None:
         ...
     @typing.overload
-    def seed_rng(self, seed: int) -> None:
+    def seed_rng(self) -> None:
         """
         Seed RNG
         """
     @typing.overload
-    def seed_rng(self) -> None:
+    def seed_rng(self, seed: int) -> None:
         """
         Seed RNG
         """
+    @typing.overload
+    def set_opencl(self, arg0: OpenCLResource) -> None:
+        ...
+    @typing.overload
+    def set_opencl(self, arg0: int, arg1: int) -> None:
+        ...
     def set_pars(self, arg0: list[float]) -> None:
         ...
+    def set_precision(self, arg0: bool) -> None:
+        ...
     def set_problem_data(self, arg0: list[float], arg1: list[float]) -> None:
         ...
+    def set_problem_info(self, arg0: ProblemInfo) -> None:
+        ...
     def set_solver_params(self, arg0: SolverParams) -> None:
         ...
+    def set_stepper(self, arg0: str) -> None:
+        ...
     def set_tspan(self, arg0: list[float]) -> None:
         ...
     def set_x0(self, arg0: list[float]) -> None:
         ...
     def shift_tspan(self) -> None:
         ...
     def shift_x0(self) -> None:
@@ -356,34 +378,30 @@
         ...
     def get_n_stored(self) -> list[int]:
         ...
     def get_t(self) -> list[float]:
         ...
     def get_x(self) -> list[float]:
         ...
-    def initialize(self, arg0: list[float], arg1: list[float], arg2: list[float], arg3: SolverParams) -> None:
-        """
-        Initialize TrajectorySimulatorBase
-        """
     def trajectory(self) -> None:
         ...
-def get_logger() -> LoggerSingleton:
+def _print_opencl() -> None:
     """
-    Get logger singleton instance
+    Print OpenCL devices
     """
-def print_opencl() -> None:
+def get_logger() -> LoggerSingleton:
     """
-    Print OpenCL devices
+    Get logger singleton instance
     """
 def query_opencl() -> list[PlatformInfo]:
     """
     Query OpenCL devices
     """
 DEVICE_TYPE_ACCELERATOR: CLDeviceType  # value = <CLDeviceType.DEVICE_TYPE_ACCELERATOR: 8>
-DEVICE_TYPE_ALL: CLDeviceType  # value = <CLDeviceType.DEVICE_TYPE_ALL: 4294967295>
+DEVICE_TYPE_ALL: CLDeviceType  # value = <CLDeviceType.DEVICE_TYPE_ALL: -1>
 DEVICE_TYPE_CPU: CLDeviceType  # value = <CLDeviceType.DEVICE_TYPE_CPU: 2>
 DEVICE_TYPE_CUSTOM: CLDeviceType  # value = <CLDeviceType.DEVICE_TYPE_CUSTOM: 16>
 DEVICE_TYPE_DEFAULT: CLDeviceType  # value = <CLDeviceType.DEVICE_TYPE_DEFAULT: 1>
 DEVICE_TYPE_GPU: CLDeviceType  # value = <CLDeviceType.DEVICE_TYPE_GPU: 4>
 VENDOR_AMD: CLVendor  # value = <CLVendor.VENDOR_AMD: 2>
 VENDOR_ANY: CLVendor  # value = <CLVendor.VENDOR_ANY: 0>
 VENDOR_INTEL: CLVendor  # value = <CLVendor.VENDOR_INTEL: 3>
```

### Comparing `clode-0.7.1/clode/cpp/features.cl` & `clode-0.8.1/clode/cpp/features.cl`

 * *Files 6% similar despite different names*

```diff
@@ -11,78 +11,77 @@
 	__constant realtype *tspan,         //time vector [t0,tf] - adds (tf-t0) to these at the end
 	__global realtype *x0,              //initial state 				[nPts*nVar]
 	__constant realtype *pars,          //parameter values				[nPts*nPar]
 	__constant struct SolverParams *sp, //dtmin/max, tols, etc
 	__global realtype *xf,              //final state 				[nPts*nVar]
 	__global ulong *RNGstate,           //state for RNG					[nPts*nRNGstate]
     __global realtype *d_dt,            //array of dt values, one per solver
-	__global ObserverData *OData,		//for continue
+	__global ObserverData *OData,		//Observer data
 	__constant struct ObserverParams *opars,
 	__global realtype *F)
 {
 	int i = get_global_id(0);
 	int nPts = get_global_size(0);
 
 	realtype ti, dt;
     realtype p[N_PAR], xi[N_VAR], dxi[N_VAR];
     realtype auxi[N_AUX>0?N_AUX:1];
     realtype wi[N_WIENER>0?N_WIENER:1];
-	rngData rd;
+	struct rngData rd;
 
 	//get private copy of ODE parameters, initial data, and compute slope at initial state
 	ti = tspan[0];
-	dt = sp->dt;
+    dt = d_dt[i];
 
 	for (int j = 0; j < N_PAR; ++j)
 		p[j] = pars[j * nPts + i];
 
 	for (int j = 0; j < N_VAR; ++j)
 		xi[j] = x0[j * nPts + i];
 
 	for (int j = 0; j < N_RNGSTATE; ++j)
 		rd.state[j] = RNGstate[j * nPts + i];
 
-	rd.randnUselast = 0;
+	ObserverData odata = OData[i]; 
 
+    // generate random numbers if needed
+    rd.randnUselast = 0;
     for (int j = 0; j < N_WIENER; ++j)
 #ifdef STOCHASTIC_STEPPER
         wi[j] = randn(&rd) / sqrt(dt);
 #else
-        wi[j] = RCONST(0.0);
+        wi[j] = ZERO;
 #endif
-	getRHS(ti, xi, p, dxi, auxi, wi); //slope at initial point, needed for FSAL steppers (bs23, dorpri5)
 
-	ObserverData odata = OData[i]; //private copy of observer data
+    //get the slope and aux at initial point
+    getRHS(ti, xi, p, dxi, auxi, wi); 
 
-	//time-stepping loop, main time interval
-    int step = 0;
+	//time-stepping loop
+    unsigned int step = 0;
     int stepflag = 0;
 	bool eventOccurred;
 	bool terminalEvent;
-	while (ti < tspan[1] && step < sp->max_steps)
+	while (ti <= tspan[1] && step < sp->max_steps)
 	{
 		++step;
-		//++odata.stepcount; //do this in updateObserverData always
         stepflag = stepper(&ti, xi, dxi, p, sp, &dt, tspan, auxi, wi, &rd);
         // if (stepflag!=0)
             // break;
 
-		//TODO: Update solution buffers here?
+		updateObserverData(&ti, xi, dxi, auxi, &odata, opars); 
 
 		eventOccurred = eventFunction(&ti, xi, dxi, auxi, &odata, opars);
 		if (eventOccurred)
 		{
+			// record current state into dedicated event buffers (same pattern as trajectory)
+
 			terminalEvent = computeEventFeatures(&ti, xi, dxi, auxi, &odata, opars);
 			if (terminalEvent)
-			{
 				break;
-			};
 		}
-
-		updateObserverData(&ti, xi, dxi, auxi, &odata, opars); 
 	}
 
 	//readout features of interest and write to global F:
 	finalizeFeatures(&ti, xi, dxi, auxi, &odata, opars, F, i, nPts);
 
 	//finalize observerdata for possible continuation
 	finalizeObserverData(&ti, xi, dxi, auxi, &odata, opars, tspan);
@@ -95,9 +94,9 @@
 		xf[j * nPts + i] = xi[j];
 
     // To get same RNG on repeat (non-continued) run, need to set the seed to same value
 	for (int j = 0; j < N_RNGSTATE; ++j)
 		RNGstate[j * nPts + i] = rd.state[j];
 
     // update dt to its final value (for adaptive stepper continue)
-    // d_dt[i] = dt;
+    d_dt[i] = dt;
 }
```

### Comparing `clode-0.7.1/clode/cpp/initializeObserver.cl` & `clode-0.8.1/clode/cpp/initializeObserver.cl`

 * *Files 9% similar despite different names*

```diff
@@ -19,56 +19,64 @@
 	int i = get_global_id(0);
 	int nPts = get_global_size(0);
 
 	realtype ti, dt;
     realtype p[N_PAR], xi[N_VAR], dxi[N_VAR];
     realtype auxi[N_AUX>0?N_AUX:1];
     realtype wi[N_WIENER>0?N_WIENER:1];
-	rngData rd;
+	struct rngData rd;
 
 	//get private copy of ODE parameters, initial data, and compute slope at initial state
 	ti = tspan[0];
-	dt = sp->dt;
+    dt = d_dt[i];
 
 	for (int j = 0; j < N_PAR; ++j)
 		p[j] = pars[j * nPts + i];
 
 	for (int j = 0; j < N_VAR; ++j)
 		xi[j] = x0[j * nPts + i];
 
 	for (int j = 0; j < N_RNGSTATE; ++j)
 		rd.state[j] = RNGstate[j * nPts + i];
 
-	rd.randnUselast = 0;
+	ObserverData odata = OData[i];
 
+    // generate random numbers if needed
+    rd.randnUselast = 0;
     for (int j = 0; j < N_WIENER; ++j)
 #ifdef STOCHASTIC_STEPPER
         wi[j] = randn(&rd) / sqrt(dt);
 #else
-        wi[j] = RCONST(0.0);
+        wi[j] = ZERO;
 #endif
-	getRHS(ti, xi, p, dxi, auxi, wi); //slope at initial point, needed for FSAL
 
-	ObserverData odata = OData[i]; //private copy of observer data
+    //get the slope and aux at initial point
+    getRHS(ti, xi, p, dxi, auxi, wi); 
 
 	initializeObserverData(&ti, xi, dxi, auxi, &odata, opars);
 
 #ifdef TWO_PASS_EVENT_DETECTOR
 
-    int step = 0;
+	//time-stepping loop
+    unsigned int step = 0;
     int stepflag = 0;
 	while (ti < tspan[1] && step < sp->max_steps)
 	{
 		++step;
         stepflag = stepper(&ti, xi, dxi, p, sp, &dt, tspan, auxi, wi, &rd);
         // if (stepflag!=0)
         //     break;
 
 		warmupObserverData(&ti, xi, dxi, auxi, &odata, opars);
 	}
+	//rewind the time and state so initializeEventDetector gets the right values
+	ti = tspan[0];
+	for (int j = 0; j < N_VAR; ++j)
+		xi[j] = x0[j * nPts + i];
+	getRHS(ti, xi, p, dxi, auxi, wi);
 
 #endif //TWO_PASS_EVENT_DETECTOR
 
 	initializeEventDetector(&ti, xi, dxi, auxi, &odata, opars);
 
 	//update the global ObserverData array
 	OData[i] = odata;
```

### Comparing `clode-0.7.1/clode/cpp/logging/MatlabSink.hpp` & `clode-0.8.1/clode/cpp/logging/MatlabSink.hpp`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/clode/cpp/logging/PythonSink.hpp` & `clode-0.8.1/clode/cpp/logging/PythonSink.hpp`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/clode/cpp/observers/BUILD` & `clode-0.8.1/clode/cpp/observers/BUILD`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/clode/cpp/observers/observer_basic.clh` & `clode-0.8.1/clode/cpp/observers/observer_basic.clh`

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,94 @@
 
 
 #ifndef OBSERVER_BASIC_H
 #define OBSERVER_BASIC_H
 
-
 #ifdef __cplusplus
-template <typename realtype>
+//Collect all the info for this observer
+static struct ObserverInfo getObserverInfo_basic(const ProblemInfo pi, const unsigned int fVarIx, const unsigned int eVarIx, const unsigned int nStoredEvents) {
+    struct ObserverInfo oi;
+    oi.define="USE_OBSERVER_BASIC";
+    oi.observerDataSizeFloat = 7*sizeof(cl_float) + sizeof(cl_uint);
+    oi.observerDataSizeDouble = 7*sizeof(cl_double) + sizeof(cl_uint); 
+    std::string varName=pi.varNames[fVarIx];
+    oi.featureNames={"max "+varName, "min "+varName, "mean "+varName, "max d"+varName+"/dt", "min d"+varName+"/dt", "step count"};
+    return oi;
+}
 #endif
+
+#ifdef USE_OBSERVER_BASIC
+
 struct ObserverData_basic
 {
     realtype xTrajectoryMax;
     realtype xTrajectoryMin;
     realtype xTrajectoryMean;
     realtype dxTrajectoryMax;
     realtype dxTrajectoryMin;
-    unsigned int eventcount;
+    realtype t_last;
+    realtype t_start;
     unsigned int stepcount;
 };
-
-#ifdef __cplusplus
-//Collect all the info for this observer. Must be a static function when defining function in header, otherwise defined for each time included.
-static ObserverInfo getObserverInfo_basic(const ProblemInfo pi, const int fVarIx, const int eVarIx)
-{
-    ObserverInfo oi;
-    oi.define="USE_OBSERVER_BASIC";
-    oi.observerDataSizeFloat=sizeof(ObserverData_basic<float>);
-    oi.observerDataSizeDouble=sizeof(ObserverData_basic<double>);
-    std::string varName=pi.varNames[fVarIx];
-    oi.featureNames={"max "+varName, "min "+varName, "mean "+varName, "max d"+varName+"/dt", "min d"+varName+"/dt", "step count"};
-    return oi;
-}
-#endif
-
-#ifdef USE_OBSERVER_BASIC
-
 typedef struct ObserverData_basic ObserverData;
 
-inline void initializeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void initializeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     od->xTrajectoryMax = -BIG_REAL;
     od->xTrajectoryMin = BIG_REAL;
-    od->xTrajectoryMean = RCONST(0.0);
+    od->xTrajectoryMean = ZERO;
     od->dxTrajectoryMax = -BIG_REAL;
     od->dxTrajectoryMin = BIG_REAL;
-    od->eventcount = 0;
+    od->t_last = *ti;
+    od->t_start = *ti;
     od->stepcount = 0;
 }
 //nothing to do - One pass detector
-inline void warmupObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void warmupObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
 }
 
 //no events
-inline void initializeEventDetector(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void initializeEventDetector(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
 }
 
 //no events
-inline bool eventFunction(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline bool eventFunction(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     return false;
 }
 
 //no events
-inline bool computeEventFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline bool computeEventFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     return false;
 }
 
 //all features are per-timestep (eventOccurred unused)
-inline void updateObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void updateObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     ++od->stepcount;
+    realtype dt = *ti - od->t_last;
+    od->t_last = *ti;
+    realtype elapsedTime = *ti - od->t_start;
     od->xTrajectoryMax = fmax(xi[op->fVarIx], od->xTrajectoryMax);
     od->xTrajectoryMin = fmin(xi[op->fVarIx], od->xTrajectoryMin);
-    runningMean(&od->xTrajectoryMean, xi[op->fVarIx], od->stepcount);
+    od->xTrajectoryMean = runningMeanTime(od->xTrajectoryMean, xi[op->fVarIx], dt, elapsedTime);
     od->dxTrajectoryMax = fmax(dxi[op->fVarIx], od->dxTrajectoryMax);
     od->dxTrajectoryMin = fmin(dxi[op->fVarIx], od->dxTrajectoryMin);
 }
 
 
-inline void finalizeFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __global realtype *F, const int i, const int nPts)
-{
+static inline void finalizeFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __global realtype *F, const int i, const int nPts) {
     int ix = 0;
     F[ix++ * nPts + i] = od->xTrajectoryMax;
     F[ix++ * nPts + i] = od->xTrajectoryMin;
     F[ix++ * nPts + i] = od->xTrajectoryMean;
     F[ix++ * nPts + i] = od->dxTrajectoryMax;
     F[ix++ * nPts + i] = od->dxTrajectoryMin;
     F[ix++ * nPts + i] = od->stepcount;
 }
 
 //Perform and post-integration cleanup of observer data to ensure it is ready for continuation if needed
-inline void finalizeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __constant realtype *tspan)
-{
-    //nothing to do
+static inline void finalizeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __constant realtype *tspan) {
+    realtype T = *ti - tspan[0];
+    od->t_start -= T;
 }
 
 #endif // USE_OBSERVER_BASIC
 
 #endif // OBSERVER_BASIC_H
```

### Comparing `clode-0.7.1/clode/cpp/observers/observer_basic_allVar.clh` & `clode-0.8.1/clode/cpp/observers/observer_basic_allVar.clh`

 * *Files 5% similar despite different names*

```diff
@@ -1,143 +1,134 @@
 
 
 #ifndef OBSERVER_BASIC_ALLVAR_H
 #define OBSERVER_BASIC_ALLVAR_H
 
 #ifdef __cplusplus
-//Collect all the info for this observer. Must be a static function when defining function in header, otherwise defined for each time included.
-static ObserverInfo getObserverInfo_basicAll(const ProblemInfo pi, const int fVarIx, const int eVarIx)
-{
-    ObserverInfo oi;
+//Collect all the info for this observer
+static struct ObserverInfo getObserverInfo_basicAll(const ProblemInfo pi, const unsigned int fVarIx, const unsigned int eVarIx, const unsigned int nStoredEvents) {
+    struct ObserverInfo oi;
     oi.define = "USE_OBSERVER_BASIC_ALLVAR";
-    size_t n_real = (5*pi.nVar + 3*pi.nAux); //hard coded, because C++ code can't see the N_VAR, N_AUX etc...
-    size_t n_int = 2;
+    size_t n_real = (5*pi.nVar + 3*pi.nAux + 2); //hard coded, because C++ code can't see the N_VAR, N_AUX etc...
+    size_t n_int = 1;
     oi.observerDataSizeFloat = n_real*sizeof(cl_float) + n_int*sizeof(cl_uint);
     oi.observerDataSizeDouble = n_real*sizeof(cl_double) + n_int*sizeof(cl_uint); 
-    for (int j = 0; j < pi.nVar; ++j)
-    {
+    for (int j = 0; j < pi.nVar; ++j) {
         oi.featureNames.push_back("max " + pi.varNames[j]);
         oi.featureNames.push_back("min " + pi.varNames[j]);
         oi.featureNames.push_back("mean " + pi.varNames[j]);
         oi.featureNames.push_back("max d" + pi.varNames[j] + "/dt");
         oi.featureNames.push_back("min d" + pi.varNames[j] + "/dt");
     }
-    for (int j = 0; j < pi.nAux; ++j)
-    {
+    for (int j = 0; j < pi.nAux; ++j) {
         oi.featureNames.push_back("max " + pi.auxNames[j]);
         oi.featureNames.push_back("min " + pi.auxNames[j]);
         oi.featureNames.push_back("mean " + pi.auxNames[j]);
     }
     oi.featureNames.push_back("step count");
     return oi;
 }
 #endif
 
 
 #ifdef USE_OBSERVER_BASIC_ALLVAR
 
-typedef struct ObserverData_basicAll
+struct ObserverData_basicAll
 {
     realtype xTrajectoryMax[N_VAR];
     realtype xTrajectoryMin[N_VAR];
     realtype xTrajectoryMean[N_VAR];
     realtype dxTrajectoryMax[N_VAR];
     realtype dxTrajectoryMin[N_VAR];
     realtype auxTrajectoryMax[N_AUX];
     realtype auxTrajectoryMin[N_AUX];
     realtype auxTrajectoryMean[N_AUX];
-    unsigned int eventcount;
+    realtype t_last;
+    realtype t_start;
     unsigned int stepcount;
-} ObserverData;
+};
 
-inline void initializeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
-    for (int j = 0; j < N_VAR; ++j)
-    {
+typedef struct ObserverData_basicAll ObserverData;
+
+static inline void initializeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
+    for (int j = 0; j < N_VAR; ++j) {
         od->xTrajectoryMax[j] = -BIG_REAL;
         od->xTrajectoryMin[j] = BIG_REAL;
-        od->xTrajectoryMean[j] = RCONST(0.0);
+        od->xTrajectoryMean[j] = ZERO;
         od->dxTrajectoryMax[j] = -BIG_REAL;
         od->dxTrajectoryMin[j] = BIG_REAL;
     }
-    for (int j = 0; j < N_AUX; ++j)
-    {
+    for (int j = 0; j < N_AUX; ++j) {
         od->auxTrajectoryMax[j] = -BIG_REAL;
         od->auxTrajectoryMin[j] = BIG_REAL;
-        od->auxTrajectoryMean[j] = RCONST(0.0);
+        od->auxTrajectoryMean[j] = ZERO;
     }
-    od->eventcount = 0;
+    od->t_last = *ti;
+    od->t_start = *ti;
     od->stepcount = 0;
 }
 
 //nothing to do - One pass detector
-inline void warmupObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void warmupObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
 }
 
 //no events
-inline void initializeEventDetector(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void initializeEventDetector(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
 }
 
 //no events
-inline bool eventFunction(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline bool eventFunction(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     return false;
 }
 
 //no events
-inline bool computeEventFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline bool computeEventFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     return false;
 }
 
 //all features are per-timestep (eventOccurred unused)
-inline void updateObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void updateObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     ++od->stepcount;
-    for (int j = 0; j < N_VAR; ++j)
-    {
+    realtype dt = *ti - od->t_last;
+    od->t_last = *ti;
+    realtype elapsedTime = *ti - od->t_start;
+    for (int j = 0; j < N_VAR; ++j) {
         od->xTrajectoryMax[j] = fmax(xi[j], od->xTrajectoryMax[j]);
         od->xTrajectoryMin[j] = fmin(xi[j], od->xTrajectoryMin[j]);
-        runningMean(&od->xTrajectoryMean[j], xi[j], od->stepcount);
+        od->xTrajectoryMean[j] = runningMeanTime(od->xTrajectoryMean[j], xi[j], dt, elapsedTime);
         od->dxTrajectoryMax[j] = fmax(dxi[j], od->dxTrajectoryMax[j]);
         od->dxTrajectoryMin[j] = fmin(dxi[j], od->dxTrajectoryMin[j]);
     }
-    for (int j = 0; j < N_AUX; ++j)
-    {
+    for (int j = 0; j < N_AUX; ++j) {
         od->auxTrajectoryMax[j] = fmax(auxi[j], od->auxTrajectoryMax[j]);
         od->auxTrajectoryMin[j] = fmin(auxi[j], od->auxTrajectoryMin[j]);
-        runningMean(&od->auxTrajectoryMean[j], auxi[j], od->stepcount);
+        od->auxTrajectoryMean[j] = runningMeanTime(od->auxTrajectoryMean[j], auxi[j], dt, elapsedTime);
     }
 }
 
 
-inline void finalizeFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __global realtype *F, int i, int nPts)
-{
+static inline void finalizeFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __global realtype *F, int i, int nPts) {
     int ix = 0;
-    for (int j = 0; j < N_VAR; ++j)
-    {
+    for (int j = 0; j < N_VAR; ++j) {
         F[ix++ * nPts + i] = od->xTrajectoryMax[j];
         F[ix++ * nPts + i] = od->xTrajectoryMin[j];
         F[ix++ * nPts + i] = od->xTrajectoryMean[j];
         F[ix++ * nPts + i] = od->dxTrajectoryMax[j];
         F[ix++ * nPts + i] = od->dxTrajectoryMin[j];
     }
-    for (int j = 0; j < N_AUX; ++j)
-    {
+    for (int j = 0; j < N_AUX; ++j) {
         F[ix++ * nPts + i] = od->auxTrajectoryMax[j];
         F[ix++ * nPts + i] = od->auxTrajectoryMin[j];
         F[ix++ * nPts + i] = od->auxTrajectoryMean[j];
     }
     F[ix++ * nPts + i] = od->stepcount;
 }
 
 //Perform and post-integration cleanup of observer data to ensure it is ready for continuation if needed
-inline void finalizeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __constant realtype *tspan)
-{
-    //nothing to do
+static inline void finalizeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __constant realtype *tspan) {
+    realtype T = *ti - tspan[0];
+    od->t_start -= T;
 }
 
 #endif // USE_OBSERVER_BASIC_ALLVAR
 
 #endif // OBSERVER_BASIC_ALLVAR_H
```

### Comparing `clode-0.7.1/clode/cpp/observers/observer_local_maximum.clh` & `clode-0.8.1/clode/cpp/observers/observer_local_maximum.clh`

 * *Files 25% similar despite different names*

```diff
@@ -1,280 +1,332 @@
 //Event is the detection of local max in specified variable fVarIx
 
 #ifndef OBSERVER_LOCAL_MAX_H
 #define OBSERVER_LOCAL_MAX_H
 
+
 #ifdef __cplusplus
-template <typename realtype>
+//Collect all the info for this observer
+static struct ObserverInfo getObserverInfo_localmax(const ProblemInfo pi, const unsigned int fVarIx, const unsigned int eVarIx, const unsigned int nStoredEvents) {
+    struct ObserverInfo oi;
+    oi.define="USE_OBSERVER_LOCAL_MAX";
+    size_t n_real=(3*pi.nVar*2 + pi.nVar*5 + pi.nAux*3 + nStoredEvents*4 + 3*3 + 4); //hard coded, because C++ code can't see the N_VAR, N_AUX etc...
+    size_t n_int=2;
+    oi.observerDataSizeFloat=n_real*sizeof(cl_float) + n_int*sizeof(cl_uint);
+    oi.observerDataSizeDouble=n_real*sizeof(cl_double) + n_int*sizeof(cl_uint); 
+
+    std::string fVarName=pi.varNames[fVarIx];
+
+    oi.featureNames.push_back("max IMI");
+    oi.featureNames.push_back("min IMI");
+    oi.featureNames.push_back("mean IMI");
+    oi.featureNames.push_back("max amplitude");
+    oi.featureNames.push_back("min amplitude");
+    oi.featureNames.push_back("mean amplitude");
+    
+    for (int j = 0; j < pi.nVar; ++j) {
+        oi.featureNames.push_back("max " + pi.varNames[j]);
+        oi.featureNames.push_back("min " + pi.varNames[j]);
+        oi.featureNames.push_back("mean " + pi.varNames[j]);
+        oi.featureNames.push_back("max d" + pi.varNames[j] + "/dt");
+        oi.featureNames.push_back("min d" + pi.varNames[j] + "/dt");
+    }
+    for (int j = 0; j < pi.nAux; ++j) {
+        oi.featureNames.push_back("max " + pi.auxNames[j]);
+        oi.featureNames.push_back("min " + pi.auxNames[j]);
+        oi.featureNames.push_back("mean " + pi.auxNames[j]);
+    }
+    for (int j = 0; j < nStoredEvents; ++j) {
+        oi.featureNames.push_back("localmax event time " + std::to_string(j));
+        oi.featureNames.push_back("localmax event evar " + std::to_string(j));
+        oi.featureNames.push_back("localmin event time " + std::to_string(j));
+        oi.featureNames.push_back("localmin event evar " + std::to_string(j));
+    }
+    oi.featureNames.push_back("event count");
+    oi.featureNames.push_back("step count");
+    return oi;
+}
 #endif
+
+
+#ifdef USE_OBSERVER_LOCAL_MAX
+//events are triggered at local maxima in the variable specified by op.fVarIx
+
 struct ObserverData_localmax
 {
-    // realtype nDistinctEvents[N_DISTINCT_MAX];
-
     realtype tbuffer[3];
-    realtype xbuffer[3];
-    realtype dxbuffer[3];
+    realtype xbuffer[3 * N_VAR]; // just keep fVar? conceptually simplest
+    realtype dxbuffer[3 * N_VAR];
 
+    realtype xTrajectoryMax[N_VAR];
+    realtype xTrajectoryMin[N_VAR];
+    realtype xTrajectoryMean[N_VAR];
+    realtype dxTrajectoryMax[N_VAR];
+    realtype dxTrajectoryMin[N_VAR];
+
+    realtype auxTrajectoryMax[N_AUX];
+    realtype auxTrajectoryMin[N_AUX];
+    realtype auxTrajectoryMean[N_AUX];
+
+    realtype tMaxList[N_STORE_EVENTS];
+    realtype xMaxList[N_STORE_EVENTS];
+    realtype tMinList[N_STORE_EVENTS];
+    realtype xMinList[N_STORE_EVENTS];
+    
     realtype IMI[3]; //max/min/mean
     realtype amp[3]; //max/min/mean
-    // realtype tMaxMin[3]; //max/min/mean
-    // realtype xMax[3]; //max/min/mean
-    // realtype xMin[3]; //max/min/mean
 
+    realtype t_start;
     realtype tLastMax;
+    //realtype xLastMax;
     realtype tLastMin;
     realtype xLastMin;
 
-    realtype xTrajectoryMean;
-    realtype xGlobalMax;
-    realtype xGlobalMin;
-    realtype dxGlobalMax;
-    realtype dxGlobalMin;
-
     unsigned int eventcount;
     unsigned int stepcount;
 
 };
 
-#ifdef __cplusplus
-//Collect all the info for this observer. Must be a static function when defining function in header, otherwise defined for each time included.
-static ObserverInfo getObserverInfo_localmax(const ProblemInfo pi, const int fVarIx, const int eVarIx)
-{
-    ObserverInfo oi;
-    oi.define="USE_OBSERVER_LOCAL_MAX";
-    oi.observerDataSizeFloat=sizeof(ObserverData_localmax<float>);
-    oi.observerDataSizeDouble=sizeof(ObserverData_localmax<double>);
-    std::string varName=pi.varNames[fVarIx];
-    oi.featureNames={
-        "max IMI",
-        "min IMI",
-        "mean IMI",
-        "max amplitude",
-        "min amplitude",
-        "mean amplitude",
-        "max " + varName,
-        "min " + varName,
-        "mean " + varName,
-        "max d" + varName + "/dt",
-        "min d" + varName + "/dt",
-        "event count",
-        "step count",
-    };
-    return oi;
-}
-#endif
-
-
-#ifdef USE_OBSERVER_LOCAL_MAX
-//events are triggered at local maxima in the variable specified by op.fVarIx
-
 typedef struct ObserverData_localmax ObserverData;
 
 //set initial values to relevant fields in ObserverData
-inline void initializeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
-
+static inline void initializeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     od->tbuffer[2] = *ti;
-    od->xbuffer[2] = xi[op->fVarIx];
-    od->dxbuffer[2] = dxi[op->fVarIx];
+    for (int j = 0; j < N_VAR; ++j) {
+        od->xbuffer[j * 3 + 2] = xi[j];
+        od->dxbuffer[j * 3 + 2] = dxi[j];
+    }
+
+    for (int j = 0; j < N_VAR; ++j) {
+        od->xTrajectoryMax[j] = -BIG_REAL;
+        od->xTrajectoryMin[j] = BIG_REAL;
+        od->xTrajectoryMean[j] = ZERO; 
+        od->dxTrajectoryMax[j] = -BIG_REAL;
+        od->dxTrajectoryMin[j] = BIG_REAL;
+    }
+    for (int j = 0; j < N_AUX; ++j) {
+        od->auxTrajectoryMax[j] = -BIG_REAL;
+        od->auxTrajectoryMin[j] = BIG_REAL;
+        od->auxTrajectoryMean[j] = ZERO;
+    }
+
+    for (int j = 0; j < N_STORE_EVENTS; ++j) {
+		od->tMaxList[j] = ZERO;
+		od->xMaxList[j] = ZERO;
+		od->tMinList[j] = ZERO;
+		od->xMinList[j] = ZERO;
+	}
 
     od->IMI[0] = -BIG_REAL;
     od->IMI[1] = BIG_REAL;
-    od->IMI[2] = RCONST(0.0);
+    od->IMI[2] = ZERO;
 
     od->amp[0] = -BIG_REAL;
     od->amp[1] = BIG_REAL;
-    od->amp[2] = RCONST(0.0);
-
-    //od->tMaxMin[0]=-BIG_REAL;
-    //od->tMaxMin[1]= BIG_REAL;
-    //od->tMaxMin[2]= RCONST(0.0);
-
-    // od->xMax[0] = -BIG_REAL;
-    // od->xMax[1] = BIG_REAL;
-    // od->xMax[2] = RCONST(0.0);
-
-    // od->xMin[0] = -BIG_REAL;
-    // od->xMin[1] = BIG_REAL;
-    // od->xMin[2] = RCONST(0.0);
+    od->amp[2] = ZERO;
 
-    od->tLastMax = RCONST(0.0);
+    od->t_start = *ti;
+    od->tLastMax = ZERO;
+    od->tLastMin = ZERO;
     od->xLastMin = BIG_REAL;
-    od->tLastMin = RCONST(0.0);
-
-    od->xTrajectoryMean = RCONST(0.0);
-    od->xGlobalMax = -BIG_REAL;
-    od->xGlobalMin = BIG_REAL;
-    od->dxGlobalMax = -BIG_REAL;
-    od->dxGlobalMin = BIG_REAL;
 
     od->eventcount = 0;
     od->stepcount = 0;
 }
 
 //no warmup needed
-inline void warmupObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void warmupObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
 }
 
 //process warmup data to compute relevant event detector quantities (e.g. thresholds)
-inline void initializeEventDetector(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void initializeEventDetector(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
 }
 
 //check buffer of slopes for local max
-inline bool eventFunction(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline bool eventFunction(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
+
     if (od->stepcount < 2)
         return false;
 
     // Event is a local maximum
-    return (od->dxbuffer[1] >= 0.0 && od->dxbuffer[2] < 0.0);
+    return (od->dxbuffer[op->fVarIx * 3 + 1] > 0.0 && od->dxbuffer[op->fVarIx * 3 + 2] < 0.0);
 }
 
 //When an event is detected, computes desired event-based features. returns true if a terminal event was reached
 // - get (t,x) at local max, compute: IMI, tMaxMin, amp
-inline bool computeEventFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
-    ++od->eventcount;
-
+static inline bool computeEventFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
+    
     //Simple Max of xbuffer
     realtype thisXbuffer[3];
     for (int j = 0; j < 3; ++j)
-     	thisXbuffer[j] = od->xbuffer[j];
+     	thisXbuffer[j] = od->xbuffer[op->fVarIx * 3 + j];
 
-    int ix;
-    realtype xThisMax;
-    maxOfArray(thisXbuffer, 3, &xThisMax, &ix);
+    int ix = array_argmax(thisXbuffer, 3);
     realtype tThisMax = od->tbuffer[ix];
+    realtype xThisMax = thisXbuffer[ix];
 
-    //Quadratic interpolation for improved accuracy BROKEN??
+    //Quadratic interpolation for improved accuracy.. broken?
     //quadraticInterpVertex(od->tbuffer, od->xbuffer, &tThisMax, &xThisMax);
 
-    if (od->eventcount > 1)
-    { //implies tLastMax, tLastMin and xLastMin are set
-    
-        // od->xMax[0] = fmax(xThisMax, od->xMax[0]);
-        // od->xMax[1] = fmin(xThisMax, od->xMax[1]);
-        // runningMean(&od->xMax[2], xThisMax, od->eventcount - 1);
-
-        // od->xMin[0] = fmax(od->xLastMin, od->xMin[0]); //must have had two maxima to have found one minimum
-        // od->xMin[1] = fmin(od->xLastMin, od->xMin[1]);
-        // runningMean(&od->xMin[2], od->xLastMin, od->eventcount - 1);
+
+    ++od->eventcount;
+
+    if (od->eventcount > 1) { //implies tLastMax, tLastMin and xLastMin are set
 
         //max/min/mean IMI
         realtype thisIMI = tThisMax - od->tLastMax;
         //if(thisIMI > op->minIMI) {
         od->IMI[0] = fmax(thisIMI, od->IMI[0]);
         od->IMI[1] = fmin(thisIMI, od->IMI[1]);
         runningMean(&od->IMI[2], thisIMI, od->eventcount - 1);
         //}
 
-        //max/min/mean tMaxMin
-        //realtype thisTMaxMin=tThisMax-od->tLastMin;
-        //od->tMaxMin[0]=fmax(thisTMaxMin, od->tMaxMin[0]);
-        //od->tMaxMin[1]=fmin(thisTMaxMin, od->tMaxMin[1]);
-        //runningMean(&od->tMaxMin[2],thisTMaxMin,od->eventcount-1);
-
         //max/min/mean amp
         realtype thisAmp = xThisMax - od->xLastMin;
+        //if(thisAmp > op->minXamp) {
         od->amp[0] = fmax(thisAmp, od->amp[0]);
         od->amp[1] = fmin(thisAmp, od->amp[1]);
         runningMean(&od->amp[2], thisAmp, od->eventcount - 1);
+        //}
     }
 
     //update stored "last" values
     od->tLastMax = tThisMax;
-    od->xLastMin = xi[op->fVarIx];
+    // od->xLastMax = xThisMax;
 
-    if (od->eventcount >= op->maxEventCount){
-        return true;
+	if (od->eventcount <= N_STORE_EVENTS){
+        od->tMaxList[od->eventcount-1] = tThisMax;
+        od->xMaxList[od->eventcount-1] = xThisMax;
     }
+
+    if (od->eventcount == op->maxEventCount)
+        return true;
+
     return false; //not terminal
 }
 
 //full per-timestep update of observer data. If an event occurred this timestep, event-based observer data is reset. Per-timestep features are computed here.
 // - advance solution/slope buffers
 // - check for any intermediate special points & store their info
 // - reset intermediates upon local max event detection
-inline void updateObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void updateObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     ++od->stepcount;
-    //advance solution buffer
-    for (int i = 0; i < 2; ++i)
-    {
-        od->tbuffer[i] = od->tbuffer[i + 1];
-        od->xbuffer[i] = od->xbuffer[i + 1];
-        od->dxbuffer[i] = od->dxbuffer[i + 1];
-    }
+
+    // advance solution buffer
+    od->tbuffer[0] = od->tbuffer[1];
+    od->tbuffer[1] = od->tbuffer[2];
     od->tbuffer[2] = *ti;
-    od->xbuffer[2] = xi[op->fVarIx]; // forces fVarIx=eVarIx
-    od->dxbuffer[2] = dxi[op->fVarIx];
 
-    //global dxMax, dxMin
-    od->xGlobalMax = fmax(od->xGlobalMax, xi[op->fVarIx]);
-    od->xGlobalMin = fmin(od->xGlobalMin, xi[op->fVarIx]);
-    od->dxGlobalMax = fmax(od->dxGlobalMax, dxi[op->fVarIx]);
-    od->dxGlobalMin = fmin(od->dxGlobalMin, dxi[op->fVarIx]);
-    runningMean(&od->xTrajectoryMean, xi[op->fVarIx], od->stepcount);
-
-    if (od->stepcount > 1)
-    {
-        //local min check - one between each max - simply overwrite tLastMin, xLastMin
-        if (od->dxbuffer[1] <= 0.0 && od->dxbuffer[2] > 0.0)
-        {
-            realtype thisXbuffer[3];
-            for (int j = 0; j < 3; ++j)
-                thisXbuffer[j] = od->xbuffer[j];
-            int ix;
-            minOfArray(thisXbuffer, 3, &od->xLastMin, &ix);
-            od->tLastMin = od->tbuffer[ix];
+    for (int j = 0; j < N_VAR; ++j) {
+        od->xbuffer[j * 3 + 0] = od->xbuffer[j * 3 + 1];
+        od->xbuffer[j * 3 + 1] = od->xbuffer[j * 3 + 2];
+        od->xbuffer[j * 3 + 2] = xi[j];
+        od->dxbuffer[j * 3 + 0] = od->dxbuffer[j * 3 + 1];
+        od->dxbuffer[j * 3 + 1] = od->dxbuffer[j * 3 + 2];
+        od->dxbuffer[j * 3 + 2] = dxi[j];
+    }
+
+    // dt is available in the calling ode-driver. 
+    realtype dt = od->tbuffer[2]-od->tbuffer[1];
+    realtype elapsedTime = *ti - od->t_start;
+
+    //global extent of all vars, var slopes, and aux vars
+    for (int j = 0; j < N_VAR; ++j) {
+        od->xTrajectoryMax[j] = fmax(xi[j], od->xTrajectoryMax[j]);
+        od->xTrajectoryMin[j] = fmin(xi[j], od->xTrajectoryMin[j]);
+        od->xTrajectoryMean[j] = runningMeanTime(od->xTrajectoryMean[j], xi[j], dt, elapsedTime);
+        od->dxTrajectoryMax[j] = fmax(dxi[j], od->dxTrajectoryMax[j]);
+        od->dxTrajectoryMin[j] = fmin(dxi[j], od->dxTrajectoryMin[j]);
+    }
+    for (int j = 0; j < N_AUX; ++j) {
+        od->auxTrajectoryMax[j] = fmax(auxi[j], od->auxTrajectoryMax[j]);
+        od->auxTrajectoryMin[j] = fmin(auxi[j], od->auxTrajectoryMin[j]);
+        od->auxTrajectoryMean[j] = runningMeanTime(od->auxTrajectoryMean[j], xi[j], dt, elapsedTime);
+    }
+
+    // if (od->stepcount < 2)
+    //     return;
+
+    // //local max check
+    // if (od->dxbuffer[op->fVarIx * 3 + 1] > 0.0 && od->dxbuffer[op->fVarIx * 3 + 2] < 0.0) {
+    //     realtype thisXbuffer[3];
+    //     for (int j = 0; j < 3; ++j)
+    //         thisXbuffer[j] = od->xbuffer[op->fVarIx * 3 + j];
+    //     int ix = array_argmax(thisXbuffer, 3);
+    //     od->tLastMax = od->tbuffer[ix];
+    //     od->xLastMax = thisXbuffer[ix];
+
+    //     if (od->eventcount <= N_STORE_EVENTS)
+    //         od->tMaxList[od->eventcount-1] = od->tLastMax;
+    //         od->xMaxList[od->eventcount-1] = od->xLastMax;
+    // }
+
+    // if (od->eventcount < 1)
+    //     return;
+
+    if (od->stepcount < 2)
+        return;
+
+    //local min check
+    if (od->dxbuffer[op->fVarIx * 3 + 1] < 0.0 && od->dxbuffer[op->fVarIx * 3 + 2] > 0.0) {
+        realtype thisXbuffer[3];
+        for (int j = 0; j < 3; ++j)
+            thisXbuffer[j] = od->xbuffer[op->fVarIx * 3 + j];
+        int ix = array_argmin(thisXbuffer, 3);
+        od->tLastMin = od->tbuffer[ix];
+        od->xLastMin = thisXbuffer[ix];
+
+        if (od->eventcount <= N_STORE_EVENTS) {
+            od->tMinList[od->eventcount-1] = od->tLastMin;
+            od->xMinList[od->eventcount-1] = od->xLastMin;
         }
     }
 }
 
 
 
 //Perform and post-integration cleanup and write desired features into the global array F
-inline void finalizeFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __global realtype *F, int i, int nPts)
-{
+static inline void finalizeFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __global realtype *F, int i, int nPts) {
     int ix = 0;
-    // F[ix++ * nPts + i] = od->xGlobalMax-od->xGlobalMin;
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->IMI[0] : 0;
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->IMI[1] : 0;
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->IMI[2] : 0;
-    // F[ix++ * nPts + i] = od->eventcount > 1 ? od->IMI[0]-od->IMI[1]  : 0;
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->amp[0] : 0;
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->amp[1] : 0;
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->amp[2] : 0;
-    // F[ix++ * nPts + i] = od->eventcount > 1 ? od->amp[0]-od->amp[1] : 0;
-    // F[ix++ * nPts + i] = od->eventcount > 0 ? od->xMax[0] : xi[op->fVarIx];
-    // F[ix++ * nPts + i] = od->eventcount > 0 ? od->xMax[1] : xi[op->fVarIx];
-    // F[ix++ * nPts + i] = od->eventcount > 0 ? od->xMax[2] : xi[op->fVarIx];
-    // F[ix++ * nPts + i] = od->eventcount > 0 ? od->xMin[0] : xi[op->fVarIx];
-    // F[ix++ * nPts + i] = od->eventcount > 0 ? od->xMin[1] : xi[op->fVarIx];
-    // F[ix++ * nPts + i] = od->eventcount > 0 ? od->xMin[2] : xi[op->fVarIx];
-    F[ix++ * nPts + i] = od->xGlobalMax;
-    F[ix++ * nPts + i] = od->xGlobalMin;
-    F[ix++ * nPts + i] = od->xTrajectoryMean;
-    F[ix++ * nPts + i] = od->dxGlobalMax;
-    F[ix++ * nPts + i] = od->dxGlobalMin;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->IMI[0] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->IMI[1] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->IMI[2] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->amp[0] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->amp[1] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->amp[2] : ZERO;
+    for (int j = 0; j < N_VAR; ++j) {
+        F[ix++ * nPts + i] = od->xTrajectoryMax[j];
+        F[ix++ * nPts + i] = od->xTrajectoryMin[j];
+        F[ix++ * nPts + i] = od->xTrajectoryMean[j];
+        F[ix++ * nPts + i] = od->dxTrajectoryMax[j];
+        F[ix++ * nPts + i] = od->dxTrajectoryMin[j];
+    }
+    for (int j = 0; j < N_AUX; ++j) {
+        F[ix++ * nPts + i] = od->auxTrajectoryMax[j];
+        F[ix++ * nPts + i] = od->auxTrajectoryMin[j];
+        F[ix++ * nPts + i] = od->auxTrajectoryMean[j];
+    }
+    for (int j = 0; j < N_STORE_EVENTS; ++j) {
+		F[ix++ * nPts + i] = od->tMaxList[j];
+		F[ix++ * nPts + i] = od->xMaxList[j];
+		F[ix++ * nPts + i] = od->tMinList[j];
+		F[ix++ * nPts + i] = od->xMinList[j];
+    }
     F[ix++ * nPts + i] = od->eventcount;
     F[ix++ * nPts + i] = od->stepcount;
 }
 
 //Perform and post-integration cleanup of observer data to ensure it is ready for continuation if needed
-inline void finalizeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __constant realtype *tspan)
-{
+static inline void finalizeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __constant realtype *tspan) {
     //shift all time-based observer members left by [tf-t0]
     realtype T = *ti - tspan[0];
+    od->t_start -= T;
     od->tLastMax = od->tLastMax - T;
     od->tLastMin = od->tLastMin - T;
-    for (int i = 0; i < 3; ++i)
-    {
+    for (int i = 0; i < 3; ++i) {
         od->tbuffer[i] = od->tbuffer[i] - T;
     }
 }
 
 #endif //USE_OBSERVER_LOCAL_MAX
 
 #endif //OBSERVER_LOCAL_MAX_H
```

### Comparing `clode-0.7.1/clode/cpp/observers/observer_neighborhood_1.clh` & `clode-0.8.1/clode/cpp/observers/observer_neighborhood_1.clh`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 #ifndef OBSERVER_NEIGHBORHOOD_1_H
 #define OBSERVER_NEIGHBORHOOD_1_H
 
 #ifdef __cplusplus
 //Collect all the info for this observer. Must be a static function when defining function in header, otherwise defined for each time included.
-static ObserverInfo getObserverInfo_nhood1(const ProblemInfo pi, const int fVarIx, const int eVarIx)
-{
-    ObserverInfo oi;
+static struct ObserverInfo getObserverInfo_nhood1(const ProblemInfo pi, const unsigned int fVarIx, const unsigned int eVarIx, const unsigned int nStoredEvents) {
+    struct ObserverInfo oi;
     oi.define="USE_OBSERVER_NEIGHBORHOOD_1";  
     size_t n_real=(12*pi.nVar + 15 + 3*pi.nAux); //hard coded, because C++ code can't see the N_VAR, N_AUX etc...
     size_t n_int=5;
     oi.observerDataSizeFloat=n_real*sizeof(cl_float) + n_int*sizeof(cl_uint);
     oi.observerDataSizeDouble=n_real*sizeof(cl_double) + n_int*sizeof(cl_uint);  
     
     oi.featureNames.push_back("max period");
     oi.featureNames.push_back("min period");
     oi.featureNames.push_back("mean period");
     oi.featureNames.push_back("max peaks");
     oi.featureNames.push_back("min peaks");
     oi.featureNames.push_back("mean peaks");
-    for (int j = 0; j < pi.nVar; ++j)
-    {
+    for (int j = 0; j < pi.nVar; ++j) {
         oi.featureNames.push_back("max " + pi.varNames[j]);
         oi.featureNames.push_back("min " + pi.varNames[j]);
         oi.featureNames.push_back("mean " + pi.varNames[j]);
         oi.featureNames.push_back("max d" + pi.varNames[j] + "/dt");
         oi.featureNames.push_back("min d" + pi.varNames[j] + "/dt");
     }
-    for (int j = 0; j < pi.nAux; ++j)
-    {
+    for (int j = 0; j < pi.nAux; ++j) {
         oi.featureNames.push_back("max " + pi.auxNames[j]);
         oi.featureNames.push_back("min " + pi.auxNames[j]);
         oi.featureNames.push_back("mean " + pi.auxNames[j]);
     }
     oi.featureNames.push_back("period count");
     oi.featureNames.push_back("step count");
     oi.featureNames.push_back("max dt");
@@ -40,15 +37,15 @@
     return oi;
 }
 #endif
 
 
 #ifdef USE_OBSERVER_NEIGHBORHOOD_1
 
-typedef struct ObserverData_nhood1
+struct ObserverData_nhood1
 {
 
     realtype tbuffer[3];
     realtype xbuffer[3 * N_VAR];
     realtype dxbuffer[3 * N_VAR];
 
     realtype x0[N_VAR]; //point for neighborhood return
@@ -68,14 +65,15 @@
     realtype period[3];  //max/min/mean
     // realtype IMI[3]; //max/min/mean
     // realtype amp[3]; //max/min/mean
     // realtype xMax[3]; //max/min/mean
     // realtype xMin[3]; //max/min/mean
     realtype stepDt[3]; //max/min/mean
 
+    realtype t_start;
     realtype tLastEvent;
     realtype thisNormXdiff;
     realtype lastNormXdiff;
 
     // realtype xLastMax;
     // realtype tLastMax;
     // realtype xLastMin;
@@ -83,207 +81,192 @@
 
     unsigned int thisNMaxima;
     unsigned int eventcount;
     unsigned int stepcount;
     unsigned int foundX0;
     unsigned int isInNhood;
 
-} ObserverData;
+};
+
+typedef struct ObserverData_nhood1 ObserverData;
 
 //set initial values to relevant fields in ObserverData
-inline void initializeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void initializeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
 
     //put x0 in the leading position of the solution buffer
     od->tbuffer[2] = *ti;
-    for (int j = 0; j < N_VAR; ++j)
-    {
+    for (int j = 0; j < N_VAR; ++j) {
         od->xbuffer[j * 3 + 2] = xi[j];
         od->dxbuffer[j * 3 + 2] = dxi[j];
     }
 
-    for (int j = 0; j < N_VAR; ++j)
-    {
-        // od->x0[j] = RCONST(0.0); //not needed - set first time anyway.
+    for (int j = 0; j < N_VAR; ++j) {
+        // od->x0[j] = ZERO; //not needed - set first time anyway.
         // od->x0[j] = xi[j];
-        od->xTrajectoryMean[j] = RCONST(0.0); //not needed - set first time anyway.
+        od->xTrajectoryMean[j] = ZERO; //not needed - set first time anyway.
         od->xTrajectoryMax[j] = -BIG_REAL;
         od->xTrajectoryMin[j] = BIG_REAL;
         od->dxTrajectoryMax[j] = -BIG_REAL;
         od->dxTrajectoryMin[j] = BIG_REAL;
     }
-    for (int j = 0; j < N_AUX; ++j)
-    {
+    for (int j = 0; j < N_AUX; ++j) {
         od->auxTrajectoryMax[j] = -BIG_REAL;
         od->auxTrajectoryMin[j] = BIG_REAL;
-        od->auxTrajectoryMean[j] = RCONST(0.0); //not needed - set first time anyway.
+        od->auxTrajectoryMean[j] = ZERO; //not needed - set first time anyway.
     }
-    // od->tLastEvent=RCONST(0.0);
+    // od->tLastEvent=ZERO;
 
     // od->xLastMax = -BIG_REAL;
-    // od->tLastMax = RCONST(0.0);
+    // od->tLastMax = ZERO;
 
     // od->xLastMin = BIG_REAL;
-    // od->tLastMin = RCONST(0.0);
+    // od->tLastMin = ZERO;
 
     od->nMaxima[0] = -BIG_REAL;
     od->nMaxima[1] = BIG_REAL;
-    od->nMaxima[2] = RCONST(0.0);
+    od->nMaxima[2] = ZERO;
 
     od->period[0] = -BIG_REAL;
     od->period[1] = BIG_REAL;
-    od->period[2] = RCONST(0.0);
+    od->period[2] = ZERO;
 
     // od->IMI[0]=-BIG_REAL;
     // od->IMI[1]= BIG_REAL;
-    // od->IMI[2]= RCONST(0.0);
+    // od->IMI[2]= ZERO;
 
     // od->amp[0]=-BIG_REAL;
     // od->amp[1]= BIG_REAL;
-    // od->amp[2]= RCONST(0.0);
+    // od->amp[2]= ZERO;
 
     // od->xMax[0]=-BIG_REAL;
     // od->xMax[1]= BIG_REAL;
-    // od->xMax[2]= RCONST(0.0);
+    // od->xMax[2]= ZERO;
 
     // od->xMin[0]=-BIG_REAL;
     // od->xMin[1]= BIG_REAL;
-    // od->xMin[2]= RCONST(0.0);
+    // od->xMin[2]= ZERO;
 
     od->stepDt[0] = -BIG_REAL;
     od->stepDt[1] = BIG_REAL;
-    od->stepDt[2] = RCONST(0.0);
+    od->stepDt[2] = ZERO;
 
     od->thisNMaxima = 0;
     od->eventcount = 0;
     od->stepcount = 0;
     od->foundX0 = 0;
     od->isInNhood = 0;
 }
 
 //restricted per-timestep update of observer data for initializing event detector
 // - get extent of trajectory in state space, and max/min slopes
-inline void warmupObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void warmupObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
 }
 
 //process warmup data to compute relevant event detector quantities (e.g. thresholds)
-inline void initializeEventDetector(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void initializeEventDetector(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
 }
 
 //check for entry into "epsilon ball" surrounding od->x0
-inline bool eventFunction(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline bool eventFunction(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     if (od->stepcount < 2 || !od->foundX0)
         return false;
 
     //minimum amplitude check in variable: fVarIx 
-    if ( (od->xTrajectoryMax[op->fVarIx] - od->xTrajectoryMin[op->fVarIx]) > op->minXamp )
-    {
-        //save values for comparison from last timepoint
-        int lastInNhood = od->isInNhood;
-        od->lastNormXdiff = od->thisNormXdiff;
-
-        realtype thisXdiff[N_VAR];
-        for (int j = 0; j < N_VAR; ++j)
-            thisXdiff[j] = fabs(xi[j] - od->x0[j]) / (od->xTrajectoryMax[j] - od->xTrajectoryMin[j]);
-
-        // od->thisNormXdiff=norm_1(thisXdiff, N_VAR);
-        od->thisNormXdiff = norm_2(thisXdiff, N_VAR);
-        od->isInNhood = od->thisNormXdiff <= op->nHoodRadius; //L-2 norm ball
-        return (od->isInNhood & !lastInNhood); //event only on entry
-    }
-    return false;
+    if (od->xTrajectoryMax[op->fVarIx] - od->xTrajectoryMin[op->fVarIx] < op->minXamp )
+        return false;
+
+    //save values for comparison from last timepoint
+    int lastInNhood = od->isInNhood;
+    od->lastNormXdiff = od->thisNormXdiff;
+
+    realtype thisXdiff[N_VAR];
+    for (int j = 0; j < N_VAR; ++j)
+        thisXdiff[j] = fabs(xi[j] - od->x0[j]) / (od->xTrajectoryMax[j] - od->xTrajectoryMin[j]);
+
+    // od->thisNormXdiff=norm_1(thisXdiff, N_VAR);
+    od->thisNormXdiff = norm_2(thisXdiff, N_VAR);
+    od->isInNhood = od->thisNormXdiff <= op->nHoodRadius; //L-2 norm ball
+    return (od->isInNhood & !lastInNhood); //event only on entry
 }
 
 //When an event is detected, computes desired event-based features. returns true if a terminal event was reached
 // - get (t,x) at local max, compute: IMI, tMaxMin, amp
-inline bool computeEventFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline bool computeEventFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     ++od->eventcount;
 
     //simplest: time and state of trajectory point that landed in the neighborhood.
     realtype tThisEvent = *ti;
 
     //alts: linearly interp to get tThisEvent using thisNormXDiff/lastNormXDiff; use norm values as x, since we know the interp value of that
     //realtype tThisEvent = linearInterp(od->lastNormXdiff, od->thisNormXdiff, od->tbuffer[2], *ti, op->nHoodRadius);
 
-    if (od->eventcount > 1)
-    { 
+    if (od->eventcount > 1) { 
         od->nMaxima[0] = fmax((realtype)od->thisNMaxima, od->nMaxima[0]); //cast to realtype (for mean)
         od->nMaxima[1] = fmin((realtype)od->thisNMaxima, od->nMaxima[1]);
         runningMean(&od->nMaxima[2], (realtype)od->thisNMaxima, od->eventcount - 1);
 
         realtype thisPeriod = tThisEvent - od->tLastEvent;
         //realtype thisPeriod=*ti-tThisEvent;
         od->period[0] = fmax(thisPeriod, od->period[0]);
         od->period[1] = fmin(thisPeriod, od->period[1]);
         runningMean(&od->period[2], thisPeriod, od->eventcount - 1);
     }
 
     od->tLastEvent = tThisEvent;
     od->thisNMaxima = 0;
 
-    if (od->eventcount >= op->maxEventCount){
+    if (od->eventcount >= op->maxEventCount)
         return true;
-    }
+
     return false; //not terminal
 }
 
 //full per-timestep update of observer data. If an event occurred this timestep, event-based observer data is reset. Per-timestep features are computed here.
 // - advance solution/slope buffers
 // - check for any intermediate special points & store their info
 // - reset intermediates upon local max event detection
-inline void updateObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void updateObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     ++od->stepcount;
     //advance solution buffer
     od->tbuffer[0] = od->tbuffer[1];
     od->tbuffer[1] = od->tbuffer[2];
     od->tbuffer[2] = *ti;
-    for (int j = 0; j < N_VAR; ++j)
-    {
+    for (int j = 0; j < N_VAR; ++j) {
         od->xbuffer[j * 3 + 0] = od->xbuffer[j * 3 + 1];
         od->xbuffer[j * 3 + 1] = od->xbuffer[j * 3 + 2];
         od->xbuffer[j * 3 + 2] = xi[j];
         od->dxbuffer[j * 3 + 0] = od->dxbuffer[j * 3 + 1];
         od->dxbuffer[j * 3 + 1] = od->dxbuffer[j * 3 + 2];
         od->dxbuffer[j * 3 + 2] = dxi[j];
     }
 
+    //record actual dt
+    realtype thisDt = od->tbuffer[2] - od->tbuffer[1];
+    od->stepDt[0] = fmax(thisDt, od->stepDt[0]);
+    od->stepDt[1] = fmin(thisDt, od->stepDt[1]);
+    runningMean(&od->stepDt[2], thisDt, od->stepcount);
 
     //global extent of all vars, var slopes, and aux vars
-    for (int j = 0; j < N_VAR; ++j)
-    {
+    for (int j = 0; j < N_VAR; ++j) {
         od->xTrajectoryMax[j] = fmax(xi[j], od->xTrajectoryMax[j]);
         od->xTrajectoryMin[j] = fmin(xi[j], od->xTrajectoryMin[j]);
         runningMean(&od->xTrajectoryMean[j], xi[j], od->stepcount);
         od->dxTrajectoryMax[j] = fmax(dxi[j], od->dxTrajectoryMax[j]);
         od->dxTrajectoryMin[j] = fmin(dxi[j], od->dxTrajectoryMin[j]);
     }
-    for (int j = 0; j < N_AUX; ++j)
-    {
+    for (int j = 0; j < N_AUX; ++j) {
         od->auxTrajectoryMax[j] = fmax(auxi[j], od->auxTrajectoryMax[j]);
         od->auxTrajectoryMin[j] = fmin(auxi[j], od->auxTrajectoryMin[j]);
         runningMean(&od->auxTrajectoryMean[j], auxi[j], od->stepcount);
     }
 
-
-    if (od->stepcount > 1)
-    {
-        //record actual dt
-        realtype thisDt = od->tbuffer[2] - od->tbuffer[1];
-        od->stepDt[0] = fmax(thisDt, od->stepDt[0]);
-        od->stepDt[1] = fmin(thisDt, od->stepDt[1]);
-        runningMean(&od->stepDt[2], thisDt, od->stepcount);
+    if (od->stepcount > 1) {
         
         //check for x0
-        if (!od->foundX0)
-        {   // Use first local min - need it to be in eVarIx, not fVarIx. 
+        if (!od->foundX0) {   // Use first local min - need it to be in eVarIx, not fVarIx. 
             if (od->dxbuffer[op->eVarIx * 3 + 1] <= 0.0 && od->dxbuffer[op->eVarIx * 3 + 2] > 0.0 ) {
             	int ix;
                 realtype xThisMin;
                 realtype thisXbuffer[N_VAR];
                 for (int j = 0; j < 3; ++j)
                     thisXbuffer[j] = od->xbuffer[op->eVarIx * 3 + j];
             	minOfArray(thisXbuffer, 3, &xThisMin, &ix);
@@ -294,19 +277,17 @@
                 //record x0
                 for (int j = 0; j < N_VAR; ++j)
                     od->x0[j] = od->xbuffer[j*3+ix];
 
                 //get plane equation with point X0=Xi and normal vector (X0 - Xi-1)
             }
         }
-        else
-        {
+        else {
             //local max check in fVarIx - one between each min - simply overwrite tLastMax, xLastMax
-            if (od->dxbuffer[op->fVarIx * 3 + 1] >= 0.0 && od->dxbuffer[op->fVarIx * 3 + 2] < 0.0)
-            {
+            if (od->dxbuffer[op->fVarIx * 3 + 1] >= 0.0 && od->dxbuffer[op->fVarIx * 3 + 2] < 0.0) {
                 od->thisNMaxima++;
                 // int ix;
                 // realtype thisXbuffer[N_VAR];
                 // for (int j = 0; j < 3; ++j)
                 // 	thisXbuffer[j] = od->xbuffer[op->fVarIx * 3 + j];
                 // maxOfArray(thisXbuffer, 3, &od->xLastMax, &ix);
                 // od->tLastMax = od->tbuffer[ix];
@@ -332,57 +313,52 @@
             // 	// 	od->xMaxDelta[j]=od->xLast[j]-xi[j];//fmax( fabs(od->xLast[j]-xi[j]), od->xMaxDelta[j] );
             // 		// od->x0[j]=xi[j];
             // 		od->xLast[j]=xi[j];
             // 		// od->tLastEvent=*ti;
             // 	}
         }
     }
-    
 }
 
 //Perform and post-integration cleanup and write desired features into the global array F
-inline void finalizeFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __global realtype *F, int i, int nPts)
-{
+static inline void finalizeFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __global realtype *F, int i, int nPts) {
     int ix = 0;
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[0] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[1] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[2] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[0] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[1] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[2] : RCONST(0.0);
-    for (int j = 0; j < N_VAR; ++j) //5*N_VAR
-    {
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[0] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[1] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[2] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[0] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[1] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[2] : ZERO;
+    for (int j = 0; j < N_VAR; ++j) {
         F[ix++ * nPts + i] = od->xTrajectoryMax[j];
         F[ix++ * nPts + i] = od->xTrajectoryMin[j];
         F[ix++ * nPts + i] = od->xTrajectoryMean[j];
         F[ix++ * nPts + i] = od->dxTrajectoryMax[j];
         F[ix++ * nPts + i] = od->dxTrajectoryMin[j];
     }
-    for (int j = 0; j < N_AUX; ++j) //3*N_AUX
-    {
+    for (int j = 0; j < N_AUX; ++j) {
         F[ix++ * nPts + i] = od->auxTrajectoryMax[j];
         F[ix++ * nPts + i] = od->auxTrajectoryMin[j];
         F[ix++ * nPts + i] = od->auxTrajectoryMean[j];
     }
     F[ix++ * nPts + i] = od->eventcount - 1; //periods
     F[ix++ * nPts + i] = od->stepcount;
     F[ix++ * nPts + i] = od->stepDt[0];
     F[ix++ * nPts + i] = od->stepDt[1];
     F[ix++ * nPts + i] = od->stepDt[2];
 }
 
 //Perform and post-integration cleanup of observer data to ensure it is ready for continuation if needed
-inline void finalizeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __constant realtype *tspan)
-{
+static inline void finalizeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __constant realtype *tspan) {
     //shift all time-based observer members left by [tf-t0]
     realtype T = *ti - tspan[0];
+    od->t_start -= T;
     od->tLastEvent -= T;
     // od->tLastMax-=T;
     // od->tLastMin-=T;
-    for (int j = 0; j < 3; ++j)
-    {
+    for (int j = 0; j < 3; ++j) {
         od->tbuffer[j] -= T;
     }
 }
 
 #endif // USE_OBSERVER_NEIGHBORHOOD_1
 #endif // OBSERVER_NEIGHBORHOOD_1_H
```

### Comparing `clode-0.7.1/clode/cpp/observers/observer_neighborhood_2.clh` & `clode-0.8.1/clode/cpp/observers/observer_neighborhood_2.clh`

 * *Files 17% similar despite different names*

```diff
@@ -1,359 +1,316 @@
 #ifndef OBSERVER_NEIGHBORHOOD_2_H
 #define OBSERVER_NEIGHBORHOOD_2_H
 
 #ifdef __cplusplus
 //Collect all the info for this observer. Must be a static function when defining function in header, otherwise defined for each time included.
-static ObserverInfo getObserverInfo_nhood2(const ProblemInfo pi, const int fVarIx, const int eVarIx)
-{
-    ObserverInfo oi;
+static struct ObserverInfo getObserverInfo_nhood2(const ProblemInfo pi, const unsigned int fVarIx, const unsigned int eVarIx, const unsigned int nStoredEvents) {
+    struct ObserverInfo oi;
     oi.define="USE_OBSERVER_NEIGHBORHOOD_2";
-    size_t n_real=(12*pi.nVar + 16 + 3*pi.nAux); //hard coded, because C++ code can't see the N_VAR, N_AUX etc...
+    size_t n_real=(3*pi.nVar*2 + pi.nVar*7 + pi.nAux*3 + nStoredEvents + 3*4 + 3 ); //hard coded, because C++ code can't see the N_VAR, N_AUX etc...
     size_t n_int=5;
     oi.observerDataSizeFloat=n_real*sizeof(cl_float) + n_int*sizeof(cl_uint);
     oi.observerDataSizeDouble=n_real*sizeof(cl_double) + n_int*sizeof(cl_uint); 
 
     oi.featureNames.push_back("max period");
     oi.featureNames.push_back("min period");
     oi.featureNames.push_back("mean period");
     oi.featureNames.push_back("max peaks");
     oi.featureNames.push_back("min peaks");
     oi.featureNames.push_back("mean peaks");
-    for (int j = 0; j < pi.nVar; ++j)
-    {
+    for (int j = 0; j < pi.nVar; ++j) {
         oi.featureNames.push_back("max " + pi.varNames[j]);
         oi.featureNames.push_back("min " + pi.varNames[j]);
         oi.featureNames.push_back("mean " + pi.varNames[j]);
+        oi.featureNames.push_back("range " + pi.varNames[j]);
+        oi.featureNames.push_back("nhood center " + pi.varNames[j]);
         oi.featureNames.push_back("max d" + pi.varNames[j] + "/dt");
         oi.featureNames.push_back("min d" + pi.varNames[j] + "/dt");
     }
-    for (int j = 0; j < pi.nAux; ++j)
-    {
+    for (int j = 0; j < pi.nAux; ++j) {
         oi.featureNames.push_back("max " + pi.auxNames[j]);
         oi.featureNames.push_back("min " + pi.auxNames[j]);
         oi.featureNames.push_back("mean " + pi.auxNames[j]);
     }
-    oi.featureNames.push_back("period count");
+    for (int j = 0; j < nStoredEvents; ++j) {
+		oi.featureNames.push_back("nhood event time " + std::to_string(j));
+	}
+    oi.featureNames.push_back("event count");
     oi.featureNames.push_back("step count");
     oi.featureNames.push_back("max dt");
     oi.featureNames.push_back("min dt");
     oi.featureNames.push_back("mean dt");
     return oi;
 }
 #endif
 
 
 #ifdef USE_OBSERVER_NEIGHBORHOOD_2
 #define TWO_PASS_EVENT_DETECTOR
 
-typedef struct ObserverData_nhood2
+struct ObserverData_nhood2
 {
-
     realtype tbuffer[3];
     realtype xbuffer[3 * N_VAR];
     realtype dxbuffer[3 * N_VAR];
 
-    realtype x0[N_VAR]; //point for neighborhood return
-
+    realtype x0[N_VAR]; //center point of neighborhood for events
     realtype xTrajectoryMax[N_VAR];
     realtype xTrajectoryMin[N_VAR];
     realtype xTrajectoryMean[N_VAR];
+    realtype xTrajectoryRange[N_VAR];
     realtype dxTrajectoryMax[N_VAR];
     realtype dxTrajectoryMin[N_VAR];
 
     realtype auxTrajectoryMax[N_AUX];
     realtype auxTrajectoryMin[N_AUX];
     realtype auxTrajectoryMean[N_AUX];
+    
+    realtype tExitNhood[N_STORE_EVENTS];
 
     //period-wise features
     realtype nMaxima[3]; //max/min/mean
-    realtype period[3];  //max/min/mean
-    // realtype IMI[3]; //max/min/mean
-    // realtype amp[3]; //max/min/mean
-    // realtype xMax[3]; //max/min/mean
-    // realtype xMin[3]; //max/min/mean
-    realtype stepDt[3]; //max/min/mean
+    realtype period[3]; 
+    realtype stepDt[3]; 
 
+    realtype t_start;
     realtype tLastEvent;
     realtype xThreshold;
-    realtype thisNormXdiff;
-    realtype lastNormXdiff;
-
-    // realtype xLastMax;
-    // realtype tLastMax;
-    // realtype xLastMin;
-    // realtype tLastMin;
 
     unsigned int thisNMaxima;
-    unsigned int eventcount;
-    unsigned int stepcount;
     unsigned int foundX0;
     unsigned int isInNhood;
+    unsigned int eventcount;
+    unsigned int stepcount;
+
+};
 
-} ObserverData;
+typedef struct ObserverData_nhood2 ObserverData;
 
 //set initial values to relevant fields in ObserverData
-inline void initializeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void initializeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
 
     //put x0 in the leading position of the solution buffer
     od->tbuffer[2] = *ti;
-    for (int j = 0; j < N_VAR; ++j)
-    {
+    for (int j = 0; j < N_VAR; ++j) {
         od->xbuffer[j * 3 + 2] = xi[j];
         od->dxbuffer[j * 3 + 2] = dxi[j];
     }
 
-    for (int j = 0; j < N_VAR; ++j)
-    {
-        // od->x0[j] = RCONST(0.0); //not needed - set first time anyway.
-        // od->x0[j] = xi[j];
-        od->xTrajectoryMean[j] = RCONST(0.0); //not needed - set first time anyway.
+    for (int j = 0; j < N_VAR; ++j) {
+        od->x0[j] = xi[j];
         od->xTrajectoryMax[j] = -BIG_REAL;
         od->xTrajectoryMin[j] = BIG_REAL;
+        od->xTrajectoryMean[j] = ZERO; 
+        od->xTrajectoryRange[j] = ZERO; 
         od->dxTrajectoryMax[j] = -BIG_REAL;
         od->dxTrajectoryMin[j] = BIG_REAL;
     }
-    for (int j = 0; j < N_AUX; ++j)
-    {
+    for (int j = 0; j < N_AUX; ++j) {
         od->auxTrajectoryMax[j] = -BIG_REAL;
         od->auxTrajectoryMin[j] = BIG_REAL;
-        od->auxTrajectoryMean[j] = RCONST(0.0); //not needed - set first time anyway.
+        od->auxTrajectoryMean[j] = ZERO;
     }
-    // od->tLastEvent=RCONST(0.0);
-
-    // od->xLastMax = -BIG_REAL;
-    // od->tLastMax = RCONST(0.0);
-
-    // od->xLastMin = BIG_REAL;
-    // od->tLastMin = RCONST(0.0);
+	for (int j = 0; j < N_STORE_EVENTS; ++j)
+        od->tExitNhood[j] = ZERO;
 
     od->nMaxima[0] = -BIG_REAL;
     od->nMaxima[1] = BIG_REAL;
-    od->nMaxima[2] = RCONST(0.0);
+    od->nMaxima[2] = ZERO;
 
     od->period[0] = -BIG_REAL;
     od->period[1] = BIG_REAL;
-    od->period[2] = RCONST(0.0);
-
-    // od->IMI[0]=-BIG_REAL;
-    // od->IMI[1]= BIG_REAL;
-    // od->IMI[2]= RCONST(0.0);
-
-    // od->amp[0]=-BIG_REAL;
-    // od->amp[1]= BIG_REAL;
-    // od->amp[2]= RCONST(0.0);
-
-    // od->xMax[0]=-BIG_REAL;
-    // od->xMax[1]= BIG_REAL;
-    // od->xMax[2]= RCONST(0.0);
-
-    // od->xMin[0]=-BIG_REAL;
-    // od->xMin[1]= BIG_REAL;
-    // od->xMin[2]= RCONST(0.0);
+    od->period[2] = ZERO;
 
     od->stepDt[0] = -BIG_REAL;
     od->stepDt[1] = BIG_REAL;
-    od->stepDt[2] = RCONST(0.0);
+    od->stepDt[2] = ZERO;
+
+    od->t_start = *ti;
+    od->tLastEvent=ZERO;
+
+    od->xThreshold = ZERO;
 
     od->thisNMaxima = 0;
-    od->eventcount = 0;
-    od->stepcount = 0;
     od->foundX0 = 0;
     od->isInNhood = 0;
+    od->eventcount = 0;
+    od->stepcount = 0;
 }
 
 //restricted per-timestep update of observer data for initializing event detector
 // - get extent of trajectory in state space, and max/min slopes
-inline void warmupObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
-    for (int j = 0; j < N_VAR; ++j)
-    {
+static inline void warmupObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
+    for (int j = 0; j < N_VAR; ++j) {
         od->xTrajectoryMax[j] = fmax(xi[j], od->xTrajectoryMax[j]);
         od->xTrajectoryMin[j] = fmin(xi[j], od->xTrajectoryMin[j]);
     }
 }
 
 //process warmup data to compute relevant event detector quantities (e.g. thresholds)
-inline void initializeEventDetector(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
-    od->xThreshold = od->xTrajectoryMin[op->eVarIx] + op->xDownThresh * (od->xTrajectoryMax[op->eVarIx] - od->xTrajectoryMin[op->eVarIx]); 
+static inline void initializeEventDetector(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
+    for (int j = 0; j < N_VAR; ++j)
+        od->xTrajectoryRange[j] = od->xTrajectoryMax[j] - od->xTrajectoryMin[j];
+    od->xThreshold = od->xTrajectoryMin[op->eVarIx] + op->xDownThresh * od->xTrajectoryRange[op->eVarIx]; 
 }
 
-//check for entry into "epsilon ball" surrounding od->x0
-inline bool eventFunction(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+//check for exit from "epsilon ball" surrounding od->x0
+static inline bool eventFunction(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     if (od->stepcount < 2 || !od->foundX0)
         return false;
 
-    //minimum amplitude check in variable: fVarIx 
-    if ( (od->xTrajectoryMax[op->fVarIx] - od->xTrajectoryMin[op->fVarIx]) > op->minXamp )
-    {
-        //save values for comparison from last timepoint
-        int lastInNhood = od->isInNhood;
-        //od->lastNormXdiff = od->thisNormXdiff;
+    // how far are we from x0 in normalized state-space?
+    // - instead of storing x0 normalized, do: (xi-xmin)/(xmax-xmin) - (x0-xmin)/(xmax-xmin) = (xi-x0)/(xmax-xmin)
+    realtype thisXdiff[N_VAR];
+    for (int j = 0; j < N_VAR; ++j)
+        thisXdiff[j] = (xi[j] - od->x0[j]) / od->xTrajectoryRange[j];
 
-        realtype thisXdiff[N_VAR];
-        for (int j = 0; j < N_VAR; ++j)
-            thisXdiff[j] = fabs(xi[j] - od->x0[j]) / (od->xTrajectoryMax[j] - od->xTrajectoryMin[j]);
+    unsigned int lastInNhood = od->isInNhood;
+    od->isInNhood = norm_2(thisXdiff, N_VAR) < op->nHoodRadius; //L-2 norm ball
+    
+    // event on exit from nhood
+    if (lastInNhood && !od->isInNhood)
+        return true;
 
-        // od->thisNormXdiff=norm_1(thisXdiff, N_VAR);
-        od->thisNormXdiff = norm_2(thisXdiff, N_VAR);
-        od->isInNhood = od->thisNormXdiff <= op->nHoodRadius; //L-2 norm ball
-        return (od->isInNhood & !lastInNhood); //event only on entry
-    }
     return false;
 }
 
 //When an event is detected, computes desired event-based features. returns true if a terminal event was reached
-// - get (t,x) at local max, compute: IMI, tMaxMin, amp
-inline bool computeEventFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline bool computeEventFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     ++od->eventcount;
     
-    //simplest: time and state of trajectory point that landed in the neighborhood.
+    //simplest: time and state of trajectory point on exit of nhood
     realtype tThisEvent=*ti;
 
-    //alts: linearly interp to get tThisEvent using thisNormXDiff/lastNormXDiff; use norm values as x, since we know the interp value of that
-    //realtype tThisEvent = linearInterp(od->lastNormXdiff, od->thisNormXdiff, od->tbuffer[2], *ti, op->nHoodRadius);
-
-    if (od->eventcount > 1)
-    { 
+    if (od->eventcount > 1) { 
         od->nMaxima[0] = fmax((realtype)od->thisNMaxima, od->nMaxima[0]); //cast to realtype (for mean)
         od->nMaxima[1] = fmin((realtype)od->thisNMaxima, od->nMaxima[1]);
         runningMean(&od->nMaxima[2], (realtype)od->thisNMaxima, od->eventcount - 1);
 
         realtype thisPeriod = tThisEvent - od->tLastEvent;
-        //realtype thisPeriod=*ti-tThisEvent;
         od->period[0] = fmax(thisPeriod, od->period[0]);
         od->period[1] = fmin(thisPeriod, od->period[1]);
         runningMean(&od->period[2], thisPeriod, od->eventcount - 1);
     }
 
     od->tLastEvent = tThisEvent;
     od->thisNMaxima = 0;
 
-    if (od->eventcount >= op->maxEventCount){
+	if (od->eventcount <= N_STORE_EVENTS)
+        od->tExitNhood[od->eventcount-1] = tThisEvent;
+
+    if (od->eventcount == op->maxEventCount){
         return true;
     }
     return false; //not terminal
 }
 
 //full per-timestep update of observer data. If an event occurred this timestep, event-based observer data is reset. Per-timestep features are computed here.
-// - advance solution/slope buffers
-// - check for any intermediate special points & store their info
-// - reset intermediates upon local max event detection
-inline void updateObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void updateObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {    
     ++od->stepcount;
-    //advance solution buffer
+
+    // advance solution buffer
     od->tbuffer[0] = od->tbuffer[1];
     od->tbuffer[1] = od->tbuffer[2];
     od->tbuffer[2] = *ti;
-    for (int j = 0; j < N_VAR; ++j)
-    {
+
+    for (int j = 0; j < N_VAR; ++j) {
         od->xbuffer[j * 3 + 0] = od->xbuffer[j * 3 + 1];
         od->xbuffer[j * 3 + 1] = od->xbuffer[j * 3 + 2];
         od->xbuffer[j * 3 + 2] = xi[j];
         od->dxbuffer[j * 3 + 0] = od->dxbuffer[j * 3 + 1];
         od->dxbuffer[j * 3 + 1] = od->dxbuffer[j * 3 + 2];
         od->dxbuffer[j * 3 + 2] = dxi[j];
     }
 
-    //global extent of all vars, var slopes, and aux vars 
-    // [NOTE: we could do this all in the warmup pass? but then won't update if continuing]
-    for (int j = 0; j < N_VAR; ++j)
-    {
+    // dt is available in the calling ode-driver. 
+    realtype dt = od->tbuffer[2]-od->tbuffer[1];
+    realtype elapsedTime = *ti - od->t_start;
+
+    od->stepDt[0] = fmax(dt, od->stepDt[0]);
+    od->stepDt[1] = fmin(dt, od->stepDt[1]);
+    runningMean(&od->stepDt[2], dt, od->stepcount);
+
+    //global extent of all vars, var slopes, and aux vars
+    for (int j = 0; j < N_VAR; ++j) {
         od->xTrajectoryMax[j] = fmax(xi[j], od->xTrajectoryMax[j]);
         od->xTrajectoryMin[j] = fmin(xi[j], od->xTrajectoryMin[j]);
-        runningMean(&od->xTrajectoryMean[j], xi[j], od->stepcount);
+        od->xTrajectoryMean[j] = runningMeanTime(od->xTrajectoryMean[j], xi[j], dt, elapsedTime);
         od->dxTrajectoryMax[j] = fmax(dxi[j], od->dxTrajectoryMax[j]);
         od->dxTrajectoryMin[j] = fmin(dxi[j], od->dxTrajectoryMin[j]);
     }
-    for (int j = 0; j < N_AUX; ++j)
-    {
+    for (int j = 0; j < N_AUX; ++j) {
         od->auxTrajectoryMax[j] = fmax(auxi[j], od->auxTrajectoryMax[j]);
         od->auxTrajectoryMin[j] = fmin(auxi[j], od->auxTrajectoryMin[j]);
-        runningMean(&od->auxTrajectoryMean[j], auxi[j], od->stepcount);
+        od->auxTrajectoryMean[j] = runningMeanTime(od->auxTrajectoryMean[j], xi[j], dt, elapsedTime);
     }
 
-    if (od->stepcount > 1)
-    {
-        //record actual dt
-        realtype thisDt = od->tbuffer[2] - od->tbuffer[1];
-        od->stepDt[0] = fmax(thisDt, od->stepDt[0]);
-        od->stepDt[1] = fmin(thisDt, od->stepDt[1]);
-        runningMean(&od->stepDt[2], thisDt, od->stepcount);
-
-        //check for x0
-        if (!od->foundX0)
-        {   //x0 is first time dropping below threshold in x[eVarIx] - xbuffer holds previous xi
-            if (od->xbuffer[op->eVarIx * 3 + 1] > od->xThreshold && od->xbuffer[op->eVarIx * 3 + 2] < od->xThreshold)
-            {
-                od->foundX0 = 1;
-
-                //record x0
-                for (int j = 0; j < N_VAR; ++j)
-                    od->x0[j] = xi[j];
+    if (od->stepcount < 2)
+        return;
 
-                //get plane equation with point X0=Xi and normal vector (X0 - Xi-1)?
-            }
-        }
-        else
-        {
-            //local max check in fVarIx - one between each min - simply overwrite tLastMax, xLastMax
-            if (od->dxbuffer[op->fVarIx * 3 + 1] >= 0.0 && od->dxbuffer[op->fVarIx * 3 + 2] < 0.0)
-            {
-                od->thisNMaxima++;
-            }
+    if (od->foundX0) {
+        //local max check in fVarIx
+        if (od->dxbuffer[op->fVarIx * 3 + 1] >= 0.0 && od->dxbuffer[op->fVarIx * 3 + 2] < 0.0) {
+            od->thisNMaxima++;
         }
+        return;
     }
-    
+
+    // getting here means we still need to determine nhood center point x0
+    // - define x0 as first time dropping below threshold in x[eVarIx]
+    if (od->xbuffer[op->eVarIx * 3 + 1] > od->xThreshold && od->xbuffer[op->eVarIx * 3 + 2] < od->xThreshold) {
+        od->foundX0 = 1;
+        od->isInNhood = 1;
+        //record x0
+        for (int j = 0; j < N_VAR; ++j)
+            od->x0[j] = xi[j];
+    }
+
 }
 
 //Perform and post-integration cleanup and write desired features into the global array F
-inline void finalizeFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __global realtype *F, int i, int nPts)
-{
+static inline void finalizeFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __global realtype *F, int i, int nPts) {
     int ix = 0;
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[0] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[1] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[2] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[0] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[1] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[2] : RCONST(0.0);
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[0] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[1] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[2] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[0] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[1] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[2] : ZERO;
     for (int j = 0; j < N_VAR; ++j) //5*N_VAR
     {
         F[ix++ * nPts + i] = od->xTrajectoryMax[j];
         F[ix++ * nPts + i] = od->xTrajectoryMin[j];
         F[ix++ * nPts + i] = od->xTrajectoryMean[j];
+        F[ix++ * nPts + i] = od->xTrajectoryRange[j];
+        F[ix++ * nPts + i] = od->x0[j];
         F[ix++ * nPts + i] = od->dxTrajectoryMax[j];
         F[ix++ * nPts + i] = od->dxTrajectoryMin[j];
     }
     for (int j = 0; j < N_AUX; ++j) //3*N_AUX
     {
         F[ix++ * nPts + i] = od->auxTrajectoryMax[j];
         F[ix++ * nPts + i] = od->auxTrajectoryMin[j];
         F[ix++ * nPts + i] = od->auxTrajectoryMean[j];
     }
-    F[ix++ * nPts + i] = od->eventcount - 1; //periods
+    for (int j = 0; j < N_STORE_EVENTS; ++j)
+		F[ix++ * nPts + i] = od->tExitNhood[j];
+    F[ix++ * nPts + i] = od->eventcount;
     F[ix++ * nPts + i] = od->stepcount;
     F[ix++ * nPts + i] = od->stepDt[0];
     F[ix++ * nPts + i] = od->stepDt[1];
     F[ix++ * nPts + i] = od->stepDt[2];
 }
 
 //Perform and post-integration cleanup of observer data to ensure it is ready for continuation if needed
-inline void finalizeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __constant realtype *tspan)
-{
+static inline void finalizeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __constant realtype *tspan) {
     //shift all time-based observer members left by [tf-t0]
     realtype T = *ti - tspan[0];
+    od->t_start -= T;
     od->tLastEvent -= T;
-    // od->tLastMax-=T;
-    // od->tLastMin-=T;
-    for (int j = 0; j < 3; ++j)
-    {
+    for (int j = 0; j < 3; ++j) {
         od->tbuffer[j] -= T;
     }
 }
 
 #endif //USE_OBSERVER_NEIGHBORHOOD_2
 #endif // OBSERVER_NEIGHBORHOOD_2_H
```

### Comparing `clode-0.7.1/clode/cpp/observers/observer_template.clh` & `clode-0.8.1/clode/cpp/observers/observer_template.clh`

 * *Files 7% similar despite different names*

```diff
@@ -11,78 +11,68 @@
 struct ObserverData_template
 {
     unsigned int eventcount;
     unsigned int stepcount;
 }
 
 #ifdef __cplusplus
-ObserverInfo getFeatureInfo_template(const ProblemInfo pi, const int fVarIx, const int eVarIx)
-{
-    ObserverInfo oi;
+static struct ObserverInfo getFeatureInfo_template(const ProblemInfo pi, const unsigned int fVarIx, const unsigned int eVarIx, const unsigned int nStoredEvents) {
+    struct ObserverInfo oi;
     oi.define="USE_OBSERVER_TEMPLATE";
     oi.observerDataSizeFloat=sizeof(ObserverData_basic<float>);
     oi.observerDataSizeDouble=sizeof(ObserverData_basic<double>);
 
     //feature names. Could depend on problem info; nVar, varNames, etc. make sure this matches number of features actually returned
     oi.featureNames={}; 
 
     return oi;
 }
 #endif
 
 #ifdef USE_OBSERVER_TEMPLATE //should only be defined for OpenCL preprocessor, thus not included by C++ clODE codes
 
-#include "clODE_utilities.cl" //common math functions
 typedef struct ObserverData_template ObserverData;
 
 //set initial values to relevant fields in ObserverData
-inline void initializeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void initializeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     od->eventcount = 0;
     od->stepcount = 0;
 }
 
 //restricted per-timestep update of observer data for initializing event detector
-inline void warmupObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void warmupObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
 }
 
 //process warmup data to compute relevant event detector quantities (e.g. thresholds)
-inline void initializeEventDetector(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void initializeEventDetector(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
 }
 
 //per-timestep check for an event.  Option: refine event (t,x,dx,aux) within the timestep with interpolation
-inline bool eventFunction(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline bool eventFunction(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     return false;
 }
 
 //When an event is detected, computes desired event-based features. returns true if a terminal event was reached
-inline bool computeEventFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline bool computeEventFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     ++od->eventcount;
     if (od->eventcount > op->maxEventCount){
         return true;
     }
     return false;
 }
 
 //full per-timestep update of observer data. If an event occurred this timestep, event-based observer data is reset. Per-timestep features are computed here.
-inline void updateObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void updateObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     ++od->stepcount;
 }
 
 //Perform and post-integration cleanup and write desired features into the global array F
-inline void finalizeFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __global realtype *F, int i, int nPts)
-{ 
+static inline void finalizeFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __global realtype *F, int i, int nPts) { 
 }
 
 //Perform and post-integration cleanup of observer data to ensure it is ready for continuation if needed
-inline void finalizeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __constant realtype *tspan)
-{//eg. times of last events need to be shifted left of t0
+static inline void finalizeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __constant realtype *tspan) {//eg. times of last events need to be shifted left of t0
 }
 
 #endif
 
 #endif // OBSERVER_TEMPLATE_H
```

### Comparing `clode-0.7.1/clode/cpp/observers/observer_threshold_1.clh` & `clode-0.8.1/clode/cpp/observers/observer_threshold_1.clh`

 * *Files 4% similar despite different names*

```diff
@@ -57,62 +57,59 @@
     realtype auxLastMax[N_AUX];
 
     realtype tLastMin;
     realtype xLastMin[N_VAR];
     realtype dxLastMin[N_VAR];
     realtype auxLastMin[N_AUX];
 
-    int stepcount;
-    int eventcount;
-    int mincount;
-    int eventmincount;
-    int maxcount;
-    int eventmaxcount;
+    unsigned int stepcount;
+    unsigned int eventcount;
     bool inUpstate;
 };
 
 typedef struct ObserverData ObserverData;
 
 //set initial values to relevant fields in ObserverData
-inline void initializeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
+static inline void initializeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
 {
 }
 
 //restricted per-timestep update of observer data for initializing event detector
-inline void warmupObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
+static inline void warmupObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
 {
 }
 
 //process warmup data to compute relevant event detector quantities (e.g. thresholds)
-inline void initializeEventDetector(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
+static inline void initializeEventDetector(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
 {
 }
 
 //per-timestep check for an event.  Option: refine event (t,x,dx,aux) within the timestep with interpolation
-inline bool eventFunction(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
+static inline bool eventFunction(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
 {
     return false;
 }
 
 //When an event is detected, computes desired event-based features. returns true if a terminal event was reached
-inline bool computeEventFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
+static inline bool computeEventFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
 {
     return false;
 }
 
 //full per-timestep update of observer data. If an event occurred this timestep, event-based observer data is reset. Per-timestep features are computed here.
-inline void updateObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
+static inline void updateObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
 {
+    ++od->stepcount;
 }
 
 //Perform and post-integration cleanup and write desired features into the global array F
-inline void finalizeFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __global realtype *F, int i, int nPts)
+static inline void finalizeFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __global realtype *F, int i, int nPts)
 {
     //Number of features is determined by this function. Must hardcode that number into the host program in order to allocate memory for F...
 }
 
 //Perform and post-integration cleanup of observer data to ensure it is ready for continuation if needed
-inline void finalizeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __constant realtype *tspan)
+static inline void finalizeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __constant realtype *tspan)
 {
     //eg. times of last events need to be shifted left of t0
 }
 #endif // OBSERVER_THRESHOLD_1_H
```

### Comparing `clode-0.7.1/clode/cpp/observers/observer_threshold_2.clh` & `clode-0.8.1/clode/cpp/observers/observer_threshold_2.clh`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #ifndef OBSERVER_THRESHOLD_2_H
 #define OBSERVER_THRESHOLD_2_H
 
 
 #ifdef __cplusplus
-//Collect all the info for this observer. Must be a static function when defining function in header, otherwise defined for each time included.
-static ObserverInfo getObserverInfo_thresh2(const ProblemInfo pi, const int fVarIx, const int eVarIx)
-{
-    ObserverInfo oi;
+//Collect all the info for this observer
+static struct ObserverInfo getObserverInfo_thresh2(const ProblemInfo pi, const unsigned int fVarIx, const unsigned int eVarIx, const unsigned int nStoredEvents) {
+    struct ObserverInfo oi;
     oi.define="USE_OBSERVER_THRESHOLD_2";
-    size_t n_real = (11*pi.nVar + 7*3 + 13 + 3*pi.nAux); //hard coded, because C++ code can't see the N_VAR, N_AUX etc...
+    size_t n_real = (3*pi.nVar*2 + pi.nVar*5 + pi.nAux*3 + nStoredEvents*2 + 3*8 + 16); //hard coded, because C++ code can't see the N_VAR, N_AUX etc...
     size_t n_int = 4;
     oi.observerDataSizeFloat = n_real*sizeof(cl_float) + n_int*sizeof(cl_uint);
     oi.observerDataSizeDouble = n_real*sizeof(cl_double) + n_int*sizeof(cl_uint); 
     
     oi.featureNames.push_back("max period");
     oi.featureNames.push_back("min period");
     oi.featureNames.push_back("mean period");
@@ -24,76 +23,89 @@
     oi.featureNames.push_back("mean upDuration");
     oi.featureNames.push_back("max downDuration");
     oi.featureNames.push_back("min downDuration");
     oi.featureNames.push_back("mean downDuration");
     oi.featureNames.push_back("max duty");
     oi.featureNames.push_back("min duty");
     oi.featureNames.push_back("mean duty");
-    for (int j = 0; j < pi.nVar; ++j)
-    {
+    oi.featureNames.push_back("max activeDip");
+    oi.featureNames.push_back("min activeDip");
+    oi.featureNames.push_back("mean activeDip");
+    for (int j = 0; j < pi.nVar; ++j) {
         oi.featureNames.push_back("max " + pi.varNames[j]);
         oi.featureNames.push_back("min " + pi.varNames[j]);
         oi.featureNames.push_back("mean " + pi.varNames[j]);
         oi.featureNames.push_back("max d" + pi.varNames[j] + "/dt");
         oi.featureNames.push_back("min d" + pi.varNames[j] + "/dt");
     }
-    for (int j = 0; j < pi.nAux; ++j)
-    {
+    for (int j = 0; j < pi.nAux; ++j) {
         oi.featureNames.push_back("max " + pi.auxNames[j]);
         oi.featureNames.push_back("min " + pi.auxNames[j]);
         oi.featureNames.push_back("mean " + pi.auxNames[j]);
     }
-    oi.featureNames.push_back("period count");
+    for (int j = 0; j < nStoredEvents; ++j) {
+		oi.featureNames.push_back("up event time " + std::to_string(j));
+		oi.featureNames.push_back("down event time " + std::to_string(j));
+	}
+    oi.featureNames.push_back("event count");
     oi.featureNames.push_back("step count");
-    oi.featureNames.push_back("max dt");
+  	oi.featureNames.push_back("max dt");
     oi.featureNames.push_back("min dt");
     oi.featureNames.push_back("mean dt");
     return oi;
 }
 #endif
 
 
 
 #ifdef USE_OBSERVER_THRESHOLD_2
 #define TWO_PASS_EVENT_DETECTOR
 
-struct ObserverData_thresh2
-{
+struct ObserverData_thresh2 {
     realtype tbuffer[3];
     realtype xbuffer[3 * N_VAR];
     realtype dxbuffer[3 * N_VAR];
 
     realtype xTrajectoryMax[N_VAR];
     realtype xTrajectoryMin[N_VAR];
     realtype xTrajectoryMean[N_VAR];
     realtype dxTrajectoryMax[N_VAR];
     realtype dxTrajectoryMin[N_VAR];
 
     realtype auxTrajectoryMax[N_AUX];
     realtype auxTrajectoryMin[N_AUX];
     realtype auxTrajectoryMean[N_AUX];
 
+    //event-wise features
+    realtype tUpTransition[N_STORE_EVENTS];
+    realtype tDownTransition[N_STORE_EVENTS];
+
+    //period-wise features
     realtype nMaxima[3]; //max/min/mean
     realtype period[3];  //max/min/mean
     realtype upDuration[3];  //max/min/mean
     realtype downDuration[3];  //max/min/mean
     realtype duty[3];  //max/min/mean
-
+    realtype activeDip[3];  //max/min/mean
     realtype stepDt[3]; //max/min/mean
 
+    realtype fVarUpstateMean;
+    realtype fVarDownstateMean;
+
     //thresholds
     realtype xGlobalMax;
     realtype xGlobalMin;
     realtype dxGlobalMax;
     realtype dxGlobalMin;
     realtype xUp;
     realtype xDown;
     realtype dxUp;
     realtype dxDown;
 
+    realtype t_start;
     realtype tLastEvent;
     realtype tThisDown;
 
     realtype tLastMax; //compare to tThis
     realtype tLastMin;
     realtype xLastMin; 
 
@@ -102,159 +114,159 @@
     unsigned int eventcount;
     unsigned int inUpstate;
 };
 
 typedef struct ObserverData_thresh2 ObserverData;
 
 //set initial values to relevant fields in ObserverData
-inline void initializeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void initializeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     od->tbuffer[2] = *ti;
-    for (int j = 0; j < N_VAR; ++j)
-    {
+    for (int j = 0; j < N_VAR; ++j) {
         od->xbuffer[j * 3 + 2] = xi[j];
         od->dxbuffer[j * 3 + 2] = dxi[j];
     }
-
-    for (int j = 0; j < N_VAR; ++j)
-    {
-        od->xTrajectoryMean[j] = RCONST(0.0); //not needed - set first time anyway.
+    for (int j = 0; j < N_VAR; ++j) {
+        od->xTrajectoryMean[j] = ZERO; //not needed - set first time anyway.
         od->xTrajectoryMax[j] = -BIG_REAL;
         od->xTrajectoryMin[j] = BIG_REAL;
         od->dxTrajectoryMax[j] = -BIG_REAL;
         od->dxTrajectoryMin[j] = BIG_REAL;
     }
-    for (int j = 0; j < N_AUX; ++j)
-    {
+    for (int j = 0; j < N_AUX; ++j) {
         od->auxTrajectoryMax[j] = -BIG_REAL;
         od->auxTrajectoryMin[j] = BIG_REAL;
-        od->auxTrajectoryMean[j] = RCONST(0.0); //not needed - set first time anyway.
+        od->auxTrajectoryMean[j] = ZERO; //not needed - set first time anyway.
     }
+    for (int j = 0; j < N_STORE_EVENTS; ++j) {
+		od->tUpTransition[j] = ZERO;
+		od->tDownTransition[j] = ZERO;
+	}
 
     od->nMaxima[0] = -BIG_REAL;
     od->nMaxima[1] = BIG_REAL;
-    od->nMaxima[2] = RCONST(0.0);
+    od->nMaxima[2] = ZERO;
 
     od->period[0] = -BIG_REAL;
     od->period[1] = BIG_REAL;
-    od->period[2] = RCONST(0.0);
+    od->period[2] = ZERO;
 
     od->upDuration[0] = -BIG_REAL;
     od->upDuration[1] = BIG_REAL;
-    od->upDuration[2] = RCONST(0.0);
+    od->upDuration[2] = ZERO;
 
     od->downDuration[0] = -BIG_REAL;
     od->downDuration[1] = BIG_REAL;
-    od->downDuration[2] = RCONST(0.0);
+    od->downDuration[2] = ZERO;
 
     od->duty[0] = -BIG_REAL;
     od->duty[1] = BIG_REAL;
-    od->duty[2] = RCONST(0.0);
+    od->duty[2] = ZERO;
+
+    od->activeDip[0] = -BIG_REAL;
+    od->activeDip[1] = BIG_REAL;
+    od->activeDip[2] = ZERO;
 
     od->stepDt[0] = -BIG_REAL;
     od->stepDt[1] = BIG_REAL;
-    od->stepDt[2] = RCONST(0.0);
+    od->stepDt[2] = ZERO;
+
+    od->fVarDownstateMean = ZERO;
 
     od->xGlobalMax = -BIG_REAL;
     od->xGlobalMin = BIG_REAL;
     od->dxGlobalMax = -BIG_REAL;
     od->dxGlobalMin = BIG_REAL;
-    od->xUp = RCONST(0.0);
-    od->xDown = RCONST(0.0);
-    od->dxUp = RCONST(0.0);
-    od->dxDown = RCONST(0.0);
-    od->tLastEvent = RCONST(0.0);
-    od->tThisDown = RCONST(0.0);
-    od->tLastMax = -BIG_REAL;
-    od->tLastMin = RCONST(0.0);
-    od->xLastMin = -BIG_REAL; 
+    od->xUp = ZERO;
+    od->xDown = ZERO;
+    od->dxUp = ZERO;
+    od->dxDown = ZERO;
+    
+    od->t_start = *ti;
+    od->tLastEvent = ZERO;
+    od->tThisDown = ZERO;
+    od->tLastMax = ZERO;
+    od->tLastMin = ZERO;
+    od->xLastMin = BIG_REAL; 
 
+    od->inUpstate=0;
     od->thisNMaxima=0;
     od->stepcount=0;
     od->eventcount=0;
-    od->inUpstate=0;
 }
 
 //restricted per-timestep update of observer data for initializing event detector
-inline void warmupObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void warmupObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     // only need eVarix for thresholds
     od->xGlobalMax = fmax(od->xGlobalMax, xi[op->eVarIx]);
     od->xGlobalMin = fmin(od->xGlobalMin, xi[op->eVarIx]);
     od->dxGlobalMax = fmax(od->dxGlobalMax, dxi[op->eVarIx]);
     od->dxGlobalMin = fmin(od->dxGlobalMin, dxi[op->eVarIx]);
 }
 
 //process warmup data to compute relevant event detector quantities (e.g. thresholds)
-inline void initializeEventDetector(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void initializeEventDetector(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     //threshold in x
     realtype xTrajectoryAmp = od->xGlobalMax - od->xGlobalMin;
     od->xUp = od->xGlobalMin + op->xUpThresh * xTrajectoryAmp;
-	if(op->xDownThresh>RCONST(0.0))
+	if(op->xDownThresh>ZERO)
 		od->xDown = od->xGlobalMin + op->xDownThresh * xTrajectoryAmp;
 	else
 		od->xDown = od->xUp;
 
     //threshold for dx
     od->dxUp =  op->dxUpThresh * od->dxGlobalMax;
-	if(op->dxDownThresh>RCONST(0.0))
+	if(op->dxDownThresh>ZERO)
         od->dxDown = op->dxDownThresh * od->dxGlobalMin;
 	else
 		od->dxDown = od->dxGlobalMin;
 
 	//determine if we are up or down.
 	od->inUpstate = xi[op->eVarIx] > od->xUp ? 1 : 0;
-	// od->inUpstate = xi[op->eVarIx] > od->xUp & dxi[op->eVarIx] > 0 ? 1 : 0;
-    // od->xGlobalMax = -BIG_REAL;
-    // od->xGlobalMin = BIG_REAL;
-    // od->dxGlobalMax = -BIG_REAL;
-    // od->dxGlobalMin = BIG_REAL;
 }
 
 //per-timestep check for an event.  Option: refine event (t,x,dx,aux) within the timestep with interpolation
-inline bool eventFunction(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline bool eventFunction(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     if (od->stepcount < 2)
         return false;
 
     if (od->xGlobalMax - od->xGlobalMin < op->minXamp)
         return false;
 
+    if (od->inUpstate)
+        return false;
+
     //event is marked by upward threshold crossing
-    return (!od->inUpstate && xi[op->eVarIx] > od->xUp && dxi[op->eVarIx] > od->dxUp);
+    return (xi[op->eVarIx] > od->xUp && dxi[op->eVarIx] > od->dxUp);
     
 }
 
 //When an event is detected, computes desired event-based features. returns true if a terminal event was reached
-inline bool computeEventFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline bool computeEventFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     realtype tThisEvent;
 
     ++od->eventcount;
     od->inUpstate = 1;
 
     //simplest: time and state of trajectory point that landed in the neighborhood.
     tThisEvent=*ti;
 
-    //alts: linearly interp to get more accurate tThisEvent within the last time step: xi-1, xi, ti-1, ti; get t @ x=xUp
+    //alt: interp to get more accurate tThisEvent within the last time step: xi-1, xi, ti-1, ti; get t @ x=xUp
     // realtype thisXbuffer[N_VAR];
     // thisXbuffer[0] = od->xbuffer[op->fVarIx * 3 + 1];
     // thisXbuffer[1] = od->xbuffer[op->fVarIx * 3 + 2];
     // thisXbuffer[2] = xi[op->fVarIx];
     // realtype thisTbuffer[3];
     // thisTbuffer[0] = od->tbuffer[1];
     // thisTbuffer[1] = od->tbuffer[2];
     // thisTbuffer[2] = *ti;
     // tThisEvent = linearInterpArray(thisXbuffer, thisTbuffer, od->xUp);
 
-    if (od->eventcount > 1)
-    {
+    if (od->eventcount > 1) {
         int nPeriods = od->eventcount - 1;
-        od->nMaxima[0] = fmax((realtype)od->thisNMaxima, od->nMaxima[0]); //int to realtype implicit cast is OK
+        od->nMaxima[0] = fmax((realtype)od->thisNMaxima, od->nMaxima[0]);
         od->nMaxima[1] = fmin((realtype)od->thisNMaxima, od->nMaxima[1]);
         runningMean(&od->nMaxima[2], (realtype)od->thisNMaxima, nPeriods);
 
         realtype thisPeriod = tThisEvent - od->tLastEvent;
         od->period[0] = fmax(thisPeriod, od->period[0]);
         od->period[1] = fmin(thisPeriod, od->period[1]);
         runningMean(&od->period[2], thisPeriod, nPeriods);
@@ -269,167 +281,193 @@
         od->downDuration[1] = fmin(thisDownDuration, od->downDuration[1]);
         runningMean(&od->downDuration[2], thisDownDuration, nPeriods);
         
         realtype thisduty = thisUpDuration/thisPeriod;
         od->duty[0] = fmax(thisduty, od->duty[0]);
         od->duty[1] = fmin(thisduty, od->duty[1]);
         runningMean(&od->duty[2], thisduty, nPeriods);
+
+        realtype thisActiveDip = od->fVarDownstateMean - od->xLastMin;
+        od->activeDip[0] = fmax(thisActiveDip, od->activeDip[0]);
+        od->activeDip[1] = fmin(thisActiveDip, od->activeDip[1]);
+        runningMean(&od->activeDip[2], thisActiveDip, nPeriods);
     }
 
+	if (od->eventcount <= N_STORE_EVENTS)
+    	od->tUpTransition[od->eventcount-1] = tThisEvent;
+
     od->tLastEvent = tThisEvent;
     od->thisNMaxima = 0;
 
-    if (od->eventcount >= op->maxEventCount){
+    if (od->eventcount == op->maxEventCount)
         return true;
-    }
+
     return false;
 }
 
 //full per-timestep update of observer data. If an event occurred this timestep, event-based observer data is reset. Per-timestep features are computed here.
-inline void updateObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op)
-{
+static inline void updateObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op) {
     ++od->stepcount;
-    //advance solution buffer
+
+    // advance solution buffer
     od->tbuffer[0] = od->tbuffer[1];
     od->tbuffer[1] = od->tbuffer[2];
     od->tbuffer[2] = *ti;
-    for (int j = 0; j < N_VAR; ++j)
-    {
+
+    for (int j = 0; j < N_VAR; ++j) {
         od->xbuffer[j * 3 + 0] = od->xbuffer[j * 3 + 1];
         od->xbuffer[j * 3 + 1] = od->xbuffer[j * 3 + 2];
         od->xbuffer[j * 3 + 2] = xi[j];
         od->dxbuffer[j * 3 + 0] = od->dxbuffer[j * 3 + 1];
         od->dxbuffer[j * 3 + 1] = od->dxbuffer[j * 3 + 2];
         od->dxbuffer[j * 3 + 2] = dxi[j];
     }
-    
+
+    // dt is available in the calling ode-driver. 
+    realtype dt = od->tbuffer[2]-od->tbuffer[1];
+    realtype elapsedTime = *ti - od->t_start;
+
+    od->stepDt[0] = fmax(dt, od->stepDt[0]);
+    od->stepDt[1] = fmin(dt, od->stepDt[1]);
+    runningMean(&od->stepDt[2], dt, od->stepcount);
+
     //global extent of all vars, var slopes, and aux vars
-    for (int j = 0; j < N_VAR; ++j)
-    {
+    for (int j = 0; j < N_VAR; ++j) {
         od->xTrajectoryMax[j] = fmax(xi[j], od->xTrajectoryMax[j]);
         od->xTrajectoryMin[j] = fmin(xi[j], od->xTrajectoryMin[j]);
-        runningMean(&od->xTrajectoryMean[j], xi[j], od->stepcount);
+        od->xTrajectoryMean[j] = runningMeanTime(od->xTrajectoryMean[j], xi[j], dt, elapsedTime);
         od->dxTrajectoryMax[j] = fmax(dxi[j], od->dxTrajectoryMax[j]);
         od->dxTrajectoryMin[j] = fmin(dxi[j], od->dxTrajectoryMin[j]);
     }
-    for (int j = 0; j < N_AUX; ++j)
-    {
+    for (int j = 0; j < N_AUX; ++j) {
         od->auxTrajectoryMax[j] = fmax(auxi[j], od->auxTrajectoryMax[j]);
         od->auxTrajectoryMin[j] = fmin(auxi[j], od->auxTrajectoryMin[j]);
-        runningMean(&od->auxTrajectoryMean[j], auxi[j], od->stepcount);
+        od->auxTrajectoryMean[j] = runningMeanTime(od->auxTrajectoryMean[j], xi[j], dt, elapsedTime);
     }
 
-    if (od->stepcount > 1)
-    {
-        //record actual dt
-        realtype thisDt = od->tbuffer[2] - od->tbuffer[1];
-        od->stepDt[0] = fmax(thisDt, od->stepDt[0]);
-        od->stepDt[1] = fmin(thisDt, od->stepDt[1]);
-        runningMean(&od->stepDt[2], thisDt, od->stepcount);
+    if (od->stepcount > 1) {
         
         //local max check in fVarIx
-        if (od->dxbuffer[op->fVarIx * 3 + 1] >= 0.0 && od->dxbuffer[op->fVarIx * 3 + 2] < 0.0)
-        {
+        if (od->dxbuffer[op->fVarIx * 3 + 1] > 0.0 && od->dxbuffer[op->fVarIx * 3 + 2] < 0.0) {
             int ix;
             realtype thisXbuffer[N_VAR];
             realtype xThisMax;
             for (int j = 0; j < 3; ++j)
             	thisXbuffer[j] = od->xbuffer[op->fVarIx * 3 + j];
             maxOfArray(thisXbuffer, 3, &xThisMax, &ix);
             realtype tThisMax = od->tbuffer[ix];
 
-            // initialize tLastMax and xLastMin such that the first time around, thisIMI and thisAmp are BIG_REAL
-            // after one max has been recorded, check for minAmp & minIMI: guaranteed a min between
-            realtype thisAmp = xThisMax - od->xLastMin;
-            realtype thisIMI = tThisMax - od->tLastMax;
-
-            if (od->thisNMaxima==0 || (thisAmp > op->minXamp && thisIMI > op->minIMI) )
-            {
-                od->thisNMaxima++;
-                od->tLastMax = tThisMax; //store this time for next IMI
-            }
+            od->thisNMaxima++;
+            od->tLastMax = tThisMax;
+
+            // // initialize tLastMax and xLastMin such that the first time around, thisIMI and thisAmp are BIG_REAL
+            // // after one max has been recorded, check for minAmp & minIMI: guaranteed a min between
+            // realtype thisAmp = xThisMax - od->xLastMin;
+            // realtype thisIMI = tThisMax - od->tLastMax;
+
+            // if (od->thisNMaxima==0 || (thisAmp > op->minXamp && thisIMI > op->minIMI) )
+            // {
+            //     od->thisNMaxima++;
+            //     od->tLastMax = tThisMax; //store this time for next IMI
+            // }
         }
 
         //local min check in fVarIx - one between each max - simply overwrite tLastMin, xLastMin
-        if (od->dxbuffer[op->fVarIx * 3 + 1] <= 0.0 && od->dxbuffer[op->fVarIx * 3 + 2] > 0.0)
-        {
+        if (od->dxbuffer[op->fVarIx * 3 + 1] < 0.0 && od->dxbuffer[op->fVarIx * 3 + 2] > 0.0) {
             int ix;
             realtype thisXbuffer[N_VAR];
             for (int j = 0; j < 3; ++j)
             	thisXbuffer[j] = od->xbuffer[op->fVarIx * 3 + j];
             minOfArray(thisXbuffer, 3, &od->xLastMin, &ix);
             od->tLastMin = od->tbuffer[ix]; //actually not used...
         }
 
-        //Check for downward threshold crossing (end of "active phase")
-        if (xi[op->fVarIx] < od->xDown && dxi[op->fVarIx] > od->dxDown && od->inUpstate)
-        {
-            //simplest: time and state of trajectory point that landed in the neighborhood.
-            od->tThisDown=*ti;
-
-            //alts: linearly interp to get more accurate tThisEvent within the last time step: xi-1, xi, ti-1, ti; get t @ x=xUp
-            // od->tThisDown = linearInterp(od->xbuffer[2], xi[op->fVarIx], od->tbuffer[2], *ti, od->xDown);
-            od->inUpstate = 0;
+        if (od->inUpstate) {
+            //Check for downward threshold crossing
+            if (xi[op->eVarIx] <= od->xDown && dxi[op->eVarIx] >= od->dxDown) {
+                //simplest: time and state of trajectory point that landed in the neighborhood.
+                od->tThisDown=*ti;
+
+                //alts: linearly interp to get more accurate tThisEvent within the last time step: xi-1, xi, ti-1, ti; get t @ x=xUp
+                // od->tThisDown = linearInterp(od->xbuffer[2], xi[op->fVarIx], od->tbuffer[2], *ti, od->xDown);
+                od->inUpstate = 0;
+                
+                if (od->eventcount > 0 && od->eventcount <= N_STORE_EVENTS)
+                    od->tDownTransition[od->eventcount-1] = od->tThisDown;
+                
+                od->fVarDownstateMean = xi[op->fVarIx];
+            }
         }
+        else {
+            // Compute running mean of the down state
+			realtype elapsedDownTime = (*ti - od->tThisDown);
+			if (elapsedDownTime > 0.0)
+                od->fVarDownstateMean = runningMeanTime(od->fVarDownstateMean, xi[op->fVarIx], dt, elapsedDownTime);
+		}
     }
 }
 
 
 //Perform and post-integration cleanup and write desired features into the global array F
-inline void finalizeFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __global realtype *F, int i, int nPts)
-{
+static inline void finalizeFeatures(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __global realtype *F, int i, int nPts) {
     //Number of features is determined by this function. Must hardcode that number into the host program in order to allocate memory for F...
     int ix = 0;
     // eventcount=2 means one period was recorded
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[0] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[1] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[2] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[0] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[1] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[2] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->upDuration[0] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->upDuration[1] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->upDuration[2] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->downDuration[0] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->downDuration[1] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->downDuration[2] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->duty[0] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->duty[1] : RCONST(0.0);
-    F[ix++ * nPts + i] = od->eventcount > 1 ? od->duty[2] : RCONST(0.0);
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[0] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[1] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->period[2] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[0] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[1] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->nMaxima[2] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->upDuration[0] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->upDuration[1] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->upDuration[2] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->downDuration[0] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->downDuration[1] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->downDuration[2] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->duty[0] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->duty[1] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->duty[2] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->activeDip[0] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->activeDip[1] : ZERO;
+    F[ix++ * nPts + i] = od->eventcount > 1 ? od->activeDip[2] : ZERO;
     for (int j = 0; j < N_VAR; ++j) //5*N_VAR
     {
         F[ix++ * nPts + i] = od->xTrajectoryMax[j];
         F[ix++ * nPts + i] = od->xTrajectoryMin[j];
         F[ix++ * nPts + i] = od->xTrajectoryMean[j];
         F[ix++ * nPts + i] = od->dxTrajectoryMax[j];
         F[ix++ * nPts + i] = od->dxTrajectoryMin[j];
     }
     for (int j = 0; j < N_AUX; ++j) //3*N_AUX
     {
         F[ix++ * nPts + i] = od->auxTrajectoryMax[j];
         F[ix++ * nPts + i] = od->auxTrajectoryMin[j];
         F[ix++ * nPts + i] = od->auxTrajectoryMean[j];
     }
-    F[ix++ * nPts + i] = od->eventcount - 1; //periods
+    for (int j = 0; j < N_STORE_EVENTS; ++j) {
+		F[ix++ * nPts + i] = od->tUpTransition[j];
+		F[ix++ * nPts + i] = od->tDownTransition[j];
+	}
+    F[ix++ * nPts + i] = od->eventcount;
     F[ix++ * nPts + i] = od->stepcount;
     F[ix++ * nPts + i] = od->stepDt[0];
     F[ix++ * nPts + i] = od->stepDt[1];
     F[ix++ * nPts + i] = od->stepDt[2];
 }
 
 //Perform and post-integration cleanup of observer data to ensure it is ready for continuation if needed
-inline void finalizeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __constant realtype *tspan)
-{
+static inline void finalizeObserverData(realtype *ti, realtype xi[], realtype dxi[], realtype auxi[], ObserverData *od, __constant struct ObserverParams *op, __constant realtype *tspan) {
     //shift all time-based observer members left by [tf-t0]
     realtype T = *ti - tspan[0];
+    od->t_start -= T;
     od->tLastEvent -= T; //i.e. tLastUp
     od->tThisDown -= T;
     od->tLastMax -= T;
     od->tLastMin -= T;
-    for (int j = 0; j < 3; ++j)
-    {
+    for (int j = 0; j < 3; ++j) {
         od->tbuffer[j] -= T;
     }
 }
 
 #endif // USE_OBSERVER_THRESHOLD_2
 #endif // OBSERVER_THRESHOLD_2_H
```

### Comparing `clode-0.7.1/clode/cpp/observers.cl` & `clode-0.8.1/clode/cpp/observers.cl`

 * *Files 22% similar despite different names*

```diff
@@ -9,27 +9,30 @@
  * - updateObserverData: per-timestep update of data structure
  * - initializeEventDetector: set any values needed to do selected type of event detection (possibly using warmup data)
  * - eventFunction: check for an event. Optionally refine location of event within timestep. Compute event-based quantities
  * - computeEventFeatures: when event is detected, compute desired per-event features
  * - finalizeFeatures: post-integration cleanup and write to global feature array
  */
 
-#include "realtype.cl"
-
 //TODO: expose different observerParams for each observer (provide relevant values only)
 //TODO: support using aux vars as event/feature var in observers.
+//TODO: concept of "solution buffer" or "solver state" data structure could simplify observer coding. Update it in the ode driver, pass to observer functions
+
+#include "realtype.cl"
+
 #ifdef __cplusplus
 template <typename realtype>
 #endif
 struct ObserverParams
 {
-    int eVarIx; //variable for event detection
-    int fVarIx; //variable for features
+    unsigned int eVarIx; //variable for event detection
+    unsigned int fVarIx; //variable for features
 
-    int maxEventCount; //time loop limiter
+    unsigned int maxEventCount; //time loop limiter
+    unsigned int maxEventTimestamps; //max number of event timestamps to store
     realtype minXamp;  //consider oscillations lower than this to be steady state (return mean X)
     realtype minIMI;
 
     //neighborhood return map
     realtype nHoodRadius;
 
     //section. Two interpretations: absolute, relative
@@ -41,76 +44,106 @@
     //local extremum - tolerance for zero crossing of dx - for single precision: if RHS involves sum of terms of O(1), dx=zero is noise at O(1e-7)
     realtype eps_dx;
 };
 
 
 #ifdef __cplusplus
 //info about available observers for access in C++
-typedef struct ObserverInfo 
+struct ObserverInfo 
 {
 	std::string define;
 	size_t observerDataSizeFloat;
 	size_t observerDataSizeDouble;
 	std::vector<std::string> featureNames;
-} ObserverInfo;
+};
 
 #endif
 
+// Design criteria
+// - use online algorithms for features such as mean, median, etc.
+// - minimize storage of state
+// - 
+
+// TODO:
+// - return sequence data: list of features per event
+// - hashing for distinct value counting [binning?] - not same as above
+// - use minimal solution buffer size for task at hand. local extrema: t[3], x[3], dx[2]?
+// - separate diagnostic features [toggle on/off independent of observer?]
+// - time (e.g., durations) vs state-space features (e.g., amplitudes, means) 
+// -- supply list of vars to track for state-space features [similarly for trajectory storage]
+// - composable observers? toggle on only what you want 
+// - how to handle domain-specific use cases? eg. AHP
+
+// TODO: combine observers with same logic but different event functions into one
+// - threshold, nhood (1/2) --> toggle with a define?
 
 ////////////////////////////////////////////////
 // one-pass detectors
 ////////////////////////////////////////////////
 
 //basic detectors: no events. Measure extent of state space explored, max/min/mean x and aux, max/min dx
 #include "observers/observer_basic.clh" //one variable, specified by fVarIx
 #include "observers/observer_basic_allVar.clh"
+
+// convex hull of trajectory in state-space?
+
+// Local maximum detector
+// - could do local extremum, toggle whether event is on max vs min?
 #include "observers/observer_local_maximum.clh"
 
+// Threshold-based event detection with thresholds defined in state-space coordinates
 // #include "observers/observer_threshold_1.clh" //not implemented
 
-//Event is the return of trajectory to small neighborhood of Xstart (specified state, eg. x0)
-// to select Xstart: local min (e.g. of user-selected slow variable) 
+// Poincaré section, specified as a normal vector and offset in state-space coordinates
+// #include "observers/observer_poincare_1.clh"
+
+// Event trigger is the return of the trajectory to small neighborhood of a point Xstart in state-space coordinates
+// - define a sensible Xstart, found in one pass: e.g., local min of a slow variable 
 #include "observers/observer_neighborhood_1.clh"
 
 ////////////////////////////////////////////////
 // two-pass detectors
 ////////////////////////////////////////////////
+// Run a first pass to establish trajectory properties - e.g., extrema for computing normalized state-space coordinates
 
-//Threshold-based event detection with relative thresholds in a specified variable xi.
-// First pass to measure the extent of state-space trajectory visits, then compute thresholds as fractions of range
+// Threshold-based event detection with thresholds defined in normalized state-space coordinates
 #include "observers/observer_threshold_2.clh"
 
-// // First pass to measure the extent of state-space trajectory visits, decide x0 based on threshold. check each crossing, period when norm(x-x0)<tol
+// Poincaré section, specified as a normal vector and offset in normalized state-space coordinates
 // #include "observers/observer_poincare_2.clh"
 
-//Use a first pass to find a good Xstart (e.g. absolute drop below 0.5*range of slowest variable)
+// Event trigger is the return of the trajectory to small neighborhood of a point Xstart in normalized state-space coordinates
+// - Use a first pass to find a good Xstart (e.g. absolute drop below 0.5*range of slowest variable)
 #include "observers/observer_neighborhood_2.clh"
 
 
 
 // collect available methods into "name"-ObserverInfo map, for C++ side access. Must come after including all the getObserverInfo_functions.
 #ifdef __cplusplus
-static void getObserverDefineMap(const ProblemInfo pi, const int fVarIx, const int eVarIx, std::map<std::string, ObserverInfo> &observerDefineMap, std::vector<std::string> &availableObserverNames) 
-{
-
-    std::map<std::string, ObserverInfo> newMap;
-    newMap["basic"]=getObserverInfo_basic(pi, fVarIx, eVarIx);
-    newMap["basicall"]=getObserverInfo_basicAll(pi, fVarIx, eVarIx);
-    newMap["localmax"]=getObserverInfo_localmax(pi, fVarIx, eVarIx);
-    newMap["nhood1"]=getObserverInfo_nhood1(pi, fVarIx, eVarIx);
-    newMap["nhood2"]=getObserverInfo_nhood2(pi, fVarIx, eVarIx);
-    newMap["thresh2"]=getObserverInfo_thresh2(pi, fVarIx, eVarIx);
-
-//export vector of names for access in C++
-std::vector<std::string> newNames;
-for (auto const& element : newMap)
-    newNames.push_back(element.first);
+static void getObserverDefineMap(const ProblemInfo pi,
+								 const unsigned int fVarIx,
+								 const unsigned int eVarIx,
+								 const unsigned int nStoredEvents,
+								 std::map<std::string, struct ObserverInfo> &observerDefineMap,
+								 std::vector<std::string> &availableObserverNames) {
+    std::map<std::string, struct ObserverInfo> newMap;
+    newMap["basic"]=getObserverInfo_basic(pi, fVarIx, eVarIx, nStoredEvents);
+    newMap["basicall"]=getObserverInfo_basicAll(pi, fVarIx, eVarIx, nStoredEvents);
+    newMap["localmax"]=getObserverInfo_localmax(pi, fVarIx, eVarIx, nStoredEvents);
+    newMap["nhood1"]=getObserverInfo_nhood1(pi, fVarIx, eVarIx, nStoredEvents);
+    newMap["nhood2"]=getObserverInfo_nhood2(pi, fVarIx, eVarIx, nStoredEvents);
+    newMap["thresh2"]=getObserverInfo_thresh2(pi, fVarIx, eVarIx, nStoredEvents);
+
+	//export vector of names for access in C++
+	std::vector<std::string> newNames;
+	for (auto const& element : newMap)
+		newNames.push_back(element.first);
 
-observerDefineMap=newMap;
-availableObserverNames=newNames;
+	observerDefineMap=newMap;
+	availableObserverNames=newNames;
 }
 #endif
 
 
 #endif //OBSERVERS_H_
 
 /*
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `clode-0.7.1/clode/cpp/odedriver.cl` & `clode-0.8.1/clode/cpp/odedriver.cl`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// currently unused...
+// Unified features + trajectory kernel. currently unused...
 
 #include "clODE_random.cl"
 #include "clODE_struct_defs.cl"
 #include "clODE_utilities.cl"
 #include "observers.cl"
 #include "realtype.cl"
 #include "steppers.cl"
@@ -10,125 +10,149 @@
 __kernel void odedriver(
     __constant realtype *tspan,         //time vector [t0,tf] - adds (tf-t0) to these at the end
     __global realtype *x0,              //initial state 				[nPts*nVar]
     __constant realtype *pars,          //parameter values				[nPts*nPar]
     __constant struct SolverParams *sp, //dtmin/max, tols, etc
     __global realtype *xf,              //final state 				[nPts*nVar]
     __global ulong *RNGstate,            //state for RNG					[nPts*nRNGstate]
-    __global ObserverData *OData,        //Observer data. Assume it is initialized externally by initialize observer kernel!
-    __constant struct ObserverParams *opars,
-    __global realtype *F,  //feature results
+    __global realtype *d_dt,            //array of dt values, one per solver
     __global realtype *t,  // trajectory storage: t, x, dx, aux
     __global realtype *x,
     __global realtype *dx,
     __global realtype *aux,
-    __global int *nStored)
+    __global int *nStored,
+    __global ObserverData *OData,        //Observer data 
+    __constant struct ObserverParams *opars,
+    __global realtype *t_event,  // trajectory storage: t, x, dx, aux
+    __global realtype *x_event,
+    __global realtype *dx_event,
+    __global realtype *aux_event,
+    __global realtype *F) 
 {
 
     int i = get_global_id(0);
     int nPts = get_global_size(0);
 
     realtype ti, dt;
-    realtype p[N_PAR], xi[N_VAR], dxi[N_VAR], auxi[N_AUX], wi[N_WIENER];
-    rngData rd;
-    __constant realtype * const tspanPtr = tspan;
+    realtype p[N_PAR], xi[N_VAR], dxi[N_VAR];
+    realtype auxi[N_AUX>0?N_AUX:1];
+    realtype wi[N_WIENER>0?N_WIENER:1];
+    struct rngData rd;
 
-    //get private copy of ODE parameters, initial data, and compute slope at initial state
+    //get private copy of ODE parameters, initial data, and random state
     ti = tspan[0];
-    dt = sp->dt;
+    dt = d_dt[i];
 
     for (int j = 0; j < N_PAR; ++j)
         p[j] = pars[j * nPts + i];
 
     for (int j = 0; j < N_VAR; ++j)
         xi[j] = x0[j * nPts + i];
 
     for (int j = 0; j < N_RNGSTATE; ++j)
         rd.state[j] = RNGstate[j * nPts + i];
 
-    rd.randnUselast = 0;
+    if (sp->useObserver){
+	    ObserverData odata = OData[i]; //private copy of observer data
+    }
 
+    // generate random numbers if needed
+    rd.randnUselast = 0;
     for (int j = 0; j < N_WIENER; ++j)
 #ifdef STOCHASTIC_STEPPER
         wi[j] = randn(&rd) / sqrt(dt);
 #else
-        wi[j] = RCONST(0.0);
+        wi[j] = ZERO;
 #endif
-	getRHS(ti, xi, p, dxi, auxi, wi); //slope at initial point, needed for FSAL steppers (bs23, dorpri5)
 
-    //store the initial point --> could be set elsewhere using an "init" kernel?
-    int storeix = 0;
-    t[storeix + i] = tspan[0];
-    for (int j = 0; j < N_VAR; ++j)
-        x[storeix * nPts * N_VAR + j * nPts + i] = xi[j];
+    //get the slope and aux at initial point
+    getRHS(ti, xi, p, dxi, auxi, wi); 
 
-    for (int j = 0; j < N_VAR; ++j)
-        dx[storeix * nPts * N_VAR + j * nPts + i] = dxi[j];
-
-    for (int j = 0; j < N_AUX; ++j)
-        aux[storeix * nPts * N_AUX + j * nPts + i] = auxi[j];
-
-    ObserverData odata = OData[i]; //private copy of observer data. Assume it is initialized externally by initialize observer kernel
+    //store the initial point
+    unsigned int storeix = 0;
+    if (sp->storeTrajectory == 1)
+    {
+        int storeix = 0;
+        t[storeix * nPts + i] = ti;
+        for (int j = 0; j < N_VAR; ++j)
+            x[storeix * nPts * N_VAR + j * nPts + i] = xi[j];
+        for (int j = 0; j < N_VAR; ++j)
+            dx[storeix * nPts * N_VAR + j * nPts + i] = dxi[j];
+        for (int j = 0; j < N_AUX; ++j)
+            aux[storeix * nPts * N_AUX + j * nPts + i] = auxi[j];
+    }
 
-    //time-stepping loop, main time interval
-    int step = 0;
+	//time-stepping loop
+    unsigned int step = 0;
+    unsigned int eventcount = 0;
+    unsigned int eventstoreix = 0;
     int stepflag = 0;
     bool eventOccurred;
     bool terminalEvent;
-    while (ti < tspan[1] && step < sp->max_steps && storeix < sp->max_store)
+    while (ti <= tspan[1] && step < sp->max_steps && storeix < sp->max_store)
     {
-
-        ++step;
-        //++odata.stepcount;
-        stepflag = stepper(&ti, xi, dxi, p, sp, &dt, tspanPtr, auxi, wi, step, &rd);
-        if (stepflag!=0)
-            break;
-
-        eventOccurred = eventFunction(&ti, xi, dxi, auxi, &odata, opars);
-        if (eventOccurred)
-        {
-            terminalEvent = computeEventFeatures(&ti, xi, dxi, auxi, &odata, opars);
-            if (terminalEvent)
+		++step;
+        stepflag = stepper(&ti, xi, dxi, p, sp, &dt, tspan, auxi, wi, &rd);
+        // if (stepflag!=0) //handle numerical problems from time-stepper?
+            // break;
+
+        if (sp->useObserver){
+            eventOccurred = eventFunction(&ti, xi, dxi, auxi, &odata, opars);
+            if (eventOccurred)
             {
-                break;
-            };
-        }
+                ++eventcount;
+                if (eventcount < op->maxEventTimestamps)
+                {
+                    t_event[eventcount * nPts + i] = ti;
+                    for (int j = 0; j < N_VAR; ++j)
+                        x_event[eventcount * nPts * N_VAR + j * nPts + i] = xi[j];
+                    for (int j = 0; j < N_VAR; ++j)
+                        dx_event[eventcount * nPts * N_VAR + j * nPts + i] = dxi[j];
+                    for (int j = 0; j < N_AUX; ++j)
+                        aux_event[eventcount * nPts * N_AUX + j * nPts + i] = auxi[j];
+                }
+                terminalEvent = computeEventFeatures(&ti, xi, dxi, auxi, &odata, opars);
+                if (terminalEvent | eventcount == op->maxEventCount)
+                    break;
+            }
 
-        updateObserverData(&ti, xi, dxi, auxi, &odata, opars); //TODO: if not FSAL, dxi buffer is delayed by one. (dxi is slope at LAST timestep)
+            updateObserverData(&ti, xi, dxi, auxi, &odata, opars); 
+        }
 
         //store every sp.nout'th step after the initial point
         if (step % sp->nout == 0)
         {
             ++storeix;
-
             t[storeix * nPts + i] = ti; //adaptive steppers give different timepoints for each trajectory
-
             for (int j = 0; j < N_VAR; ++j)
                 x[storeix * nPts * N_VAR + j * nPts + i] = xi[j];
-
             for (int j = 0; j < N_VAR; ++j)
                 dx[storeix * nPts * N_VAR + j * nPts + i] = dxi[j];
-
             for (int j = 0; j < N_AUX; ++j)
                 aux[storeix * nPts * N_AUX + j * nPts + i] = auxi[j];
         }
     }
 
-    //readout features of interest and write to global F:
-    finalizeFeatures(&ti, xi, dxi, auxi, &odata, opars, F, i, nPts);
+    if (sp->useObserver){
+        //readout features of interest and write to global F:
+        finalizeFeatures(&ti, xi, dxi, auxi, &odata, opars, F, i, nPts);
+
+        //finalize observerdata for possible continuation
+        finalizeObserverData(&ti, xi, dxi, auxi, &odata, opars, tspan);
 
-    //finalize observerdata for possible continuation
-    finalizeObserverData(&ti, xi, dxi, auxi, &odata, opars, tspan);
+        //store the observerData in global memory
+        OData[i] = odata;
+    }
 
+    nStored[i] = storeix; //storeix ranged from 0 to nStored-1
 
     //write the final solution values to global memory.
     for (int j = 0; j < N_VAR; ++j)
         xf[j * nPts + i] = xi[j];
 
     // To get same RNG on repeat (non-continued) run, need to set the seed to same value
     for (int j = 0; j < N_RNGSTATE; ++j)
         RNGstate[j * nPts + i] = rd.state[j];
-
-    OData[i] = odata;
     
-    nStored[i] = storeix; //storeix ranged from 0 to nStored-1
+    // update dt to its final value (for adaptive stepper continue)
+    d_dt[i] = dt;
 }
```

### Comparing `clode-0.7.1/clode/cpp/steppers/BUILD` & `clode-0.8.1/clode/cpp/steppers/BUILD`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/clode/cpp/steppers/adaptive_bs23.clh` & `clode-0.8.1/clode/cpp/steppers/adaptive_bs23.clh`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 // E1=B1-_C1 directly in error estimate dt*(E dot k) = xnew_B - xnewB
 #define E1 RCONST(-5.0)/RCONST(72.0)
 #define E2 RCONST(1.0)/RCONST(12.0)
 #define E3 RCONST(1.0)/RCONST(9.0)
 #define E4 RCONST(-1.0)/RCONST(8.0)
 
 //this is ode23 in matlab
-inline realtype do_step(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], const realtype dt, realtype aux[], realtype err[], const realtype wi[])
+static inline realtype do_step(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], const realtype dt, realtype aux[], realtype err[], const realtype wi[])
 {
     realtype tNew = *ti + dt;
     realtype newDt = tNew - *ti; //use the effective part of dt
     realtype xtmp[N_VAR], k2[N_VAR], k3[N_VAR], k4[N_VAR];
 
     //expects k1 to be precomputed (FSAL)
```

### Comparing `clode-0.7.1/clode/cpp/steppers/adaptive_dp45.clh` & `clode-0.8.1/clode/cpp/steppers/adaptive_dp45.clh`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 #define E1 RCONST(71.0)/RCONST(57600.0)
 #define E3 RCONST(-71.0)/RCONST(16695.0)
 #define E4 RCONST(71.0)/RCONST(1920.0)
 #define E5 RCONST(-17253.0)/RCONST(339200.0)
 #define E6 RCONST(22.0)/RCONST(525.0)
 #define E7 RCONST(-1.0)/RCONST(40.0)
 
-inline realtype do_step(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], const realtype dt, realtype aux[], realtype err[], const realtype wi[])
+static inline realtype do_step(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], const realtype dt, realtype aux[], realtype err[], const realtype wi[])
 {
     realtype tNew = *ti + dt;
     realtype newDt = tNew - *ti; //use the effective part of dt
     realtype xtmp[N_VAR], k2[N_VAR], k3[N_VAR], k4[N_VAR], k5[N_VAR], k6[N_VAR], k7[N_VAR];
     //matlab: k <-> f, x <-> y, 
 
     //expects k1 to be precomputed (FSAL)
```

### Comparing `clode-0.7.1/clode/cpp/steppers/adaptive_explicit_step.clh` & `clode-0.8.1/clode/cpp/steppers/adaptive_explicit_step.clh`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 #include "realtype.cl"
 
 #define SAFETY_FACTOR RCONST(0.8)
 // #define EXPON RCONST(1.0)/LOCAL_ERROR_ORDER  //controls error per step -> local error only; err~tol
 #define EXPON RCONST(1.0)/(LOCAL_ERROR_ORDER+RCONST(1.0))  //controls error per unit step (err/dt~tol) -> global error proportional to tol (tolerance proportional) 
 
 //Wrapper to handle step-size adaptation.  note: wi should be zeros
-inline int stepper(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], 
+static inline int stepper(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], 
 __constant struct SolverParams *sp, realtype *dt, __constant realtype *tspan, 
-realtype aux[], realtype wi[], __private rngData *rd)
+realtype aux[], realtype wi[], __private struct rngData *rd)
 {
     realtype tNew, normErr, relErr, err[N_VAR], newxi[N_VAR], newk1[N_VAR];
 
     realtype newDt = *dt;
     realtype threshold = sp->abstol / sp->reltol;
     realtype hmin = RCONST(16.0) * fabs(fabs(nextafter(*ti, RCONST(1.1)*tspan[1])) - *ti); //matches Matlab: hmin=16*eps(t)
```

### Comparing `clode-0.7.1/clode/cpp/steppers/adaptive_he12.clh` & `clode-0.8.1/clode/cpp/steppers/adaptive_he12.clh`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 #define ADAPTIVE_STEPSIZE_EXPLICIT
 #define FSAL_STEP_PROPERTY
 #define LOCAL_ERROR_ORDER RCONST(1.0)
 #define ADAPTIVE_STEP_MAX_SHRINK RCONST(0.5)
 #define ADAPTIVE_STEP_MAX_GROW RCONST(5.0)
 
-inline realtype do_step(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], const realtype dt, realtype aux[], realtype err[], const realtype wi[])
+static inline realtype do_step(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], const realtype dt, realtype aux[], realtype err[], const realtype wi[])
 {
     realtype tNew = *ti + dt;
     realtype newDt = tNew - *ti; //use the effective part of dt
     realtype xtmp[N_VAR], k2[N_VAR];
 
     //compute k1
     //getRHS(*ti, xi, pars, k1, aux, wi); //slope at *ti
```

### Comparing `clode-0.7.1/clode/cpp/steppers/adaptive_rkck.clh` & `clode-0.8.1/clode/cpp/steppers/adaptive_rkck.clh`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 #define E1 RCONST(71.0)/RCONST(57600.0)
 #define E3 RCONST(-71.0)/RCONST(16695.0)
 #define E4 RCONST(71.0)/RCONST(1920.0)
 #define E5 RCONST(-277.0)/RCONST(14336.0)
 #define E6 RCONST(22.0)/RCONST(525.0)
 #define E7 RCONST(-1.0)/RCONST(40.0)
 
-inline realtype do_step(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], const realtype dt, realtype aux[], realtype err[], const realtype wi[])
+static inline realtype do_step(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], const realtype dt, realtype aux[], realtype err[], const realtype wi[])
 {
     realtype tNew = *ti + dt;
     realtype newDt = tNew - *ti; //use the effective part of dt
     realtype xtmp[N_VAR], k2[N_VAR], k3[N_VAR], k4[N_VAR], k5[N_VAR], k6[N_VAR], k7[N_VAR];
     //matlab: k <-> f, x <-> y, 
 
     //expects k1 to be precomputed (FSAL)
```

### Comparing `clode-0.7.1/clode/cpp/steppers/fixed_explicit_Euler.clh` & `clode-0.8.1/clode/cpp/steppers/fixed_explicit_Euler.clh`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #include "realtype.cl"
 
 //Explicit (Forward) Euler
 #define FIXED_STEPSIZE_EXPLICIT
-inline void do_step(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], const realtype dt, realtype aux[], const realtype wi[])
+static inline void do_step(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], const realtype dt, realtype aux[], const realtype wi[])
 {    
     //k1 passed in
     
     //update to new ti, xi, k1: xi = fma(dt, k1[k], xi[k]);
     for (int k = 0; k < N_VAR; k++)
         xi[k] += dt * k1[k];
```

### Comparing `clode-0.7.1/clode/cpp/steppers/fixed_explicit_RK4.clh` & `clode-0.8.1/clode/cpp/steppers/fixed_explicit_RK4.clh`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #include "realtype.cl"
 
 //Explicit Runge-Kutta 4 time step
 #define FIXED_STEPSIZE_EXPLICIT
-inline void do_step(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], const realtype dt, realtype aux[], const realtype wi[])
+static inline void do_step(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], const realtype dt, realtype aux[], const realtype wi[])
 {
     realtype tmp[N_VAR], k2[N_VAR], k3[N_VAR], k4[N_VAR];
     realtype h2 = dt * RCONST(0.5);
     realtype th2 = *ti + h2;
     realtype th = *ti + dt;
 
     //k1 passed in
```

### Comparing `clode-0.7.1/clode/cpp/steppers/fixed_explicit_Trapezoidal.clh` & `clode-0.8.1/clode/cpp/steppers/fixed_explicit_Trapezoidal.clh`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #include "realtype.cl"
 
 //Explicit trapezoidal (Heun's method, improved Euler) time step
 #define FIXED_STEPSIZE_EXPLICIT
-inline void do_step(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], const realtype dt, realtype aux[], const realtype wi[])
+static inline void do_step(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], const realtype dt, realtype aux[], const realtype wi[])
 {
     realtype th = *ti + dt;
     realtype tmp[N_VAR], k2[N_VAR];
 
     //compute k1
     // getRHS(*ti, xi, pars, k1, aux, wi);
```

### Comparing `clode-0.7.1/clode/cpp/steppers/fixed_explicit_step.clh` & `clode-0.8.1/clode/cpp/steppers/fixed_explicit_step.clh`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #include "clODE_struct_defs.cl" //for SolverParams struct definition
 #include "realtype.cl"
 
-//TODO: seems like there's no need for this if we use naive time update, except to allow Wiener vars in any solver without cluttering the steppers
+// time update: Which should it be? adaptive uses:
+// realtype tNew = *ti + dt;
+// realtype newDt = tNew - *ti; //use the effective part of dt
 
 //Wrapper to handle step-size adaptation.  note: wi should be zeros
-inline int stepper(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], 
+static inline int stepper(realtype *ti, realtype xi[], realtype k1[], const realtype pars[], 
 __constant struct SolverParams *sp, realtype *dt, __constant realtype *tspan, 
-realtype aux[], realtype wi[], __private rngData *rd)
+realtype aux[], realtype wi[], __private struct rngData *rd)
 {
     // xi and ti are updated inside do_step. 
     do_step(ti, xi, k1, pars, *dt, aux, wi);
 
     // naive time update - this is the one consistent with what's in each stepper...
     // *ti += *dt;
```

### Comparing `clode-0.7.1/clode/cpp/steppers.cl` & `clode-0.8.1/clode/cpp/steppers.cl`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,20 @@
-//TODO: Force all steppers to follow FSAL? allows "free" interpolation in any timestep (important for event detection, trajectory output at specified times).
-//      if purifying ti (fixed steppers) must get new dxi in main loop.
-//TODO: Adaptive stepper seems to fail to keep stepsize small enough to prevent blowups. Something to do with abstol??
-//TODO: stepper wishlist: Multi-step method support,  implicit methods
-//TODO: does fma(a,b,c)=a*b+c for improved accuracy? vs mad? Does compiler do it anyway (if so write normal version for readability)?
-//TODO: fixed stepsize: if always purifying ti in main loop (t0+step*dt), don't update ti here?
-//TODO: test speed increases for "minimizing registers" vs reuse of computations (e.g. h2=*dt*0.5)
+// wishlist: DIRK (stiff explicit), implicit, multistep
+
+// TODO: generalize implementation via using Butcher Tableau?
+// https://en.wikipedia.org/wiki/List_of_Runge%E2%80%93Kutta_methods
+
+// TODO: options for controllers. I/PI/PID
+// - adaptive steppers should return their internal error estimate. 
+// https://docs.sciml.ai/DiffEqDocs/stable/extras/timestepping/
+
+// TODO: for methods with "free interpolants" expose them for use in observer? or is xbuffer + dxbuffer sufficient?
+
+//TODO: precision/speed tradeoffs: fma(a,b,c) vs a*b+c vs mad? compiler flags? Does compiler do it anyway (if so write normal version for readability)?
+//TODO: time summation vs dt -> loss of precision? Kahan/TwoSum? 
 
 #ifndef STEPPERS_H_
 #define STEPPERS_H_
 
 //available methods "manifest" for C++ use
 #ifdef __cplusplus 
 
@@ -40,15 +46,14 @@
 
 #include "realtype.cl"
 
 //forward declaration of the RHS function
 void getRHS(const realtype t, const realtype x_[], const realtype p_[], realtype dx_[], realtype aux_[], const realtype w_[]);
 
 // FIXED STEPSIZE EXPLICIT METHODS
-// The fixed steppers use stepcount to purify the T values (eliminates roundoff)
 
 #ifdef STOCHASTIC_EULER
 #define STOCHASTIC_STEPPER
 #include "steppers/fixed_explicit_Euler.clh"
 #endif
 
 #ifdef EXPLICIT_EULER
@@ -107,16 +112,13 @@
 //~ #ifdef RK549_KENNEDY
 //~ #endif
 
 #ifdef ADAPTIVE_STEPSIZE_EXPLICIT
 #include "steppers/adaptive_explicit_step.clh"
 #endif
 
-
-
 //TODO: implicit fixed/adaptive steppers
 
 
-
-
 #endif //__cplusplus
+
 #endif //STEPPERS_H_
```

### Comparing `clode-0.7.1/clode/cpp/trajectory.cl` & `clode-0.8.1/clode/cpp/trajectory.cl`

 * *Files 10% similar despite different names*

```diff
@@ -28,89 +28,81 @@
     int i = get_global_id(0);
     int nPts = get_global_size(0);
 
     realtype ti, dt;
     realtype p[N_PAR], xi[N_VAR], dxi[N_VAR];
     realtype auxi[N_AUX>0?N_AUX:1];
     realtype wi[N_WIENER>0?N_WIENER:1];
-    rngData rd;
+    struct rngData rd;
 
     //get private copy of ODE parameters, initial data, and compute slope at initial state
     ti = tspan[0];
-    dt = sp->dt;
+    dt = d_dt[i];
 
     for (int j = 0; j < N_PAR; ++j)
         p[j] = pars[j * nPts + i];
 
     for (int j = 0; j < N_VAR; ++j)
         xi[j] = x0[j * nPts + i];
 
     for (int j = 0; j < N_RNGSTATE; ++j)
         rd.state[j] = RNGstate[j * nPts + i];
 
+    // generate random numbers if needed
     rd.randnUselast = 0;
-
     for (int j = 0; j < N_WIENER; ++j)
 #ifdef STOCHASTIC_STEPPER
         wi[j] = randn(&rd) / sqrt(dt);
 #else
-        wi[j] = RCONST(0.0);
+        wi[j] = ZERO;
 #endif
-    getRHS(ti, xi, p, dxi, auxi, wi); //slope at initial point, needed for FSAL steppers (bs23, dorpri5) and for DX output
 
-    //store the initial point
+    //get the slope and aux at initial point
+    getRHS(ti, xi, p, dxi, auxi, wi); 
 
+    //store the initial point
     int storeix = 0;
     t[storeix * nPts + i] = ti;
     for (int j = 0; j < N_VAR; ++j)
         x[storeix * nPts * N_VAR + j * nPts + i] = xi[j];
-
     for (int j = 0; j < N_VAR; ++j)
         dx[storeix * nPts * N_VAR + j * nPts + i] = dxi[j];
-
     for (int j = 0; j < N_AUX; ++j)
         aux[storeix * nPts * N_AUX + j * nPts + i] = auxi[j];
-
-    ++storeix;
     
-    //time-stepping loop, main time interval
-    int step = 0;
+	//time-stepping loop
+    unsigned int step = 0;
     int stepflag = 0;
-    while (ti < tspan[1] && step < sp->max_steps && storeix < sp->max_store)
+    while (ti <= tspan[1] && step < sp->max_steps && storeix < sp->max_store)
     {
-        ++step;
+		++step;
         stepflag = stepper(&ti, xi, dxi, p, sp, &dt, tspan, auxi, wi, &rd);
         // if (stepflag!=0)
         //     break;
 
         //store every sp.nout'th step after the initial point
         if (step % sp->nout == 0)
         {
-
-            t[storeix * nPts + i] = ti; //adaptive steppers give different timepoints for each trajectory
-
+            ++storeix;
+            t[storeix * nPts + i] = ti;
             for (int j = 0; j < N_VAR; ++j)
                 x[storeix * nPts * N_VAR + j * nPts + i] = xi[j];
-
             for (int j = 0; j < N_VAR; ++j)
                 dx[storeix * nPts * N_VAR + j * nPts + i] = dxi[j];
-
             for (int j = 0; j < N_AUX; ++j)
                 aux[storeix * nPts * N_AUX + j * nPts + i] = auxi[j];
-                
-            ++storeix;
         }
     }
 
     nStored[i] = storeix; //storeix ranged from 0 to nStored-1
 
     //write the final solution values to global memory.
     for (int j = 0; j < N_VAR; ++j)
         xf[j * nPts + i] = xi[j];
 
     // To get same RNG on repeat (non-continued) run, need to set the seed to same value
     for (int j = 0; j < N_RNGSTATE; ++j)
         RNGstate[j * nPts + i] = rd.state[j];
 
     // update dt to its final value (for adaptive stepper continue)
-    // d_dt[i] = dt;
+    d_dt[i] = dt;
 }
```

### Comparing `clode-0.7.1/clode/cpp/transient.cl` & `clode-0.8.1/clode/cpp/transient.cl`

 * *Files 12% similar despite different names*

```diff
@@ -19,54 +19,56 @@
     int i = get_global_id(0);
     int nPts = get_global_size(0);
 
     realtype ti, dt;
     realtype p[N_PAR], xi[N_VAR], dxi[N_VAR];
     realtype auxi[N_AUX>0?N_AUX:1];
     realtype wi[N_WIENER>0?N_WIENER:1];
-    rngData rd;
+    struct rngData rd;
 
     //get private copy of ODE parameters, initial data, and compute slope at initial state
     ti = tspan[0];
-    dt = sp->dt;
+    dt = d_dt[i];
 
     for (int j = 0; j < N_PAR; ++j)
         p[j] = pars[j * nPts + i];
 
     for (int j = 0; j < N_VAR; ++j)
         xi[j] = x0[j * nPts + i];
 
     for (int j = 0; j < N_RNGSTATE; ++j)
         rd.state[j] = RNGstate[j * nPts + i];
 
+    // generate random numbers if needed
     rd.randnUselast = 0;
-
     for (int j = 0; j < N_WIENER; ++j)
 #ifdef STOCHASTIC_STEPPER
         wi[j] = randn(&rd) / sqrt(dt);
 #else
-        wi[j] = RCONST(0.0);
+        wi[j] = ZERO;
 #endif
-    getRHS(ti, xi, p, dxi, auxi, wi); //slope at initial point, needed for FSAL steppers (bs23, dorpri5)
 
-    //time-stepping loop, main time interval
-    int step = 0;
+    //get the slope and aux at initial point
+    getRHS(ti, xi, p, dxi, auxi, wi); 
+
+	//time-stepping loop
+    unsigned int step = 0;
     int stepflag = 0;
-    while (ti < tspan[1] && step < sp->max_steps)
+    while (ti <= tspan[1] && step < sp->max_steps)
     {
-        ++step;
+		++step;
         stepflag = stepper(&ti, xi, dxi, p, sp, &dt, tspan, auxi, wi, &rd);
         // if (stepflag!=0)
         //     break;
     }
 
     //write the final solution values to global memory.
     for (int j = 0; j < N_VAR; ++j)
         xf[j * nPts + i] = xi[j];
 
     // To get same RNG on repeat (non-continued) run, need to set the seed to same value
     for (int j = 0; j < N_RNGSTATE; ++j)
         RNGstate[j * nPts + i] = rd.state[j];
 
     // update dt to its final value (for adaptive stepper continue)
-    // d_dt[i] = dt;
+    d_dt[i] = dt;
 }
```

### Comparing `clode-0.7.1/clode/features.py` & `clode-0.8.1/clode/features.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,95 +1,155 @@
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import numpy as np
+from numpy.lib import recfunctions as rfn
 
-from .function_converter import OpenCLRhsEquation
-from .runtime import (
-    CLDeviceType,
-    CLVendor,
+from clode.cpp.clode_cpp_wrapper import (
     FeatureSimulatorBase,
     ObserverParams,
-    _clode_root_dir,
+    SolverParams,
 )
+
+from .function_converter import OpenCLRhsEquation
+from .runtime import CLDeviceType, CLVendor, _clode_root_dir
 from .solver import Simulator, Stepper
 
+# TODO[API]: defaults for ObserverParams are here and in wrapper. Should be only ONE place globally.
+# - Prefer the struct defaults? Create a default config?
+# TODO[API]: Observer param subsets are specific to different observers. Should model each as a class
+
 
 class Observer(Enum):
     basic = "basic"
     basic_all_variables = "basicall"
     local_max = "localmax"
     neighbourhood_1 = "nhood1"
     neighbourhood_2 = "nhood2"
     threshold_2 = "thresh2"
 
 
 # may want other functionality here.
-# - full feature matrix, with names (pandas?)
-# - separate diagnostics (period count, step count, min dt, max dt , ...), summarize on print along with observer info/pars?
+# - full feature matrix, with names [numpy sturctured arrays?]
+# - separate diagnostic features (period count, step count, min dt, max dt , ...)
 class ObserverOutput:
     def __init__(
         self,
         observer_params: ObserverParams,
-        results_array: np.ndarray[Any, np.dtype[np.float64]],
-        num_result_features: int,
+        feature_array: np.ndarray[Any, np.dtype[np.float64]],
+        num_features: int,
         variables: List[str],
         observer_type: Observer,
         feature_names: List[str],
-    ):
-        # print(type(observer_params))
+        ensemble_shape: Tuple,
+    ) -> None:
         self._op = observer_params
-        self._data = results_array
-        self._num_result_features = num_result_features
+        self._num_features = num_features
         self._vars = variables
         self._observer_type = observer_type
         self._feature_names = feature_names
+        self._ensemble_shape = ensemble_shape
 
-        shape = (
-            self._num_result_features,
-            len(results_array) // self._num_result_features,
+        # support indexing F via feature name directly
+        F_dtype = np.dtype(
+            {"names": feature_names, "formats": [np.float64] * len(feature_names)}
         )
-        self._data = results_array.reshape(shape).transpose()
+        self.F = rfn.unstructured_to_structured(feature_array, dtype=F_dtype)
+
+    def __repr__(self) -> str:
+        ensemble_size = len(self.F[self._feature_names[0]])
+        num_features = len(self._feature_names)
+        feature_names = self._feature_names
+        return f"ObserverOutput( ensemble size: {ensemble_size}, number of features: {num_features}, feature_names: {feature_names})"
+
+    def to_ndarray(self, **kwargs):
+        return rfn.structured_to_unstructured(self.F, **kwargs)
 
     def get_feature_names(self) -> List[str]:
         return self._feature_names
 
-    def _get_var(self, var: str, op: str) -> np.ndarray[Any, np.dtype[np.float64]]:
+    def _get_var(self, var: str) -> np.ndarray[Any, np.dtype[np.float64]]:
         try:
-            index = self._feature_names.index(f"{op} {var}")
-            return self._data[:, index : index + 1].squeeze()
+            result = self.F[var].squeeze().reshape(self._ensemble_shape)
+            result = result[0] if result.size == 1 else result
+            return result
         except ValueError:
-            raise NotImplementedError(
-                f"{self._observer_type} does not track {op} {var}!"
-            )
+            raise NotImplementedError(f"{self._observer_type} does not track {var}!")
 
     def get_var_max(self, var: str) -> np.ndarray[Any, np.dtype[np.float64]]:
-        return self._get_var(var, "max")
+        return self._get_var(" ".join(["max", var]))
 
     def get_var_min(self, var: str) -> np.ndarray[Any, np.dtype[np.float64]]:
-        return self._get_var(var, "min")
+        return self._get_var(" ".join(["min", var]))
 
     def get_var_mean(self, var: str) -> np.ndarray[Any, np.dtype[np.float64]]:
-        return self._get_var(var, "mean")
+        return self._get_var(" ".join(["mean", var]))
 
-    def get_var_max_dt(self, var: str) -> np.ndarray[Any, np.dtype[np.float64]]:
+    def get_var_max_slope(self, var: str) -> np.ndarray[Any, np.dtype[np.float64]]:
         return self.get_var_max(f"d{var}/dt")
 
-    def get_var_min_dt(self, var: str) -> np.ndarray[Any, np.dtype[np.float64]]:
+    def get_var_min_slope(self, var: str) -> np.ndarray[Any, np.dtype[np.float64]]:
         return self.get_var_min(f"d{var}/dt")
 
     def get_var_count(self, var: str) -> np.ndarray[Any, np.dtype[np.float64]]:
-        return self._get_var("count", var)
+        return self._get_var(" ".join([var, "count"]))
+
+    def get_event_data(
+        self, name: str, type: Optional[str] = "time"
+    ) -> np.ndarray[Any, np.dtype[np.float64]]:
+        # event data feature names have format: "{name} event {time/var} {event idx}"
+        # name - distinguish event types (up/down, localmax/localmin) in some observers, others (nhood2) just track single type
+        # type - use to extract event time or event var [e.g., var = eVar value at event time]
+        #
+        # return: for now, force user to specify one name that makes sense, optionally type
+        event_features = [
+            feature_name
+            for feature_name in self._feature_names
+            if name in feature_name
+            and "event" in feature_name
+            and "count" not in feature_name
+        ]
+        if len(event_features) == 0:
+            raise NotImplementedError(
+                f"{self._observer_type} does not track {name} event {type}s!"
+            )
+        data = []
+        for event_idx in range(0, self._op.max_event_timestamps):
+            datapoint = self._get_var(f"{name} event {type} {event_idx}")
+            if np.all(datapoint == 0):
+                break
+            data.append(datapoint)
+        return np.stack(data, axis=-1).squeeze()
+
+    # TODO deprecate function
+    def get_timestamps(
+        self, var: str = "event"
+    ) -> np.ndarray[Any, np.dtype[np.float64]]:
+        first_key = f"{var} event time 0"
+        if first_key not in self._feature_names:
+            raise NotImplementedError(
+                f"{self._observer_type} does not track {var} event times!"
+            )
+        data = []
+        for key_idx in range(0, self._op.max_event_timestamps):
+            datapoint = self._get_var(f"{var} event time {key_idx}")
+            if np.all(datapoint == 0):
+                break
+            datapoint = (
+                datapoint[np.newaxis] if len(datapoint.shape) == 0 else datapoint
+            )
+            data.append(datapoint)
+        return np.stack(data, axis=1).squeeze() if data else []
 
 
+# TODO[mkdocs] - make consistent
 class FeatureSimulator(Simulator):
-    """
-    A class for computing features from a CLODE model.
+    """Simulator class that stores trajectory features, computed on-the-fly
 
     Parameters
     ----------
     src_file : str
         Path to the CLODE model source file.
     variable_names : List[str]
         List of variable names in the model.
@@ -122,15 +182,15 @@
         upper threshold, by default 0
     observer_dx_down_thresh : float, optional
         Threshold for detecting an event when the feature variable crosses the
         lower threshold, by default 0
     observer_eps_dx : float, optional
         Threshold for detecting an event when the feature variable crosses the
         lower threshold, by default 1e-7
-    tspan : tuple[float, float], optional
+    t_span : tuple[float, float], optional
         Time span for the simulation, by default (0.0, 1000.0)
     stepper : Stepper, optional
         Stepper to use for the simulation, by default Stepper.euler
     single_precision : bool, optional
         Whether to use single precision for the simulation, by default False
     dt : float, optional
         Time step for the simulation, by default 0.1
@@ -209,76 +269,85 @@
     ... )
     >>> model.set_parameter_values({"F": 8.0})
     >>> model.set_initial_values({"x": np.random.rand(40)})
     >>> model.simulate()
     >>> model.plot()
     >>> plt.show()"""
 
+    _device_features: np.ndarray[Any, np.dtype[np.float64]] | None
     _integrator: FeatureSimulatorBase
 
     def __init__(
         self,
         variables: Dict[str, float],
         parameters: Dict[str, float],
+        aux: Optional[List[str]] = None,
+        num_noise: int = 0,
         src_file: Optional[str] = None,
         rhs_equation: Optional[OpenCLRhsEquation] = None,
         supplementary_equations: Optional[List[Callable[[Any], Any]]] = None,
-        aux: Optional[List[str]] = None,
-        num_noise: int = 0,
-        t_span: Tuple[float, float] = (0.0, 1000.0),
         stepper: Stepper = Stepper.rk4,
-        observer: Observer = Observer.basic_all_variables,
-        single_precision: bool = True,
         dt: float = 0.1,
         dtmax: float = 1.0,
         abstol: float = 1e-6,
         reltol: float = 1e-3,
         max_steps: int = 10000000,
         max_store: int = 10000000,
         nout: int = 1,
-        device_type: CLDeviceType | None = None,
-        vendor: CLVendor | None = None,
-        platform_id: int | None = None,
-        device_id: int | None = None,
-        device_ids: List[int] | None = None,
+        solver_parameters: Optional[SolverParams] = None,
+        t_span: Tuple[float, float] = (0.0, 1000.0),
+        single_precision: bool = True,
+        device_type: Optional[CLDeviceType] = None,
+        vendor: Optional[CLVendor] = None,
+        platform_id: Optional[int] = None,
+        device_id: Optional[int] = None,
+        device_ids: Optional[List[int]] = None,
+        observer: Observer = Observer.basic_all_variables,
         event_var: str = "",
         feature_var: str = "",
-        observer_max_event_count: int = 100,
+        observer_max_event_count: int = 100,  # TODO: defaults are set in two places - here and ObserverParam wrapper
+        observer_max_event_timestamps: int = 0,
         observer_min_x_amp: float = 0.0,
         observer_min_imi: float = 0.0,
         observer_neighbourhood_radius: float = 0.05,
         observer_x_up_thresh: float = 0.3,
         observer_x_down_thresh: float = 0.2,
         observer_dx_up_thresh: float = 0,
         observer_dx_down_thresh: float = 0,
         observer_eps_dx: float = 0.0,
+        observer_parameters: Optional[ObserverParams] = None,
     ) -> None:
 
         self._observer_type = observer
 
         event_var_idx = (
             list(variables.keys()).index(event_var) if event_var != "" else 0
         )
         feature_var_idx = (
             list(variables.keys()).index(feature_var) if feature_var != "" else 0
         )
 
-        self._op = ObserverParams(
-            event_var_idx,
-            feature_var_idx,
-            observer_max_event_count,
-            observer_min_x_amp,
-            observer_min_imi,
-            observer_neighbourhood_radius,
-            observer_x_up_thresh,
-            observer_x_down_thresh,
-            observer_dx_up_thresh,
-            observer_dx_down_thresh,
-            observer_eps_dx,
-        )
+        # can't sync yet because observer_max_event_timestamps is needed for building cl program.
+        if observer_parameters is not None:
+            self._op = observer_parameters
+        else:
+            self._op = ObserverParams(
+                event_var_idx,
+                feature_var_idx,
+                observer_max_event_count,
+                observer_max_event_timestamps,
+                observer_min_x_amp,
+                observer_min_imi,
+                observer_neighbourhood_radius,
+                observer_x_up_thresh,
+                observer_x_down_thresh,
+                observer_dx_up_thresh,
+                observer_dx_down_thresh,
+                observer_eps_dx,
+            )
 
         super().__init__(
             variables=variables,
             parameters=parameters,
             src_file=src_file,
             rhs_equation=rhs_equation,
             supplementary_equations=supplementary_equations,
@@ -290,74 +359,168 @@
             dt=dt,
             dtmax=dtmax,
             abstol=abstol,
             reltol=reltol,
             max_steps=max_steps,
             max_store=max_store,
             nout=nout,
+            solver_parameters=solver_parameters,
             device_type=device_type,
             vendor=vendor,
             platform_id=platform_id,
             device_id=device_id,
             device_ids=device_ids,
         )
+        # op could come after super_init if max_event_timestamps treated like trajectory max_store
 
-    def _build_integrator(self) -> None:
+    def _create_integrator(self) -> None:
         self._integrator = FeatureSimulatorBase(
             self._pi,
             self._stepper.value,
             self._observer_type.value,
+            self._op,  # remove from constructor & add set_observer_pars below.
             self._single_precision,
             self._runtime,
             _clode_root_dir,
         )
+        # self.set_observer_parameters()
 
-    def _init_integrator(self) -> None:
-        vars_array, pars_array = self._pack_data()
-        self._integrator.initialize(
-            self.tspan,
-            vars_array,
-            pars_array,
-            self._sp,
-            self._op,
-        )
+    def set_observer(self, observer_type: Observer):
+        """Change the observer"""
+        if observer_type != self._observer_type:
+            self._integrator.set_observer(observer_type)
+            self._cl_program_is_valid = False
+
+    # Changing solver parameters does not require re-building CL program
+    def set_observer_parameters(
+        self,
+        op: Optional[ObserverParams] = None,
+        event_var: Optional[str] = None,
+        feature_var: Optional[str] = None,
+        max_event_count: Optional[int] = None,
+        max_event_timestamps: Optional[
+            int
+        ] = None,  # NOTE! Changing this invalidates the CL program!!
+        min_amp: Optional[float] = None,
+        min_imi: Optional[float] = None,
+        nhood_radius: Optional[float] = None,
+        x_up_threshold: Optional[float] = None,
+        x_down_threshold: Optional[float] = None,
+        dx_up_threshold: Optional[float] = None,
+        dx_down_threshold: Optional[float] = None,
+        eps_dx: Optional[float] = None,
+    ) -> None:
+        """Update any of the solver parameters and push to device
+
+        Args:
+            parameters (np.array): The parameters.
+
+        Returns:
+            None
+        """
+        if op is not None:
+            self._op = op
+        else:
+            if event_var is not None:
+                self._op.e_var_ix = self.variable_names.index(event_var)
+            if feature_var is not None:
+                self._op.f_var_ix = self.variable_names.index(feature_var)
+            if max_event_count is not None:
+                self._op.max_event_count = max_event_count
+            if max_event_timestamps is not None:
+                if self._op.max_event_timestamps != max_event_timestamps:
+                    self._cl_program_is_valid = False  # NOTE! Changing max_event_timestamps invalidates the CL program!!
+                self._op.max_event_timestamps = max_event_timestamps
+            if min_amp is not None:
+                self._op.min_amp = min_amp
+            if min_imi is not None:
+                self._op.min_imi = min_imi
+            if nhood_radius is not None:
+                self._op.nhood_radius = nhood_radius
+            if x_up_threshold is not None:
+                self._op.x_up_threshold = x_up_threshold
+            if x_down_threshold is not None:
+                self._op.x_down_threshold = x_down_threshold
+            if dx_up_threshold is not None:
+                self._op.dx_up_threshold = dx_up_threshold
+            if dx_down_threshold is not None:
+                self._op.dx_down_threshold = dx_down_threshold
+            if eps_dx is not None:
+                self._op.eps_dx = eps_dx
+        self._integrator.set_observer_params(self._op)
+
+    def get_observer_parameters(self):
+        """Get the current observer parameter struct"""
+        return self._integrator.get_observer_params()
 
     def get_feature_names(self) -> List[str]:
+        """Get the list of feature names for the current observer"""
         return self._integrator.get_feature_names()
 
     def features(
-        self, initialize_observer: Optional[bool] = None, update_x0: bool = True
-    ) -> ObserverOutput:
+        self,
+        t_span: Optional[Tuple[float, float]] = None,
+        initialize_observer: Optional[bool] = None,
+        update_x0: bool = True,
+        fetch_results: bool = True,
+    ) -> Optional[ObserverOutput]:
         """Run a simulation with feature detection.
 
+        Args:
+        t_span (tuple[float, float]): Time interval for integration.
+        initialize_observer (bool): Whether the observer data be initialized
+        update_x0 (bool): After the simulation, whether to overwrite the initial state buffer with the final state
+        fetch_results (bool): Whether to fetch the feature results from the device and return them here
+
         Returns:
-            None
+            ObserverOutput | None
         """
-        if not self.is_initialized:
-            raise RuntimeError("Simulator is not initialized")
+        # if not self._cl_program_is_valid:
+        #     self._integrator.build_cl()
+        #     self._cl_program_is_valid = True
+
+        if t_span is not None:
+            self.set_tspan(t_span=t_span)
 
         if initialize_observer is not None:
-            print("Reinitializing observer")
+            print(f"Setting {initialize_observer=}")
             self._integrator.features(initialize_observer)
         else:
             self._integrator.features()
+        # invalidate _device_features
+        # invalidate _device_final_state
+
         if update_x0:
-            self.shift_x0()
+            self._integrator.shift_x0()
+            # invalidate _device_initial_state
 
-        return self.get_observer_results()
+        if fetch_results:
+            return self.get_observer_results()
 
     def get_observer_results(self) -> ObserverOutput:
-        """Get the feature data.
+        """Get the features measured by the observer
 
         Returns:
-            np.array: The feature data.
+            ObserverOutput: object containing features that summarize trajectories
         """
-        self._result_integrator = self._integrator.get_f()
-        self._num_result_features = self._integrator.get_n_features()
+        self._device_features = self._integrator.get_f()
+        self._num_features = self._integrator.get_n_features()
+
+        if self._num_features is None:
+            raise ValueError("Must run trajectory() before getting trajectory data")
+        elif self._device_features is None:
+            raise ValueError("Must run trajectory() before getting trajectory data")
+
+        shape = (self._ensemble_size, self._num_features)
+        self._device_features = np.array(
+            self._device_features[: np.prod(shape)]
+        ).reshape(shape, order="F")
+
         return ObserverOutput(
             self._op,
-            np.array(self._result_integrator),
-            self._num_result_features,
+            self._device_features,
+            self._num_features,
             self.variable_names,
             self._observer_type,
             self._integrator.get_feature_names(),
+            self._ensemble_shape,
         )
```

### Comparing `clode-0.7.1/clode/function_converter.py` & `clode-0.8.1/clode/function_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     "floor": OpenCLBuiltin(1, "floor", OpenCLType("realtype")),
     # "fma": OpenCLBuiltin(3, "fma", OpenCLType("realtype")), # OpenCL returns nan
     "max": OpenCLBuiltin(2, "fmax", OpenCLType("realtype")),
     "min": OpenCLBuiltin(2, "fmin", OpenCLType("realtype")),
     "mod": OpenCLBuiltin(2, "fmod", OpenCLType("realtype")),
     # "fract": OpenCLBuiltin(1, "fract", OpenCLType("realtype")), # OpenCL Compiler error
     # "frexp": OpenCLBuiltin(2, "frexp", OpenCLType("realtype")),
+    "heaviside": OpenCLBuiltin(1, "heaviside", OpenCLType("realtype")),
     "hypot": OpenCLBuiltin(2, "hypot", OpenCLType("realtype")),
     "ilogb": OpenCLBuiltin(1, "ilogb", OpenCLType("int")),
     "ldexp": OpenCLBuiltin(2, "ldexp", OpenCLType("realtype")),
     "lgamma": OpenCLBuiltin(1, "lgamma", OpenCLType("realtype")),
     # "lgamma_r": OpenCLBuiltin(2, "lgamma_r", OpenCLType("realtype")), # Pointers not supported
     "log": OpenCLBuiltin(1, "log", OpenCLType("realtype")),
     "log2": OpenCLBuiltin(1, "log2", OpenCLType("realtype")),
@@ -808,15 +809,15 @@
 
 
 class OpenCLConverter(ast.NodeTransformer):
     syntax_tree: OpenCLSyntaxTree
     mutable_args: Optional[Union[List[str], List[int]]] = None
     function_name: Optional[str] = None
 
-    def __init__(self, entry_function_name: str = "get_rhs"):
+    def __init__(self, entry_function_name: str = "getRHS"):
         # Initialize any necessary variables
         self.entry_function_name = entry_function_name
         self.syntax_tree = OpenCLSyntaxTree()
 
     def visit_FunctionDef(self, node: ast.FunctionDef) -> ast.FunctionDef:
         # Change the function signature for OpenCL kernel
         # For example, change 'def' to '__kernel void'
```

### Comparing `clode-0.7.1/clode/opencl_builtins.py` & `clode-0.8.1/clode/opencl_builtins.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,18 @@
 #     return x - floor(x)
 
 
 def ilogb(x: float) -> int:
     return int(log2(x))
 
 
+def heaviside(x: float) -> float:
+    return 1.0 if x >= 0.0 else 0.0
+
+
 # OpenCL returns nan
 # def logb(x: float) -> float:
 #     if x == 0:
 #         return float("-inf")  # Return negative infinity for 0
 #     else:
 #         return log2(abs(x))
 
@@ -158,14 +162,15 @@
     "fabs",
     "fdim",
     "floor",
     # "fma",
     "fmod",
     # "fract",
     "gamma",
+    "heaviside",
     "hypot",
     "ilogb",
     "ldexp",
     "lgamma",
     "log",
     "log1p",
     "log2",
```

### Comparing `clode-0.7.1/clode/runtime.py` & `clode-0.8.1/clode/runtime.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,91 @@
 from __future__ import annotations
 
 import os
 
-from clode.cpp import clode_cpp_wrapper as _clode
 from clode.cpp.clode_cpp_wrapper import (
-    FeatureSimulatorBase,
+    CLDeviceType,
+    CLVendor,
+    DeviceInfo,
     LogLevel,
-    ObserverParams,
     OpenCLResource,
-    SimulatorBase,
-    TrajectorySimulatorBase,
-    print_opencl,
+    PlatformInfo,
+    _print_opencl,
+    get_logger,
     query_opencl,
 )
 
 _clode_root_dir: str = os.path.join(os.path.dirname(__file__), "cpp", "")
 
-DEFAULT_LOG_LEVEL = _clode.LogLevel.warn
+DEFAULT_LOG_LEVEL = LogLevel.warn
 
 
 def initialize_runtime(
-    device_type: _clode.CLDeviceType | None,
-    vendor: _clode.CLVendor | None,
+    device_type: CLDeviceType | None,
+    vendor: CLVendor | None,
     platform_id: int | None,
     device_id: int | None,
     device_ids: list[int] | None,
 ) -> OpenCLResource:
     if platform_id is not None:
         if device_type is not None:
             raise ValueError("Cannot specify device_type when platform_id is specified")
         if vendor is not None:
             raise ValueError("Cannot specify vendor when platform_id is specified")
         if device_id is not None and device_ids is not None:
             raise ValueError("Cannot specify both device_id and device_ids")
         if device_id is None and device_ids is None:
             raise ValueError("Must specify one of device_id and device_ids")
         if device_id is not None:
-            return _clode.OpenCLResource(platform_id, device_id)
+            return OpenCLResource(platform_id, device_id)
         if device_ids is not None:
-            return _clode.OpenCLResource(platform_id, device_ids)
+            return OpenCLResource(platform_id, device_ids)
         raise ValueError("Must specify one of device_id and device_ids")
     elif device_id is not None:
         raise ValueError("Must specify platform_id when specifying device_id")
     elif device_ids is not None:
         raise ValueError("Must specify platform_id when specifying device_ids")
     else:
         if device_type is None:
-            device_type = _clode.CLDeviceType.DEVICE_TYPE_DEFAULT
+            device_type = CLDeviceType.DEVICE_TYPE_DEFAULT
         if vendor is None:
-            vendor = _clode.CLVendor.VENDOR_ANY
-        return _clode.OpenCLResource(device_type, vendor)
-
-
-CLDeviceType = _clode.CLDeviceType
-CLVendor = _clode.CLVendor
-ProblemInfo = _clode.ProblemInfo
-SolverParams = _clode.SolverParams
+            vendor = CLVendor.VENDOR_ANY
+        return OpenCLResource(device_type, vendor)
 
 
 def get_log_level() -> LogLevel:
-    return _clode.get_logger().get_log_level()
+    return get_logger().get_log_level()
 
 
 def set_log_level(level: LogLevel) -> None:
-    _clode.get_logger().set_log_level(level)
+    get_logger().set_log_level(level)
 
 
 def set_log_pattern(pattern: str) -> None:
-    _clode.get_logger().set_log_pattern(pattern)
+    get_logger().set_log_pattern(pattern)
 
 
 set_log_level(DEFAULT_LOG_LEVEL)
 
+
+def print_opencl():
+    old_level = get_log_level()
+    set_log_level(LogLevel.info)
+    _print_opencl()
+    set_log_level(old_level)
+
+
 __all__ = [
     "CLDeviceType",
     "CLVendor",
-    "DEFAULT_LOG_LEVEL",
-    "get_log_level",
+    "DeviceInfo",
+    "PlatformInfo",
+    "OpenCLResource",
     "initialize_runtime",
+    "print_opencl",
+    "query_opencl",
+    "DEFAULT_LOG_LEVEL",
     "LogLevel",
     "set_log_level",
     "set_log_pattern",
-    "ProblemInfo",
-    "SolverParams",
-    "ObserverParams",
-    "SimulatorBase",
-    "OpenCLResource",
-    "FeatureSimulatorBase",
-    "TrajectorySimulatorBase",
-    "print_opencl",
-    "query_opencl",
+    "get_log_level",
 ]
```

### Comparing `clode-0.7.1/clode/xpp_parser.py` & `clode-0.8.1/clode/xpp_parser.py`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/clode.egg-info/PKG-INFO` & `clode-0.8.1/clode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clode
-Version: 0.7.1
+Version: 0.8.1
 Summary: A Python package for solving ordinary differential equations on the GPU using OpenCL
 Author-email: Patrick Fletcher <patrick.allen.fletcher@gmail.com>
 Maintainer-email: Patrick Fletcher <patrick.allen.fletcher@gmail.com>, Wolf Byttner <wolf@byttner.org>
 Project-URL: Documentation, https://patrickfletcher.github.io/clODE/
 Project-URL: Repository, https://github.com/patrickfletcher/clODE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `clode-0.7.1/clode.egg-info/SOURCES.txt` & `clode-0.8.1/clode.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -115,28 +115,35 @@
 docs/fast_and_slow_variables.md
 docs/feature_extraction.md
 docs/getting_started.md
 docs/init_runtime.md
 docs/install.md
 docs/logging_levels.md
 docs/matlab.md
+docs/observers.md
 docs/pycon.py
 docs/querying_opencl.md
 docs/specifying_odes.md
 docs/spike_counting.md
 docs/spike_counting.png
 docs/spike_counting_trajectories.png
 docs/trajectory_simulation.md
 docs/xpp_files.md
 examples/Ornstein_Uhlenbeck.py
 examples/chay_keizer.cl
 examples/dump_device_performance.py
 examples/dump_opencl_info.py
 examples/fast_and_slow.py
+examples/find_steady_states.py
+examples/observe_sine_curve.py
+examples/phase_response_curve.py
 examples/spike_counting.py
+examples/visualize_events_localmax.py
+examples/visualize_events_nhood2.py
+examples/visualize_events_threshold2.py
 matlab/BUILD
 matlab/Chart.m
 matlab/GridSimulation.m
 matlab/InitialValueProblem.m
 matlab/README.md
 matlab/clODE.m
 matlab/clODEfeatures.m
@@ -158,46 +165,46 @@
 matlab/plot_twopar.m
 matlab/queryOpenCL.cpp
 matlab/trajectoryfigure.m
 paper/paper.bib
 paper/paper.md
 samples/BUILD
 samples/Makefile
-samples/lacto_more_vars.cl
 samples/lactotroph.cl
 samples/lactotroph.ode
 samples/lactotroph_noise.cl
 samples/lactotroph_noise.ode
 samples/listOpenCL.cpp
 samples/plot_twopar.m
 samples/run_twopar.m
 samples/test.cl
 samples/testCLODE.m
 samples/testCLODEfeatures.m
 samples/testCLODEmex.m
 samples/testCLODEtrajectory.m
 samples/testFeatures.cpp
-samples/testFeatures_morevars.cpp
 samples/testTrajectory.cpp
 samples/testTransient.cpp
 samples/test_outputs_cpp.md
 samples/windowsCompileListOpenCL.txt
 test/BUILD
 test/__init__.py
 test/lorenz.cl
 test/ornl_thompson_a1.cl
-test/test.cl
-test/test_convert_python_to_opencl.py
+test/test_clODE_utilities.py
+test/test_features.py
+test/test_function_converter.py
 test/test_logger.py
 test/test_observers.py
 test/test_opencl_builtins.py
 test/test_ornl_thompson_a1.py
-test/test_pituitary.py
-test/test_print_runtime.py
 test/test_runtime.py
+test/test_solver.py
+test/test_trajectory.py
 test/test_vdp.py
 test/test_vdp_long.py
-test/test_xpp_converter.py
+test/test_xpp_parser.py
+test/tests.md
 test/van_der_pol_oscillator.cl
 test/xpp/.gitignore
 test/xpp/van_der_pol_oscillator.xpp
 test/xpp/van_der_pol_oscillator_reference.cl
```

### Comparing `clode-0.7.1/docs/LICENSE.md` & `clode-0.8.1/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/docs/Ornstein-Uhlenbeck_process.md` & `clode-0.8.1/docs/Ornstein-Uhlenbeck_process.md`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/docs/Ornstein-Uhlenbeck_process.png` & `clode-0.8.1/docs/Ornstein-Uhlenbeck_process.png`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/docs/README.md` & `clode-0.8.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/docs/fast_and_slow_variables.md` & `clode-0.8.1/docs/fast_and_slow_variables.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,27 +43,27 @@
 ensemble_parameters = {"current": np.arange(0.0, 0.6, 0.1)}
 
 simulator.set_ensemble(parameters=ensemble_parameters)
 
 trajectories = simulator.trajectory()
 
 plt.figure(figsize=(8, 6))
-for index in range(len(trajectories)):
+for index, trajectory in enumerate(trajectories):
     label = f"I={ensemble_parameters['current'][index]:.1f}"
-    plt.plot(trajectories[index].x[:, 0], trajectories[index].x[:, 1], label=label)
+    plt.plot(trajectory.x["V"], trajectory.x["w"], label=label)
 plt.xlabel("V")
 plt.ylabel("w")
 plt.legend()
 plt.title("FitzHugh-Nagumo phase plane")
 plt.show()
 
 # Plot the time series
 plt.figure(figsize=(8, 6))
 for index in range(0, len(trajectories), 2):
     label = f"I={ensemble_parameters['current'][index]}"
-    plt.plot(trajectories[index].t, trajectories[index].x[:, 0], label=label)
+    plt.plot(trajectories[index].t, trajectories[index].x["V"], label=label)
 plt.xlabel("t")
 plt.ylabel("V")
 plt.legend()
 plt.title("FitzHugh-Nagumo time series")
 plt.show()
 ```
```

### Comparing `clode-0.7.1/docs/feature_extraction.md` & `clode-0.8.1/docs/feature_extraction.md`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/docs/getting_started.md` & `clode-0.8.1/docs/getting_started.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 functions to OpenCL code. This code is then executed on an OpenCL device, such
 as a GPU or a multi-core CPU.
 
 ## Usage Example - computing the period of the Van der Pol oscillator
 
 [The Van der Pol oscillator](https://en.wikipedia.org/wiki/Van_der_Pol_oscillator) can be written as a system of two differential equations:
 
-$
+$$
 \dot{x} = y\\
 \dot{y} = \mu(1-x^2)y - x
-$
+$$
 
 Oscillations occur when $\mu>0$. Suppose we wish to measure the period of oscillations as $\mu$ varies.
 First, we will need to implement the vector field above as function -
 the right-hand-side (RHS) function - with the signature expected by clODE:
 
 ```python
 def van_der_pol(float t,
@@ -169,41 +169,28 @@
 integrator.set_ensemble(x0, P0)
 
 # Run the simulation for tspan time, storing only the final state.
 # Useful for integrating past transient behavior
 integrator.transient()
 
 # Continue the simulation, now storing the trajectories
-integrator.trajectory()
-
-# get the results, and plot
-trajectories = integrator.get_trajectory()
+trajectories = integrator.trajectory()
 
 # plot
-varix = 0
 fig, ax = plt.subplots(4, 1, sharex=True, sharey=True)
 
 for i, trajectory in enumerate(trajectories):
-    ax[i].plot(trajectory["t"], trajectory["X"][:, varix])
+    ax[i].plot(trajectory["t"], trajectory.x['x'])
 
 ax[1].set_ylabel('x')
 ax[-1].set_xlabel('time')
 plt.show()
 ```
 
 ## Implementation details
 
 The Python library wraps a CPP library, clode_cpp_wrapper.[so|dll]
 The CPP library assumes that the variables/parameters are grouped
 by columns, i.e. if your variables are a, b and c,
 the CPP library expects data in the format [aaaabbbbcccc].
 The Python library expects data in the format
 [[a, b, c], [a, b, c], [a, b, c], ...]
-
-```py run
-import matplotlib.pyplot as plt
-
-plt.plot([1,2,3,4], [1,4,9,16])
-plt.show()
-plt.plot([1, 3, 5, 7], [2, 3, 4, 5])
-plt.show()
-```
```

### Comparing `clode-0.7.1/docs/init_runtime.md` & `clode-0.8.1/docs/init_runtime.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # (Advanced) Initialize runtimes
 
 Each CLODEFeature and CLODETrajectory object
 maintains its own OpenCL runtime. This is so
 that users can initialize multiple runtimes
 across different devices.
 
-## Automatic initialisation
+## Automatic initialization
 
 The simplest way to initialize the clODE runtime is to call
 CLODEFeatures and CLODETrajectory without any runtime-specific
 arguments. The runtime device and vendor will be selected
 automatically.
 
 The default runtime device is cl_device_type.DEVICE_TYPE_DEFAULT.
```

### Comparing `clode-0.7.1/docs/install.md` & `clode-0.8.1/docs/install.md`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/docs/logging_levels.md` & `clode-0.8.1/docs/logging_levels.md`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/docs/matlab.md` & `clode-0.8.1/docs/matlab.md`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/docs/pycon.py` & `clode-0.8.1/docs/pycon.py`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/docs/querying_opencl.md` & `clode-0.8.1/docs/querying_opencl.md`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/docs/specifying_odes.md` & `clode-0.8.1/docs/specifying_odes.md`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/docs/spike_counting.md` & `clode-0.8.1/docs/spike_counting.md`

 * *Files 2% similar despite different names*

```diff
@@ -137,24 +137,22 @@
 
 traj_parameters = {"gca":points[:, 0], "kpmca": points[:, 1]}
 
 integrator_traj.set_ensemble(parameters = traj_parameters)
 
 integrator_traj.transient()
 integrator_traj.set_tspan((0.0, 10000.0))
-integrator_traj.trajectory()
-
-trajectories = integrator_traj.get_trajectory()
+trajectories = integrator_traj.trajectory()
 
 fig, ax = plt.subplots(4, 1, sharex=True, sharey=True)
 for i, trajectory in enumerate(trajectories):
-    ax[i].plot(trajectory.t / 1000.0, trajectory.x[:, 0])
+    ax[i].plot(trajectory.t / 1000.0, trajectory.x["v"])
 
 ax[1].set_ylabel("v")
-ax[-1].set_xlabel('time (s)')
+ax[-1].set_xlabel("time (s)")
 plt.show()
 ```
 
 ## Output
 
 The spike counting diagram shows silent, spiking, and bursting regions. Chaotic dynamics occur near some of the spike-adding bifurcation boundaries (yellow indicates >=12 spikes per event, as detected with the threshold observer method). The trajectories associated with the numbered points are shown in the following figure.
```

### Comparing `clode-0.7.1/docs/spike_counting.png` & `clode-0.8.1/docs/spike_counting.png`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/docs/spike_counting_trajectories.png` & `clode-0.8.1/docs/spike_counting_trajectories.png`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/docs/trajectory_simulation.md` & `clode-0.8.1/docs/trajectory_simulation.md`

 * *Files 21% similar despite different names*

```diff
@@ -52,25 +52,25 @@
 simulator.set_ensemble(parameters=ensemble_parameters)
 
 trajectories = simulator.trajectory()
 
 plt.figure(figsize=(8, 6))
 for index in range(len(trajectories)):
     label = f"I={ensemble_parameters['current'][index]:.1f}"
-    plt.plot(trajectories[index].x[:, 0], trajectories[index].x[:, 1], label=label)
+    plt.plot(trajectories[index].x["V"], trajectories[index].x["w"], label=label)
 plt.xlabel("V")
 plt.ylabel("w")
 plt.legend()
 plt.title("FitzHugh-Nagumo phase plane")
 plt.show()
 
 # Plot the time series
 plt.figure(figsize=(8, 6))
 for index in range(0, len(trajectories), 2):
     label = f"I={ensemble_parameters['current'][index]}"
-    plt.plot(trajectories[index].t, trajectories[index].x[:, 0], label=label)
+    plt.plot(trajectories[index].t, trajectories[index].x["V"], label=label)
 plt.xlabel("t")
 plt.ylabel("V")
 plt.legend()
 plt.title("FitzHugh-Nagumo time series")
 plt.show()
 ```
```

### Comparing `clode-0.7.1/docs/xpp_files.md` & `clode-0.8.1/docs/xpp_files.md`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/examples/Ornstein_Uhlenbeck.py` & `clode-0.8.1/examples/Ornstein_Uhlenbeck.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     num_noise=1,
     stepper=clode.Stepper.stochastic_euler,
     single_precision=True,
     t_span=t_span,
     dt=0.001,
 )
 
-# set up the ensemble of Wiener processes with identical parameters and initial conditions
-# Any parameters or initial conditions that are not specified will be set to the default values
+# set up the ensemble of Wiener processes with identical parameters and initial state
+# Any parameters or initial state that are not specified will be set to the default values
 nPts = 8192
 integrator.set_repeat_ensemble(nPts)
 
 integrator.transient()
 
 XF = integrator.get_final_state()
```

### Comparing `clode-0.7.1/examples/chay_keizer.cl` & `clode-0.8.1/examples/chay_keizer.cl`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/examples/dump_device_performance.py` & `clode-0.8.1/examples/dump_device_performance.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,99 +1,105 @@
-import numpy as np
-import clode
-import time
+''' Benchmark: Time for solution of Lorenz system, 1000 steps of RK4
+
+    For now tests only "transient" with no intermediate storage.
+    TODO: test with trajectory and observers
+'''
+
 from typing import List
+import time
+import numpy as np
 import matplotlib.pyplot as plt
+import clode
 
 def lorenz(
     t: float,
     var: List[float],
     par: List[float],
     dvar: List[float],
     aux: List[float],
     wiener: List[float],
 ) -> None:
     x: float = var[0]
     y: float = var[1]
     z: float = var[2]
-    
+
     r: float = par[0]
     s: float = par[1]
     beta: float = par[2]
 
     dx: float = s*(y - x)
     dy: float = r*x - y - x*z
     dz: float = x*y - beta*z
     dvar[0] = dx
     dvar[1] = dy
     dvar[2] = dz
 
 def test_lorenz_rk4(platform_id, device_id, num_pts, reps):
-    
+
     parameters = {"r": 27.0, "s": 10.0, "beta": 8.0/3.0}
     variables = {"x": 1.0, "y": 1.0, "z": 1.0}
-    
+
     t_span = (0.0, 10.0)
 
-    src_file = "test/lorenz.cl"
+    # src_file = "test/lorenz.cl"
     integrator = clode.Simulator(
         # src_file=src_file,
         rhs_equation=lorenz,
         variables=variables,
         parameters=parameters,
         single_precision=True,
         platform_id=platform_id,
         device_id=device_id,
         t_span=t_span,
         stepper=clode.Stepper.rk4,
         dt=0.01,
     )
 
     t_average = []
-    print(f"Time for 1000 RK4 steps of the Lorenz system. {reps} repetitions.\n(N, min, median, max time)")
+    print(f"Lorenz system, 1000 RK4 steps, {reps} repetitions.\nN, min (s), median (s), max (s)")
     for num in num_pts:
         times = []
-        
+
         integrator.set_repeat_ensemble(num_repeats=num)
 
         #warm-up passes - seems to make output more reliable
         for _ in range(5):
             integrator.transient(update_x0=False)
 
         for _ in range(reps):
             t0 = time.perf_counter()
             integrator.transient(update_x0=False)
             times.append(time.perf_counter() - t0)
 
-        t_mean = sum(times)/reps
+        # t_mean = sum(times)/reps
         t_min = min(times)
         t_max = max(times)
         t_median = np.median(times)
         print(f"{num}\t {t_min:.3g}, {t_median:.3g}, {t_max:.3g} s")
         t_average.append(t_median)
 
     return t_average
-    
+
 
 # if using 'bazel test ...'
 if __name__ == "__main__":
 
     ocl_info = clode.runtime.query_opencl()
-    ocl_info = ocl_info[:3]
+    # ocl_info = ocl_info[:3]
+
+    N = [int(2**n) for n in np.arange(0,18)]
+    REPS = 50
 
-    num_pts = [int(2**n) for n in np.arange(0,18)]
-    reps = 50
-    
     device_names = []
     for i, ocl in enumerate(ocl_info):
         if ocl.device_count==0:
             continue
         print("\n", ocl)
         for j, dev in enumerate(ocl.device_info):
-            t_average = test_lorenz_rk4(platform_id=i, device_id=j, num_pts=num_pts, reps=reps)
-            plt.plot(num_pts, t_average)
+            median_time = test_lorenz_rk4(platform_id=i, device_id=j, num_pts=N, reps=REPS)
+            plt.plot(N, median_time)
             device_names.append(dev.name)
-    
+
     plt.legend(device_names)
     plt.xscale('log')
     plt.yscale('log')
-    plt.show()
+    plt.show()
```

### Comparing `clode-0.7.1/examples/fast_and_slow.py` & `clode-0.8.1/examples/fast_and_slow.py`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/examples/spike_counting.py` & `clode-0.8.1/examples/spike_counting.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from typing import List
 
 import clode
 from clode import exp
+# clode.set_log_level(clode.LogLevel.debug)
 
 def get_rhs(t: float,
             x: List[float],
             p: List[float],
             dx: List[float],
             aux: List[float],   
             w: List[float]) -> None:    
@@ -59,47 +60,40 @@
     abstol=1e-6,
     reltol=1e-5,
     event_var="v",
     feature_var="v",
     observer=clode.Observer.threshold_2,
     observer_x_up_thresh=0.5,
     observer_x_down_thresh=0.05,
-    observer_min_x_amp=1.0,
-    observer_min_imi=0.0,
-    observer_max_event_count=50,
 )
 
 # set up the ensemble of systems
-nx = 512
-ny = 512
-nPts = nx * ny
+nx = ny = 128
 gca = np.linspace(550.0, 1050.0, nx)
 kpmca = np.linspace(0.095, 0.155, ny)
-px, py = np.meshgrid(gca, kpmca)
+gca_grid, kpmca_grid = np.meshgrid(gca, kpmca)
 
-ensemble_parameters = {"gca" : px.flatten(), "kpmca" : py.flatten()} #gkca will have default value
-ensemble_parameters_names = list(ensemble_parameters.keys())
-
-integrator.set_ensemble(parameters=ensemble_parameters)
+# the 2D grid shape is noted internally, and features will be returned in this shape
+integrator.set_ensemble(parameters= {"gca" : gca_grid, "kpmca" : kpmca_grid})
 
 integrator.set_tspan((0.0, 50000.0))
 integrator.transient()
 integrator.set_tspan((0.0, 10000.0))
 integrator.features()
 
 features = integrator.get_observer_results()
 
-feature = features.get_var_max("peaks")
-feature = np.reshape(feature, (nx, ny))
+# the feature output knows to return the feature with shape matching the 2D grid input
+max_peaks = features.get_var_max("peaks")
 
-plt.pcolormesh(px, py, feature, shading='nearest', vmax=12)
+plt.pcolormesh(gca_grid, kpmca_grid, max_peaks, shading='nearest', vmax=12)
 plt.title("peaks")
 plt.colorbar()
-plt.xlabel(ensemble_parameters_names[0])
-plt.ylabel(ensemble_parameters_names[1])
+plt.xlabel("gca")
+plt.ylabel("kpmca")
 plt.axis("tight")
 
 # highlight a few example points - we'll get their trajectories next
 points = np.array([[950, 0.145], [700, 0.105], [750, 0.125], [800, 0.142]])
 plt.plot(points[:, 0], points[:, 1], 'o', color='black')
 for i, txt in enumerate(range(4)):
     plt.annotate(txt, (points[i, 0] - 10, points[i, 1] - 0.003))
@@ -120,25 +114,19 @@
     dt = 0.001,
     dtmax = 0.1,
     abstol = 1e-6,
     reltol = 1e-5,
     max_store = max_store,
 )
 
-traj_parameters = {"gca":points[:, 0], "kpmca": points[:, 1]}
-
-integrator_traj.set_ensemble(parameters = traj_parameters)
-
-integrator_traj.set_tspan((0.0, 50000.0))
-integrator_traj.transient()
-integrator_traj.set_tspan((0.0, 10000.0))
-integrator_traj.trajectory()
+integrator_traj.set_ensemble(parameters = {"gca":points[:, 0], "kpmca": points[:, 1]})
 
-trajectories = integrator_traj.get_trajectory()
+integrator_traj.transient(t_span=(0.0, 50000.0))
+trajectories = integrator_traj.trajectory(t_span=(0.0, 10000.0))
 
 fig, ax = plt.subplots(4, 1, sharex=True, sharey=True)
 for i, trajectory in enumerate(trajectories):
-    ax[i].plot(trajectory.t / 1000.0, trajectory.x[:, 0])
+    ax[i].plot(trajectory.t / 1000.0, trajectory.x["v"])
 
 ax[1].set_ylabel("v")
-ax[-1].set_xlabel('time (s)')
+ax[-1].set_xlabel("time (s)")
 plt.show()
```

### Comparing `clode-0.7.1/matlab/Chart.m` & `clode-0.8.1/matlab/Chart.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/matlab/GridSimulation.m` & `clode-0.8.1/matlab/GridSimulation.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/matlab/InitialValueProblem.m` & `clode-0.8.1/matlab/InitialValueProblem.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/matlab/clODE.m` & `clode-0.8.1/matlab/clODE.m`

 * *Files 1% similar despite different names*

```diff
@@ -115,18 +115,18 @@
             obj.sp=clODE.defaultSolverParams(); %default solver params (device transfer during init)
 %             obj.buildCL();
         end
         
         % new and delete are inherited
         
         %set a new problem - must initialize again!
-        function setNewProblem(obj, newprob)
+        function setProblemInfo(obj, newprob)
             newprob = clODE.purifyProblemStruct(newprob);
             if ~strcmp(newprob,obj.prob)
-                obj.cppmethod('setnewproblem', newprob);
+                obj.cppmethod('setProblemInfo', newprob);
                 obj.prob=newprob;
                 obj.clBuilt=false;
                 obj.clInitialized=false;
             end
         end
         
         %set a new time step method - must initialize again!
```

### Comparing `clode-0.7.1/matlab/clODEfeatures.m` & `clode-0.8.1/matlab/clODEfeatures.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/matlab/clODEfeaturesmex.cpp` & `clode-0.8.1/matlab/clODEfeaturesmex.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 typedef CLODEfeatures class_type;
 
 // List actions
 enum class Action
 {
     New,
     Delete,
-    SetNewProblem,
+    setProblemInfo,
     SetStepper,
     SetPrecision,
     SetOpenCL,
     BuildCL,
     Initialize, //overridden for clODEfeatures
     SetNPts,
     SetProblemData,
@@ -63,15 +63,15 @@
 };
 
 // Map string (first input argument to mexFunction) to an Action
 const std::map<std::string, Action> actionTypeMap =
 {
     { "new",            Action::New },
     { "delete",         Action::Delete },
-    { "setnewproblem",  Action::SetNewProblem },
+    { "setProblemInfo",  Action::setProblemInfo },
     { "setstepper",     Action::SetStepper },
     { "setprecision",   Action::SetPrecision },
     { "setopencl",      Action::SetOpenCL },
     { "buildcl",        Action::BuildCL},
     { "initialize",     Action::Initialize },
     { "setnpts",        Action::SetNPts },
     { "setproblemdata", Action::SetProblemData },
@@ -195,17 +195,17 @@
         instanceMap_type::const_iterator instIt = checkHandle(instanceTab, getHandle(nrhs, prhs));
         instanceTab.erase(instIt);
         mexUnlock();
         plhs[0] = mxCreateLogicalScalar(instanceTab.empty()); // info
         break;
     }
     //base class CLODE methods (rhs 0='methodName', 1=instanceID, ...)
-    case Action::SetNewProblem:
+    case Action::setProblemInfo:
 	{ //inputs: prob
-        instance->setNewProblem(getMatlabProblemStruct(prhs[2]));
+        instance->setProblemInfo(getMatlabProblemStruct(prhs[2]));
         break;
 	}
     case Action::SetStepper:
 	{ //inputs: stepper name
         std::string stepper = mxArrayToString(prhs[2]);
         instance->setStepper(stepper);
         break;
```

### Comparing `clode-0.7.1/matlab/clODEmex.cpp` & `clode-0.8.1/matlab/clODEmex.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 typedef CLODE class_type;
 
 // List actions
 enum class Action
 {
     New,
     Delete,
-    SetNewProblem,
+    setProblemInfo,
     SetStepper,
     SetPrecision,
     SetOpenCL,
     BuildCL,
     Initialize,
     SetNPts,
     SetProblemData,
@@ -57,15 +57,15 @@
 };
 
 // Map string (first input argument to mexFunction) to an Action
 const std::map<std::string, Action> actionTypeMap =
 {
     { "new",            Action::New },
     { "delete",         Action::Delete },
-    { "setnewproblem",  Action::SetNewProblem },
+    { "setProblemInfo",  Action::setProblemInfo },
     { "setstepper",     Action::SetStepper },
     { "setprecision",   Action::SetPrecision },
     { "setopencl",      Action::SetOpenCL },
     { "buildcl",        Action::BuildCL },
     { "initialize",     Action::Initialize },
     { "setnpts",        Action::SetNPts },
     { "setproblemdata", Action::SetProblemData },
@@ -179,17 +179,17 @@
     { //rhs='delete',instanceID
         instanceMap_type::const_iterator instIt = checkHandle(instanceTab, getHandle(nrhs, prhs));
         instanceTab.erase(instIt);
         mexUnlock();
         plhs[0] = mxCreateLogicalScalar(instanceTab.empty()); // info
         break;
     }
-    case Action::SetNewProblem:
+    case Action::setProblemInfo:
 	{ //inputs: prob
-        instance->setNewProblem(getMatlabProblemStruct(prhs[2]));
+        instance->setProblemInfo(getMatlabProblemStruct(prhs[2]));
         break;
 	}
     case Action::SetStepper:
 	{ //inputs: stepper name
         std::string stepper = mxArrayToString(prhs[2]);
         instance->setStepper(stepper);
         break;
```

### Comparing `clode-0.7.1/matlab/clODEmexHelpers.hpp` & `clode-0.8.1/matlab/clODEmexHelpers.hpp`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/matlab/clODEtrajectory.m` & `clode-0.8.1/matlab/clODEtrajectory.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/matlab/clODEtrajectorymex.cpp` & `clode-0.8.1/matlab/clODEtrajectorymex.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 typedef CLODEtrajectory class_type;
 
 // List actions
 enum class Action
 {
     New,
     Delete, 
-    SetNewProblem,
+    setProblemInfo,
     SetStepper,
     SetPrecision,
     SetOpenCL,
     BuildCL,
     Initialize, //overridden for clODEtrajectory
     SetNPts,
     SetProblemData,
@@ -64,15 +64,15 @@
 };
 
 // Map string (first input argument to mexFunction) to an Action
 const std::map<std::string, Action> actionTypeMap =
 {
     { "new",            Action::New },
     { "delete",         Action::Delete },
-    { "setnewproblem",  Action::SetNewProblem },
+    { "setProblemInfo",  Action::setProblemInfo },
     { "setstepper",     Action::SetStepper },
     { "setprecision",   Action::SetPrecision },
     { "setopencl",      Action::SetOpenCL },
     { "buildcl",        Action::BuildCL},
     { "initialize",     Action::Initialize },
     { "setnpts",        Action::SetNPts },
     { "setproblemdata", Action::SetProblemData },
@@ -191,17 +191,17 @@
         instanceMap_type::const_iterator instIt = checkHandle(instanceTab, getHandle(nrhs, prhs));
         instanceTab.erase(instIt);
         mexUnlock();
         plhs[0] = mxCreateLogicalScalar(instanceTab.empty()); // info
         break;
     }
     //base class CLODE methods (rhs 0='methodName', 1=instanceID, ...)
-    case Action::SetNewProblem:
+    case Action::setProblemInfo:
 	{ //inputs: prob
-        instance->setNewProblem(getMatlabProblemStruct(prhs[2]));
+        instance->setProblemInfo(getMatlabProblemStruct(prhs[2]));
         break;
 	}
     case Action::SetStepper:
 	{ //inputs: stepper name
         std::string stepper = mxArrayToString(prhs[2]);
         instance->setStepper(stepper);
         break;
```

### Comparing `clode-0.7.1/matlab/clickTrajectory.m` & `clode-0.8.1/matlab/clickTrajectory.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/matlab/compileCLODEmex.m` & `clode-0.8.1/matlab/compileCLODEmex.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/matlab/cppclass.m` & `clode-0.8.1/matlab/cppclass.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/matlab/generate_pointset.m` & `clode-0.8.1/matlab/generate_pointset.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/matlab/gridKeyPress.m` & `clode-0.8.1/matlab/gridKeyPress.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/matlab/gridfigure.m` & `clode-0.8.1/matlab/gridfigure.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/matlab/gridtool.m` & `clode-0.8.1/matlab/gridtool.m`

 * *Files 0% similar despite different names*

```diff
@@ -315,16 +315,16 @@
             end
             
             app.currentFileLabel.Text=app.prob.name+".ode";
             
             if isempty(app.clo_g)
                 
             else %to avoid reverting to default sp and op:
-                app.clo_g.setNewProblem(app.prob);
-                app.clo_t.setNewProblem(app.prob);
+                app.clo_g.setProblemInfo(app.prob);
+                app.clo_t.setProblemInfo(app.prob);
                 
                 %remove grid.name to allow new grid to be set below
                 app.listenerGrid.Enabled=0;
                 app.gridtab.name={'';''};
                 app.listenerGrid.Enabled=1;
                 app.clo_g.F=[]; %to allow new nVar
                 app.clo_g.Xf=[]; %to allow new nVar
```

### Comparing `clode-0.7.1/matlab/gridtool_old.m` & `clode-0.8.1/matlab/gridtool_old.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/matlab/matlabLogging.hpp` & `clode-0.8.1/matlab/matlabLogging.hpp`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/matlab/plot_twopar.m` & `clode-0.8.1/matlab/plot_twopar.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/matlab/queryOpenCL.cpp` & `clode-0.8.1/matlab/queryOpenCL.cpp`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/mkdocs.yml` & `clode-0.8.1/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,20 @@
     - 'install.md'
     - 'getting_started.md'
   - Functionality:
     - Feature Extraction: 'feature_extraction.md'
     - Trajectory Simulation: 'trajectory_simulation.md'
     - Stochastic Simulations: 'Ornstein-Uhlenbeck_process.md'
     - Spike Counting: 'spike_counting.md'
+  - Observers:
+    - 'observers.md'
   - Configuration:
       - Specifying systems of ODEs: 'specifying_odes.md'
       - XPP files: 'xpp_files.md'
-      - Initialising the runtime: 'init_runtime.md'
+      - Initializing the runtime: 'init_runtime.md'
       - Selecting logging levels: 'logging_levels.md'
       - Querying OpenCL devices: 'querying_opencl.md'
       - Running in Matlab: 'matlab.md'
   #Generate the API reference from the python code in clode/python
   - API Reference: 'api_reference.md'
 
 #https://squidfunk.github.io/mkdocs-material/reference/math/
```

### Comparing `clode-0.7.1/pyproject.toml` & `clode-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/samples/BUILD` & `clode-0.8.1/samples/BUILD`

 * *Files 6% similar despite different names*

```diff
@@ -58,32 +58,14 @@
     linkstatic = True,
     deps = [
         "//clode/cpp",
     ],
 )
 
 cc_test(
-    name = "testFeatLarge",
-    srcs = ["testFeatures_morevars.cpp"],
-    data = [
-        ":lactotroph",
-        "//clode/cpp:opencl",
-    ],
-    linkopts = select({
-        "@platforms//os:osx": [],
-        "@platforms//os:linux": ["-lOpenCL"],
-        "@platforms//os:windows": [],
-    }),
-    linkstatic = True,
-    deps = [
-        "//clode/cpp",
-    ],
-)
-
-cc_test(
     name = "listOpenCL",
     srcs = ["listOpenCL.cpp"],
     data = [
         "//clode/cpp:opencl",
     ],
     linkopts = select({
         "@platforms//os:osx": [],
```

### Comparing `clode-0.7.1/samples/Makefile` & `clode-0.8.1/samples/Makefile`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/samples/lacto_more_vars.cl` & `clode-0.8.1/samples/lactotroph_noise.cl`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,20 @@
 
 void getRHS(const realtype t, const realtype x_[], const realtype p_[], realtype dx_[], realtype aux_[], const realtype w_[]) {
+realtype c2=x_[3]*x_[3];
+realtype vkdrive=x_[0]-RCONST(-75.0);
 realtype minf=RCONST(1.0)/(RCONST(1.0)+exp((RCONST(-20.0)-x_[0])/RCONST(12.0)));
-realtype mtinf=RCONST(1.0)/(RCONST(1.0)+exp((RCONST(-38.0)-x_[0])/RCONST(6.0)));
-realtype htinf=RCONST(1.0)/(RCONST(1.0)+exp((RCONST(-56.0)-x_[0])/RCONST(-5.0)));
 realtype ninf=RCONST(1.0)/(RCONST(1.0)+exp((RCONST(-5.0)-x_[0])/RCONST(10.0)));
-realtype sinf=x_[7]*x_[7]/(x_[7]*x_[7]+RCONST(0.40)*RCONST(0.40));
-realtype nkinf=RCONST(1.0)/(RCONST(1.0)+exp((RCONST(-65.0)-x_[0])/RCONST(-8.0)));
-realtype binf=RCONST(1.0)/(RCONST(1.0)+exp((RCONST(-20.0)-x_[0])/RCONST(2.0)));
-realtype v_na_inf=RCONST(1.0)/(RCONST(1.0)+exp((RCONST(-15.0)-x_[0])/RCONST(5.0)));
-realtype hnainf=RCONST(1.0)/(RCONST(1.0)+exp((RCONST(-60.0)-x_[0])/RCONST(-10.0)));
-realtype ainf=RCONST(1.0)/(RCONST(1.0)+exp((RCONST(-20.0)-x_[0])/RCONST(10.0)));
-realtype hinf=RCONST(1.0)/(RCONST(1.0)+exp((RCONST(-60.0)-x_[0])/RCONST(-5.0)));
-realtype i_cal=p_[0]*x_[2]*(x_[0]-RCONST(60.0));
-realtype i_cat=p_[1]*mtinf*x_[5]*(x_[0]-RCONST(60.0));
-realtype i_k=p_[2]*x_[1]*(x_[0]-RCONST(-75.0));
-realtype i_sk=p_[3]*sinf*(x_[0]-RCONST(-75.0));
-realtype i_kir=p_[4]*nkinf*(x_[0]-RCONST(-75.0));
-realtype i_bk=p_[5]*x_[3]*(x_[0]-RCONST(-75.0));
-realtype i_nav=p_[6]*v_na_inf*v_na_inf*v_na_inf*x_[6]*(x_[0]-RCONST(75.0));
-realtype i_a=p_[7]*ainf*x_[4]*(x_[0]-RCONST(-75.0));
-realtype i_leak=p_[8]*(x_[0]-p_[10]);
-realtype i_noise=p_[18]*w_[0];
-realtype i=i_cal+i_cat+i_k+i_sk+i_kir+i_bk+i_nav+i_a+i_leak+i_noise;
-dx_[0]=-i/p_[9];
-dx_[1]=(ninf-x_[1])/p_[13];
-dx_[2]=(minf-x_[2])/p_[11];
-dx_[3]=(binf-x_[3])/p_[14];
-dx_[4]=(hinf-x_[4])/p_[15];
-dx_[5]=(htinf-x_[5])/p_[12];
-dx_[6]=(hnainf-x_[6])/p_[16];
-dx_[7]=-RCONST(0.010)*(RCONST(0.00150)*i_cal+p_[17]*x_[7]);
-aux_[0]=i_noise;
+realtype ica=p_[0]*minf*(x_[0]-RCONST(60.0));
+realtype isk=p_[1]*c2/(c2+RCONST(0.40)*RCONST(0.40))*vkdrive;
+realtype ibk=p_[2]*x_[2]*vkdrive;
+realtype ik=RCONST(2.0)*x_[1]*vkdrive;
+realtype il=RCONST(0.050)*(x_[0]-RCONST(-50.0));
+realtype inoise=p_[3]*w_[0];
+realtype itot=ica+isk+ibk+ik+il+inoise;
+dx_[0]=-itot/RCONST(10.0);
+dx_[1]=(ninf-x_[1])/RCONST(30.0);
+dx_[2]=(RCONST(1.0)/(RCONST(1.0)+exp((RCONST(-20.0)-x_[0])/RCONST(2.0)))-x_[2])/RCONST(8.0);
+dx_[3]=-RCONST(0.010)*(RCONST(0.00150)*ica+RCONST(0.20)*x_[3]);
+aux_[0]=ica;
 }
```

### Comparing `clode-0.7.1/samples/lactotroph.cl` & `clode-0.8.1/samples/lactotroph.cl`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/samples/lactotroph.ode` & `clode-0.8.1/samples/lactotroph.ode`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/samples/lactotroph_noise.ode` & `clode-0.8.1/samples/lactotroph_noise.ode`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/samples/plot_twopar.m` & `clode-0.8.1/samples/plot_twopar.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/samples/run_twopar.m` & `clode-0.8.1/samples/run_twopar.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/samples/test.cl` & `clode-0.8.1/samples/test.cl`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/samples/testCLODE.m` & `clode-0.8.1/samples/testCLODE.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/samples/testCLODEfeatures.m` & `clode-0.8.1/samples/testCLODEfeatures.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/samples/testCLODEmex.m` & `clode-0.8.1/samples/testCLODEmex.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/samples/testCLODEtrajectory.m` & `clode-0.8.1/samples/testCLODEtrajectory.m`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/samples/testFeatures.cpp` & `clode-0.8.1/samples/testFeatures.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -75,40 +75,43 @@
 	std::vector<double> x0(nPts*prob.nVar, 0.0);
 	
 	std::string observer = "thresh2";
 	ObserverParams<double> op;
 	op.eVarIx=0;
 	op.fVarIx=0;
 	op.maxEventCount=100;
-	op.minXamp=1;
+	op.maxEventTimestamps=0;
+	op.minXamp=0.0;
+	op.minIMI=0.0;
 	op.nHoodRadius=0.01;
 	op.xUpThresh=0.3;
 	op.xDownThresh=0.2;
-	op.dxUpThresh=0;
-	op.dxDownThresh=0;
+	op.dxUpThresh=0.0;
+	op.dxDownThresh=0.0;
 	op.eps_dx=1e-7;
 
 	
 	// Select device type and/or vendor using command line flags ("--device cpu/gpu/accel", "--vendor amd/intel/nvidia")
 	OpenCLResource opencl( argc, argv);
 	
 	//prep timer and PRNG
 	srand(static_cast <unsigned> (time(0))); 
     std::chrono::time_point<std::chrono::high_resolution_clock> start, end;
 	std::chrono::duration<double, std::milli> elapsed_ms;
 
 	// create the simulator
-	CLODEfeatures clo(prob, stepper, observer, CLSinglePrecision, opencl, CLODE_ROOT);
+	CLODEfeatures clo(prob, stepper, observer, op, CLSinglePrecision, opencl, CLODE_ROOT);
 
 	//~ std::cout<<"here"<<std::endl;
 	//copy problem data to the device
 
     clo.buildCL();
-	clo.initialize(tspan, x0, pars, sp, op);
-
+	clo.setSolverParams(sp);
+	clo.setProblemData(x0, pars);
+	clo.setTspan(tspan);
 	clo.seedRNG(mySeed);
 	
 	//run the simulation 
 	clo.transient();
     clo.shiftX0();
```

### Comparing `clode-0.7.1/samples/testTrajectory.cpp` & `clode-0.8.1/samples/testTrajectory.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -76,15 +76,17 @@
     std::chrono::time_point<std::chrono::high_resolution_clock> start, end;
 	std::chrono::duration<double, std::milli> elapsed_ms;
 
 	// create the solver
 	CLODEtrajectory clo(prob, stepper, CLSinglePrecision, opencl, CLODE_ROOT);
 
     clo.buildCL();
-    clo.initialize(tspan, x0, pars, sp);
+	clo.setSolverParams(sp);
+	clo.setProblemData(x0, pars);
+	clo.setTspan(tspan);
 
     int mySeed = 1;
     clo.seedRNG(mySeed);
 	
 	//warm up to pre-set nSteps and nPts
 	clo.transient();
```

### Comparing `clode-0.7.1/samples/testTransient.cpp` & `clode-0.8.1/samples/testTransient.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -85,27 +85,23 @@
 	std::chrono::duration<double, std::milli> elapsed_ms;
 	
 
 	// create the simulator
 	CLODE clo(prob, stepper, CLSinglePrecision, opencl, CLODE_ROOT);
 
     clo.buildCL();
-
-    //copy problem data to the device
-	clo.initialize(tspan, x0, pars, sp); 
+	clo.setSolverParams(sp);
+	clo.setProblemData(x0, pars);
+	clo.setTspan(tspan);
 	
-	// std::cout<<"here"<<std::endl;
-	// clo.seedRNG(mySeed);
+	clo.seedRNG();
 	
 	//run the simulation 
 	clo.transient();
 	
-	// clo.initialize(tspan, x0, pars, sp); 
-	// clo.initializeProblem(tspan, x0, pars); 
-	
 	// clo.transient(); 
 	// clo.transient(pars);
 	// clo.transient(tspan, x0);
 	// clo.transient(tspan, x0, pars);
 	
 	
 	std::cout<<std::endl;
```

### Comparing `clode-0.7.1/samples/test_outputs_cpp.md` & `clode-0.8.1/samples/test_outputs_cpp.md`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/setup.py` & `clode-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/test/lorenz.cl` & `clode-0.8.1/test/lorenz.cl`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/test/ornl_thompson_a1.cl` & `clode-0.8.1/test/ornl_thompson_a1.cl`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/test/test_convert_python_to_opencl.py` & `clode-0.8.1/test/test_function_converter.py`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/test/test_logger.py` & `clode-0.8.1/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/test/test_observers.py` & `clode-0.8.1/test/test_observers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-from math import pi
+from math import cos, pi, sqrt
 from typing import List
+
 import pytest
 
 import clode
+
 clode.set_log_level(clode.LogLevel.info)
 
 # test each observer to make sure they:
 # - handle zero aux
 # - return expected results
 
-# Notes:
+# oscillatory system
+# harmonic oscillator. Solution is x=cos(t), y=sin(t) --> the unit circle
 # Starting at the top of the unit circle, the trajectory should proceed counter-clockwise.
 # We use "y" as the feature variable
 #
 # local_max
 # - event triggers at any local maximum in event_var
 # - starting at (-1.0, 0.0) means we'll see one local max in y per period
 #
 # nhood1 (one-pass, neighborhood event detector) **first period can be off
 # - trigger point is first local min of event_var
 # - after that, event triggers if the trajectory enters a ball of radius=observer_neighbourhood_radius, measured in unit-normalized state space
 # - starting at (-1.0, 0.0) should trigger on first rotation.
-# ** it takes a full period to visit the full extent of state-space (required for computing the positiong in unit-normalized state space)
+# ** it takes a full period to visit the full extent of state-space (required for computing the position in unit-normalized state space)
 # ** this one doesn't do a warmup pass, so the unit-normalization will be based on unpredictable amount of event_var range! here, exactly half of truth...
 # **--> however, it adapts: as long as it runs a full period, the threshold will settle to correct value.
 # - number of periods = event count - 1
 #
 # nhood2 (two-pass, neighborhood event detector)
 # - trigger point is the point in state space where eVarIx first drops below observer_x_down_thresh
 # - after that, event triggers if the trajectory enters a ball of radius=observer_neighbourhood_radius, measured in unit-normalized state space
@@ -36,41 +39,47 @@
 # thresh2 (two-pass, Shmitt trigger-like threshold detector)
 # - thresholds calculated based on unit-normalized values of event_var (first pass finds max and min for normalization)
 # - initialization: if event_var > observer_x_up_thresh, considered to be in the "up-state"
 # - event triggers at upward crossing of observer_x_up_thresh for the event_var (from "down-state" to "up-state")
 # - starting at (-1.0, 0.0) should start in the up-state; triggers on first rotation
 # - number of periods = event count - 1
 
-# TODO: per-observer parameter struct?
-# TODO: support zero parameters? (for sweeps of initial conditions only)
-
-# harmonic oscillator
-def get_rhs(t: float,
-            vars: List[float],
-            p: List[float],
-            dy: List[float],
-            aux: List[float],   
-            w: List[float]) -> None:
+# harmonic oscillator.
+# Solution: x=cos(t), y=sin(t)
+def get_rhs(
+    t: float,
+    vars: List[float],
+    p: List[float],
+    dy: List[float],
+    aux: List[float],
+    w: List[float],
+) -> None:
     k: float = p[0]
     x: float = vars[0]
     y: float = vars[1]
     dy[0] = y
-    dy[1] = -k*x
+    dy[1] = -k * x
+
 
 # start at the left of the unit circle
-variables = {"x": -1.0, "y":0.0} 
+variables = {"x": -1.0, "y": 0.0}
+parameters = {"k": 1.0}
 
-parameters = {"k": 1.0} 
-expected_period = 2*pi
+expected_period = 2 * pi
+expected_amplitude = 2.0
+expected_max_xy = 1.0
+expected_min_xy = -1.0
+expected_mean_xy = 0.0
 
 # 10 full periods
 expected_events = 10
-t_span = (0.0, expected_events*expected_period)
+t_span = (0.0, expected_events * expected_period)
 dt = 0.01
-expected_steps = int(t_span[1]/dt)+1
+expected_steps = int(t_span[1] / dt) + 1
+
 
 @pytest.mark.skip(reason="for now just to validate/debug observers")
 def test_observer(observer):
     integrator = clode.FeatureSimulator(
         rhs_equation=get_rhs,
         variables=variables,
         parameters=parameters,
@@ -79,48 +88,62 @@
         observer=observer,
         event_var="y",
         feature_var="y",
         observer_min_x_amp=0.0,
         observer_x_up_thresh=0.3,
         observer_x_down_thresh=0.2,
         observer_neighbourhood_radius=0.05,
+        observer_max_event_timestamps=10,
     )
 
-    integrator.set_repeat_ensemble(num_repeats=1)
-
-    integrator.features()
+    features = integrator.features()
+    feature_names = features.get_feature_names()
 
+    print(f"--- {observer} ---")
     print(f"final state: {integrator.get_final_state()[0]}")
 
-    features = integrator.get_observer_results()
-    feature_names = features.get_feature_names()
-
-    #TODO: switch to asserts?
+    # TODO: map of feature_names --> expected results (including event times)
+    # TODO: switch to asserts?
+    if "max x" in feature_names:
+        max_x = features.get_var_max("x")
+        print(f"expected max x: {expected_max_xy},\t\t actual:{max_x:0.6}")
+    if "min x" in feature_names:
+        min_x = features.get_var_min("x")
+        print(f"expected min x: {expected_min_xy},\t\t actual:{min_x:0.6}")
+    if "mean x" in feature_names:
+        mean_x = features.get_var_mean("x")
+        print(f"expected mean x: {expected_mean_xy},\t\t actual:{mean_x:0.6}")
     if "mean y" in feature_names:
         mean_y = features.get_var_mean("y")
-        print(f"expected mean y: {0.0},\t\t actual:{mean_y:0.4}")
+        print(f"expected mean y: {expected_mean_xy},\t\t actual:{mean_y:0.6}")
+    if "mean amplitude" in feature_names:
+        amp = features.get_var_mean("amplitude")
+        print(f"expected amplitude: {expected_amplitude},\t actual:{amp:0.6}")
     if "mean IMI" in feature_names:
-        inter_maximum_interval = features.get_var_mean("IMI")
-        print(f"expected IMI: {expected_period:0.4},\t\t actual:{inter_maximum_interval:0.4}")
+        imi = features.get_var_max("IMI")
+        print(f"expected IMI: {expected_period:0.6},\t\t actual:{imi:0.6}")
+        imi = features.get_var_min("IMI")
+        print(f"expected IMI: {expected_period:0.6},\t\t actual:{imi:0.6}")
+        imi = features.get_var_mean("IMI")
+        print(f"expected IMI: {expected_period:0.6},\t\t actual:{imi:0.6}")
     if "mean period" in feature_names:
         period = features.get_var_mean("period")
-        print(f"expected period: {expected_period:0.4},\t\t actual:{period:0.4}")
+        print(f"expected period: {expected_period:0.6},\t actual:{period:0.6}")
     if "event count" in feature_names:
         event_count = features.get_var_count("event")
         print(f"expected event count: {expected_events},\t actual:{int(event_count)}")
-    if "period count" in feature_names:
-        period_count = features.get_var_count("period")
-        print(f"expected period count: {expected_events-1},\t actual:{int(period_count)}")
     if "step count" in feature_names:
         step_count = features.get_var_count("step")
         print(f"expected step count: {expected_steps},\t actual:{int(step_count)}")
     print("\n")
 
-observers = [observer for observer in clode.Observer]
 
 @pytest.mark.skip(reason="for now just to validate/debug observers")
 def test_all_observers():
+    observers = [observer for observer in clode.Observer]
+    # observers = [clode.Observer.local_max]
     for observer in observers:
         test_observer(observer)
 
+
 if __name__ == "__main__":
-    test_all_observers()
+    test_all_observers()
```

### Comparing `clode-0.7.1/test/test_opencl_builtins.py` & `clode-0.8.1/test/test_opencl_builtins.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     exp10,
     expm1,
     fabs,
     fdim,
     floor,
     fmod,
     gamma,
+    heaviside,
     hypot,
     ilogb,
     ldexp,
     lgamma,
     log,
     log1p,
     log2,
@@ -102,27 +103,27 @@
         aux[22] = expm1(x0)
         aux[23] = fabs(x0)
         aux[24] = fdim(x0, x1)
         aux[25] = floor(x1)
         aux[26] = 0.0  # fma(x0, x1, x2)
         aux[27] = fmod(x0, x1 + 1)
         # aux[28] = fract(x0) # Compile error
-        aux[28] = t
+        aux[28] = heaviside(t - 0.5)
         aux[29] = gamma(x0 + 1)
         aux[30] = hypot(x0, x1)
         aux[31] = float(ilogb(x0 + 1))
         aux[32] = ldexp(x0, int(x1))
         aux[33] = lgamma(x0 + 1)
         aux[34] = log(x0 + 1)
         aux[35] = log1p(x0 + 1)
         aux[36] = log2(x0 + 1)
         aux[37] = log10(x0 + 1)
         aux[38] = 0.0  # logb(x0 + 1)
         aux[39] = 0.0  # mad(x0, x1, x2)
-        # aux[40] = nan()
+        aux[40] = 0.0  # nan()
         aux[41] = nextafter(x0, x1)
         aux[42] = pow(x0, x1)
         aux[43] = pown(x0, p0)
         aux[44] = powr(x0 + 0.5, x1 + 0.2)
         aux[45] = remainder(x0, x1 + 1)
         aux[46] = rint(x0)
         aux[47] = rootn(x0, p1)
@@ -152,21 +153,25 @@
         aux=aux,
         t_span=(0, 1),
         stepper=clode.Stepper.euler,
         max_store=3,
         max_steps=3,
     )
 
-    sim.trajectory()
-    aux_values = sim.get_aux()[0]
+    trajectory = sim.trajectory()
 
     vars_arr = list(variables.values())
     params_arr = list(parameters.values())
     for t_index, t in enumerate([0, 0.5, 1]):
         aux_arr = [0.0] * len(aux)
         dx = [0.0] * len(vars_arr)
         w: List[float] = []
         rhs(t, vars_arr, params_arr, dx, aux_arr, w)
-        for i in range(len(aux)):
+        for i, auxi in enumerate(aux):
+            cl_aux_arr = trajectory.aux[auxi]
             assert np.isclose(
-                aux_values[t_index, i], aux_arr[i], atol=1e-7
-            ), f"Divergence at index {i} at time {t}, expected {aux_arr[i]}, got {aux_values[t_index, i]}"
+                cl_aux_arr[t_index], aux_arr[i], atol=1e-7
+            ), f"Assertion failed for {auxi} at time {t}, expected {aux_arr[i]}, got {cl_aux_arr[t_index]}"
+
+
+if __name__ == "__main__":
+    test_opencl_builtins()
```

### Comparing `clode-0.7.1/test/test_runtime.py` & `clode-0.8.1/test/test_runtime.py`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/test/test_vdp.py` & `clode-0.8.1/test/test_vdp.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     parameters = {
         "mu": [-1, 0, 0.01, 0.1, 0.5, 1.0, 1.5, 2.0, 2.5, 3.0, 3.5, 4.0]
         + list(range(5, end))
     }
 
     integrator.set_ensemble(parameters=parameters)
 
-    integrator.transient()
+    # integrator.transient()
     integrator.features()
     observer_output = integrator.get_observer_results()
 
     periods = observer_output.get_var_max("period")
 
     for index, mu in enumerate(parameters["mu"]):
         period = periods[index]
@@ -97,10 +97,11 @@
 
 def test_vdp_dormand_prince_python_rhs():
     vdp_dormand_prince(end=7, input_eq=getRHS)
 
 
 # if using 'bazel test ...'
 if __name__ == "__main__":
-    print(clode)
-    sys.exit(pytest.main(sys.argv[1:]))
-    # test_vdp_dormand_prince()
+    # print(clode)
+    # sys.exit(pytest.main(sys.argv[1:]))
+    # clode.set_log_level(clode.LogLevel.debug)
+    vdp_dormand_prince(end=100)
```

### Comparing `clode-0.7.1/test/test_xpp_converter.py` & `clode-0.8.1/test/test_xpp_parser.py`

 * *Files identical despite different names*

### Comparing `clode-0.7.1/test/xpp/van_der_pol_oscillator_reference.cl` & `clode-0.8.1/test/xpp/van_der_pol_oscillator_reference.cl`

 * *Files identical despite different names*

