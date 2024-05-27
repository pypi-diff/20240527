# Comparing `tmp/qulacs-0.6.2.tar.gz` & `tmp/qulacs-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qulacs-0.6.2.tar", last modified: Wed Sep 13 07:05:52 2023, max compression
+gzip compressed data, was "qulacs-0.6.3.tar", last modified: Mon Dec 25 09:28:15 2023, max compression
```

## Comparing `qulacs-0.6.2.tar` & `qulacs-0.6.3.tar`

### file list

```diff
@@ -1,450 +1,453 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.231306 qulacs-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-09-13 07:05:24.000000 qulacs-0.6.2/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.159304 qulacs-0.6.2/.devcontainer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.163304 qulacs-0.6.2/.devcontainer/cpu/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-09-13 07:05:24.000000 qulacs-0.6.2/.devcontainer/cpu/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2023-09-13 07:05:24.000000 qulacs-0.6.2/.devcontainer/cpu/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.163304 qulacs-0.6.2/.devcontainer/gpu/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-09-13 07:05:24.000000 qulacs-0.6.2/.devcontainer/gpu/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2023-09-13 07:05:24.000000 qulacs-0.6.2/.devcontainer/gpu/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.159304 qulacs-0.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.167304 qulacs-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2023-09-13 07:05:24.000000 qulacs-0.6.2/.github/workflows/ci_macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2023-09-13 07:05:24.000000 qulacs-0.6.2/.github/workflows/ci_ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-09-13 07:05:24.000000 qulacs-0.6.2/.github/workflows/ci_windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2023-09-13 07:05:24.000000 qulacs-0.6.2/.github/workflows/wheel.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-09-13 07:05:24.000000 qulacs-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-09-13 07:05:24.000000 qulacs-0.6.2/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.167304 qulacs-0.6.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2023-09-13 07:05:24.000000 qulacs-0.6.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)    16670 2023-09-13 07:05:24.000000 qulacs-0.6.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2023-09-13 07:05:24.000000 qulacs-0.6.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-09-13 07:05:24.000000 qulacs-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14136 2023-09-13 07:05:52.231306 qulacs-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11068 2023-09-13 07:05:24.000000 qulacs-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    11431 2023-09-13 07:05:24.000000 qulacs-0.6.2/README_MPI.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-09-13 07:05:24.000000 qulacs-0.6.2/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.167304 qulacs-0.6.2/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-09-13 07:05:24.000000 qulacs-0.6.2/benchmark/AdaptiveGate.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-09-13 07:05:24.000000 qulacs-0.6.2/benchmark/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2023-09-13 07:05:24.000000 qulacs-0.6.2/benchmark/bench_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-09-13 07:05:24.000000 qulacs-0.6.2/benchmark/benchmark2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-09-13 07:05:24.000000 qulacs-0.6.2/benchmark/causalconetest.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.167304 qulacs-0.6.2/benchmark/circuits/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-09-13 07:05:24.000000 qulacs-0.6.2/benchmark/circuits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2023-09-13 07:05:24.000000 qulacs-0.6.2/benchmark/circuits/quantumvolume.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2023-09-13 07:05:24.000000 qulacs-0.6.2/benchmark/circuits/qulacsbench.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2023-09-13 07:05:24.000000 qulacs-0.6.2/benchmark/libcppsim_benchmark.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    17638 2023-09-13 07:05:24.000000 qulacs-0.6.2/benchmark/libcsim_benchmark.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      308 2023-09-13 07:05:24.000000 qulacs-0.6.2/benchmark/merge_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2023-09-13 07:05:24.000000 qulacs-0.6.2/benchmark/test_qulacs_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-09-13 07:05:24.000000 qulacs-0.6.2/benchmark/test_qulacs_2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.167304 qulacs-0.6.2/cmake_script/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.167304 qulacs-0.6.2/cmake_script/FetchContent/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-09-13 07:05:24.000000 qulacs-0.6.2/cmake_script/FetchContent/CMakeLists.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)    38023 2023-09-13 07:05:24.000000 qulacs-0.6.2/cmake_script/FetchContent.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2023-09-13 07:05:24.000000 qulacs-0.6.2/cmake_script/FindAVX2.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      975 2023-09-13 07:05:24.000000 qulacs-0.6.2/cmake_script/FindSVE.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-09-13 07:05:24.000000 qulacs-0.6.2/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.167304 qulacs-0.6.2/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.167304 qulacs-0.6.2/doc/en/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.167304 qulacs-0.6.2/doc/en/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.159304 qulacs-0.6.2/doc/en/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.167304 qulacs-0.6.2/doc/en/source/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/_static/images/dojo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/_static/images/github.png
--rw-r--r--   0 runner    (1001) docker     (127)    54241 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/_static/images/logo-c-h.png
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/_static/images/slack.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.171304 qulacs-0.6.2/doc/en/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.171304 qulacs-0.6.2/doc/en/source/_templates/autoapi/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/_templates/autoapi/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/_templates/autoapi/macros.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.171304 qulacs-0.6.2/doc/en/source/_templates/autoapi/python/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/_templates/autoapi/python/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/_templates/autoapi/python/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/_templates/autoapi/python/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/_templates/autoapi/python/exception.rst
--rw-r--r--   0 runner    (1001) docker     (127)      652 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/_templates/autoapi/python/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)      704 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/_templates/autoapi/python/method.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/_templates/autoapi/python/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/_templates/autoapi/python/package.rst
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/_templates/autoapi/python/property.rst
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/_templates/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.175304 qulacs-0.6.2/doc/en/source/apply/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/apply/0_overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   162833 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/apply/5.2_qcl.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    30093 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/apply/6.2_vqe.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    55651 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/apply/6.3_ssvqe.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.175304 qulacs-0.6.2/doc/en/source/apply/img/
--rw-r--r--   0 runner    (1001) docker     (127)    59895 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/apply/img/QCL.png
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.175304 qulacs-0.6.2/doc/en/source/guide/
--rw-r--r--   0 runner    (1001) docker     (127)   157994 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/guide/2.0_python_advanced.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.175304 qulacs-0.6.2/doc/en/source/intro/
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/intro/0_about.md
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/intro/1_install.md
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/intro/2_faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/intro/3_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)    27329 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/intro/4.1_python_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    26841 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/intro/4.2_cpp_tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.175304 qulacs-0.6.2/doc/en/source/write/
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/en/source/write/0_readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.175304 qulacs-0.6.2/doc/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.175304 qulacs-0.6.2/doc/ja/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.159304 qulacs-0.6.2/doc/ja/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.175304 qulacs-0.6.2/doc/ja/source/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/_static/images/dojo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/_static/images/github.png
--rw-r--r--   0 runner    (1001) docker     (127)    54241 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/_static/images/logo-c-h.png
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/_static/images/slack.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.175304 qulacs-0.6.2/doc/ja/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.175304 qulacs-0.6.2/doc/ja/source/_templates/autoapi/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/_templates/autoapi/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/_templates/autoapi/macros.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.179304 qulacs-0.6.2/doc/ja/source/_templates/autoapi/python/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/_templates/autoapi/python/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/_templates/autoapi/python/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/_templates/autoapi/python/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/_templates/autoapi/python/exception.rst
--rw-r--r--   0 runner    (1001) docker     (127)      652 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/_templates/autoapi/python/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)      704 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/_templates/autoapi/python/method.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/_templates/autoapi/python/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/_templates/autoapi/python/package.rst
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/_templates/autoapi/python/property.rst
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.179304 qulacs-0.6.2/doc/ja/source/guide/
--rw-r--r--   0 runner    (1001) docker     (127)    78839 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/guide/2.0_python_advanced.md
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.179304 qulacs-0.6.2/doc/ja/source/intro/
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/intro/0_about.md
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/intro/1_install.md
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/intro/2_faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/intro/3_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)    14702 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/intro/4.1_python_tutorial.md
--rw-r--r--   0 runner    (1001) docker     (127)    27502 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/ja/source/intro/4.2_cpp_tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.179304 qulacs-0.6.2/doc/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/scripts/customdoxygen.css
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/scripts/doxy-boot.js
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/scripts/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/scripts/header.html
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2023-09-13 07:05:24.000000 qulacs-0.6.2/doc/scripts/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2023-09-13 07:05:24.000000 qulacs-0.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.159304 qulacs-0.6.2/pysrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.183304 qulacs-0.6.2/pysrc/qulacs/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36484 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-09-13 07:05:51.000000 qulacs-0.6.2/pysrc/qulacs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.183304 qulacs-0.6.2/pysrc/qulacs/circuit/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/circuit/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/circuit/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/circuit.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.183304 qulacs-0.6.2/pysrc/qulacs/converter/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13126 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/converter/qasm_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.183304 qulacs-0.6.2/pysrc/qulacs/gate/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/gate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/gate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/gate/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10900 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/gate.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.183304 qulacs-0.6.2/pysrc/qulacs/observable/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/observable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/observable/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/observable/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/observable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.187305 qulacs-0.6.2/pysrc/qulacs/quantum_operator/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/quantum_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/quantum_operator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/quantum_operator/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/quantum_operator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.187305 qulacs-0.6.2/pysrc/qulacs/state/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/state/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/state/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/state.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.187305 qulacs-0.6.2/pysrc/qulacs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/utils/conversions_openfermion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.187305 qulacs-0.6.2/pysrc/qulacs/vistest/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/vistest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/vistest/test_vis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.187305 qulacs-0.6.2/pysrc/qulacs/visualizer/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2023-09-13 07:05:24.000000 qulacs-0.6.2/pysrc/qulacs/visualizer/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.183304 qulacs-0.6.2/pysrc/qulacs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14136 2023-09-13 07:05:52.000000 qulacs-0.6.2/pysrc/qulacs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12202 2023-09-13 07:05:52.000000 qulacs-0.6.2/pysrc/qulacs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-13 07:05:52.000000 qulacs-0.6.2/pysrc/qulacs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-13 07:05:51.000000 qulacs-0.6.2/pysrc/qulacs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-09-13 07:05:52.000000 qulacs-0.6.2/pysrc/qulacs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-09-13 07:05:52.000000 qulacs-0.6.2/pysrc/qulacs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.187305 qulacs-0.6.2/python/
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    75574 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/cppsim_wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.187305 qulacs-0.6.2/python/stub-test/
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/stub-test/generate_mypy_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.187305 qulacs-0.6.2/python/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.187305 qulacs-0.6.2/python/tests/multi_cpu/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/tests/multi_cpu/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/tests/multi_cpu/test_state_multi_cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.191305 qulacs-0.6.2/python/tests/single_cpu/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/tests/single_cpu/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/tests/single_cpu/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/tests/single_cpu/test_density_matrix_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    12303 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/tests/single_cpu/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/tests/single_cpu/test_noise_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/tests/single_cpu/test_observable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/tests/single_cpu/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)    17686 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/tests/single_cpu/test_pointer_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/tests/single_cpu/test_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/tests/single_cpu/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2023-09-13 07:05:24.000000 qulacs-0.6.2/python/tests/single_cpu/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.195305 qulacs-0.6.2/script/
--rwxr-xr-x   0 runner    (1001) docker     (127)      303 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/build_clang.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      691 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/build_gcc.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      440 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/build_gcc_with_gpu.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      441 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/build_gcc_with_memory_sanitizer.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      122 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/build_mpicc.sh
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/build_msvc_2015.bat
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/build_msvc_2015_with_gpu.bat
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/build_msvc_2017.bat
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/build_msvc_2017_with_gpu.bat
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/build_msvc_2019.bat
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/build_msvc_2019_with_gpu.bat
--rwxr-xr-x   0 runner    (1001) docker     (127)      127 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/clean.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/download_wheel.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      318 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/fix_wheel_osx.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      141 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/format.sh
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/generate_msvc_project_2015.bat
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/generate_msvc_project_2015_with_gpu.bat
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/generate_msvc_project_2017.bat
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/generate_msvc_project_2017_with_gpu.bat
--rwxr-xr-x   0 runner    (1001) docker     (127)      166 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/generate_msvc_project_2019.bat
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/generate_msvc_project_2019_with_gpu.bat
--rwxr-xr-x   0 runner    (1001) docker     (127)      430 2023-09-13 07:05:24.000000 qulacs-0.6.2/script/update_stubs.sh
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-09-13 07:05:52.231306 qulacs-0.6.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5242 2023-09-13 07:05:24.000000 qulacs-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.195305 qulacs-0.6.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.203305 qulacs-0.6.2/src/cppsim/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20392 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/circuit.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    24277 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/circuit.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/circuit_builder.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/circuit_optimizer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/circuit_optimizer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9609 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/exception.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    32399 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19956 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_factory.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    24644 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_general.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13445 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_matrix_diagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_matrix_diagonal.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_matrix_sparse.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_matrix_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20532 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_merge.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_merge.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_named_npair.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_named_one.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    16353 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_named_one.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7977 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_named_pauli.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8986 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_named_two.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23274 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_noisy_evolution.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12950 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_noisy_evolution.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_reflect.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_reversible.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/gate_to_gqo.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    36921 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/general_quantum_operator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14781 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/general_quantum_operator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14140 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/matrix_decomposition.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7033 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/noisesimulator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/noisesimulator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13716 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/observable.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/observable.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14801 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/pauli_operator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/pauli_operator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      830 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/qubit_info.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7181 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/qubit_info.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/simulator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/simulator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/state.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    34493 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/state.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5116 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/state_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/state_dm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/state_gpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15703 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/state_gpu.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/type.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10550 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/utility.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/cppsim/utility.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.211305 qulacs-0.6.2/src/csim/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7145 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/MPIutil.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/MPIutil.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/constant.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/constant.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/init_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/init_ops_fill.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/init_ops_random.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/memory_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/memory_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/memory_ops_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/memory_ops_dm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/stat_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/stat_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10432 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/stat_ops_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/stat_ops_dm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    30440 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/stat_ops_expectation_value.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/stat_ops_probability.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/stat_ops_transition_amplitude.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/type.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    60932 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7802 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_control_multi_target_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14209 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_control_multi_target_single.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_control_single_target_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19452 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_control_single_target_single.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    34691 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_dm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    82604 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_matrix_dense_double.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_matrix_dense_double_eigen.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_matrix_dense_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_matrix_dense_multi_eigen.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    17967 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_matrix_dense_single.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_matrix_diagonal_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_matrix_diagonal_single.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_matrix_phase_single.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_named.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_named_CNOT.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_named_CZ.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12677 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_named_FusedSWAP.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_named_H.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_named_SWAP.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_named_X.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9384 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_named_Y.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_named_Z.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_named_projection.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_named_state.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    16633 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_pauli_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_pauli_single.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_qft.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      705 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_reflection.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/update_ops_reversible_boolean.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/utility.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/csim/utility.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.215305 qulacs-0.6.2/src/gpusim/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/memory_ops.cu
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/memory_ops.h
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/memory_ops_device_functions.h
--rw-r--r--   0 runner    (1001) docker     (127)    52450 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/stat_ops.cu
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/stat_ops.h
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/stat_ops_device_functions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/update_ops_cuda.h
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/update_ops_cuda_device_functions.h
--rw-r--r--   0 runner    (1001) docker     (127)    69614 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/update_ops_multi.cu
--rw-r--r--   0 runner    (1001) docker     (127)    21139 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/update_ops_named.cu
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/update_ops_single.cu
--rw-r--r--   0 runner    (1001) docker     (127)    24452 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/util.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/util.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/util.h
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/util_common.h
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/util_export.h
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/util_func.h
--rw-r--r--   0 runner    (1001) docker     (127)      359 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/util_type.h
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/gpusim/util_type_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.219305 qulacs-0.6.2/src/vqcsim/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/GradCalculator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      408 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/GradCalculator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      730 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/boolean_formula.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/causalcone_simulator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/differential.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/differential.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/loss_function.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/loss_function.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/optimizer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14300 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/parametric_circuit.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/parametric_circuit.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/parametric_circuit_builder.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/parametric_gate.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/parametric_gate_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      823 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/parametric_gate_factory.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/parametric_simulator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      603 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/parametric_simulator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/parser.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/problem.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2023-09-13 07:05:24.000000 qulacs-0.6.2/src/vqcsim/solver.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.219305 qulacs-0.6.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.223306 qulacs-0.6.2/test/cppsim/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/H2.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_KAK.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    32101 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_circuit.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    34318 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_circuit_multicpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9942 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_circuit_optimize_light.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    57296 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_gate.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    29782 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_gate_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    58300 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_gate_multicpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    23845 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_hamiltonian.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_hamiltonian_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15636 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_hamiltonian_multicpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_mpiutil_multicpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12025 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_noise_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_noisesimulator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    20764 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_noisyevolution.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_pauli_operator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_simulator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11552 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_state.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11267 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_state_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/cppsim/test_state_multicpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.223306 qulacs-0.6.2/test/csim/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/csim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/csim/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/csim/test_memory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/csim/test_omputil.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    26768 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/csim/test_stat.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10235 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/csim/test_update_control.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/csim/test_update_dense.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/csim/test_update_dense_double.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/csim/test_update_diagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/csim/test_update_diagonal_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13376 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/csim/test_update_named.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6955 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/csim/test_update_pauli.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.227306 qulacs-0.6.2/test/gpusim/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/gpusim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      492 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/gpusim/H2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    33345 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/gpusim/test_circuit.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9054 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/gpusim/test_compat_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/gpusim/test_func_memory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    47172 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/gpusim/test_gate.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9409 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/gpusim/test_hamiltonian.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    43543 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/gpusim/test_state.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8633 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/gpusim/test_update_control.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15382 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/gpusim/test_update_dense.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/gpusim/test_update_diagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10371 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/gpusim/test_update_named.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/gpusim/test_update_pauli.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/gpusim/test_util.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.227306 qulacs-0.6.2/test/util/
--rw-r--r--   0 runner    (1001) docker     (127)    13090 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/util/util.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 07:05:52.227306 qulacs-0.6.2/test/vqcsim/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/vqcsim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/vqcsim/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    17741 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/vqcsim/test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2023-09-13 07:05:24.000000 qulacs-0.6.2/test/vqcsim/test_backprop.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.446617 qulacs-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-12-25 09:27:50.000000 qulacs-0.6.3/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.386617 qulacs-0.6.3/.devcontainer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.394616 qulacs-0.6.3/.devcontainer/cpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-12-25 09:27:50.000000 qulacs-0.6.3/.devcontainer/cpu/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2023-12-25 09:27:50.000000 qulacs-0.6.3/.devcontainer/cpu/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.394616 qulacs-0.6.3/.devcontainer/gpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-12-25 09:27:50.000000 qulacs-0.6.3/.devcontainer/gpu/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2023-12-25 09:27:50.000000 qulacs-0.6.3/.devcontainer/gpu/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.386617 qulacs-0.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.394616 qulacs-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2023-12-25 09:27:50.000000 qulacs-0.6.3/.github/workflows/ci_macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2023-12-25 09:27:50.000000 qulacs-0.6.3/.github/workflows/ci_ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-12-25 09:27:50.000000 qulacs-0.6.3/.github/workflows/ci_windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2023-12-25 09:27:50.000000 qulacs-0.6.3/.github/workflows/wheel.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-12-25 09:27:50.000000 qulacs-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-25 09:27:50.000000 qulacs-0.6.3/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.394616 qulacs-0.6.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2023-12-25 09:27:50.000000 qulacs-0.6.3/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16670 2023-12-25 09:27:50.000000 qulacs-0.6.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2023-12-25 09:27:50.000000 qulacs-0.6.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-25 09:27:50.000000 qulacs-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14080 2023-12-25 09:28:15.446617 qulacs-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11068 2023-12-25 09:27:50.000000 qulacs-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11409 2023-12-25 09:27:50.000000 qulacs-0.6.3/README_MPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-25 09:27:50.000000 qulacs-0.6.3/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.394616 qulacs-0.6.3/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/AdaptiveGate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/bench_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/benchmark2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/causalconetest.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/benchmark/circuits/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/circuits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/circuits/quantumvolume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/circuits/qulacsbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/libcppsim_benchmark.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17638 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/libcsim_benchmark.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/merge_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/test_qulacs_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/test_qulacs_2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/cmake_script/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/cmake_script/FetchContent/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-25 09:27:50.000000 qulacs-0.6.3/cmake_script/FetchContent/CMakeLists.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)    38023 2023-12-25 09:27:50.000000 qulacs-0.6.3/cmake_script/FetchContent.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2023-12-25 09:27:50.000000 qulacs-0.6.3/cmake_script/FindAVX2.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2023-12-25 09:27:50.000000 qulacs-0.6.3/cmake_script/FindSVE.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-25 09:27:50.000000 qulacs-0.6.3/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/doc/en/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/doc/en/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.386617 qulacs-0.6.3/doc/en/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/doc/en/source/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_static/images/dojo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_static/images/github.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54241 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_static/images/logo-c-h.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_static/images/slack.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/doc/en/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/doc/en/source/_templates/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/macros.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/method.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/package.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/property.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/footer.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/en/source/apply/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/apply/0_overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   162833 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/apply/5.2_qcl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30093 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/apply/6.2_vqe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    55651 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/apply/6.3_ssvqe.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/en/source/apply/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    59895 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/apply/img/QCL.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/en/source/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)   158374 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/guide/2.0_python_advanced.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/en/source/intro/
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/intro/0_about.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/intro/1_install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/intro/2_faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/intro/3_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)    27329 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/intro/4.1_python_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    26841 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/intro/4.2_cpp_tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/en/source/write/
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/write/0_readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/ja/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.386617 qulacs-0.6.3/doc/ja/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/ja/source/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_static/images/dojo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_static/images/github.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54241 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_static/images/logo-c-h.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_static/images/slack.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/ja/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/ja/source/_templates/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/macros.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.406617 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/method.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/package.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/property.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.406617 qulacs-0.6.3/doc/ja/source/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)    79037 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/guide/2.0_python_advanced.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.406617 qulacs-0.6.3/doc/ja/source/intro/
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/intro/0_about.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/intro/1_install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/intro/2_faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/intro/3_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14702 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/intro/4.1_python_tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)    27502 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/intro/4.2_cpp_tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.406617 qulacs-0.6.3/doc/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/scripts/customdoxygen.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/scripts/doxy-boot.js
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/scripts/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/scripts/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/scripts/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2023-12-25 09:27:50.000000 qulacs-0.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.390617 qulacs-0.6.3/pysrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.406617 qulacs-0.6.3/pysrc/qulacs/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36717 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-25 09:28:15.000000 qulacs-0.6.3/pysrc/qulacs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/circuit/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/circuit/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/circuit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/circuit.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13126 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/converter/qasm_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/gate/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/gate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/gate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/gate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10882 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/gate.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/observable/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/observable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/observable/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/observable/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/observable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/quantum_operator/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/quantum_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/quantum_operator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/quantum_operator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/quantum_operator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/state/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/state/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/state/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/state.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/utils/conversions_openfermion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/vistest/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/vistest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/vistest/test_vis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/visualizer/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.446617 qulacs-0.6.3/pysrc/qulacs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14080 2023-12-25 09:28:15.000000 qulacs-0.6.3/pysrc/qulacs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12305 2023-12-25 09:28:15.000000 qulacs-0.6.3/pysrc/qulacs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-25 09:28:15.000000 qulacs-0.6.3/pysrc/qulacs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-25 09:28:15.000000 qulacs-0.6.3/pysrc/qulacs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-25 09:28:15.000000 qulacs-0.6.3/pysrc/qulacs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-25 09:28:15.000000 qulacs-0.6.3/pysrc/qulacs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    75995 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/cppsim_wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/python/stub-test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/stub-test/generate_mypy_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.414617 qulacs-0.6.3/python/tests/multi_cpu/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/multi_cpu/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/multi_cpu/test_circuit_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/multi_cpu/test_state_multi_cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.414617 qulacs-0.6.3/python/tests/single_cpu/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_density_matrix_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12303 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_noise_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_observable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17686 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_pointer_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.418617 qulacs-0.6.3/script/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      303 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_clang.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      691 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_gcc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      440 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_gcc_with_gpu.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      441 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_gcc_with_memory_sanitizer.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      122 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_mpicc.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_msvc_2015.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_msvc_2015_with_gpu.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_msvc_2017.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_msvc_2017_with_gpu.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_msvc_2019.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_msvc_2019_with_gpu.bat
+-rwxr-xr-x   0 runner    (1001) docker     (127)      127 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/clean.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/download_wheel.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      318 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/fix_wheel_osx.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      141 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/format.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/generate_msvc_project_2015.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/generate_msvc_project_2015_with_gpu.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/generate_msvc_project_2017.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/generate_msvc_project_2017_with_gpu.bat
+-rwxr-xr-x   0 runner    (1001) docker     (127)      166 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/generate_msvc_project_2019.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/generate_msvc_project_2019_with_gpu.bat
+-rwxr-xr-x   0 runner    (1001) docker     (127)      430 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/update_stubs.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2023-12-25 09:28:15.446617 qulacs-0.6.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5242 2023-12-25 09:27:50.000000 qulacs-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.418617 qulacs-0.6.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.426617 qulacs-0.6.3/src/cppsim/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21217 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/circuit.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24688 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/circuit.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/circuit_builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    33866 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/circuit_optimizer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/circuit_optimizer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9609 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/exception.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    32399 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19956 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_factory.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24644 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_general.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13445 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_matrix_diagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_matrix_diagonal.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_matrix_sparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_matrix_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20532 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_merge.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_merge.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_named_npair.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_named_one.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16353 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_named_one.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_named_pauli.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8986 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_named_two.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23276 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_noisy_evolution.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12950 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_noisy_evolution.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_reflect.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_reversible.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_to_gqo.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    36921 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/general_quantum_operator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14781 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/general_quantum_operator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/matrix_decomposition.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7033 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/noisesimulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/noisesimulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13716 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/observable.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/observable.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14801 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/pauli_operator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/pauli_operator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/qubit_info.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7181 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/qubit_info.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/qubit_table.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/qubit_table.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/simulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/simulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/state.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    34497 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/state.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5116 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/state_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/state_dm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/state_gpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15703 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/state_gpu.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/type.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/utility.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/utility.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.430617 qulacs-0.6.3/src/csim/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7145 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/MPIutil.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/MPIutil.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/constant.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/constant.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/init_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/init_ops_fill.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/init_ops_random.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/memory_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/memory_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/memory_ops_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/memory_ops_dm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/stat_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/stat_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10432 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/stat_ops_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/stat_ops_dm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30440 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/stat_ops_expectation_value.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/stat_ops_probability.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/stat_ops_transition_amplitude.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/type.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    60932 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7802 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_control_multi_target_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14209 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_control_multi_target_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_control_single_target_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19452 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_control_single_target_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    34691 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_dm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    82604 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_matrix_dense_double.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_matrix_dense_double_eigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_matrix_dense_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_matrix_dense_multi_eigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17967 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_matrix_dense_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_matrix_diagonal_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_matrix_diagonal_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_matrix_phase_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_CNOT.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_CZ.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12677 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_FusedSWAP.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9614 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_H.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_SWAP.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_X.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9384 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_Y.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_Z.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_projection.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16633 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_pauli_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_pauli_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_qft.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_reflection.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_reversible_boolean.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/utility.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/utility.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.434617 qulacs-0.6.3/src/gpusim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/memory_ops.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/memory_ops.h
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/memory_ops_device_functions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    52450 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/stat_ops.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/stat_ops.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/stat_ops_device_functions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/update_ops_cuda.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/update_ops_cuda_device_functions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    69614 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/update_ops_multi.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    21139 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/update_ops_named.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/update_ops_single.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    24452 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/util.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/util.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/util.h
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/util_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/util_export.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/util_func.h
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/util_type.h
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/util_type_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.438617 qulacs-0.6.3/src/vqcsim/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/GradCalculator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/GradCalculator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/boolean_formula.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/causalcone_simulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/differential.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/differential.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/loss_function.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/loss_function.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/optimizer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14300 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parametric_circuit.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parametric_circuit.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parametric_circuit_builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parametric_gate.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parametric_gate_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parametric_gate_factory.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parametric_simulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parametric_simulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parser.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/problem.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/solver.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.438617 qulacs-0.6.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.442617 qulacs-0.6.3/test/cppsim/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/H2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_KAK.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    32101 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_circuit.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    54983 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_circuit_multicpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9942 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_circuit_optimize_light.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    57300 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_gate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    29782 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_gate_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    58304 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_gate_multicpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23845 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_hamiltonian.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_hamiltonian_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15636 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_hamiltonian_multicpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_mpiutil_multicpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12025 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_noise_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_noisesimulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20764 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_noisyevolution.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_pauli_operator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_simulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11552 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11267 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_state_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_state_multicpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.442617 qulacs-0.6.3/test/csim/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_memory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_omputil.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26768 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_stat.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10235 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_update_control.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_update_dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_update_dense_double.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_update_diagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_update_diagonal_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13376 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_update_named.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6955 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_update_pauli.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.442617 qulacs-0.6.3/test/gpusim/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/H2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    33346 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_circuit.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9054 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_compat_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_func_memory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    47173 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_gate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9409 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_hamiltonian.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    43547 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8633 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_update_control.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15382 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_update_dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_update_diagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10371 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_update_named.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_update_pauli.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_util.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.446617 qulacs-0.6.3/test/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    13090 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/util/util.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.446617 qulacs-0.6.3/test/vqcsim/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/vqcsim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/vqcsim/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17741 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/vqcsim/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/vqcsim/test_backprop.cpp
```

### Comparing `qulacs-0.6.2/.devcontainer/cpu/Dockerfile` & `qulacs-0.6.3/.devcontainer/cpu/Dockerfile`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/.devcontainer/cpu/devcontainer.json` & `qulacs-0.6.3/.devcontainer/cpu/devcontainer.json`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/.devcontainer/gpu/Dockerfile` & `qulacs-0.6.3/.devcontainer/gpu/Dockerfile`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/.devcontainer/gpu/devcontainer.json` & `qulacs-0.6.3/.devcontainer/gpu/devcontainer.json`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/.github/workflows/ci_macos.yml` & `qulacs-0.6.3/.github/workflows/ci_macos.yml`

 * *Files 6% similar despite different names*

```diff
@@ -61,17 +61,17 @@
 
       - name: Install qulacs for macOS
         run: USE_TEST=Yes ./script/build_gcc.sh
 
       - name: Install qulacs Python module
         run: pip install .[ci]
 
-      - name: Test if stub is working
-        run: |
-          python python/stub-test/generate_mypy_tester.py qulacs
-          mypy python/stub-test/names_qulacs.py
+      # - name: Test if stub is working
+      #   run: |
+      #     python python/stub-test/generate_mypy_tester.py qulacs
+      #     mypy python/stub-test/names_qulacs.py
 
       - name: Test in macOS
         run: |
           cd ./build
           make test -j
           make pythontest -j
```

### Comparing `qulacs-0.6.2/.github/workflows/ci_ubuntu.yml` & `qulacs-0.6.3/.github/workflows/ci_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/.github/workflows/ci_windows.yml` & `qulacs-0.6.3/.github/workflows/ci_windows.yml`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/.github/workflows/wheel.yml` & `qulacs-0.6.3/.github/workflows/wheel.yml`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
       - name: Upload wheel to GitHub
         uses: actions/upload-artifact@v3
         with:
           path: ./wheels/*.whl
 
       - name: Upload wheel data if the Git tag is set
-        run: python -m twine upload wheels/*.whl
+        run: python -m twine upload wheels/*.whl --verbose
         if: ${{ contains(github.ref, '/tags/') }}
         env:
           TWINE_PASSWORD: ${{ secrets.TWINE_PASSWORD_QULACS }}
 
   sdist:
     name: Source distribution
     if: ${{ github.event_name == 'push' || github.event_name == 'workflow_dispatch' || github.event.review.state == 'approved' }}
@@ -119,11 +119,11 @@
       - name: Install Python dependencies
         run: python -m pip install twine build
 
       - name: create sdist
         run: python -m build --sdist
 
       - name: Upload sdist data if the Git tag is set
-        run: python -m twine upload dist/*.tar.gz
+        run: python -m twine upload dist/*.tar.gz --verbose
         if: ${{ contains(github.ref, '/tags/') }}
         env:
           TWINE_PASSWORD: ${{ secrets.TWINE_PASSWORD_QULACS }}
```

### Comparing `qulacs-0.6.2/.gitignore` & `qulacs-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/.vscode/tasks.json` & `qulacs-0.6.3/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/CMakeLists.txt` & `qulacs-0.6.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/CONTRIBUTING.md` & `qulacs-0.6.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/LICENSE` & `qulacs-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/PKG-INFO` & `qulacs-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qulacs
-Version: 0.6.2
+Version: 0.6.3
 Summary: Quantum circuit simulator for research
 Author-email: QunaSys <qulacs@qunasys.com>
 License: MIT License
         
         Copyright (c) 2018 Qulacs Authors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,23 +54,23 @@
 Requires-Dist: flake8; extra == "ci"
 Requires-Dist: isort; extra == "ci"
 Requires-Dist: mypy; extra == "ci"
 Requires-Dist: pybind11-stubgen; extra == "ci"
 Requires-Dist: openfermion; extra == "ci"
 Requires-Dist: pytest; extra == "ci"
 Provides-Extra: doc
-Requires-Dist: sphinx==4.5.0; extra == "doc"
-Requires-Dist: sphinx-rtd-theme==1.0.*; extra == "doc"
-Requires-Dist: breathe==4.33.*; extra == "doc"
-Requires-Dist: exhale==0.3.*; extra == "doc"
-Requires-Dist: nbsphinx==0.8.*; extra == "doc"
-Requires-Dist: myst-parser==0.18.*; extra == "doc"
-Requires-Dist: sphinx-copybutton==0.5.*; extra == "doc"
-Requires-Dist: ipykernel==6.17.*; extra == "doc"
-Requires-Dist: sphinx-autoapi==2.0.*; extra == "doc"
+Requires-Dist: sphinx==7.*; extra == "doc"
+Requires-Dist: sphinx-rtd-theme; extra == "doc"
+Requires-Dist: breathe; extra == "doc"
+Requires-Dist: exhale; extra == "doc"
+Requires-Dist: nbsphinx; extra == "doc"
+Requires-Dist: myst-parser; extra == "doc"
+Requires-Dist: sphinx-copybutton; extra == "doc"
+Requires-Dist: ipykernel; extra == "doc"
+Requires-Dist: sphinx-autoapi==3.*; extra == "doc"
 
 # Qulacs
 
 [![Ubuntu CI](https://github.com/qulacs/qulacs/actions/workflows/ci_ubuntu.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/ci_ubuntu.yml)
 [![macOS CI](https://github.com/qulacs/qulacs/actions/workflows/ci_macos.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/ci_macos.yml)
 [![Windows CI](https://github.com/qulacs/qulacs/actions/workflows/ci_windows.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/ci_windows.yml)
 [![Wheel build](https://github.com/qulacs/qulacs/actions/workflows/wheel.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/wheel.yml)
```

### Comparing `qulacs-0.6.2/README.md` & `qulacs-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/README_MPI.md` & `qulacs-0.6.3/README_MPI.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
   - state.load(vector)
     - In the case state vector distributed in multi nodes, load to the element with each rank.
 
   - state.get_vector()
     - In the case state vector distributed in multi nodes, returns the elements that each rank has.
 
-  - Automatic FusedSWAP gate insertion of QuantumCircuitOptimizer  // not supported yet
+  - Automatic FusedSWAP gate insertion of QuantumCircuitOptimizer
     - optimize(circuit, block_size, swap_level=0)
       - swap_level = 0
         - No SWAP/FusedSWAP gate insertion
       - swap_level = 1
         - Insert SWAP/FusedSWAP gates to reduce communication without changing gate order
       - swap_level = 2
         - Insert SWAP/FusedSWAP gates to reduce communication with changing gate order
@@ -287,21 +287,21 @@
       - merge
       - to_matrix_gate
       - DenseMatrix gate (number of qubits <= number of local qubits)
       - DiagonalMatrix gate (single target)
   - GeneralQuantumOperator (w/o get_transition_amplitude)
   - Observable (w/o get_transition_amplitude)
   - PauliOperator (w/o get_transition_amplitude)
+  - QuantumCircuitOptimizer
+      - optimize
+      - optimize_light
 
 ## Additional info
 
 - Might be supported in future (T.B.D.)
-  - QuantumCircuitOptimizer
-      - optimize
-      - optimize_light
   - ParametricQuantumCircuit
   - gate
       - Measurement
       - merge (number of qubits > number of local qubits)
       - CPTP
       - Instrument
       - Adaptive
```

### Comparing `qulacs-0.6.2/benchmark/AdaptiveGate.py` & `qulacs-0.6.3/benchmark/AdaptiveGate.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/benchmark/bench_circuit.py` & `qulacs-0.6.3/benchmark/bench_circuit.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,21 @@
     argparser.add_argument(
         "-o",
         "--opt",
         type=int,
         default=-1,
         help="Enable QuantumCircuitOptimizer: 99 is to use optmize_light(), 0-6 is to use optimize(). (default no-use)",
     )
-    # argparser.add_argument('-f', '--fused', type = int,
-    #        default = -1, help = 'Enable QuantumCircuitOptimizer: 0 is not to use, 1-2 is to use Fused-swap opt')
+    argparser.add_argument(
+        "-f",
+        "--fused",
+        type=int,
+        default=-1,
+        help="Enable QuantumCircuitOptimizer: 0 is not to use, 1-2 is to use Fused-swap opt",
+    )
     argparser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         help="Verbose switch, Output circuit infomations",
     )
     argparser.add_argument("-s", "--seed", type=int, default=-1, help="Random Seed")
@@ -96,42 +101,39 @@
         np.random.seed(seed)
         rng = np.random.default_rng(seed=seed)
 
     # make a quantum circuit
     circuit = get_circuit(
         args.circuit,
         nqubits=args.nqubits,
-        global_nqubits=num_global_qubits,
-        # global_nqubits = 0 if args.fused >= 0 else num_global_qubits,
+        global_nqubits=0 if args.fused >= 0 else num_global_qubits,
         depth=args.depth,
         verbose=(args.verbose and (mpirank == 0)),
         random_gen=rng,
     )
 
     if args.check:
         circuit_ref = circuit.copy()
     if args.opt == 99:
-        # if args.fused == -1:
-        QCO().optimize_light(circuit)
-    # else:
-    #    QCO().optimize_light(circuit, args.fused)
+        if args.fused == -1:
+            QCO().optimize_light(circuit)
+        else:
+            QCO().optimize_light(circuit, args.fused)
     elif args.opt >= 0:
-        # if args.fused == -1:
-        QCO().optimize(circuit, args.opt)
-    # else:
-    #    QCO().optimize(circuit, args.opt, args.fused)
+        if args.fused == -1:
+            QCO().optimize(circuit, args.opt)
+        else:
+            QCO().optimize(circuit, args.opt, args.fused)
 
     if mpirank == 0:
         print(
             "# A quantum circuit was created. ",
             args.circuit,
             f"nqubits= {args.nqubits} depth= {args.depth}",
-            #        "optimize =", (args.opt, args.fused), elapsed())
-            "optimize=",
-            args.opt,
+            " optimize= {args.opt, args.fused}",
             elapsed(),
         )
         print(circuit)
 
     # update the state vector
     circuit.update_quantum_state(st)
     mpicomm.barrier()
```

### Comparing `qulacs-0.6.2/benchmark/causalconetest.cpp` & `qulacs-0.6.3/benchmark/causalconetest.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/benchmark/circuits/quantumvolume.py` & `qulacs-0.6.3/benchmark/circuits/quantumvolume.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/benchmark/circuits/qulacsbench.py` & `qulacs-0.6.3/benchmark/circuits/qulacsbench.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/benchmark/libcppsim_benchmark.cpp` & `qulacs-0.6.3/benchmark/libcppsim_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/benchmark/libcsim_benchmark.cpp` & `qulacs-0.6.3/benchmark/libcsim_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/benchmark/test_qulacs_1.py` & `qulacs-0.6.3/benchmark/test_qulacs_1.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/benchmark/test_qulacs_2.py` & `qulacs-0.6.3/benchmark/test_qulacs_2.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/cmake_script/FetchContent/CMakeLists.cmake.in` & `qulacs-0.6.3/cmake_script/FetchContent/CMakeLists.cmake.in`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/cmake_script/FetchContent.cmake` & `qulacs-0.6.3/cmake_script/FetchContent.cmake`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/cmake_script/FindAVX2.cmake` & `qulacs-0.6.3/cmake_script/FindAVX2.cmake`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/cmake_script/FindSVE.cmake` & `qulacs-0.6.3/cmake_script/FindSVE.cmake`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/.gitignore` & `qulacs-0.6.3/doc/.gitignore`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/Makefile` & `qulacs-0.6.3/doc/en/Makefile`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/make.bat` & `qulacs-0.6.3/doc/en/make.bat`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/_static/images/dojo.png` & `qulacs-0.6.3/doc/en/source/_static/images/dojo.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/_static/images/github.png` & `qulacs-0.6.3/doc/en/source/_static/images/github.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/_static/images/logo-c-h.png` & `qulacs-0.6.3/doc/en/source/_static/images/logo-c-h.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/_static/images/slack.png` & `qulacs-0.6.3/doc/en/source/_static/images/slack.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/_templates/autoapi/python/class.rst` & `qulacs-0.6.3/doc/en/source/_templates/autoapi/python/class.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/_templates/autoapi/python/data.rst` & `qulacs-0.6.3/doc/en/source/_templates/autoapi/python/data.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/_templates/autoapi/python/function.rst` & `qulacs-0.6.3/doc/en/source/_templates/autoapi/python/function.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/_templates/autoapi/python/method.rst` & `qulacs-0.6.3/doc/en/source/_templates/autoapi/python/method.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/_templates/autoapi/python/module.rst` & `qulacs-0.6.3/doc/en/source/_templates/autoapi/python/module.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/apply/0_overview.ipynb` & `qulacs-0.6.3/doc/en/source/apply/0_overview.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/apply/5.2_qcl.ipynb` & `qulacs-0.6.3/doc/en/source/apply/5.2_qcl.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/apply/6.2_vqe.ipynb` & `qulacs-0.6.3/doc/en/source/apply/6.2_vqe.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/apply/6.3_ssvqe.ipynb` & `qulacs-0.6.3/doc/en/source/apply/6.3_ssvqe.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/apply/img/QCL.png` & `qulacs-0.6.3/doc/en/source/apply/img/QCL.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/conf.py` & `qulacs-0.6.3/doc/en/source/conf.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/guide/2.0_python_advanced.ipynb` & `qulacs-0.6.3/doc/en/source/guide/2.0_python_advanced.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998985138088223%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(4, 'del state\\n')], delete: [4]}}, 5: {'source': {insert: "*

 * *            "[(7, 'print(state.get_amplitude(2))\\n')], delete: [7]}}, 7: {'source': {insert: [(6, "*

 * *            "'    # some computation and get results\\n')], delete: [6]}}, 9: {'source': {insert: "*

 * *            '[(9, \'print("restored:", r_state.get_vector())\\n\')], delete: [9]}}, 11: '*

 * *            "{'source': {insert: [(11, '    state = pickle.load(f)\\n')], delete: [11]}}, 13: "*

 * *            "{'source': { […]*

```diff
@@ -50,15 +50,15 @@
                 }
             ],
             "source": [
                 "from qulacs import QuantumState\n",
                 "n = 2\n",
                 "state = QuantumState(n)\n",
                 "print(state)\n",
-                "del state"
+                "del state\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -86,15 +86,15 @@
                 "from qulacs import QuantumState\n",
                 "\n",
                 "state = QuantumState(2)\n",
                 "vec = state.get_vector()\n",
                 "print(vec)\n",
                 "state.load([0,1,2,3])\n",
                 "print(state.get_vector())\n",
-                "print(state.get_amplitude(2))"
+                "print(state.get_amplitude(2))\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -110,15 +110,15 @@
             "source": [
                 "from qulacs import QuantumState\n",
                 "\n",
                 "initial_state = QuantumState(3)\n",
                 "buffer = initial_state.allocate_buffer()\n",
                 "for ind in range(10):\n",
                 "    buffer.load(initial_state)\n",
-                "    # some computation and get results"
+                "    # some computation and get results\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -149,15 +149,15 @@
                 "\n",
                 "o_state = QuantumState(2)\n",
                 "o_state.set_Haar_random_state()\n",
                 "print(\"original:\", o_state.get_vector())\n",
                 "state_json = o_state.to_json()\n",
                 "\n",
                 "r_state = state.from_json(state_json)\n",
-                "print(\"restored:\", r_state.get_vector())"
+                "print(\"restored:\", r_state.get_vector())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -177,15 +177,15 @@
                 "\n",
                 "# store\n",
                 "with open('state.pickle', 'wb') as f:\n",
                 "    pickle.dump(state, f)\n",
                 "\n",
                 "# load\n",
                 "with open('state.pickle', 'rb') as f:\n",
-                "    state = pickle.load(f)"
+                "    state = pickle.load(f)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -222,15 +222,15 @@
                 "# Initialize the specified value to the calculation base in binary notation\n",
                 "state.set_computational_basis(0b101)\n",
                 "print(state.get_vector())\n",
                 "\n",
                 "# Initialize to random pure state with Haar measure using argument value as seed\n",
                 "# If no value is specified, the time function is used as a seed. Pseudo random number uses xorshift.\n",
                 "state.set_Haar_random_state(0)\n",
-                "print(state.get_vector())"
+                "print(state.get_vector())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -298,15 +298,15 @@
                 "# You can supply a random seed as second argument.\n",
                 "# If the same seed is given, always returns the same sampling result.\n",
                 "samples_with_seed = state.sampling(10, 314)\n",
                 "print(\"sampling (with seed)\", samples_with_seed)\n",
                 "\n",
                 "# Get a character string indicating whether the state vector is on CPU or GPU\n",
                 "dev_type = state.get_device_name()\n",
-                "print(\"device\", dev_type)"
+                "print(\"device\", dev_type)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -368,15 +368,15 @@
                 "\n",
                 "# Normalize quantum states\n",
                 "# Provide the current squared norm as an argument.\n",
                 "squared_norm = state.get_squared_norm()\n",
                 "print(\"sq_norm\", squared_norm)\n",
                 "state.normalize(squared_norm)\n",
                 "print(\"normalized\", state.get_vector())\n",
-                "print(\"sq_norm\", state.get_squared_norm())"
+                "print(\"sq_norm\", state.get_squared_norm())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -401,15 +401,15 @@
                 "from qulacs import QuantumState\n",
                 "state = QuantumState(3)\n",
                 "position = 0\n",
                 "# Write the value to `position`-th register\n",
                 "state.set_classical_value(position, 20)\n",
                 "# Get the value of the `position`-th register\n",
                 "obtained = state.get_classical_value(position)\n",
-                "print(obtained)"
+                "print(obtained)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -450,15 +450,15 @@
                 "state_ket1.set_computational_basis(1)\n",
                 "n2 = 2\n",
                 "state_ket2 = QuantumState(n2)\n",
                 "state_ket2.set_computational_basis(2)\n",
                 "\n",
                 "# Calculation of tensor product\n",
                 "tensor_product_state = tensor_product(state_ket1, state_ket2)\n",
-                "print(tensor_product_state.get_vector())"
+                "print(tensor_product_state.get_vector())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -511,15 +511,15 @@
                 "n = 3\n",
                 "state = QuantumState(n)\n",
                 "state.set_Haar_random_state()\n",
                 "print(\"original:\", state.get_vector())\n",
                 "state0 = drop_qubit(state, [1], [0])\n",
                 "print(\"projection to 0:\", state0.get_vector()) # projection: qubit 1 is 0\n",
                 "state1 = drop_qubit(state, [1], [1])\n",
-                "print(\"projection to 1:\", state1.get_vector()) # projection: qubit 1 is 1"
+                "print(\"projection to 1:\", state1.get_vector()) # projection: qubit 1 is 1\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -575,15 +575,15 @@
                 "dm_state = DensityMatrix(3)\n",
                 "dm_state.set_computational_basis(0)\n",
                 "H(0).update_quantum_state(dm_state)\n",
                 "X(1).update_quantum_state(dm_state)\n",
                 "print(dm_state.get_matrix())\n",
                 "\n",
                 "trace = partial_trace(dm_state, [1])\n",
-                "print(trace.get_matrix())"
+                "print(trace.get_matrix())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -654,15 +654,15 @@
                 }
             ],
             "source": [
                 "from qulacs import QuantumState\n",
                 "n = 2\n",
                 "state = DensityMatrix(n)\n",
                 "print(state)\n",
-                "del state"
+                "del state\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -701,15 +701,15 @@
                 "\n",
                 "state = DensityMatrix(2)\n",
                 "mat = state.get_matrix()\n",
                 "print(mat)\n",
                 "state.load([0,1,2,3])\n",
                 "print(state.get_matrix())\n",
                 "state.load([[0,1,2,3], [1,2,3,4], [2,3,4,5], [3,4,5,6]])\n",
-                "print(state.get_matrix())"
+                "print(state.get_matrix())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -728,15 +728,15 @@
                 "from qulacs import QuantumState, DensityMatrix\n",
                 "\n",
                 "initial_state = DensityMatrix(3)\n",
                 "copied_state = initial_state.copy()\n",
                 "buffer = initial_state.allocate_buffer()\n",
                 "buffer.load(initial_state)\n",
                 "state_vector = QuantumState(3)\n",
-                "buffer.load(state_vector)"
+                "buffer.load(state_vector)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -778,15 +778,15 @@
                 "\n",
                 "o_state = DensityMatrix(2)\n",
                 "o_state.set_Haar_random_state()\n",
                 "print(\"original:\", o_state.get_matrix())\n",
                 "state_json = o_state.to_json()\n",
                 "\n",
                 "r_state = state.from_json(state_json)\n",
-                "print(\"restored:\", r_state.get_matrix())"
+                "print(\"restored:\", r_state.get_matrix())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -806,15 +806,15 @@
                 "\n",
                 "# store\n",
                 "with open('state.pickle', 'wb') as f:\n",
                 "    pickle.dump(state, f)\n",
                 "\n",
                 "# load\n",
                 "with open('state.pickle', 'rb') as f:\n",
-                "    state = pickle.load(f)"
+                "    state = pickle.load(f)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -865,15 +865,15 @@
                 "print(state.get_matrix())\n",
                 "\n",
                 "\n",
                 "# Initialize as a random pure state in Haar measure with the seed given as an argument.\n",
                 "# If you do not give the seed, `time` function is used for seed.\n",
                 "# Xorshift is used for psuedo random.\n",
                 "state.set_Haar_random_state(0)\n",
-                "print(state.get_matrix())"
+                "print(state.get_matrix())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -941,15 +941,15 @@
                 "# You can supply a random seed as second argument.\n",
                 "# If the same seed is given, always returns the same sampling result.\n",
                 "samples_with_seed = state.sampling(10, 314)\n",
                 "print(\"sampling (with seed)\", samples_with_seed)\n",
                 "\n",
                 "# Get a character string indicating whether the state vector is on CPU or GPU\n",
                 "dev_type = state.get_device_name()\n",
-                "print(\"device\", dev_type)"
+                "print(\"device\", dev_type)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1023,15 +1023,15 @@
                 "\n",
                 "# Normalize quantum states\n",
                 "# Provide the current squared norm as an argument.\n",
                 "squared_norm = state.get_squared_norm()\n",
                 "print(\"sq_norm\", squared_norm)\n",
                 "state.normalize(squared_norm)\n",
                 "print(\"normalized\", state.get_matrix())\n",
-                "print(\"sq_norm\", state.get_squared_norm())"
+                "print(\"sq_norm\", state.get_squared_norm())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1056,15 +1056,15 @@
                 "from qulacs import DensityMatrix\n",
                 "state = DensityMatrix(3)\n",
                 "position = 0\n",
                 "# Set the value at `position`-th register.\n",
                 "state.set_classical_value(position, 20)\n",
                 "# Get the value at `position`-th register.\n",
                 "obtained = state.get_classical_value(position)\n",
-                "print(obtained)"
+                "print(obtained)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1108,15 +1108,15 @@
                 "a = QuantumState(2)\n",
                 "a.set_computational_basis(0b00)\n",
                 "b = DensityMatrix(2)\n",
                 "b.set_computational_basis(0b11)\n",
                 "p = 1 / 2\n",
                 "q = 1 / 2\n",
                 "c = make_mixture(p, a, q, b)\n",
-                "print(c.get_matrix())"
+                "print(c.get_matrix())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1160,15 +1160,15 @@
             ],
             "source": [
                 "import numpy as np\n",
                 "from qulacs.gate import X\n",
                 "gate = X(2)\n",
                 "mat = gate.get_matrix()\n",
                 "print(mat)\n",
-                "print(gate)"
+                "print(gate)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1215,15 +1215,15 @@
                 "from qulacs import gate\n",
                 "\n",
                 "o_gate = X(2)\n",
                 "print(o_gate)\n",
                 "gate_json = o_gate.to_json()\n",
                 "\n",
                 "r_gate = gate.from_json(gate_json)\n",
-                "print(r_gate)"
+                "print(r_gate)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1269,15 +1269,15 @@
                 "from qulacs.gate import X\n",
                 "\n",
                 "n = 2\n",
                 "initial_gate = X(n)\n",
                 "print(initial_gate)\n",
                 "\n",
                 "copied_gate = initial_gate.copy()\n",
-                "print(copied_gate)"
+                "print(copied_gate)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The `update_quantum_state` function is used to change the quantum state by a quantum gate.\n",
@@ -1314,15 +1314,15 @@
                 "\n",
                 "quantum_state.set_zero_state()\n",
                 "\n",
                 "hadamard_gate = H(0)\n",
                 "\n",
                 "hadamard_gate.update_quantum_state(quantum_state)\n",
                 "\n",
-                "print(quantum_state)"
+                "print(quantum_state)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Special gate\n",
@@ -1359,15 +1359,15 @@
                 "from qulacs.gate import Identity # Identity matrix\n",
                 "from qulacs.gate import X, Y, Z\t# Pauli\n",
                 "from qulacs.gate import H, S, Sdag, sqrtX, sqrtXdag, sqrtY, sqrtYdag # \u30af\u30ea\u30d5\u30a9\u30fc\u30c9\n",
                 "from qulacs.gate import T, Tdag # T gate\n",
                 "from qulacs.gate import P0, P1 # Projection to 0,1 (not normalized)\n",
                 "target = 3\n",
                 "gate = T(target)\n",
-                "print(gate)"
+                "print(gate)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1405,15 +1405,15 @@
             "source": [
                 "import numpy as np\n",
                 "from qulacs.gate import RX, RY, RZ\n",
                 "target = 0\n",
                 "angle = 0.1\n",
                 "gate = RX(target, angle)\n",
                 "print(gate)\n",
-                "print(gate.get_matrix())"
+                "print(gate.get_matrix())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1484,15 +1484,15 @@
                         " (0.0489829,0.00992933)     (0.876486,0.478826)\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
                 "from qulacs.gate import U1,U2,U3\n",
-                "print(U3(0, 0.1, 0.2, 0.3))"
+                "print(U3(0, 0.1, 0.2, 0.3))\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1536,15 +1536,15 @@
                 "from qulacs.gate import CNOT, CZ, SWAP\n",
                 "control = 5\n",
                 "target = 2\n",
                 "target2 = 3\n",
                 "gate = CNOT(control, target)\n",
                 "print(gate)\n",
                 "gate = CZ(control, target)\n",
-                "gate = SWAP(target, target2)"
+                "gate = SWAP(target, target2)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1587,15 +1587,15 @@
             ],
             "source": [
                 "from qulacs.gate import Pauli\n",
                 "target_list = [0,3,5]\n",
                 "pauli_index = [1,3,1] # 1:X , 2:Y, 3:Z\n",
                 "gate = Pauli(target_list, pauli_index) # = X_0 Z_3 X_5\n",
                 "print(gate)\n",
-                "print(gate.get_matrix())"
+                "print(gate.get_matrix())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1632,15 +1632,15 @@
             "source": [
                 "from qulacs.gate import PauliRotation\n",
                 "target_list = [0,3,5]\n",
                 "pauli_index = [1,3,1] # 1:X , 2:Y, 3:Z\n",
                 "angle = 0.5\n",
                 "gate = PauliRotation(target_list, pauli_index, angle) # = exp(i angle/2 X_0 Z_3 X_5)\n",
                 "print(gate)\n",
-                "print(gate.get_matrix().shape)"
+                "print(gate.get_matrix().shape)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1681,15 +1681,15 @@
                 "target_list = [0,1]\n",
                 "gate = ReversibleBoolean(target_list, upper)\n",
                 "print(gate)\n",
                 "state = QuantumState(3)\n",
                 "state.load(np.arange(2**3))\n",
                 "print(state.get_vector())\n",
                 "gate.update_quantum_state(state)\n",
-                "print(state.get_vector())"
+                "print(state.get_vector())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1723,15 +1723,15 @@
                 "axis.set_Haar_random_state(0)\n",
                 "state = QuantumState(2)\n",
                 "gate = StateReflection(axis)\n",
                 "gate.update_quantum_state(state)\n",
                 "print(\"axis\", axis.get_vector())\n",
                 "print(\"reflected\", state.get_vector())\n",
                 "gate.update_quantum_state(state)\n",
-                "print(\"two reflection\", state.get_vector())"
+                "print(\"two reflection\", state.get_vector())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1790,15 +1790,15 @@
                 "\n",
                 "# 1-qubit gate\n",
                 "gate = DenseMatrix(0, [[0,1],[1,0]])\n",
                 "print(gate)\n",
                 "\n",
                 "# 2-qubit gate\n",
                 "gate = DenseMatrix([0,1], [[1,0,0,0],[0,1,0,0],[0,0,0,1],[0,0,1,0]])\n",
-                "print(gate)"
+                "print(gate)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1845,15 +1845,15 @@
                 "\n",
                 "gate = SparseMatrix([0], mat)\n",
                 "print(gate)\n",
                 "\n",
                 "qs = QuantumState(2)\n",
                 "qs.load([1,2,3,4])\n",
                 "gate.update_quantum_state(qs)\n",
-                "print(qs.get_vector())"
+                "print(qs.get_vector())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1906,15 +1906,15 @@
                 "\n",
                 "from qulacs import QuantumState\n",
                 "state = QuantumState(3)\n",
                 "state.load(np.arange(2**3))\n",
                 "print(state.get_vector())\n",
                 "\n",
                 "x_mat_gate.update_quantum_state(state)\n",
-                "print(state.get_vector())"
+                "print(state.get_vector())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1962,15 +1962,15 @@
                 "x_gate = X(index)\n",
                 "angle = np.pi / 4.0\n",
                 "ry_gate = RY(index, angle)\n",
                 "\n",
                 "# Create the new gate by combining gates\n",
                 "# The gate in the first augement is applied first\n",
                 "x_and_ry_gate = merge(x_gate, ry_gate)\n",
-                "print(x_and_ry_gate)"
+                "print(x_and_ry_gate)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -2035,15 +2035,15 @@
                 "print(proj_00_or_11)\n",
                 "\n",
                 "gate_ii_zz = add(Identity(0), merge(Z(0),Z(1)))\n",
                 "gate_ii_xx = add(Identity(0), merge(X(0),X(1)))\n",
                 "proj_00_plus_11 = merge(gate_ii_zz, gate_ii_xx)\n",
                 "# ((|00>+|11>)(<00|+<11|))/2 = (II + ZZ)(II + XX)/4\n",
                 "proj_00_plus_11.multiply_scalar(0.25)\n",
-                "print(proj_00_plus_11)"
+                "print(proj_00_plus_11)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -2080,15 +2080,15 @@
                     ]
                 }
             ],
             "source": [
                 "from qulacs.gate import RandomUnitary\n",
                 "target_list = [2,3]\n",
                 "gate = RandomUnitary(target_list)\n",
-                "print(gate)"
+                "print(gate)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -2135,15 +2135,15 @@
                 "gate = Probabilistic(distribution, gate_list)\n",
                 "print(gate)\n",
                 "\n",
                 "from qulacs import QuantumState\n",
                 "state = QuantumState(2)\n",
                 "for _ in range(10):\n",
                 "    gate.update_quantum_state(state)\n",
-                "    print(state.get_vector())"
+                "    print(state.get_vector())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -2183,15 +2183,15 @@
                 "gate = DepolarizingNoise(target, error_prob) # X,Y,Z : prob/3\n",
                 "gate = TwoQubitDepolarizingNoise(target, second_target, error_prob) # {I,X,Y,Z} \\times {I,X,Y,Z} \\setminus {II} : prob/15\n",
                 "\n",
                 "from qulacs import QuantumState\n",
                 "state = QuantumState(2)\n",
                 "for _ in range(10):\n",
                 "    gate.update_quantum_state(state)\n",
-                "    print(state.get_vector())"
+                "    print(state.get_vector())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3259,15 +3259,15 @@
                 "state = QuantumState(n)\n",
                 "for k in range(n_samples):\n",
                 "   state.set_zero_state()\n",
                 "   H(0).update_quantum_state(state)\n",
                 "   H(1).update_quantum_state(state)\n",
                 "   gate.update_quantum_state(state)\n",
                 "   exp += observable.get_expectation_value(state) / n_samples\n",
-                "   print(f\"[{k}] exp: {exp}\")"
+                "   print(f\"[{k}] exp: {exp}\")\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3311,15 +3311,15 @@
                 "from qulacs import QuantumState\n",
                 "from qulacs.gate import H,merge\n",
                 "state = QuantumState(2)\n",
                 "for _ in range(10):\n",
                 "    state.set_zero_state()\n",
                 "    merge(H(0),H(1)).update_quantum_state(state)\n",
                 "    gate.update_quantum_state(state)\n",
-                "    print(state.get_vector())"
+                "    print(state.get_vector())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3351,15 +3351,15 @@
                 }
             ],
             "source": [
                 "from qulacs.gate import AmplitudeDampingNoise\n",
                 "target = 0\n",
                 "damping_rate = 0.1\n",
                 "AmplitudeDampingNoise(target, damping_rate) \n",
-                "#K_0: [[1,0],[0,sqrt(1-p)]], K_1: [[0,sqrt(p)], [0,0]]"
+                "#K_0: [[1,0],[0,sqrt(1-p)]], K_1: [[0,sqrt(p)], [0,0]]\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3406,15 +3406,15 @@
                 "from qulacs.gate import H,merge\n",
                 "state = QuantumState(2)\n",
                 "for index in range(10):\n",
                 "    state.set_zero_state()\n",
                 "    merge(H(0),H(1)).update_quantum_state(state)\n",
                 "    gate.update_quantum_state(state)\n",
                 "    result = state.get_classical_value(classical_pos)\n",
-                "    print(index, format(result,\"b\").zfill(2), state.get_vector())"
+                "    print(index, format(result,\"b\").zfill(2), state.get_vector())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3426,15 +3426,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from qulacs.gate import Measurement\n",
                 "target = 0\n",
                 "classical_pos = 0\n",
-                "gate = Measurement(target, classical_pos)"
+                "gate = Measurement(target, classical_pos)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3475,15 +3475,15 @@
                 "state.set_classical_value(0,0)\n",
                 "gate.update_quantum_state(state)\n",
                 "print(state.get_vector())\n",
                 "\n",
                 "# func returns True, so X operates\n",
                 "state.set_classical_value(0,1)\n",
                 "gate.update_quantum_state(state)\n",
-                "print(state.get_vector())"
+                "print(state.get_vector())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3506,17 +3506,23 @@
                     "text": [
                         "(0.1+0j) X0 Y1 Z3 Y3\n"
                     ]
                 }
             ],
             "source": [
                 "from qulacs import PauliOperator\n",
+                "# Create Pauli Operator from pauli_string\n",
                 "coef = 0.1\n",
                 "s = \"X 0 Y 1 Z 3\"\n",
                 "pauli = PauliOperator(s, coef)\n",
+                "# Or, from index_list and type_list\n",
+                "coef =  0.1\n",
+                "index_list = [0, 1, 3]\n",
+                "type_list = \"XYZ\"\n",
+                "pauli = PauliOperator(index_list, type_list, coef)\n",
                 "\n",
                 "# Added pauli symbol later\n",
                 "pauli.add_single_Pauli(3, 2)\n",
                 "\n",
                 "# Get the subscript of each pauli symbol\n",
                 "index_list = pauli.get_index_list()\n",
                 "\n",
@@ -3529,15 +3535,15 @@
                 "# Create a copy of pauli operator\n",
                 "another_pauli = pauli.copy()\n",
                 "\n",
                 "s = [\"I\",\"X\",\"Y\",\"Z\"]\n",
                 "pauli_str = [s[i] for i in pauli_id_list]\n",
                 "terms_str = [item[0]+str(item[1]) for item in zip(pauli_str,index_list)]\n",
                 "full_str = str(coef) + \" \" + \" \".join(terms_str)\n",
-                "print(full_str)"
+                "print(full_str)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3574,15 +3580,15 @@
                 "print(\"expect\", value)\n",
                 "\n",
                 "# Calculate transition moment <a|H|b>\n",
                 "# The first arguments comes to the bra side\n",
                 "bra = QuantumState(n)\n",
                 "bra.set_Haar_random_state()\n",
                 "value = pauli.get_transition_amplitude(bra, state)\n",
-                "print(\"transition\", value)"
+                "print(\"transition\", value)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3637,15 +3643,15 @@
                 "print(\"expect\", value)\n",
                 "\n",
                 "# Transition moment calculation <a|H|b>\n",
                 "# The first arguments comes to the bra side\n",
                 "bra = QuantumState(n)\n",
                 "bra.set_Haar_random_state()\n",
                 "value = operator.get_transition_amplitude(bra, state)\n",
-                "print(\"transition\", value)"
+                "print(\"transition\", value)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Store linear operators\n",
@@ -3673,15 +3679,15 @@
                 "o_operator = GeneralQuantumOperator(3)\n",
                 "o_operator.add_operator(1.0, \"X 2 Y 0\")\n",
                 "o_operator.add_operator(0.5j, \"Y 1 Z 0\")\n",
                 "operator_json = o_operator.to_json()\n",
                 "print(\"original:\", o_operator)\n",
                 "\n",
                 "r_operator = quantum_operator.from_json(operator_json)\n",
-                "print(\"restored:\", r_operator)"
+                "print(\"restored:\", r_operator)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3724,15 +3730,15 @@
                 "(0.17434925+0j) [Z1 Z3] +\n",
                 "(-0.22279649999999998+0j) [Z2]\n",
                 "\"\"\"\n",
                 "\n",
                 "operator = create_quantum_operator_from_openfermion_text(open_fermion_text)\n",
                 "print(operator.get_term_count())\n",
                 "print(operator.get_qubit_count())\n",
-                "# In the case of create_quantum_operator_from_openfermion_file, specify the path of the file where the above is written in the argument."
+                "# In the case of create_quantum_operator_from_openfermion_file, specify the path of the file where the above is written in the argument.\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3761,15 +3767,15 @@
             "source": [
                 "from qulacs.observable import create_split_observable, create_observable_from_openfermion_file\n",
                 "\n",
                 "# H2.txt must be placed in openfermon format beforehand.\n",
                 "operator = create_observable_from_openfermion_file(\"./H2.txt\")\n",
                 "diag, nondiag = create_split_observable(\"./H2.txt\")\n",
                 "print(operator.get_term_count(), diag.get_term_count(), nondiag.get_term_count())\n",
-                "print(operator.get_qubit_count(), diag.get_qubit_count(), nondiag.get_qubit_count())"
+                "print(operator.get_qubit_count(), diag.get_qubit_count(), nondiag.get_qubit_count())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3789,15 +3795,15 @@
                 "from qulacs.observable import create_observable_from_openfermion_file\n",
                 "\n",
                 "n = 4\n",
                 "operator = create_observable_from_openfermion_file(\"./H2.txt\")\n",
                 "state = QuantumState(n)\n",
                 "state.set_Haar_random_state()\n",
                 "value = operator.solve_ground_state_eigenvalue_by_power_method(state, 50)\n",
-                "print(value)"
+                "print(value)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3814,15 +3820,15 @@
                 "from qulacs.observable import create_observable_from_openfermion_file\n",
                 "\n",
                 "n = 4\n",
                 "operator = create_observable_from_openfermion_file(\"./H2.txt\")\n",
                 "state = QuantumState(n)\n",
                 "state.set_Haar_random_state()\n",
                 "value = operator.solve_ground_state_eigenvalue_by_arnoldi_method(state, 50)\n",
-                "print(value)"
+                "print(value)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3839,15 +3845,15 @@
                 "from qulacs.observable import create_observable_from_openfermion_file\n",
                 "\n",
                 "n = 4\n",
                 "operator = create_observable_from_openfermion_file(\"./H2.txt\")\n",
                 "state = QuantumState(n)\n",
                 "state.set_Haar_random_state()\n",
                 "value = operator.solve_ground_state_eigenvalue_by_lanczos_method(state, 50)\n",
-                "print(value)"
+                "print(value)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3867,15 +3873,15 @@
                 "n = 4\n",
                 "operator = create_observable_from_openfermion_file(\"./H2.txt\")\n",
                 "state = QuantumState(n)\n",
                 "state.set_Haar_random_state()\n",
                 "result = QuantumState(n)\n",
                 "work_state = QuantumState(n)\n",
                 "operator.apply_to_state(work_state, state, result)\n",
-                "print(result)"
+                "print(result)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3915,15 +3921,15 @@
                 "# Create gate, which can also be added\n",
                 "for i in range(n):\n",
                 "    circuit.add_gate(Z(i))\n",
                 "\n",
                 "# Operate quantum circuit to state\n",
                 "circuit.update_quantum_state(state)\n",
                 "\n",
-                "print(state.get_vector())"
+                "print(state.get_vector())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -3972,15 +3978,15 @@
                 "copy_circuit = circuit.copy()\n",
                 "\n",
                 "# merge the gates of the provided quantum circuit as arguments\n",
                 "# modifying the merged side does not affect the side that has been merged\n",
                 "circuit.merge_circuit(copy_circuit)\n",
                 "\n",
                 "circuit.update_quantum_state(state)\n",
-                "print(state.get_vector())"
+                "print(state.get_vector())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -4020,15 +4026,15 @@
                 "# Optimization\n",
                 "opt = QuantumCircuitOptimizer()\n",
                 "# The maximum quantum gate size allowed to be created\n",
                 "max_block_size = 1\n",
                 "opt.optimize(circuit, max_block_size)\n",
                 "\n",
                 "# Calculate the depth (depth=1\u3078)\n",
-                "print(circuit.calculate_depth())"
+                "print(circuit.calculate_depth())\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -4063,15 +4069,15 @@
                 "n = 5\n",
                 "depth = 10\n",
                 "circuit = QuantumCircuit(n)\n",
                 "for d in range(depth):\n",
                 "    for i in range(n):\n",
                 "        circuit.add_H_gate(i)\n",
                 "\n",
-                "print(circuit)"
+                "print(circuit)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Store QuantumCircuit\n",
@@ -4119,15 +4125,15 @@
                 "o_circuit.add_H_gate(0)\n",
                 "o_circuit.add_CNOT_gate(0, 1)\n",
                 "o_circuit.add_RZ_gate(2, 0.7)\n",
                 "circuit_json = o_circuit.to_json()\n",
                 "print(o_circuit)\n",
                 "\n",
                 "r_circuit = circuit.from_json(circuit_json)\n",
-                "print(r_circuit)"
+                "print(r_circuit)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Quantum circuits can be stored to files in pickle format."
@@ -4149,15 +4155,15 @@
                 "\n",
                 "# store\n",
                 "with open('circuit.pickle', 'wb') as f:\n",
                 "    pickle.dump(circuit, f)\n",
                 "\n",
                 "# load\n",
                 "with open('circuit.pickle', 'rb') as f:\n",
-                "    circuit = pickle.load(f)"
+                "    circuit = pickle.load(f)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -4267,15 +4273,15 @@
                 "\n",
                 "# update quantum state\n",
                 "state = QuantumState(n)\n",
                 "circuit.update_quantum_state(state)\n",
                 "\n",
                 "# output state and circuit info\n",
                 "print(state)\n",
-                "print(circuit)"
+                "print(circuit)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -4316,15 +4322,15 @@
                 "\n",
                 "# GradCalculator\u306e\u5834\u5408\n",
                 "gcalc = GradCalculator()\n",
                 "print(gcalc.calculate_grad(circuit, observable))\n",
                 "# \u7b2c\u4e09\u5f15\u6570\u306b\u56de\u8ee2\u89d2\u3092\u6307\u5b9a\u3059\u308b\u3053\u3068\u3082\u53ef\u80fd\n",
                 "print(gcalc.calculate_grad(circuit, observable, theta))\n",
                 "# Backprop\u3092\u4f7f\u3063\u3066\u6c42\u3081\u305f\u5834\u5408\n",
-                "print(circuit.backprop(observable))"
+                "print(circuit.backprop(observable))\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Store parametric quantum circuits\n",
@@ -4379,15 +4385,15 @@
                 "o_circuit.add_H_gate(0)\n",
                 "o_circuit.add_parametric_RX_gate(1, 0.3)\n",
                 "o_circuit.add_multi_Pauli_rotation_gate([0, 1, 2], [1, 3, 2], 1.4)\n",
                 "circuit_json = o_circuit.to_json()\n",
                 "print(o_circuit)\n",
                 "\n",
                 "r_circuit = circuit.from_json(circuit_json)\n",
-                "print(r_circuit)"
+                "print(r_circuit)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Parametric quantum circuits can be converted to files in pickle format."
@@ -4409,15 +4415,15 @@
                 "\n",
                 "# store\n",
                 "with open('circuit.pickle', 'wb') as f:\n",
                 "    pickle.dump(circuit, f)\n",
                 "\n",
                 "# load\n",
                 "with open('circuit.pickle', 'rb') as f:\n",
-                "    circuit = pickle.load(f)"
+                "    circuit = pickle.load(f)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -4535,15 +4541,15 @@
                 "sim.copy_state_from_buffer()\n",
                 "sim.simulate()\n",
                 "print(state)\n",
                 "\n",
                 "# \u91cf\u5b50\u72b6\u614b\u3092\u30b3\u30d4\u30fc\uff08\u73fe\u72b6\u614b->\u30d0\u30c3\u30d5\u30a1\uff09\n",
                 "sim.copy_state_to_buffer()\n",
                 "sim.simulate()\n",
-                "print(state)"
+                "print(state)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -4607,15 +4613,15 @@
                 "            if i + 1 < n:\n",
                 "               circuit.add_noise_gate(CZ(i, i+1), \"Depolarizing\", 0.01)\n",
                 "\n",
                 "state = QuantumState(n)\n",
                 "state.set_Haar_random_state()\n",
                 "sim = NoiseSimulator(circuit, state)\n",
                 "sim.execute(100)\n",
-                "print(state)"
+                "print(state)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -4646,15 +4652,15 @@
                 "observable.add_operator(1.0, \"Z 0\")\n",
                 "circuit = ParametricQuantumCircuit(n)\n",
                 "for i in range(n):\n",
                 "   circuit.add_parametric_RX_gate(i, 1.0)\n",
                 "   circuit.add_parametric_RY_gate(i, 1.0)\n",
                 "\n",
                 "ccs = CausalConeSimulator(circuit, observable)\n",
-                "print(ccs.get_expectation_value())"
+                "print(ccs.get_expectation_value())\n"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.9.2 64-bit",
             "language": "python",
```

### Comparing `qulacs-0.6.2/doc/en/source/index.md` & `qulacs-0.6.3/doc/en/source/index.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/intro/0_about.md` & `qulacs-0.6.3/doc/en/source/intro/0_about.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/intro/1_install.md` & `qulacs-0.6.3/doc/ja/source/intro/1_install.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/intro/2_faq.md` & `qulacs-0.6.3/doc/en/source/intro/2_faq.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/intro/3_usage.md` & `qulacs-0.6.3/doc/en/source/intro/3_usage.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/intro/4.1_python_tutorial.ipynb` & `qulacs-0.6.3/doc/en/source/intro/4.1_python_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/intro/4.2_cpp_tutorial.md` & `qulacs-0.6.3/doc/en/source/intro/4.2_cpp_tutorial.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/en/source/write/0_readme.md` & `qulacs-0.6.3/doc/en/source/write/0_readme.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/Makefile` & `qulacs-0.6.3/doc/ja/Makefile`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/make.bat` & `qulacs-0.6.3/doc/ja/make.bat`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/source/_static/images/dojo.png` & `qulacs-0.6.3/doc/ja/source/_static/images/dojo.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/source/_static/images/github.png` & `qulacs-0.6.3/doc/ja/source/_static/images/github.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/source/_static/images/logo-c-h.png` & `qulacs-0.6.3/doc/ja/source/_static/images/logo-c-h.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/source/_static/images/slack.png` & `qulacs-0.6.3/doc/ja/source/_static/images/slack.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/source/_templates/autoapi/python/class.rst` & `qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/class.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/source/_templates/autoapi/python/data.rst` & `qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/data.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/source/_templates/autoapi/python/function.rst` & `qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/function.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/source/_templates/autoapi/python/method.rst` & `qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/method.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/source/_templates/autoapi/python/module.rst` & `qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/module.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/source/conf.py` & `qulacs-0.6.3/doc/ja/source/conf.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/source/guide/2.0_python_advanced.md` & `qulacs-0.6.3/doc/ja/source/guide/2.0_python_advanced.md`

 * *Files 1% similar despite different names*

```diff
@@ -1821,17 +1821,23 @@
 `PauliOperator` クラスはその中のそれぞれの項を表す、$n$-qubitパウリ演算子の元に係数を付与したものを表現するクラスです。
 ゲートと異なり、量子状態の更新はできません。
 
 #### パウリ演算子の生成と状態の取得
 
 ```python
 from qulacs import PauliOperator
+# pauli_stringからパウリ演算子を生成
 coef = 0.1
 s = "X 0 Y 1 Z 3"
 pauli = PauliOperator(s, coef)
+# index_listとtype_listからも生成可能
+coef =  0.1
+index_list = [0, 1, 3]
+type_list = "XYZ"
+pauli = PauliOperator(index_list, type_list, coef)
 
 # pauliの記号を後から追加
 pauli.add_single_Pauli(3, 2)
 
 # pauliの各記号の添え字を取得
 index_list = pauli.get_index_list()
```

### Comparing `qulacs-0.6.2/doc/ja/source/index.md` & `qulacs-0.6.3/doc/ja/source/index.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/source/intro/0_about.md` & `qulacs-0.6.3/doc/ja/source/intro/0_about.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/source/intro/1_install.md` & `qulacs-0.6.3/doc/en/source/intro/1_install.md`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,17 @@
 
 Install with default options (Multi-thread without GPU):
 
 ```
 pip install .
 ```
 
+Your build may fail with python's `cmake` package installed. Adding `--no-build-isolation` option will help.
+
+
 If AVX2 instructions are not supported, SIMD optimization is automatically disabled.
 
 
 Install with GPU support (CUDA is required):
 
 ```
 USE_GPU=Yes pip install .
```

### Comparing `qulacs-0.6.2/doc/ja/source/intro/2_faq.md` & `qulacs-0.6.3/doc/ja/source/intro/2_faq.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/source/intro/3_usage.md` & `qulacs-0.6.3/doc/ja/source/intro/3_usage.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/source/intro/4.1_python_tutorial.md` & `qulacs-0.6.3/doc/ja/source/intro/4.1_python_tutorial.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/ja/source/intro/4.2_cpp_tutorial.md` & `qulacs-0.6.3/doc/ja/source/intro/4.2_cpp_tutorial.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/scripts/customdoxygen.css` & `qulacs-0.6.3/doc/scripts/customdoxygen.css`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/scripts/doxy-boot.js` & `qulacs-0.6.3/doc/scripts/doxy-boot.js`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/scripts/footer.html` & `qulacs-0.6.3/doc/scripts/footer.html`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/scripts/header.html` & `qulacs-0.6.3/doc/scripts/header.html`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/doc/scripts/index.html` & `qulacs-0.6.3/doc/scripts/index.html`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/pyproject.toml` & `qulacs-0.6.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -58,23 +58,24 @@
     "mypy",
     "pybind11-stubgen",
     "openfermion",
     "pytest"
 ]
 
 doc = [
-    "sphinx == 4.5.0",
-    "sphinx-rtd-theme == 1.0.*",
-    "breathe == 4.33.*",
-    "exhale == 0.3.*",
-    "nbsphinx == 0.8.*",
-    "myst-parser == 0.18.*",
-    "sphinx-copybutton == 0.5.*",
-    "ipykernel == 6.17.*",
-    "sphinx-autoapi == 2.0.*"
+    "sphinx==7.*",
+    "sphinx-rtd-theme",
+    "breathe",
+    #"exhale@git+https://github.com/svenevs/exhale.git@fix/packaging-requirements", # workaround until https://github.com/svenevs/exhale/pull/205 is merged
+    "exhale",
+    "nbsphinx",
+    "myst-parser",
+    "sphinx-copybutton",
+    "ipykernel",
+    "sphinx-autoapi==3.*"
 ]
 
 [tool.setuptools]
 include-package-data = true
 zip-safe = false
 
 [tool.cibuildwheel]
```

### Comparing `qulacs-0.6.2/pysrc/qulacs/__init__.pyi` & `qulacs-0.6.3/pysrc/qulacs/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -307,15 +307,15 @@
         """
         Get expectation value
         """
     def get_expectation_value_single_thread(self, state: QuantumStateBase) -> complex:
         """
         Get expectation value
         """
-    def get_matrix(self) -> scipy.sparse.csr_matrix[numpy.complex128]:
+    def get_matrix(self) -> scipy.sparse.csr_matrix:
         """
         Get the Hermitian matrix representation of the observable
         """
     def get_qubit_count(self) -> int:
         """
         Get qubit count
         """
@@ -453,27 +453,27 @@
     def get_transition_amplitude(
         self, state_bra: QuantumStateBase, state_ket: QuantumStateBase
     ) -> complex:
         """
         Get transition amplitude
         """
     def solve_ground_state_eigenvalue_by_arnoldi_method(
-        self, state: QuantumStateBase, iter_count: int, mu: complex = ...
+        self, state: QuantumStateBase, iter_count: int, mu: complex = 0.0
     ) -> complex:
         """
         Compute ground state eigenvalue by arnoldi method
         """
     def solve_ground_state_eigenvalue_by_lanczos_method(
-        self, state: QuantumStateBase, iter_count: int, mu: complex = ...
+        self, state: QuantumStateBase, iter_count: int, mu: complex = 0.0
     ) -> complex:
         """
         Compute ground state eigenvalue by lanczos method
         """
     def solve_ground_state_eigenvalue_by_power_method(
-        self, state: QuantumStateBase, iter_count: int, mu: complex = ...
+        self, state: QuantumStateBase, iter_count: int, mu: complex = 0.0
     ) -> complex:
         """
         Compute ground state eigenvalue by power method
         """
 
 class ParametricQuantumCircuit(QuantumCircuit):
     def __getstate__(self) -> str: ...
@@ -563,20 +563,30 @@
         Set parameter
         """
 
 class PauliOperator:
     def __IMUL__(self, arg0: complex) -> PauliOperator: ...
     def __imul__(self, arg0: PauliOperator) -> PauliOperator: ...
     @typing.overload
-    def __init__(self, coef: complex) -> None:
+    def __init__(self, coef: complex = (1 + 0j)) -> None:
         """
         Constructor
         """
     @typing.overload
-    def __init__(self, pauli_string: str, coef: complex) -> None:
+    def __init__(self, pauli_string: str, coef: complex = (1 + 0j)) -> None:
+        """
+        Constructor
+        """
+    @typing.overload
+    def __init__(
+        self,
+        target_qubit_index_list: list[int],
+        pauli_operator_type_list: str,
+        coef: complex = (1 + 0j),
+    ) -> None:
         """
         Constructor
         """
     @typing.overload
     def __mul__(self, arg0: PauliOperator) -> PauliOperator: ...
     @typing.overload
     def __mul__(self, arg0: complex) -> PauliOperator: ...
```

### Comparing `qulacs-0.6.2/pysrc/qulacs/circuit/__init__.pyi` & `qulacs-0.6.3/pysrc/qulacs/circuit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/pysrc/qulacs/circuit.pyi` & `qulacs-0.6.3/pysrc/qulacs/circuit.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from __future__ import annotations
 
 import qulacs_core
 
 __all__ = ["QuantumCircuitOptimizer", "from_json"]
 
 class QuantumCircuitOptimizer:
-    def __init__(self) -> None:
+    def __init__(self, mpi_size: int = 0) -> None:
         """
         Constructor
         """
     def merge_all(
         self, circuit: qulacs_core.QuantumCircuit
     ) -> qulacs_core.QuantumGateMatrix: ...
-    def optimize(self, circuit: qulacs_core.QuantumCircuit, block_size: int) -> None:
+    def optimize(
+        self, circuit: qulacs_core.QuantumCircuit, block_size: int, swap_level: int = 0
+    ) -> None:
         """
         Optimize quantum circuit
         """
-    def optimize_light(self, circuit: qulacs_core.QuantumCircuit) -> None:
+    def optimize_light(
+        self, circuit: qulacs_core.QuantumCircuit, swap_level: int = 0
+    ) -> None:
         """
         Optimize quantum circuit with light method
         """
 
 def from_json(arg0: str) -> qulacs_core.QuantumCircuit:
     """
     from json string
```

### Comparing `qulacs-0.6.2/pysrc/qulacs/converter/qasm_converter.py` & `qulacs-0.6.3/pysrc/qulacs/converter/qasm_converter.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/pysrc/qulacs/gate/__init__.pyi` & `qulacs-0.6.3/pysrc/qulacs/gate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/pysrc/qulacs/gate.pyi` & `qulacs-0.6.3/pysrc/qulacs/gate.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -71,24 +71,24 @@
     "sqrtY",
     "sqrtYdag",
     "to_matrix_gate",
 ]
 
 @typing.overload
 def Adaptive(
-    gate: qulacs_core.QuantumGateBase, condition: typing.Callable[[List[int]], bool]
+    gate: qulacs_core.QuantumGateBase, condition: typing.Callable[[list[int]], bool]
 ) -> qulacs_core.QuantumGateBase:
     """
     Create adaptive gate
     """
 
 @typing.overload
 def Adaptive(
     gate: qulacs_core.QuantumGateBase,
-    condition: typing.Callable[[List[int], int], bool],
+    condition: typing.Callable[[list[int], int], bool],
     id: int,
 ) -> qulacs_core.QuantumGateBase:
     """
     Create adaptive gate
     """
 
 def AmplitudeDampingNoise(index: int, prob: float) -> qulacs_core.QuantumGate_CPTP:
@@ -351,15 +351,15 @@
 
 def Sdag(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create adjoint of pi/4-phase gate
     """
 
 def SparseMatrix(
-    index_list: list[int], matrix: scipy.sparse.csc_matrix[numpy.complex128]
+    index_list: list[int], matrix: scipy.sparse.csc_matrix
 ) -> qulacs_core.QuantumGateSparseMatrix:
     """
     Create sparse matrix gate
     """
 
 def StateReflection(
     state: qulacs_core.QuantumState,
```

### Comparing `qulacs-0.6.2/pysrc/qulacs/observable/__init__.pyi` & `qulacs-0.6.3/pysrc/qulacs/observable/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/pysrc/qulacs/observable.pyi` & `qulacs-0.6.3/pysrc/qulacs/observable.pyi`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/pysrc/qulacs/quantum_operator/__init__.pyi` & `qulacs-0.6.3/pysrc/qulacs/quantum_operator/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/pysrc/qulacs/quantum_operator.pyi` & `qulacs-0.6.3/pysrc/qulacs/quantum_operator.pyi`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/pysrc/qulacs/state/__init__.pyi` & `qulacs-0.6.3/pysrc/qulacs/state/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/pysrc/qulacs/state.pyi` & `qulacs-0.6.3/pysrc/qulacs/state.pyi`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/pysrc/qulacs/utils/conversions_openfermion.py` & `qulacs-0.6.3/pysrc/qulacs/utils/conversions_openfermion.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/pysrc/qulacs/vistest/test_vis.py` & `qulacs-0.6.3/pysrc/qulacs/vistest/test_vis.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/pysrc/qulacs/visualizer/visualizer.py` & `qulacs-0.6.3/pysrc/qulacs/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/pysrc/qulacs.egg-info/PKG-INFO` & `qulacs-0.6.3/pysrc/qulacs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qulacs
-Version: 0.6.2
+Version: 0.6.3
 Summary: Quantum circuit simulator for research
 Author-email: QunaSys <qulacs@qunasys.com>
 License: MIT License
         
         Copyright (c) 2018 Qulacs Authors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,23 +54,23 @@
 Requires-Dist: flake8; extra == "ci"
 Requires-Dist: isort; extra == "ci"
 Requires-Dist: mypy; extra == "ci"
 Requires-Dist: pybind11-stubgen; extra == "ci"
 Requires-Dist: openfermion; extra == "ci"
 Requires-Dist: pytest; extra == "ci"
 Provides-Extra: doc
-Requires-Dist: sphinx==4.5.0; extra == "doc"
-Requires-Dist: sphinx-rtd-theme==1.0.*; extra == "doc"
-Requires-Dist: breathe==4.33.*; extra == "doc"
-Requires-Dist: exhale==0.3.*; extra == "doc"
-Requires-Dist: nbsphinx==0.8.*; extra == "doc"
-Requires-Dist: myst-parser==0.18.*; extra == "doc"
-Requires-Dist: sphinx-copybutton==0.5.*; extra == "doc"
-Requires-Dist: ipykernel==6.17.*; extra == "doc"
-Requires-Dist: sphinx-autoapi==2.0.*; extra == "doc"
+Requires-Dist: sphinx==7.*; extra == "doc"
+Requires-Dist: sphinx-rtd-theme; extra == "doc"
+Requires-Dist: breathe; extra == "doc"
+Requires-Dist: exhale; extra == "doc"
+Requires-Dist: nbsphinx; extra == "doc"
+Requires-Dist: myst-parser; extra == "doc"
+Requires-Dist: sphinx-copybutton; extra == "doc"
+Requires-Dist: ipykernel; extra == "doc"
+Requires-Dist: sphinx-autoapi==3.*; extra == "doc"
 
 # Qulacs
 
 [![Ubuntu CI](https://github.com/qulacs/qulacs/actions/workflows/ci_ubuntu.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/ci_ubuntu.yml)
 [![macOS CI](https://github.com/qulacs/qulacs/actions/workflows/ci_macos.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/ci_macos.yml)
 [![Windows CI](https://github.com/qulacs/qulacs/actions/workflows/ci_windows.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/ci_windows.yml)
 [![Wheel build](https://github.com/qulacs/qulacs/actions/workflows/wheel.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/wheel.yml)
```

### Comparing `qulacs-0.6.2/pysrc/qulacs.egg-info/SOURCES.txt` & `qulacs-0.6.3/pysrc/qulacs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,15 @@
 pysrc/qulacs/visualizer/__init__.py
 pysrc/qulacs/visualizer/visualizer.py
 python/CMakeLists.txt
 python/cppsim_wrapper.cpp
 python/stub-test/generate_mypy_tester.py
 python/tests/__init__.py
 python/tests/multi_cpu/conftest.py
+python/tests/multi_cpu/test_circuit_optimizer.py
 python/tests/multi_cpu/test_state_multi_cpu.py
 python/tests/single_cpu/conftest.py
 python/tests/single_cpu/test_circuit.py
 python/tests/single_cpu/test_density_matrix_handling.py
 python/tests/single_cpu/test_json.py
 python/tests/single_cpu/test_noise_simulator.py
 python/tests/single_cpu/test_observable.py
@@ -219,14 +220,16 @@
 src/cppsim/noisesimulator.hpp
 src/cppsim/observable.cpp
 src/cppsim/observable.hpp
 src/cppsim/pauli_operator.cpp
 src/cppsim/pauli_operator.hpp
 src/cppsim/qubit_info.cpp
 src/cppsim/qubit_info.hpp
+src/cppsim/qubit_table.cpp
+src/cppsim/qubit_table.hpp
 src/cppsim/simulator.cpp
 src/cppsim/simulator.hpp
 src/cppsim/state.cpp
 src/cppsim/state.hpp
 src/cppsim/state_dm.cpp
 src/cppsim/state_dm.hpp
 src/cppsim/state_gpu.cpp
```

### Comparing `qulacs-0.6.2/python/CMakeLists.txt` & `qulacs-0.6.3/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/python/cppsim_wrapper.cpp` & `qulacs-0.6.3/python/cppsim_wrapper.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#define PYBIND11_DETAILED_ERROR_MESSAGES
 #include <pybind11/complex.h>
 #include <pybind11/eigen.h>
 #include <pybind11/functional.h>
 #include <pybind11/operators.h>
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 
@@ -36,17 +37,22 @@
 #include <vqcsim/parametric_gate_factory.hpp>
 
 namespace py = pybind11;
 PYBIND11_MODULE(qulacs_core, m) {
     m.doc() = "cppsim python interface";
 
     py::class_<PauliOperator>(m, "PauliOperator")
-        .def(py::init<std::complex<double>>(), "Constructor", py::arg("coef"))
+        .def(py::init<std::complex<double>>(), "Constructor",
+            py::arg("coef") = 1. + 0.i)
         .def(py::init<std::string, std::complex<double>>(), "Constructor",
-            py::arg("pauli_string"), py::arg("coef"))
+            py::arg("pauli_string"),
+            py::arg("coef") = std::complex<double>(1., 0.))
+        .def(py::init<std::vector<UINT>, std::string, std::complex<double>>(),
+            "Constructor", py::arg("target_qubit_index_list"),
+            py::arg("pauli_operator_type_list"), py::arg("coef") = 1. + 0.i)
         .def("get_index_list", &PauliOperator::get_index_list,
             "Get list of target qubit indices")
         .def("get_pauli_id_list", &PauliOperator::get_pauli_id_list,
             "Get list of Pauli IDs (I,X,Y,Z) = (0,1,2,3)")
         .def("get_coef", &PauliOperator::get_coef,
             "Get coefficient of Pauli term")
         .def("add_single_Pauli", &PauliOperator::add_single_Pauli,
@@ -1521,20 +1527,21 @@
             } else {
                 return circuit::from_ptree(pt);
             }
         },
         "from json string", py::return_value_policy::take_ownership);
 
     py::class_<QuantumCircuitOptimizer>(mcircuit, "QuantumCircuitOptimizer")
-        .def(py::init<>(), "Constructor")
+        .def(py::init<UINT>(), "Constructor", py::arg("mpi_size") = 0)
         .def("optimize", &QuantumCircuitOptimizer::optimize,
             "Optimize quantum circuit", py::arg("circuit"),
-            py::arg("block_size"))
+            py::arg("block_size"), py::arg("swap_level") = 0)
         .def("optimize_light", &QuantumCircuitOptimizer::optimize_light,
-            "Optimize quantum circuit with light method", py::arg("circuit"))
+            "Optimize quantum circuit with light method", py::arg("circuit"),
+            py::arg("swap_level") = 0)
         .def("merge_all", &QuantumCircuitOptimizer::merge_all,
             py::return_value_policy::take_ownership, py::arg("circuit"));
 
     py::class_<QuantumCircuitSimulator>(m, "QuantumCircuitSimulator")
         .def(py::init<QuantumCircuit*, QuantumStateBase*>(), "Constructor",
             py::arg("circuit"), py::arg("state"))
         .def("initialize_state", &QuantumCircuitSimulator::initialize_state,
```

### Comparing `qulacs-0.6.2/python/stub-test/generate_mypy_tester.py` & `qulacs-0.6.3/python/stub-test/generate_mypy_tester.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/python/tests/multi_cpu/conftest.py` & `qulacs-0.6.3/python/tests/multi_cpu/conftest.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/python/tests/multi_cpu/test_state_multi_cpu.py` & `qulacs-0.6.3/python/tests/multi_cpu/test_state_multi_cpu.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/python/tests/single_cpu/test_circuit.py` & `qulacs-0.6.3/python/tests/single_cpu/test_circuit.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/python/tests/single_cpu/test_density_matrix_handling.py` & `qulacs-0.6.3/python/tests/single_cpu/test_density_matrix_handling.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/python/tests/single_cpu/test_json.py` & `qulacs-0.6.3/python/tests/single_cpu/test_json.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/python/tests/single_cpu/test_noise_simulator.py` & `qulacs-0.6.3/python/tests/single_cpu/test_noise_simulator.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/python/tests/single_cpu/test_observable.py` & `qulacs-0.6.3/python/tests/single_cpu/test_observable.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/python/tests/single_cpu/test_pickle.py` & `qulacs-0.6.3/python/tests/single_cpu/test_pickle.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/python/tests/single_cpu/test_pointer_handling.py` & `qulacs-0.6.3/python/tests/single_cpu/test_pointer_handling.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/python/tests/single_cpu/test_qasm.py` & `qulacs-0.6.3/python/tests/single_cpu/test_qasm.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/python/tests/single_cpu/test_state.py` & `qulacs-0.6.3/python/tests/single_cpu/test_state.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/python/tests/single_cpu/test_utils.py` & `qulacs-0.6.3/python/tests/single_cpu/test_utils.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/script/build_gcc.sh` & `qulacs-0.6.3/script/build_gcc.sh`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/script/download_wheel.sh` & `qulacs-0.6.3/script/download_wheel.sh`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/setup.py` & `qulacs-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/CMakeLists.txt` & `qulacs-0.6.3/src/cppsim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/circuit.cpp` & `qulacs-0.6.3/src/cppsim/circuit.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,33 @@
             "Error: QuantumCircuit::remove_gate(UINT) : index must be "
             "smaller than gate_count");
     }
     delete this->_gate_list[index];
     this->_gate_list.erase(this->_gate_list.begin() + index);
 }
 
+void QuantumCircuit::move_gate(UINT from_index, UINT to_index) {
+    if (from_index >= this->_gate_list.size() ||
+        to_index >= this->_gate_list.size()) {
+        throw GateIndexOutOfRangeException(
+            "Error: QuantumCircuit::move_gate(UINT, UINT) : "
+            "index must be smaller than gate_count");
+    }
+    if (from_index < to_index) {
+        std::rotate(this->_gate_list.begin() + from_index,
+            this->_gate_list.begin() + from_index + 1,
+            this->_gate_list.begin() + to_index + 1);
+    } else {
+        std::rotate(this->_gate_list.rbegin() +
+                        (this->_gate_list.size() - from_index - 1),
+            this->_gate_list.rbegin() + (this->_gate_list.size() - from_index),
+            this->_gate_list.rbegin() + (this->_gate_list.size() - to_index));
+    }
+}
+
 QuantumCircuit::~QuantumCircuit() {
     for (auto& gate : this->_gate_list) {
         delete gate;
     }
 }
 
 bool QuantumCircuit::is_Clifford() const {
```

### Comparing `qulacs-0.6.2/src/cppsim/circuit.hpp` & `qulacs-0.6.3/src/cppsim/circuit.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,23 @@
      * \~japanese-en 量子回路からゲートを削除する。
      *
      * 削除した量子ゲートは解放される。
      * @param[in] index 削除するゲートの位置
      */
     virtual void remove_gate(UINT index);
     /**
+     * \~japanese-en 量子回路内のゲートを移動する。
+     *
+     * 回路内の量子ゲートを移動する。
+     * from_indexとto_indexの間のゲートはfrom_indexの方向にシフトする。
+     * @param[in] from_index 移動元のゲートの位置
+     * @param[in] to_index 移動先のゲートの位置
+     */
+    virtual void move_gate(UINT from_index, UINT to_index);
+    /**
      *  \~japanese-en 量子回路をマージする。
      *
      * 引数で与えた量子回路のゲートを後ろに追加していく。
      * マージされた側の量子回路に変更を加えてもマージした側の量子回路には変更は加わらないことに注意する。
      * circuit1.add_circuit(circuit2)
      * circuit2.add_gate(gate) # これをしても、circuit1にgateは追加されない
      *
```

### Comparing `qulacs-0.6.2/src/cppsim/circuit_optimizer.hpp` & `qulacs-0.6.3/src/cppsim/simulator.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,100 @@
 
 #pragma once
 
-#include "type.hpp"
+#include <cstdlib>
 
-class QuantumCircuit;
-class QuantumGateBase;
-class QuantumGateMatrix;
+#include "circuit.hpp"
+#include "type.hpp"
+class QuantumStateBase;
+class HermitianQuantumOperator;
+using Observable = HermitianQuantumOperator;
 
 /**
- * \~japanese-en 量子回路の圧縮を行うクラス
- *
- * 量子回路の圧縮を行う。
- * 与えらえた量子回路を適切なサイズまで圧縮したり、まとめたゲートに変換するなどの処理を行う。
+ * \~japanese-en 量子回路をシミュレートするためのクラス
  */
-class DllExport QuantumCircuitOptimizer {
+class DllExport QuantumCircuitSimulator {
 private:
-    QuantumCircuit* circuit;
-    UINT get_rightmost_commute_index(UINT gate_index);
-    UINT get_leftmost_commute_index(UINT gate_index);
-    UINT get_merged_gate_size(UINT gate_index1, UINT gate_index2);
-    bool is_neighboring(UINT gate_index1, UINT gate_index2);
+    QuantumCircuit* _circuit;
+    QuantumStateBase* _state;
+    QuantumStateBase* _buffer;
+    bool _own_state = false;
 
 public:
     /**
      * \~japanese-en コンストラクタ
+     *
+     * @param circuit シミュレートする量子回路
+     * @param initial_state
+     * 初期量子状態。デフォルト値はNULLで、NULLの場合は0状態に初期化される。
      */
-    QuantumCircuitOptimizer(){};
+    explicit QuantumCircuitSimulator(
+        QuantumCircuit* circuit, QuantumStateBase* initial_state = NULL);
 
     /**
      * \~japanese-en デストラクタ
      */
-    virtual ~QuantumCircuitOptimizer(){};
+    ~QuantumCircuitSimulator();
 
     /**
-     * \~japanese-en 与えられた量子回路のゲートを指定されたブロックまで纏める。
+     * \~japanese-en 量子状態を計算基底に初期化する
      *
-     * 与えられた量子回路において、若い添え字から任意の二つのゲートを選び、二つが他のゲートに影響を与えず合成可能なら合成を行う。
-     * これを合成可能なペアがなくなるまで繰り返す。
-     * 二つのゲートが合成可能であるとは、二つのゲートそれぞれについて隣接するゲートとの交換を繰り返し、二つのゲートが隣接した位置まで移動できることを指す。
+     * @param computationl_basis 初期化する計算基底を二進数にした値
+     */
+    void initialize_state(ITYPE computationl_basis = 0);
+    /**
+     * \~japanese-en ランダムな量子状態に初期化する。
+     * @param seed 乱数のシード値
+     */
+    void initialize_random_state();
+    void initialize_random_state(UINT seed);
+
+    /**
+     * \~japanese-en 量子回路全体シミュレートする。
+     */
+    void simulate();
+
+    /**
+     * \~japanese-en
+     * 量子回路を<code>start</code>から<code>end</code>までの区間シミュレートする
      *
-     * @param[in] circuit 量子回路のインスタンス
-     * @param[in] max_block_size 合成後に許されるブロックの最大サイズ
+     * @param start シミュレートを開始する添え字
+     * @param end シミュレートを終了する添え字
      */
-    void optimize(QuantumCircuit* circuit, UINT max_block_size = 2);
+    void simulate_range(UINT start, UINT end);
 
     /**
-     * \~japanese-en 与えられた量子回路のゲートを指定されたブロックまで纏める。
+     * \~japanese-en
+     * 現在の量子状態の受け取ったオブザーバブルの期待値を計算する。
      *
-     * 与えられた量子回路において、若い添え字から任意の二つのゲートを選び、二つが他のゲートに影響を与えず合成可能なら合成を行う。
-     * これを合成可能なペアがなくなるまで繰り返す。
-     * 二つのゲートが合成可能であるとは、二つのゲートそれぞれについて隣接するゲートとの交換を繰り返し、二つのゲートが隣接した位置まで移動できることを指す。
+     * @param observable オブザーバブル
+     * @return 期待値
+     */
+    CPPCTYPE get_expectation_value(const Observable* observable);
+
+    /**
+     * \~japanese-en 量子回路中のゲートの数を取得する
      *
-     * @param[in] circuit 量子回路のインスタンス
+     * @return ゲートの数
+     */
+    UINT get_gate_count();
+
+    /**
+     * \~japanese-en 量子状態をバッファへコピーする
+     */
+    void copy_state_to_buffer();
+    /**
+     * \~japanese-en バッファの量子状態を現在の量子状態へコピーする
+     */
+    void copy_state_from_buffer();
+    /**
+     * \~japanese-en 現在の量子状態をバッファと交換する
      */
-    void optimize_light(QuantumCircuit* circuit);
+    void swap_state_and_buffer();
 
     /**
-     * \~japanese-en 量子回路を纏めて一つの巨大な量子ゲートにする
+     * \~japanese-en 現在の量子状態のポインタを取得する
      *
-     * @param[in] circuit 量子回路のインスタンス
-     * @return 変換された量子ゲート
+     * @return 量子状態のポインタ
      */
-    QuantumGateMatrix* merge_all(const QuantumCircuit* circuit);
+    const QuantumStateBase* get_state_ptr() const { return _state; }
 };
```

### Comparing `qulacs-0.6.2/src/cppsim/exception.hpp` & `qulacs-0.6.3/src/cppsim/exception.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate.cpp` & `qulacs-0.6.3/src/cppsim/gate.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate.hpp` & `qulacs-0.6.3/src/cppsim/gate.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_factory.cpp` & `qulacs-0.6.3/src/cppsim/gate_factory.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_factory.hpp` & `qulacs-0.6.3/src/cppsim/gate_factory.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_general.hpp` & `qulacs-0.6.3/src/cppsim/gate_general.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_matrix.cpp` & `qulacs-0.6.3/src/cppsim/gate_matrix.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_matrix.hpp` & `qulacs-0.6.3/src/cppsim/gate_matrix.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_matrix_diagonal.cpp` & `qulacs-0.6.3/src/cppsim/gate_matrix_diagonal.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_matrix_diagonal.hpp` & `qulacs-0.6.3/src/cppsim/gate_matrix_diagonal.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_matrix_sparse.cpp` & `qulacs-0.6.3/src/cppsim/gate_matrix_sparse.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_matrix_sparse.hpp` & `qulacs-0.6.3/src/cppsim/gate_matrix_sparse.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_merge.cpp` & `qulacs-0.6.3/src/cppsim/gate_merge.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_merge.hpp` & `qulacs-0.6.3/src/cppsim/gate_merge.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_named_npair.hpp` & `qulacs-0.6.3/src/cppsim/gate_named_npair.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_named_one.cpp` & `qulacs-0.6.3/src/cppsim/gate_named_one.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_named_one.hpp` & `qulacs-0.6.3/src/cppsim/gate_named_one.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_named_pauli.hpp` & `qulacs-0.6.3/src/cppsim/gate_named_pauli.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_named_two.hpp` & `qulacs-0.6.3/src/cppsim/gate_named_two.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_noisy_evolution.cpp` & `qulacs-0.6.3/src/cppsim/gate_noisy_evolution.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -416,19 +416,19 @@
         "unexpectedly come to end of _find_collapse function.");
 }
 
 void ClsNoisyEvolution_fast::_evolve_one_step(
     QuantumStateBase* state, double t_step) {
     // 対角化したものを持っておき、　ここではそれを使う
     eigenMatrixRevGate->update_quantum_state(state);
-    UINT dim = eigenvalue_mto.size();
+    ITYPE dim = eigenvalue_mto.size();
 
     ComplexVector eigenvalues(dim);
 
-    for (UINT i = 0; i < dim; i++) {
+    for (ITYPE i = 0; i < dim; i++) {
         eigenvalues[i] = std::exp(eigenvalue_mto[i] * t_step);
     }
     // eigenvalues[i] を掛ける必要がある
     QuantumGateBase* eigenValueGate =
         gate::DiagonalMatrix(this->get_target_index_list(), eigenvalues);
 
     eigenValueGate->update_quantum_state(state);
```

### Comparing `qulacs-0.6.2/src/cppsim/gate_noisy_evolution.hpp` & `qulacs-0.6.3/src/cppsim/gate_noisy_evolution.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_reflect.hpp` & `qulacs-0.6.3/src/cppsim/gate_reflect.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_reversible.hpp` & `qulacs-0.6.3/src/cppsim/gate_reversible.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/gate_to_gqo.hpp` & `qulacs-0.6.3/src/cppsim/gate_to_gqo.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/general_quantum_operator.cpp` & `qulacs-0.6.3/src/cppsim/general_quantum_operator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/general_quantum_operator.hpp` & `qulacs-0.6.3/src/cppsim/general_quantum_operator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/matrix_decomposition.hpp` & `qulacs-0.6.3/src/cppsim/matrix_decomposition.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/noisesimulator.cpp` & `qulacs-0.6.3/src/cppsim/noisesimulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/noisesimulator.hpp` & `qulacs-0.6.3/src/cppsim/noisesimulator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/observable.cpp` & `qulacs-0.6.3/src/cppsim/observable.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/observable.hpp` & `qulacs-0.6.3/src/cppsim/observable.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/pauli_operator.cpp` & `qulacs-0.6.3/src/cppsim/pauli_operator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/pauli_operator.hpp` & `qulacs-0.6.3/src/cppsim/pauli_operator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/qubit_info.cpp` & `qulacs-0.6.3/src/cppsim/qubit_info.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/qubit_info.hpp` & `qulacs-0.6.3/src/cppsim/qubit_info.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/simulator.cpp` & `qulacs-0.6.3/src/cppsim/simulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/state.cpp` & `qulacs-0.6.3/src/cppsim/state.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/state.hpp` & `qulacs-0.6.3/src/cppsim/state.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -362,15 +362,15 @@
      *
      * @return 生成した文字列
      */
     virtual std::string to_string() const {
         std::stringstream os;
         ComplexVector eigen_state(this->dim);
         auto data = this->data_cpp();
-        for (UINT i = 0; i < this->dim; ++i) eigen_state[i] = data[i];
+        for (ITYPE i = 0; i < this->dim; ++i) eigen_state[i] = data[i];
 
         os << " *** Quantum State ***" << std::endl;
         UINT myrank = 0;
 #ifdef _USE_MPI
         if (this->outer_qc > 0) {
             MPIutil& mpiutil = MPIutil::get_inst();
             myrank = mpiutil.get_rank();
@@ -907,20 +907,20 @@
         }
 #endif
         std::vector<double> stacked_prob;
         std::vector<ITYPE> result;
         double sum = 0.;
         auto ptr = this->data_cpp();
         stacked_prob.push_back(0.);
-        for (UINT i = 0; i < this->dim; ++i) {
+        for (ITYPE i = 0; i < this->dim; ++i) {
             sum += norm(ptr[i]);
             stacked_prob.push_back(sum);
         }
 
-        for (UINT count = 0; count < sampling_count; ++count) {
+        for (ITYPE count = 0; count < sampling_count; ++count) {
             double r = random.uniform();
             auto ite =
                 std::lower_bound(stacked_prob.begin(), stacked_prob.end(), r);
             auto index = std::distance(stacked_prob.begin(), ite) - 1;
             result.push_back(index);
         }
         return result;
@@ -940,15 +940,15 @@
             double sum = 0.;
             auto ptr = this->data_cpp();
             // resize
             stacked_prob.resize(this->dim + 1);
             result.resize(sampling_count);
 
             stacked_prob[0] = 0.;
-            for (UINT i = 0; i < this->dim; ++i) {
+            for (ITYPE i = 0; i < this->dim; ++i) {
                 sum += norm(ptr[i]);
                 stacked_prob[i + 1] = sum;
             }
 
             double* sumrank_prob;
             sumrank_prob = new double[mpisize];
```

### Comparing `qulacs-0.6.2/src/cppsim/state_dm.cpp` & `qulacs-0.6.3/src/cppsim/state_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/state_dm.hpp` & `qulacs-0.6.3/src/cppsim/state_dm.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/state_gpu.cpp` & `qulacs-0.6.3/src/cppsim/state_gpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/state_gpu.hpp` & `qulacs-0.6.3/src/cppsim/state_gpu.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/type.hpp` & `qulacs-0.6.3/src/cppsim/type.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/utility.cpp` & `qulacs-0.6.3/src/cppsim/utility.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/cppsim/utility.hpp` & `qulacs-0.6.3/src/cppsim/utility.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/CMakeLists.txt` & `qulacs-0.6.3/src/csim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/MPIutil.cpp` & `qulacs-0.6.3/src/csim/MPIutil.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/MPIutil.hpp` & `qulacs-0.6.3/src/csim/MPIutil.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/constant.cpp` & `qulacs-0.6.3/src/csim/constant.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/constant.hpp` & `qulacs-0.6.3/src/csim/constant.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/init_ops.hpp` & `qulacs-0.6.3/src/csim/init_ops.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/init_ops_fill.cpp` & `qulacs-0.6.3/src/csim/init_ops_fill.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/init_ops_random.cpp` & `qulacs-0.6.3/src/csim/init_ops_random.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/memory_ops.cpp` & `qulacs-0.6.3/src/csim/memory_ops.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/memory_ops_dm.cpp` & `qulacs-0.6.3/src/csim/memory_ops_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/memory_ops_dm.hpp` & `qulacs-0.6.3/src/csim/memory_ops_dm.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/stat_ops.cpp` & `qulacs-0.6.3/src/csim/stat_ops.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/stat_ops.hpp` & `qulacs-0.6.3/src/csim/stat_ops.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/stat_ops_dm.cpp` & `qulacs-0.6.3/src/csim/stat_ops_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/stat_ops_dm.hpp` & `qulacs-0.6.3/src/csim/stat_ops_dm.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/stat_ops_expectation_value.cpp` & `qulacs-0.6.3/src/csim/stat_ops_expectation_value.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/stat_ops_probability.cpp` & `qulacs-0.6.3/src/csim/stat_ops_probability.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/stat_ops_transition_amplitude.cpp` & `qulacs-0.6.3/src/csim/stat_ops_transition_amplitude.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/type.hpp` & `qulacs-0.6.3/src/csim/type.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops.hpp` & `qulacs-0.6.3/src/csim/update_ops.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_control_multi_target_multi.cpp` & `qulacs-0.6.3/src/csim/update_ops_control_multi_target_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_control_multi_target_single.cpp` & `qulacs-0.6.3/src/csim/update_ops_control_multi_target_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_control_single_target_multi.cpp` & `qulacs-0.6.3/src/csim/update_ops_control_single_target_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_control_single_target_single.cpp` & `qulacs-0.6.3/src/csim/update_ops_control_single_target_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_cpp.hpp` & `qulacs-0.6.3/src/csim/update_ops_cpp.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_dm.cpp` & `qulacs-0.6.3/src/csim/update_ops_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_dm.hpp` & `qulacs-0.6.3/src/csim/update_ops_dm.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_matrix_dense_double.cpp` & `qulacs-0.6.3/src/csim/update_ops_matrix_dense_double.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_matrix_dense_double_eigen.cpp` & `qulacs-0.6.3/src/csim/update_ops_matrix_dense_double_eigen.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_matrix_dense_multi.cpp` & `qulacs-0.6.3/src/csim/update_ops_matrix_dense_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_matrix_dense_multi_eigen.cpp` & `qulacs-0.6.3/src/csim/update_ops_matrix_dense_multi_eigen.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_matrix_dense_single.cpp` & `qulacs-0.6.3/src/csim/update_ops_matrix_dense_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_matrix_diagonal_multi.cpp` & `qulacs-0.6.3/src/csim/update_ops_matrix_diagonal_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_matrix_diagonal_single.cpp` & `qulacs-0.6.3/src/csim/update_ops_matrix_diagonal_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_matrix_phase_single.cpp` & `qulacs-0.6.3/src/csim/update_ops_matrix_phase_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_named.cpp` & `qulacs-0.6.3/src/csim/update_ops_named.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_named_CNOT.cpp` & `qulacs-0.6.3/src/csim/update_ops_named_CNOT.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_named_CZ.cpp` & `qulacs-0.6.3/src/csim/update_ops_named_CZ.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_named_FusedSWAP.cpp` & `qulacs-0.6.3/src/csim/update_ops_named_FusedSWAP.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_named_H.cpp` & `qulacs-0.6.3/src/csim/update_ops_named_H.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_named_SWAP.cpp` & `qulacs-0.6.3/src/csim/update_ops_named_SWAP.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_named_X.cpp` & `qulacs-0.6.3/src/csim/update_ops_named_X.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_named_Y.cpp` & `qulacs-0.6.3/src/csim/update_ops_named_Y.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_named_Z.cpp` & `qulacs-0.6.3/src/csim/update_ops_named_Z.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_named_projection.cpp` & `qulacs-0.6.3/src/csim/update_ops_named_projection.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_named_state.cpp` & `qulacs-0.6.3/src/csim/update_ops_named_state.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_pauli_multi.cpp` & `qulacs-0.6.3/src/csim/update_ops_pauli_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_pauli_single.cpp` & `qulacs-0.6.3/src/csim/update_ops_pauli_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_qft.cpp` & `qulacs-0.6.3/src/csim/update_ops_qft.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_reflection.cpp` & `qulacs-0.6.3/src/csim/update_ops_reflection.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/update_ops_reversible_boolean.cpp` & `qulacs-0.6.3/src/csim/update_ops_reversible_boolean.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/utility.cpp` & `qulacs-0.6.3/src/csim/utility.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/csim/utility.hpp` & `qulacs-0.6.3/src/csim/utility.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/CMakeLists.txt` & `qulacs-0.6.3/src/gpusim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/memory_ops.cu` & `qulacs-0.6.3/src/gpusim/memory_ops.cu`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/memory_ops.h` & `qulacs-0.6.3/src/gpusim/memory_ops.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/memory_ops_device_functions.h` & `qulacs-0.6.3/src/gpusim/memory_ops_device_functions.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/stat_ops.cu` & `qulacs-0.6.3/src/gpusim/stat_ops.cu`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/stat_ops.h` & `qulacs-0.6.3/src/gpusim/stat_ops.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/stat_ops_device_functions.h` & `qulacs-0.6.3/src/gpusim/stat_ops_device_functions.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/test.cpp` & `qulacs-0.6.3/src/gpusim/test.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/update_ops_cuda.h` & `qulacs-0.6.3/src/gpusim/update_ops_cuda.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/update_ops_cuda_device_functions.h` & `qulacs-0.6.3/src/gpusim/update_ops_cuda_device_functions.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/update_ops_multi.cu` & `qulacs-0.6.3/src/gpusim/update_ops_multi.cu`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/update_ops_named.cu` & `qulacs-0.6.3/src/gpusim/update_ops_named.cu`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/update_ops_single.cu` & `qulacs-0.6.3/src/gpusim/update_ops_single.cu`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/util.cu` & `qulacs-0.6.3/src/gpusim/util.cu`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/util.cuh` & `qulacs-0.6.3/src/gpusim/util.cuh`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/util.h` & `qulacs-0.6.3/src/gpusim/util.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/util_common.h` & `qulacs-0.6.3/src/gpusim/util_common.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/gpusim/util_func.h` & `qulacs-0.6.3/src/gpusim/util_func.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/GradCalculator.cpp` & `qulacs-0.6.3/src/vqcsim/GradCalculator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/boolean_formula.hpp` & `qulacs-0.6.3/src/vqcsim/boolean_formula.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/causalcone_simulator.hpp` & `qulacs-0.6.3/src/vqcsim/causalcone_simulator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/differential.cpp` & `qulacs-0.6.3/src/vqcsim/differential.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/differential.hpp` & `qulacs-0.6.3/src/vqcsim/differential.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/loss_function.cpp` & `qulacs-0.6.3/src/vqcsim/loss_function.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/loss_function.hpp` & `qulacs-0.6.3/src/vqcsim/loss_function.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/optimizer.hpp` & `qulacs-0.6.3/src/vqcsim/optimizer.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/parametric_circuit.cpp` & `qulacs-0.6.3/src/vqcsim/parametric_circuit.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/parametric_circuit.hpp` & `qulacs-0.6.3/src/vqcsim/parametric_circuit.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/parametric_gate.hpp` & `qulacs-0.6.3/src/vqcsim/parametric_gate.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/parametric_gate_factory.cpp` & `qulacs-0.6.3/src/vqcsim/parametric_gate_factory.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/parametric_gate_factory.hpp` & `qulacs-0.6.3/src/vqcsim/parametric_gate_factory.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/parametric_simulator.cpp` & `qulacs-0.6.3/src/vqcsim/parametric_simulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/parametric_simulator.hpp` & `qulacs-0.6.3/src/vqcsim/parametric_simulator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/problem.hpp` & `qulacs-0.6.3/src/vqcsim/problem.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/src/vqcsim/solver.hpp` & `qulacs-0.6.3/src/vqcsim/solver.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/cppsim/test_KAK.cpp` & `qulacs-0.6.3/test/cppsim/test_KAK.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/cppsim/test_circuit.cpp` & `qulacs-0.6.3/test/cppsim/test_circuit.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/cppsim/test_circuit_multicpu.cpp` & `qulacs-0.6.3/test/gpusim/test_circuit.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,1033 +1,924 @@
-#ifdef _USE_MPI
 #include <gtest/gtest.h>
 
+#include <cppsim/state_gpu.hpp>
+#include <cppsim/type.hpp>
+#include <csim/constant.hpp>
+
+#include "../util/util.hpp"
+// #define _USE_MATH_DEFINES
+// #include <cmath>
 #include <cppsim/circuit.hpp>
 #include <cppsim/circuit_optimizer.hpp>
 #include <cppsim/gate_factory.hpp>
 #include <cppsim/gate_matrix.hpp>
 #include <cppsim/gate_merge.hpp>
 #include <cppsim/observable.hpp>
 #include <cppsim/pauli_operator.hpp>
 #include <cppsim/state.hpp>
-#include <cppsim/type.hpp>
 #include <cppsim/utility.hpp>
-#include <csim/constant.hpp>
 #include <unsupported/Eigen/MatrixFunctions>
 #include <utility>
 
-#include "../util/util.hpp"
-
-TEST(CircuitTest_multicpu, CircuitBasic) {
-    const auto Identity = make_Identity();
-    const auto X = make_X();
-    const auto Y = make_Y();
-    const auto Z = make_Z();
-    const auto H = make_H();
-    const auto S = make_S();
-    const auto T = make_T();
-    const auto sqrtX = make_sqrtX();
-    const auto sqrtY = make_sqrtY();
-    const auto P0 = make_P0();
-    const auto P1 = make_P1();
-
-    const UINT n = 4;
-    UINT dim = 1ULL << n;
-    MPIutil& mpiutil = MPIutil::get_inst();
-    UINT mpirank = mpiutil.get_rank();
-    UINT mpisize = mpiutil.get_size();
-    ITYPE inner_dim = dim / mpisize;
-    ITYPE offs = inner_dim * mpirank;
-
-    Random random;
-    random.set_seed(2022);
+inline void set_eigen_from_gpu(
+    ComplexVector& dst, QuantumStateGpu& src, ITYPE dim) {
+    auto ptr = src.duplicate_data_cpp();
+    for (ITYPE i = 0; i < dim; ++i) dst[i] = ptr[i];
+    free(ptr);
+}
 
-    QuantumState state_ref(n, false);
-    QuantumState state(n, true);
-    ComplexVector state_eigen(dim);
-
-    state.set_Haar_random_state();
-    state_ref.load(&state);
-    for (ITYPE i = 0; i < dim; ++i) state_eigen[i] = state_ref.data_cpp()[i];
+inline void assert_eigen_eq_gpu(
+    ComplexVector& v1, QuantumStateGpu& v2, ITYPE dim, double eps) {
+    auto ptr = v2.duplicate_data_cpp();
+    for (ITYPE i = 0; i < dim; ++i) {
+        ASSERT_NEAR(ptr[i].real(), v1[i].real(), eps);
+        ASSERT_NEAR(ptr[i].imag(), v1[i].imag(), eps);
+    }
+    free(ptr);
+}
 
-    QuantumCircuit circuit(n);
-    UINT target, target_sub;
-    double angle;
-    std::complex<double> imag_unit(0, 1);
+inline void assert_cpu_eq_gpu(QuantumStateCpu& state_cpu,
+    QuantumStateGpu& state_gpu, ITYPE dim, double eps) {
+    auto gpu_state_vector = state_gpu.duplicate_data_cpp();
+    for (ITYPE i = 0; i < dim; ++i) {
+        ASSERT_NEAR(
+            state_cpu.data_cpp()[i].real(), gpu_state_vector[i].real(), eps);
+        ASSERT_NEAR(
+            state_cpu.data_cpp()[i].imag(), gpu_state_vector[i].imag(), eps);
+    }
+    free(gpu_state_vector);
+}
 
-    target = random.int32() % n;
-    circuit.add_X_gate(target);
-    state_eigen = get_expanded_eigen_matrix_with_identity(
-                      target, get_eigen_matrix_single_Pauli(1), n) *
-                  state_eigen;
-
-    target = random.int32() % n;
-    circuit.add_Y_gate(target);
-    state_eigen = get_expanded_eigen_matrix_with_identity(
-                      target, get_eigen_matrix_single_Pauli(2), n) *
-                  state_eigen;
-
-    target = random.int32() % n;
-    circuit.add_Z_gate(target);
-    state_eigen = get_expanded_eigen_matrix_with_identity(
-                      target, get_eigen_matrix_single_Pauli(3), n) *
-                  state_eigen;
-
-    target = random.int32() % n;
-    circuit.add_H_gate(target);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target, H, n) * state_eigen;
-
-    target = random.int32() % n;
-    circuit.add_S_gate(target);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target, S, n) * state_eigen;
-
-    target = random.int32() % n;
-    circuit.add_Sdag_gate(target);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target, S.adjoint(), n) *
-        state_eigen;
-
-    target = random.int32() % n;
-    circuit.add_T_gate(target);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target, T, n) * state_eigen;
-
-    target = random.int32() % n;
-    circuit.add_Tdag_gate(target);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target, T.adjoint(), n) *
-        state_eigen;
-
-    target = random.int32() % n;
-    circuit.add_sqrtX_gate(target);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target, sqrtX, n) * state_eigen;
-
-    target = random.int32() % n;
-    circuit.add_sqrtXdag_gate(target);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target, sqrtX.adjoint(), n) *
-        state_eigen;
-
-    target = random.int32() % n;
-    circuit.add_sqrtY_gate(target);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target, sqrtY, n) * state_eigen;
-
-    target = random.int32() % n;
-    circuit.add_sqrtYdag_gate(target);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target, sqrtY.adjoint(), n) *
-        state_eigen;
-
-    target = random.int32() % n;
-    circuit.add_P0_gate(target);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target, P0, n) * state_eigen;
-
-    target = (target + 1) % n;
-    circuit.add_P1_gate(target);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target, P1, n) * state_eigen;
-
-    target = random.int32() % n;
-    angle = random.uniform() * 3.14159;
-    circuit.add_RX_gate(target, angle);
-    circuit.add_RotInvX_gate(target, angle);
-    circuit.add_RotX_gate(target, angle);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target,
-            cos(angle / 2) * Identity + imag_unit * sin(angle / 2) * X, n) *
-        state_eigen;
-
-    target = random.int32() % n;
-    angle = random.uniform() * 3.14159;
-    circuit.add_RY_gate(target, angle);
-    circuit.add_RotInvY_gate(target, angle);
-    circuit.add_RotY_gate(target, angle);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target,
-            cos(angle / 2) * Identity + imag_unit * sin(angle / 2) * Y, n) *
-        state_eigen;
-
-    target = random.int32() % n;
-    angle = random.uniform() * 3.14159;
-    circuit.add_RZ_gate(target, angle);
-    circuit.add_RotInvZ_gate(target, angle);
-    circuit.add_RotZ_gate(target, angle);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target,
-            cos(angle / 2) * Identity + imag_unit * sin(angle / 2) * Z, n) *
-        state_eigen;
-
-    target = random.int32() % n;
-    target_sub = random.int32() % (n - 1);
-    if (target_sub >= target) target_sub++;
-    circuit.add_CNOT_gate(target, target_sub);
-    state_eigen =
-        get_eigen_matrix_full_qubit_CNOT(target, target_sub, n) * state_eigen;
-
-    target = random.int32() % n;
-    target_sub = random.int32() % (n - 1);
-    if (target_sub >= target) target_sub++;
-    circuit.add_CZ_gate(target, target_sub);
-    state_eigen =
-        get_eigen_matrix_full_qubit_CZ(target, target_sub, n) * state_eigen;
-
-    target = random.int32() % n;
-    target_sub = random.int32() % (n - 1);
-    if (target_sub >= target) target_sub++;
-    circuit.add_SWAP_gate(target, target_sub);
-    state_eigen =
-        get_eigen_matrix_full_qubit_SWAP(target, target_sub, n) * state_eigen;
-
-    target = random.int32() % n;
-    circuit.add_U1_gate(target, M_PI);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target, Z, n) * state_eigen;
-
-    target = random.int32() % n;
-    circuit.add_U2_gate(target, 0, M_PI);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target, H, n) * state_eigen;
-
-    target = random.int32() % n;
-    angle = random.uniform() * 3.14159;
-    circuit.add_U3_gate(target, -angle, 0, 0);
-    state_eigen =
-        get_expanded_eigen_matrix_with_identity(target,
-            cos(angle / 2) * Identity + imag_unit * sin(angle / 2) * Y, n) *
-        state_eigen;
-
-    std::vector<UINT> target_index_list{0, 1, 2, 3};
-    std::vector<UINT> pauli_id_list{0, 1, 2, 3};
-    circuit.add_multi_Pauli_gate(target_index_list, pauli_id_list);
-
-    // add same gate == cancel above pauli gate
-    PauliOperator pauli = PauliOperator("I 0 X 1 Y 2 Z 3");
-    circuit.add_multi_Pauli_gate(pauli);
-
-    ComplexMatrix mat_x(2, 2);
-    target = random.int32() % n;
-    mat_x << 0, 1, 1, 0;
-    circuit.add_dense_matrix_gate(target, mat_x);
-
-    state_eigen = get_expanded_eigen_matrix_with_identity(
-                      target, get_eigen_matrix_single_Pauli(1), n) *
-                  state_eigen;
-
-    circuit.update_quantum_state(&state);
-
-    if (state.get_device_name() == "multi-cpu")
-        for (ITYPE i = 0; i < inner_dim; ++i)
-            ASSERT_NEAR(
-                abs(state_eigen[i + offs] - state.data_cpp()[i]), 0, eps);
-    else
-        for (ITYPE i = 0; i < dim; ++i)
-            ASSERT_NEAR(abs(state_eigen[i] - state.data_cpp()[i]), 0, eps);
+inline void assert_gpu_eq_gpu(QuantumStateGpu& state_gpu1,
+    QuantumStateGpu& state_gpu2, ITYPE dim, double eps) {
+    auto gpu_state_vector1 = state_gpu1.duplicate_data_cpp();
+    auto gpu_state_vector2 = state_gpu2.duplicate_data_cpp();
+    for (ITYPE i = 0; i < dim; ++i) {
+        ASSERT_NEAR(
+            gpu_state_vector1[i].real(), gpu_state_vector2[i].real(), eps);
+        ASSERT_NEAR(
+            gpu_state_vector1[i].imag(), gpu_state_vector2[i].imag(), eps);
+    }
+    free(gpu_state_vector1);
+    free(gpu_state_vector2);
 }
 
-TEST(CircuitTest_multicpu, CircuitRev) {
+TEST(CircuitTest, CircuitBasic) {
+    Eigen::MatrixXcd Identity(2, 2), X(2, 2), Y(2, 2), Z(2, 2), H(2, 2),
+        S(2, 2), T(2, 2), sqrtX(2, 2), sqrtY(2, 2), P0(2, 2), P1(2, 2);
+
+    Identity << 1, 0, 0, 1;
+    X << 0, 1, 1, 0;
+    Y << 0, -1.i, 1.i, 0;
+    Z << 1, 0, 0, -1;
+    H << 1, 1, 1, -1;
+    H /= sqrt(2.);
+    S << 1, 0, 0, 1.i;
+    T << 1, 0, 0, (1. + 1.i) / sqrt(2.);
+    sqrtX << 0.5 + 0.5i, 0.5 - 0.5i, 0.5 - 0.5i, 0.5 + 0.5i;
+    sqrtY << 0.5 + 0.5i, -0.5 - 0.5i, 0.5 + 0.5i, 0.5 + 0.5i;
+    P0 << 1, 0, 0, 0;
+    P1 << 0, 0, 0, 1;
+
     const UINT n = 4;
     const UINT dim = 1ULL << n;
-    MPIutil& mpiutil = MPIutil::get_inst();
-    UINT mpirank = mpiutil.get_rank();
-    UINT mpisize = mpiutil.get_size();
-    ITYPE inner_dim = dim / mpisize;
-    ITYPE offs = inner_dim * mpirank;
 
     Random random;
-    random.set_seed(2022);
-
-    QuantumState state(n, true);
-    QuantumState state_ref(n, false);
-    ComplexVector state_eigen(dim);
-
-    state.set_Haar_random_state();
-    state_ref.load(&state);
-    for (ITYPE i = 0; i < dim; ++i) state_eigen[i] = state_ref.data_cpp()[i];
-
-    QuantumCircuit circuit(n);
-    UINT target, target_sub;
-    double angle;
-
-    target = random.int32() % n;
-    circuit.add_X_gate(target);
-
-    target = random.int32() % n;
-    circuit.add_Y_gate(target);
-
-    target = random.int32() % n;
-    circuit.add_Z_gate(target);
-
-    target = random.int32() % n;
-    circuit.add_H_gate(target);
-
-    target = random.int32() % n;
-    circuit.add_S_gate(target);
-
-    target = random.int32() % n;
-    circuit.add_Sdag_gate(target);
-
-    target = random.int32() % n;
-    circuit.add_T_gate(target);
-
-    target = random.int32() % n;
-    circuit.add_Tdag_gate(target);
-
-    target = random.int32() % n;
-    circuit.add_sqrtX_gate(target);
-
-    target = random.int32() % n;
-    circuit.add_sqrtXdag_gate(target);
-
-    target = random.int32() % n;
-    circuit.add_sqrtY_gate(target);
-
-    target = random.int32() % n;
-    circuit.add_sqrtYdag_gate(target);
-
-    target = random.int32() % n;
-    angle = random.uniform() * 3.14159;
-    circuit.add_RX_gate(target, angle);
-    circuit.add_RotInvX_gate(target, angle);
-    circuit.add_RotX_gate(target, angle);
-
-    target = random.int32() % n;
-    angle = random.uniform() * 3.14159;
-    circuit.add_RY_gate(target, angle);
-    circuit.add_RotInvY_gate(target, angle);
-    circuit.add_RotInvY_gate(target, angle);
-
-    target = random.int32() % n;
-    angle = random.uniform() * 3.14159;
-    circuit.add_RZ_gate(target, angle);
-    circuit.add_RotInvZ_gate(target, angle);
-    circuit.add_RotZ_gate(target, -angle);
-
-    target = random.int32() % n;
-    target_sub = random.int32() % (n - 1);
-    if (target_sub >= target) target_sub++;
-    circuit.add_CNOT_gate(target, target_sub);
-
-    target = random.int32() % n;
-    target_sub = random.int32() % (n - 1);
-    if (target_sub >= target) target_sub++;
-    circuit.add_CZ_gate(target, target_sub);
-
-    target = random.int32() % n;
-    target_sub = random.int32() % (n - 1);
-    if (target_sub >= target) target_sub++;
-    circuit.add_SWAP_gate(target, target_sub);
-
-    Observable observable(n);
-    angle = 2 * PI * random.uniform();
-
-    observable.add_operator(1.0, "Z 0");
-    observable.add_operator(2.0, "Z 0 Z 1");
-
-    circuit.add_diagonal_observable_rotation_gate(observable, angle);
-
-    circuit.update_quantum_state(&state);
-
-    auto revcircuit = circuit.get_inverse();
+    std::complex<double> imag_unit(0, 1);
 
-    revcircuit->update_quantum_state(&state);
+    int ngpus = get_num_device();
+    for (int idx = 0; idx < ngpus; ++idx) {
+        set_device(idx);
+        auto stream_ptr = allocate_cuda_stream_host(1, idx);
+
+        QuantumStateGpu state(n, idx);
+        ComplexVector state_eigen(dim);
+
+        state.set_Haar_random_state();
+        set_eigen_from_gpu(state_eigen, state, dim);
+
+        QuantumCircuit circuit(n);
+        UINT target, target_sub;
+        double angle;
+
+        target = random.int32() % n;
+        circuit.add_X_gate(target);
+        state_eigen = get_expanded_eigen_matrix_with_identity(
+                          target, get_eigen_matrix_single_Pauli(1), n) *
+                      state_eigen;
+
+        target = random.int32() % n;
+        circuit.add_Y_gate(target);
+        state_eigen = get_expanded_eigen_matrix_with_identity(
+                          target, get_eigen_matrix_single_Pauli(2), n) *
+                      state_eigen;
+
+        target = random.int32() % n;
+        circuit.add_Z_gate(target);
+        state_eigen = get_expanded_eigen_matrix_with_identity(
+                          target, get_eigen_matrix_single_Pauli(3), n) *
+                      state_eigen;
+
+        target = random.int32() % n;
+        circuit.add_H_gate(target);
+        state_eigen =
+            get_expanded_eigen_matrix_with_identity(target, H, n) * state_eigen;
+
+        target = random.int32() % n;
+        circuit.add_S_gate(target);
+        state_eigen =
+            get_expanded_eigen_matrix_with_identity(target, S, n) * state_eigen;
+
+        target = random.int32() % n;
+        circuit.add_Sdag_gate(target);
+        state_eigen =
+            get_expanded_eigen_matrix_with_identity(target, S.adjoint(), n) *
+            state_eigen;
+
+        target = random.int32() % n;
+        circuit.add_T_gate(target);
+        state_eigen =
+            get_expanded_eigen_matrix_with_identity(target, T, n) * state_eigen;
+
+        target = random.int32() % n;
+        circuit.add_Tdag_gate(target);
+        state_eigen =
+            get_expanded_eigen_matrix_with_identity(target, T.adjoint(), n) *
+            state_eigen;
+
+        target = random.int32() % n;
+        circuit.add_sqrtX_gate(target);
+        state_eigen =
+            get_expanded_eigen_matrix_with_identity(target, sqrtX, n) *
+            state_eigen;
+
+        target = random.int32() % n;
+        circuit.add_sqrtXdag_gate(target);
+        state_eigen = get_expanded_eigen_matrix_with_identity(
+                          target, sqrtX.adjoint(), n) *
+                      state_eigen;
+
+        target = random.int32() % n;
+        circuit.add_sqrtY_gate(target);
+        state_eigen =
+            get_expanded_eigen_matrix_with_identity(target, sqrtY, n) *
+            state_eigen;
+
+        target = random.int32() % n;
+        circuit.add_sqrtYdag_gate(target);
+        state_eigen = get_expanded_eigen_matrix_with_identity(
+                          target, sqrtY.adjoint(), n) *
+                      state_eigen;
+
+        target = random.int32() % n;
+        circuit.add_P0_gate(target);
+        state_eigen = get_expanded_eigen_matrix_with_identity(target, P0, n) *
+                      state_eigen;
+
+        target = (target + 1) % n;
+        circuit.add_P1_gate(target);
+        state_eigen = get_expanded_eigen_matrix_with_identity(target, P1, n) *
+                      state_eigen;
+
+        target = random.int32() % n;
+        angle = random.uniform() * 3.14159;
+        circuit.add_RotInvX_gate(target, angle);
+        state_eigen =
+            get_expanded_eigen_matrix_with_identity(target,
+                cos(angle / 2) * Identity + 1.i * sin(angle / 2) * X, n) *
+            state_eigen;
+
+        target = random.int32() % n;
+        angle = random.uniform() * 3.14159;
+        circuit.add_RotInvY_gate(target, angle);
+        state_eigen =
+            get_expanded_eigen_matrix_with_identity(target,
+                cos(angle / 2) * Identity + 1.i * sin(angle / 2) * Y, n) *
+            state_eigen;
+
+        target = random.int32() % n;
+        angle = random.uniform() * 3.14159;
+        circuit.add_RotInvZ_gate(target, angle);
+        state_eigen =
+            get_expanded_eigen_matrix_with_identity(target,
+                cos(angle / 2) * Identity + 1.i * sin(angle / 2) * Z, n) *
+            state_eigen;
+
+        target = random.int32() % n;
+        target_sub = random.int32() % (n - 1);
+        if (target_sub >= target) target_sub++;
+        circuit.add_CNOT_gate(target, target_sub);
+        state_eigen = get_eigen_matrix_full_qubit_CNOT(target, target_sub, n) *
+                      state_eigen;
+
+        target = random.int32() % n;
+        target_sub = random.int32() % (n - 1);
+        if (target_sub >= target) target_sub++;
+        circuit.add_CZ_gate(target, target_sub);
+        state_eigen =
+            get_eigen_matrix_full_qubit_CZ(target, target_sub, n) * state_eigen;
+
+        target = random.int32() % n;
+        target_sub = random.int32() % (n - 1);
+        if (target_sub >= target) target_sub++;
+        circuit.add_SWAP_gate(target, target_sub);
+        state_eigen = get_eigen_matrix_full_qubit_SWAP(target, target_sub, n) *
+                      state_eigen;
 
-    if (state.get_device_name() == "multi-cpu")
-        for (ITYPE i = 0; i < inner_dim; ++i)
-            ASSERT_NEAR(
-                abs(state_eigen[i + offs] - state.data_cpp()[i]), 0, eps);
-    else
-        for (ITYPE i = 0; i < dim; ++i)
-            ASSERT_NEAR(abs(state_eigen[i] - state.data_cpp()[i]), 0, eps);
+        circuit.update_quantum_state(&state);
 
-    delete revcircuit;
+        assert_eigen_eq_gpu(state_eigen, state, dim, eps);
+    }
 }
 
-TEST(CircuitTest_multicpu, CircuitOptimize) {
-    MPIutil& m = MPIutil::get_inst();
-    const UINT num_global_qubit = (UINT)std::log2(m.get_size());
-    UINT n = 4 + num_global_qubit;
+TEST(CircuitTest, CircuitOptimize) {
+    const UINT n = 4;
     const UINT dim = 1ULL << n;
 
     {
         // merge successive gates
-        QuantumState state(n, true), test_state(n, true);
-        state.set_Haar_random_state();
-        test_state.load(&state);
-        QuantumCircuit circuit(n);
+        int ngpus = get_num_device();
+        for (int idx = 0; idx < ngpus; ++idx) {
+            set_device(idx);
+
+            QuantumStateGpu state(n, idx), test_state(n, idx);
+            state.set_Haar_random_state();
+            test_state.load(&state);
+            QuantumCircuit circuit(n);
+
+            circuit.add_X_gate(0);
+            circuit.add_Y_gate(0);
+            UINT block_size = 2;
+            UINT expected_depth = 1;
+            UINT expected_gate_count = 1;
 
-        circuit.add_X_gate(0);
-        circuit.add_Y_gate(0);
-        UINT block_size = 2;
-        UINT expected_depth = 1;
-        UINT expected_gate_count = 1;
-
-        QuantumCircuit* copy_circuit = circuit.copy();
-        QuantumCircuitOptimizer qco;
-        qco.optimize(copy_circuit, block_size);
-        circuit.update_quantum_state(&test_state);
-        copy_circuit->update_quantum_state(&state);
-
-        ASSERT_STATE_NEAR(state, test_state, eps);
-        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-        delete copy_circuit;
+            QuantumCircuit* copy_circuit = circuit.copy();
+            QuantumCircuitOptimizer qco;
+            qco.optimize(copy_circuit, block_size);
+            circuit.update_quantum_state(&test_state);
+            copy_circuit->update_quantum_state(&state);
+            // std::cout << circuit << std::endl << copy_circuit << std::endl;
+            assert_gpu_eq_gpu(state, test_state, dim, eps);
+            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+            delete copy_circuit;
+        }
     }
 
     {
         // tensor product, merged
-        QuantumState state(n, true), test_state(n, true);
-        state.set_Haar_random_state();
-        test_state.load(&state);
-        QuantumCircuit circuit(n);
+        int ngpus = get_num_device();
+        for (int idx = 0; idx < ngpus; ++idx) {
+            set_device(idx);
+
+            QuantumStateGpu state(n, idx), test_state(n, idx);
+            state.set_Haar_random_state();
+            test_state.load(&state);
+            QuantumCircuit circuit(n);
+
+            circuit.add_X_gate(0);
+            circuit.add_Y_gate(1);
+            UINT block_size = 2;
+            UINT expected_depth = 1;
+            UINT expected_gate_count = 1;
 
-        circuit.add_X_gate(0);
-        circuit.add_Y_gate(1);
-        UINT block_size = 2;
-        UINT expected_depth = 1;
-        UINT expected_gate_count = 1;
-
-        QuantumCircuit* copy_circuit = circuit.copy();
-        QuantumCircuitOptimizer qco;
-        qco.optimize(copy_circuit, block_size);
-        circuit.update_quantum_state(&test_state);
-        copy_circuit->update_quantum_state(&state);
-
-        ASSERT_STATE_NEAR(state, test_state, eps);
-        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-        delete copy_circuit;
+            QuantumCircuit* copy_circuit = circuit.copy();
+            QuantumCircuitOptimizer qco;
+            qco.optimize(copy_circuit, block_size);
+            circuit.update_quantum_state(&test_state);
+            copy_circuit->update_quantum_state(&state);
+            // std::cout << circuit << std::endl << copy_circuit << std::endl;
+            assert_gpu_eq_gpu(state, test_state, dim, eps);
+            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+            delete copy_circuit;
+        }
     }
 
     {
         // do not take tensor product
-        QuantumState state(n, true), test_state(n, true);
-        state.set_Haar_random_state();
-        test_state.load(&state);
-        QuantumCircuit circuit(n);
+        int ngpus = get_num_device();
+        for (int idx = 0; idx < ngpus; ++idx) {
+            set_device(idx);
+
+            QuantumStateGpu state(n, idx), test_state(n, idx);
+            state.set_Haar_random_state();
+            test_state.load(&state);
+            QuantumCircuit circuit(n);
+
+            circuit.add_X_gate(0);
+            circuit.add_Y_gate(1);
+            UINT block_size = 1;
+            UINT expected_depth = 1;
+            UINT expected_gate_count = 2;
 
-        circuit.add_X_gate(0);
-        circuit.add_Y_gate(1);
-        UINT block_size = 1;
-        UINT expected_depth = 1;
-        UINT expected_gate_count = 2;
-
-        QuantumCircuit* copy_circuit = circuit.copy();
-        QuantumCircuitOptimizer qco;
-        qco.optimize(copy_circuit, block_size);
-        circuit.update_quantum_state(&test_state);
-        copy_circuit->update_quantum_state(&state);
-
-        ASSERT_STATE_NEAR(state, test_state, eps);
-        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-        delete copy_circuit;
+            QuantumCircuit* copy_circuit = circuit.copy();
+            QuantumCircuitOptimizer qco;
+            qco.optimize(copy_circuit, block_size);
+            circuit.update_quantum_state(&test_state);
+            copy_circuit->update_quantum_state(&state);
+            // std::cout << circuit << std::endl << copy_circuit << std::endl;
+            assert_gpu_eq_gpu(state, test_state, dim, eps);
+            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+            delete copy_circuit;
+        }
     }
 
     {
         // CNOT, control does not commute with X
-        QuantumState state(n, true), test_state(n, true);
-        state.set_Haar_random_state();
-        test_state.load(&state);
-        QuantumCircuit circuit(n);
+        int ngpus = get_num_device();
+        for (int idx = 0; idx < ngpus; ++idx) {
+            set_device(idx);
+
+            QuantumStateGpu state(n, idx), test_state(n, idx);
+            state.set_Haar_random_state();
+            test_state.load(&state);
+            QuantumCircuit circuit(n);
+
+            circuit.add_X_gate(0);
+            circuit.add_CNOT_gate(0, 1);
+            circuit.add_Y_gate(0);
+            UINT block_size = 1;
+            UINT expected_depth = 3;
+            UINT expected_gate_count = 3;
 
-        circuit.add_X_gate(0);
-        circuit.add_CNOT_gate(0, 1);
-        circuit.add_Y_gate(0);
-        UINT block_size = 1;
-        UINT expected_depth = 3;
-        UINT expected_gate_count = 3;
-
-        QuantumCircuit* copy_circuit = circuit.copy();
-        QuantumCircuitOptimizer qco;
-        qco.optimize(copy_circuit, block_size);
-        circuit.update_quantum_state(&test_state);
-        copy_circuit->update_quantum_state(&state);
-
-        ASSERT_STATE_NEAR(state, test_state, eps);
-        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-        delete copy_circuit;
+            QuantumCircuit* copy_circuit = circuit.copy();
+            QuantumCircuitOptimizer qco;
+            qco.optimize(copy_circuit, block_size);
+            circuit.update_quantum_state(&test_state);
+            copy_circuit->update_quantum_state(&state);
+            // std::cout << circuit << std::endl << copy_circuit << std::endl;
+            assert_gpu_eq_gpu(state, test_state, dim, eps);
+            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+            delete copy_circuit;
+        }
     }
 
     {
         // CNOT, control does not commute with Z
-        QuantumState state(n, true), test_state(n, true);
-        state.set_Haar_random_state();
-        test_state.load(&state);
-        QuantumCircuit circuit(n);
+        int ngpus = get_num_device();
+        for (int idx = 0; idx < ngpus; ++idx) {
+            set_device(idx);
+
+            QuantumStateGpu state(n, idx), test_state(n, idx);
+            state.set_Haar_random_state();
+            test_state.load(&state);
+            QuantumCircuit circuit(n);
+
+            circuit.add_X_gate(0);
+            circuit.add_CNOT_gate(0, 1);
+            circuit.add_Z_gate(0);
+            UINT block_size = 1;
+            UINT expected_depth = 2;
+            UINT expected_gate_count = 2;
 
-        circuit.add_X_gate(0);
-        circuit.add_CNOT_gate(0, 1);
-        circuit.add_Z_gate(0);
-        UINT block_size = 1;
-        UINT expected_depth = 2;
-        UINT expected_gate_count = 2;
-
-        QuantumCircuit* copy_circuit = circuit.copy();
-        QuantumCircuitOptimizer qco;
-        qco.optimize(copy_circuit, block_size);
-        circuit.update_quantum_state(&test_state);
-        copy_circuit->update_quantum_state(&state);
-
-        ASSERT_STATE_NEAR(state, test_state, eps);
-        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-        delete copy_circuit;
+            QuantumCircuit* copy_circuit = circuit.copy();
+            QuantumCircuitOptimizer qco;
+            qco.optimize(copy_circuit, block_size);
+            circuit.update_quantum_state(&test_state);
+            copy_circuit->update_quantum_state(&state);
+            // std::cout << circuit << std::endl << copy_circuit << std::endl;
+            assert_gpu_eq_gpu(state, test_state, dim, eps);
+            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+            delete copy_circuit;
+        }
     }
 
     {
         // CNOT, control commute with Z
-        QuantumState state(n, true), test_state(n, true);
-        state.set_Haar_random_state();
-        test_state.load(&state);
-        QuantumCircuit circuit(n);
+        int ngpus = get_num_device();
+        for (int idx = 0; idx < ngpus; ++idx) {
+            set_device(idx);
+
+            QuantumStateGpu state(n, idx), test_state(n, idx);
+            state.set_Haar_random_state();
+            test_state.load(&state);
+            QuantumCircuit circuit(n);
+
+            circuit.add_Z_gate(0);
+            circuit.add_CNOT_gate(0, 1);
+            circuit.add_Z_gate(0);
+            UINT block_size = 1;
+            UINT expected_depth = 2;
+            UINT expected_gate_count = 2;
 
-        circuit.add_Z_gate(0);
-        circuit.add_CNOT_gate(0, 1);
-        circuit.add_Z_gate(0);
-        UINT block_size = 1;
-        UINT expected_depth = 2;
-        UINT expected_gate_count = 2;
-
-        QuantumCircuit* copy_circuit = circuit.copy();
-        QuantumCircuitOptimizer qco;
-        qco.optimize(copy_circuit, block_size);
-        circuit.update_quantum_state(&test_state);
-        copy_circuit->update_quantum_state(&state);
-        ASSERT_STATE_NEAR(state, test_state, eps);
-        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-        delete copy_circuit;
+            QuantumCircuit* copy_circuit = circuit.copy();
+            QuantumCircuitOptimizer qco;
+            qco.optimize(copy_circuit, block_size);
+            circuit.update_quantum_state(&test_state);
+            copy_circuit->update_quantum_state(&state);
+            // std::cout << circuit << std::endl << copy_circuit << std::endl;
+            assert_gpu_eq_gpu(state, test_state, dim, eps);
+            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+            delete copy_circuit;
+        }
     }
 
     {
         // CNOT, target commute with X
-        QuantumState state(n, true), test_state(n, true);
-        state.set_Haar_random_state();
-        test_state.load(&state);
-        QuantumCircuit circuit(n);
+        int ngpus = get_num_device();
+        for (int idx = 0; idx < ngpus; ++idx) {
+            set_device(idx);
+
+            QuantumStateGpu state(n, idx), test_state(n, idx);
+            state.set_Haar_random_state();
+            test_state.load(&state);
+            QuantumCircuit circuit(n);
+
+            circuit.add_X_gate(1);
+            circuit.add_CNOT_gate(0, 1);
+            circuit.add_X_gate(1);
+            UINT block_size = 1;
+            UINT expected_depth = 2;
+            UINT expected_gate_count = 2;
 
-        circuit.add_X_gate(1);
-        circuit.add_CNOT_gate(0, 1);
-        circuit.add_X_gate(1);
-        UINT block_size = 1;
-        UINT expected_depth = 2;
-        UINT expected_gate_count = 2;
-
-        QuantumCircuit* copy_circuit = circuit.copy();
-        QuantumCircuitOptimizer qco;
-        qco.optimize(copy_circuit, block_size);
-        circuit.update_quantum_state(&test_state);
-        copy_circuit->update_quantum_state(&state);
-
-        ASSERT_STATE_NEAR(state, test_state, eps);
-        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-        delete copy_circuit;
+            QuantumCircuit* copy_circuit = circuit.copy();
+            QuantumCircuitOptimizer qco;
+            qco.optimize(copy_circuit, block_size);
+            circuit.update_quantum_state(&test_state);
+            copy_circuit->update_quantum_state(&state);
+            // std::cout << circuit << std::endl << copy_circuit << std::endl;
+            assert_gpu_eq_gpu(state, test_state, dim, eps);
+            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+            delete copy_circuit;
+        }
     }
 
     {
         // CNOT, target commute with X
-        QuantumState state(n, true), test_state(n, true);
-        state.set_Haar_random_state();
-        test_state.load(&state);
-        QuantumCircuit circuit(n);
+        int ngpus = get_num_device();
+        for (int idx = 0; idx < ngpus; ++idx) {
+            set_device(idx);
+
+            QuantumStateGpu state(n, idx), test_state(n, idx);
+            state.set_Haar_random_state();
+            test_state.load(&state);
+            QuantumCircuit circuit(n);
+
+            circuit.add_Z_gate(1);
+            circuit.add_CNOT_gate(0, 1);
+            circuit.add_X_gate(1);
+            UINT block_size = 1;
+            UINT expected_depth = 2;
+            UINT expected_gate_count = 2;
 
-        circuit.add_Z_gate(1);
-        circuit.add_CNOT_gate(0, 1);
-        circuit.add_X_gate(1);
-        UINT block_size = 1;
-        UINT expected_depth = 2;
-        UINT expected_gate_count = 2;
-
-        QuantumCircuit* copy_circuit = circuit.copy();
-        QuantumCircuitOptimizer qco;
-        qco.optimize(copy_circuit, block_size);
-        circuit.update_quantum_state(&test_state);
-        copy_circuit->update_quantum_state(&state);
-
-        ASSERT_STATE_NEAR(state, test_state, eps);
-        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-        delete copy_circuit;
+            QuantumCircuit* copy_circuit = circuit.copy();
+            QuantumCircuitOptimizer qco;
+            qco.optimize(copy_circuit, block_size);
+            circuit.update_quantum_state(&test_state);
+            copy_circuit->update_quantum_state(&state);
+            // std::cout << circuit << std::endl << copy_circuit << std::endl;
+            assert_gpu_eq_gpu(state, test_state, dim, eps);
+            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+            delete copy_circuit;
+        }
     }
 
     {
         // CNOT, target commute with X
-        QuantumState state(n, true), test_state(n, true);
-        state.set_Haar_random_state();
-        test_state.load(&state);
-        QuantumCircuit circuit(n);
+        int ngpus = get_num_device();
+        for (int idx = 0; idx < ngpus; ++idx) {
+            set_device(idx);
+
+            QuantumStateGpu state(n, idx), test_state(n, idx);
+            state.set_Haar_random_state();
+            test_state.load(&state);
+            QuantumCircuit circuit(n);
+
+            circuit.add_X_gate(1);
+            circuit.add_CNOT_gate(0, 1);
+            circuit.add_Z_gate(1);
+            UINT block_size = 1;
+            UINT expected_depth = 2;
+            UINT expected_gate_count = 2;
 
-        circuit.add_X_gate(1);
-        circuit.add_CNOT_gate(0, 1);
-        circuit.add_Z_gate(1);
-        UINT block_size = 1;
-        UINT expected_depth = 2;
-        UINT expected_gate_count = 2;
-
-        QuantumCircuit* copy_circuit = circuit.copy();
-        QuantumCircuitOptimizer qco;
-        qco.optimize(copy_circuit, block_size);
-        circuit.update_quantum_state(&test_state);
-        copy_circuit->update_quantum_state(&state);
-        ASSERT_STATE_NEAR(state, test_state, eps);
-        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-        delete copy_circuit;
+            QuantumCircuit* copy_circuit = circuit.copy();
+            QuantumCircuitOptimizer qco;
+            qco.optimize(copy_circuit, block_size);
+            circuit.update_quantum_state(&test_state);
+            copy_circuit->update_quantum_state(&state);
+            // std::cout << circuit << std::endl << copy_circuit << std::endl;
+            // std::cout << state << std::endl << test_state << std::endl;
+            assert_gpu_eq_gpu(state, test_state, dim, eps);
+            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+            delete copy_circuit;
+        }
     }
 
     {
         // CNOT, target commute with X
-        QuantumState state(n, true), test_state(n, true);
-        state.set_Haar_random_state();
-        test_state.load(&state);
-        QuantumCircuit circuit(n);
+        int ngpus = get_num_device();
+        for (int idx = 0; idx < ngpus; ++idx) {
+            set_device(idx);
+
+            QuantumStateGpu state(n, idx), test_state(n, idx);
+            state.set_Haar_random_state();
+            test_state.load(&state);
+            QuantumCircuit circuit(n);
+
+            circuit.add_Z_gate(1);
+            circuit.add_CNOT_gate(0, 1);
+            circuit.add_Z_gate(1);
+            UINT block_size = 1;
+            UINT expected_depth = 3;
+            UINT expected_gate_count = 3;
 
-        circuit.add_Z_gate(1);
-        circuit.add_CNOT_gate(0, 1);
-        circuit.add_Z_gate(1);
-        UINT block_size = 1;
-        UINT expected_depth = 3;
-        UINT expected_gate_count = 3;
-
-        QuantumCircuit* copy_circuit = circuit.copy();
-        QuantumCircuitOptimizer qco;
-        qco.optimize(copy_circuit, block_size);
-        circuit.update_quantum_state(&test_state);
-        copy_circuit->update_quantum_state(&state);
-
-        ASSERT_STATE_NEAR(state, test_state, eps);
-        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-        delete copy_circuit;
+            QuantumCircuit* copy_circuit = circuit.copy();
+            QuantumCircuitOptimizer qco;
+            qco.optimize(copy_circuit, block_size);
+            circuit.update_quantum_state(&test_state);
+            copy_circuit->update_quantum_state(&state);
+            // std::cout << circuit << std::endl << copy_circuit << std::endl;
+            assert_gpu_eq_gpu(state, test_state, dim, eps);
+            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+            delete copy_circuit;
+        }
     }
 
     {
         // CNOT, target commute with X
-        QuantumState state(n, true), test_state(n, true);
-        state.set_Haar_random_state();
-        test_state.load(&state);
-        QuantumCircuit circuit(n);
+        int ngpus = get_num_device();
+        for (int idx = 0; idx < ngpus; ++idx) {
+            set_device(idx);
+
+            QuantumStateGpu state(n, idx), test_state(n, idx);
+            state.set_Haar_random_state();
+            test_state.load(&state);
+            QuantumCircuit circuit(n);
+
+            circuit.add_Z_gate(1);
+            circuit.add_CNOT_gate(0, 1);
+            circuit.add_Z_gate(1);
+            UINT block_size = 2;
+            UINT expected_depth = 1;
+            UINT expected_gate_count = 1;
 
-        circuit.add_Z_gate(1);
-        circuit.add_CNOT_gate(0, 1);
-        circuit.add_Z_gate(1);
-        UINT block_size = 2;
-        UINT expected_depth = 1;
-        UINT expected_gate_count = 1;
-
-        QuantumCircuit* copy_circuit = circuit.copy();
-        QuantumCircuitOptimizer qco;
-        qco.optimize(copy_circuit, block_size);
-        circuit.update_quantum_state(&test_state);
-        copy_circuit->update_quantum_state(&state);
-        ASSERT_STATE_NEAR(state, test_state, eps);
-        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-        delete copy_circuit;
+            QuantumCircuit* copy_circuit = circuit.copy();
+            QuantumCircuitOptimizer qco;
+            qco.optimize(copy_circuit, block_size);
+            circuit.update_quantum_state(&test_state);
+            copy_circuit->update_quantum_state(&state);
+            // std::cout << circuit << std::endl << copy_circuit << std::endl;
+            assert_gpu_eq_gpu(state, test_state, dim, eps);
+            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+            delete copy_circuit;
+        }
     }
 
     {
         // CNOT, target commute with X
-        QuantumState state(n, true), test_state(n, true);
-        state.set_Haar_random_state();
-        test_state.load(&state);
-        QuantumCircuit circuit(n);
+        int ngpus = get_num_device();
+        for (int idx = 0; idx < ngpus; ++idx) {
+            set_device(idx);
+
+            QuantumStateGpu state(n, idx), test_state(n, idx);
+            state.set_Haar_random_state();
+            test_state.load(&state);
+            QuantumCircuit circuit(n);
+
+            circuit.add_Z_gate(0);
+            circuit.add_gate(gate::merge(gate::CNOT(0, 1), gate::Y(2)));
+            circuit.add_gate(gate::merge(gate::CNOT(1, 0), gate::Y(2)));
+            circuit.add_Z_gate(1);
+            UINT block_size = 2;
+            UINT expected_depth = 3;
+            UINT expected_gate_count = 3;
 
-        auto gate1 = gate::CNOT(0, 1);
-        auto gate2 = gate::CNOT(1, 2);
-        auto gate3 = gate::Y(2);
-
-        circuit.add_Z_gate(0);
-        circuit.add_gate(gate::merge(gate1, gate3));
-        circuit.add_gate(gate::merge(gate2, gate3));
-        circuit.add_Z_gate(1);
-
-        delete gate1;
-        delete gate2;
-        delete gate3;
-
-        UINT block_size = 2;
-        UINT expected_depth = 3;
-        UINT expected_gate_count = 3;
-
-        QuantumCircuit* copy_circuit = circuit.copy();
-        QuantumCircuitOptimizer qco;
-        qco.optimize(copy_circuit, block_size);
-        circuit.update_quantum_state(&test_state);
-        copy_circuit->update_quantum_state(&state);
-        ASSERT_STATE_NEAR(state, test_state, eps);
-        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-        delete copy_circuit;
+            QuantumCircuit* copy_circuit = circuit.copy();
+            QuantumCircuitOptimizer qco;
+            qco.optimize(copy_circuit, block_size);
+            circuit.update_quantum_state(&test_state);
+            copy_circuit->update_quantum_state(&state);
+            // std::cout << circuit << std::endl << copy_circuit << std::endl;
+            assert_gpu_eq_gpu(state, test_state, dim, eps);
+            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+            delete copy_circuit;
+        }
     }
 
     {
         // CNOT, target commute with X
-        QuantumState state(n, true), test_state(n, true);
-        state.set_Haar_random_state();
-        test_state.load(&state);
-        QuantumCircuit circuit(n);
+        int ngpus = get_num_device();
+        for (int idx = 0; idx < ngpus; ++idx) {
+            set_device(idx);
+
+            QuantumStateGpu state(n, idx), test_state(n, idx);
+            state.set_Haar_random_state();
+            test_state.load(&state);
+            QuantumCircuit circuit(n);
+
+            circuit.add_Z_gate(0);
+            circuit.add_gate(gate::merge(gate::CNOT(0, 1), gate::Y(2)));
+            circuit.add_gate(gate::merge(gate::CNOT(1, 0), gate::Y(2)));
+            circuit.add_Z_gate(1);
+            UINT block_size = 3;
+            UINT expected_depth = 1;
+            UINT expected_gate_count = 1;
 
-        auto gate1 = gate::CNOT(0, 1);
-        auto gate2 = gate::CNOT(1, 2);
-        auto gate3 = gate::Y(2);
-
-        circuit.add_Z_gate(0);
-        circuit.add_gate(gate::merge(gate1, gate3));
-        circuit.add_gate(gate::merge(gate2, gate3));
-        circuit.add_Z_gate(1);
-
-        delete gate1;
-        delete gate2;
-        delete gate3;
-
-        UINT block_size = 3;
-        UINT expected_depth = 1;
-        UINT expected_gate_count = 1;
-
-        QuantumCircuit* copy_circuit = circuit.copy();
-        QuantumCircuitOptimizer qco;
-        qco.optimize(copy_circuit, block_size);
-        circuit.update_quantum_state(&test_state);
-        copy_circuit->update_quantum_state(&state);
-        ASSERT_STATE_NEAR(state, test_state, eps);
-        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-        delete copy_circuit;
-    }
-}
-
-TEST(CircuitTest_multicpu, RandomCircuitOptimize) {
-    const UINT n = 5;
-    const UINT dim = 1ULL << n;
-    const UINT depth = 5;
-    Random random;
-    random.set_seed(2022);
-
-    UINT max_repeat = 3;
-    // UINT max_block_size = n;
-    UINT max_block_size = 1;  // TODO: multi-cpu limitation.
-
-    for (UINT repeat = 0; repeat < max_repeat; ++repeat) {
-        QuantumState state(n, true), org_state(n, true), test_state(n, true);
-        state.set_Haar_random_state();
-        org_state.load(&state);
-        QuantumCircuit circuit(n);
-
-        for (UINT d = 0; d < depth; ++d) {
-            for (UINT i = 0; i < n; ++i) {
-                UINT r = random.int32() % 5;
-                if (r == 0)
-                    circuit.add_sqrtX_gate(i);
-                else if (r == 1)
-                    circuit.add_sqrtY_gate(i);
-                else if (r == 2)
-                    circuit.add_T_gate(i);
-                else if (r == 3) {
-                    if (i + 1 < n) circuit.add_CNOT_gate(i, i + 1);
-                } else if (r == 4) {
-                    if (i + 1 < n) circuit.add_CZ_gate(i, i + 1);
-                }
-            }
-        }
-
-        test_state.load(&org_state);
-        circuit.update_quantum_state(&test_state);
-        QuantumCircuitOptimizer qco;
-        for (UINT block_size = 1; block_size <= max_block_size; ++block_size) {
             QuantumCircuit* copy_circuit = circuit.copy();
+            QuantumCircuitOptimizer qco;
             qco.optimize(copy_circuit, block_size);
-            state.load(&org_state);
+            circuit.update_quantum_state(&test_state);
             copy_circuit->update_quantum_state(&state);
-            ASSERT_STATE_NEAR(state, test_state, eps);
+            // std::cout << circuit << std::endl << copy_circuit << std::endl;
+            assert_gpu_eq_gpu(state, test_state, dim, eps);
+            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
             delete copy_circuit;
         }
     }
 }
 
-TEST(CircuitTest_multicpu, RandomCircuitOptimize2) {
+TEST(CircuitTest, RandomCircuitOptimize) {
     const UINT n = 5;
     const UINT dim = 1ULL << n;
-    const UINT depth = 10;
+    const UINT depth = 5;
     Random random;
-    random.set_seed(2022);
 
     UINT max_repeat = 3;
-    // UINT max_block_size = n;
-    UINT max_block_size = 1;  // TODO: multi-cpu limitation.
+    UINT max_block_size = n;
 
-    for (UINT repeat = 0; repeat < max_repeat; ++repeat) {
-        QuantumState state(n, true), org_state(n, true), test_state(n, true);
-        state.set_Haar_random_state();
-        org_state.load(&state);
-        QuantumCircuit circuit(n);
-
-        for (UINT d = 0; d < depth; ++d) {
-            for (UINT i = 0; i < n; ++i) {
-                UINT r = random.int32() % 6;
-                if (r == 0)
-                    circuit.add_sqrtX_gate(i);
-                else if (r == 1)
-                    circuit.add_sqrtY_gate(i);
-                else if (r == 2)
-                    circuit.add_T_gate(i);
-                else if (r == 3) {
-                    UINT r2 = random.int32() % n;
-                    if (r2 == i) r2 = (r2 + 1) % n;
-                    if (i + 1 < n) circuit.add_CNOT_gate(i, r2);
-                } else if (r == 4) {
-                    UINT r2 = random.int32() % n;
-                    if (r2 == i) r2 = (r2 + 1) % n;
-                    if (i + 1 < n) circuit.add_CZ_gate(i, r2);
-                } else if (r == 5) {
-                    UINT r2 = random.int32() % n;
-                    if (r2 == i) r2 = (r2 + 1) % n;
-                    if (i + 1 < n) circuit.add_SWAP_gate(i, r2);
+    int ngpus = get_num_device();
+    for (int idx = 0; idx < ngpus; ++idx) {
+        set_device(idx);
+        for (UINT repeat = 0; repeat < max_repeat; ++repeat) {
+            QuantumStateGpu state(n, idx), org_state(n, idx),
+                test_state(n, idx);
+            state.set_Haar_random_state();
+            org_state.load(&state);
+            QuantumCircuit circuit(n);
+
+            for (UINT d = 0; d < depth; ++d) {
+                for (UINT i = 0; i < n; ++i) {
+                    UINT r = random.int32() % 5;
+                    if (r == 0)
+                        circuit.add_sqrtX_gate(i);
+                    else if (r == 1)
+                        circuit.add_sqrtY_gate(i);
+                    else if (r == 2)
+                        circuit.add_T_gate(i);
+                    else if (r == 3) {
+                        if (i + 1 < n) circuit.add_CNOT_gate(i, i + 1);
+                    } else if (r == 4) {
+                        if (i + 1 < n) circuit.add_CZ_gate(i, i + 1);
+                    }
                 }
             }
-        }
 
-        test_state.load(&org_state);
-        circuit.update_quantum_state(&test_state);
-        QuantumCircuitOptimizer qco;
-        for (UINT block_size = 1; block_size <= max_block_size; ++block_size) {
-            QuantumCircuit* copy_circuit = circuit.copy();
-            qco.optimize(copy_circuit, block_size);
-            state.load(&org_state);
-            copy_circuit->update_quantum_state(&state);
-            ASSERT_STATE_NEAR(state, test_state, eps);
-            delete copy_circuit;
+            test_state.load(&org_state);
+            circuit.update_quantum_state(&test_state);
+            // std::cout << circuit << std::endl;
+            QuantumCircuitOptimizer qco;
+            for (UINT block_size = 1; block_size <= max_block_size;
+                 ++block_size) {
+                QuantumCircuit* copy_circuit = circuit.copy();
+                qco.optimize(copy_circuit, block_size);
+                state.load(&org_state);
+                copy_circuit->update_quantum_state(&state);
+                // std::cout << copy_circuit << std::endl;
+                assert_gpu_eq_gpu(state, test_state, dim, eps);
+                delete copy_circuit;
+            }
         }
     }
 }
 
-TEST(CircuitTest_multicpu, RandomCircuitOptimize3) {
+TEST(CircuitTest, RandomCircuitOptimizeLarge) {
     const UINT n = 5;
     const UINT dim = 1ULL << n;
-    const UINT depth = 10 * n;
+    const UINT depth = 5;
     Random random;
-    random.set_seed(2022);
-    MPIutil& mpiutil = MPIutil::get_inst();
-    UINT mpirank = mpiutil.get_rank();
-    UINT mpisize = mpiutil.get_size();
 
     UINT max_repeat = 3;
-    // UINT max_block_size = n;
-    UINT max_block_size = 1;  // TODO: multi-cpu limitation.
-    UINT seed = 2021;
-    std::mt19937 eng(seed);
-
-    std::vector<UINT> qubit_list;
-    for (int i = 0; i < n; ++i) qubit_list.push_back(i);
-
-    for (UINT repeat = 0; repeat < max_repeat; ++repeat) {
-        QuantumState state(n, true), org_state(n, true), test_state(n, true);
-        state.set_Haar_random_state(2000);
-        org_state.load(&state);
-        QuantumCircuit circuit(n);
-
-        for (UINT d = 0; d < depth; ++d) {
-            std::shuffle(qubit_list.begin(), qubit_list.end(), eng);
-            std::vector<UINT> mylist;
-            mylist.push_back(qubit_list[0]);
-            mylist.push_back(qubit_list[1]);
-            circuit.add_random_unitary_gate(mylist, seed + d);
-            // circuit.add_CNOT_gate(qubit_list[0], qubit_list[1]);
-        }
+    UINT max_block_size = n;
+    int ngpus = get_num_device();
+    for (int idx = 0; idx < ngpus; ++idx) {
+        set_device(idx);
+        for (UINT repeat = 0; repeat < max_repeat; ++repeat) {
+            QuantumStateGpu state(n, idx), org_state(n, idx),
+                test_state(n, idx);
+            state.set_Haar_random_state();
+            org_state.load(&state);
+            QuantumCircuit circuit(n);
+
+            for (UINT d = 0; d < depth; ++d) {
+                for (UINT i = 0; i < n; ++i) {
+                    UINT r = random.int32() % 5;
+                    if (r == 0)
+                        circuit.add_sqrtX_gate(i);
+                    else if (r == 1)
+                        circuit.add_sqrtY_gate(i);
+                    else if (r == 2)
+                        circuit.add_T_gate(i);
+                    else if (r == 3) {
+                        if (i + 1 < n) circuit.add_CNOT_gate(i, i + 1);
+                    } else if (r == 4) {
+                        if (i + 1 < n) circuit.add_CZ_gate(i, i + 1);
+                    }
+                }
+            }
 
-        test_state.load(&org_state);
-        circuit.update_quantum_state(&test_state);
-        // std::cout << "#original-circuit " << mpirank << ":" << circuit <<
-        // std::endl; std::cout << "# test_state" << mpirank << ": " <<
-        // test_state << std::endl;
-        QuantumCircuitOptimizer qco;
-        for (UINT block_size = 1; block_size <= max_block_size; ++block_size) {
-            QuantumCircuit* copy_circuit = circuit.copy();
-            qco.optimize(copy_circuit, block_size);
-            state.load(&org_state);
-            copy_circuit->update_quantum_state(&state);
-            // std::cout << "#optimized-circuit " << mpirank << ":" <<
-            // block_size << ", " << circuit << std::endl; std::cout << "#
-            // state" << mpirank << ": " << state << std::endl;
-            ASSERT_STATE_NEAR(state, test_state, eps);
-            delete copy_circuit;
+            test_state.load(&org_state);
+            circuit.update_quantum_state(&test_state);
+            // std::cout << circuit << std::endl;
+            QuantumCircuitOptimizer qco;
+            for (UINT block_size = 1; block_size <= max_block_size;
+                 ++block_size) {
+                QuantumCircuit* copy_circuit = circuit.copy();
+                qco.optimize(copy_circuit, block_size);
+                state.load(&org_state);
+                copy_circuit->update_quantum_state(&state);
+                // std::cout << copy_circuit << std::endl;
+                assert_gpu_eq_gpu(state, test_state, dim, eps);
+                delete copy_circuit;
+            }
         }
     }
 }
 
-TEST(CircuitTest_multicpu, SuzukiTrotterExpansion) {
+TEST(CircuitTest, SuzukiTrotterExpansion) {
     CPPCTYPE J(0.0, 1.0);
-    const auto Identity = make_Identity();
-    const auto X = make_X();
-    const auto Y = make_Y();
-    const auto Z = make_Z();
+    Eigen::MatrixXcd Identity(2, 2), X(2, 2), Y(2, 2), Z(2, 2);
+    Identity << 1, 0, 0, 1;
+    X << 0, 1, 1, 0;
+    Y << 0, -J, J, 0;
+    Z << 1, 0, 0, -1;
 
     const UINT n = 2;
+    UINT num_repeats;
     const UINT dim = 1ULL << n;
 
     double angle;
     std::vector<double> coef;
 
     const UINT seed = 1918;
     Random random;
     random.set_seed(seed);
 
-    CPPCTYPE res;
+    double res;
     CPPCTYPE test_res;
 
-    Observable diag_observable(n), non_diag_observable(n), observable(n);
-    Eigen::MatrixXcd test_observable;
+    int ngpus = get_num_device();
+    for (int idx = 0; idx < ngpus; ++idx) {
+        Observable diag_observable(n), non_diag_observable(n), observable(n);
+        Eigen::MatrixXcd test_observable;
+
+        QuantumStateGpu state(n, idx);
+        Eigen::VectorXcd test_state = Eigen::VectorXcd::Zero(dim);
 
-    QuantumState state(n, true);
-    Eigen::VectorXcd test_state = Eigen::VectorXcd::Zero(dim);
+        QuantumCircuit circuit(n);
+        Eigen::MatrixXcd test_circuit;
 
-    QuantumCircuit circuit(n);
-    Eigen::MatrixXcd test_circuit;
+        for (ITYPE i = 0; i < 6; ++i) {
+            coef.push_back(-random.uniform());
+            // coef.push_back(-1.);
+        }
+        angle = 2 * PI * random.uniform();
 
-    for (ITYPE i = 0; i < 6; ++i) {
-        coef.push_back(-random.uniform());
-        // coef.push_back(-1.);
-    }
-    angle = 2 * PI * random.uniform();
-
-    observable.add_operator(coef[0], "Z 0 I 1");
-    observable.add_operator(coef[1], "X 0 Y 1");
-    observable.add_operator(coef[2], "Z 0 Z 1");
-    observable.add_operator(coef[3], "Z 0 X 1");
-    observable.add_operator(coef[4], "Y 0 X 1");
-    observable.add_operator(coef[5], "I 0 Z 1");
-
-    test_observable =
-        coef[0] * get_expanded_eigen_matrix_with_identity(0, Z, n);
-    test_observable += coef[1] * kronecker_product(Y, X);
-    test_observable += coef[2] * kronecker_product(Z, Z);
-    test_observable += coef[3] * kronecker_product(X, Z);
-    test_observable += coef[4] * kronecker_product(X, Y);
-    test_observable +=
-        coef[5] * get_expanded_eigen_matrix_with_identity(1, Z, n);
-
-    const auto num_repeats =
-        static_cast<UINT>(std::ceil(angle * (double)n * 100.));
-    // circuit.add_diagonal_observable_rotation_gate(diag_observable, angle);
-    circuit.add_observable_rotation_gate(observable, angle, num_repeats);
-
-    test_circuit = J * angle * test_observable;
-    test_circuit = test_circuit.exp();
-
-    state.set_computational_basis(0);
-    test_state(0) = 1.;
-
-    res = observable.get_expectation_value(&state);
-    test_res = (test_state.adjoint() * test_observable * test_state)(0, 0);
-
-    circuit.update_quantum_state(&state);
-    test_state = test_circuit * test_state;
-
-    res = observable.get_expectation_value(&state);
-    test_res = (test_state.adjoint() * test_observable * test_state)(0, 0);
-    ASSERT_NEAR(abs(test_res.real() - res.real()) / test_res.real(), 0, 0.01);
-
-    state.set_Haar_random_state(seed);
-    for (ITYPE i = 0; i < dim; ++i) test_state[i] = state.data_cpp()[i];
-
-    test_state = test_circuit * test_state;
-    circuit.update_quantum_state(&state);
-
-    res = observable.get_expectation_value(&state);
-    test_res = (test_state.adjoint() * test_observable * test_state)(0, 0);
-    ASSERT_NEAR(abs(test_res.real() - res.real()) / test_res.real(), 0, 0.01);
+        observable.add_operator(coef[0], "Z 0 I 1");
+        observable.add_operator(coef[1], "X 0 Y 1");
+        observable.add_operator(coef[2], "Z 0 Z 1");
+        observable.add_operator(coef[3], "Z 0 X 1");
+        observable.add_operator(coef[4], "Y 0 X 1");
+        observable.add_operator(coef[5], "I 0 Z 1");
+
+        test_observable =
+            coef[0] * get_expanded_eigen_matrix_with_identity(0, Z, n);
+        test_observable += coef[1] * kronecker_product(Y, X);
+        test_observable += coef[2] * kronecker_product(Z, Z);
+        test_observable += coef[3] * kronecker_product(X, Z);
+        test_observable += coef[4] * kronecker_product(X, Y);
+        test_observable +=
+            coef[5] * get_expanded_eigen_matrix_with_identity(1, Z, n);
+
+        num_repeats = (UINT)std::ceil(angle * (double)n * 100.);
+        // circuit.add_diagonal_observable_rotation_gate(diag_observable,
+        // angle);
+        circuit.add_observable_rotation_gate(observable, angle, num_repeats);
+
+        test_circuit = J * angle * test_observable;
+        test_circuit = test_circuit.exp();
+
+        state.set_computational_basis(0);
+        test_state(0) = 1.;
+
+        res = observable.get_expectation_value(&state).real();
+        test_res = (test_state.adjoint() * test_observable * test_state);
+
+        circuit.update_quantum_state(&state);
+        test_state = test_circuit * test_state;
+
+        res = observable.get_expectation_value(&state).real();
+        test_res = (test_state.adjoint() * test_observable * test_state);
+        ASSERT_NEAR(abs(test_res.real() - res) / res, 0, 0.01);
+
+        state.set_Haar_random_state(seed);
+        set_eigen_from_gpu(test_state, state, dim);
+
+        test_state = test_circuit * test_state;
+        circuit.update_quantum_state(&state);
+
+        res = observable.get_expectation_value(&state).real();
+        test_res = (test_state.adjoint() * test_observable * test_state);
+        ASSERT_NEAR(abs(test_res.real() - res) / res, 0, 0.01);
+    }
 }
 
-TEST(CircuitTest_multicpu, RotateDiagonalObservable) {
+TEST(CircuitTest, RotateDiagonalObservable) {
     CPPCTYPE J(0.0, 1.0);
-    const auto Identity = make_Identity();
-    const auto X = make_X();
-    const auto Y = make_Y();
-    const auto Z = make_Z();
+    Eigen::MatrixXcd Identity(2, 2), X(2, 2), Y(2, 2), Z(2, 2);
+    Identity << 1, 0, 0, 1;
+    X << 0, 1, 1, 0;
+    Y << 0, -J, J, 0;
+    Z << 1, 0, 0, -1;
 
     const UINT n = 2;
     const UINT dim = 1ULL << n;
 
     double angle, coef1, coef2;
     Random random;
-    random.set_seed(2022);
 
-    CPPCTYPE res;
+    double res;
     CPPCTYPE test_res;
 
-    Observable observable(n);
-    Eigen::MatrixXcd test_observable;
+    int ngpus = get_num_device();
+    for (int idx = 0; idx < ngpus; ++idx) {
+        Observable observable(n);
+        Eigen::MatrixXcd test_observable;
 
-    QuantumState state(n, true);
-    Eigen::VectorXcd test_state = Eigen::VectorXcd::Zero(dim);
+        QuantumStateGpu state(n, idx);
+        Eigen::VectorXcd test_state = Eigen::VectorXcd::Zero(dim);
 
-    QuantumCircuit circuit(n);
-    Eigen::MatrixXcd test_circuit;
+        QuantumCircuit circuit(n);
+        Eigen::MatrixXcd test_circuit;
 
-    coef1 = -random.uniform();
-    coef2 = -random.uniform();
-    angle = 2 * PI * random.uniform();
+        coef1 = -random.uniform();
+        coef2 = -random.uniform();
+        angle = 2 * PI * random.uniform();
 
-    observable.add_operator(coef1, "Z 0");
-    observable.add_operator(coef2, "Z 0 Z 1");
+        observable.add_operator(coef1, "Z 0");
+        observable.add_operator(coef2, "Z 0 Z 1");
 
-    test_observable = coef1 * get_expanded_eigen_matrix_with_identity(0, Z, n);
-    test_observable += coef2 * kronecker_product(Z, Z);
+        test_observable =
+            coef1 * get_expanded_eigen_matrix_with_identity(0, Z, n);
+        test_observable += coef2 * kronecker_product(Z, Z);
 
-    circuit.add_diagonal_observable_rotation_gate(observable, angle);
-    test_circuit = (J * angle * test_observable).exp();
+        circuit.add_diagonal_observable_rotation_gate(observable, angle);
+        test_circuit = (J * angle * test_observable).exp();
 
-    state.set_computational_basis(0);
-    test_state(0) = 1.;
+        state.set_computational_basis(0);
+        test_state(0) = 1.;
 
-    circuit.update_quantum_state(&state);
-    test_state = test_circuit * test_state;
+        // for (ITYPE i = 0; i < dim; ++i) ASSERT_NEAR(abs(test_state[i] -
+        // state.data_cpp()[i]), 0, eps);
 
-    res = observable.get_expectation_value(&state);
-    test_res = (test_state.adjoint() * test_observable * test_state)(0, 0);
+        circuit.update_quantum_state(&state);
+        test_state = test_circuit * test_state;
 
-    ASSERT_NEAR(res.imag(), 0, eps);
-    ASSERT_NEAR(test_res.imag(), 0, eps);
+        res = observable.get_expectation_value(&state).real();
+        test_res = (test_state.adjoint() * test_observable * test_state);
 
-    state.set_Haar_random_state();
-    for (ITYPE i = 0; i < dim; ++i) test_state[i] = state.data_cpp()[i];
+        // for (ITYPE i = 0; i < dim; ++i) ASSERT_NEAR(abs(test_state[i] -
+        // state.data_cpp()[i]), 0, eps);
+        ASSERT_NEAR(abs(test_res.real() - res) / test_res.real(), 0, 0.01);
+        ASSERT_NEAR(test_res.imag(), 0, eps);
 
-    res = observable.get_expectation_value(&state);
-    test_res = (test_state.adjoint() * test_observable * test_state)(0, 0);
+        state.set_Haar_random_state();
+        set_eigen_from_gpu(test_state, state, dim);
 
-    test_state = test_circuit * test_state;
-    circuit.update_quantum_state(&state);
+        res = observable.get_expectation_value(&state).real();
+        test_res = (test_state.adjoint() * test_observable * test_state);
 
-    res = observable.get_expectation_value(&state);
-    test_res = (test_state.adjoint() * test_observable * test_state)(0, 0);
+        test_state = test_circuit * test_state;
+        circuit.update_quantum_state(&state);
 
-    ASSERT_NEAR(abs(test_res.real() - res.real()) / test_res.real(), 0, 0.01);
-    ASSERT_NEAR(res.imag(), 0, eps);
-    ASSERT_NEAR(test_res.imag(), 0, eps);
-}
+        res = observable.get_expectation_value(&state).real();
+        test_res = (test_state.adjoint() * test_observable * test_state);
 
-TEST(CircuitTest_multicpu, SpecialGatesToString) {
-    QuantumState state(1, true);
-    QuantumCircuit c(1);
-    c.add_gate(gate::DepolarizingNoise(0, 0));
-    c.update_quantum_state(&state);
-    std::string s = c.to_string();
+        // for (ITYPE i = 0; i < dim; ++i) ASSERT_NEAR(abs(test_state[i] -
+        // state.data_cpp()[i]), 0, eps);
+        ASSERT_NEAR(abs(test_res.real() - res) / test_res.real(), 0, 0.01);
+        ASSERT_NEAR(test_res.imag(), 0, eps);
+    }
 }
 
-TEST(CircuitTest_multicpu, MergeCircuits) {
-    QuantumState state(2, true);
-    QuantumCircuit circuit1(2), circuit2(2);
-    circuit1.add_X_gate(0);
-    circuit2.add_X_gate(1);
-    state.set_zero_state();
-    circuit1.merge_circuit(&circuit2);
-    circuit1.update_quantum_state(&state);
-    ASSERT_NEAR(abs(state.data_cpp()[3]), 1.0, 0.0001);
+TEST(CircuitTest, SpecialGatesToString) {
+    int ngpus = get_num_device();
+    for (int idx = 0; idx < ngpus; ++idx) {
+        set_device(idx);
+        QuantumStateGpu state(1, idx);
+        QuantumCircuit c(1);
+        c.add_gate(gate::DepolarizingNoise(0, 0));
+        c.update_quantum_state(&state);
+        std::string s = c.to_string();
+    }
 }
-#endif
```

### Comparing `qulacs-0.6.2/test/cppsim/test_circuit_optimize_light.cpp` & `qulacs-0.6.3/test/cppsim/test_circuit_optimize_light.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/cppsim/test_gate.cpp` & `qulacs-0.6.3/test/cppsim/test_gate.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1477,16 +1477,16 @@
         for (UINT i = 0; i < qubit_count; ++i) {
             target_qubit_list.push_back(i);
         }
         auto gate = gate::RandomUnitary(target_qubit_list);
         ComplexMatrix cm;
         gate->set_matrix(cm);
         auto eye = cm * cm.adjoint();
-        for (int i = 0; i < dim; ++i) {
-            for (int j = 0; j < dim; ++j) {
+        for (ITYPE i = 0; i < dim; ++i) {
+            for (ITYPE j = 0; j < dim; ++j) {
                 if (i == j) {
                     ASSERT_NEAR(abs(eye(i, j)), 1, eps);
                 } else {
                     ASSERT_NEAR(abs(eye(i, j)), 0, eps);
                 }
             }
         }
```

### Comparing `qulacs-0.6.2/test/cppsim/test_gate_dm.cpp` & `qulacs-0.6.3/test/cppsim/test_gate_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/cppsim/test_gate_multicpu.cpp` & `qulacs-0.6.3/test/cppsim/test_gate_multicpu.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1435,16 +1435,16 @@
         for (UINT i = 0; i < qubit_count; ++i) {
             target_qubit_list.push_back(i);
         }
         auto gate = gate::RandomUnitary(target_qubit_list);
         ComplexMatrix cm;
         gate->set_matrix(cm);
         auto eye = cm * cm.adjoint();
-        for (int i = 0; i < dim; ++i) {
-            for (int j = 0; j < dim; ++j) {
+        for (ITYPE i = 0; i < dim; ++i) {
+            for (ITYPE j = 0; j < dim; ++j) {
                 if (i == j) {
                     ASSERT_NEAR(abs(eye(i, j)), 1, eps);
                 } else {
                     ASSERT_NEAR(abs(eye(i, j)), 0, eps);
                 }
             }
         }
```

### Comparing `qulacs-0.6.2/test/cppsim/test_hamiltonian.cpp` & `qulacs-0.6.3/test/cppsim/test_hamiltonian.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/cppsim/test_hamiltonian_dm.cpp` & `qulacs-0.6.3/test/cppsim/test_hamiltonian_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/cppsim/test_hamiltonian_multicpu.cpp` & `qulacs-0.6.3/test/cppsim/test_hamiltonian_multicpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/cppsim/test_mpiutil_multicpu.cpp` & `qulacs-0.6.3/test/cppsim/test_mpiutil_multicpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/cppsim/test_noise_dm.cpp` & `qulacs-0.6.3/test/cppsim/test_noise_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/cppsim/test_noisesimulator.cpp` & `qulacs-0.6.3/test/cppsim/test_noisesimulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/cppsim/test_noisyevolution.cpp` & `qulacs-0.6.3/test/cppsim/test_noisyevolution.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/cppsim/test_pauli_operator.cpp` & `qulacs-0.6.3/test/cppsim/test_pauli_operator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/cppsim/test_simulator.cpp` & `qulacs-0.6.3/test/cppsim/test_simulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/cppsim/test_state.cpp` & `qulacs-0.6.3/test/cppsim/test_state.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/cppsim/test_state_dm.cpp` & `qulacs-0.6.3/test/cppsim/test_state_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/cppsim/test_state_multicpu.cpp` & `qulacs-0.6.3/test/cppsim/test_state_multicpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/csim/test_memory.cpp` & `qulacs-0.6.3/test/csim/test_memory.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/csim/test_omputil.cpp` & `qulacs-0.6.3/test/csim/test_omputil.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/csim/test_stat.cpp` & `qulacs-0.6.3/test/csim/test_stat.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/csim/test_update_control.cpp` & `qulacs-0.6.3/test/csim/test_update_control.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/csim/test_update_dense.cpp` & `qulacs-0.6.3/test/csim/test_update_dense.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/csim/test_update_dense_double.cpp` & `qulacs-0.6.3/test/csim/test_update_dense_double.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/csim/test_update_diagonal.cpp` & `qulacs-0.6.3/test/csim/test_update_diagonal.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/csim/test_update_diagonal_multi.cpp` & `qulacs-0.6.3/test/csim/test_update_diagonal_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/csim/test_update_named.cpp` & `qulacs-0.6.3/test/csim/test_update_named.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/csim/test_update_pauli.cpp` & `qulacs-0.6.3/test/csim/test_update_pauli.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/gpusim/test_circuit.cpp` & `qulacs-0.6.3/test/cppsim/test_circuit_multicpu.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -1,924 +1,1651 @@
+#ifdef _USE_MPI
 #include <gtest/gtest.h>
 
-#include <cppsim/state_gpu.hpp>
-#include <cppsim/type.hpp>
-#include <csim/constant.hpp>
-
-#include "../util/util.hpp"
-// #define _USE_MATH_DEFINES
-// #include <cmath>
 #include <cppsim/circuit.hpp>
 #include <cppsim/circuit_optimizer.hpp>
 #include <cppsim/gate_factory.hpp>
 #include <cppsim/gate_matrix.hpp>
 #include <cppsim/gate_merge.hpp>
 #include <cppsim/observable.hpp>
 #include <cppsim/pauli_operator.hpp>
 #include <cppsim/state.hpp>
+#include <cppsim/type.hpp>
 #include <cppsim/utility.hpp>
+#include <csim/constant.hpp>
 #include <unsupported/Eigen/MatrixFunctions>
 #include <utility>
 
-inline void set_eigen_from_gpu(
-    ComplexVector& dst, QuantumStateGpu& src, ITYPE dim) {
-    auto ptr = src.duplicate_data_cpp();
-    for (ITYPE i = 0; i < dim; ++i) dst[i] = ptr[i];
-    free(ptr);
-}
-
-inline void assert_eigen_eq_gpu(
-    ComplexVector& v1, QuantumStateGpu& v2, ITYPE dim, double eps) {
-    auto ptr = v2.duplicate_data_cpp();
-    for (UINT i = 0; i < dim; ++i) {
-        ASSERT_NEAR(ptr[i].real(), v1[i].real(), eps);
-        ASSERT_NEAR(ptr[i].imag(), v1[i].imag(), eps);
-    }
-    free(ptr);
-}
-
-inline void assert_cpu_eq_gpu(QuantumStateCpu& state_cpu,
-    QuantumStateGpu& state_gpu, ITYPE dim, double eps) {
-    auto gpu_state_vector = state_gpu.duplicate_data_cpp();
-    for (ITYPE i = 0; i < dim; ++i) {
-        ASSERT_NEAR(
-            state_cpu.data_cpp()[i].real(), gpu_state_vector[i].real(), eps);
-        ASSERT_NEAR(
-            state_cpu.data_cpp()[i].imag(), gpu_state_vector[i].imag(), eps);
-    }
-    free(gpu_state_vector);
-}
-
-inline void assert_gpu_eq_gpu(QuantumStateGpu& state_gpu1,
-    QuantumStateGpu& state_gpu2, ITYPE dim, double eps) {
-    auto gpu_state_vector1 = state_gpu1.duplicate_data_cpp();
-    auto gpu_state_vector2 = state_gpu2.duplicate_data_cpp();
-    for (ITYPE i = 0; i < dim; ++i) {
-        ASSERT_NEAR(
-            gpu_state_vector1[i].real(), gpu_state_vector2[i].real(), eps);
-        ASSERT_NEAR(
-            gpu_state_vector1[i].imag(), gpu_state_vector2[i].imag(), eps);
-    }
-    free(gpu_state_vector1);
-    free(gpu_state_vector2);
-}
-
-TEST(CircuitTest, CircuitBasic) {
-    Eigen::MatrixXcd Identity(2, 2), X(2, 2), Y(2, 2), Z(2, 2), H(2, 2),
-        S(2, 2), T(2, 2), sqrtX(2, 2), sqrtY(2, 2), P0(2, 2), P1(2, 2);
-
-    Identity << 1, 0, 0, 1;
-    X << 0, 1, 1, 0;
-    Y << 0, -1.i, 1.i, 0;
-    Z << 1, 0, 0, -1;
-    H << 1, 1, 1, -1;
-    H /= sqrt(2.);
-    S << 1, 0, 0, 1.i;
-    T << 1, 0, 0, (1. + 1.i) / sqrt(2.);
-    sqrtX << 0.5 + 0.5i, 0.5 - 0.5i, 0.5 - 0.5i, 0.5 + 0.5i;
-    sqrtY << 0.5 + 0.5i, -0.5 - 0.5i, 0.5 + 0.5i, 0.5 + 0.5i;
-    P0 << 1, 0, 0, 0;
-    P1 << 0, 0, 0, 1;
+#include "../util/util.hpp"
+
+TEST(CircuitTest_multicpu, CircuitBasic) {
+    const auto Identity = make_Identity();
+    const auto X = make_X();
+    const auto Y = make_Y();
+    const auto Z = make_Z();
+    const auto H = make_H();
+    const auto S = make_S();
+    const auto T = make_T();
+    const auto sqrtX = make_sqrtX();
+    const auto sqrtY = make_sqrtY();
+    const auto P0 = make_P0();
+    const auto P1 = make_P1();
 
     const UINT n = 4;
-    const UINT dim = 1ULL << n;
+    UINT dim = 1ULL << n;
+    MPIutil& mpiutil = MPIutil::get_inst();
+    UINT mpirank = mpiutil.get_rank();
+    UINT mpisize = mpiutil.get_size();
+    ITYPE inner_dim = dim / mpisize;
+    ITYPE offs = inner_dim * mpirank;
 
     Random random;
-    std::complex<double> imag_unit(0, 1);
+    random.set_seed(2022);
 
-    int ngpus = get_num_device();
-    for (int idx = 0; idx < ngpus; ++idx) {
-        set_device(idx);
-        auto stream_ptr = allocate_cuda_stream_host(1, idx);
-
-        QuantumStateGpu state(n, idx);
-        ComplexVector state_eigen(dim);
-
-        state.set_Haar_random_state();
-        set_eigen_from_gpu(state_eigen, state, dim);
-
-        QuantumCircuit circuit(n);
-        UINT target, target_sub;
-        double angle;
-
-        target = random.int32() % n;
-        circuit.add_X_gate(target);
-        state_eigen = get_expanded_eigen_matrix_with_identity(
-                          target, get_eigen_matrix_single_Pauli(1), n) *
-                      state_eigen;
-
-        target = random.int32() % n;
-        circuit.add_Y_gate(target);
-        state_eigen = get_expanded_eigen_matrix_with_identity(
-                          target, get_eigen_matrix_single_Pauli(2), n) *
-                      state_eigen;
-
-        target = random.int32() % n;
-        circuit.add_Z_gate(target);
-        state_eigen = get_expanded_eigen_matrix_with_identity(
-                          target, get_eigen_matrix_single_Pauli(3), n) *
-                      state_eigen;
-
-        target = random.int32() % n;
-        circuit.add_H_gate(target);
-        state_eigen =
-            get_expanded_eigen_matrix_with_identity(target, H, n) * state_eigen;
-
-        target = random.int32() % n;
-        circuit.add_S_gate(target);
-        state_eigen =
-            get_expanded_eigen_matrix_with_identity(target, S, n) * state_eigen;
-
-        target = random.int32() % n;
-        circuit.add_Sdag_gate(target);
-        state_eigen =
-            get_expanded_eigen_matrix_with_identity(target, S.adjoint(), n) *
-            state_eigen;
-
-        target = random.int32() % n;
-        circuit.add_T_gate(target);
-        state_eigen =
-            get_expanded_eigen_matrix_with_identity(target, T, n) * state_eigen;
-
-        target = random.int32() % n;
-        circuit.add_Tdag_gate(target);
-        state_eigen =
-            get_expanded_eigen_matrix_with_identity(target, T.adjoint(), n) *
-            state_eigen;
-
-        target = random.int32() % n;
-        circuit.add_sqrtX_gate(target);
-        state_eigen =
-            get_expanded_eigen_matrix_with_identity(target, sqrtX, n) *
-            state_eigen;
-
-        target = random.int32() % n;
-        circuit.add_sqrtXdag_gate(target);
-        state_eigen = get_expanded_eigen_matrix_with_identity(
-                          target, sqrtX.adjoint(), n) *
-                      state_eigen;
-
-        target = random.int32() % n;
-        circuit.add_sqrtY_gate(target);
-        state_eigen =
-            get_expanded_eigen_matrix_with_identity(target, sqrtY, n) *
-            state_eigen;
-
-        target = random.int32() % n;
-        circuit.add_sqrtYdag_gate(target);
-        state_eigen = get_expanded_eigen_matrix_with_identity(
-                          target, sqrtY.adjoint(), n) *
-                      state_eigen;
-
-        target = random.int32() % n;
-        circuit.add_P0_gate(target);
-        state_eigen = get_expanded_eigen_matrix_with_identity(target, P0, n) *
-                      state_eigen;
-
-        target = (target + 1) % n;
-        circuit.add_P1_gate(target);
-        state_eigen = get_expanded_eigen_matrix_with_identity(target, P1, n) *
-                      state_eigen;
-
-        target = random.int32() % n;
-        angle = random.uniform() * 3.14159;
-        circuit.add_RotInvX_gate(target, angle);
-        state_eigen =
-            get_expanded_eigen_matrix_with_identity(target,
-                cos(angle / 2) * Identity + 1.i * sin(angle / 2) * X, n) *
-            state_eigen;
-
-        target = random.int32() % n;
-        angle = random.uniform() * 3.14159;
-        circuit.add_RotInvY_gate(target, angle);
-        state_eigen =
-            get_expanded_eigen_matrix_with_identity(target,
-                cos(angle / 2) * Identity + 1.i * sin(angle / 2) * Y, n) *
-            state_eigen;
-
-        target = random.int32() % n;
-        angle = random.uniform() * 3.14159;
-        circuit.add_RotInvZ_gate(target, angle);
-        state_eigen =
-            get_expanded_eigen_matrix_with_identity(target,
-                cos(angle / 2) * Identity + 1.i * sin(angle / 2) * Z, n) *
-            state_eigen;
-
-        target = random.int32() % n;
-        target_sub = random.int32() % (n - 1);
-        if (target_sub >= target) target_sub++;
-        circuit.add_CNOT_gate(target, target_sub);
-        state_eigen = get_eigen_matrix_full_qubit_CNOT(target, target_sub, n) *
-                      state_eigen;
-
-        target = random.int32() % n;
-        target_sub = random.int32() % (n - 1);
-        if (target_sub >= target) target_sub++;
-        circuit.add_CZ_gate(target, target_sub);
-        state_eigen =
-            get_eigen_matrix_full_qubit_CZ(target, target_sub, n) * state_eigen;
-
-        target = random.int32() % n;
-        target_sub = random.int32() % (n - 1);
-        if (target_sub >= target) target_sub++;
-        circuit.add_SWAP_gate(target, target_sub);
-        state_eigen = get_eigen_matrix_full_qubit_SWAP(target, target_sub, n) *
-                      state_eigen;
+    QuantumState state_ref(n, false);
+    QuantumState state(n, true);
+    ComplexVector state_eigen(dim);
+
+    state.set_Haar_random_state();
+    state_ref.load(&state);
+    for (ITYPE i = 0; i < dim; ++i) state_eigen[i] = state_ref.data_cpp()[i];
 
-        circuit.update_quantum_state(&state);
+    QuantumCircuit circuit(n);
+    UINT target, target_sub;
+    double angle;
+    std::complex<double> imag_unit(0, 1);
 
-        assert_eigen_eq_gpu(state_eigen, state, dim, eps);
-    }
+    target = random.int32() % n;
+    circuit.add_X_gate(target);
+    state_eigen = get_expanded_eigen_matrix_with_identity(
+                      target, get_eigen_matrix_single_Pauli(1), n) *
+                  state_eigen;
+
+    target = random.int32() % n;
+    circuit.add_Y_gate(target);
+    state_eigen = get_expanded_eigen_matrix_with_identity(
+                      target, get_eigen_matrix_single_Pauli(2), n) *
+                  state_eigen;
+
+    target = random.int32() % n;
+    circuit.add_Z_gate(target);
+    state_eigen = get_expanded_eigen_matrix_with_identity(
+                      target, get_eigen_matrix_single_Pauli(3), n) *
+                  state_eigen;
+
+    target = random.int32() % n;
+    circuit.add_H_gate(target);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target, H, n) * state_eigen;
+
+    target = random.int32() % n;
+    circuit.add_S_gate(target);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target, S, n) * state_eigen;
+
+    target = random.int32() % n;
+    circuit.add_Sdag_gate(target);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target, S.adjoint(), n) *
+        state_eigen;
+
+    target = random.int32() % n;
+    circuit.add_T_gate(target);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target, T, n) * state_eigen;
+
+    target = random.int32() % n;
+    circuit.add_Tdag_gate(target);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target, T.adjoint(), n) *
+        state_eigen;
+
+    target = random.int32() % n;
+    circuit.add_sqrtX_gate(target);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target, sqrtX, n) * state_eigen;
+
+    target = random.int32() % n;
+    circuit.add_sqrtXdag_gate(target);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target, sqrtX.adjoint(), n) *
+        state_eigen;
+
+    target = random.int32() % n;
+    circuit.add_sqrtY_gate(target);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target, sqrtY, n) * state_eigen;
+
+    target = random.int32() % n;
+    circuit.add_sqrtYdag_gate(target);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target, sqrtY.adjoint(), n) *
+        state_eigen;
+
+    target = random.int32() % n;
+    circuit.add_P0_gate(target);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target, P0, n) * state_eigen;
+
+    target = (target + 1) % n;
+    circuit.add_P1_gate(target);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target, P1, n) * state_eigen;
+
+    target = random.int32() % n;
+    angle = random.uniform() * 3.14159;
+    circuit.add_RX_gate(target, angle);
+    circuit.add_RotInvX_gate(target, angle);
+    circuit.add_RotX_gate(target, angle);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target,
+            cos(angle / 2) * Identity + imag_unit * sin(angle / 2) * X, n) *
+        state_eigen;
+
+    target = random.int32() % n;
+    angle = random.uniform() * 3.14159;
+    circuit.add_RY_gate(target, angle);
+    circuit.add_RotInvY_gate(target, angle);
+    circuit.add_RotY_gate(target, angle);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target,
+            cos(angle / 2) * Identity + imag_unit * sin(angle / 2) * Y, n) *
+        state_eigen;
+
+    target = random.int32() % n;
+    angle = random.uniform() * 3.14159;
+    circuit.add_RZ_gate(target, angle);
+    circuit.add_RotInvZ_gate(target, angle);
+    circuit.add_RotZ_gate(target, angle);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target,
+            cos(angle / 2) * Identity + imag_unit * sin(angle / 2) * Z, n) *
+        state_eigen;
+
+    target = random.int32() % n;
+    target_sub = random.int32() % (n - 1);
+    if (target_sub >= target) target_sub++;
+    circuit.add_CNOT_gate(target, target_sub);
+    state_eigen =
+        get_eigen_matrix_full_qubit_CNOT(target, target_sub, n) * state_eigen;
+
+    target = random.int32() % n;
+    target_sub = random.int32() % (n - 1);
+    if (target_sub >= target) target_sub++;
+    circuit.add_CZ_gate(target, target_sub);
+    state_eigen =
+        get_eigen_matrix_full_qubit_CZ(target, target_sub, n) * state_eigen;
+
+    target = random.int32() % n;
+    target_sub = random.int32() % (n - 1);
+    if (target_sub >= target) target_sub++;
+    circuit.add_SWAP_gate(target, target_sub);
+    state_eigen =
+        get_eigen_matrix_full_qubit_SWAP(target, target_sub, n) * state_eigen;
+
+    target = random.int32() % n;
+    circuit.add_U1_gate(target, M_PI);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target, Z, n) * state_eigen;
+
+    target = random.int32() % n;
+    circuit.add_U2_gate(target, 0, M_PI);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target, H, n) * state_eigen;
+
+    target = random.int32() % n;
+    angle = random.uniform() * 3.14159;
+    circuit.add_U3_gate(target, -angle, 0, 0);
+    state_eigen =
+        get_expanded_eigen_matrix_with_identity(target,
+            cos(angle / 2) * Identity + imag_unit * sin(angle / 2) * Y, n) *
+        state_eigen;
+
+    std::vector<UINT> target_index_list{0, 1, 2, 3};
+    std::vector<UINT> pauli_id_list{0, 1, 2, 3};
+    circuit.add_multi_Pauli_gate(target_index_list, pauli_id_list);
+
+    // add same gate == cancel above pauli gate
+    PauliOperator pauli = PauliOperator("I 0 X 1 Y 2 Z 3");
+    circuit.add_multi_Pauli_gate(pauli);
+
+    ComplexMatrix mat_x(2, 2);
+    target = random.int32() % n;
+    mat_x << 0, 1, 1, 0;
+    circuit.add_dense_matrix_gate(target, mat_x);
+
+    state_eigen = get_expanded_eigen_matrix_with_identity(
+                      target, get_eigen_matrix_single_Pauli(1), n) *
+                  state_eigen;
+
+    circuit.update_quantum_state(&state);
+
+    if (state.get_device_name() == "multi-cpu")
+        for (ITYPE i = 0; i < inner_dim; ++i)
+            ASSERT_NEAR(
+                abs(state_eigen[i + offs] - state.data_cpp()[i]), 0, eps);
+    else
+        for (ITYPE i = 0; i < dim; ++i)
+            ASSERT_NEAR(abs(state_eigen[i] - state.data_cpp()[i]), 0, eps);
 }
 
-TEST(CircuitTest, CircuitOptimize) {
+TEST(CircuitTest_multicpu, CircuitRev) {
     const UINT n = 4;
     const UINT dim = 1ULL << n;
+    MPIutil& mpiutil = MPIutil::get_inst();
+    UINT mpirank = mpiutil.get_rank();
+    UINT mpisize = mpiutil.get_size();
+    ITYPE inner_dim = dim / mpisize;
+    ITYPE offs = inner_dim * mpirank;
+
+    Random random;
+    random.set_seed(2022);
+
+    QuantumState state(n, true);
+    QuantumState state_ref(n, false);
+    ComplexVector state_eigen(dim);
+
+    state.set_Haar_random_state();
+    state_ref.load(&state);
+    for (ITYPE i = 0; i < dim; ++i) state_eigen[i] = state_ref.data_cpp()[i];
+
+    QuantumCircuit circuit(n);
+    UINT target, target_sub;
+    double angle;
+
+    target = random.int32() % n;
+    circuit.add_X_gate(target);
+
+    target = random.int32() % n;
+    circuit.add_Y_gate(target);
+
+    target = random.int32() % n;
+    circuit.add_Z_gate(target);
+
+    target = random.int32() % n;
+    circuit.add_H_gate(target);
+
+    target = random.int32() % n;
+    circuit.add_S_gate(target);
+
+    target = random.int32() % n;
+    circuit.add_Sdag_gate(target);
+
+    target = random.int32() % n;
+    circuit.add_T_gate(target);
+
+    target = random.int32() % n;
+    circuit.add_Tdag_gate(target);
+
+    target = random.int32() % n;
+    circuit.add_sqrtX_gate(target);
+
+    target = random.int32() % n;
+    circuit.add_sqrtXdag_gate(target);
+
+    target = random.int32() % n;
+    circuit.add_sqrtY_gate(target);
+
+    target = random.int32() % n;
+    circuit.add_sqrtYdag_gate(target);
+
+    target = random.int32() % n;
+    angle = random.uniform() * 3.14159;
+    circuit.add_RX_gate(target, angle);
+    circuit.add_RotInvX_gate(target, angle);
+    circuit.add_RotX_gate(target, angle);
+
+    target = random.int32() % n;
+    angle = random.uniform() * 3.14159;
+    circuit.add_RY_gate(target, angle);
+    circuit.add_RotInvY_gate(target, angle);
+    circuit.add_RotInvY_gate(target, angle);
+
+    target = random.int32() % n;
+    angle = random.uniform() * 3.14159;
+    circuit.add_RZ_gate(target, angle);
+    circuit.add_RotInvZ_gate(target, angle);
+    circuit.add_RotZ_gate(target, -angle);
+
+    target = random.int32() % n;
+    target_sub = random.int32() % (n - 1);
+    if (target_sub >= target) target_sub++;
+    circuit.add_CNOT_gate(target, target_sub);
+
+    target = random.int32() % n;
+    target_sub = random.int32() % (n - 1);
+    if (target_sub >= target) target_sub++;
+    circuit.add_CZ_gate(target, target_sub);
+
+    target = random.int32() % n;
+    target_sub = random.int32() % (n - 1);
+    if (target_sub >= target) target_sub++;
+    circuit.add_SWAP_gate(target, target_sub);
+
+    Observable observable(n);
+    angle = 2 * PI * random.uniform();
+
+    observable.add_operator(1.0, "Z 0");
+    observable.add_operator(2.0, "Z 0 Z 1");
+
+    circuit.add_diagonal_observable_rotation_gate(observable, angle);
+
+    circuit.update_quantum_state(&state);
+
+    auto revcircuit = circuit.get_inverse();
+
+    revcircuit->update_quantum_state(&state);
+
+    if (state.get_device_name() == "multi-cpu")
+        for (ITYPE i = 0; i < inner_dim; ++i)
+            ASSERT_NEAR(
+                abs(state_eigen[i + offs] - state.data_cpp()[i]), 0, eps);
+    else
+        for (ITYPE i = 0; i < dim; ++i)
+            ASSERT_NEAR(abs(state_eigen[i] - state.data_cpp()[i]), 0, eps);
+
+    delete revcircuit;
+}
+
+TEST(CircuitTest_multicpu, CircuitOptimize) {
+    MPIutil& m = MPIutil::get_inst();
+    const UINT num_global_qubit = (UINT)std::log2(m.get_size());
+    UINT n = 4 + num_global_qubit;
+    const UINT dim = 1ULL << n;
 
     {
         // merge successive gates
-        int ngpus = get_num_device();
-        for (int idx = 0; idx < ngpus; ++idx) {
-            set_device(idx);
-
-            QuantumStateGpu state(n, idx), test_state(n, idx);
-            state.set_Haar_random_state();
-            test_state.load(&state);
-            QuantumCircuit circuit(n);
-
-            circuit.add_X_gate(0);
-            circuit.add_Y_gate(0);
-            UINT block_size = 2;
-            UINT expected_depth = 1;
-            UINT expected_gate_count = 1;
+        QuantumState state(n, true), test_state(n, true);
+        state.set_Haar_random_state();
+        test_state.load(&state);
+        QuantumCircuit circuit(n);
 
-            QuantumCircuit* copy_circuit = circuit.copy();
-            QuantumCircuitOptimizer qco;
-            qco.optimize(copy_circuit, block_size);
-            circuit.update_quantum_state(&test_state);
-            copy_circuit->update_quantum_state(&state);
-            // std::cout << circuit << std::endl << copy_circuit << std::endl;
-            assert_gpu_eq_gpu(state, test_state, dim, eps);
-            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-            delete copy_circuit;
-        }
+        circuit.add_X_gate(0);
+        circuit.add_Y_gate(0);
+        UINT block_size = 2;
+        UINT expected_depth = 1;
+        UINT expected_gate_count = 1;
+
+        QuantumCircuit* copy_circuit = circuit.copy();
+        QuantumCircuitOptimizer qco;
+        qco.optimize(copy_circuit, block_size);
+        circuit.update_quantum_state(&test_state);
+        copy_circuit->update_quantum_state(&state);
+
+        ASSERT_STATE_NEAR(state, test_state, eps);
+        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+        delete copy_circuit;
     }
 
     {
         // tensor product, merged
-        int ngpus = get_num_device();
-        for (int idx = 0; idx < ngpus; ++idx) {
-            set_device(idx);
-
-            QuantumStateGpu state(n, idx), test_state(n, idx);
-            state.set_Haar_random_state();
-            test_state.load(&state);
-            QuantumCircuit circuit(n);
-
-            circuit.add_X_gate(0);
-            circuit.add_Y_gate(1);
-            UINT block_size = 2;
-            UINT expected_depth = 1;
-            UINT expected_gate_count = 1;
+        QuantumState state(n, true), test_state(n, true);
+        state.set_Haar_random_state();
+        test_state.load(&state);
+        QuantumCircuit circuit(n);
 
-            QuantumCircuit* copy_circuit = circuit.copy();
-            QuantumCircuitOptimizer qco;
-            qco.optimize(copy_circuit, block_size);
-            circuit.update_quantum_state(&test_state);
-            copy_circuit->update_quantum_state(&state);
-            // std::cout << circuit << std::endl << copy_circuit << std::endl;
-            assert_gpu_eq_gpu(state, test_state, dim, eps);
-            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-            delete copy_circuit;
-        }
+        circuit.add_X_gate(0);
+        circuit.add_Y_gate(1);
+        UINT block_size = 2;
+        UINT expected_depth = 1;
+        UINT expected_gate_count = 1;
+
+        QuantumCircuit* copy_circuit = circuit.copy();
+        QuantumCircuitOptimizer qco;
+        qco.optimize(copy_circuit, block_size);
+        circuit.update_quantum_state(&test_state);
+        copy_circuit->update_quantum_state(&state);
+
+        ASSERT_STATE_NEAR(state, test_state, eps);
+        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+        delete copy_circuit;
     }
 
     {
         // do not take tensor product
-        int ngpus = get_num_device();
-        for (int idx = 0; idx < ngpus; ++idx) {
-            set_device(idx);
-
-            QuantumStateGpu state(n, idx), test_state(n, idx);
-            state.set_Haar_random_state();
-            test_state.load(&state);
-            QuantumCircuit circuit(n);
-
-            circuit.add_X_gate(0);
-            circuit.add_Y_gate(1);
-            UINT block_size = 1;
-            UINT expected_depth = 1;
-            UINT expected_gate_count = 2;
+        QuantumState state(n, true), test_state(n, true);
+        state.set_Haar_random_state();
+        test_state.load(&state);
+        QuantumCircuit circuit(n);
 
-            QuantumCircuit* copy_circuit = circuit.copy();
-            QuantumCircuitOptimizer qco;
-            qco.optimize(copy_circuit, block_size);
-            circuit.update_quantum_state(&test_state);
-            copy_circuit->update_quantum_state(&state);
-            // std::cout << circuit << std::endl << copy_circuit << std::endl;
-            assert_gpu_eq_gpu(state, test_state, dim, eps);
-            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-            delete copy_circuit;
-        }
+        circuit.add_X_gate(0);
+        circuit.add_Y_gate(1);
+        UINT block_size = 1;
+        UINT expected_depth = 1;
+        UINT expected_gate_count = 2;
+
+        QuantumCircuit* copy_circuit = circuit.copy();
+        QuantumCircuitOptimizer qco;
+        qco.optimize(copy_circuit, block_size);
+        circuit.update_quantum_state(&test_state);
+        copy_circuit->update_quantum_state(&state);
+
+        ASSERT_STATE_NEAR(state, test_state, eps);
+        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+        delete copy_circuit;
     }
 
     {
         // CNOT, control does not commute with X
-        int ngpus = get_num_device();
-        for (int idx = 0; idx < ngpus; ++idx) {
-            set_device(idx);
-
-            QuantumStateGpu state(n, idx), test_state(n, idx);
-            state.set_Haar_random_state();
-            test_state.load(&state);
-            QuantumCircuit circuit(n);
-
-            circuit.add_X_gate(0);
-            circuit.add_CNOT_gate(0, 1);
-            circuit.add_Y_gate(0);
-            UINT block_size = 1;
-            UINT expected_depth = 3;
-            UINT expected_gate_count = 3;
+        QuantumState state(n, true), test_state(n, true);
+        state.set_Haar_random_state();
+        test_state.load(&state);
+        QuantumCircuit circuit(n);
 
-            QuantumCircuit* copy_circuit = circuit.copy();
-            QuantumCircuitOptimizer qco;
-            qco.optimize(copy_circuit, block_size);
-            circuit.update_quantum_state(&test_state);
-            copy_circuit->update_quantum_state(&state);
-            // std::cout << circuit << std::endl << copy_circuit << std::endl;
-            assert_gpu_eq_gpu(state, test_state, dim, eps);
-            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-            delete copy_circuit;
-        }
+        circuit.add_X_gate(0);
+        circuit.add_CNOT_gate(0, 1);
+        circuit.add_Y_gate(0);
+        UINT block_size = 1;
+        UINT expected_depth = 3;
+        UINT expected_gate_count = 3;
+
+        QuantumCircuit* copy_circuit = circuit.copy();
+        QuantumCircuitOptimizer qco;
+        qco.optimize(copy_circuit, block_size);
+        circuit.update_quantum_state(&test_state);
+        copy_circuit->update_quantum_state(&state);
+
+        ASSERT_STATE_NEAR(state, test_state, eps);
+        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+        delete copy_circuit;
     }
 
     {
         // CNOT, control does not commute with Z
-        int ngpus = get_num_device();
-        for (int idx = 0; idx < ngpus; ++idx) {
-            set_device(idx);
-
-            QuantumStateGpu state(n, idx), test_state(n, idx);
-            state.set_Haar_random_state();
-            test_state.load(&state);
-            QuantumCircuit circuit(n);
-
-            circuit.add_X_gate(0);
-            circuit.add_CNOT_gate(0, 1);
-            circuit.add_Z_gate(0);
-            UINT block_size = 1;
-            UINT expected_depth = 2;
-            UINT expected_gate_count = 2;
+        QuantumState state(n, true), test_state(n, true);
+        state.set_Haar_random_state();
+        test_state.load(&state);
+        QuantumCircuit circuit(n);
 
-            QuantumCircuit* copy_circuit = circuit.copy();
-            QuantumCircuitOptimizer qco;
-            qco.optimize(copy_circuit, block_size);
-            circuit.update_quantum_state(&test_state);
-            copy_circuit->update_quantum_state(&state);
-            // std::cout << circuit << std::endl << copy_circuit << std::endl;
-            assert_gpu_eq_gpu(state, test_state, dim, eps);
-            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-            delete copy_circuit;
-        }
+        circuit.add_X_gate(0);
+        circuit.add_CNOT_gate(0, 1);
+        circuit.add_Z_gate(0);
+        UINT block_size = 1;
+        UINT expected_depth = 2;
+        UINT expected_gate_count = 2;
+
+        QuantumCircuit* copy_circuit = circuit.copy();
+        QuantumCircuitOptimizer qco;
+        qco.optimize(copy_circuit, block_size);
+        circuit.update_quantum_state(&test_state);
+        copy_circuit->update_quantum_state(&state);
+
+        ASSERT_STATE_NEAR(state, test_state, eps);
+        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+        delete copy_circuit;
     }
 
     {
         // CNOT, control commute with Z
-        int ngpus = get_num_device();
-        for (int idx = 0; idx < ngpus; ++idx) {
-            set_device(idx);
-
-            QuantumStateGpu state(n, idx), test_state(n, idx);
-            state.set_Haar_random_state();
-            test_state.load(&state);
-            QuantumCircuit circuit(n);
-
-            circuit.add_Z_gate(0);
-            circuit.add_CNOT_gate(0, 1);
-            circuit.add_Z_gate(0);
-            UINT block_size = 1;
-            UINT expected_depth = 2;
-            UINT expected_gate_count = 2;
+        QuantumState state(n, true), test_state(n, true);
+        state.set_Haar_random_state();
+        test_state.load(&state);
+        QuantumCircuit circuit(n);
 
-            QuantumCircuit* copy_circuit = circuit.copy();
-            QuantumCircuitOptimizer qco;
-            qco.optimize(copy_circuit, block_size);
-            circuit.update_quantum_state(&test_state);
-            copy_circuit->update_quantum_state(&state);
-            // std::cout << circuit << std::endl << copy_circuit << std::endl;
-            assert_gpu_eq_gpu(state, test_state, dim, eps);
-            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-            delete copy_circuit;
-        }
+        circuit.add_Z_gate(0);
+        circuit.add_CNOT_gate(0, 1);
+        circuit.add_Z_gate(0);
+        UINT block_size = 1;
+        UINT expected_depth = 2;
+        UINT expected_gate_count = 2;
+
+        QuantumCircuit* copy_circuit = circuit.copy();
+        QuantumCircuitOptimizer qco;
+        qco.optimize(copy_circuit, block_size);
+        circuit.update_quantum_state(&test_state);
+        copy_circuit->update_quantum_state(&state);
+        ASSERT_STATE_NEAR(state, test_state, eps);
+        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+        delete copy_circuit;
     }
 
     {
         // CNOT, target commute with X
-        int ngpus = get_num_device();
-        for (int idx = 0; idx < ngpus; ++idx) {
-            set_device(idx);
-
-            QuantumStateGpu state(n, idx), test_state(n, idx);
-            state.set_Haar_random_state();
-            test_state.load(&state);
-            QuantumCircuit circuit(n);
-
-            circuit.add_X_gate(1);
-            circuit.add_CNOT_gate(0, 1);
-            circuit.add_X_gate(1);
-            UINT block_size = 1;
-            UINT expected_depth = 2;
-            UINT expected_gate_count = 2;
+        QuantumState state(n, true), test_state(n, true);
+        state.set_Haar_random_state();
+        test_state.load(&state);
+        QuantumCircuit circuit(n);
 
-            QuantumCircuit* copy_circuit = circuit.copy();
-            QuantumCircuitOptimizer qco;
-            qco.optimize(copy_circuit, block_size);
-            circuit.update_quantum_state(&test_state);
-            copy_circuit->update_quantum_state(&state);
-            // std::cout << circuit << std::endl << copy_circuit << std::endl;
-            assert_gpu_eq_gpu(state, test_state, dim, eps);
-            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-            delete copy_circuit;
-        }
+        circuit.add_X_gate(1);
+        circuit.add_CNOT_gate(0, 1);
+        circuit.add_X_gate(1);
+        UINT block_size = 1;
+        UINT expected_depth = 2;
+        UINT expected_gate_count = 2;
+
+        QuantumCircuit* copy_circuit = circuit.copy();
+        QuantumCircuitOptimizer qco;
+        qco.optimize(copy_circuit, block_size);
+        circuit.update_quantum_state(&test_state);
+        copy_circuit->update_quantum_state(&state);
+
+        ASSERT_STATE_NEAR(state, test_state, eps);
+        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+        delete copy_circuit;
     }
 
     {
         // CNOT, target commute with X
-        int ngpus = get_num_device();
-        for (int idx = 0; idx < ngpus; ++idx) {
-            set_device(idx);
-
-            QuantumStateGpu state(n, idx), test_state(n, idx);
-            state.set_Haar_random_state();
-            test_state.load(&state);
-            QuantumCircuit circuit(n);
-
-            circuit.add_Z_gate(1);
-            circuit.add_CNOT_gate(0, 1);
-            circuit.add_X_gate(1);
-            UINT block_size = 1;
-            UINT expected_depth = 2;
-            UINT expected_gate_count = 2;
+        QuantumState state(n, true), test_state(n, true);
+        state.set_Haar_random_state();
+        test_state.load(&state);
+        QuantumCircuit circuit(n);
 
-            QuantumCircuit* copy_circuit = circuit.copy();
-            QuantumCircuitOptimizer qco;
-            qco.optimize(copy_circuit, block_size);
-            circuit.update_quantum_state(&test_state);
-            copy_circuit->update_quantum_state(&state);
-            // std::cout << circuit << std::endl << copy_circuit << std::endl;
-            assert_gpu_eq_gpu(state, test_state, dim, eps);
-            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-            delete copy_circuit;
-        }
+        circuit.add_Z_gate(1);
+        circuit.add_CNOT_gate(0, 1);
+        circuit.add_X_gate(1);
+        UINT block_size = 1;
+        UINT expected_depth = 2;
+        UINT expected_gate_count = 2;
+
+        QuantumCircuit* copy_circuit = circuit.copy();
+        QuantumCircuitOptimizer qco;
+        qco.optimize(copy_circuit, block_size);
+        circuit.update_quantum_state(&test_state);
+        copy_circuit->update_quantum_state(&state);
+
+        ASSERT_STATE_NEAR(state, test_state, eps);
+        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+        delete copy_circuit;
     }
 
     {
         // CNOT, target commute with X
-        int ngpus = get_num_device();
-        for (int idx = 0; idx < ngpus; ++idx) {
-            set_device(idx);
-
-            QuantumStateGpu state(n, idx), test_state(n, idx);
-            state.set_Haar_random_state();
-            test_state.load(&state);
-            QuantumCircuit circuit(n);
-
-            circuit.add_X_gate(1);
-            circuit.add_CNOT_gate(0, 1);
-            circuit.add_Z_gate(1);
-            UINT block_size = 1;
-            UINT expected_depth = 2;
-            UINT expected_gate_count = 2;
+        QuantumState state(n, true), test_state(n, true);
+        state.set_Haar_random_state();
+        test_state.load(&state);
+        QuantumCircuit circuit(n);
 
-            QuantumCircuit* copy_circuit = circuit.copy();
-            QuantumCircuitOptimizer qco;
-            qco.optimize(copy_circuit, block_size);
-            circuit.update_quantum_state(&test_state);
-            copy_circuit->update_quantum_state(&state);
-            // std::cout << circuit << std::endl << copy_circuit << std::endl;
-            // std::cout << state << std::endl << test_state << std::endl;
-            assert_gpu_eq_gpu(state, test_state, dim, eps);
-            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-            delete copy_circuit;
-        }
+        circuit.add_X_gate(1);
+        circuit.add_CNOT_gate(0, 1);
+        circuit.add_Z_gate(1);
+        UINT block_size = 1;
+        UINT expected_depth = 2;
+        UINT expected_gate_count = 2;
+
+        QuantumCircuit* copy_circuit = circuit.copy();
+        QuantumCircuitOptimizer qco;
+        qco.optimize(copy_circuit, block_size);
+        circuit.update_quantum_state(&test_state);
+        copy_circuit->update_quantum_state(&state);
+        ASSERT_STATE_NEAR(state, test_state, eps);
+        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+        delete copy_circuit;
     }
 
     {
         // CNOT, target commute with X
-        int ngpus = get_num_device();
-        for (int idx = 0; idx < ngpus; ++idx) {
-            set_device(idx);
-
-            QuantumStateGpu state(n, idx), test_state(n, idx);
-            state.set_Haar_random_state();
-            test_state.load(&state);
-            QuantumCircuit circuit(n);
-
-            circuit.add_Z_gate(1);
-            circuit.add_CNOT_gate(0, 1);
-            circuit.add_Z_gate(1);
-            UINT block_size = 1;
-            UINT expected_depth = 3;
-            UINT expected_gate_count = 3;
+        QuantumState state(n, true), test_state(n, true);
+        state.set_Haar_random_state();
+        test_state.load(&state);
+        QuantumCircuit circuit(n);
 
-            QuantumCircuit* copy_circuit = circuit.copy();
-            QuantumCircuitOptimizer qco;
-            qco.optimize(copy_circuit, block_size);
-            circuit.update_quantum_state(&test_state);
-            copy_circuit->update_quantum_state(&state);
-            // std::cout << circuit << std::endl << copy_circuit << std::endl;
-            assert_gpu_eq_gpu(state, test_state, dim, eps);
-            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-            delete copy_circuit;
-        }
+        circuit.add_Z_gate(1);
+        circuit.add_CNOT_gate(0, 1);
+        circuit.add_Z_gate(1);
+        UINT block_size = 1;
+        UINT expected_depth = 3;
+        UINT expected_gate_count = 3;
+
+        QuantumCircuit* copy_circuit = circuit.copy();
+        QuantumCircuitOptimizer qco;
+        qco.optimize(copy_circuit, block_size);
+        circuit.update_quantum_state(&test_state);
+        copy_circuit->update_quantum_state(&state);
+
+        ASSERT_STATE_NEAR(state, test_state, eps);
+        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+        delete copy_circuit;
     }
 
     {
         // CNOT, target commute with X
-        int ngpus = get_num_device();
-        for (int idx = 0; idx < ngpus; ++idx) {
-            set_device(idx);
-
-            QuantumStateGpu state(n, idx), test_state(n, idx);
-            state.set_Haar_random_state();
-            test_state.load(&state);
-            QuantumCircuit circuit(n);
-
-            circuit.add_Z_gate(1);
-            circuit.add_CNOT_gate(0, 1);
-            circuit.add_Z_gate(1);
-            UINT block_size = 2;
-            UINT expected_depth = 1;
-            UINT expected_gate_count = 1;
+        QuantumState state(n, true), test_state(n, true);
+        state.set_Haar_random_state();
+        test_state.load(&state);
+        QuantumCircuit circuit(n);
 
-            QuantumCircuit* copy_circuit = circuit.copy();
-            QuantumCircuitOptimizer qco;
-            qco.optimize(copy_circuit, block_size);
-            circuit.update_quantum_state(&test_state);
-            copy_circuit->update_quantum_state(&state);
-            // std::cout << circuit << std::endl << copy_circuit << std::endl;
-            assert_gpu_eq_gpu(state, test_state, dim, eps);
-            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-            delete copy_circuit;
-        }
+        circuit.add_Z_gate(1);
+        circuit.add_CNOT_gate(0, 1);
+        circuit.add_Z_gate(1);
+        UINT block_size = 2;
+        UINT expected_depth = 1;
+        UINT expected_gate_count = 1;
+
+        QuantumCircuit* copy_circuit = circuit.copy();
+        QuantumCircuitOptimizer qco;
+        qco.optimize(copy_circuit, block_size);
+        circuit.update_quantum_state(&test_state);
+        copy_circuit->update_quantum_state(&state);
+        ASSERT_STATE_NEAR(state, test_state, eps);
+        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+        delete copy_circuit;
     }
 
     {
         // CNOT, target commute with X
-        int ngpus = get_num_device();
-        for (int idx = 0; idx < ngpus; ++idx) {
-            set_device(idx);
-
-            QuantumStateGpu state(n, idx), test_state(n, idx);
-            state.set_Haar_random_state();
-            test_state.load(&state);
-            QuantumCircuit circuit(n);
-
-            circuit.add_Z_gate(0);
-            circuit.add_gate(gate::merge(gate::CNOT(0, 1), gate::Y(2)));
-            circuit.add_gate(gate::merge(gate::CNOT(1, 0), gate::Y(2)));
-            circuit.add_Z_gate(1);
-            UINT block_size = 2;
-            UINT expected_depth = 3;
-            UINT expected_gate_count = 3;
+        QuantumState state(n, true), test_state(n, true);
+        state.set_Haar_random_state();
+        test_state.load(&state);
+        QuantumCircuit circuit(n);
 
-            QuantumCircuit* copy_circuit = circuit.copy();
-            QuantumCircuitOptimizer qco;
-            qco.optimize(copy_circuit, block_size);
-            circuit.update_quantum_state(&test_state);
-            copy_circuit->update_quantum_state(&state);
-            // std::cout << circuit << std::endl << copy_circuit << std::endl;
-            assert_gpu_eq_gpu(state, test_state, dim, eps);
-            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
-            delete copy_circuit;
-        }
+        auto gate1 = gate::CNOT(0, 1);
+        auto gate2 = gate::CNOT(1, 2);
+        auto gate3 = gate::Y(2);
+
+        circuit.add_Z_gate(0);
+        circuit.add_gate(gate::merge(gate1, gate3));
+        circuit.add_gate(gate::merge(gate2, gate3));
+        circuit.add_Z_gate(1);
+
+        delete gate1;
+        delete gate2;
+        delete gate3;
+
+        UINT block_size = 2;
+        UINT expected_depth = 3;
+        UINT expected_gate_count = 3;
+
+        QuantumCircuit* copy_circuit = circuit.copy();
+        QuantumCircuitOptimizer qco;
+        qco.optimize(copy_circuit, block_size);
+        circuit.update_quantum_state(&test_state);
+        copy_circuit->update_quantum_state(&state);
+        ASSERT_STATE_NEAR(state, test_state, eps);
+        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+        delete copy_circuit;
     }
 
     {
         // CNOT, target commute with X
-        int ngpus = get_num_device();
-        for (int idx = 0; idx < ngpus; ++idx) {
-            set_device(idx);
-
-            QuantumStateGpu state(n, idx), test_state(n, idx);
-            state.set_Haar_random_state();
-            test_state.load(&state);
-            QuantumCircuit circuit(n);
-
-            circuit.add_Z_gate(0);
-            circuit.add_gate(gate::merge(gate::CNOT(0, 1), gate::Y(2)));
-            circuit.add_gate(gate::merge(gate::CNOT(1, 0), gate::Y(2)));
-            circuit.add_Z_gate(1);
-            UINT block_size = 3;
-            UINT expected_depth = 1;
-            UINT expected_gate_count = 1;
+        QuantumState state(n, true), test_state(n, true);
+        state.set_Haar_random_state();
+        test_state.load(&state);
+        QuantumCircuit circuit(n);
+
+        auto gate1 = gate::CNOT(0, 1);
+        auto gate2 = gate::CNOT(1, 2);
+        auto gate3 = gate::Y(2);
+
+        circuit.add_Z_gate(0);
+        circuit.add_gate(gate::merge(gate1, gate3));
+        circuit.add_gate(gate::merge(gate2, gate3));
+        circuit.add_Z_gate(1);
+
+        delete gate1;
+        delete gate2;
+        delete gate3;
+
+        UINT block_size = 3;
+        UINT expected_depth = 1;
+        UINT expected_gate_count = 1;
+
+        QuantumCircuit* copy_circuit = circuit.copy();
+        QuantumCircuitOptimizer qco;
+        qco.optimize(copy_circuit, block_size);
+        circuit.update_quantum_state(&test_state);
+        copy_circuit->update_quantum_state(&state);
+        ASSERT_STATE_NEAR(state, test_state, eps);
+        ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+        ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+        delete copy_circuit;
+    }
+}
+
+TEST(CircuitTest_multicpu, RandomCircuitOptimize) {
+    const UINT n = 5;
+    const UINT dim = 1ULL << n;
+    const UINT depth = 5;
+    Random random;
+    random.set_seed(2022);
+
+    UINT max_repeat = 3;
+    // UINT max_block_size = n;
+    UINT max_block_size = 1;  // TODO: multi-cpu limitation.
+
+    for (UINT repeat = 0; repeat < max_repeat; ++repeat) {
+        QuantumState state(n, true), org_state(n, true), test_state(n, true);
+        state.set_Haar_random_state();
+        org_state.load(&state);
+        QuantumCircuit circuit(n);
+
+        for (UINT d = 0; d < depth; ++d) {
+            for (UINT i = 0; i < n; ++i) {
+                UINT r = random.int32() % 5;
+                if (r == 0)
+                    circuit.add_sqrtX_gate(i);
+                else if (r == 1)
+                    circuit.add_sqrtY_gate(i);
+                else if (r == 2)
+                    circuit.add_T_gate(i);
+                else if (r == 3) {
+                    if (i + 1 < n) circuit.add_CNOT_gate(i, i + 1);
+                } else if (r == 4) {
+                    if (i + 1 < n) circuit.add_CZ_gate(i, i + 1);
+                }
+            }
+        }
 
+        test_state.load(&org_state);
+        circuit.update_quantum_state(&test_state);
+        QuantumCircuitOptimizer qco;
+        for (UINT block_size = 1; block_size <= max_block_size; ++block_size) {
             QuantumCircuit* copy_circuit = circuit.copy();
-            QuantumCircuitOptimizer qco;
             qco.optimize(copy_circuit, block_size);
-            circuit.update_quantum_state(&test_state);
+            state.load(&org_state);
             copy_circuit->update_quantum_state(&state);
-            // std::cout << circuit << std::endl << copy_circuit << std::endl;
-            assert_gpu_eq_gpu(state, test_state, dim, eps);
-            ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
-            ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+            ASSERT_STATE_NEAR(state, test_state, eps);
             delete copy_circuit;
         }
     }
 }
 
-TEST(CircuitTest, RandomCircuitOptimize) {
+TEST(CircuitTest_multicpu, RandomCircuitOptimize2) {
     const UINT n = 5;
     const UINT dim = 1ULL << n;
-    const UINT depth = 5;
+    const UINT depth = 10;
     Random random;
+    random.set_seed(2022);
 
     UINT max_repeat = 3;
-    UINT max_block_size = n;
+    // UINT max_block_size = n;
+    UINT max_block_size = 1;  // TODO: multi-cpu limitation.
 
-    int ngpus = get_num_device();
-    for (int idx = 0; idx < ngpus; ++idx) {
-        set_device(idx);
-        for (UINT repeat = 0; repeat < max_repeat; ++repeat) {
-            QuantumStateGpu state(n, idx), org_state(n, idx),
-                test_state(n, idx);
-            state.set_Haar_random_state();
-            org_state.load(&state);
-            QuantumCircuit circuit(n);
-
-            for (UINT d = 0; d < depth; ++d) {
-                for (UINT i = 0; i < n; ++i) {
-                    UINT r = random.int32() % 5;
-                    if (r == 0)
-                        circuit.add_sqrtX_gate(i);
-                    else if (r == 1)
-                        circuit.add_sqrtY_gate(i);
-                    else if (r == 2)
-                        circuit.add_T_gate(i);
-                    else if (r == 3) {
-                        if (i + 1 < n) circuit.add_CNOT_gate(i, i + 1);
-                    } else if (r == 4) {
-                        if (i + 1 < n) circuit.add_CZ_gate(i, i + 1);
-                    }
+    for (UINT repeat = 0; repeat < max_repeat; ++repeat) {
+        QuantumState state(n, true), org_state(n, true), test_state(n, true);
+        state.set_Haar_random_state();
+        org_state.load(&state);
+        QuantumCircuit circuit(n);
+
+        for (UINT d = 0; d < depth; ++d) {
+            for (UINT i = 0; i < n; ++i) {
+                UINT r = random.int32() % 6;
+                if (r == 0)
+                    circuit.add_sqrtX_gate(i);
+                else if (r == 1)
+                    circuit.add_sqrtY_gate(i);
+                else if (r == 2)
+                    circuit.add_T_gate(i);
+                else if (r == 3) {
+                    UINT r2 = random.int32() % n;
+                    if (r2 == i) r2 = (r2 + 1) % n;
+                    if (i + 1 < n) circuit.add_CNOT_gate(i, r2);
+                } else if (r == 4) {
+                    UINT r2 = random.int32() % n;
+                    if (r2 == i) r2 = (r2 + 1) % n;
+                    if (i + 1 < n) circuit.add_CZ_gate(i, r2);
+                } else if (r == 5) {
+                    UINT r2 = random.int32() % n;
+                    if (r2 == i) r2 = (r2 + 1) % n;
+                    if (i + 1 < n) circuit.add_SWAP_gate(i, r2);
                 }
             }
+        }
 
-            test_state.load(&org_state);
-            circuit.update_quantum_state(&test_state);
-            // std::cout << circuit << std::endl;
-            QuantumCircuitOptimizer qco;
-            for (UINT block_size = 1; block_size <= max_block_size;
-                 ++block_size) {
-                QuantumCircuit* copy_circuit = circuit.copy();
-                qco.optimize(copy_circuit, block_size);
-                state.load(&org_state);
-                copy_circuit->update_quantum_state(&state);
-                // std::cout << copy_circuit << std::endl;
-                assert_gpu_eq_gpu(state, test_state, dim, eps);
-                delete copy_circuit;
-            }
+        test_state.load(&org_state);
+        circuit.update_quantum_state(&test_state);
+        QuantumCircuitOptimizer qco;
+        for (UINT block_size = 1; block_size <= max_block_size; ++block_size) {
+            QuantumCircuit* copy_circuit = circuit.copy();
+            qco.optimize(copy_circuit, block_size);
+            state.load(&org_state);
+            copy_circuit->update_quantum_state(&state);
+            ASSERT_STATE_NEAR(state, test_state, eps);
+            delete copy_circuit;
         }
     }
 }
 
-TEST(CircuitTest, RandomCircuitOptimizeLarge) {
+TEST(CircuitTest_multicpu, RandomCircuitOptimize3) {
     const UINT n = 5;
     const UINT dim = 1ULL << n;
-    const UINT depth = 5;
+    const UINT depth = 10 * n;
     Random random;
+    random.set_seed(2022);
+    MPIutil& mpiutil = MPIutil::get_inst();
+    UINT mpirank = mpiutil.get_rank();
+    UINT mpisize = mpiutil.get_size();
 
     UINT max_repeat = 3;
-    UINT max_block_size = n;
-    int ngpus = get_num_device();
-    for (int idx = 0; idx < ngpus; ++idx) {
-        set_device(idx);
-        for (UINT repeat = 0; repeat < max_repeat; ++repeat) {
-            QuantumStateGpu state(n, idx), org_state(n, idx),
-                test_state(n, idx);
-            state.set_Haar_random_state();
-            org_state.load(&state);
-            QuantumCircuit circuit(n);
-
-            for (UINT d = 0; d < depth; ++d) {
-                for (UINT i = 0; i < n; ++i) {
-                    UINT r = random.int32() % 5;
-                    if (r == 0)
-                        circuit.add_sqrtX_gate(i);
-                    else if (r == 1)
-                        circuit.add_sqrtY_gate(i);
-                    else if (r == 2)
-                        circuit.add_T_gate(i);
-                    else if (r == 3) {
-                        if (i + 1 < n) circuit.add_CNOT_gate(i, i + 1);
-                    } else if (r == 4) {
-                        if (i + 1 < n) circuit.add_CZ_gate(i, i + 1);
-                    }
-                }
-            }
+    // UINT max_block_size = n;
+    UINT max_block_size = 1;  // TODO: multi-cpu limitation.
+    UINT seed = 2021;
+    std::mt19937 eng(seed);
+
+    std::vector<UINT> qubit_list;
+    for (int i = 0; i < n; ++i) qubit_list.push_back(i);
+
+    for (UINT repeat = 0; repeat < max_repeat; ++repeat) {
+        QuantumState state(n, true), org_state(n, true), test_state(n, true);
+        state.set_Haar_random_state(2000);
+        org_state.load(&state);
+        QuantumCircuit circuit(n);
 
-            test_state.load(&org_state);
-            circuit.update_quantum_state(&test_state);
-            // std::cout << circuit << std::endl;
-            QuantumCircuitOptimizer qco;
-            for (UINT block_size = 1; block_size <= max_block_size;
-                 ++block_size) {
-                QuantumCircuit* copy_circuit = circuit.copy();
-                qco.optimize(copy_circuit, block_size);
-                state.load(&org_state);
-                copy_circuit->update_quantum_state(&state);
-                // std::cout << copy_circuit << std::endl;
-                assert_gpu_eq_gpu(state, test_state, dim, eps);
-                delete copy_circuit;
-            }
+        for (UINT d = 0; d < depth; ++d) {
+            std::shuffle(qubit_list.begin(), qubit_list.end(), eng);
+            std::vector<UINT> mylist;
+            mylist.push_back(qubit_list[0]);
+            mylist.push_back(qubit_list[1]);
+            circuit.add_random_unitary_gate(mylist, seed + d);
+            // circuit.add_CNOT_gate(qubit_list[0], qubit_list[1]);
+        }
+
+        test_state.load(&org_state);
+        circuit.update_quantum_state(&test_state);
+        // std::cout << "#original-circuit " << mpirank << ":" << circuit <<
+        // std::endl; std::cout << "# test_state" << mpirank << ": " <<
+        // test_state << std::endl;
+        QuantumCircuitOptimizer qco;
+        for (UINT block_size = 1; block_size <= max_block_size; ++block_size) {
+            QuantumCircuit* copy_circuit = circuit.copy();
+            qco.optimize(copy_circuit, block_size);
+            state.load(&org_state);
+            copy_circuit->update_quantum_state(&state);
+            // std::cout << "#optimized-circuit " << mpirank << ":" <<
+            // block_size << ", " << circuit << std::endl; std::cout << "#
+            // state" << mpirank << ": " << state << std::endl;
+            ASSERT_STATE_NEAR(state, test_state, eps);
+            delete copy_circuit;
         }
     }
 }
 
-TEST(CircuitTest, SuzukiTrotterExpansion) {
+TEST(CircuitTest_multicpu, SuzukiTrotterExpansion) {
     CPPCTYPE J(0.0, 1.0);
-    Eigen::MatrixXcd Identity(2, 2), X(2, 2), Y(2, 2), Z(2, 2);
-    Identity << 1, 0, 0, 1;
-    X << 0, 1, 1, 0;
-    Y << 0, -J, J, 0;
-    Z << 1, 0, 0, -1;
+    const auto Identity = make_Identity();
+    const auto X = make_X();
+    const auto Y = make_Y();
+    const auto Z = make_Z();
 
     const UINT n = 2;
-    UINT num_repeats;
     const UINT dim = 1ULL << n;
 
     double angle;
     std::vector<double> coef;
 
     const UINT seed = 1918;
     Random random;
     random.set_seed(seed);
 
-    double res;
+    CPPCTYPE res;
     CPPCTYPE test_res;
 
-    int ngpus = get_num_device();
-    for (int idx = 0; idx < ngpus; ++idx) {
-        Observable diag_observable(n), non_diag_observable(n), observable(n);
-        Eigen::MatrixXcd test_observable;
+    Observable diag_observable(n), non_diag_observable(n), observable(n);
+    Eigen::MatrixXcd test_observable;
 
-        QuantumStateGpu state(n, idx);
-        Eigen::VectorXcd test_state = Eigen::VectorXcd::Zero(dim);
+    QuantumState state(n, true);
+    Eigen::VectorXcd test_state = Eigen::VectorXcd::Zero(dim);
 
-        QuantumCircuit circuit(n);
-        Eigen::MatrixXcd test_circuit;
+    QuantumCircuit circuit(n);
+    Eigen::MatrixXcd test_circuit;
 
-        for (ITYPE i = 0; i < 6; ++i) {
-            coef.push_back(-random.uniform());
-            // coef.push_back(-1.);
-        }
-        angle = 2 * PI * random.uniform();
+    for (ITYPE i = 0; i < 6; ++i) {
+        coef.push_back(-random.uniform());
+        // coef.push_back(-1.);
+    }
+    angle = 2 * PI * random.uniform();
+
+    observable.add_operator(coef[0], "Z 0 I 1");
+    observable.add_operator(coef[1], "X 0 Y 1");
+    observable.add_operator(coef[2], "Z 0 Z 1");
+    observable.add_operator(coef[3], "Z 0 X 1");
+    observable.add_operator(coef[4], "Y 0 X 1");
+    observable.add_operator(coef[5], "I 0 Z 1");
+
+    test_observable =
+        coef[0] * get_expanded_eigen_matrix_with_identity(0, Z, n);
+    test_observable += coef[1] * kronecker_product(Y, X);
+    test_observable += coef[2] * kronecker_product(Z, Z);
+    test_observable += coef[3] * kronecker_product(X, Z);
+    test_observable += coef[4] * kronecker_product(X, Y);
+    test_observable +=
+        coef[5] * get_expanded_eigen_matrix_with_identity(1, Z, n);
+
+    const auto num_repeats =
+        static_cast<UINT>(std::ceil(angle * (double)n * 100.));
+    // circuit.add_diagonal_observable_rotation_gate(diag_observable, angle);
+    circuit.add_observable_rotation_gate(observable, angle, num_repeats);
+
+    test_circuit = J * angle * test_observable;
+    test_circuit = test_circuit.exp();
+
+    state.set_computational_basis(0);
+    test_state(0) = 1.;
+
+    res = observable.get_expectation_value(&state);
+    test_res = (test_state.adjoint() * test_observable * test_state)(0, 0);
+
+    circuit.update_quantum_state(&state);
+    test_state = test_circuit * test_state;
+
+    res = observable.get_expectation_value(&state);
+    test_res = (test_state.adjoint() * test_observable * test_state)(0, 0);
+    ASSERT_NEAR(abs(test_res.real() - res.real()) / test_res.real(), 0, 0.01);
+
+    state.set_Haar_random_state(seed);
+    for (ITYPE i = 0; i < dim; ++i) test_state[i] = state.data_cpp()[i];
+
+    test_state = test_circuit * test_state;
+    circuit.update_quantum_state(&state);
+
+    res = observable.get_expectation_value(&state);
+    test_res = (test_state.adjoint() * test_observable * test_state)(0, 0);
+    ASSERT_NEAR(abs(test_res.real() - res.real()) / test_res.real(), 0, 0.01);
+}
+
+TEST(CircuitTest_multicpu, RotateDiagonalObservable) {
+    CPPCTYPE J(0.0, 1.0);
+    const auto Identity = make_Identity();
+    const auto X = make_X();
+    const auto Y = make_Y();
+    const auto Z = make_Z();
+
+    const UINT n = 2;
+    const UINT dim = 1ULL << n;
+
+    double angle, coef1, coef2;
+    Random random;
+    random.set_seed(2022);
+
+    CPPCTYPE res;
+    CPPCTYPE test_res;
+
+    Observable observable(n);
+    Eigen::MatrixXcd test_observable;
+
+    QuantumState state(n, true);
+    Eigen::VectorXcd test_state = Eigen::VectorXcd::Zero(dim);
+
+    QuantumCircuit circuit(n);
+    Eigen::MatrixXcd test_circuit;
 
-        observable.add_operator(coef[0], "Z 0 I 1");
-        observable.add_operator(coef[1], "X 0 Y 1");
-        observable.add_operator(coef[2], "Z 0 Z 1");
-        observable.add_operator(coef[3], "Z 0 X 1");
-        observable.add_operator(coef[4], "Y 0 X 1");
-        observable.add_operator(coef[5], "I 0 Z 1");
+    coef1 = -random.uniform();
+    coef2 = -random.uniform();
+    angle = 2 * PI * random.uniform();
 
-        test_observable =
-            coef[0] * get_expanded_eigen_matrix_with_identity(0, Z, n);
-        test_observable += coef[1] * kronecker_product(Y, X);
-        test_observable += coef[2] * kronecker_product(Z, Z);
-        test_observable += coef[3] * kronecker_product(X, Z);
-        test_observable += coef[4] * kronecker_product(X, Y);
-        test_observable +=
-            coef[5] * get_expanded_eigen_matrix_with_identity(1, Z, n);
+    observable.add_operator(coef1, "Z 0");
+    observable.add_operator(coef2, "Z 0 Z 1");
 
-        num_repeats = (UINT)std::ceil(angle * (double)n * 100.);
-        // circuit.add_diagonal_observable_rotation_gate(diag_observable,
-        // angle);
-        circuit.add_observable_rotation_gate(observable, angle, num_repeats);
+    test_observable = coef1 * get_expanded_eigen_matrix_with_identity(0, Z, n);
+    test_observable += coef2 * kronecker_product(Z, Z);
 
-        test_circuit = J * angle * test_observable;
-        test_circuit = test_circuit.exp();
+    circuit.add_diagonal_observable_rotation_gate(observable, angle);
+    test_circuit = (J * angle * test_observable).exp();
 
-        state.set_computational_basis(0);
-        test_state(0) = 1.;
+    state.set_computational_basis(0);
+    test_state(0) = 1.;
 
-        res = observable.get_expectation_value(&state).real();
-        test_res = (test_state.adjoint() * test_observable * test_state);
+    circuit.update_quantum_state(&state);
+    test_state = test_circuit * test_state;
 
-        circuit.update_quantum_state(&state);
-        test_state = test_circuit * test_state;
+    res = observable.get_expectation_value(&state);
+    test_res = (test_state.adjoint() * test_observable * test_state)(0, 0);
 
-        res = observable.get_expectation_value(&state).real();
-        test_res = (test_state.adjoint() * test_observable * test_state);
-        ASSERT_NEAR(abs(test_res.real() - res) / res, 0, 0.01);
+    ASSERT_NEAR(res.imag(), 0, eps);
+    ASSERT_NEAR(test_res.imag(), 0, eps);
+
+    state.set_Haar_random_state();
+    for (ITYPE i = 0; i < dim; ++i) test_state[i] = state.data_cpp()[i];
+
+    res = observable.get_expectation_value(&state);
+    test_res = (test_state.adjoint() * test_observable * test_state)(0, 0);
+
+    test_state = test_circuit * test_state;
+    circuit.update_quantum_state(&state);
+
+    res = observable.get_expectation_value(&state);
+    test_res = (test_state.adjoint() * test_observable * test_state)(0, 0);
+
+    ASSERT_NEAR(abs(test_res.real() - res.real()) / test_res.real(), 0, 0.01);
+    ASSERT_NEAR(res.imag(), 0, eps);
+    ASSERT_NEAR(test_res.imag(), 0, eps);
+}
 
-        state.set_Haar_random_state(seed);
-        set_eigen_from_gpu(test_state, state, dim);
+TEST(CircuitTest_multicpu, SpecialGatesToString) {
+    QuantumState state(1, true);
+    QuantumCircuit c(1);
+    c.add_gate(gate::DepolarizingNoise(0, 0));
+    c.update_quantum_state(&state);
+    std::string s = c.to_string();
+}
 
-        test_state = test_circuit * test_state;
-        circuit.update_quantum_state(&state);
+TEST(CircuitTest_multicpu, MergeCircuits) {
+    QuantumState state(2, true);
+    QuantumCircuit circuit1(2), circuit2(2);
+    circuit1.add_X_gate(0);
+    circuit2.add_X_gate(1);
+    state.set_zero_state();
+    circuit1.merge_circuit(&circuit2);
+    circuit1.update_quantum_state(&state);
+    ASSERT_NEAR(abs(state.data_cpp()[3]), 1.0, 0.0001);
+}
 
-        res = observable.get_expectation_value(&state).real();
-        test_res = (test_state.adjoint() * test_observable * test_state);
-        ASSERT_NEAR(abs(test_res.real() - res) / res, 0, 0.01);
+void _PrintCircuit(QuantumCircuit* circuit) {
+    for (auto& gate : circuit->gate_list) {
+        auto t_index_list = gate->get_target_index_list();
+        auto c_index_list = gate->get_control_index_list();
+        std::cout << gate->get_name() << "(t:{";
+        for (auto idx : t_index_list) {
+            std::cout << idx << ",";
+        }
+        std::cout << "}, c:{";
+        for (auto idx : c_index_list) {
+            std::cout << idx << ",";
+        }
+        std::cout << "})" << std::endl;
     }
 }
 
-TEST(CircuitTest, RotateDiagonalObservable) {
-    CPPCTYPE J(0.0, 1.0);
-    Eigen::MatrixXcd Identity(2, 2), X(2, 2), Y(2, 2), Z(2, 2);
-    Identity << 1, 0, 0, 1;
-    X << 0, 1, 1, 0;
-    Y << 0, -J, J, 0;
-    Z << 1, 0, 0, -1;
+void _ApplyOptimizer(QuantumCircuit* circuit_ref, int opt_lv, UINT swap_lv,
+    UINT num_exp_outer_swaps) {
+    const UINT n = circuit_ref->qubit_count;
+    const ITYPE dim = 1ULL << n;
+
+    QuantumState state_ref(n);
+    QuantumState state(n, true);
+
+    MPIutil& m = MPIutil::get_inst();
+    const ITYPE inner_dim = dim >> state.outer_qc;
+    const ITYPE offs = inner_dim * m.get_rank();
 
-    const UINT n = 2;
-    const UINT dim = 1ULL << n;
+    {
+        state_ref.set_Haar_random_state(2022);
+        for (ITYPE i = 0; i < inner_dim; ++i)
+            state.data_cpp()[i] = state_ref.data_cpp()[(i + offs) % dim];
+
+        QuantumCircuit* circuit = circuit_ref->copy();
+        QuantumCircuitOptimizer qco;
+        if (opt_lv >= 0) {
+            qco.optimize(circuit, opt_lv, swap_lv);
+        } else {
+            qco.optimize_light(circuit, swap_lv);
+        }
+
+        circuit->update_quantum_state(&state);
+        circuit_ref->update_quantum_state(&state_ref);
+
+#if 0
+        if (m.get_rank() == 0) {
+            std::cout << "-----original circuit-----" << std::endl;
+            _PrintCircuit(circuit_ref);
+            std::cout << "-----optimized circuit-----" << std::endl;
+            _PrintCircuit(circuit);
+            std::cout << "---------------------------" << std::endl;
+        }
+#endif
+
+        // check if all target qubits are inner except for SWAP, FusedSWAP,
+        // and diagonal gate (e.g., CZ, RZ)
+        for (auto& gate : circuit->gate_list) {
+            auto gate_name = gate->get_name();
+            if (gate_name == "SWAP" || gate_name == "FusedSWAP" ||
+                gate_name == "I" || gate_name == "Z" ||
+                gate_name == "Z-rotation" || gate_name == "CZ" ||
+                gate_name == "Projection-0" || gate_name == "Projection-1" ||
+                gate_name == "S" || gate_name == "Sdag" || gate_name == "T" ||
+                gate_name == "Tdag" || gate_name == "DiagonalMatrix") {
+                continue;
+            }
+            auto t_index_list = gate->get_target_index_list();
+            for (auto idx : t_index_list) {
+                ASSERT_TRUE(idx < state.inner_qc);
+            }
+        }
+
+        // check the number of SWAP and FusedSWAP is the same with expected.
+        UINT num_outer_swap_gates = 0;
+        for (auto& gate : circuit->gate_list) {
+            if (gate->get_name() == "SWAP" || gate->get_name() == "FusedSWAP") {
+                auto t_index_list = gate->get_target_index_list();
+                for (auto idx : t_index_list) {
+                    if (idx >= state.inner_qc) {
+                        num_outer_swap_gates++;
+                        break;
+                    }
+                }
+            }
+        }
+
+#if 0
+        if (m.get_rank() == 0) {
+            std::cout << "num_outer_swap_gates=" << num_outer_swap_gates << std::endl;
+            std::cout << "num_exp_outer_swap_gates=" << num_exp_outer_swaps << std::endl;
+        }
+#endif
+        ASSERT_TRUE(num_outer_swap_gates <= num_exp_outer_swaps)
+            << "# outer swaps is " << num_outer_swap_gates
+            << ", but expected is " << num_exp_outer_swaps;
+
+        for (ITYPE i = 0; i < inner_dim; ++i)
+            ASSERT_NEAR(abs(state.data_cpp()[i] -
+                            state_ref.data_cpp()[(i + offs) % dim]),
+                0, eps)
+                << "[rank:" << m.get_rank() << "] Optimizer diff at " << i;
+
+        delete circuit;
+    }
+}
+
+TEST(CircuitTest_multicpu, FSWAPOptimizer_6qubits) {
+    UINT n = 6;
+
+    MPIutil& m = MPIutil::get_inst();
+    const UINT log_nodes = std::log2(m.get_size());
+    if (log_nodes == 0 || log_nodes > n - 2) {
+        return;
+    }
+    const UINT outer_qc = log_nodes;
+    const UINT inner_qc = n - log_nodes;
 
-    double angle, coef1, coef2;
     Random random;
+    {
+        random.set_seed(2022);
+        QuantumCircuit circuit(n);
+        circuit.add_RX_gate(0, random.uniform() * 3.14159);
+        circuit.add_RX_gate(n - 1, random.uniform() * 3.14159);
+        _ApplyOptimizer(&circuit, 0, 1, 2);
+    }
 
-    double res;
-    CPPCTYPE test_res;
+    if (inner_qc >= outer_qc * 2) {
+        random.set_seed(2022);
+        QuantumCircuit circuit(n);
+        for (UINT rep = 0; rep < 2; rep++) {
+            for (UINT i = 0; i < n; i++) {
+                circuit.add_H_gate(i);
+            }
+        }
+        // TODO gate順序変更に対応したら2回に変更
+        _ApplyOptimizer(&circuit, 0, 1, 4);
+    }
+
+    if (inner_qc >= outer_qc * 2) {
+        random.set_seed(2022);
+        QuantumCircuit circuit(n);
+        for (UINT rep = 0; rep < 2; rep++) {
+            for (UINT i = 0; i < n; i++) {
+                circuit.add_CNOT_gate(i, (i + 1) % n);
+            }
+        }
+        // TODO gate順序変更に対応したら2回に変更
+        _ApplyOptimizer(&circuit, 0, 1, 4);
+    }
+
+    if (outer_qc <= n / 2) {
+        random.set_seed(2022);
+        QuantumCircuit circuit(n);
+
+        // outer
+        for (UINT rep = 0; rep < n * 2; rep++) {
+            circuit.add_RX_gate(
+                inner_qc + (rep % outer_qc), random.uniform() * 3.14159);
+        }
+        // inner
+        for (UINT rep = 0; rep < n * 2; rep++) {
+            circuit.add_RX_gate((rep % inner_qc), random.uniform() * 3.14159);
+        }
+        // outer
+        for (UINT rep = 0; rep < n * 2; rep++) {
+            circuit.add_RX_gate(
+                inner_qc + (rep % outer_qc), random.uniform() * 3.14159);
+        }
+
+        _ApplyOptimizer(&circuit, 0, 1, 4);
+    }
+
+    {
+        random.set_seed(2022);
+        QuantumCircuit circuit(n);
 
-    int ngpus = get_num_device();
-    for (int idx = 0; idx < ngpus; ++idx) {
-        Observable observable(n);
-        Eigen::MatrixXcd test_observable;
+        for (UINT rep = 0; rep < n * 4; rep++) {
+            circuit.add_RX_gate(
+                ((UINT)(random.uniform() * n)) % n, random.uniform() * 3.14159);
+        }
 
-        QuantumStateGpu state(n, idx);
-        Eigen::VectorXcd test_state = Eigen::VectorXcd::Zero(dim);
+        _ApplyOptimizer(&circuit, 0, 1, n * 8);
+    }
 
+    if (inner_qc >= 3 && outer_qc >= 3) {
+        random.set_seed(2022);
         QuantumCircuit circuit(n);
-        Eigen::MatrixXcd test_circuit;
 
-        coef1 = -random.uniform();
-        coef2 = -random.uniform();
-        angle = 2 * PI * random.uniform();
+        circuit.add_H_gate(n - 1);
+        circuit.add_H_gate(n - 3);
+
+        _ApplyOptimizer(&circuit, 0, 1, 2);
+    }
+}
+
+TEST(CircuitTest_multicpu, FSWAPOptimizer_nocomm_6qubits) {
+    UINT n = 6;
+
+    MPIutil& m = MPIutil::get_inst();
+    const UINT log_nodes = std::log2(m.get_size());
+    if (log_nodes == 0 || log_nodes > n - 2) {
+        return;
+    }
+    const UINT outer_qc = log_nodes;
+    const UINT inner_qc = n - log_nodes;
+
+    Random random;
+
+    std::vector<int> block_sizes = {
+        0, (int)n, -1};  // -1 means using optimize_light
+    const UINT swap_lv = 1;
+    const UINT depth = 2;
+
+    for (auto block_size : block_sizes) {
+        // X, Yゲートはouter qubitを使わなければFSWAP不要
+        {
+            random.set_seed(2022);
+            QuantumCircuit circuit(n);
+            for (UINT d = 0; d < depth; d++) {
+                for (UINT i = 0; i < inner_qc; i++) {
+                    circuit.add_X_gate(i);
+                    circuit.add_Y_gate(i);
+                }
+            }
+            _ApplyOptimizer(&circuit, block_size, swap_lv, 0);
+        }
+        // CNOTゲートはtargetでouter qubitを使わなければFSWAP不要
+        {
+            random.set_seed(2022);
+            QuantumCircuit circuit(n);
+            for (UINT d = 0; d < depth; d++) {
+                for (UINT i = 0; i < n; i++) {
+                    if ((i + 1) % n < inner_qc) {
+                        circuit.add_CNOT_gate(i, (i + 1) % n);
+                    }
+                }
+            }
+            _ApplyOptimizer(&circuit, block_size, swap_lv, 0);
+        }
+        // Hゲートはouter qubitを使わなければFSWAP不要
+        {
+            random.set_seed(2022);
+            QuantumCircuit circuit(n);
+            for (UINT d = 0; d < depth; d++) {
+                for (UINT i = 0; i < inner_qc; i++) {
+                    circuit.add_H_gate(i);
+                }
+            }
+            _ApplyOptimizer(&circuit, block_size, swap_lv, 0);
+        }
+        // RX, RYゲートはouter qubitを使わなければFSWAP不要
+        {
+            random.set_seed(2022);
+            QuantumCircuit circuit(n);
+            for (UINT d = 0; d < depth; d++) {
+                for (UINT i = 0; i < inner_qc; i++) {
+                    circuit.add_RX_gate(i, random.uniform() * 3.14159);
+                    circuit.add_RY_gate(i, random.uniform() * 3.14159);
+                }
+            }
+            _ApplyOptimizer(&circuit, block_size, swap_lv, 0);
+        }
+        // SqrtX, SqrtXdag, SqrtY, SqrtYdagゲートはtargetでouter
+        // qubitを使わなければFSWAP不要
+        {
+            random.set_seed(2022);
+            QuantumCircuit circuit(n);
+            for (UINT d = 0; d < depth; d++) {
+                for (UINT i = 0; i < inner_qc; i++) {
+                    circuit.add_sqrtX_gate(i);
+                    circuit.add_sqrtXdag_gate(i);
+                    circuit.add_sqrtY_gate(i);
+                    circuit.add_sqrtYdag_gate(i);
+                }
+            }
+            _ApplyOptimizer(&circuit, block_size, swap_lv, 0);
+        }
+        // U1, U2, U3ゲートはtargetでouter qubitを使わなければFSWAP不要
+        {
+            random.set_seed(2022);
+            QuantumCircuit circuit(n);
+            for (UINT d = 0; d < depth; d++) {
+                for (UINT i = 0; i < inner_qc; i++) {
+                    circuit.add_U1_gate(i, random.uniform() * 3.14159);
+                    circuit.add_U2_gate(i, random.uniform() * 3.14159,
+                        random.uniform() * 3.14159);
+                    circuit.add_U3_gate(i, random.uniform() * 3.14159,
+                        random.uniform() * 3.14159, random.uniform() * 3.14159);
+                }
+            }
+            _ApplyOptimizer(&circuit, block_size, swap_lv, 0);
+        }
+        // DenseMatrixゲートはtargetでouter qubitを使わなければFSWAP不要
+        {
+            random.set_seed(2022);
+            QuantumCircuit circuit(n);
+            for (UINT d = 0; d < depth; d++) {
+                for (UINT i = 0; i < inner_qc; i++) {
+                    std::vector<UINT> target{i};
+                    ComplexMatrix mat =
+                        get_eigen_matrix_random_single_qubit_unitary();
+                    auto DenseMatrix_gate = gate::DenseMatrix(target, mat);
+                    circuit.add_gate(DenseMatrix_gate);
+                }
+            }
+            _ApplyOptimizer(&circuit, block_size, swap_lv, 0);
+        }
+        // Zゲートは全てのパターンでFSWAP不要
+        {
+            random.set_seed(2022);
+            QuantumCircuit circuit(n);
+            for (UINT d = 0; d < depth; d++) {
+                for (UINT i = 0; i < n; i++) {
+                    circuit.add_Z_gate(i);
+                }
+            }
+            _ApplyOptimizer(&circuit, block_size, swap_lv, 0);
+        }
+        // CZゲートは全てのパターンでFSWAP不要
+        {
+            random.set_seed(2022);
+            QuantumCircuit circuit(n);
+            for (UINT d = 0; d < depth; d++) {
+                for (UINT i = 0; i < n; i++) {
+                    circuit.add_CZ_gate(i, (i + 1) % n);
+                }
+            }
+            _ApplyOptimizer(&circuit, block_size, swap_lv, 0);
+        }
+        // Iゲートは全てのパターンでFSWAP不要
+        {
+            random.set_seed(2022);
+            QuantumCircuit circuit(n);
+            for (UINT d = 0; d < depth; d++) {
+                for (UINT i = 0; i < n; i++) {
+                    auto I_gate = gate::Identity(i);
+                    circuit.add_gate(I_gate);
+                }
+            }
+            _ApplyOptimizer(&circuit, block_size, swap_lv, 0);
+        }
+        // P0, P1ゲートは全てのパターンでFSWAP不要
+        {
+            random.set_seed(2022);
+            QuantumCircuit circuit(n);
+            for (UINT d = 0; d < depth; d++) {
+                for (UINT i = 0; i < n; i++) {
+                    circuit.add_P0_gate(i);
+                    circuit.add_P1_gate(i);
+                }
+            }
+            _ApplyOptimizer(&circuit, block_size, swap_lv, 0);
+        }
+        // RZゲートは全てのパターンでFSWAP不要
+        {
+            random.set_seed(2022);
+            QuantumCircuit circuit(n);
+            for (UINT d = 0; d < depth; d++) {
+                for (UINT i = 0; i < n; i++) {
+                    circuit.add_RZ_gate(i, random.uniform() * 3.14159);
+                }
+            }
+            _ApplyOptimizer(&circuit, block_size, swap_lv, 0);
+        }
+        // S, Sdag, T, Tdagゲートは全てのパターンでFSWAP不要
+        {
+            random.set_seed(2022);
+            QuantumCircuit circuit(n);
+            for (UINT d = 0; d < depth; d++) {
+                for (UINT i = 0; i < n; i++) {
+                    circuit.add_S_gate(i);
+                    circuit.add_Sdag_gate(i);
+                    circuit.add_T_gate(i);
+                    circuit.add_Tdag_gate(i);
+                }
+            }
+            _ApplyOptimizer(&circuit, block_size, swap_lv, 0);
+        }
+        // DiagonalMatrixゲートは全てのパターンでFSWAP不要
+        {
+            random.set_seed(2022);
+            QuantumCircuit circuit(n);
+            for (UINT d = 0; d < depth; d++) {
+                for (UINT i = 0; i < n; i++) {
+                    std::vector<UINT> target{i};
+                    ComplexVector diag =
+                        get_eigen_diagonal_matrix_random_multi_qubit_unitary(1);
+                    auto DiagonalMatrix_gate =
+                        gate::DiagonalMatrix(target, diag);
+                    circuit.add_gate(DiagonalMatrix_gate);
+                }
+            }
+            _ApplyOptimizer(&circuit, block_size, swap_lv, 0);
+        }
+    }
+}
+
+void _BuildQulacsBenchmark(
+    QuantumCircuit& circuit, UINT nqubits, UINT depth, Random& random) {
+    // first rotation
+    for (UINT k = 0; k < nqubits; k++) {
+        circuit.add_RX_gate(k, random.uniform() * 3.14159);
+        circuit.add_RZ_gate(k, random.uniform() * 3.14159);
+    }
+
+    // entangler
+    for (UINT k = 0; k < nqubits; k++) {
+        circuit.add_CNOT_gate(k, (k + 1) % nqubits);
+    }
+
+    for (UINT i = 0; i < depth; i++) {
+        // mid rotation
+        for (UINT k = 0; k < nqubits; k++) {
+            circuit.add_RZ_gate(k, random.uniform() * 3.14159);
+            circuit.add_RX_gate(k, random.uniform() * 3.14159);
+            circuit.add_RZ_gate(k, random.uniform() * 3.14159);
+        }
+
+        // entangler
+        for (UINT k = 0; k < nqubits; k++) {
+            circuit.add_CNOT_gate(k, (k + 1) % nqubits);
+        }
+    }
 
-        observable.add_operator(coef1, "Z 0");
-        observable.add_operator(coef2, "Z 0 Z 1");
+    // last rotation
+    for (UINT k = 0; k < nqubits; k++) {
+        circuit.add_RZ_gate(k, random.uniform() * 3.14159);
+        circuit.add_RX_gate(k, random.uniform() * 3.14159);
+    }
+}
 
-        test_observable =
-            coef1 * get_expanded_eigen_matrix_with_identity(0, Z, n);
-        test_observable += coef2 * kronecker_product(Z, Z);
+void _BuildQVolumeBenchmark(
+    QuantumCircuit& circuit, UINT nqubits, UINT depth, Random& random) {
+    for (UINT d = 0; d < depth; ++d) {
+        std::vector<UINT> index(nqubits), perm;
+        std::iota(index.begin(), index.end(), 0);  // [0, ..., nqubits-1]
+        for (UINT i = 0; i < nqubits; i++) {
+            auto p = index.begin() + random.int32() % index.size();
+            perm.push_back(*p);
+            index.erase(p);
+        }
 
-        circuit.add_diagonal_observable_rotation_gate(observable, angle);
-        test_circuit = (J * angle * test_observable).exp();
+        for (UINT w = 0; w < nqubits; w += 2) {
+            std::vector<UINT> target_qubits = {perm[w], perm[w + 1]};
+            circuit.add_random_unitary_gate(target_qubits, random.int32());
+        }
+    }
+}
 
-        state.set_computational_basis(0);
-        test_state(0) = 1.;
+TEST(CircuitTest_multicpu, FSWAPOptimizer_reorder_6qubits) {
+    UINT n = 6;
 
-        // for (ITYPE i = 0; i < dim; ++i) ASSERT_NEAR(abs(test_state[i] -
-        // state.data_cpp()[i]), 0, eps);
+    MPIutil& m = MPIutil::get_inst();
+    const UINT log_nodes = std::log2(m.get_size());
+    if (log_nodes == 0 || log_nodes > n - 2) {
+        return;
+    }
+    const UINT outer_qc = log_nodes;
+    const UINT inner_qc = n - log_nodes;
 
-        circuit.update_quantum_state(&state);
-        test_state = test_circuit * test_state;
+    Random random;
 
-        res = observable.get_expectation_value(&state).real();
-        test_res = (test_state.adjoint() * test_observable * test_state);
+    std::vector<int> block_sizes = {0, (int)n, -1};
 
-        // for (ITYPE i = 0; i < dim; ++i) ASSERT_NEAR(abs(test_state[i] -
-        // state.data_cpp()[i]), 0, eps);
-        ASSERT_NEAR(abs(test_res.real() - res) / test_res.real(), 0, 0.01);
-        ASSERT_NEAR(test_res.imag(), 0, eps);
+    // Qulacs Benchmark
+    for (int block_size : block_sizes) {
+        random.set_seed(2022);
+        QuantumCircuit circuit(n);
+        _BuildQulacsBenchmark(circuit, n, 9, random);
+        UINT n_expected_swaps = 0;
+        switch (outer_qc) {
+            case 1:
+                n_expected_swaps = 14;
+                break;
+            case 2:
+                n_expected_swaps = 18;
+                break;
+            case 3:
+                n_expected_swaps = 23;
+                break;
+            case 4:
+                n_expected_swaps = 68;
+                break;
+        }
+        _ApplyOptimizer(&circuit, block_size, 2, n_expected_swaps);
+    }
 
-        state.set_Haar_random_state();
-        set_eigen_from_gpu(test_state, state, dim);
+    // QVolume Benchmark
+    for (int block_size : block_sizes) {
+        random.set_seed(2022);
+        QuantumCircuit circuit(n);
+        _BuildQVolumeBenchmark(circuit, n, 10, random);
+        UINT n_expected_swaps = 0;
+        switch (outer_qc) {
+            case 1:
+                n_expected_swaps = 6;
+                break;
+            case 2:
+                n_expected_swaps = 9;
+                break;
+            case 3:
+                n_expected_swaps = 21;
+                break;
+            case 4:
+                n_expected_swaps = 38;
+                break;
+        }
+        _ApplyOptimizer(&circuit, 0, 2, n_expected_swaps);
+    }
 
-        res = observable.get_expectation_value(&state).real();
-        test_res = (test_state.adjoint() * test_observable * test_state);
+    // check for a reorder bug
+    if (outer_qc == 1) {
+        random.set_seed(2022);
+        QuantumCircuit circuit(n);
+        for (UINT i = 0; i < n; i++) {
+            circuit.add_RX_gate(i, random.uniform() * 3.14159);
+        }
+        {
+            QuantumGateBase* merged_gates =
+                gate::RY(0, random.uniform() * 3.14159);
+            for (UINT i = 1; i + 1 < n; i++) {
+                merged_gates = gate::merge(
+                    merged_gates, gate::RY(i, random.uniform() * 3.14159));
+            }
+            circuit.add_gate(merged_gates);
+        }
+        circuit.add_RY_gate(n - 1, random.uniform() * 3.14159);
+        {
+            QuantumGateBase* merged_gates =
+                gate::RZ(0, random.uniform() * 3.14159);
+            for (UINT i = 1; i + 1 < n; i++) {
+                merged_gates = gate::merge(
+                    merged_gates, gate::RZ(i, random.uniform() * 3.14159));
+            }
+            circuit.add_gate(merged_gates);
+        }
+
+        _ApplyOptimizer(&circuit, 0, 2, 2);
+    }
+}
+
+TEST(CircuitTest_multicpu, FSWAPOptimizer_global_control) {
+    UINT n = 6;
+
+    MPIutil& m = MPIutil::get_inst();
+    const UINT log_nodes = std::log2(m.get_size());
+    if (log_nodes == 0 || log_nodes > n - 2) {
+        return;
+    }
+    const UINT outer_qc = log_nodes;
+    const UINT inner_qc = n - log_nodes;
 
-        test_state = test_circuit * test_state;
-        circuit.update_quantum_state(&state);
+    {
+        QuantumCircuit circuit(n);
+        circuit.add_X_gate(0);
+        circuit.add_CNOT_gate(n - 1, 0);
+
+        // expect that gates are not merged
+        _ApplyOptimizer(&circuit, -1, 2, 0);
+    }
+
+    {
+        QuantumCircuit circuit(n);
+        // TOFFOLI(n-1, 1, 0)
+        auto ptr = gate::X(0);
+        auto toffoli = gate::to_matrix_gate(ptr);
+        toffoli->add_control_qubit(n - 1, 1);
+        toffoli->add_control_qubit(1, 1);
+        delete ptr;
+        circuit.add_gate(toffoli);
+        // CNOT(n-1, 0)
+        circuit.add_CNOT_gate(n - 1, 0);
+
+        // expect that gates are merged to
+        // DenseMatrix(target=[0, 1], control=[n-1])
+        _ApplyOptimizer(&circuit, -1, 2, 0);
+    }
 
-        res = observable.get_expectation_value(&state).real();
-        test_res = (test_state.adjoint() * test_observable * test_state);
+    {
+        QuantumCircuit circuit(n);
+        // TOFFOLI(n-1, 1, 0)
+        auto ptr = gate::X(0);
+        auto toffoli = gate::to_matrix_gate(ptr);
+        toffoli->add_control_qubit(n - 1, 1);
+        toffoli->add_control_qubit(1, 1);
+        delete ptr;
+        circuit.add_gate(toffoli);
+        // CNOT(1, 0)
+        circuit.add_CNOT_gate(1, 0);
 
-        // for (ITYPE i = 0; i < dim; ++i) ASSERT_NEAR(abs(test_state[i] -
-        // state.data_cpp()[i]), 0, eps);
-        ASSERT_NEAR(abs(test_res.real() - res) / test_res.real(), 0, 0.01);
-        ASSERT_NEAR(test_res.imag(), 0, eps);
+        // expect that gates are not merged
+        _ApplyOptimizer(&circuit, -1, 2, 0);
     }
 }
 
-TEST(CircuitTest, SpecialGatesToString) {
-    int ngpus = get_num_device();
-    for (int idx = 0; idx < ngpus; ++idx) {
-        set_device(idx);
-        QuantumStateGpu state(1, idx);
-        QuantumCircuit c(1);
-        c.add_gate(gate::DepolarizingNoise(0, 0));
-        c.update_quantum_state(&state);
-        std::string s = c.to_string();
+TEST(CircuitTest_multicpu, FSWAPOptimizer_with_mpisize) {
+    UINT n = 6;
+
+    QuantumCircuit circuit(n);
+    for (UINT k = 0; k < n; k++) {
+        circuit.add_H_gate(k);
+        circuit.add_X_gate(k);
+    }
+
+    QuantumCircuitOptimizer qco(4);
+    qco.optimize(&circuit, 2, 2);
+
+    bool has_swap_gate = false;
+    for (auto& gate : circuit.gate_list) {
+        auto gate_name = gate->get_name();
+        if (gate_name == "FusedSWAP") {
+            has_swap_gate = true;
+        }
     }
+    ASSERT_TRUE(has_swap_gate)
+        << "circuit optimized with mpi_size=4 should have FusedSWAP gates";
 }
+#endif
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qulacs-0.6.2/test/gpusim/test_compat_cpu.cpp` & `qulacs-0.6.3/test/gpusim/test_compat_cpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/gpusim/test_func_memory.cpp` & `qulacs-0.6.3/test/gpusim/test_func_memory.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/gpusim/test_gate.cpp` & `qulacs-0.6.3/test/gpusim/test_gate.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     for (ITYPE i = 0; i < dim; ++i) dst[i] = ptr[i];
     free(ptr);
 }
 
 inline void assert_eigen_eq_gpu(
     ComplexVector& v1, QuantumStateGpu& v2, ITYPE dim, double eps) {
     auto ptr = v2.duplicate_data_cpp();
-    for (UINT i = 0; i < dim; ++i) {
+    for (ITYPE i = 0; i < dim; ++i) {
         ASSERT_NEAR(ptr[i].real(), v1[i].real(), eps);
         ASSERT_NEAR(ptr[i].imag(), v1[i].imag(), eps);
     }
     free(ptr);
 }
 
 inline void assert_cpu_eq_gpu(QuantumStateCpu& state_cpu,
```

### Comparing `qulacs-0.6.2/test/gpusim/test_hamiltonian.cpp` & `qulacs-0.6.3/test/gpusim/test_hamiltonian.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/gpusim/test_state.cpp` & `qulacs-0.6.3/test/gpusim/test_state.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     for (ITYPE i = 0; i < dim; ++i) dst[i] = ptr[i];
     free(ptr);
 }
 
 inline void assert_vector_eq_gpu(std::vector<std::complex<double>>& v1,
     QuantumStateGpu& v2, ITYPE dim, double eps) {
     auto ptr = v2.duplicate_data_cpp();
-    for (UINT i = 0; i < dim; ++i) {
+    for (ITYPE i = 0; i < dim; ++i) {
         ASSERT_NEAR(ptr[i].real(), v1[i].real(), eps);
         ASSERT_NEAR(ptr[i].imag(), v1[i].imag(), eps);
     }
     free(ptr);
 }
 
 inline void assert_cpu_eq_gpu(QuantumStateCpu& state_cpu,
@@ -944,15 +944,15 @@
 TEST(StateTest, SetState) {
     const UINT n = 10;
     int ngpus = get_num_device();
     for (int idx = 0; idx < ngpus; ++idx) {
         QuantumStateGpu state(n, idx);
         const ITYPE dim = 1ULL << n;
         std::vector<std::complex<double>> state_vector(dim);
-        for (UINT i = 0; i < dim; ++i) {
+        for (ITYPE i = 0; i < dim; ++i) {
             double d = (double)i;
             state_vector[i] = d + std::complex<double>(0, 1) * (d + 0.1);
         }
         state.load(state_vector);
 
         assert_vector_eq_gpu(state_vector, state, dim, eps);
     }
@@ -969,15 +969,15 @@
         const ITYPE dim = 1ULL << n;
         void* state_gpu = allocate_quantum_state_host(dim, idx);
         copy_quantum_state_from_host_to_device(
             state_gpu, state.data(), dim, stream_ptr, idx);
         CPPCTYPE* state_cpu_copy = (CPPCTYPE*)malloc(sizeof(CPPCTYPE) * dim);
         get_quantum_state_host(state_gpu, state_cpu_copy, dim, stream_ptr, idx);
 
-        for (UINT i = 0; i < dim; ++i) {
+        for (ITYPE i = 0; i < dim; ++i) {
             ASSERT_NEAR(
                 state.data_cpp()[i].real(), state_cpu_copy[i].real(), eps);
             ASSERT_NEAR(
                 state.data_cpp()[i].imag(), state_cpu_copy[i].imag(), eps);
         }
         release_quantum_state_host(state_gpu, idx);
     }
@@ -1001,15 +1001,15 @@
         get_quantum_state_host(
             state1_gpu, state1_cpu_copy, dim, stream_ptr, idx);
         copy_quantum_state_from_device_to_device(
             state2_gpu, state1_gpu, dim, stream_ptr, idx);
         get_quantum_state_host(
             state2_gpu, state2_cpu_copy, dim, stream_ptr, idx);
 
-        for (UINT i = 0; i < dim; ++i) {
+        for (ITYPE i = 0; i < dim; ++i) {
             ASSERT_NEAR(
                 state1_cpu_copy[i].real(), state2_cpu_copy[i].real(), eps);
             ASSERT_NEAR(
                 state1_cpu_copy[i].imag(), state2_cpu_copy[i].imag(), eps);
         }
         release_quantum_state_host(state1_gpu, idx);
         release_quantum_state_host(state2_gpu, idx);
```

### Comparing `qulacs-0.6.2/test/gpusim/test_update_control.cpp` & `qulacs-0.6.3/test/gpusim/test_update_control.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/gpusim/test_update_dense.cpp` & `qulacs-0.6.3/test/gpusim/test_update_dense.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/gpusim/test_update_diagonal.cpp` & `qulacs-0.6.3/test/gpusim/test_update_diagonal.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/gpusim/test_update_named.cpp` & `qulacs-0.6.3/test/gpusim/test_update_named.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/gpusim/test_update_pauli.cpp` & `qulacs-0.6.3/test/gpusim/test_update_pauli.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/gpusim/test_util.hpp` & `qulacs-0.6.3/test/gpusim/test_util.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/util/util.hpp` & `qulacs-0.6.3/test/util/util.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/vqcsim/test.cpp` & `qulacs-0.6.3/test/vqcsim/test.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.2/test/vqcsim/test_backprop.cpp` & `qulacs-0.6.3/test/vqcsim/test_backprop.cpp`

 * *Files identical despite different names*

