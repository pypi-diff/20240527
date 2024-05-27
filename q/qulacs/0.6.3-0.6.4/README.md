# Comparing `tmp/qulacs-0.6.3.tar.gz` & `tmp/qulacs-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qulacs-0.6.3.tar", last modified: Mon Dec 25 09:28:15 2023, max compression
+gzip compressed data, was "qulacs-0.6.4.tar", last modified: Mon May 27 09:46:13 2024, max compression
```

## Comparing `qulacs-0.6.3.tar` & `qulacs-0.6.4.tar`

### file list

```diff
@@ -1,453 +1,443 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.446617 qulacs-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-12-25 09:27:50.000000 qulacs-0.6.3/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.386617 qulacs-0.6.3/.devcontainer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.394616 qulacs-0.6.3/.devcontainer/cpu/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-12-25 09:27:50.000000 qulacs-0.6.3/.devcontainer/cpu/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2023-12-25 09:27:50.000000 qulacs-0.6.3/.devcontainer/cpu/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.394616 qulacs-0.6.3/.devcontainer/gpu/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-12-25 09:27:50.000000 qulacs-0.6.3/.devcontainer/gpu/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2023-12-25 09:27:50.000000 qulacs-0.6.3/.devcontainer/gpu/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.386617 qulacs-0.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.394616 qulacs-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2023-12-25 09:27:50.000000 qulacs-0.6.3/.github/workflows/ci_macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2023-12-25 09:27:50.000000 qulacs-0.6.3/.github/workflows/ci_ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-12-25 09:27:50.000000 qulacs-0.6.3/.github/workflows/ci_windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2023-12-25 09:27:50.000000 qulacs-0.6.3/.github/workflows/wheel.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-12-25 09:27:50.000000 qulacs-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-25 09:27:50.000000 qulacs-0.6.3/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.394616 qulacs-0.6.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2023-12-25 09:27:50.000000 qulacs-0.6.3/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)    16670 2023-12-25 09:27:50.000000 qulacs-0.6.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2023-12-25 09:27:50.000000 qulacs-0.6.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-25 09:27:50.000000 qulacs-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14080 2023-12-25 09:28:15.446617 qulacs-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11068 2023-12-25 09:27:50.000000 qulacs-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    11409 2023-12-25 09:27:50.000000 qulacs-0.6.3/README_MPI.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-25 09:27:50.000000 qulacs-0.6.3/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.394616 qulacs-0.6.3/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/AdaptiveGate.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/bench_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/benchmark2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/causalconetest.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/benchmark/circuits/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/circuits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/circuits/quantumvolume.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/circuits/qulacsbench.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/libcppsim_benchmark.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    17638 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/libcsim_benchmark.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      308 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/merge_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/test_qulacs_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-12-25 09:27:50.000000 qulacs-0.6.3/benchmark/test_qulacs_2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/cmake_script/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/cmake_script/FetchContent/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-25 09:27:50.000000 qulacs-0.6.3/cmake_script/FetchContent/CMakeLists.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)    38023 2023-12-25 09:27:50.000000 qulacs-0.6.3/cmake_script/FetchContent.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2023-12-25 09:27:50.000000 qulacs-0.6.3/cmake_script/FindAVX2.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      975 2023-12-25 09:27:50.000000 qulacs-0.6.3/cmake_script/FindSVE.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-25 09:27:50.000000 qulacs-0.6.3/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/doc/en/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/doc/en/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.386617 qulacs-0.6.3/doc/en/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/doc/en/source/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_static/images/dojo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_static/images/github.png
--rw-r--r--   0 runner    (1001) docker     (127)    54241 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_static/images/logo-c-h.png
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_static/images/slack.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/doc/en/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/doc/en/source/_templates/autoapi/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/macros.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.398617 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/exception.rst
--rw-r--r--   0 runner    (1001) docker     (127)      652 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)      704 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/method.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/package.rst
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/autoapi/python/property.rst
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/_templates/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/en/source/apply/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/apply/0_overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   162833 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/apply/5.2_qcl.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    30093 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/apply/6.2_vqe.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    55651 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/apply/6.3_ssvqe.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/en/source/apply/img/
--rw-r--r--   0 runner    (1001) docker     (127)    59895 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/apply/img/QCL.png
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/en/source/guide/
--rw-r--r--   0 runner    (1001) docker     (127)   158374 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/guide/2.0_python_advanced.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/en/source/intro/
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/intro/0_about.md
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/intro/1_install.md
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/intro/2_faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/intro/3_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)    27329 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/intro/4.1_python_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    26841 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/intro/4.2_cpp_tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/en/source/write/
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/en/source/write/0_readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/ja/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.386617 qulacs-0.6.3/doc/ja/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/ja/source/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_static/images/dojo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_static/images/github.png
--rw-r--r--   0 runner    (1001) docker     (127)    54241 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_static/images/logo-c-h.png
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_static/images/slack.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/ja/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.402617 qulacs-0.6.3/doc/ja/source/_templates/autoapi/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/macros.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.406617 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/exception.rst
--rw-r--r--   0 runner    (1001) docker     (127)      652 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)      704 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/method.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/package.rst
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/property.rst
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.406617 qulacs-0.6.3/doc/ja/source/guide/
--rw-r--r--   0 runner    (1001) docker     (127)    79037 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/guide/2.0_python_advanced.md
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.406617 qulacs-0.6.3/doc/ja/source/intro/
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/intro/0_about.md
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/intro/1_install.md
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/intro/2_faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/intro/3_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)    14702 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/intro/4.1_python_tutorial.md
--rw-r--r--   0 runner    (1001) docker     (127)    27502 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/ja/source/intro/4.2_cpp_tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.406617 qulacs-0.6.3/doc/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/scripts/customdoxygen.css
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/scripts/doxy-boot.js
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/scripts/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/scripts/header.html
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2023-12-25 09:27:50.000000 qulacs-0.6.3/doc/scripts/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2023-12-25 09:27:50.000000 qulacs-0.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.390617 qulacs-0.6.3/pysrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.406617 qulacs-0.6.3/pysrc/qulacs/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36717 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-25 09:28:15.000000 qulacs-0.6.3/pysrc/qulacs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/circuit/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/circuit/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/circuit/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      804 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/circuit.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/converter/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13126 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/converter/qasm_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/gate/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/gate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/gate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/gate/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10882 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/gate.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/observable/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/observable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/observable/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/observable/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/observable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/quantum_operator/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/quantum_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/quantum_operator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/quantum_operator/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/quantum_operator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/state/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/state/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/state/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/state.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/utils/conversions_openfermion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/vistest/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/vistest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/vistest/test_vis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/pysrc/qulacs/visualizer/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2023-12-25 09:27:50.000000 qulacs-0.6.3/pysrc/qulacs/visualizer/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.446617 qulacs-0.6.3/pysrc/qulacs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14080 2023-12-25 09:28:15.000000 qulacs-0.6.3/pysrc/qulacs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12305 2023-12-25 09:28:15.000000 qulacs-0.6.3/pysrc/qulacs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-25 09:28:15.000000 qulacs-0.6.3/pysrc/qulacs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-25 09:28:15.000000 qulacs-0.6.3/pysrc/qulacs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-25 09:28:15.000000 qulacs-0.6.3/pysrc/qulacs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-25 09:28:15.000000 qulacs-0.6.3/pysrc/qulacs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/python/
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    75995 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/cppsim_wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/python/stub-test/
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/stub-test/generate_mypy_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.410617 qulacs-0.6.3/python/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.414617 qulacs-0.6.3/python/tests/multi_cpu/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/multi_cpu/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/multi_cpu/test_circuit_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/multi_cpu/test_state_multi_cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.414617 qulacs-0.6.3/python/tests/single_cpu/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_density_matrix_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    12303 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_noise_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_observable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)    17686 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_pointer_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_qasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2023-12-25 09:27:50.000000 qulacs-0.6.3/python/tests/single_cpu/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.418617 qulacs-0.6.3/script/
--rwxr-xr-x   0 runner    (1001) docker     (127)      303 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_clang.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      691 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_gcc.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      440 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_gcc_with_gpu.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      441 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_gcc_with_memory_sanitizer.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      122 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_mpicc.sh
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_msvc_2015.bat
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_msvc_2015_with_gpu.bat
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_msvc_2017.bat
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_msvc_2017_with_gpu.bat
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_msvc_2019.bat
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/build_msvc_2019_with_gpu.bat
--rwxr-xr-x   0 runner    (1001) docker     (127)      127 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/clean.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/download_wheel.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      318 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/fix_wheel_osx.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      141 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/format.sh
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/generate_msvc_project_2015.bat
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/generate_msvc_project_2015_with_gpu.bat
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/generate_msvc_project_2017.bat
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/generate_msvc_project_2017_with_gpu.bat
--rwxr-xr-x   0 runner    (1001) docker     (127)      166 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/generate_msvc_project_2019.bat
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/generate_msvc_project_2019_with_gpu.bat
--rwxr-xr-x   0 runner    (1001) docker     (127)      430 2023-12-25 09:27:50.000000 qulacs-0.6.3/script/update_stubs.sh
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-12-25 09:28:15.446617 qulacs-0.6.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5242 2023-12-25 09:27:50.000000 qulacs-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.418617 qulacs-0.6.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.426617 qulacs-0.6.3/src/cppsim/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21217 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/circuit.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    24688 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/circuit.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/circuit_builder.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    33866 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/circuit_optimizer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/circuit_optimizer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9609 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/exception.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    32399 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19956 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_factory.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    24644 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_general.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13445 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_matrix_diagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_matrix_diagonal.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_matrix_sparse.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_matrix_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20532 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_merge.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_merge.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_named_npair.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_named_one.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    16353 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_named_one.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7977 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_named_pauli.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8986 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_named_two.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23276 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_noisy_evolution.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12950 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_noisy_evolution.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_reflect.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_reversible.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/gate_to_gqo.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    36921 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/general_quantum_operator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14781 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/general_quantum_operator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14140 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/matrix_decomposition.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7033 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/noisesimulator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/noisesimulator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13716 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/observable.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/observable.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14801 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/pauli_operator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/pauli_operator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      830 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/qubit_info.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7181 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/qubit_info.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/qubit_table.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/qubit_table.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/simulator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/simulator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/state.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    34497 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/state.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5116 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/state_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/state_dm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/state_gpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15703 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/state_gpu.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/type.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10550 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/utility.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/cppsim/utility.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.430617 qulacs-0.6.3/src/csim/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7145 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/MPIutil.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/MPIutil.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/constant.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/constant.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/init_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/init_ops_fill.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/init_ops_random.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/memory_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/memory_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/memory_ops_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/memory_ops_dm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/stat_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/stat_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10432 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/stat_ops_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/stat_ops_dm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    30440 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/stat_ops_expectation_value.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/stat_ops_probability.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/stat_ops_transition_amplitude.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/type.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    60932 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7802 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_control_multi_target_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14209 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_control_multi_target_single.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_control_single_target_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19452 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_control_single_target_single.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    34691 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_dm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    82604 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_matrix_dense_double.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_matrix_dense_double_eigen.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_matrix_dense_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_matrix_dense_multi_eigen.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    17967 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_matrix_dense_single.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_matrix_diagonal_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_matrix_diagonal_single.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_matrix_phase_single.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_CNOT.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_CZ.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12677 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_FusedSWAP.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_H.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_SWAP.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_X.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9384 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_Y.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_Z.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_projection.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_named_state.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    16633 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_pauli_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_pauli_single.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_qft.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      705 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_reflection.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/update_ops_reversible_boolean.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/utility.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/csim/utility.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.434617 qulacs-0.6.3/src/gpusim/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/memory_ops.cu
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/memory_ops.h
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/memory_ops_device_functions.h
--rw-r--r--   0 runner    (1001) docker     (127)    52450 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/stat_ops.cu
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/stat_ops.h
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/stat_ops_device_functions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/update_ops_cuda.h
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/update_ops_cuda_device_functions.h
--rw-r--r--   0 runner    (1001) docker     (127)    69614 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/update_ops_multi.cu
--rw-r--r--   0 runner    (1001) docker     (127)    21139 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/update_ops_named.cu
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/update_ops_single.cu
--rw-r--r--   0 runner    (1001) docker     (127)    24452 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/util.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/util.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/util.h
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/util_common.h
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/util_export.h
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/util_func.h
--rw-r--r--   0 runner    (1001) docker     (127)      359 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/util_type.h
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/gpusim/util_type_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.438617 qulacs-0.6.3/src/vqcsim/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/GradCalculator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      408 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/GradCalculator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      730 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/boolean_formula.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/causalcone_simulator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/differential.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/differential.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/loss_function.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/loss_function.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/optimizer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14300 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parametric_circuit.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parametric_circuit.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parametric_circuit_builder.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parametric_gate.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parametric_gate_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      823 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parametric_gate_factory.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parametric_simulator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      603 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parametric_simulator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/parser.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/problem.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2023-12-25 09:27:50.000000 qulacs-0.6.3/src/vqcsim/solver.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.438617 qulacs-0.6.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.442617 qulacs-0.6.3/test/cppsim/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/H2.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_KAK.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    32101 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_circuit.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    54983 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_circuit_multicpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9942 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_circuit_optimize_light.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    57300 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_gate.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    29782 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_gate_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    58304 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_gate_multicpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    23845 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_hamiltonian.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_hamiltonian_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15636 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_hamiltonian_multicpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_mpiutil_multicpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12025 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_noise_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_noisesimulator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    20764 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_noisyevolution.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_pauli_operator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_simulator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11552 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_state.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11267 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_state_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/cppsim/test_state_multicpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.442617 qulacs-0.6.3/test/csim/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_memory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_omputil.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    26768 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_stat.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10235 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_update_control.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_update_dense.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_update_dense_double.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_update_diagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_update_diagonal_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13376 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_update_named.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6955 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/csim/test_update_pauli.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.442617 qulacs-0.6.3/test/gpusim/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      492 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/H2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    33346 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_circuit.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9054 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_compat_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_func_memory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    47173 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_gate.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9409 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_hamiltonian.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    43547 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_state.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8633 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_update_control.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15382 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_update_dense.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_update_diagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10371 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_update_named.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_update_pauli.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/gpusim/test_util.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.446617 qulacs-0.6.3/test/util/
--rw-r--r--   0 runner    (1001) docker     (127)    13090 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/util/util.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 09:28:15.446617 qulacs-0.6.3/test/vqcsim/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/vqcsim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/vqcsim/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    17741 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/vqcsim/test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2023-12-25 09:27:50.000000 qulacs-0.6.3/test/vqcsim/test_backprop.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.775196 qulacs-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-27 09:43:30.000000 qulacs-0.6.4/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.703195 qulacs-0.6.4/.devcontainer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.711196 qulacs-0.6.4/.devcontainer/cpu/
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-27 09:43:30.000000 qulacs-0.6.4/.devcontainer/cpu/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-27 09:43:30.000000 qulacs-0.6.4/.devcontainer/cpu/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.711196 qulacs-0.6.4/.devcontainer/gpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 09:43:30.000000 qulacs-0.6.4/.devcontainer/gpu/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-27 09:43:30.000000 qulacs-0.6.4/.devcontainer/gpu/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.703195 qulacs-0.6.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.711196 qulacs-0.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-27 09:43:30.000000 qulacs-0.6.4/.github/workflows/ci_macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-05-27 09:43:30.000000 qulacs-0.6.4/.github/workflows/ci_ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-27 09:43:30.000000 qulacs-0.6.4/.github/workflows/ci_windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-27 09:43:30.000000 qulacs-0.6.4/.github/workflows/wheel.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-27 09:43:30.000000 qulacs-0.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-27 09:43:30.000000 qulacs-0.6.4/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.711196 qulacs-0.6.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-27 09:43:30.000000 qulacs-0.6.4/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16670 2024-05-27 09:43:30.000000 qulacs-0.6.4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-27 09:43:30.000000 qulacs-0.6.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-27 09:43:30.000000 qulacs-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-27 09:46:13.775196 qulacs-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-05-27 09:43:30.000000 qulacs-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-05-27 09:43:30.000000 qulacs-0.6.4/README_MPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 09:43:30.000000 qulacs-0.6.4/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.715196 qulacs-0.6.4/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-27 09:43:30.000000 qulacs-0.6.4/benchmark/AdaptiveGate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-27 09:43:30.000000 qulacs-0.6.4/benchmark/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-27 09:43:30.000000 qulacs-0.6.4/benchmark/bench_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-27 09:43:30.000000 qulacs-0.6.4/benchmark/benchmark2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-27 09:43:30.000000 qulacs-0.6.4/benchmark/causalconetest.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.715196 qulacs-0.6.4/benchmark/circuits/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-27 09:43:30.000000 qulacs-0.6.4/benchmark/circuits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-27 09:43:30.000000 qulacs-0.6.4/benchmark/circuits/quantumvolume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-27 09:43:30.000000 qulacs-0.6.4/benchmark/circuits/qulacsbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-27 09:43:30.000000 qulacs-0.6.4/benchmark/libcppsim_benchmark.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17638 2024-05-27 09:43:30.000000 qulacs-0.6.4/benchmark/libcsim_benchmark.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-27 09:43:30.000000 qulacs-0.6.4/benchmark/merge_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-27 09:43:30.000000 qulacs-0.6.4/benchmark/test_qulacs_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-27 09:43:30.000000 qulacs-0.6.4/benchmark/test_qulacs_2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.715196 qulacs-0.6.4/cmake_script/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.715196 qulacs-0.6.4/cmake_script/FetchContent/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-27 09:43:30.000000 qulacs-0.6.4/cmake_script/FetchContent/CMakeLists.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)    38023 2024-05-27 09:43:30.000000 qulacs-0.6.4/cmake_script/FetchContent.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-27 09:43:30.000000 qulacs-0.6.4/cmake_script/FindAVX2.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-27 09:43:30.000000 qulacs-0.6.4/cmake_script/FindSVE.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-27 09:43:30.000000 qulacs-0.6.4/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.715196 qulacs-0.6.4/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.715196 qulacs-0.6.4/doc/en/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.715196 qulacs-0.6.4/doc/en/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.703195 qulacs-0.6.4/doc/en/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.719195 qulacs-0.6.4/doc/en/source/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/_static/images/dojo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/_static/images/github.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54241 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/_static/images/logo-c-h.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/_static/images/slack.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.719195 qulacs-0.6.4/doc/en/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.719195 qulacs-0.6.4/doc/en/source/_templates/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/_templates/autoapi/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/_templates/autoapi/macros.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.719195 qulacs-0.6.4/doc/en/source/_templates/autoapi/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/_templates/autoapi/python/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/_templates/autoapi/python/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/_templates/autoapi/python/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/_templates/autoapi/python/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/_templates/autoapi/python/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/_templates/autoapi/python/method.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/_templates/autoapi/python/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/_templates/autoapi/python/package.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/_templates/autoapi/python/property.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/_templates/footer.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.719195 qulacs-0.6.4/doc/en/source/apply/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/apply/0_overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   162833 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/apply/5.2_qcl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30083 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/apply/6.2_vqe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    55651 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/apply/6.3_ssvqe.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.719195 qulacs-0.6.4/doc/en/source/apply/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    59895 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/apply/img/QCL.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.719195 qulacs-0.6.4/doc/en/source/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)   160276 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/guide/2.0_python_advanced.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.723195 qulacs-0.6.4/doc/en/source/intro/
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/intro/0_about.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/intro/1_install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/intro/2_faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/intro/3_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)    33847 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/intro/4.1_python_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    26841 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/intro/4.2_cpp_tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.723195 qulacs-0.6.4/doc/en/source/write/
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/en/source/write/0_readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.723195 qulacs-0.6.4/doc/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.723195 qulacs-0.6.4/doc/ja/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.703195 qulacs-0.6.4/doc/ja/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.723195 qulacs-0.6.4/doc/ja/source/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/_static/images/dojo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/_static/images/github.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54241 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/_static/images/logo-c-h.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/_static/images/slack.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.723195 qulacs-0.6.4/doc/ja/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.723195 qulacs-0.6.4/doc/ja/source/_templates/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/_templates/autoapi/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/_templates/autoapi/macros.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.727196 qulacs-0.6.4/doc/ja/source/_templates/autoapi/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/_templates/autoapi/python/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/_templates/autoapi/python/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/_templates/autoapi/python/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/_templates/autoapi/python/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/_templates/autoapi/python/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/_templates/autoapi/python/method.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/_templates/autoapi/python/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/_templates/autoapi/python/package.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/_templates/autoapi/python/property.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.727196 qulacs-0.6.4/doc/ja/source/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)    80376 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/guide/2.0_python_advanced.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.727196 qulacs-0.6.4/doc/ja/source/intro/
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/intro/0_about.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/intro/1_install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/intro/2_faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/intro/3_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19094 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/intro/4.1_python_tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)    27502 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/ja/source/intro/4.2_cpp_tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.727196 qulacs-0.6.4/doc/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/scripts/customdoxygen.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/scripts/doxy-boot.js
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/scripts/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/scripts/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-27 09:43:30.000000 qulacs-0.6.4/doc/scripts/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-27 09:43:30.000000 qulacs-0.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.707195 qulacs-0.6.4/pysrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.727196 qulacs-0.6.4/pysrc/qulacs/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-27 09:43:30.000000 qulacs-0.6.4/pysrc/qulacs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36775 2024-05-27 09:46:08.000000 qulacs-0.6.4/pysrc/qulacs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 09:46:13.000000 qulacs-0.6.4/pysrc/qulacs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.731196 qulacs-0.6.4/pysrc/qulacs/circuit/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 09:43:30.000000 qulacs-0.6.4/pysrc/qulacs/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-27 09:46:08.000000 qulacs-0.6.4/pysrc/qulacs/circuit.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.731196 qulacs-0.6.4/pysrc/qulacs/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-27 09:43:30.000000 qulacs-0.6.4/pysrc/qulacs/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-05-27 09:43:30.000000 qulacs-0.6.4/pysrc/qulacs/converter/qasm_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.731196 qulacs-0.6.4/pysrc/qulacs/gate/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 09:43:30.000000 qulacs-0.6.4/pysrc/qulacs/gate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-05-27 09:46:08.000000 qulacs-0.6.4/pysrc/qulacs/gate.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.731196 qulacs-0.6.4/pysrc/qulacs/observable/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 09:43:30.000000 qulacs-0.6.4/pysrc/qulacs/observable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-27 09:46:08.000000 qulacs-0.6.4/pysrc/qulacs/observable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:08.000000 qulacs-0.6.4/pysrc/qulacs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.731196 qulacs-0.6.4/pysrc/qulacs/quantum_operator/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-27 09:43:30.000000 qulacs-0.6.4/pysrc/qulacs/quantum_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-27 09:46:08.000000 qulacs-0.6.4/pysrc/qulacs/quantum_operator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.731196 qulacs-0.6.4/pysrc/qulacs/state/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 09:43:30.000000 qulacs-0.6.4/pysrc/qulacs/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-27 09:46:08.000000 qulacs-0.6.4/pysrc/qulacs/state.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.731196 qulacs-0.6.4/pysrc/qulacs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 09:43:30.000000 qulacs-0.6.4/pysrc/qulacs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-27 09:43:30.000000 qulacs-0.6.4/pysrc/qulacs/utils/conversions_openfermion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.731196 qulacs-0.6.4/pysrc/qulacs/vistest/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 09:43:30.000000 qulacs-0.6.4/pysrc/qulacs/vistest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-27 09:43:30.000000 qulacs-0.6.4/pysrc/qulacs/vistest/test_vis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.731196 qulacs-0.6.4/pysrc/qulacs/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 09:43:30.000000 qulacs-0.6.4/pysrc/qulacs/visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-27 09:43:30.000000 qulacs-0.6.4/pysrc/qulacs/visualizer/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.771196 qulacs-0.6.4/pysrc/qulacs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-27 09:46:13.000000 qulacs-0.6.4/pysrc/qulacs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11971 2024-05-27 09:46:13.000000 qulacs-0.6.4/pysrc/qulacs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:46:13.000000 qulacs-0.6.4/pysrc/qulacs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:43:59.000000 qulacs-0.6.4/pysrc/qulacs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-27 09:46:13.000000 qulacs-0.6.4/pysrc/qulacs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 09:46:13.000000 qulacs-0.6.4/pysrc/qulacs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.731196 qulacs-0.6.4/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    75835 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/cppsim_wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.731196 qulacs-0.6.4/python/stub-test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/stub-test/generate_mypy_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.731196 qulacs-0.6.4/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.735195 qulacs-0.6.4/python/tests/multi_cpu/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/tests/multi_cpu/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/tests/multi_cpu/test_circuit_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/tests/multi_cpu/test_state_multi_cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.735195 qulacs-0.6.4/python/tests/single_cpu/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/tests/single_cpu/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/tests/single_cpu/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/tests/single_cpu/test_density_matrix_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12303 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/tests/single_cpu/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/tests/single_cpu/test_noise_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/tests/single_cpu/test_observable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/tests/single_cpu/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17686 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/tests/single_cpu/test_pointer_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/tests/single_cpu/test_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/tests/single_cpu/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-27 09:43:30.000000 qulacs-0.6.4/python/tests/single_cpu/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.739196 qulacs-0.6.4/script/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      303 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/build_clang.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      691 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/build_gcc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      440 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/build_gcc_with_gpu.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      441 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/build_gcc_with_memory_sanitizer.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      122 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/build_mpicc.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/build_msvc_2015.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/build_msvc_2015_with_gpu.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/build_msvc_2017.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/build_msvc_2017_with_gpu.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/build_msvc_2019.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/build_msvc_2019_with_gpu.bat
+-rwxr-xr-x   0 runner    (1001) docker     (127)      127 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/clean.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/download_wheel.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      318 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/fix_wheel_osx.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      141 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/format.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/generate_msvc_project_2015.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/generate_msvc_project_2015_with_gpu.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/generate_msvc_project_2017.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/generate_msvc_project_2017_with_gpu.bat
+-rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/generate_msvc_project_2019.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/generate_msvc_project_2019_with_gpu.bat
+-rwxr-xr-x   0 runner    (1001) docker     (127)      279 2024-05-27 09:43:30.000000 qulacs-0.6.4/script/update_stubs.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-27 09:46:13.775196 qulacs-0.6.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5242 2024-05-27 09:43:30.000000 qulacs-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.739196 qulacs-0.6.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.747196 qulacs-0.6.4/src/cppsim/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21592 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/circuit.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25641 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/circuit.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/circuit_builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    33797 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/circuit_optimizer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/circuit_optimizer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9609 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/exception.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    32399 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19956 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_factory.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24644 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_general.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13445 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_matrix_diagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_matrix_diagonal.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_matrix_sparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_matrix_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20532 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_merge.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_merge.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_named_npair.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_named_one.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16353 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_named_one.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_named_pauli.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_named_two.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23276 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_noisy_evolution.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12950 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_noisy_evolution.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_reflect.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_reversible.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/gate_to_gqo.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    36921 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/general_quantum_operator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14781 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/general_quantum_operator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/matrix_decomposition.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7033 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/noisesimulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/noisesimulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13716 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/observable.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/observable.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/pauli_operator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/pauli_operator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/qubit_info.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7181 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/qubit_info.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/qubit_table.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/qubit_table.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/simulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/simulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/state.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    34496 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/state.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/state_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/state_dm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/state_gpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/state_gpu.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/type.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/utility.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/cppsim/utility.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.759196 qulacs-0.6.4/src/csim/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/MPIutil.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/MPIutil.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/constant.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/constant.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/init_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/init_ops_fill.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/init_ops_random.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/memory_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/memory_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/memory_ops_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/memory_ops_dm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/stat_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/stat_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/stat_ops_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/stat_ops_dm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30440 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/stat_ops_expectation_value.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/stat_ops_probability.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/stat_ops_transition_amplitude.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/type.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    60932 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7802 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_control_multi_target_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14209 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_control_multi_target_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_control_single_target_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19452 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_control_single_target_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    34691 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_dm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    82604 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_matrix_dense_double.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_matrix_dense_double_eigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_matrix_dense_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_matrix_dense_multi_eigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17967 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_matrix_dense_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_matrix_diagonal_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_matrix_diagonal_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_matrix_phase_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_named.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_named_CNOT.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_named_CZ.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_named_FusedSWAP.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_named_H.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_named_SWAP.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_named_X.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_named_Y.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_named_Z.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_named_projection.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_named_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16633 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_pauli_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_pauli_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_qft.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_reflection.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/update_ops_reversible_boolean.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/utility.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/csim/utility.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.759196 qulacs-0.6.4/src/gpusim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/memory_ops.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/memory_ops.h
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/memory_ops_device_functions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    54626 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/stat_ops.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/stat_ops.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/stat_ops_device_functions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/update_ops_cuda.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/update_ops_cuda_device_functions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    72073 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/update_ops_multi.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/update_ops_named.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    15974 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/update_ops_single.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    25384 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/util.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/util.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/util.h
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/util_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/util_export.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/util_func.h
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/util_type.h
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/gpusim/util_type_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.763196 qulacs-0.6.4/src/vqcsim/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/GradCalculator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/GradCalculator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/boolean_formula.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/causalcone_simulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/differential.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/differential.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/loss_function.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/loss_function.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/optimizer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/parametric_circuit.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/parametric_circuit.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/parametric_circuit_builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/parametric_gate.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/parametric_gate_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/parametric_gate_factory.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/parametric_simulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/parametric_simulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/parser.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/problem.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-05-27 09:43:30.000000 qulacs-0.6.4/src/vqcsim/solver.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.763196 qulacs-0.6.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.767196 qulacs-0.6.4/test/cppsim/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/H2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_KAK.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    32101 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_circuit.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    54983 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_circuit_multicpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_circuit_optimize_light.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    57300 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_gate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    29782 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_gate_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    58304 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_gate_multicpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23845 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_hamiltonian.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_hamiltonian_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_hamiltonian_multicpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_mpiutil_multicpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12025 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_noise_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_noisesimulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20764 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_noisyevolution.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_pauli_operator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_simulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_state_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/cppsim/test_state_multicpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.771196 qulacs-0.6.4/test/csim/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/csim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/csim/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/csim/test_memory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/csim/test_omputil.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26768 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/csim/test_stat.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/csim/test_update_control.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/csim/test_update_dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/csim/test_update_dense_double.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/csim/test_update_diagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/csim/test_update_diagonal_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13376 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/csim/test_update_named.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/csim/test_update_pauli.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.771196 qulacs-0.6.4/test/gpusim/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/gpusim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/gpusim/H2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    33346 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/gpusim/test_circuit.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/gpusim/test_compat_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/gpusim/test_func_memory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    47173 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/gpusim/test_gate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9409 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/gpusim/test_hamiltonian.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    43547 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/gpusim/test_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/gpusim/test_update_control.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/gpusim/test_update_dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/gpusim/test_update_diagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/gpusim/test_update_named.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/gpusim/test_update_pauli.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/gpusim/test_util.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.771196 qulacs-0.6.4/test/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    13090 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/util/util.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:46:13.771196 qulacs-0.6.4/test/vqcsim/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/vqcsim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/vqcsim/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17741 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/vqcsim/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-27 09:43:30.000000 qulacs-0.6.4/test/vqcsim/test_backprop.cpp
```

### Comparing `qulacs-0.6.3/.devcontainer/cpu/Dockerfile` & `qulacs-0.6.4/.devcontainer/cpu/Dockerfile`

 * *Files 9% similar despite different names*

```diff
@@ -18,10 +18,7 @@
     clang-format \
     gdb \
     cmake \
     libboost-dev \
     doxygen \
     pandoc \
     && apt-get autoremove -y && apt-get clean -y && rm -rf /var/lib/apt/lists/*
-
-RUN pip install -U pip \
-    && pip install black flake8 openfermion mypy pybind11-stubgen
```

### Comparing `qulacs-0.6.3/.devcontainer/cpu/devcontainer.json` & `qulacs-0.6.4/.devcontainer/cpu/devcontainer.json`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/.devcontainer/gpu/Dockerfile` & `qulacs-0.6.4/.devcontainer/gpu/Dockerfile`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/.devcontainer/gpu/devcontainer.json` & `qulacs-0.6.4/.devcontainer/gpu/devcontainer.json`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/.github/workflows/ci_macos.yml` & `qulacs-0.6.4/.github/workflows/ci_macos.yml`

 * *Files 7% similar despite different names*

```diff
@@ -16,62 +16,53 @@
 
 jobs:
   macos-build:
     name: Build on macOS
     strategy:
       matrix:
         python-version: ["3.10"]
-        compiler: ["gcc", "clang"]
+        compiler: ["clang"]
         include:
-          - compiler: "gcc"
-            c_compiler: "/usr/local/opt/ccache/libexec/gcc-11"
-            cxx_compiler: "/usr/local/opt/ccache/libexec/g++-11"
           - compiler: "clang"
             c_compiler: "/usr/local/opt/ccache/libexec/clang"
             cxx_compiler: "/usr/local/opt/ccache/libexec/clang++"
-    runs-on: "macos-12"
+    runs-on: "macos-13"
     env:
       C_COMPILER: ${{ matrix.c_compiler }}
       CXX_COMPILER: ${{ matrix.cxx_compiler }}
       PYTHON: ${{ matrix.python-version }}
       CACHE_NAME: "ccache-qulacs-build-v2"
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Setup cmake
         uses: lukka/get-cmake@latest
 
       - name: Setup ccache
         uses: hendrikmuhs/ccache-action@v1.2
         with:
           # Include compiler to distinguish cache for each compiler.
           key: ${{ github.job }}-macos-12-${{ matrix.compiler }}
           verbose: 2
 
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
-          architecture: x64
 
       - name: Install Boost for macOS
         run: |
-          brew upgrade
+          brew update
           brew install boost
           brew link boost
 
       - name: Install qulacs for macOS
         run: USE_TEST=Yes ./script/build_gcc.sh
 
       - name: Install qulacs Python module
         run: pip install .[ci]
 
-      # - name: Test if stub is working
-      #   run: |
-      #     python python/stub-test/generate_mypy_tester.py qulacs
-      #     mypy python/stub-test/names_qulacs.py
-
       - name: Test in macOS
         run: |
           cd ./build
           make test -j
           make pythontest -j
```

### Comparing `qulacs-0.6.3/.github/workflows/ci_ubuntu.yml` & `qulacs-0.6.4/.github/workflows/ci_ubuntu.yml`

 * *Files 6% similar despite different names*

```diff
@@ -11,43 +11,42 @@
     paths-ignore:
       - ".devcontainer/**"
       - ".vscode/**"
       - "doc/**"
       - "*.md"
 
 jobs:
-  gcc8-build:
-    name: GCC8 build
+  gcc-build:
+    name: GCC build
     strategy:
       matrix:
-        python-version: ["3.10"]
+        python-version: ["3.11"]
     runs-on: "ubuntu-20.04"
     env:
       CXX_COMPILER: "/usr/lib/ccache/g++"
       C_COMPILER: "/usr/lib/ccache/gcc"
       QULACS_OPT_FLAGS: "-mtune=haswell -march=haswell -mfpmath=both"
       COVERAGE: "Yes"
       USE_TEST: "Yes"
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Setup cmake
         uses: lukka/get-cmake@latest
 
       - name: Setup ccache
         uses: hendrikmuhs/ccache-action@v1.2
         with:
           key: "${{ github.job }}-ubuntu-20.04"
           verbose: 2
 
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
-          architecture: x64
 
       - name: Install boost
         run: sudo apt install libboost-dev
 
       - name: Install LCOV
         run: |
           git clone -b v1.15 --depth 1 https://github.com/linux-test-project/lcov.git
@@ -56,46 +55,35 @@
 
       - name: Install qulacs for Ubuntu
         run: ./script/build_gcc.sh
 
       - name: Install qulacs Python module
         run: pip install .[ci]
 
-      - name: Check stubs
-        run: |
-          ./script/update_stubs.sh
-          diff=$(git diff)
-          echo -n "$diff"
-          # Without `-n`, `echo -n "$diff" | wc -l` is 1 even if `"$diff" is empty.`
-          test $(echo -n "$diff" | wc -l) -eq 0
-
-      - name: Test if stub is working
-        run: |
-          python python/stub-test/generate_mypy_tester.py qulacs
-          mypy python/stub-test/names_qulacs.py
-
       - name: Test in Ubuntu
         run: |
           cd ./build
           make coverage -j $(nproc)
           make pythontest -j $(nproc)
 
       - name: Upload coverage to codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
 
   gcc10-build-with-address-sanitizer:
     name: GCC10 build with -fsanitizer=address enabled
     runs-on: "ubuntu-20.04"
     env:
       CXX_COMPILER: "/usr/lib/ccache/g++"
       C_COMPILER: "/usr/lib/ccache/gcc"
       QULACS_OPT_FLAGS: "-mtune=haswell -march=haswell -mfpmath=both"
       USE_TEST: "Yes"
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Setup cmake
         uses: lukka/get-cmake@latest
 
       - name: Setup ccache
         uses: hendrikmuhs/ccache-action@v1.2
         with:
@@ -110,39 +98,39 @@
 
       - name: Test in Ubuntu
         # -j option is not appended because running this test in parallel is slower than sequential version.
         run: |
           cd ./build
           make test
 
-  nvcc-gcc8-GPUbuild:
-    name: nvcc + gcc8 build
+  nvcc-gcc-GPUbuild:
+    name: nvcc + gcc build
     runs-on: "ubuntu-20.04"
     env:
       CXX_COMPILER: "/usr/lib/ccache/g++"
       C_COMPILER: "/usr/lib/ccache/gcc"
       QULACS_OPT_FLAGS: "-mtune=haswell -march=haswell -mfpmath=both"
       PYTHON: "3.7.5"
       COVERAGE: "ON"
       USE_TEST: "Yes"
       USE_GPU: "Yes"
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Setup cmake
         uses: lukka/get-cmake@latest
 
       - name: Setup ccache
         uses: hendrikmuhs/ccache-action@v1.2
         with:
           key: "${{ github.job }}-ubuntu-20.04"
           verbose: 2
 
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.7.5"
           architecture: x64
 
       - name: Install boost
         run: sudo apt install libboost-dev
 
@@ -168,15 +156,15 @@
     runs-on: "ubuntu-22.04"
     env:
       C_COMPILER: "aarch64-linux-gnu-gcc-11"
       CXX_COMPILER: "aarch64-linux-gnu-g++-11"
       QULACS_OPT_FLAGS: "-march=armv8.2-a+sve"
       QEMU_LD_PREFIX: "/usr/aarch64-linux-gnu"
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Setup qemu
         run: |
           sudo apt-get update
           sudo apt-get install -y cmake ninja-build pkg-config libglib2.0-dev gcc-11-aarch64-linux-gnu g++-11-aarch64-linux-gnu
           wget -q https://download.qemu.org/qemu-7.2.0.tar.xz
           tar xJf qemu-7.2.0.tar.xz
@@ -206,15 +194,15 @@
           QEMU_CPU="max,sve512=on" qemu-aarch64 ../bin/vqcsim_test
           QEMU_CPU="max,sve256=on" qemu-aarch64 ../bin/vqcsim_test
 
   format:
     name: Format with clang-format
     runs-on: "ubuntu-20.04"
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - run: sudo apt install clang-format=1:10.0-50~exp1
 
       - name: format
         run: |
           ./script/format.sh
 
@@ -226,53 +214,53 @@
           test $(echo -n "$diff" | wc -l) -eq 0
 
   python-format:
     name: Format with Python formatters
     runs-on: "ubuntu-20.04"
     strategy:
       matrix:
-        python-version: ["3.10"]
+        python-version: ["3.11"]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
 
       - name: Install formatters
-        run: pip install black isort
+        run: python -m pip install black isort
 
       - name: Check format
         run: |
-          black . --check --diff
-          isort . --check --diff
+          python -m black . --check --diff
+          python -m isort . --check --diff
 
   mpicc-build:
     name: MPICC build
     strategy:
       matrix:
-        python-version: ["3.10"]
+        python-version: ["3.11"]
     runs-on: "ubuntu-20.04"
     env:
       CXX_COMPILER: "mpic++"
       C_COMPILER: "mpicc"
       QULACS_OPT_FLAGS: "-mtune=haswell -march=haswell -mfpmath=both"
       PYTHON: ${{ matrix.python-version }}
       COVERAGE: "ON"
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Setup cmake
         uses: lukka/get-cmake@latest
 
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
 
       - name: Install mpi-bin
         run: sudo apt install openmpi-bin
 
@@ -290,35 +278,22 @@
 
       - name: Install qulacs Python module
         run: USE_MPI=Yes pip install .[ci]
 
       - name: Install MPI Python module
         run: pip install mpi4py
 
-      - name: Check stubs
-        run: |
-          ./script/update_stubs.sh
-          diff=$(git diff)
-          echo -n "$diff"
-          # Without `-n`, `echo -n "$diff" | wc -l` is 1 even if `"$diff" is empty.`
-          test $(echo -n "$diff" | wc -l) -eq 0
-
-      - name: Test if stub is working
-        run: |
-          python python/stub-test/generate_mypy_tester.py qulacs
-          mypy python/stub-test/names_qulacs.py
-
       - name: Test in Ubuntu
         run: |
           cd ./build
           make coverage
           make pythontest
 
       - name: Test in Ubuntu
         run: |
           pip install pytest
           mpirun -n 2 bin/cppsim_test --gtest_filter="*multicpu*"
           mpirun -n 2 bin/vqcsim_test --gtest_filter="*multicpu*"
           mpirun -n 2 pytest python/tests/multi_cpu
 
       - name: Upload coverage to codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
```

### Comparing `qulacs-0.6.3/.github/workflows/ci_windows.yml` & `qulacs-0.6.4/.github/workflows/ci_windows.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,41 @@
 name: Windows CI
 
 on:
-  push:
-    paths-ignore:
-      - ".devcontainer/**"
-      - ".vscode/**"
-      - "doc/**"
-      - "*.md"
-    branches:
-      - "dev"
   pull_request_review:
     types: [submitted, edited]
   workflow_dispatch:
 
 jobs:
-  gcc8-build:
-    name: GCC8 build
+  gcc-build:
+    name: GCC build
     # For jobs triggered by pull_request_review, build task should run only if is in `approved` state.
-    if: ${{ github.event_name == 'push' || github.event_name == 'workflow_dispatch' || github.event.review.state == 'approved' }}
+    if: ${{ github.event_name == 'workflow_dispatch' || github.event.review.state == 'approved' }}
     strategy:
       matrix:
         python-version: ["3.10"]
     runs-on: "windows-2019"
     env:
       CXX_COMPILER: "g++-8"
       C_COMPILER: "gcc-8"
       PYTHON: ${{ matrix.python-version }}
       COVERAGE: "ON"
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Setup cmake
         uses: lukka/get-cmake@latest
 
       # TODO: In Windows, ccache is not used because its behavior is not stable.
       # mozilla/sccache is one candidate for this situation.
 
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
-          architecture: x64
 
       - name: Install boost
         uses: MarkusJx/install-boost@v2.4.3
         id: install-boost
         with:
           boost_version: 1.77.0
 
@@ -56,18 +47,13 @@
           BOOST_ROOT: ${{ steps.install-boost.outputs.BOOST_ROOT }}
 
       - name: Install qulacs Python module
         env:
           BOOST_ROOT: ${{ steps.install-boost.outputs.BOOST_ROOT }}
         run: pip install .[ci]
 
-      - name: Test if stub is working
-        run: |
-          python python/stub-test/generate_mypy_tester.py qulacs
-          mypy python/stub-test/names_qulacs.py
-
       - name: Test in Windows
         env:
           BOOST_ROOT: ${{ steps.install-boost.outputs.BOOST_ROOT }}
         run: |
           cmake --build ./visualstudio --target test --config Release
           cmake --build ./visualstudio --target pythontest --config Release
```

### Comparing `qulacs-0.6.3/.gitignore` & `qulacs-0.6.4/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -206,16 +206,18 @@
 Mkfile.old
 dkms.conf
 
 # End of https://www.gitignore.io/api/c
 
 # End of https://www.gitignore.io/api/python,macos
 
-# ignore stub files generated by https://github.com/Qulacs-Osaka/DevOps-OsakaUniv
-/typings/
+# ignore stub files
+*.pyi
+py.typed
+
 !/.vscode/tasks.json
 
 # ignore names_* for stub test
 /python/stub-test/names_*
 
 # ignore coverage
 /coverage/
```

### Comparing `qulacs-0.6.3/.vscode/tasks.json` & `qulacs-0.6.4/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/CMakeLists.txt` & `qulacs-0.6.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/CONTRIBUTING.md` & `qulacs-0.6.4/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 Issue title should be prefixed with `[Feat]`.
 
 ## Pull Request
 
 ### Pull Request Process
 PR is always welcome!
 
-Writing to Issue is not necessary (but recommended) to create single PR. Just create PR to the `dev` branch.
+Writing to Issue is not necessary (but recommended) to create single PR. Just create PR to the `main` branch.
 
 However, if you want to make changes that requires multiple PR, please discuss the change you wish to make via Issue.
 ### Size of Pull Request
 When you want to create PR, non-automatically created diff should not be more than about 300 lines.
 
 If you want to make large PR, then first ask to maintainers and feature branch will be created for review.
 ## Requirements to merge Pull Request
@@ -61,10 +61,10 @@
 $ python setup.py install
 $ cmake --build ./visualstudio --target test --config Release
 $ cmake --build ./visualstudio --target pythontest --config Release
 ```
 
 ### Tips
 
-- We recommend use Python from [pyenv](https://github.com/pyenv/pyenv) and [vertualenv](https://pypi.org/project/virtualenv/) for the local test.
+- We recommend use Python from [pyenv](https://github.com/pyenv/pyenv) and [virtualenv](https://pypi.org/project/virtualenv/) for the local test.
     - Since we run `python setup.py install` at global Python unstable qulacs would be installed unintentionally.
     - And it would be difficult to show dependencies version when we need for debug
```

### Comparing `qulacs-0.6.3/LICENSE` & `qulacs-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/PKG-INFO` & `qulacs-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qulacs
-Version: 0.6.3
+Version: 0.6.4
 Summary: Quantum circuit simulator for research
 Author-email: QunaSys <qulacs@qunasys.com>
 License: MIT License
         
         Copyright (c) 2018 Qulacs Authors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,14 +54,16 @@
 Requires-Dist: flake8; extra == "ci"
 Requires-Dist: isort; extra == "ci"
 Requires-Dist: mypy; extra == "ci"
 Requires-Dist: pybind11-stubgen; extra == "ci"
 Requires-Dist: openfermion; extra == "ci"
 Requires-Dist: pytest; extra == "ci"
 Provides-Extra: doc
+Requires-Dist: mypy; extra == "doc"
+Requires-Dist: pybind11-stubgen; extra == "doc"
 Requires-Dist: sphinx==7.*; extra == "doc"
 Requires-Dist: sphinx-rtd-theme; extra == "doc"
 Requires-Dist: breathe; extra == "doc"
 Requires-Dist: exhale; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
 Requires-Dist: myst-parser; extra == "doc"
 Requires-Dist: sphinx-copybutton; extra == "doc"
@@ -181,14 +183,23 @@
 
 Install single-thread Qulacs:
 
 ```
 USE_OMP=No pip install .
 ```
 
+If you install qulacs manually, it does not have type stubs.
+To include type stubs into the package, you have to run `script/generate_stubs.sh` after the first install and reinstall.
+
+```
+pip install .
+script/update_stubs.sh
+pip install .
+```
+
 The number of threads used in Qulacs installed with default options can be controlled via the environment variable `OMP_NUM_THREADS` or `QULACS_NUM_THREADS`.
 While `OMP_NUM_THREADS` affects the parallelization of other libraries, `QULACS_NUM_THREADS` controls only the parallelization of QULACS.
 Or, if you want to force only Qulacs to use a single thread, You can install single-thread Qulacs with the above command.
 
 For development purpose, optional dependencies can be installed as follows.
 ```
 # Install development tools
```

### Comparing `qulacs-0.6.3/README.md` & `qulacs-0.6.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,23 @@
 
 Install single-thread Qulacs:
 
 ```
 USE_OMP=No pip install .
 ```
 
+If you install qulacs manually, it does not have type stubs.
+To include type stubs into the package, you have to run `script/generate_stubs.sh` after the first install and reinstall.
+
+```
+pip install .
+script/update_stubs.sh
+pip install .
+```
+
 The number of threads used in Qulacs installed with default options can be controlled via the environment variable `OMP_NUM_THREADS` or `QULACS_NUM_THREADS`.
 While `OMP_NUM_THREADS` affects the parallelization of other libraries, `QULACS_NUM_THREADS` controls only the parallelization of QULACS.
 Or, if you want to force only Qulacs to use a single thread, You can install single-thread Qulacs with the above command.
 
 For development purpose, optional dependencies can be installed as follows.
 ```
 # Install development tools
```

### Comparing `qulacs-0.6.3/README_MPI.md` & `qulacs-0.6.4/README_MPI.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/benchmark/AdaptiveGate.py` & `qulacs-0.6.4/benchmark/AdaptiveGate.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/benchmark/bench_circuit.py` & `qulacs-0.6.4/benchmark/bench_circuit.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/benchmark/causalconetest.cpp` & `qulacs-0.6.4/benchmark/causalconetest.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/benchmark/circuits/quantumvolume.py` & `qulacs-0.6.4/benchmark/circuits/quantumvolume.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/benchmark/circuits/qulacsbench.py` & `qulacs-0.6.4/benchmark/circuits/qulacsbench.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/benchmark/libcppsim_benchmark.cpp` & `qulacs-0.6.4/benchmark/libcppsim_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/benchmark/libcsim_benchmark.cpp` & `qulacs-0.6.4/benchmark/libcsim_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/benchmark/test_qulacs_1.py` & `qulacs-0.6.4/benchmark/test_qulacs_1.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/benchmark/test_qulacs_2.py` & `qulacs-0.6.4/benchmark/test_qulacs_2.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/cmake_script/FetchContent/CMakeLists.cmake.in` & `qulacs-0.6.4/cmake_script/FetchContent/CMakeLists.cmake.in`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/cmake_script/FetchContent.cmake` & `qulacs-0.6.4/cmake_script/FetchContent.cmake`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/cmake_script/FindAVX2.cmake` & `qulacs-0.6.4/cmake_script/FindAVX2.cmake`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/cmake_script/FindSVE.cmake` & `qulacs-0.6.4/cmake_script/FindSVE.cmake`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/.gitignore` & `qulacs-0.6.4/doc/.gitignore`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/Makefile` & `qulacs-0.6.4/doc/en/Makefile`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/make.bat` & `qulacs-0.6.4/doc/en/make.bat`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/_static/images/dojo.png` & `qulacs-0.6.4/doc/en/source/_static/images/dojo.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/_static/images/github.png` & `qulacs-0.6.4/doc/en/source/_static/images/github.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/_static/images/logo-c-h.png` & `qulacs-0.6.4/doc/en/source/_static/images/logo-c-h.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/_static/images/slack.png` & `qulacs-0.6.4/doc/en/source/_static/images/slack.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/_templates/autoapi/python/class.rst` & `qulacs-0.6.4/doc/en/source/_templates/autoapi/python/class.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/_templates/autoapi/python/data.rst` & `qulacs-0.6.4/doc/en/source/_templates/autoapi/python/data.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/_templates/autoapi/python/function.rst` & `qulacs-0.6.4/doc/en/source/_templates/autoapi/python/function.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/_templates/autoapi/python/method.rst` & `qulacs-0.6.4/doc/en/source/_templates/autoapi/python/method.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/_templates/autoapi/python/module.rst` & `qulacs-0.6.4/doc/en/source/_templates/autoapi/python/module.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/apply/0_overview.ipynb` & `qulacs-0.6.4/doc/en/source/apply/0_overview.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/apply/5.2_qcl.ipynb` & `qulacs-0.6.4/doc/en/source/apply/5.2_qcl.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/apply/6.2_vqe.ipynb` & `qulacs-0.6.4/doc/en/source/apply/6.2_vqe.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967651833460657%*

 * *Differences: {"'cells'": "{2: {'execution_count': 4, 'source': {insert: [(2, 'from openfermion.linalg import "*

 * *            "get_sparse_operator\\n'), (3, 'from openfermion.chem import MolecularData\\n')], "*

 * *            'delete: [3, 2]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.12'}}"}*

```diff
@@ -31,22 +31,22 @@
                 "## When use Google Colaboratory, please ignore 'You must restart the runtime in order to use newly installed versions'.\n",
                 "## Crash when restarting runtime.\n",
                 "!pip install qulacs pyscf openfermion openfermionpyscf"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import qulacs\n",
                 "from openfermion.transforms import get_fermion_operator, jordan_wigner\n",
-                "from openfermion.transforms import get_sparse_operator\n",
-                "from openfermion.hamiltonians import MolecularData\n",
+                "from openfermion.linalg import get_sparse_operator\n",
+                "from openfermion.chem import MolecularData\n",
                 "from openfermionpyscf import run_pyscf\n",
                 "from scipy.optimize import minimize\n",
                 "from pyscf import fci\n",
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt"
             ]
         },
@@ -257,13 +257,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.6"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `qulacs-0.6.3/doc/en/source/apply/6.3_ssvqe.ipynb` & `qulacs-0.6.4/doc/en/source/apply/6.3_ssvqe.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/apply/img/QCL.png` & `qulacs-0.6.4/doc/en/source/apply/img/QCL.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/conf.py` & `qulacs-0.6.4/doc/en/source/conf.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/guide/2.0_python_advanced.ipynb` & `qulacs-0.6.4/doc/en/source/guide/2.0_python_advanced.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963234126984127%*

 * *Differences: {"'cells'": "{18: {'source': {insert: [(0, '### Operation on classic registers\\n')], delete: "*

 * *            "[0]}}, 30: {'execution_count': 3, 'source': {insert: [(0, 'from qulacs import "*

 * *            "DensityMatrix\\n'), (1, '\\n')], delete: [0]}}, 127: {'execution_count': None}, 135: "*

 * *            "{'execution_count': None}, 141: {'execution_count': None}, 143: {'execution_count': "*

 * *            "None}, insert: [(99, OrderedDict([('cell_type', 'markdown'), ('metadata', "*

 * *            "OrderedDict()), ('sour […]*

```diff
@@ -376,15 +376,15 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Opetation on classic registers\n",
+                "### Operation on classic registers\n",
                 "Quantum states have classical registers as integer arrays with variable length. The classical register is used to write the result of the Instrument operation or to describe a gate that executes conditions as the result of the classical register. The value of a classic register that has not yet been written is 0. The classical register is copied at the same time when the quantum state is copied by the `copy` and `load` functions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {},
@@ -630,15 +630,15 @@
                 "\n",
                 "### Generate and delete\n",
                 "The necessary memory is allocated when the instance is created. The memory is released when Python interpreter destroys the instance, but can be released with `del` if you want to explicitly destroy it to free memory."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** Density Matrix ***\n",
@@ -650,15 +650,16 @@
                         "(0,0) (0,0) (0,0) (0,0)\n",
                         "(0,0) (0,0) (0,0) (0,0)\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
-                "from qulacs import QuantumState\n",
+                "from qulacs import DensityMatrix\n",
+                "\n",
                 "n = 2\n",
                 "state = DensityMatrix(n)\n",
                 "print(state)\n",
                 "del state\n"
             ]
         },
         {
@@ -3430,14 +3431,64 @@
                 "from qulacs.gate import Measurement\n",
                 "target = 0\n",
                 "classical_pos = 0\n",
                 "gate = Measurement(target, classical_pos)\n"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "#### ProbabilisticInstrument\n",
+                "In addition to the `Probabilistic` function, it is a function that can get the index of the operated gate. If the sum of the distribution is less than 1, or for some other reason no gate has acted, the number of elements in `gate_list` is saved in `classical_address`."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "2 [0.70710678+0.j 0.70710678+0.j 0.        +0.j 0.        +0.j]\n",
+                        "0 [0.+0.j 1.+0.j 0.+0.j 0.+0.j]\n",
+                        "1 [0.-0.j 0.+1.j 0.-0.j 0.+0.j]\n",
+                        "1 [0.-0.j 0.+1.j 0.-0.j 0.+0.j]\n",
+                        "2 [0.70710678+0.j 0.70710678+0.j 0.        +0.j 0.        +0.j]\n",
+                        "0 [0.+0.j 1.+0.j 0.+0.j 0.+0.j]\n",
+                        "1 [0.-0.j 0.+1.j 0.-0.j 0.+0.j]\n",
+                        "1 [0.-0.j 0.+1.j 0.-0.j 0.+0.j]\n",
+                        "2 [0.70710678+0.j 0.70710678+0.j 0.        +0.j 0.        +0.j]\n",
+                        "2 [0.70710678+0.j 0.70710678+0.j 0.        +0.j 0.        +0.j]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from qulacs import QuantumState\n",
+                "from qulacs.gate import X, Y, H, ProbabilisticInstrument\n",
+                "n = 2\n",
+                "state = QuantumState(n)\n",
+                "index = 0\n",
+                "x_gate = X(index)\n",
+                "y_gate = Y(index)\n",
+                "h_gate = H(index)\n",
+                "distribution = [0.25, 0.25, 0.25]\n",
+                "gate_list = [x_gate, y_gate, h_gate]\n",
+                "classical_address = 0\n",
+                "for _ in range(10):\n",
+                "  state = QuantumState(n)\n",
+                "  probabilistic_instrument_gate = ProbabilisticInstrument(distribution, gate_list, classical_address)\n",
+                "  probabilistic_instrument_gate.update_quantum_state(state)\n",
+                "  result = state.get_classical_value(classical_address)\n",
+                "  print(result, state.get_vector())\n"
+            ]
+        },
+        {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Adaptive operation\n",
                 "This is a gate that uses a function that returns a Boolean value with variable-length list of classical register values as an argument, and determines whether to perform an operation according to the conditions obtained from the classical register. Conditions can be written as python functions. A python function must be a function that takes a list of type `int` as an argument and returns a bool type value."
             ]
@@ -3935,15 +3986,15 @@
             "source": [
                 "### Further operations on a quantum circuit\n",
                 "You can add gates at specific positions to a quantum circuit and perform operations such as ```copy``` and ```merge_circuit```. Here is the code that summarizes these operations."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "qubit count = 3\n",
@@ -4137,15 +4188,15 @@
             "metadata": {},
             "source": [
                 "Quantum circuits can be stored to files in pickle format."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from qulacs import QuantumCircuit\n",
                 "import pickle\n",
                 "\n",
                 "circuit = QuantumCircuit(3)\n",
@@ -4337,15 +4388,15 @@
                 "\n",
                 "Parametric quantum circuits can be converted to/from JSON string.\n",
                 "If it has unsupported gates, the conversion fails with an error."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "*** Quantum Circuit Info ***\n",
@@ -4397,15 +4448,15 @@
             "metadata": {},
             "source": [
                 "Parametric quantum circuits can be converted to files in pickle format."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from qulacs import ParametricQuantumCircuit\n",
                 "from qulacs import circuit\n",
                 "\n",
                 "circuit = ParametricQuantumCircuit(3)\n",
@@ -4672,15 +4723,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.11.4"
         },
         "vscode": {
             "interpreter": {
                 "hash": "949777d72b0d2535278d3dc13498b2535136f6dfe0678499012e853ee9abcab1"
             }
         }
     },
```

### Comparing `qulacs-0.6.3/doc/en/source/index.md` & `qulacs-0.6.4/doc/en/source/index.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/intro/0_about.md` & `qulacs-0.6.4/doc/en/source/intro/0_about.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/intro/1_install.md` & `qulacs-0.6.4/doc/en/source/intro/1_install.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/intro/2_faq.md` & `qulacs-0.6.4/doc/en/source/intro/2_faq.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/intro/3_usage.md` & `qulacs-0.6.4/doc/en/source/intro/3_usage.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/intro/4.1_python_tutorial.ipynb` & `qulacs-0.6.4/doc/en/source/intro/4.1_python_tutorial.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807445112132612%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(4, 'print(state)\\n')], delete: [4]}}, 8: {'source': "*

 * *            "{insert: [(18, 'print(state)\\n')], delete: [18]}}, 11: {'source': {insert: [(14, "*

 * *            "'print(state)\\n')], delete: [14]}}, 14: {'source': {insert: [(10, "*

 * *            "'print(third_state.get_vector())\\n')], delete: [10]}}, 17: {'source': {insert: [(10, "*

 * *            "'print(obtained_value)\\n')], delete: [10]}}, 20: {'source': {insert: [(9, "*

 * *            '\'print("prob_meas_3rd : ",zero_pro […]*

```diff
@@ -50,15 +50,15 @@
                 }
             ],
             "source": [
                 "from qulacs import QuantumState\n",
                 "# Generate 2 qubit states\n",
                 "n = 2\n",
                 "state = QuantumState(n)\n",
-                "print(state)"
+                "print(state)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "You can not generate the quantum states if the memory is not sufficient.\n",
@@ -127,15 +127,15 @@
                 "# Generate random initial state\n",
                 "state.set_Haar_random_state()\n",
                 "print(state)\n",
                 "\n",
                 "# Generate random initial state with specifying seed\n",
                 "seed = 0\n",
                 "state.set_Haar_random_state(seed)\n",
-                "print(state)"
+                "print(state)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Obtain data of quantum state"
@@ -182,15 +182,15 @@
                 "vec = state.get_vector()\n",
                 "print(type(vec), vec.dtype)\n",
                 "print(vec)\n",
                 "\n",
                 "# Set the state vector\n",
                 "myvec = np.array([0.5,0.5,0.5,0.5])\n",
                 "state.load(myvec)\n",
-                "print(state)"
+                "print(state)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Copy and load quantum state data"
@@ -230,15 +230,15 @@
                 "state.set_computational_basis(0b00101)\n",
                 "# Copy to generate another quantum state\n",
                 "second_state = state.copy()\n",
                 "print(second_state.get_vector())\n",
                 "# Generate a new quantum state, and copy from an existing quantum state\n",
                 "third_state = QuantumState(n)\n",
                 "third_state.load(state)\n",
-                "print(third_state.get_vector())"
+                "print(third_state.get_vector())\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Operate classic registers"
@@ -271,15 +271,15 @@
                 "state.set_zero_state()\n",
                 "# Set the 3rd classical register as 1\n",
                 "register_position = 3\n",
                 "register_value = 1\n",
                 "state.set_classical_value(register_position, register_value)\n",
                 "# Obtain the value of the 3rd classical register\n",
                 "obtained_value = state.get_classical_value(register_position)\n",
-                "print(obtained_value)"
+                "print(obtained_value)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Calculate quantum states"
@@ -311,15 +311,15 @@
                 "n = 5\n",
                 "state = QuantumState(n)\n",
                 "state.set_Haar_random_state(0)\n",
                 "\n",
                 "# Calculate the probability to get 0 in measurement of the qubit in the given index at Z-basis\n",
                 "index = 3\n",
                 "zero_probability = state.get_zero_probability(index)\n",
-                "print(\"prob_meas_3rd : \",zero_probability)"
+                "print(\"prob_meas_3rd : \",zero_probability)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The `sampling` function can be used to sample the results of a quantum state measurement. The argument of the function is the number of data to sample."
@@ -345,15 +345,15 @@
                 "\n",
                 "n = 2\n",
                 "state = QuantumState(n)\n",
                 "state.load([1/np.sqrt(2), 0, 0.5, 0.5])\n",
                 "data = state.sampling(10)\n",
                 "print(data)\n",
                 "# Show in binary format\n",
-                "print([format(value, \"b\").zfill(2) for value in data])"
+                "print([format(value, \"b\").zfill(2) for value in data])\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "You can find many other functions in \"Advanced\" section. "
@@ -392,15 +392,15 @@
                 "n = 5\n",
                 "state_bra = QuantumState(n)\n",
                 "state_ket = QuantumState(n)\n",
                 "state_bra.set_Haar_random_state()\n",
                 "state_ket.set_computational_basis(0)\n",
                 "# Calculate the inner product\n",
                 "value = inner_product(state_bra, state_ket)\n",
-                "print(value)"
+                "print(value)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Quantum gate"
@@ -444,15 +444,15 @@
                 }
             ],
             "source": [
                 "from qulacs.gate import X\n",
                 "\n",
                 "target_index = 1\n",
                 "x_gate = X(target_index)\n",
-                "print(x_gate)"
+                "print(x_gate)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Operation of quantum gates"
@@ -502,15 +502,15 @@
                 "n = 2\n",
                 "state = QuantumState(n)\n",
                 "print(state)\n",
                 "\n",
                 "index = 1\n",
                 "x_gate = X(index)\n",
                 "x_gate.update_quantum_state(state)\n",
-                "print(state)"
+                "print(state)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Various quantum gates"
@@ -549,15 +549,188 @@
                 "\n",
                 "# CNOT, CZ, SWAP gate\n",
                 "from qulacs.gate import CNOT, CZ, SWAP\n",
                 "control = 1\n",
                 "target2 = 1\n",
                 "cnot_gate = CNOT(control, target)\n",
                 "cz_gate = CZ(control, target)\n",
-                "swap_gate = SWAP(target, target2)"
+                "swap_gate = SWAP(target, target2)\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Here is an introduction of some of the named gates with examples.\n",
+                "\n",
+                "#### TOFFOLI gate\n",
+                "\n",
+                "TOFFOLI gate has control indices in the first and second arguments, and the target index in the third argument.\n",
+                "When the qubits corresponding to the control indices given in the first and second arguments are both $\\ket{1}$, the qubits corresponding to the target index given in the third argument is flipped."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from qulacs.gate import TOFFOLI\n",
+                "control1 = 0\n",
+                "control2 = 1\n",
+                "target1 = 2\n",
+                "toffoli_gate = TOFFOLI(control1, control2, target1)\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Here is an example of the operation of the TOFFOLI gate. Since 0 and 1 are given as control indices and 2 is given as the target index, the qubit of the 2-nd qubit is flipped when the 0-th qubit and the 1-st qubit are $\\ket{1}$.\n",
+                "You can see that the quantum states $\\ket{011}$ and $\\ket{111}$ are swapped before and after the action of the TOFFOLI gate."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        " *** Quantum State ***\n",
+                        " * Qubit Count : 3\n",
+                        " * Dimension   : 8\n",
+                        " * State vector : \n",
+                        "(-0.0845729,-0.14143)\n",
+                        "  (-0.133864,0.11328)\n",
+                        " (-0.22522,-0.165467)\n",
+                        " (-0.151059,0.481251)\n",
+                        " (-0.450874,0.172713)\n",
+                        " (-0.0585584,0.32498)\n",
+                        " (0.359721,0.0264336)\n",
+                        "(-0.101035,-0.356517)\n",
+                        "\n",
+                        " *** Quantum State ***\n",
+                        " * Qubit Count : 3\n",
+                        " * Dimension   : 8\n",
+                        " * State vector : \n",
+                        "(-0.0845729,-0.14143)\n",
+                        "  (-0.133864,0.11328)\n",
+                        " (-0.22522,-0.165467)\n",
+                        "(-0.101035,-0.356517)\n",
+                        " (-0.450874,0.172713)\n",
+                        " (-0.0585584,0.32498)\n",
+                        " (0.359721,0.0264336)\n",
+                        " (-0.151059,0.481251)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from qulacs import QuantumState\n",
+                "from qulacs.gate import TOFFOLI\n",
+                "\n",
+                "n = 3\n",
+                "state = QuantumState(n)\n",
+                "\n",
+                "state.set_Haar_random_state(0)\n",
+                "print(state)\n",
+                "\n",
+                "toffoli_gate = TOFFOLI(0, 1, 2)\n",
+                "\n",
+                "toffoli_gate.update_quantum_state(state)\n",
+                "\n",
+                "print(state)\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "#### FREDKIN gate\n",
+                "\n",
+                "FREDKIN gate has control indices in the first argument, and target indices in the second and third arguments.\n",
+                "When the qubit corresponding to the control index given in the first argument is $\\ket{1}$, the qubits corresponding to the target indices given in the second and third arguments are swapped."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from qulacs.gate import FREDKIN\n",
+                "control1 = 0\n",
+                "target1 = 1\n",
+                "target2 = 2\n",
+                "fredkin_gate = FREDKIN(control1, target1, target2)\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Here is an example of the operation of the FREDKIN gate. Since 0 is given as the control index and 1 and 2 are given as the target indices, the qubits of the 1-st qubit and the 2-nd qubit are swapped when the 0-th qubit is $\\ket{1}$."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        " *** Quantum State ***\n",
+                        " * Qubit Count : 3\n",
+                        " * Dimension   : 8\n",
+                        " * State vector : \n",
+                        "(-0.0845729,-0.14143)\n",
+                        "  (-0.133864,0.11328)\n",
+                        " (-0.22522,-0.165467)\n",
+                        " (-0.151059,0.481251)\n",
+                        " (-0.450874,0.172713)\n",
+                        " (-0.0585584,0.32498)\n",
+                        " (0.359721,0.0264336)\n",
+                        "(-0.101035,-0.356517)\n",
+                        "\n",
+                        " *** Quantum State ***\n",
+                        " * Qubit Count : 3\n",
+                        " * Dimension   : 8\n",
+                        " * State vector : \n",
+                        "(-0.0845729,-0.14143)\n",
+                        "  (-0.133864,0.11328)\n",
+                        " (-0.22522,-0.165467)\n",
+                        " (-0.0585584,0.32498)\n",
+                        " (-0.450874,0.172713)\n",
+                        " (-0.151059,0.481251)\n",
+                        " (0.359721,0.0264336)\n",
+                        "(-0.101035,-0.356517)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from qulacs import QuantumState\n",
+                "from qulacs.gate import FREDKIN\n",
+                "\n",
+                "n = 3\n",
+                "state = QuantumState(n)\n",
+                "\n",
+                "state.set_Haar_random_state(0)\n",
+                "print(state)\n",
+                "\n",
+                "fredkin_gate = FREDKIN(0, 1, 2)\n",
+                "\n",
+                "fredkin_gate.update_quantum_state(state)\n",
+                "\n",
+                "print(state)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### General quantum gates"
@@ -596,15 +769,15 @@
                     ]
                 }
             ],
             "source": [
                 "from qulacs.gate import DenseMatrix\n",
                 "\n",
                 "gate = DenseMatrix(1, [[0,1],[1,0]])\n",
-                "print(gate)"
+                "print(gate)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "To create a gate of size larger than 2 qubits, give a list of target subscripts as the first argument and a matrix as the second. When creating an $n$-qubit gate, the matrix must be of dimension $2^n$."
@@ -639,15 +812,15 @@
                     ]
                 }
             ],
             "source": [
                 "from qulacs.gate import DenseMatrix\n",
                 "\n",
                 "gate = DenseMatrix([0,1], [[0,1,0,0],[1,0,0,0],[0,0,0,1],[0,0,1,0]])\n",
-                "print(gate)"
+                "print(gate)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Note that the indices that are lower bits when counting the columns and rows of a gated matrix correspond to the order of the subscripts given during gate generation, so the list of subscripts acting in the above example has a different meaning for `[0,1]` and `[1,0]`. The following shows the difference when the indices are swapped."
@@ -677,15 +850,15 @@
                 "\n",
                 "state.set_zero_state()\n",
                 "gate1.update_quantum_state(state)\n",
                 "print(state.get_vector())\n",
                 "\n",
                 "state.set_zero_state()\n",
                 "gate2.update_quantum_state(state)\n",
-                "print(state.get_vector())"
+                "print(state.get_vector())\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Append a control bit"
@@ -726,21 +899,22 @@
                 }
             ],
             "source": [
                 "from qulacs.gate import DenseMatrix\n",
                 "\n",
                 "gate = DenseMatrix(1, [[0,1],[1,0]])\n",
                 "gate.add_control_qubit(3,1)\n",
-                "print(gate)"
+                "print(gate)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "### Conversion to General Matrix Gates\n",
                 "While special named gates such as X gates can update quantum states faster than general matrix gates, they cannot be modified with functions like the `add_control_qubit`. To process a gate based on a special gate, use the `to_matrix_gate` function to convert the special gate to a general gate."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 58,
             "metadata": {},
@@ -780,15 +954,76 @@
             "source": [
                 "from qulacs.gate import X, to_matrix_gate\n",
                 "\n",
                 "gate = X(1)\n",
                 "print(gate)\n",
                 "gate = to_matrix_gate(gate)\n",
                 "print(gate)\n",
-                "gate.add_control_qubit(3,1)"
+                "gate.add_control_qubit(3,1)\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Merge quantum gates\n",
+                "\n",
+                "You can merge multiple gates using the `merge` function in the `qulacs.gate` module. The merged gate behaves the same as when each gate is applied in order."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        " *** Quantum State ***\n",
+                        " * Qubit Count : 2\n",
+                        " * Dimension   : 4\n",
+                        " * State vector : \n",
+                        "(0,-1)\n",
+                        "(0,-0)\n",
+                        " (0,0)\n",
+                        " (0,0)\n",
+                        "\n",
+                        " *** Quantum State ***\n",
+                        " * Qubit Count : 2\n",
+                        " * Dimension   : 4\n",
+                        " * State vector : \n",
+                        "(0,-1)\n",
+                        " (0,0)\n",
+                        " (0,0)\n",
+                        " (0,0)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from qulacs import QuantumState\n",
+                "from qulacs.gate import X, Y, merge\n",
+                "\n",
+                "n = 2\n",
+                "state1 = QuantumState(n)\n",
+                "\n",
+                "index = 1\n",
+                "x_gate = X(index)\n",
+                "y_gate = Y(index)\n",
+                "\n",
+                "x_gate.update_quantum_state(state1)\n",
+                "y_gate.update_quantum_state(state1)\n",
+                "print(state1)\n",
+                "\n",
+                "state2 = QuantumState(n)\n",
+                "\n",
+                "merged_gate = merge([x_gate, y_gate])\n",
+                "merged_gate.update_quantum_state(state2)\n",
+                "print(state2)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Obtain a gate matrix from a quantum gate"
@@ -821,15 +1056,15 @@
                 "from qulacs.gate import H, CNOT\n",
                 "\n",
                 "h_gate = H(2)\n",
                 "matrix = h_gate.get_matrix()\n",
                 "print(matrix)\n",
                 "cnot_gate = CNOT(1,2)\n",
                 "matrix = cnot_gate.get_matrix()\n",
-                "print(matrix)"
+                "print(matrix)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Obtain a inverse gate from a quantum gate\n",
@@ -865,15 +1100,15 @@
                 "print(\"inversed:\\n\", s_dagger_gate.get_matrix())\n",
                 "\n",
                 "noise_gate = DepolarizingNoise(0, 0.05)\n",
                 "try:\n",
                 "        noise_gate.get_inverse()\n",
                 "        assert 0, \"No exception occured. should not reach here.\"\n",
                 "except Exception as err:\n",
-                "        print(f\"Exception occured as expected: {err}\")"
+                "        print(f\"Exception occured as expected: {err}\")\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -924,15 +1159,15 @@
                 "circuit.add_H_gate(0)\n",
                 "circuit.add_X_gate(2)\n",
                 "\n",
                 "from qulacs.gate import X\n",
                 "gate = X(2)\n",
                 "circuit.add_gate(gate)\n",
                 "\n",
-                "print(circuit)"
+                "print(circuit)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Note: The quantum circuit added by `add_gate` is released from memory when the quantum circuit is released. Therefore, the assigned gate cannot be reused. If you want to reuse the gate given as an argument, make a copy of itself using `gate.copy` or use the `add_gate_copy` function."
@@ -984,15 +1219,15 @@
                 "circuit = QuantumCircuit(n)\n",
                 "circuit.add_H_gate(1)\n",
                 "circuit.add_RX_gate(2,0.1)\n",
                 "\n",
                 "from qulacs import QuantumState\n",
                 "state = QuantumState(n)\n",
                 "circuit.update_quantum_state(state)\n",
-                "print(state)"
+                "print(state)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Obtain a inverse circuit from a quantum circuit\n",
@@ -1036,15 +1271,15 @@
                 "\n",
                 "inverse_circuit = circuit.get_inverse()\n",
                 "\n",
                 "from qulacs import QuantumState\n",
                 "state = QuantumState(n)\n",
                 "circuit.update_quantum_state(state)\n",
                 "inverse_circuit.update_quantum_state(state)\n",
-                "print(state)"
+                "print(state)\n"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.9.10 64-bit",
             "language": "python",
@@ -1056,15 +1291,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.10"
+            "version": "3.11.4"
         },
         "vscode": {
             "interpreter": {
                 "hash": "949777d72b0d2535278d3dc13498b2535136f6dfe0678499012e853ee9abcab1"
             }
         }
     },
```

### Comparing `qulacs-0.6.3/doc/en/source/intro/4.2_cpp_tutorial.md` & `qulacs-0.6.4/doc/en/source/intro/4.2_cpp_tutorial.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/en/source/write/0_readme.md` & `qulacs-0.6.4/doc/en/source/write/0_readme.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/Makefile` & `qulacs-0.6.4/doc/ja/Makefile`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/make.bat` & `qulacs-0.6.4/doc/ja/make.bat`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/source/_static/images/dojo.png` & `qulacs-0.6.4/doc/ja/source/_static/images/dojo.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/source/_static/images/github.png` & `qulacs-0.6.4/doc/ja/source/_static/images/github.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/source/_static/images/logo-c-h.png` & `qulacs-0.6.4/doc/ja/source/_static/images/logo-c-h.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/source/_static/images/slack.png` & `qulacs-0.6.4/doc/ja/source/_static/images/slack.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/class.rst` & `qulacs-0.6.4/doc/ja/source/_templates/autoapi/python/class.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/data.rst` & `qulacs-0.6.4/doc/ja/source/_templates/autoapi/python/data.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/function.rst` & `qulacs-0.6.4/doc/ja/source/_templates/autoapi/python/function.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/method.rst` & `qulacs-0.6.4/doc/ja/source/_templates/autoapi/python/method.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/source/_templates/autoapi/python/module.rst` & `qulacs-0.6.4/doc/ja/source/_templates/autoapi/python/module.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/source/conf.py` & `qulacs-0.6.4/doc/ja/source/conf.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/source/guide/2.0_python_advanced.md` & `qulacs-0.6.4/doc/ja/source/guide/2.0_python_advanced.md`

 * *Files 2% similar despite different names*

```diff
@@ -1773,14 +1773,49 @@
 ```python
 from qulacs.gate import Measurement
 target = 0
 classical_pos = 0
 gate = Measurement(target, classical_pos)
 ```
 
+#### ProbabilisticInstrument
+`Probabilistic` 関数に加え、作用したゲートの添え字を取得することができる関数です。distributionの総和が1未満であるなどの理由でどのゲートも作用しなかった場合、`gate_list` の要素数が `classical_address` に保存されます。
+
+```python
+from qulacs import QuantumState
+from qulacs.gate import X, Y, H, ProbabilisticInstrument
+n = 2
+state = QuantumState(n)
+index = 0
+x_gate = X(index)
+y_gate = Y(index)
+h_gate = H(index)
+distribution = [0.25, 0.25, 0.25]
+gate_list = [x_gate, y_gate, h_gate]
+classical_address = 0
+for _ in range(10):
+  state = QuantumState(n)
+  probabilistic_instrument_gate = ProbabilisticInstrument(distribution, gate_list, classical_address)
+  probabilistic_instrument_gate.update_quantum_state(state)
+  result = state.get_classical_value(classical_address)
+  print(result, state.get_vector())
+```
+```
+0 [0.+0.j 1.+0.j 0.+0.j 0.+0.j]
+1 [0.-0.j 0.+1.j 0.-0.j 0.+0.j]
+2 [0.70710678+0.j 0.70710678+0.j 0.        +0.j 0.        +0.j]
+0 [0.+0.j 1.+0.j 0.+0.j 0.+0.j]
+2 [0.70710678+0.j 0.70710678+0.j 0.        +0.j 0.        +0.j]
+1 [0.-0.j 0.+1.j 0.-0.j 0.+0.j]
+3 [1.+0.j 0.+0.j 0.+0.j 0.+0.j]
+2 [0.70710678+0.j 0.70710678+0.j 0.        +0.j 0.        +0.j]
+3 [1.+0.j 0.+0.j 0.+0.j 0.+0.j]
+0 [0.+0.j 1.+0.j 0.+0.j 0.+0.j]
+```
+
 #### Adaptive操作
 
 古典レジスタの値の可変長リストを引数としブール値を返す関数を用いて、古典レジスタから求まる条件に応じて操作を行うか決定するゲートです。条件はPythonの関数として記述することができます。
 Pythonの関数は `int` 型のリストを引数として受け取り、`bool` 型を返す関数でなくてはなりません。
 
 ```python
 from qulacs.gate import Adaptive, X
```

### Comparing `qulacs-0.6.3/doc/ja/source/index.md` & `qulacs-0.6.4/doc/ja/source/index.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/source/intro/0_about.md` & `qulacs-0.6.4/doc/ja/source/intro/0_about.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/source/intro/1_install.md` & `qulacs-0.6.4/doc/ja/source/intro/1_install.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/source/intro/2_faq.md` & `qulacs-0.6.4/doc/ja/source/intro/2_faq.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/source/intro/3_usage.md` & `qulacs-0.6.4/doc/ja/source/intro/3_usage.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/ja/source/intro/4.1_python_tutorial.md` & `qulacs-0.6.4/doc/ja/source/intro/4.1_python_tutorial.md`

 * *Files 13% similar despite different names*

```diff
@@ -267,14 +267,141 @@
 control = 1
 target2 = 1
 cnot_gate = CNOT(control, target)
 cz_gate = CZ(control, target)
 swap_gate = SWAP(target, target2)
 ```
 
+ここでは名前のついたいくつかのゲートについて、動作説明と共に紹介します。
+
+#### TOFFOLIゲート
+
+TOFFOLIゲートは第1, 2引数にコントロールindexを、第3引数にターゲットのindexをもちます。
+第1, 2引数で与えられたコントロールindexに対応する量子ビットがどちらも $\ket{1}$ のときに、第3引数で与えられたターゲットindexに対応する量子ビットが反転します。
+
+```python
+# TOFFOLIゲート
+from qulacs.gate import TOFFOLI
+control1 = 0
+control2 = 1
+target1 = 1
+toffoli_gate = TOFFOLI(control1, control2, target1)
+```
+
+下記にTOFFOLIゲートの動作の例を示しています。コントロールindexとして0, 1、ターゲットのindexとして2を与えられているため、0-th qubitと1-st qubitが $\ket{1}$ のときに2-nd qubitの量子ビットが反転します。
+TOFFOLIゲートの作用前と作用後では、 $\ket{011}$ と $\ket{111}$ の量子状態が入れ替わっていることが分かります。
+
+```python
+from qulacs import QuantumState
+from qulacs.gate import TOFFOLI
+
+n = 3
+state = QuantumState(n)
+
+state.set_Haar_random_state(0)
+print(state)
+
+toffoli_gate = TOFFOLI(0, 1, 2)
+
+toffoli_gate.update_quantum_state(state)
+
+print(state)
+
+del state
+```
+
+```
+*** Quantum State ***
+ * Qubit Count : 3
+ * Dimension   : 8
+ * State vector : 
+(-0.0845729,-0.14143)
+  (-0.133864,0.11328)
+ (-0.22522,-0.165467)
+ (-0.151059,0.481251)
+ (-0.450874,0.172713)
+ (-0.0585584,0.32498)
+ (0.359721,0.0264336)
+(-0.101035,-0.356517)
+
+ *** Quantum State ***
+ * Qubit Count : 3
+ * Dimension   : 8
+ * State vector : 
+(-0.0845729,-0.14143)
+  (-0.133864,0.11328)
+ (-0.22522,-0.165467)
+(-0.101035,-0.356517)
+ (-0.450874,0.172713)
+ (-0.0585584,0.32498)
+ (0.359721,0.0264336)
+ (-0.151059,0.481251)
+```
+
+#### FREDKINゲート
+
+FREDKINゲートは第1引数にコントロールindexを、第2, 3引数にターゲットのindexをもちます。
+第1引数で与えられたコントロールindexに対応する量子ビットが $\ket{1}$ のときに、第2, 3引数で与えられたターゲットindexに対応する量子ビットが入れ替わります。
+
+```python
+# FREDKINゲート
+from qulacs.gate import FREDKIN
+control1 = 0
+target1 = 1
+target2 = 2
+fredkin_gate = FREDKIN(control1, target1, target2)
+```
+
+下記にFREDKINゲートの動作の例を示しています。コントロールindexとして0、ターゲットのindexとして1, 2を与えられているため、0-th qubitが $\ket{1}$ のときに1-st qubit, 2-nd qubitの量子ビットが入れ替わります。FREDKINゲートの作用前と作用後では、 $\ket{011}$ と $\ket{101} $の量子状態が入れ替わっていることが分かります。
+
+```python
+from qulacs import QuantumState
+from qulacs.gate import FREDKIN
+
+n = 3
+state = QuantumState(n)
+
+state.set_Haar_random_state(0)
+print(state)
+
+fredkin_gate = FREDKIN(0, 1, 2)
+
+fredkin_gate.update_quantum_state(state)
+
+print(state)
+```
+
+```
+ *** Quantum State ***
+ * Qubit Count : 3
+ * Dimension   : 8
+ * State vector : 
+(-0.0845729,-0.14143)
+  (-0.133864,0.11328)
+ (-0.22522,-0.165467)
+ (-0.151059,0.481251)
+ (-0.450874,0.172713)
+ (-0.0585584,0.32498)
+ (0.359721,0.0264336)
+(-0.101035,-0.356517)
+
+ *** Quantum State ***
+ * Qubit Count : 3
+ * Dimension   : 8
+ * State vector : 
+(-0.0845729,-0.14143)
+  (-0.133864,0.11328)
+ (-0.22522,-0.165467)
+ (-0.0585584,0.32498)
+ (-0.450874,0.172713)
+ (-0.151059,0.481251)
+ (0.359721,0.0264336)
+(-0.101035,-0.356517)
+```
+
 ### 一般的な量子ゲート
 
 量子ゲートの行列をnumpy arrayで指定してゲートを生成するには、`DenseMatrix` クラスを用います。一つ目の引数が作用する添え字で、二つ目が行列です。1量子ビットゲートの場合は一つの整数と2×2行列を与えます。
 
 ```python
 from qulacs.gate import DenseMatrix
 
@@ -418,14 +545,60 @@
  * Matrix
 (0,0) (1,0)
 (1,0) (0,0)
 ```
 
 変換によりゲート名が `X` から `DenseMatrix` に変わり陽にゲート行列を保持していることが分かります。
 
+### 量子ゲートの合成
+
+`qulacs.gate` モジュール内に存在する `merge` 関数を用いることで複数のゲートを合成できます。合成したゲートは各ゲートを順番に作用させた場合と同じ立ち振る舞いをします。
+
+```python
+from qulacs import QuantumState
+from qulacs.gate import X, Y, merge
+
+n = 2
+state1 = QuantumState(n)
+
+index = 1
+x_gate = X(index)
+y_gate = Y(index)
+
+x_gate.update_quantum_state(state1)
+y_gate.update_quantum_state(state1)
+print(state1)
+
+state2 = QuantumState(n)
+
+merged_gate = merge([x_gate, y_gate])
+merged_gate.update_quantum_state(state2)
+print(state2)
+```
+
+```
+*** Quantum State ***
+ * Qubit Count : 2
+ * Dimension   : 4
+ * State vector : 
+(0,-1)
+(0,-0)
+ (0,0)
+ (0,0)
+
+ *** Quantum State ***
+ * Qubit Count : 2
+ * Dimension   : 4
+ * State vector : 
+(0,-1)
+ (0,0)
+ (0,0)
+ (0,0)
+```
+
 ### 量子ゲートのゲート行列の取得
 
 生成した量子ゲートのゲート行列は `get_matrix` 関数で取得できます。なお重要な注意点として、controlled-qubitがあるゲートの場合、controlled-qubitはゲート行列には含まれません。このため、例えばCNOTゲートのゲート行列は2x2行列になります。
 
 ```python
 from qulacs.gate import H, CNOT
```

### Comparing `qulacs-0.6.3/doc/ja/source/intro/4.2_cpp_tutorial.md` & `qulacs-0.6.4/doc/ja/source/intro/4.2_cpp_tutorial.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/scripts/customdoxygen.css` & `qulacs-0.6.4/doc/scripts/customdoxygen.css`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/scripts/doxy-boot.js` & `qulacs-0.6.4/doc/scripts/doxy-boot.js`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/scripts/footer.html` & `qulacs-0.6.4/doc/scripts/footer.html`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/scripts/header.html` & `qulacs-0.6.4/doc/scripts/header.html`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/doc/scripts/index.html` & `qulacs-0.6.4/doc/scripts/index.html`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/pyproject.toml` & `qulacs-0.6.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -58,18 +58,19 @@
     "mypy",
     "pybind11-stubgen",
     "openfermion",
     "pytest"
 ]
 
 doc = [
+    "mypy",
+    "pybind11-stubgen",
     "sphinx==7.*",
     "sphinx-rtd-theme",
     "breathe",
-    #"exhale@git+https://github.com/svenevs/exhale.git@fix/packaging-requirements", # workaround until https://github.com/svenevs/exhale/pull/205 is merged
     "exhale",
     "nbsphinx",
     "myst-parser",
     "sphinx-copybutton",
     "ipykernel",
     "sphinx-autoapi==3.*"
 ]
```

### Comparing `qulacs-0.6.3/pysrc/qulacs/__init__.pyi` & `qulacs-0.6.4/pysrc/qulacs/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,20 @@
 """
 cppsim python interface
 """
 from __future__ import annotations
-
-import typing
-
 import numpy
 import scipy.sparse
-
-from . import circuit, gate, observable, quantum_operator, state
-
-__all__ = [
-    "CausalConeSimulator",
-    "ClsNoisyEvolution",
-    "ClsNoisyEvolution_fast",
-    "ClsNpairQubitGate",
-    "ClsOneControlOneTargetGate",
-    "ClsOneQubitGate",
-    "ClsOneQubitRotationGate",
-    "ClsPauliGate",
-    "ClsPauliRotationGate",
-    "ClsReversibleBooleanGate",
-    "ClsStateReflectionGate",
-    "ClsTwoQubitGate",
-    "DensityMatrix",
-    "GeneralQuantumOperator",
-    "GradCalculator",
-    "NoiseSimulator",
-    "Observable",
-    "ParametricQuantumCircuit",
-    "PauliOperator",
-    "QuantumCircuit",
-    "QuantumCircuitSimulator",
-    "QuantumGateBase",
-    "QuantumGateDiagonalMatrix",
-    "QuantumGateMatrix",
-    "QuantumGateSparseMatrix",
-    "QuantumGate_Adaptive",
-    "QuantumGate_CP",
-    "QuantumGate_CPTP",
-    "QuantumGate_Probabilistic",
-    "QuantumGate_SingleParameter",
-    "QuantumState",
-    "QuantumStateBase",
-    "SimulationResult",
-    "StateVector",
-    "check_build_for_mpi",
-    "circuit",
-    "gate",
-    "observable",
-    "quantum_operator",
-    "state",
-    "to_general_quantum_operator",
-]
-
+import typing
+from . import circuit
+from . import gate
+from . import observable
+from . import quantum_operator
+from . import state
+__all__ = ['CausalConeSimulator', 'ClsNoisyEvolution', 'ClsNoisyEvolution_fast', 'ClsNpairQubitGate', 'ClsOneControlOneTargetGate', 'ClsOneQubitGate', 'ClsOneQubitRotationGate', 'ClsPauliGate', 'ClsPauliRotationGate', 'ClsReversibleBooleanGate', 'ClsStateReflectionGate', 'ClsTwoQubitGate', 'DensityMatrix', 'GeneralQuantumOperator', 'GradCalculator', 'NoiseSimulator', 'Observable', 'ParametricQuantumCircuit', 'PauliOperator', 'QuantumCircuit', 'QuantumCircuitSimulator', 'QuantumGateBase', 'QuantumGateDiagonalMatrix', 'QuantumGateMatrix', 'QuantumGateSparseMatrix', 'QuantumGate_Adaptive', 'QuantumGate_CP', 'QuantumGate_CPTP', 'QuantumGate_Probabilistic', 'QuantumGate_SingleParameter', 'QuantumState', 'QuantumStateBase', 'SimulationResult', 'StateVector', 'check_build_for_mpi', 'circuit', 'gate', 'observable', 'quantum_operator', 'state', 'to_general_quantum_operator']
 class CausalConeSimulator:
     def __init__(self, arg0: ParametricQuantumCircuit, arg1: Observable) -> None:
         """
         Constructor
         """
     def build(self) -> None:
         """
@@ -75,55 +32,45 @@
         """
         Return expectation_value
         """
     def get_pauli_operator_list(self) -> list[list[PauliOperator]]:
         """
         Return pauli_operator_list
         """
-
 class ClsNoisyEvolution(QuantumGateBase):
     pass
-
 class ClsNoisyEvolution_fast(QuantumGateBase):
     pass
-
 class ClsNpairQubitGate(QuantumGateBase):
     pass
-
 class ClsOneControlOneTargetGate(QuantumGateBase):
     pass
-
 class ClsOneQubitGate(QuantumGateBase):
     pass
-
 class ClsOneQubitRotationGate(QuantumGateBase):
     pass
-
 class ClsPauliGate(QuantumGateBase):
     pass
-
 class ClsPauliRotationGate(QuantumGateBase):
     pass
-
 class ClsReversibleBooleanGate(QuantumGateBase):
     pass
-
 class ClsStateReflectionGate(QuantumGateBase):
     pass
-
 class ClsTwoQubitGate(QuantumGateBase):
     pass
-
 class DensityMatrix(QuantumStateBase):
-    def __getstate__(self) -> str: ...
+    def __getstate__(self) -> str:
+        ...
     def __init__(self, qubit_count: int) -> None:
         """
         Constructor
         """
-    def __setstate__(self, arg0: str) -> None: ...
+    def __setstate__(self, arg0: str) -> None:
+        ...
     def __str__(self) -> str:
         """
         to string
         """
     def add_state(self, state: QuantumStateBase) -> None:
         """
         Add state vector to this state
@@ -227,47 +174,60 @@
         """
         to json string
         """
     def to_string(self) -> str:
         """
         to string
         """
-
 class GeneralQuantumOperator:
-    def __IADD__(self, arg0: PauliOperator) -> GeneralQuantumOperator: ...
-    @typing.overload
-    def __IMUL__(self, arg0: PauliOperator) -> GeneralQuantumOperator: ...
-    @typing.overload
-    def __IMUL__(self, arg0: complex) -> GeneralQuantumOperator: ...
-    def __ISUB__(self, arg0: PauliOperator) -> GeneralQuantumOperator: ...
+    def __IADD__(self, arg0: PauliOperator) -> GeneralQuantumOperator:
+        ...
     @typing.overload
-    def __add__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator: ...
+    def __IMUL__(self, arg0: PauliOperator) -> GeneralQuantumOperator:
+        ...
     @typing.overload
-    def __add__(self, arg0: PauliOperator) -> GeneralQuantumOperator: ...
-    def __iadd__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator: ...
-    def __imul__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator: ...
+    def __IMUL__(self, arg0: complex) -> GeneralQuantumOperator:
+        ...
+    def __ISUB__(self, arg0: PauliOperator) -> GeneralQuantumOperator:
+        ...
+    @typing.overload
+    def __add__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator:
+        ...
+    @typing.overload
+    def __add__(self, arg0: PauliOperator) -> GeneralQuantumOperator:
+        ...
+    def __iadd__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator:
+        ...
+    def __imul__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator:
+        ...
     def __init__(self, qubit_count: int) -> None:
         """
         Constructor
         """
-    def __isub__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator: ...
+    def __isub__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator:
+        ...
     @typing.overload
-    def __mul__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator: ...
+    def __mul__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator:
+        ...
     @typing.overload
-    def __mul__(self, arg0: PauliOperator) -> GeneralQuantumOperator: ...
+    def __mul__(self, arg0: PauliOperator) -> GeneralQuantumOperator:
+        ...
     @typing.overload
-    def __mul__(self, arg0: complex) -> GeneralQuantumOperator: ...
+    def __mul__(self, arg0: complex) -> GeneralQuantumOperator:
+        ...
     def __str__(self) -> str:
         """
         to string
         """
     @typing.overload
-    def __sub__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator: ...
+    def __sub__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator:
+        ...
     @typing.overload
-    def __sub__(self, arg0: PauliOperator) -> GeneralQuantumOperator: ...
+    def __sub__(self, arg0: PauliOperator) -> GeneralQuantumOperator:
+        ...
     @typing.overload
     def add_operator(self, pauli_operator: PauliOperator) -> None:
         """
         Add Pauli operator
         """
     @typing.overload
     def add_operator(self, coef: complex, pauli_string: str) -> None:
@@ -279,27 +239,20 @@
         Add Pauli operator
         """
     def add_operator_move(self, pauli_operator: PauliOperator) -> None:
         """
         Add Pauli operator
         """
     @typing.overload
-    def apply_to_state(
-        self,
-        work_state: QuantumStateBase,
-        state_to_be_multiplied: QuantumStateBase,
-        dst_state: QuantumStateBase,
-    ) -> None:
+    def apply_to_state(self, work_state: QuantumStateBase, state_to_be_multiplied: QuantumStateBase, dst_state: QuantumStateBase) -> None:
         """
         Apply observable to `state_to_be_multiplied`. The result is stored into `dst_state`.
         """
     @typing.overload
-    def apply_to_state(
-        self, state_to_be_multiplied: QuantumStateBase, dst_state: QuantumStateBase
-    ) -> None:
+    def apply_to_state(self, state_to_be_multiplied: QuantumStateBase, dst_state: QuantumStateBase) -> None:
         """
         Apply observable to `state_to_be_multiplied`. The result is stored into `dst_state`.
         """
     def copy(self) -> GeneralQuantumOperator:
         """
         Create copied instance of General Quantum operator class
         """
@@ -327,63 +280,52 @@
         """
         Get Pauli term
         """
     def get_term_count(self) -> int:
         """
         Get count of Pauli terms
         """
-    def get_transition_amplitude(
-        self, state_bra: QuantumStateBase, state_ket: QuantumStateBase
-    ) -> complex:
+    def get_transition_amplitude(self, state_bra: QuantumStateBase, state_ket: QuantumStateBase) -> complex:
         """
         Get transition amplitude
         """
     def is_hermitian(self) -> bool:
         """
         Get is Herimitian
         """
     def to_json(self) -> str:
         """
         to json string
         """
-
 class GradCalculator:
-    def __init__(self) -> None: ...
+    def __init__(self) -> None:
+        ...
     @typing.overload
-    def calculate_grad(
-        self, parametric_circuit: ParametricQuantumCircuit, observable: Observable
-    ) -> list[complex]:
+    def calculate_grad(self, parametric_circuit: ParametricQuantumCircuit, observable: Observable) -> list[complex]:
         """
         Calculate Grad
         """
     @typing.overload
-    def calculate_grad(
-        self,
-        parametric_circuit: ParametricQuantumCircuit,
-        observable: Observable,
-        angles_of_gates: list[float],
-    ) -> list[complex]:
+    def calculate_grad(self, parametric_circuit: ParametricQuantumCircuit, observable: Observable, angles_of_gates: list[float]) -> list[complex]:
         """
         Calculate Grad
         """
-
 class NoiseSimulator:
     def __init__(self, arg0: QuantumCircuit, arg1: QuantumState) -> None:
         """
         Constructor
         """
     def execute(self, arg0: int) -> list[int]:
         """
         Sampling & Return result [array]
         """
     def execute_and_get_result(self, arg0: int) -> SimulationResult:
         """
         Simulate & Return ressult [array of (state, frequency)]
         """
-
 class Observable(GeneralQuantumOperator):
     def __init__(self, qubit_count: int) -> None:
         """
         Constructor
         """
     def __str__(self) -> str:
         """
@@ -413,20 +355,15 @@
         Add random pauli operator
         """
     @typing.overload
     def add_random_operator(self, operator_count: int, seed: int) -> None:
         """
         Add random pauli operator
         """
-    def apply_to_state(
-        self,
-        work_state: QuantumStateBase,
-        state_to_be_multiplied: QuantumStateBase,
-        dst_state: QuantumStateBase,
-    ) -> None:
+    def apply_to_state(self, work_state: QuantumStateBase, state_to_be_multiplied: QuantumStateBase, dst_state: QuantumStateBase) -> None:
         """
         Apply observable to `state_to_be_multiplied`. The result is stored into `dst_state`.
         """
     def get_expectation_value(self, state: QuantumStateBase) -> float:
         """
         Get expectation value
         """
@@ -446,46 +383,39 @@
         """
         Get Pauli term
         """
     def get_term_count(self) -> int:
         """
         Get count of Pauli terms
         """
-    def get_transition_amplitude(
-        self, state_bra: QuantumStateBase, state_ket: QuantumStateBase
-    ) -> complex:
+    def get_transition_amplitude(self, state_bra: QuantumStateBase, state_ket: QuantumStateBase) -> complex:
         """
         Get transition amplitude
         """
-    def solve_ground_state_eigenvalue_by_arnoldi_method(
-        self, state: QuantumStateBase, iter_count: int, mu: complex = 0.0
-    ) -> complex:
+    def solve_ground_state_eigenvalue_by_arnoldi_method(self, state: QuantumStateBase, iter_count: int, mu: complex = 0.0) -> complex:
         """
         Compute ground state eigenvalue by arnoldi method
         """
-    def solve_ground_state_eigenvalue_by_lanczos_method(
-        self, state: QuantumStateBase, iter_count: int, mu: complex = 0.0
-    ) -> complex:
+    def solve_ground_state_eigenvalue_by_lanczos_method(self, state: QuantumStateBase, iter_count: int, mu: complex = 0.0) -> complex:
         """
         Compute ground state eigenvalue by lanczos method
         """
-    def solve_ground_state_eigenvalue_by_power_method(
-        self, state: QuantumStateBase, iter_count: int, mu: complex = 0.0
-    ) -> complex:
+    def solve_ground_state_eigenvalue_by_power_method(self, state: QuantumStateBase, iter_count: int, mu: complex = 0.0) -> complex:
         """
         Compute ground state eigenvalue by power method
         """
-
 class ParametricQuantumCircuit(QuantumCircuit):
-    def __getstate__(self) -> str: ...
+    def __getstate__(self) -> str:
+        ...
     def __init__(self, qubit_count: int) -> None:
         """
         Constructor
         """
-    def __setstate__(self, arg0: str) -> None: ...
+    def __setstate__(self, arg0: str) -> None:
+        ...
     def __str__(self) -> str:
         """
         to string
         """
     @typing.overload
     def add_gate(self, gate: QuantumGateBase) -> None:
         """
@@ -510,23 +440,19 @@
         """
     @typing.overload
     def add_parametric_gate(self, gate: QuantumGate_SingleParameter) -> None:
         """
         Add parametric gate
         """
     @typing.overload
-    def add_parametric_gate(
-        self, gate: QuantumGate_SingleParameter, position: int
-    ) -> None:
+    def add_parametric_gate(self, gate: QuantumGate_SingleParameter, position: int) -> None:
         """
         Add parametric gate
         """
-    def add_parametric_multi_Pauli_rotation_gate(
-        self, index_list: list[int], pauli_ids: list[int], angle: float
-    ) -> None:
+    def add_parametric_multi_Pauli_rotation_gate(self, index_list: list[int], pauli_ids: list[int], angle: float) -> None:
         """
         Add parametric multi-qubit Pauli rotation gate
         """
     def backprop(self, obs: GeneralQuantumOperator) -> list[float]:
         """
         Do backprop
         """
@@ -558,42 +484,40 @@
         """
         Remove gate
         """
     def set_parameter(self, index: int, parameter: float) -> None:
         """
         Set parameter
         """
-
 class PauliOperator:
-    def __IMUL__(self, arg0: complex) -> PauliOperator: ...
-    def __imul__(self, arg0: PauliOperator) -> PauliOperator: ...
+    def __IMUL__(self, arg0: complex) -> PauliOperator:
+        ...
+    def __imul__(self, arg0: PauliOperator) -> PauliOperator:
+        ...
     @typing.overload
-    def __init__(self, coef: complex = (1 + 0j)) -> None:
+    def __init__(self, coef: complex = (1+0j)) -> None:
         """
         Constructor
         """
     @typing.overload
-    def __init__(self, pauli_string: str, coef: complex = (1 + 0j)) -> None:
+    def __init__(self, pauli_string: str, coef: complex = (1+0j)) -> None:
         """
         Constructor
         """
     @typing.overload
-    def __init__(
-        self,
-        target_qubit_index_list: list[int],
-        pauli_operator_type_list: str,
-        coef: complex = (1 + 0j),
-    ) -> None:
+    def __init__(self, target_qubit_index_list: list[int], pauli_operator_type_list: str, coef: complex = (1+0j)) -> None:
         """
         Constructor
         """
     @typing.overload
-    def __mul__(self, arg0: PauliOperator) -> PauliOperator: ...
+    def __mul__(self, arg0: PauliOperator) -> PauliOperator:
+        ...
     @typing.overload
-    def __mul__(self, arg0: complex) -> PauliOperator: ...
+    def __mul__(self, arg0: complex) -> PauliOperator:
+        ...
     def add_single_Pauli(self, index: int, pauli_type: int) -> None:
         """
         Add Pauli operator to this term
         """
     def change_coef(self, new_coef: complex) -> None:
         """
         Change coefficient
@@ -622,28 +546,27 @@
         """
         Get list of Pauli IDs (I,X,Y,Z) = (0,1,2,3)
         """
     def get_pauli_string(self) -> str:
         """
         Get pauli string
         """
-    def get_transition_amplitude(
-        self, state_bra: QuantumStateBase, state_ket: QuantumStateBase
-    ) -> complex:
+    def get_transition_amplitude(self, state_bra: QuantumStateBase, state_ket: QuantumStateBase) -> complex:
         """
         Get transition amplitude
         """
-
 class QuantumCircuit:
-    def __getstate__(self) -> str: ...
+    def __getstate__(self) -> str:
+        ...
     def __init__(self, qubit_count: int) -> None:
         """
         Constructor
         """
-    def __setstate__(self, arg0: str) -> None: ...
+    def __setstate__(self, arg0: str) -> None:
+        ...
     def __str__(self) -> str:
         """
         to string
         """
     def add_CNOT_gate(self, control: int, target: int) -> None:
         """
         Add CNOT gate
@@ -673,139 +596,139 @@
         Add Pauli-X rotation gate
         
         Notes
         -----
         Matrix Representation
         
         .. math::
-            R_X(\\theta) = \exp(i\\frac{\\theta}{2} X) =
+            R_X(\\theta) = \\exp(i\\frac{\\theta}{2} X) =
                 \\begin{pmatrix}
-                \cos(\\frac{\\theta}{2})  & i\sin(\\frac{\\theta}{2}) \\\\
-                i\sin(\\frac{\\theta}{2}) & \cos(\\frac{\\theta}{2})
-                \end{pmatrix}
+                \\cos(\\frac{\\theta}{2})  & i\\sin(\\frac{\\theta}{2}) \\\\
+                i\\sin(\\frac{\\theta}{2}) & \\cos(\\frac{\\theta}{2})
+                \\end{pmatrix}
         """
     def add_RY_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-Y rotation gate
         
         Notes
         -----
         Matrix Representation
         
         .. math::
-            R_Y(\\theta) = \exp(i\\frac{\\theta}{2} Y) =
+            R_Y(\\theta) = \\exp(i\\frac{\\theta}{2} Y) =
                 \\begin{pmatrix}
-                \cos(\\frac{\\theta}{2})  & \sin(\\frac{\\theta}{2}) \\\\
-                -\sin(\\frac{\\theta}{2}) & \cos(\\frac{\\theta}{2})
-                \end{pmatrix}
+                \\cos(\\frac{\\theta}{2})  & \\sin(\\frac{\\theta}{2}) \\\\
+                -\\sin(\\frac{\\theta}{2}) & \\cos(\\frac{\\theta}{2})
+                \\end{pmatrix}
         """
     def add_RZ_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-Z rotation gate
         
         Notes
         -----
         Matrix Representation
         
         .. math::
-            R_Z(\\theta) = \exp(i\\frac{\\theta}{2} Z) =
+            R_Z(\\theta) = \\exp(i\\frac{\\theta}{2} Z) =
                 \\begin{pmatrix}
                 e^{i\\frac{\\theta}{2}} & 0 \\\\
                 0 & e^{-i\\frac{\\theta}{2}}
-                \end{pmatrix}
+                \\end{pmatrix}
         """
     def add_RotInvX_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-X rotation gate
         
         Notes
         -----
         Matrix Representation
         
         .. math::
-            R_X(\\theta) = \exp(i\\frac{\\theta}{2} X) =
+            R_X(\\theta) = \\exp(i\\frac{\\theta}{2} X) =
                 \\begin{pmatrix}
-                \cos(\\frac{\\theta}{2})  & i\sin(\\frac{\\theta}{2}) \\\\
-                i\sin(\\frac{\\theta}{2}) & \cos(\\frac{\\theta}{2})
-                \end{pmatrix}
+                \\cos(\\frac{\\theta}{2})  & i\\sin(\\frac{\\theta}{2}) \\\\
+                i\\sin(\\frac{\\theta}{2}) & \\cos(\\frac{\\theta}{2})
+                \\end{pmatrix}
         """
     def add_RotInvY_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-Y rotation gate
         
         Notes
         -----
         Matrix Representation
         
         .. math::
-            R_Y(\\theta) = \exp(i\\frac{\\theta}{2} Y) =
+            R_Y(\\theta) = \\exp(i\\frac{\\theta}{2} Y) =
                 \\begin{pmatrix}
-                \cos(\\frac{\\theta}{2})  & \sin(\\frac{\\theta}{2}) \\\\
-                -\sin(\\frac{\\theta}{2}) & \cos(\\frac{\\theta}{2})
-                \end{pmatrix}
+                \\cos(\\frac{\\theta}{2})  & \\sin(\\frac{\\theta}{2}) \\\\
+                -\\sin(\\frac{\\theta}{2}) & \\cos(\\frac{\\theta}{2})
+                \\end{pmatrix}
         """
     def add_RotInvZ_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-Z rotation gate
         
         Notes
         -----
         Matrix Representation
         
         .. math::
-            R_Z(\\theta) = \exp(i\\frac{\\theta}{2} Z) =
+            R_Z(\\theta) = \\exp(i\\frac{\\theta}{2} Z) =
                 \\begin{pmatrix}
                 e^{i\\frac{\\theta}{2}} & 0 \\\\
                 0 & e^{-i\\frac{\\theta}{2}}
-                \end{pmatrix}
+                \\end{pmatrix}
         """
     def add_RotX_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-X rotation gate
         
         Notes
         -----
         Matrix Representation
         
         .. math::
-            RotX(\\theta) = \exp(-i\\frac{\\theta}{2} X) =
+            RotX(\\theta) = \\exp(-i\\frac{\\theta}{2} X) =
                 \\begin{pmatrix}
-                \cos(\\frac{\\theta}{2})  & -i\sin(\\frac{\\theta}{2}) \\\\
-                -i\sin(\\frac{\\theta}{2}) & \cos(\\frac{\\theta}{2})
-                \end{pmatrix}
+                \\cos(\\frac{\\theta}{2})  & -i\\sin(\\frac{\\theta}{2}) \\\\
+                -i\\sin(\\frac{\\theta}{2}) & \\cos(\\frac{\\theta}{2})
+                \\end{pmatrix}
         """
     def add_RotY_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-Y rotation gate
         
         Notes
         -----
         Matrix Representation
         
         .. math::
-            RotY(\\theta) = \exp(-i\\frac{\\theta}{2} Y) =
+            RotY(\\theta) = \\exp(-i\\frac{\\theta}{2} Y) =
                 \\begin{pmatrix}
-                \cos(\\frac{\\theta}{2})  & -\sin(\\frac{\\theta}{2}) \\\\
-                \sin(\\frac{\\theta}{2}) & \cos(\\frac{\\theta}{2})
-                \end{pmatrix}
+                \\cos(\\frac{\\theta}{2})  & -\\sin(\\frac{\\theta}{2}) \\\\
+                \\sin(\\frac{\\theta}{2}) & \\cos(\\frac{\\theta}{2})
+                \\end{pmatrix}
         """
     def add_RotZ_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-Z rotation gate
         
         Notes
         -----
         Matrix Representation
         
         .. math::
-            RotZ(\\theta) = \exp(-i\\frac{\\theta}{2} Z) =
+            RotZ(\\theta) = \\exp(-i\\frac{\\theta}{2} Z) =
                 \\begin{pmatrix}
                 e^{-i\\frac{\\theta}{2}} & 0 \\\\
                 0 & e^{i\\frac{\\theta}{2}}
-                \end{pmatrix}
+                \\end{pmatrix}
         """
     def add_SWAP_gate(self, target1: int, target2: int) -> None:
         """
         Add SWAP gate
         """
     def add_S_gate(self, index: int) -> None:
         """
@@ -849,23 +772,19 @@
         """
     @typing.overload
     def add_dense_matrix_gate(self, index: int, matrix: numpy.ndarray) -> None:
         """
         Add dense matrix gate
         """
     @typing.overload
-    def add_dense_matrix_gate(
-        self, index_list: list[int], matrix: numpy.ndarray
-    ) -> None:
+    def add_dense_matrix_gate(self, index_list: list[int], matrix: numpy.ndarray) -> None:
         """
         Add dense matrix gate
         """
-    def add_diagonal_observable_rotation_gate(
-        self, observable: Observable, angle: float
-    ) -> None:
+    def add_diagonal_observable_rotation_gate(self, observable: Observable, angle: float) -> None:
         """
         Add diagonal observable rotation gate
         """
     @typing.overload
     def add_gate(self, gate: QuantumGateBase) -> None:
         """
         Add gate with copy
@@ -882,34 +801,28 @@
         """
     @typing.overload
     def add_multi_Pauli_gate(self, pauli: PauliOperator) -> None:
         """
         Add multi-qubit Pauli gate
         """
     @typing.overload
-    def add_multi_Pauli_rotation_gate(
-        self, index_list: list[int], pauli_ids: list[int], angle: float
-    ) -> None:
+    def add_multi_Pauli_rotation_gate(self, index_list: list[int], pauli_ids: list[int], angle: float) -> None:
         """
         Add multi-qubit Pauli rotation gate
         """
     @typing.overload
     def add_multi_Pauli_rotation_gate(self, pauli: PauliOperator) -> None:
         """
         Add multi-qubit Pauli rotation gate
         """
-    def add_noise_gate(
-        self, gate: QuantumGateBase, NoiseType: str, NoiseProbability: float
-    ) -> None:
+    def add_noise_gate(self, gate: QuantumGateBase, NoiseType: str, NoiseProbability: float) -> None:
         """
         Add noise gate with copy
         """
-    def add_observable_rotation_gate(
-        self, observable: Observable, angle: float, repeat: int
-    ) -> None:
+    def add_observable_rotation_gate(self, observable: Observable, angle: float, repeat: int) -> None:
         """
         Add observable rotation gate
         """
     @typing.overload
     def add_random_unitary_gate(self, index_list: list[int]) -> None:
         """
         Add random unitary gate
@@ -955,37 +868,46 @@
         """
         get inverse circuit
         """
     def get_qubit_count(self) -> int:
         """
         Get qubit count
         """
-    def merge_circuit(self, circuit: QuantumCircuit) -> None: ...
+    def merge_circuit(self, circuit: QuantumCircuit) -> None:
+        ...
     def remove_gate(self, position: int) -> None:
         """
         Remove gate
         """
-    def to_json(self) -> str: ...
+    def to_json(self) -> str:
+        ...
     def to_string(self) -> str:
         """
         Get string representation
         """
     @typing.overload
     def update_quantum_state(self, state: QuantumStateBase) -> None:
         """
         Update quantum state
         """
     @typing.overload
-    def update_quantum_state(
-        self, state: QuantumStateBase, start: int, end: int
-    ) -> None:
+    def update_quantum_state(self, state: QuantumStateBase, start: int, end: int) -> None:
+        """
+        Update quantum state
+        """
+    @typing.overload
+    def update_quantum_state(self, state: QuantumStateBase, seed: int) -> None:
+        """
+        Update quantum state
+        """
+    @typing.overload
+    def update_quantum_state(self, state: QuantumStateBase, start: int, end: int, seed: int) -> None:
         """
         Update quantum state
         """
-
 class QuantumCircuitSimulator:
     def __init__(self, circuit: QuantumCircuit, state: QuantumStateBase) -> None:
         """
         Constructor
         """
     def copy_state_from_buffer(self) -> None:
         """
@@ -1025,17 +947,17 @@
         """
         Simulate circuit
         """
     def swap_state_and_buffer(self) -> None:
         """
         Swap state and buffer
         """
-
 class QuantumGateBase:
-    def __str__(self) -> str: ...
+    def __str__(self) -> str:
+        ...
     def copy(self) -> QuantumGateBase:
         """
         Create copied instance
         """
     def get_control_index_list(self) -> list[int]:
         """
         Get control qubit index list
@@ -1096,55 +1018,46 @@
         """
         to string
         """
     def update_quantum_state(self, state: QuantumStateBase) -> None:
         """
         Update quantum state
         """
-
 class QuantumGateDiagonalMatrix(QuantumGateBase):
     pass
-
 class QuantumGateMatrix(QuantumGateBase):
     def add_control_qubit(self, index: int, control_value: int) -> None:
         """
         Add control qubit
         """
     def multiply_scalar(self, value: complex) -> None:
         """
         Multiply scalar value to gate matrix
         """
-
 class QuantumGateSparseMatrix(QuantumGateBase):
     pass
-
 class QuantumGate_Adaptive(QuantumGateBase):
     pass
-
 class QuantumGate_CP(QuantumGateBase):
     def get_gate_list(self) -> list[QuantumGateBase]:
         """
         get_gate_list
         """
-
 class QuantumGate_CPTP(QuantumGateBase):
     """
     QuantumGate_Instrument
     """
-
     def get_gate_list(self) -> list[QuantumGateBase]:
         """
         get_gate_list
         """
-
 class QuantumGate_Probabilistic(QuantumGateBase):
     """
     QuantumGate_ProbabilisticInstrument
     """
-
     def get_cumulative_distribution(self) -> list[float]:
         """
         get_cumulative_distribution
         """
     def get_distribution(self) -> list[float]:
         """
         get_distribution
@@ -1153,42 +1066,42 @@
         """
         get_gate_list
         """
     def optimize_ProbablisticGate(self) -> None:
         """
         optimize_ProbablisticGate
         """
-
 class QuantumGate_SingleParameter(QuantumGateBase):
     def copy(self) -> QuantumGate_SingleParameter:
         """
         Create copied instance
         """
     def get_parameter_value(self) -> float:
         """
         Get parameter value
         """
     def set_parameter_value(self, value: float) -> None:
         """
         Set parameter value
         """
-
 class QuantumState(QuantumStateBase):
-    def __getstate__(self) -> str: ...
+    def __getstate__(self) -> str:
+        ...
     @typing.overload
     def __init__(self, qubit_count: int) -> None:
         """
         Constructor
         """
     @typing.overload
     def __init__(self, qubit_count: int, use_multi_cpu: bool) -> None:
         """
         Constructor
         """
-    def __setstate__(self, arg0: str) -> None: ...
+    def __setstate__(self, arg0: str) -> None:
+        ...
     def __str__(self) -> str:
         """
         to string
         """
     def add_state(self, state: QuantumStateBase) -> None:
         """
         Add state vector to this state
@@ -1247,17 +1160,15 @@
         """
         Load quantum state vector
         """
     def multiply_coef(self, coef: complex) -> None:
         """
         Multiply coefficient to this state
         """
-    def multiply_elementwise_function(
-        self, func: typing.Callable[[int], complex]
-    ) -> None:
+    def multiply_elementwise_function(self, func: typing.Callable[[int], complex]) -> None:
         """
         Multiply elementwise function
         """
     def normalize(self, squared_norm: float) -> None:
         """
         Normalize quantum state
         """
@@ -1297,34 +1208,30 @@
         """
         to json string
         """
     def to_string(self) -> str:
         """
         to string
         """
-
 class QuantumStateBase:
     pass
-
 class SimulationResult:
     def get_count(self) -> int:
         """
         get state count
         """
     def get_frequency(self, arg0: int) -> int:
         """
         get state frequency
         """
     def get_state(self, arg0: int) -> QuantumState:
         """
         get state
         """
-
 def StateVector(arg0: int) -> QuantumState:
     """
     StateVector
     """
-
-def check_build_for_mpi() -> bool: ...
-def to_general_quantum_operator(
-    gate: QuantumGateBase, qubits: int, tol: float
-) -> GeneralQuantumOperator: ...
+def check_build_for_mpi() -> bool:
+    ...
+def to_general_quantum_operator(gate: QuantumGateBase, qubits: int, tol: float) -> GeneralQuantumOperator:
+    ...
```

### Comparing `qulacs-0.6.3/pysrc/qulacs/circuit/__init__.pyi` & `qulacs-0.6.4/pysrc/qulacs/circuit.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 from __future__ import annotations
-
-import typing
-
 import qulacs_core
-import qulacs_core.circuit
-
-__all__ = ["QuantumCircuitOptimizer", "from_json"]
-
+__all__ = ['QuantumCircuitOptimizer', 'from_json']
 class QuantumCircuitOptimizer:
-    def __init__(self) -> None:
+    def __init__(self, mpi_size: int = 0) -> None:
         """
         Constructor
         """
-    def merge_all(
-        self, circuit: qulacs_core.QuantumCircuit
-    ) -> qulacs_core.QuantumGateMatrix: ...
-    def optimize(self, circuit: qulacs_core.QuantumCircuit, block_size: int) -> None:
+    def merge_all(self, circuit: qulacs_core.QuantumCircuit) -> qulacs_core.QuantumGateMatrix:
+        ...
+    def optimize(self, circuit: qulacs_core.QuantumCircuit, block_size: int, swap_level: int = 0) -> None:
         """
         Optimize quantum circuit
         """
-    def optimize_light(self, circuit: qulacs_core.QuantumCircuit) -> None:
+    def optimize_light(self, circuit: qulacs_core.QuantumCircuit, swap_level: int = 0) -> None:
         """
         Optimize quantum circuit with light method
         """
-    pass
-
 def from_json(arg0: str) -> qulacs_core.QuantumCircuit:
     """
     from json string
     """
```

### Comparing `qulacs-0.6.3/pysrc/qulacs/converter/qasm_converter.py` & `qulacs-0.6.4/pysrc/qulacs/converter/qasm_converter.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/pysrc/qulacs/gate/__init__.pyi` & `qulacs-0.6.4/pysrc/qulacs/gate.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,485 +1,292 @@
 from __future__ import annotations
-
-import typing
-
 import numpy
 import qulacs_core
-import qulacs_core.gate
 import scipy.sparse
-
-__all__ = [
-    "Adaptive",
-    "AmplitudeDampingNoise",
-    "BitFlipNoise",
-    "CNOT",
-    "CP",
-    "CPTP",
-    "CZ",
-    "DenseMatrix",
-    "DephasingNoise",
-    "DepolarizingNoise",
-    "DiagonalMatrix",
-    "FREDKIN",
-    "FusedSWAP",
-    "H",
-    "Identity",
-    "IndependentXZNoise",
-    "Instrument",
-    "Measurement",
-    "NoisyEvolution",
-    "NoisyEvolution_fast",
-    "P0",
-    "P1",
-    "ParametricPauliRotation",
-    "ParametricRX",
-    "ParametricRY",
-    "ParametricRZ",
-    "Pauli",
-    "PauliRotation",
-    "Probabilistic",
-    "ProbabilisticInstrument",
-    "RX",
-    "RY",
-    "RZ",
-    "RandomUnitary",
-    "ReversibleBoolean",
-    "RotInvX",
-    "RotInvY",
-    "RotInvZ",
-    "RotX",
-    "RotY",
-    "RotZ",
-    "S",
-    "SWAP",
-    "Sdag",
-    "SparseMatrix",
-    "StateReflection",
-    "T",
-    "TOFFOLI",
-    "Tdag",
-    "TwoQubitDepolarizingNoise",
-    "U1",
-    "U2",
-    "U3",
-    "X",
-    "Y",
-    "Z",
-    "add",
-    "from_json",
-    "merge",
-    "sqrtX",
-    "sqrtXdag",
-    "sqrtY",
-    "sqrtYdag",
-    "to_matrix_gate",
-]
-
+import typing
+__all__ = ['Adaptive', 'AmplitudeDampingNoise', 'BitFlipNoise', 'CNOT', 'CP', 'CPTP', 'CZ', 'DenseMatrix', 'DephasingNoise', 'DepolarizingNoise', 'DiagonalMatrix', 'FREDKIN', 'FusedSWAP', 'H', 'Identity', 'IndependentXZNoise', 'Instrument', 'Measurement', 'NoisyEvolution', 'NoisyEvolution_fast', 'P0', 'P1', 'ParametricPauliRotation', 'ParametricRX', 'ParametricRY', 'ParametricRZ', 'Pauli', 'PauliRotation', 'Probabilistic', 'ProbabilisticInstrument', 'RX', 'RY', 'RZ', 'RandomUnitary', 'ReversibleBoolean', 'RotInvX', 'RotInvY', 'RotInvZ', 'RotX', 'RotY', 'RotZ', 'S', 'SWAP', 'Sdag', 'SparseMatrix', 'StateReflection', 'T', 'TOFFOLI', 'Tdag', 'TwoQubitDepolarizingNoise', 'U1', 'U2', 'U3', 'X', 'Y', 'Z', 'add', 'from_json', 'merge', 'sqrtX', 'sqrtXdag', 'sqrtY', 'sqrtYdag', 'to_matrix_gate']
 @typing.overload
-def Adaptive(
-    gate: qulacs_core.QuantumGateBase,
-    condition: typing.Callable[[typing.List[int]], bool],
-) -> qulacs_core.QuantumGateBase:
+def Adaptive(gate: qulacs_core.QuantumGateBase, condition: typing.Callable[[list[int]], bool]) -> qulacs_core.QuantumGateBase:
     """
     Create adaptive gate
     """
-
 @typing.overload
-def Adaptive(
-    gate: qulacs_core.QuantumGateBase,
-    condition: typing.Callable[[typing.List[int], int], bool],
-    id: int,
-) -> qulacs_core.QuantumGateBase:
-    pass
-
+def Adaptive(gate: qulacs_core.QuantumGateBase, condition: typing.Callable[[list[int], int], bool], id: int) -> qulacs_core.QuantumGateBase:
+    """
+    Create adaptive gate
+    """
 def AmplitudeDampingNoise(index: int, prob: float) -> qulacs_core.QuantumGate_CPTP:
     """
     Create amplitude damping noise
     """
-
 def BitFlipNoise(index: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic:
     """
     Create bit-flip noise
     """
-
 def CNOT(control: int, target: int) -> qulacs_core.ClsOneControlOneTargetGate:
     """
     Create CNOT gate
     """
-
-def CP(
-    kraus_list: typing.List[qulacs_core.QuantumGateBase],
-    state_normalize: bool,
-    probability_normalize: bool,
-    assign_zero_if_not_matched: bool,
-) -> qulacs_core.QuantumGateBase:
+def CP(kraus_list: list[qulacs_core.QuantumGateBase], state_normalize: bool, probability_normalize: bool, assign_zero_if_not_matched: bool) -> qulacs_core.QuantumGateBase:
     """
     Create completely-positive map
     """
-
-def CPTP(
-    kraus_list: typing.List[qulacs_core.QuantumGateBase],
-) -> qulacs_core.QuantumGateBase:
+def CPTP(kraus_list: list[qulacs_core.QuantumGateBase]) -> qulacs_core.QuantumGateBase:
     """
     Create completely-positive trace preserving map
     """
-
 def CZ(control: int, target: int) -> qulacs_core.ClsOneControlOneTargetGate:
     """
     Create CZ gate
     """
-
 @typing.overload
 def DenseMatrix(index: int, matrix: numpy.ndarray) -> qulacs_core.QuantumGateMatrix:
     """
     Create dense matrix gate
     """
-
 @typing.overload
-def DenseMatrix(
-    index_list: typing.List[int], matrix: numpy.ndarray
-) -> qulacs_core.QuantumGateMatrix:
-    pass
-
+def DenseMatrix(index_list: list[int], matrix: numpy.ndarray) -> qulacs_core.QuantumGateMatrix:
+    """
+    Create dense matrix gate
+    """
 def DephasingNoise(index: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic:
     """
     Create dephasing noise
     """
-
 def DepolarizingNoise(index: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic:
     """
     Create depolarizing noise
     """
-
-def DiagonalMatrix(
-    index_list: typing.List[int], diagonal_element: numpy.ndarray
-) -> qulacs_core.QuantumGateDiagonalMatrix:
+def DiagonalMatrix(index_list: list[int], diagonal_element: numpy.ndarray) -> qulacs_core.QuantumGateDiagonalMatrix:
     """
     Create diagonal matrix gate
     """
-
 def FREDKIN(control: int, target1: int, target2: int) -> qulacs_core.QuantumGateMatrix:
     """
     Create FREDKIN gate
     """
-
-def FusedSWAP(target1: int, target2: int, block_size: int) -> ClsNpairQubitGate:
+def FusedSWAP(target1: int, target2: int, block_size: int) -> qulacs_core.ClsNpairQubitGate:
     """
     Create FusedSWAP gate
     """
-
 def H(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create Hadamard gate
     """
-
 def Identity(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create identity gate
     """
-
-def IndependentXZNoise(
-    index: int, prob: float
-) -> qulacs_core.QuantumGate_Probabilistic:
+def IndependentXZNoise(index: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic:
     """
     Create independent XZ noise
     """
-
-def Instrument(
-    kraus_list: typing.List[qulacs_core.QuantumGateBase], register: int
-) -> qulacs_core.QuantumGateBase:
+def Instrument(kraus_list: list[qulacs_core.QuantumGateBase], register: int) -> qulacs_core.QuantumGateBase:
     """
     Create instruments
     """
-
 def Measurement(index: int, register: int) -> qulacs_core.QuantumGate_CPTP:
     """
     Create measurement gate
     """
-
-def NoisyEvolution(
-    hamiltonian: qulacs_core.Observable,
-    c_ops: typing.List[qulacs_core.GeneralQuantumOperator],
-    time: float,
-    dt: float,
-) -> qulacs_core.ClsNoisyEvolution:
+def NoisyEvolution(hamiltonian: qulacs_core.Observable, c_ops: list[qulacs_core.GeneralQuantumOperator], time: float, dt: float) -> qulacs_core.ClsNoisyEvolution:
     """
     Create noisy evolution
     """
-
-def NoisyEvolution_fast(
-    hamiltonian: qulacs_core.Observable,
-    c_ops: typing.List[qulacs_core.GeneralQuantumOperator],
-    time: float,
-) -> qulacs_core.ClsNoisyEvolution_fast:
+def NoisyEvolution_fast(hamiltonian: qulacs_core.Observable, c_ops: list[qulacs_core.GeneralQuantumOperator], time: float) -> qulacs_core.ClsNoisyEvolution_fast:
     """
     Create noisy evolution fast version
     """
-
 def P0(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create projection gate to |0> subspace
     """
-
 def P1(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create projection gate to |1> subspace
     """
-
-def ParametricPauliRotation(
-    index_list: typing.List[int], pauli_ids: typing.List[int], angle: float
-) -> qulacs_core.QuantumGate_SingleParameter:
+def ParametricPauliRotation(index_list: list[int], pauli_ids: list[int], angle: float) -> qulacs_core.QuantumGate_SingleParameter:
     """
     Create parametric multi-qubit Pauli rotation gate
     """
-
 def ParametricRX(index: int, angle: float) -> qulacs_core.QuantumGate_SingleParameter:
     """
     Create parametric Pauli-X rotation gate
     """
-
 def ParametricRY(index: int, angle: float) -> qulacs_core.QuantumGate_SingleParameter:
     """
     Create parametric Pauli-Y rotation gate
     """
-
 def ParametricRZ(index: int, angle: float) -> qulacs_core.QuantumGate_SingleParameter:
     """
     Create parametric Pauli-Z rotation gate
     """
-
-def Pauli(
-    index_list: typing.List[int], pauli_ids: typing.List[int]
-) -> qulacs_core.ClsPauliGate:
+def Pauli(index_list: list[int], pauli_ids: list[int]) -> qulacs_core.ClsPauliGate:
     """
     Create multi-qubit Pauli gate
     """
-
-def PauliRotation(
-    index_list: typing.List[int], pauli_ids: typing.List[int], angle: float
-) -> qulacs_core.ClsPauliRotationGate:
+def PauliRotation(index_list: list[int], pauli_ids: list[int], angle: float) -> qulacs_core.ClsPauliRotationGate:
     """
     Create multi-qubit Pauli rotation
     """
-
-def Probabilistic(
-    prob_list: typing.List[float], gate_list: typing.List[qulacs_core.QuantumGateBase]
-) -> qulacs_core.QuantumGateBase:
+def Probabilistic(prob_list: list[float], gate_list: list[qulacs_core.QuantumGateBase]) -> qulacs_core.QuantumGateBase:
     """
     Create probabilistic gate
     """
-
-def ProbabilisticInstrument(
-    prob_list: typing.List[float],
-    gate_list: typing.List[qulacs_core.QuantumGateBase],
-    register: int,
-) -> qulacs_core.QuantumGateBase:
+def ProbabilisticInstrument(prob_list: list[float], gate_list: list[qulacs_core.QuantumGateBase], register: int) -> qulacs_core.QuantumGateBase:
     """
     Create probabilistic instrument gate
     """
-
 def RX(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-X rotation gate
     """
-
 def RY(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-Y rotation gate
     """
-
 def RZ(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-Z rotation gate
     """
-
 @typing.overload
-def RandomUnitary(index_list: typing.List[int]) -> qulacs_core.QuantumGateMatrix:
+def RandomUnitary(index_list: list[int]) -> qulacs_core.QuantumGateMatrix:
     """
     Create random unitary gate
     """
-
 @typing.overload
-def RandomUnitary(
-    index_list: typing.List[int], seed: int
-) -> qulacs_core.QuantumGateMatrix:
-    pass
-
-def ReversibleBoolean(
-    index_list: typing.List[int], func: typing.Callable[[int, int], int]
-) -> qulacs_core.ClsReversibleBooleanGate:
+def RandomUnitary(index_list: list[int], seed: int) -> qulacs_core.QuantumGateMatrix:
+    """
+    Create random unitary gate
+    """
+def ReversibleBoolean(index_list: list[int], func: typing.Callable[[int, int], int]) -> qulacs_core.ClsReversibleBooleanGate:
     """
     Create reversible boolean gate
     """
-
 def RotInvX(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-X rotation gate
     """
-
 def RotInvY(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-Y rotation gate
     """
-
 def RotInvZ(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-Z rotation gate
     """
-
 def RotX(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-X rotation gate
     """
-
 def RotY(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-Y rotation gate
     """
-
 def RotZ(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-Z rotation gate
     """
-
 def S(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create pi/4-phase gate
     """
-
 def SWAP(target1: int, target2: int) -> qulacs_core.ClsTwoQubitGate:
     """
     Create SWAP gate
     """
-
 def Sdag(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create adjoint of pi/4-phase gate
     """
-
-def SparseMatrix(
-    index_list: typing.List[int], matrix: scipy.sparse.csc_matrix[numpy.complex128]
-) -> qulacs_core.QuantumGateSparseMatrix:
+def SparseMatrix(index_list: list[int], matrix: scipy.sparse.csc_matrix) -> qulacs_core.QuantumGateSparseMatrix:
     """
     Create sparse matrix gate
     """
-
-def StateReflection(
-    state: qulacs_core.QuantumState,
-) -> qulacs_core.ClsStateReflectionGate:
+def StateReflection(state: qulacs_core.QuantumState) -> qulacs_core.ClsStateReflectionGate:
     """
     Create state reflection gate
     """
-
 def T(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create pi/8-phase gate
     """
-
 def TOFFOLI(control1: int, control2: int, target: int) -> qulacs_core.QuantumGateMatrix:
     """
     Create TOFFOLI gate
     """
-
 def Tdag(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create adjoint of pi/8-phase gate
     """
-
-def TwoQubitDepolarizingNoise(
-    index1: int, index2: int, prob: float
-) -> qulacs_core.QuantumGate_Probabilistic:
+def TwoQubitDepolarizingNoise(index1: int, index2: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic:
     """
     Create two-qubit depolarizing noise
     """
-
 def U1(index: int, lambda_: float) -> qulacs_core.QuantumGateMatrix:
     """
     Create QASM U1 gate
     """
-
 def U2(index: int, phi: float, lambda_: float) -> qulacs_core.QuantumGateMatrix:
     """
     Create QASM U2 gate
     """
-
-def U3(
-    index: int, theta: float, phi: float, lambda_: float
-) -> qulacs_core.QuantumGateMatrix:
+def U3(index: int, theta: float, phi: float, lambda_: float) -> qulacs_core.QuantumGateMatrix:
     """
     Create QASM U3 gate
     """
-
 def X(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create Pauli-X gate
     """
-
 def Y(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create Pauli-Y gate
     """
-
 def Z(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create Pauli-Z gate
     """
-
 @typing.overload
-def add(
-    gate1: qulacs_core.QuantumGateBase, gate2: qulacs_core.QuantumGateBase
-) -> qulacs_core.QuantumGateMatrix:
+def add(gate1: qulacs_core.QuantumGateBase, gate2: qulacs_core.QuantumGateBase) -> qulacs_core.QuantumGateMatrix:
     """
     Add quantum gate matrices
-
-    Add quantum gate matrices
     """
-
 @typing.overload
-def add(
-    gate_list: typing.List[qulacs_core.QuantumGateBase],
-) -> qulacs_core.QuantumGateMatrix:
-    pass
-
+def add(gate_list: list[qulacs_core.QuantumGateBase]) -> qulacs_core.QuantumGateMatrix:
+    """
+    Add quantum gate matrices
+    """
 def from_json(arg0: str) -> qulacs_core.QuantumGateBase:
     """
     from json string
     """
-
 @typing.overload
-def merge(
-    gate1: qulacs_core.QuantumGateBase, gate2: qulacs_core.QuantumGateBase
-) -> qulacs_core.QuantumGateMatrix:
+def merge(gate1: qulacs_core.QuantumGateBase, gate2: qulacs_core.QuantumGateBase) -> qulacs_core.QuantumGateMatrix:
     """
-    Merge two quantum gate or gate list
+    Merge two quantum gates
     """
-
 @typing.overload
-def merge(
-    gate_list: typing.List[qulacs_core.QuantumGateBase],
-) -> qulacs_core.QuantumGateMatrix:
-    pass
-
+def merge(gate_list: list[qulacs_core.QuantumGateBase]) -> qulacs_core.QuantumGateMatrix:
+    """
+    Merge quantum gate list
+    """
 def sqrtX(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create pi/4 Pauli-X rotation gate
     """
-
 def sqrtXdag(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create adjoint of pi/4 Pauli-X rotation gate
     """
-
 def sqrtY(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create pi/4 Pauli-Y rotation gate
     """
-
 def sqrtYdag(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create adjoint of pi/4 Pauli-Y rotation gate
     """
-
 def to_matrix_gate(gate: qulacs_core.QuantumGateBase) -> qulacs_core.QuantumGateMatrix:
     """
     Convert named gate to matrix gate
     """
```

### Comparing `qulacs-0.6.3/pysrc/qulacs/observable/__init__.pyi` & `qulacs-0.6.4/pysrc/qulacs/observable.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,17 @@
 from __future__ import annotations
-
-import typing
-
 import qulacs_core
-import qulacs_core.observable
-
-__all__ = [
-    "create_observable_from_openfermion_file",
-    "create_observable_from_openfermion_text",
-    "create_split_observable",
-    "from_json",
-]
-
+__all__ = ['create_observable_from_openfermion_file', 'create_observable_from_openfermion_text', 'create_split_observable', 'from_json']
 def create_observable_from_openfermion_file(file_path: str) -> qulacs_core.Observable:
     """
     Create GeneralQuantumOperator from openfermion file
     """
-
 def create_observable_from_openfermion_text(text: str) -> qulacs_core.Observable:
     """
     Create GeneralQuantumOperator from openfermion text
     """
-
-def create_split_observable(
-    arg0: str,
-) -> typing.Tuple[qulacs_core.Observable, qulacs_core.Observable]:
-    pass
-
+def create_split_observable(arg0: str) -> tuple[qulacs_core.Observable, qulacs_core.Observable]:
+    ...
 def from_json(json: str) -> qulacs_core.Observable:
     """
     from json string
     """
```

### Comparing `qulacs-0.6.3/pysrc/qulacs/quantum_operator/__init__.pyi` & `qulacs-0.6.4/pysrc/qulacs/quantum_operator.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,13 @@
 from __future__ import annotations
-
-import typing
-
 import qulacs_core
-import qulacs_core.quantum_operator
-
-__all__ = [
-    "create_quantum_operator_from_openfermion_file",
-    "create_quantum_operator_from_openfermion_text",
-    "create_split_quantum_operator",
-    "from_json",
-]
-
-def create_quantum_operator_from_openfermion_file(
-    arg0: str,
-) -> qulacs_core.GeneralQuantumOperator:
-    pass
-
-def create_quantum_operator_from_openfermion_text(
-    arg0: str,
-) -> qulacs_core.GeneralQuantumOperator:
-    pass
-
-def create_split_quantum_operator(
-    arg0: str,
-) -> typing.Tuple[
-    qulacs_core.GeneralQuantumOperator, qulacs_core.GeneralQuantumOperator
-]:
-    pass
-
+__all__ = ['create_quantum_operator_from_openfermion_file', 'create_quantum_operator_from_openfermion_text', 'create_split_quantum_operator', 'from_json']
+def create_quantum_operator_from_openfermion_file(arg0: str) -> qulacs_core.GeneralQuantumOperator:
+    ...
+def create_quantum_operator_from_openfermion_text(arg0: str) -> qulacs_core.GeneralQuantumOperator:
+    ...
+def create_split_quantum_operator(arg0: str) -> tuple[qulacs_core.GeneralQuantumOperator, qulacs_core.GeneralQuantumOperator]:
+    ...
 def from_json(json: str) -> qulacs_core.GeneralQuantumOperator:
     """
     from json string
     """
```

### Comparing `qulacs-0.6.3/pysrc/qulacs/state/__init__.pyi` & `qulacs-0.6.4/pysrc/qulacs/state.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,54 @@
 from __future__ import annotations
-
-import typing
-
 import qulacs_core
-import qulacs_core.state
-
-__all__ = [
-    "drop_qubit",
-    "from_json",
-    "inner_product",
-    "make_mixture",
-    "make_superposition",
-    "partial_trace",
-    "permutate_qubit",
-    "tensor_product",
-]
-
-def drop_qubit(
-    state: qulacs_core.QuantumState,
-    target: typing.List[int],
-    projection: typing.List[int],
-) -> qulacs_core.QuantumState:
+import typing
+__all__ = ['drop_qubit', 'from_json', 'inner_product', 'make_mixture', 'make_superposition', 'partial_trace', 'permutate_qubit', 'tensor_product']
+def drop_qubit(state: qulacs_core.QuantumState, target: list[int], projection: list[int]) -> qulacs_core.QuantumState:
     """
     Drop qubits from state
     """
-
 def from_json(json: str) -> qulacs_core.QuantumStateBase:
     """
     from json string
     """
-
-def inner_product(
-    state_bra: qulacs_core.QuantumState, state_ket: qulacs_core.QuantumState
-) -> complex:
+def inner_product(state_bra: qulacs_core.QuantumState, state_ket: qulacs_core.QuantumState) -> complex:
     """
     Get inner product
     """
-
-def make_mixture(
-    prob1: complex,
-    state1: qulacs_core.QuantumStateBase,
-    prob2: complex,
-    state2: qulacs_core.QuantumStateBase,
-) -> qulacs_core.DensityMatrix:
+def make_mixture(prob1: complex, state1: qulacs_core.QuantumStateBase, prob2: complex, state2: qulacs_core.QuantumStateBase) -> qulacs_core.DensityMatrix:
     """
     Create a mixed state
     """
-
-def make_superposition(
-    coef1: complex,
-    state1: qulacs_core.QuantumState,
-    coef2: complex,
-    state2: qulacs_core.QuantumState,
-) -> qulacs_core.QuantumState:
+def make_superposition(coef1: complex, state1: qulacs_core.QuantumState, coef2: complex, state2: qulacs_core.QuantumState) -> qulacs_core.QuantumState:
     """
     Create superposition of states
     """
-
 @typing.overload
-def partial_trace(
-    state: qulacs_core.QuantumState, target_traceout: typing.List[int]
-) -> qulacs_core.DensityMatrix:
+def partial_trace(state: qulacs_core.QuantumState, target_traceout: list[int]) -> qulacs_core.DensityMatrix:
     """
     Take partial trace
     """
-
 @typing.overload
-def partial_trace(
-    state: qulacs_core.DensityMatrix, target_traceout: typing.List[int]
-) -> qulacs_core.DensityMatrix:
-    pass
-
-@typing.overload
-def permutate_qubit(
-    state: qulacs_core.QuantumState, qubit_order: typing.List[int]
-) -> qulacs_core.QuantumState:
+def partial_trace(state: qulacs_core.DensityMatrix, target_traceout: list[int]) -> qulacs_core.DensityMatrix:
+    """
+    Take partial trace
+    """
+@typing.overload
+def permutate_qubit(state: qulacs_core.QuantumState, qubit_order: list[int]) -> qulacs_core.QuantumState:
     """
     Permutate qubits from state
     """
-
 @typing.overload
-def permutate_qubit(
-    state: qulacs_core.DensityMatrix, qubit_order: typing.List[int]
-) -> qulacs_core.DensityMatrix:
-    pass
-
-@typing.overload
-def tensor_product(
-    state_left: qulacs_core.QuantumState, state_right: qulacs_core.QuantumState
-) -> qulacs_core.QuantumState:
+def permutate_qubit(state: qulacs_core.DensityMatrix, qubit_order: list[int]) -> qulacs_core.DensityMatrix:
+    """
+    Permutate qubits from state
+    """
+@typing.overload
+def tensor_product(state_left: qulacs_core.QuantumState, state_right: qulacs_core.QuantumState) -> qulacs_core.QuantumState:
     """
     Get tensor product of states
     """
-
 @typing.overload
-def tensor_product(
-    state_left: qulacs_core.DensityMatrix, state_right: qulacs_core.DensityMatrix
-) -> qulacs_core.DensityMatrix:
-    pass
+def tensor_product(state_left: qulacs_core.DensityMatrix, state_right: qulacs_core.DensityMatrix) -> qulacs_core.DensityMatrix:
+    """
+    Get tensor product of states
+    """
```

### Comparing `qulacs-0.6.3/pysrc/qulacs/utils/conversions_openfermion.py` & `qulacs-0.6.4/pysrc/qulacs/utils/conversions_openfermion.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/pysrc/qulacs/vistest/test_vis.py` & `qulacs-0.6.4/pysrc/qulacs/vistest/test_vis.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/pysrc/qulacs/visualizer/visualizer.py` & `qulacs-0.6.4/pysrc/qulacs/visualizer/visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """回路のグラフ化をできます。量子状態の棒グラフ、縮約した後の玉表示"""
+
 import matplotlib.pyplot as plt
 import numpy as np
 
 from qulacs import Observable, QuantumState
 
 # bar(x, y, color=["red", "blue", "green", "pink", "orange"], width=0.5)
```

### Comparing `qulacs-0.6.3/pysrc/qulacs.egg-info/PKG-INFO` & `qulacs-0.6.4/pysrc/qulacs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qulacs
-Version: 0.6.3
+Version: 0.6.4
 Summary: Quantum circuit simulator for research
 Author-email: QunaSys <qulacs@qunasys.com>
 License: MIT License
         
         Copyright (c) 2018 Qulacs Authors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,14 +54,16 @@
 Requires-Dist: flake8; extra == "ci"
 Requires-Dist: isort; extra == "ci"
 Requires-Dist: mypy; extra == "ci"
 Requires-Dist: pybind11-stubgen; extra == "ci"
 Requires-Dist: openfermion; extra == "ci"
 Requires-Dist: pytest; extra == "ci"
 Provides-Extra: doc
+Requires-Dist: mypy; extra == "doc"
+Requires-Dist: pybind11-stubgen; extra == "doc"
 Requires-Dist: sphinx==7.*; extra == "doc"
 Requires-Dist: sphinx-rtd-theme; extra == "doc"
 Requires-Dist: breathe; extra == "doc"
 Requires-Dist: exhale; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
 Requires-Dist: myst-parser; extra == "doc"
 Requires-Dist: sphinx-copybutton; extra == "doc"
@@ -181,14 +183,23 @@
 
 Install single-thread Qulacs:
 
 ```
 USE_OMP=No pip install .
 ```
 
+If you install qulacs manually, it does not have type stubs.
+To include type stubs into the package, you have to run `script/generate_stubs.sh` after the first install and reinstall.
+
+```
+pip install .
+script/update_stubs.sh
+pip install .
+```
+
 The number of threads used in Qulacs installed with default options can be controlled via the environment variable `OMP_NUM_THREADS` or `QULACS_NUM_THREADS`.
 While `OMP_NUM_THREADS` affects the parallelization of other libraries, `QULACS_NUM_THREADS` controls only the parallelization of QULACS.
 Or, if you want to force only Qulacs to use a single thread, You can install single-thread Qulacs with the above command.
 
 For development purpose, optional dependencies can be installed as follows.
 ```
 # Install development tools
```

### Comparing `qulacs-0.6.3/pysrc/qulacs.egg-info/SOURCES.txt` & `qulacs-0.6.4/pysrc/qulacs.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -116,30 +116,20 @@
 pysrc/qulacs.egg-info/PKG-INFO
 pysrc/qulacs.egg-info/SOURCES.txt
 pysrc/qulacs.egg-info/dependency_links.txt
 pysrc/qulacs.egg-info/not-zip-safe
 pysrc/qulacs.egg-info/requires.txt
 pysrc/qulacs.egg-info/top_level.txt
 pysrc/qulacs/circuit/__init__.py
-pysrc/qulacs/circuit/__init__.pyi
-pysrc/qulacs/circuit/py.typed
 pysrc/qulacs/converter/__init__.py
 pysrc/qulacs/converter/qasm_converter.py
 pysrc/qulacs/gate/__init__.py
-pysrc/qulacs/gate/__init__.pyi
-pysrc/qulacs/gate/py.typed
 pysrc/qulacs/observable/__init__.py
-pysrc/qulacs/observable/__init__.pyi
-pysrc/qulacs/observable/py.typed
 pysrc/qulacs/quantum_operator/__init__.py
-pysrc/qulacs/quantum_operator/__init__.pyi
-pysrc/qulacs/quantum_operator/py.typed
 pysrc/qulacs/state/__init__.py
-pysrc/qulacs/state/__init__.pyi
-pysrc/qulacs/state/py.typed
 pysrc/qulacs/utils/__init__.py
 pysrc/qulacs/utils/conversions_openfermion.py
 pysrc/qulacs/vistest/__init__.py
 pysrc/qulacs/vistest/test_vis.py
 pysrc/qulacs/visualizer/__init__.py
 pysrc/qulacs/visualizer/visualizer.py
 python/CMakeLists.txt
```

### Comparing `qulacs-0.6.3/python/CMakeLists.txt` & `qulacs-0.6.4/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/python/cppsim_wrapper.cpp` & `qulacs-0.6.4/python/cppsim_wrapper.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -958,15 +958,15 @@
     mgate.def(
         "DiagonalMatrix",
         [](std::vector<UINT> target_qubit_index_list,
             ComplexVector diagonal_element) -> QuantumGateDiagonalMatrix* {
             const ITYPE dim = 1ULL << target_qubit_index_list.size();
             if (diagonal_element.size() != dim)
                 throw std::invalid_argument(
-                    "dim of diagonal elemet is not consistent.");
+                    "dim of diagonal element is not consistent.");
             auto ptr =
                 gate::DiagonalMatrix(target_qubit_index_list, diagonal_element);
             return ptr;
         },
         py::return_value_policy::take_ownership, "Create diagonal matrix gate",
         py::arg("index_list"), py::arg("diagonal_element"));
 
@@ -1170,26 +1170,23 @@
                 &QuantumCircuit::update_quantum_state),
             "Update quantum state", py::arg("state"))
         .def("update_quantum_state",
             py::overload_cast<QuantumStateBase*, UINT, UINT>(
                 &QuantumCircuit::update_quantum_state),
             "Update quantum state", py::arg("state"), py::arg("start"),
             py::arg("end"))
-#if 0  // not supported yet
         .def("update_quantum_state",
             py::overload_cast<QuantumStateBase*, UINT>(
                 &QuantumCircuit::update_quantum_state),
-            "Update quantum state",
-            py::arg("state"), py::arg("seed"))
+            "Update quantum state", py::arg("state"), py::arg("seed"))
         .def("update_quantum_state",
             py::overload_cast<QuantumStateBase*, UINT, UINT, UINT>(
                 &QuantumCircuit::update_quantum_state),
-            "Update quantum state",
-            py::arg("state"), py::arg("start"), py::arg("end"), py::arg("seed"))
-#endif
+            "Update quantum state", py::arg("state"), py::arg("start"),
+            py::arg("end"), py::arg("seed"))
         .def("calculate_depth", &QuantumCircuit::calculate_depth,
             "Calculate depth of circuit")
         .def("to_string", &QuantumCircuit::to_string,
             "Get string representation")
 
         .def("add_X_gate", &QuantumCircuit::add_X_gate, "Add Pauli-X gate",
             py::arg("index"))
@@ -1234,138 +1231,138 @@
 Add Pauli-X rotation gate
 
 Notes
 -----
 Matrix Representation
 
 .. math::
-    R_X(\\theta) = \exp(i\\frac{\\theta}{2} X) =
-        \\begin{pmatrix}
-        \cos(\\frac{\\theta}{2})  & i\sin(\\frac{\\theta}{2}) \\\\
-        i\sin(\\frac{\\theta}{2}) & \cos(\\frac{\\theta}{2})
+    R_X(\theta) = \exp(i\frac{\theta}{2} X) =
+        \begin{pmatrix}
+        \cos(\frac{\theta}{2})  & i\sin(\frac{\theta}{2}) \\
+        i\sin(\frac{\theta}{2}) & \cos(\frac{\theta}{2})
         \end{pmatrix}
 )",
             py::arg("index"), py::arg("angle"))
         .def("add_RY_gate", &QuantumCircuit::add_RY_gate, R"(
 Add Pauli-Y rotation gate
 
 Notes
 -----
 Matrix Representation
 
 .. math::
-    R_Y(\\theta) = \exp(i\\frac{\\theta}{2} Y) =
-        \\begin{pmatrix}
-        \cos(\\frac{\\theta}{2})  & \sin(\\frac{\\theta}{2}) \\\\
-        -\sin(\\frac{\\theta}{2}) & \cos(\\frac{\\theta}{2})
+    R_Y(\theta) = \exp(i\frac{\theta}{2} Y) =
+        \begin{pmatrix}
+        \cos(\frac{\theta}{2})  & \sin(\frac{\theta}{2}) \\
+        -\sin(\frac{\theta}{2}) & \cos(\frac{\theta}{2})
         \end{pmatrix}
 )",
             py::arg("index"), py::arg("angle"))
         .def("add_RZ_gate", &QuantumCircuit::add_RZ_gate, R"(
 Add Pauli-Z rotation gate
 
 Notes
 -----
 Matrix Representation
 
 .. math::
-    R_Z(\\theta) = \exp(i\\frac{\\theta}{2} Z) =
-        \\begin{pmatrix}
-        e^{i\\frac{\\theta}{2}} & 0 \\\\
-        0 & e^{-i\\frac{\\theta}{2}}
+    R_Z(\theta) = \exp(i\frac{\theta}{2} Z) =
+        \begin{pmatrix}
+        e^{i\frac{\theta}{2}} & 0 \\
+        0 & e^{-i\frac{\theta}{2}}
         \end{pmatrix}
 )",
             py::arg("index"), py::arg("angle"))
         .def("add_RotInvX_gate", &QuantumCircuit::add_RotInvX_gate, R"(
 Add Pauli-X rotation gate
 
 Notes
 -----
 Matrix Representation
 
 .. math::
-    R_X(\\theta) = \exp(i\\frac{\\theta}{2} X) =
-        \\begin{pmatrix}
-        \cos(\\frac{\\theta}{2})  & i\sin(\\frac{\\theta}{2}) \\\\
-        i\sin(\\frac{\\theta}{2}) & \cos(\\frac{\\theta}{2})
+    R_X(\theta) = \exp(i\frac{\theta}{2} X) =
+        \begin{pmatrix}
+        \cos(\frac{\theta}{2})  & i\sin(\frac{\theta}{2}) \\
+        i\sin(\frac{\theta}{2}) & \cos(\frac{\theta}{2})
         \end{pmatrix}
 )",
             py::arg("index"), py::arg("angle"))
         .def("add_RotInvY_gate", &QuantumCircuit::add_RotInvY_gate, R"(
 Add Pauli-Y rotation gate
 
 Notes
 -----
 Matrix Representation
 
 .. math::
-    R_Y(\\theta) = \exp(i\\frac{\\theta}{2} Y) =
-        \\begin{pmatrix}
-        \cos(\\frac{\\theta}{2})  & \sin(\\frac{\\theta}{2}) \\\\
-        -\sin(\\frac{\\theta}{2}) & \cos(\\frac{\\theta}{2})
+    R_Y(\theta) = \exp(i\frac{\theta}{2} Y) =
+        \begin{pmatrix}
+        \cos(\frac{\theta}{2})  & \sin(\frac{\theta}{2}) \\
+        -\sin(\frac{\theta}{2}) & \cos(\frac{\theta}{2})
         \end{pmatrix}
 )",
             py::arg("index"), py::arg("angle"))
         .def("add_RotInvZ_gate", &QuantumCircuit::add_RotInvZ_gate, R"(
 Add Pauli-Z rotation gate
 
 Notes
 -----
 Matrix Representation
 
 .. math::
-    R_Z(\\theta) = \exp(i\\frac{\\theta}{2} Z) =
-        \\begin{pmatrix}
-        e^{i\\frac{\\theta}{2}} & 0 \\\\
-        0 & e^{-i\\frac{\\theta}{2}}
+    R_Z(\theta) = \exp(i\frac{\theta}{2} Z) =
+        \begin{pmatrix}
+        e^{i\frac{\theta}{2}} & 0 \\
+        0 & e^{-i\frac{\theta}{2}}
         \end{pmatrix}
 )",
             py::arg("index"), py::arg("angle"))
         .def("add_RotX_gate", &QuantumCircuit::add_RotX_gate, R"(
 Add Pauli-X rotation gate
 
 Notes
 -----
 Matrix Representation
 
 .. math::
-    RotX(\\theta) = \exp(-i\\frac{\\theta}{2} X) =
-        \\begin{pmatrix}
-        \cos(\\frac{\\theta}{2})  & -i\sin(\\frac{\\theta}{2}) \\\\
-        -i\sin(\\frac{\\theta}{2}) & \cos(\\frac{\\theta}{2})
+    RotX(\theta) = \exp(-i\frac{\theta}{2} X) =
+        \begin{pmatrix}
+        \cos(\frac{\theta}{2})  & -i\sin(\frac{\theta}{2}) \\
+        -i\sin(\frac{\theta}{2}) & \cos(\frac{\theta}{2})
         \end{pmatrix}
 )",
             py::arg("index"), py::arg("angle"))
         .def("add_RotY_gate", &QuantumCircuit::add_RotY_gate, R"(
 Add Pauli-Y rotation gate
 
 Notes
 -----
 Matrix Representation
 
 .. math::
-    RotY(\\theta) = \exp(-i\\frac{\\theta}{2} Y) =
-        \\begin{pmatrix}
-        \cos(\\frac{\\theta}{2})  & -\sin(\\frac{\\theta}{2}) \\\\
-        \sin(\\frac{\\theta}{2}) & \cos(\\frac{\\theta}{2})
+    RotY(\theta) = \exp(-i\frac{\theta}{2} Y) =
+        \begin{pmatrix}
+        \cos(\frac{\theta}{2})  & -\sin(\frac{\theta}{2}) \\
+        \sin(\frac{\theta}{2}) & \cos(\frac{\theta}{2})
         \end{pmatrix}
 )",
             py::arg("index"), py::arg("angle"))
         .def("add_RotZ_gate", &QuantumCircuit::add_RotZ_gate, R"(
 Add Pauli-Z rotation gate
 
 Notes
 -----
 Matrix Representation
 
 .. math::
-    RotZ(\\theta) = \exp(-i\\frac{\\theta}{2} Z) =
-        \\begin{pmatrix}
-        e^{-i\\frac{\\theta}{2}} & 0 \\\\
-        0 & e^{i\\frac{\\theta}{2}}
+    RotZ(\theta) = \exp(-i\frac{\theta}{2} Z) =
+        \begin{pmatrix}
+        e^{-i\frac{\theta}{2}} & 0 \\
+        0 & e^{i\frac{\theta}{2}}
         \end{pmatrix}
 )",
             py::arg("index"), py::arg("angle"))
         .def("add_U1_gate", &QuantumCircuit::add_U1_gate, "Add QASM U1 gate",
             py::arg("index"), py::arg("lambda_"))
         .def("add_U2_gate", &QuantumCircuit::add_U2_gate, "Add QASM U2 gate",
             py::arg("index"), py::arg("phi"), py::arg("lambda_"))
```

### Comparing `qulacs-0.6.3/python/stub-test/generate_mypy_tester.py` & `qulacs-0.6.4/python/stub-test/generate_mypy_tester.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/python/tests/multi_cpu/conftest.py` & `qulacs-0.6.4/python/tests/multi_cpu/conftest.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/python/tests/multi_cpu/test_circuit_optimizer.py` & `qulacs-0.6.4/python/tests/multi_cpu/test_circuit_optimizer.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/python/tests/multi_cpu/test_state_multi_cpu.py` & `qulacs-0.6.4/python/tests/multi_cpu/test_state_multi_cpu.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/python/tests/single_cpu/test_circuit.py` & `qulacs-0.6.4/python/tests/single_cpu/test_circuit.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/python/tests/single_cpu/test_density_matrix_handling.py` & `qulacs-0.6.4/python/tests/single_cpu/test_density_matrix_handling.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/python/tests/single_cpu/test_json.py` & `qulacs-0.6.4/python/tests/single_cpu/test_json.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/python/tests/single_cpu/test_noise_simulator.py` & `qulacs-0.6.4/python/tests/single_cpu/test_noise_simulator.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/python/tests/single_cpu/test_observable.py` & `qulacs-0.6.4/python/tests/single_cpu/test_observable.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/python/tests/single_cpu/test_pickle.py` & `qulacs-0.6.4/python/tests/single_cpu/test_pickle.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/python/tests/single_cpu/test_pointer_handling.py` & `qulacs-0.6.4/python/tests/single_cpu/test_pointer_handling.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/python/tests/single_cpu/test_qasm.py` & `qulacs-0.6.4/python/tests/single_cpu/test_qasm.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/python/tests/single_cpu/test_state.py` & `qulacs-0.6.4/python/tests/single_cpu/test_state.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/python/tests/single_cpu/test_utils.py` & `qulacs-0.6.4/python/tests/single_cpu/test_utils.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/script/build_gcc.sh` & `qulacs-0.6.4/script/build_gcc.sh`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/script/download_wheel.sh` & `qulacs-0.6.4/script/download_wheel.sh`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/setup.py` & `qulacs-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/CMakeLists.txt` & `qulacs-0.6.4/src/cppsim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/circuit.cpp` & `qulacs-0.6.4/src/cppsim/circuit.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,20 @@
     }
 
     for (const auto& gate : this->_gate_list) {
         gate->update_quantum_state(state);
     }
 }
 
+void QuantumCircuit::update_quantum_state(QuantumStateBase* state, UINT seed) {
+    Random random;
+    random.set_seed(seed);
+    this->update_quantum_state(state);
+}
+
 void QuantumCircuit::update_quantum_state(
     QuantumStateBase* state, UINT start, UINT end) {
     if (state->qubit_count != this->qubit_count) {
         throw InvalidQubitCountException(
             "Error: "
             "QuantumCircuit::update_quantum_state(QuantumStateBase,UINT,"
             "UINT) : invalid qubit count");
@@ -54,14 +60,21 @@
             "UINT) : end must be smaller than or equal to gate_count");
     }
     for (UINT cursor = start; cursor < end; ++cursor) {
         this->_gate_list[cursor]->update_quantum_state(state);
     }
 }
 
+void QuantumCircuit::update_quantum_state(
+    QuantumStateBase* state, UINT start, UINT end, UINT seed) {
+    Random random;
+    random.set_seed(seed);
+    this->update_quantum_state(state, start, end);
+}
+
 QuantumCircuit::QuantumCircuit(const QuantumCircuit& obj)
     : qubit_count(_qubit_count), gate_list(_gate_list) {
     _gate_list.clear();
     _qubit_count = (obj.qubit_count);
     for (UINT i = 0; i < obj.gate_list.size(); ++i) {
         _gate_list.push_back(obj.gate_list[i]->copy());
     }
```

### Comparing `qulacs-0.6.3/src/cppsim/circuit.hpp` & `qulacs-0.6.4/src/cppsim/circuit.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,36 @@
      * @param[in,out] state 作用する量子状態
      * @param[in] start_index 開始位置
      * @param[in] end_index 修了位置
      */
     void update_quantum_state(
         QuantumStateBase* state, UINT start_index, UINT end_index);
 
+    /**
+     * \~japanese-en 量子状態を更新する(random seed指定)
+     *
+     * 順番にすべての量子ゲートを作用する。量子状態の初期化などは行わない。
+     * @param[in,out] state 作用する量子状態
+     * @param[in] seed 乱数の種
+     */
+    void update_quantum_state(QuantumStateBase* state, UINT seed);
+
+    /**
+     * \~japanese-en 量子回路の指定範囲のみを用いて量子状態をを更新する(random
+     * seed指定)
+     *
+     * 添え字がstart_indexからend_index-1までの量子ゲートを順番に量子ゲートを作用する。量子状態の初期化などは行わない。
+     * @param[in,out] state 作用する量子状態
+     * @param[in] start_index 開始位置
+     * @param[in] end_index 修了位置
+     * @param[in] seed 乱数の種
+     */
+    void update_quantum_state(
+        QuantumStateBase* state, UINT start_index, UINT end_index, UINT seed);
+
     /////////////////////////////// CHECK PROPERTY OF QUANTUM CIRCUIT
 
     /**
      * \~japanese-en 量子回路がCliffordかどうかを判定する。
      *
      * 全ての量子ゲートがCliffordである場合にtrueと判定される。
      * Non-Cliffordゲートが複数あり積がCliffordとなっている場合もfalseとして判定される点に注意。
```

### Comparing `qulacs-0.6.3/src/cppsim/circuit_optimizer.cpp` & `qulacs-0.6.4/src/cppsim/circuit_optimizer.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -197,26 +197,24 @@
             }
         }
         if (hit != -1) parent_qubits = current_step[hit].second;
         if (std::includes(parent_qubits.begin(), parent_qubits.end(),
                 target_qubits.begin(), target_qubits.end())) {
             // we merge gates only when it does not interfere swap insertion
             if (can_merge_with_swap_insertion(pos, ind1, swap_level)) {
+                // parametric gate cannot be merged
+                if (circuit->gate_list[pos]->is_parametric() ||
+                    gate->is_parametric())
+                    continue;
                 auto merged_gate = gate::merge(circuit->gate_list[pos], gate);
                 circuit->remove_gate(ind1);
                 circuit->add_gate(merged_gate, pos + 1);
                 circuit->remove_gate(pos);
                 ind1--;
             }
-
-            // std::cout << "merge ";
-            // for (auto val : target_qubits) std::cout << val << " ";
-            // std::cout << " into ";
-            // for (auto val : parent_qubits) std::cout << val << " ";
-            // std::cout << std::endl;
         } else {
             for (auto target_qubit : target_qubits) {
                 current_step[target_qubit] = make_pair(ind1, target_qubits);
             }
         }
     }
 }
```

### Comparing `qulacs-0.6.3/src/cppsim/circuit_optimizer.hpp` & `qulacs-0.6.4/src/cppsim/circuit_optimizer.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/exception.hpp` & `qulacs-0.6.4/src/cppsim/exception.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate.cpp` & `qulacs-0.6.4/src/cppsim/gate.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate.hpp` & `qulacs-0.6.4/src/cppsim/gate.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_factory.cpp` & `qulacs-0.6.4/src/cppsim/gate_factory.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_factory.hpp` & `qulacs-0.6.4/src/cppsim/gate_factory.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_general.hpp` & `qulacs-0.6.4/src/cppsim/gate_general.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_matrix.cpp` & `qulacs-0.6.4/src/cppsim/gate_matrix.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_matrix.hpp` & `qulacs-0.6.4/src/cppsim/gate_matrix.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_matrix_diagonal.cpp` & `qulacs-0.6.4/src/cppsim/gate_matrix_diagonal.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_matrix_diagonal.hpp` & `qulacs-0.6.4/src/cppsim/gate_matrix_diagonal.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_matrix_sparse.cpp` & `qulacs-0.6.4/src/cppsim/gate_matrix_sparse.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_matrix_sparse.hpp` & `qulacs-0.6.4/src/cppsim/gate_matrix_sparse.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_merge.cpp` & `qulacs-0.6.4/src/cppsim/gate_merge.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_merge.hpp` & `qulacs-0.6.4/src/cppsim/gate_merge.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_named_npair.hpp` & `qulacs-0.6.4/src/cppsim/gate_named_npair.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_named_one.cpp` & `qulacs-0.6.4/src/cppsim/gate_named_one.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_named_one.hpp` & `qulacs-0.6.4/src/cppsim/gate_named_one.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_named_pauli.hpp` & `qulacs-0.6.4/src/cppsim/gate_named_pauli.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_named_two.hpp` & `qulacs-0.6.4/src/cppsim/gate_named_two.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_noisy_evolution.cpp` & `qulacs-0.6.4/src/cppsim/gate_noisy_evolution.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_noisy_evolution.hpp` & `qulacs-0.6.4/src/cppsim/gate_noisy_evolution.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_reflect.hpp` & `qulacs-0.6.4/src/cppsim/gate_reflect.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_reversible.hpp` & `qulacs-0.6.4/src/cppsim/gate_reversible.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/gate_to_gqo.hpp` & `qulacs-0.6.4/src/cppsim/gate_to_gqo.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/general_quantum_operator.cpp` & `qulacs-0.6.4/src/cppsim/general_quantum_operator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/general_quantum_operator.hpp` & `qulacs-0.6.4/src/cppsim/general_quantum_operator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/matrix_decomposition.hpp` & `qulacs-0.6.4/src/cppsim/matrix_decomposition.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/noisesimulator.cpp` & `qulacs-0.6.4/src/cppsim/noisesimulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/noisesimulator.hpp` & `qulacs-0.6.4/src/cppsim/noisesimulator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/observable.cpp` & `qulacs-0.6.4/src/cppsim/observable.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/observable.hpp` & `qulacs-0.6.4/src/cppsim/observable.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/pauli_operator.cpp` & `qulacs-0.6.4/src/cppsim/pauli_operator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/pauli_operator.hpp` & `qulacs-0.6.4/src/cppsim/pauli_operator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/qubit_info.cpp` & `qulacs-0.6.4/src/cppsim/qubit_info.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/qubit_info.hpp` & `qulacs-0.6.4/src/cppsim/qubit_info.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/qubit_table.cpp` & `qulacs-0.6.4/src/cppsim/qubit_table.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/qubit_table.hpp` & `qulacs-0.6.4/src/cppsim/qubit_table.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/simulator.cpp` & `qulacs-0.6.4/src/cppsim/simulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/simulator.hpp` & `qulacs-0.6.4/src/cppsim/simulator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/state.cpp` & `qulacs-0.6.4/src/cppsim/state.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/state.hpp` & `qulacs-0.6.4/src/cppsim/state.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -912,15 +912,15 @@
         auto ptr = this->data_cpp();
         stacked_prob.push_back(0.);
         for (ITYPE i = 0; i < this->dim; ++i) {
             sum += norm(ptr[i]);
             stacked_prob.push_back(sum);
         }
 
-        for (ITYPE count = 0; count < sampling_count; ++count) {
+        for (UINT count = 0; count < sampling_count; ++count) {
             double r = random.uniform();
             auto ite =
                 std::lower_bound(stacked_prob.begin(), stacked_prob.end(), r);
             auto index = std::distance(stacked_prob.begin(), ite) - 1;
             result.push_back(index);
         }
         return result;
```

### Comparing `qulacs-0.6.3/src/cppsim/state_dm.cpp` & `qulacs-0.6.4/src/cppsim/state_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/state_dm.hpp` & `qulacs-0.6.4/src/cppsim/state_dm.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/state_gpu.cpp` & `qulacs-0.6.4/src/cppsim/state_gpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/state_gpu.hpp` & `qulacs-0.6.4/src/cppsim/state_gpu.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/type.hpp` & `qulacs-0.6.4/src/cppsim/type.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/utility.cpp` & `qulacs-0.6.4/src/cppsim/utility.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/cppsim/utility.hpp` & `qulacs-0.6.4/src/cppsim/utility.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/CMakeLists.txt` & `qulacs-0.6.4/src/csim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/MPIutil.cpp` & `qulacs-0.6.4/src/csim/MPIutil.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/MPIutil.hpp` & `qulacs-0.6.4/src/csim/MPIutil.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/constant.cpp` & `qulacs-0.6.4/src/csim/constant.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/constant.hpp` & `qulacs-0.6.4/src/csim/constant.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/init_ops.hpp` & `qulacs-0.6.4/src/csim/init_ops.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/init_ops_fill.cpp` & `qulacs-0.6.4/src/csim/init_ops_fill.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/init_ops_random.cpp` & `qulacs-0.6.4/src/csim/init_ops_random.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/memory_ops.cpp` & `qulacs-0.6.4/src/csim/memory_ops.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/memory_ops_dm.cpp` & `qulacs-0.6.4/src/csim/memory_ops_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/memory_ops_dm.hpp` & `qulacs-0.6.4/src/csim/memory_ops_dm.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/stat_ops.cpp` & `qulacs-0.6.4/src/csim/stat_ops.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/stat_ops.hpp` & `qulacs-0.6.4/src/csim/stat_ops.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/stat_ops_dm.cpp` & `qulacs-0.6.4/src/csim/stat_ops_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/stat_ops_dm.hpp` & `qulacs-0.6.4/src/csim/stat_ops_dm.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/stat_ops_expectation_value.cpp` & `qulacs-0.6.4/src/csim/stat_ops_expectation_value.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/stat_ops_probability.cpp` & `qulacs-0.6.4/src/csim/stat_ops_probability.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/stat_ops_transition_amplitude.cpp` & `qulacs-0.6.4/src/csim/stat_ops_transition_amplitude.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/type.hpp` & `qulacs-0.6.4/src/csim/type.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops.hpp` & `qulacs-0.6.4/src/csim/update_ops.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_control_multi_target_multi.cpp` & `qulacs-0.6.4/src/csim/update_ops_control_multi_target_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_control_multi_target_single.cpp` & `qulacs-0.6.4/src/csim/update_ops_control_multi_target_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_control_single_target_multi.cpp` & `qulacs-0.6.4/src/csim/update_ops_control_single_target_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_control_single_target_single.cpp` & `qulacs-0.6.4/src/csim/update_ops_control_single_target_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_cpp.hpp` & `qulacs-0.6.4/src/csim/update_ops_cpp.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_dm.cpp` & `qulacs-0.6.4/src/csim/update_ops_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_dm.hpp` & `qulacs-0.6.4/src/csim/update_ops_dm.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_matrix_dense_double.cpp` & `qulacs-0.6.4/src/csim/update_ops_matrix_dense_double.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_matrix_dense_double_eigen.cpp` & `qulacs-0.6.4/src/csim/update_ops_matrix_dense_double_eigen.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_matrix_dense_multi.cpp` & `qulacs-0.6.4/src/csim/update_ops_matrix_dense_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_matrix_dense_multi_eigen.cpp` & `qulacs-0.6.4/src/csim/update_ops_matrix_dense_multi_eigen.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_matrix_dense_single.cpp` & `qulacs-0.6.4/src/csim/update_ops_matrix_dense_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_matrix_diagonal_multi.cpp` & `qulacs-0.6.4/src/csim/update_ops_matrix_diagonal_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_matrix_diagonal_single.cpp` & `qulacs-0.6.4/src/csim/update_ops_matrix_diagonal_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_matrix_phase_single.cpp` & `qulacs-0.6.4/src/csim/update_ops_matrix_phase_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_named.cpp` & `qulacs-0.6.4/src/csim/update_ops_named.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_named_CNOT.cpp` & `qulacs-0.6.4/src/csim/update_ops_named_CNOT.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_named_CZ.cpp` & `qulacs-0.6.4/src/csim/update_ops_named_CZ.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_named_FusedSWAP.cpp` & `qulacs-0.6.4/src/csim/update_ops_named_FusedSWAP.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_named_H.cpp` & `qulacs-0.6.4/src/csim/update_ops_named_H.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_named_SWAP.cpp` & `qulacs-0.6.4/src/csim/update_ops_named_SWAP.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_named_X.cpp` & `qulacs-0.6.4/src/csim/update_ops_named_X.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_named_Y.cpp` & `qulacs-0.6.4/src/csim/update_ops_named_Y.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_named_Z.cpp` & `qulacs-0.6.4/src/csim/update_ops_named_Z.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_named_projection.cpp` & `qulacs-0.6.4/src/csim/update_ops_named_projection.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_named_state.cpp` & `qulacs-0.6.4/src/csim/update_ops_named_state.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_pauli_multi.cpp` & `qulacs-0.6.4/src/csim/update_ops_pauli_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_pauli_single.cpp` & `qulacs-0.6.4/src/csim/update_ops_pauli_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_qft.cpp` & `qulacs-0.6.4/src/csim/update_ops_qft.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_reflection.cpp` & `qulacs-0.6.4/src/csim/update_ops_reflection.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/update_ops_reversible_boolean.cpp` & `qulacs-0.6.4/src/csim/update_ops_reversible_boolean.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/utility.cpp` & `qulacs-0.6.4/src/csim/utility.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/csim/utility.hpp` & `qulacs-0.6.4/src/csim/utility.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/gpusim/CMakeLists.txt` & `qulacs-0.6.4/src/gpusim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/gpusim/memory_ops.cu` & `qulacs-0.6.4/src/gpusim/memory_ops.cu`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #include <cuda_runtime.h>
 
 #include "cuda_runtime.h"
 #include "device_launch_parameters.h"
-//#include <cuda.h>
+// #include <cuda.h>
 #include <assert.h>
 #include <cuComplex.h>
 #include <curand.h>
 #include <curand_kernel.h>
 
 #include <algorithm>
 #include <cmath>
@@ -68,16 +68,18 @@
 __host__ void initialize_quantum_state_host(
     void* state, ITYPE dim, void* stream, unsigned int device_number) {
     int current_device = get_current_device();
     if (device_number != current_device) cudaSetDevice(device_number);
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
 
-    unsigned int block = dim <= 1024 ? dim : 1024;
-    unsigned int grid = dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(init_qstate);
+    unsigned int block = dim <= max_block_size ? dim : max_block_size;
+    unsigned int grid = (dim + block - 1) / block;
     init_qstate<<<grid, block, 0, *cuda_stream>>>(state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     checkCudaErrors(cudaGetLastError(), __FILE__, __LINE__);
 }
 
 __host__ void release_quantum_state_host(
@@ -85,17 +87,19 @@
     int current_device = get_current_device();
     if (device_number != current_device) cudaSetDevice(device_number);
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     checkCudaErrors(cudaFree(state_gpu), __FILE__, __LINE__);
 }
 
 __global__ void init_rnd(
-    curandState* const rnd_state, const unsigned int seed) {
+    curandState* const rnd_state, const unsigned int seed, ITYPE dim) {
     unsigned int tid = blockIdx.x * blockDim.x + threadIdx.x;
-    curand_init(seed, tid, 0, &rnd_state[tid]);
+    if (tid < dim) {
+        curand_init(seed, tid, 0, &rnd_state[tid]);
+    }
 }
 
 /*
 __global__ void rand_normal_mtgp32(curandState* rnd_state, GTYPE* state, ITYPE
 dim){ ITYPE idx = blockIdx.x * blockDim.x + threadIdx.x; double2 rnd;
     curandStateMtgp32 localState = rnd_state[idx];
         if (idx < dim) {
@@ -139,18 +143,20 @@
     curandState* rnd_state;
     checkCudaErrors(cudaMalloc((void**)&rnd_state, dim * sizeof(curandState)),
         __FILE__, __LINE__);
 
     // CURAND_RNG_PSEUDO_XORWOW
     // CURAND_RNG_PSEUDO_MT19937 offset cannot be used and need sm_35 or higher.
 
-    unsigned int block = dim <= 512 ? dim : 512;
-    unsigned int grid = min((int)(dim / block), 512);
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(init_rnd);
+    unsigned int block = dim <= max_block_size ? dim : max_block_size;
+    unsigned int grid = (dim + block - 1) / block;
 
-    init_rnd<<<grid, block, 0, *cuda_stream>>>(rnd_state, seed);
+    init_rnd<<<grid, block, 0, *cuda_stream>>>(rnd_state, seed, dim);
     checkCudaErrors(cudaGetLastError(), __FILE__, __LINE__);
 
     rand_normal_xorwow<<<grid, block, 0, *cuda_stream>>>(
         rnd_state, state_gpu, dim);
     checkCudaErrors(cudaGetLastError(), __FILE__, __LINE__);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
```

### Comparing `qulacs-0.6.3/src/gpusim/memory_ops.h` & `qulacs-0.6.4/src/gpusim/memory_ops.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/gpusim/memory_ops_device_functions.h` & `qulacs-0.6.4/src/gpusim/memory_ops_device_functions.h`

 * *Files 20% similar despite different names*

```diff
@@ -8,12 +8,13 @@
 #include "cuda_runtime.h"
 #include "device_launch_parameters.h"
 #include "util_export.h"
 #include "util_type.h"
 #include "util_type_internal.h"
 
 __global__ void init_qstate(GTYPE* state_gpu, ITYPE dim);
-__global__ void init_rnd(curandState* const rnd_state, const unsigned int seed);
+__global__ void init_rnd(
+    curandState* const rnd_state, const unsigned int seed, ITYPE dim);
 __global__ void rand_normal_xorwow(
     curandState* rnd_state, GTYPE* state, ITYPE dim);
 
 #endif  // _MEMORY_OPS_CU_DEVICE_H_
```

### Comparing `qulacs-0.6.3/src/gpusim/stat_ops.cu` & `qulacs-0.6.4/src/gpusim/stat_ops.cu`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #include <cuda_runtime.h>
 
 #include "device_launch_parameters.h"
-//#include <cuda.h>
+// #include <cuda.h>
 
 #include <cmath>
 #include <complex>
 #include <cstdio>
 #include <cstdlib>
 #include <cstring>
-//#include <sys/time.h>
+// #include <sys/time.h>
 
 #include <cuComplex.h>
 #include <cublas_v2.h>
 #include <limits.h>
 
 #include "stat_ops.h"
 #include "stat_ops_device_functions.h"
@@ -127,24 +127,19 @@
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
 
     checkCudaErrors(
         cudaMalloc((void**)&norm_gpu, sizeof(double)), __FILE__, __LINE__);
     checkCudaErrors(cudaMemsetAsync(norm_gpu, 0, sizeof(double), *cuda_stream),
         __FILE__, __LINE__);
 
-    ITYPE loop_dim;
-    if (dim <= 32)
-        loop_dim = dim;
-    else if (dim <= 4096)
-        loop_dim = dim >> 2;
-    else
-        loop_dim = dim >> 5;
-
-    unsigned int block = loop_dim <= 256 ? loop_dim : 256;
-    unsigned int grid = loop_dim / block;
+    ITYPE loop_dim = get_loop_dim_of_reduction_function(dim);
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(state_norm_squared_gpu);
+    unsigned int block = dim <= max_block_size ? dim : max_block_size;
+    unsigned int grid = (dim + block - 1) / block;
 
     state_norm_squared_gpu<<<grid, block, 0, *cuda_stream>>>(
         norm_gpu, state_gpu, dim);
 
     // Check for any errors launching the kernel
     cudaStatus = cudaGetLastError();
 
@@ -192,24 +187,19 @@
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
 
     checkCudaErrors(
         cudaMalloc((void**)&ent_gpu, sizeof(double)), __FILE__, __LINE__);
     checkCudaErrors(cudaMemsetAsync(ent_gpu, 0, sizeof(double), *cuda_stream),
         __FILE__, __LINE__);
 
-    ITYPE loop_dim;
-    if (dim <= 32)
-        loop_dim = dim;
-    else if (dim <= 4096)
-        loop_dim = dim >> 2;
-    else
-        loop_dim = dim >> 5;
-
-    unsigned int block = loop_dim <= 256 ? loop_dim : 256;
-    unsigned int grid = loop_dim / block;
+    ITYPE loop_dim = get_loop_dim_of_reduction_function(dim);
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        measurement_distribution_entropy_gpu);
+    unsigned int block = dim <= max_block_size ? dim : max_block_size;
+    unsigned int grid = (dim + block - 1) / block;
 
     measurement_distribution_entropy_gpu<<<grid, block, 0, *cuda_stream>>>(
         ent_gpu, state_gpu, dim);
 
     // Check for any errors launching the kernel
     cudaStatus = cudaGetLastError();
 
@@ -245,16 +235,18 @@
 
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     GTYPE* state_added_gpu = reinterpret_cast<GTYPE*>(state_added);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
 
     ITYPE loop_dim = dim;
 
-    unsigned int block = loop_dim <= 1024 ? loop_dim : 1024;
-    unsigned int grid = loop_dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(state_add_gpu);
+    unsigned int block = dim <= max_block_size ? dim : max_block_size;
+    unsigned int grid = (dim + block - 1) / block;
 
     state_add_gpu<<<grid, block, 0, *cuda_stream>>>(
         state_added_gpu, state_gpu, dim);
 
     checkCudaErrors(cudaGetLastError(), __FILE__, __LINE__);
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     state = reinterpret_cast<void*>(state_gpu);
@@ -277,16 +269,18 @@
     if (device_number != current_device) cudaSetDevice(device_number);
 
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     ITYPE loop_dim = dim;
 
     GTYPE coef_gpu = make_cuDoubleComplex(coef.real(), coef.imag());
-    unsigned int block = loop_dim <= 1024 ? loop_dim : 1024;
-    unsigned int grid = loop_dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(state_multiply_gpu);
+    unsigned int block = dim <= max_block_size ? dim : max_block_size;
+    unsigned int grid = (dim + block - 1) / block;
 
     state_multiply_gpu<<<grid, block, 0, *cuda_stream>>>(
         coef_gpu, state_gpu, dim);
 
     checkCudaErrors(cudaGetLastError(), __FILE__, __LINE__);
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     state = reinterpret_cast<void*>(state_gpu);
@@ -404,24 +398,19 @@
 
     checkCudaErrors(
         cudaMalloc((void**)&ret_gpu, sizeof(GTYPE)), __FILE__, __LINE__);
     checkCudaErrors(cudaMemcpyAsync(ret_gpu, &ret, sizeof(GTYPE),
                         cudaMemcpyHostToDevice, *cuda_stream),
         __FILE__, __LINE__);
 
-    ITYPE loop_dim;
-    if (dim <= 32)
-        loop_dim = dim;
-    else if (dim <= 4096)
-        loop_dim = dim >> 2;
-    else
-        loop_dim = dim >> 5;
-
-    unsigned int block = loop_dim <= 256 ? loop_dim : 256;
-    unsigned int grid = loop_dim / block;
+    ITYPE loop_dim = get_loop_dim_of_reduction_function(dim);
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(inner_product_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
 
     inner_product_gpu<<<grid, block, 0, *cuda_stream>>>(
         ret_gpu, bra_state_gpu, ket_state_gpu, dim);
 
     // Check for any errors launching the kernel
     cudaStatus = cudaGetLastError();
 
@@ -537,42 +526,53 @@
     if (device_number != current_device) cudaSetDevice(device_number);
 
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     double h_ret = 0.0;
     double* d_ret;
 
-    // this loop_dim is not the same as that of the gpu function
-    // and the function uses grid stride loops
-    ITYPE loop_dim;
-    if (dim <= 64)
-        loop_dim = dim >> 1;
-    else if (dim <= (1ULL << 11))
-        loop_dim = dim >> 2;
-    else
-        loop_dim = dim >> 5;
-
-    unsigned int block = loop_dim <= 256 ? loop_dim : 256;
-    unsigned int grid = loop_dim / block;
-
     checkCudaErrors(
         cudaMalloc((void**)&d_ret, sizeof(double)), __FILE__, __LINE__);
     checkCudaErrors(cudaMemsetAsync(d_ret, 0, sizeof(double), *cuda_stream),
         __FILE__, __LINE__);
 
     if (operator_index == 1) {
+        ITYPE loop_dim = get_loop_dim_of_reduction_function(dim >> 1);
+        unsigned int max_block_size =
+            get_block_size_to_maximize_occupancy(expectation_value_PauliX_gpu);
+        unsigned int block =
+            loop_dim <= max_block_size ? loop_dim : max_block_size;
+        unsigned int grid = (loop_dim + block - 1) / block;
         expectation_value_PauliX_gpu<<<grid, block, 0, *cuda_stream>>>(
             d_ret, state_gpu, target_qubit_index, dim);
     } else if (operator_index == 2) {
+        ITYPE loop_dim = get_loop_dim_of_reduction_function(dim >> 1);
+        unsigned int max_block_size =
+            get_block_size_to_maximize_occupancy(expectation_value_PauliY_gpu);
+        unsigned int block =
+            loop_dim <= max_block_size ? loop_dim : max_block_size;
+        unsigned int grid = (loop_dim + block - 1) / block;
         expectation_value_PauliY_gpu<<<grid, block, 0, *cuda_stream>>>(
             d_ret, state_gpu, target_qubit_index, dim);
     } else if (operator_index == 3) {
+        ITYPE loop_dim = get_loop_dim_of_reduction_function(dim >> 1);
+        unsigned int max_block_size =
+            get_block_size_to_maximize_occupancy(expectation_value_PauliZ_gpu);
+        unsigned int block =
+            loop_dim <= max_block_size ? loop_dim : max_block_size;
+        unsigned int grid = (loop_dim + block - 1) / block;
         expectation_value_PauliZ_gpu<<<grid, block, 0, *cuda_stream>>>(
             d_ret, state_gpu, target_qubit_index, dim);
     } else if (operator_index == 0) {
+        ITYPE loop_dim = get_loop_dim_of_reduction_function(dim);
+        unsigned int max_block_size =
+            get_block_size_to_maximize_occupancy(expectation_value_PauliI_gpu);
+        unsigned int block =
+            loop_dim <= max_block_size ? loop_dim : max_block_size;
+        unsigned int grid = (loop_dim + block - 1) / block;
         expectation_value_PauliI_gpu<<<grid, block, 0, *cuda_stream>>>(
             d_ret, state_gpu, target_qubit_index, dim);
     } else {
         printf("operator_index must be an integer of 0, 1, 2, or 3!!");
     }
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
@@ -608,16 +608,18 @@
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     ITYPE bit_mask = 0;
     for (int i = 0; i < n_qubits; ++i) {
         if (gates[i] == 3) bit_mask ^= (1ULL << i);
     }
     cudaError_t cudaStatus;
-    unsigned int block = dim <= 1024 ? dim : 1024;
-    unsigned int grid = dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(multi_Z_gate_gpu);
+    unsigned int block = dim <= max_block_size ? dim : max_block_size;
+    unsigned int grid = (dim + block - 1) / block;
     multi_Z_gate_gpu<<<grid, block, 0, *cuda_stream>>>(
         bit_mask, dim, state_gpu);
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
     checkCudaErrors(cudaStatus, __FILE__, __LINE__);
     state = reinterpret_cast<void*>(state_gpu);
     // stream = reinterpret_cast<void*>(cuda_stream);
@@ -725,45 +727,45 @@
     GTYPE* ret_gpu;
 
     checkCudaErrors(
         cudaMalloc((void**)&ret_gpu, sizeof(GTYPE)), __FILE__, __LINE__);
     checkCudaErrors(cudaMemsetAsync(ret_gpu, 0, sizeof(double), *cuda_stream),
         __FILE__, __LINE__);
 
-    ITYPE loop_dim;
-    if (dim <= 32)
-        loop_dim = dim >> 1;
-    else if (dim <= (1ULL << 11))
-        loop_dim = dim >> 2;
-    else
-        loop_dim = dim >> 5;
-
-    unsigned int block = loop_dim <= 256 ? loop_dim : 256;
-    unsigned int grid = loop_dim / block;
+    ITYPE loop_dim = get_loop_dim_of_reduction_function(dim);
 
     unsigned int num_pauli_op[4] = {0, 0, 0, 0};
     for (int i = 0; i < n_qubits; ++i) ++num_pauli_op[gates[i]];
     ITYPE bit_mask[4] = {0, 0, 0, 0};
     for (int i = 0; i < n_qubits; ++i) {
         bit_mask[gates[i]] ^= (1ULL << i);
     }
     if (num_pauli_op[1] == 0 && num_pauli_op[2] == 0) {
+        unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+            multi_Z_get_expectation_value_gpu);
+        unsigned int block =
+            loop_dim <= max_block_size ? loop_dim : max_block_size;
+        unsigned int grid = (loop_dim + block - 1) / block;
         multi_Z_get_expectation_value_gpu<<<grid, block, 0, *cuda_stream>>>(
             ret_gpu, bit_mask[3], dim, state_gpu);
         checkCudaErrors(
             cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
         checkCudaErrors(cudaGetLastError(), __FILE__, __LINE__);
         checkCudaErrors(cudaMemcpyAsync(ret, ret_gpu, sizeof(CPPCTYPE),
                             cudaMemcpyDeviceToHost, *cuda_stream),
             __FILE__, __LINE__);
         checkCudaErrors(cudaFree(ret_gpu), __FILE__, __LINE__);
         state = reinterpret_cast<void*>(state_gpu);
         return ret[0].real();
     }
 
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        multipauli_get_expectation_value_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
     checkCudaErrors(
         cudaMemcpyToSymbolAsync(num_pauli_op_gpu, num_pauli_op,
             sizeof(unsigned int) * 4, 0, cudaMemcpyHostToDevice, *cuda_stream),
         __FILE__, __LINE__);
     checkCudaErrors(
         cudaMemcpyToSymbolAsync(bit_mask_gpu, bit_mask, sizeof(ITYPE) * 4, 0,
             cudaMemcpyHostToDevice, *cuda_stream),
@@ -814,25 +816,20 @@
     double* ret_gpu;
 
     checkCudaErrors(
         cudaMalloc((void**)&ret_gpu, sizeof(double)), __FILE__, __LINE__);
     checkCudaErrors(cudaMemsetAsync(ret_gpu, 0, sizeof(double), *cuda_stream),
         __FILE__, __LINE__);
 
-    ITYPE loop_dim;
+    ITYPE loop_dim = get_loop_dim_of_reduction_function(dim >> 1);
 
-    if (dim <= 64)
-        loop_dim = dim >> 1;
-    else if (dim <= (1ULL << 11))
-        loop_dim = dim >> 2;
-    else
-        loop_dim = dim >> 5;
-
-    unsigned int block = loop_dim <= 256 ? loop_dim : 256;
-    unsigned int grid = loop_dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(M0_prob_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
 
     M0_prob_gpu<<<grid, block, 0, *cuda_stream>>>(
         ret_gpu, target_qubit_index, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     checkCudaErrors(cudaGetLastError(), __FILE__, __LINE__);
     checkCudaErrors(cudaMemcpyAsync(ret, ret_gpu, sizeof(double),
@@ -876,25 +873,19 @@
     double* ret_gpu;
 
     checkCudaErrors(
         cudaMalloc((void**)&ret_gpu, sizeof(double)), __FILE__, __LINE__);
     checkCudaErrors(cudaMemsetAsync(ret_gpu, 0, sizeof(double), *cuda_stream),
         __FILE__, __LINE__);
 
-    ITYPE loop_dim;
-
-    if (dim <= 64)
-        loop_dim = dim >> 1;
-    else if (dim <= (1ULL << 11))
-        loop_dim = dim >> 2;
-    else
-        loop_dim = dim >> 5;
-
-    unsigned int block = loop_dim <= 256 ? loop_dim : 256;
-    unsigned int grid = loop_dim / block;
+    ITYPE loop_dim = get_loop_dim_of_reduction_function(dim >> 1);
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(M1_prob_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
 
     M1_prob_gpu<<<grid, block, 0, *cuda_stream>>>(
         ret_gpu, target_qubit_index, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     checkCudaErrors(cudaGetLastError(), __FILE__, __LINE__);
     checkCudaErrors(cudaMemcpyAsync(ret, ret_gpu, sizeof(double),
@@ -964,16 +955,20 @@
         __FILE__, __LINE__);
     checkCudaErrors(
         cudaMemcpyAsync(measured_value_list_gpu, measured_value_list,
             sizeof(UINT) * target_qubit_index_count, cudaMemcpyHostToDevice,
             *cuda_stream),
         __FILE__, __LINE__);
 
-    unsigned int block = dim <= 1024 ? dim : 1024;
-    unsigned int grid = dim / block;
+    ITYPE loop_dim =
+        get_loop_dim_of_reduction_function(dim >> target_qubit_index_count);
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(marginal_prob_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
 
     marginal_prob_gpu<<<grid, block, 0, *cuda_stream>>>(ret_gpu,
         sorted_target_qubit_index_list_gpu, measured_value_list_gpu,
         target_qubit_index_count, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     checkCudaErrors(cudaGetLastError(), __FILE__, __LINE__);
@@ -1035,25 +1030,19 @@
     checkCudaErrors(cudaMemsetAsync(ret_gpu, 0, sizeof(double), *cuda_stream),
         __FILE__, __LINE__);
     checkCudaErrors(
         cudaMemcpyToSymbolAsync(PHASE_90ROT_gpu, PHASE_90ROT, sizeof(GTYPE) * 4,
             0, cudaMemcpyHostToDevice, *cuda_stream),
         __FILE__, __LINE__);
 
-    ITYPE loop_dim;
-
-    if (dim <= 64)
-        loop_dim = dim >> 1;
-    else if (dim <= (1ULL << 11))
-        loop_dim = dim >> 2;
-    else
-        loop_dim = dim >> 5;
-
-    unsigned int block = loop_dim <= 256 ? loop_dim : 256;
-    unsigned int grid = loop_dim / block;
+    ITYPE loop_dim = get_loop_dim_of_reduction_function(dim >> 1);
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        expectation_value_multi_qubit_Pauli_operator_XZ_mask_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
 
     expectation_value_multi_qubit_Pauli_operator_XZ_mask_gpu<<<grid, block, 0,
         *cuda_stream>>>(ret_gpu, bit_flip_mask, phase_flip_mask,
         global_phase_90rot_count, pivot_qubit_index, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
@@ -1099,30 +1088,19 @@
     double* ret_gpu;
 
     checkCudaErrors(
         cudaMalloc((void**)&ret_gpu, sizeof(double)), __FILE__, __LINE__);
     checkCudaErrors(cudaMemsetAsync(ret_gpu, 0, sizeof(double), *cuda_stream),
         __FILE__, __LINE__);
 
-    // this loop_dim is not the same as that of the gpu function
-    // and the function uses grid stride loops
-    ITYPE loop_dim;
-
-    if (dim <= 64)
-        loop_dim = dim >> 1;
-    else if (dim <= (1ULL << 11))
-        loop_dim = dim >> 2;
-    else
-        loop_dim = dim >> 5;
-
-    unsigned int block = loop_dim <= 256 ? loop_dim : 256;
-    unsigned int grid = loop_dim / block;
-
-    // unsigned int block = loop_dim <= 1024 ? loop_dim : 1024;
-    // unsigned int grid = loop_dim / block;
+    ITYPE loop_dim = get_loop_dim_of_reduction_function(dim);
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        expectation_value_multi_qubit_Pauli_operator_Z_mask_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
 
     expectation_value_multi_qubit_Pauli_operator_Z_mask_gpu<<<grid, block, 0,
         *cuda_stream>>>(ret_gpu, phase_flip_mask, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
     checkCudaErrors(cudaStatus, __FILE__, __LINE__);
@@ -1227,24 +1205,19 @@
     GTYPE* ret_gpu;
 
     checkCudaErrors(
         cudaMalloc((void**)&ret_gpu, sizeof(GTYPE)), __FILE__, __LINE__);
     checkCudaErrors(cudaMemsetAsync(ret_gpu, 0, sizeof(GTYPE), *cuda_stream),
         __FILE__, __LINE__);
 
-    ITYPE loop_dim;
-    if (dim <= 32)
-        loop_dim = dim >> 1;
-    else if (dim <= 4096)
-        loop_dim = dim >> 2;
-    else
-        loop_dim = dim >> 5;
-
-    unsigned int block = loop_dim <= 256 ? loop_dim : 256;
-    unsigned int grid = loop_dim / block;
+    ITYPE loop_dim = get_loop_dim_of_reduction_function(dim >> 1);
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        transition_amplitude_multi_qubit_Pauli_operator_XZ_mask_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
 
     transition_amplitude_multi_qubit_Pauli_operator_XZ_mask_gpu<<<grid, block,
         0, *cuda_stream>>>(ret_gpu, bit_flip_mask, phase_flip_mask,
         global_phase_90rot_count, pivot_qubit_index, state_bra_gpu,
         state_ket_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
@@ -1296,24 +1269,19 @@
     GTYPE* ret_gpu;
 
     checkCudaErrors(
         cudaMalloc((void**)&ret_gpu, sizeof(GTYPE)), __FILE__, __LINE__);
     checkCudaErrors(cudaMemsetAsync(ret_gpu, 0, sizeof(GTYPE), *cuda_stream),
         __FILE__, __LINE__);
 
-    ITYPE loop_dim;
-    if (dim <= 32)
-        loop_dim = dim >> 1;
-    else if (dim <= 4096)
-        loop_dim = dim >> 2;
-    else
-        loop_dim = dim >> 5;
-
-    unsigned int block = loop_dim <= 256 ? loop_dim : 256;
-    unsigned int grid = loop_dim / block;
+    ITYPE loop_dim = get_loop_dim_of_reduction_function(dim);
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        transition_amplitude_multi_qubit_Pauli_operator_Z_mask_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
 
     transition_amplitude_multi_qubit_Pauli_operator_Z_mask_gpu<<<grid, block, 0,
         *cuda_stream>>>(
         ret_gpu, phase_flip_mask, state_bra_gpu, state_ket_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
```

### Comparing `qulacs-0.6.3/src/gpusim/stat_ops.h` & `qulacs-0.6.4/src/gpusim/stat_ops.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/gpusim/stat_ops_device_functions.h` & `qulacs-0.6.4/src/gpusim/stat_ops_device_functions.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/gpusim/test.cpp` & `qulacs-0.6.4/src/gpusim/test.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/gpusim/update_ops_cuda.h` & `qulacs-0.6.4/src/gpusim/update_ops_cuda.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/gpusim/update_ops_cuda_device_functions.h` & `qulacs-0.6.4/src/gpusim/update_ops_cuda_device_functions.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/gpusim/update_ops_multi.cu` & `qulacs-0.6.4/src/gpusim/update_ops_multi.cu`

 * *Files 6% similar despite different names*

```diff
@@ -229,16 +229,18 @@
     cudaError cudaStatus;
     checkCudaErrors(
         cudaMemcpyToSymbolAsync(matrix_const_gpu, matrix, sizeof(GTYPE) * 256,
             0, cudaMemcpyHostToDevice, *cuda_stream),
         __FILE__, __LINE__);
     ITYPE loop_dim = dim >> 4;
 
-    unsigned int block = loop_dim <= 512 ? loop_dim : 512;
-    unsigned int grid = loop_dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(quad_qubit_dense_matrix_gate_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
     unsigned int target0_qubit_index, target1_qubit_index, target2_qubit_index,
         target3_qubit_index;
     target0_qubit_index = target_qubit_index[0];
     target1_qubit_index = target_qubit_index[1];
     target2_qubit_index = target_qubit_index[2];
     target3_qubit_index = target_qubit_index[3];
 
@@ -331,16 +333,18 @@
     checkCudaErrors(
         cudaMemcpyToSymbolAsync(matrix_const_gpu, matrix, sizeof(GTYPE) * 64, 0,
             cudaMemcpyHostToDevice, *cuda_stream),
         __FILE__, __LINE__);
 
     // (not using shared memory)
     ITYPE loop_dim = dim >> 3;
-    unsigned int block = loop_dim <= 512 ? loop_dim : 512;
-    unsigned int grid = loop_dim / block;
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        triple_qubit_dense_matrix_gate_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
 
     unsigned int small, mid, large, tmp;
     small = target0_qubit_index;
     mid = target1_qubit_index;
     large = target2_qubit_index;
     if (small > mid) {
         tmp = small;
@@ -428,16 +432,18 @@
     cudaError cudaStatus;
 
     checkCudaErrors(
         cudaMemcpyToSymbolAsync(matrix_const_gpu, matrix, sizeof(GTYPE) * 16, 0,
             cudaMemcpyHostToDevice, *cuda_stream),
         __FILE__, __LINE__);
     ITYPE quad_dim = dim >> 2;
-    unsigned int block = quad_dim <= 1024 ? quad_dim : 1024;
-    unsigned int grid = quad_dim / block;
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        double_qubit_dense_matrix_gate_gpu);
+    unsigned int block = quad_dim <= max_block_size ? quad_dim : max_block_size;
+    unsigned int grid = (quad_dim + block - 1) / block;
 
     unsigned int small;
     unsigned int large;
     small = (target0_qubit_index < target1_qubit_index) ? target0_qubit_index
                                                         : target1_qubit_index;
     large = (target0_qubit_index < target1_qubit_index) ? target1_qubit_index
                                                         : target0_qubit_index;
@@ -478,16 +484,18 @@
     void* state, ITYPE dim, void* stream, unsigned int device_number) {
     int current_device = get_current_device();
     if (device_number != current_device) cudaSetDevice((int)device_number);
 
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaError cudaStatus;
-    unsigned int block = dim <= 1024 ? dim : 1024;
-    unsigned int grid = dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(multi_qubit_Pauli_gate_Z_mask_gpu);
+    unsigned int block = dim <= max_block_size ? dim : max_block_size;
+    unsigned int grid = (dim + block - 1) / block;
 
     multi_qubit_Pauli_gate_Z_mask_gpu<<<grid, block, 0, *cuda_stream>>>(
         phase_flip_mask, state_gpu, dim);
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
     checkCudaErrors(cudaStatus, __FILE__, __LINE__);
     state = reinterpret_cast<void*>(state_gpu);
@@ -541,16 +549,19 @@
     UINT pivot_qubit_index, void* state, ITYPE dim, void* stream,
     unsigned int device_number) {
     int current_device = get_current_device();
     if (device_number != current_device) cudaSetDevice((int)device_number);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaError cudaStatus;
-    unsigned int block = dim <= 1024 ? dim : 1024;
-    unsigned int grid = dim / block;
+    ITYPE loop_dim = dim >> 1;
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        multi_qubit_Pauli_gate_XZ_mask_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
 
     multi_qubit_Pauli_gate_XZ_mask_gpu<<<grid, block, 0, *cuda_stream>>>(
         bit_flip_mask, phase_flip_mask, global_phase_90rot_count,
         pivot_qubit_index, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
@@ -624,16 +635,19 @@
     UINT pivot_qubit_index, double angle, void* state, ITYPE dim, void* stream,
     unsigned int device_number) {
     int current_device = get_current_device();
     if (device_number != current_device) cudaSetDevice((int)device_number);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaError cudaStatus;
-    unsigned int block = dim <= 1024 ? dim : 1024;
-    unsigned int grid = dim / block;
+    ITYPE loop_dim = dim >> 1;
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        multi_qubit_Pauli_rotation_gate_XZ_mask_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
 
     multi_qubit_Pauli_rotation_gate_XZ_mask_gpu<<<grid, block, 0,
         *cuda_stream>>>(bit_flip_mask, phase_flip_mask,
         global_phase_90rot_count, pivot_qubit_index, angle, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
@@ -671,16 +685,18 @@
     double angle, void* state, ITYPE dim, void* stream,
     unsigned int device_number) {
     int current_device = get_current_device();
     if (device_number != current_device) cudaSetDevice((int)device_number);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaError cudaStatus;
-    unsigned int block = dim <= 1024 ? dim : 1024;
-    unsigned int grid = dim / block;
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        multi_qubit_Pauli_rotation_gate_Z_mask_gpu);
+    unsigned int block = dim <= max_block_size ? dim : max_block_size;
+    unsigned int grid = (dim + block - 1) / block;
 
     multi_qubit_Pauli_rotation_gate_Z_mask_gpu<<<grid, block, 0,
         *cuda_stream>>>(phase_flip_mask, angle, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
     checkCudaErrors(cudaStatus, __FILE__, __LINE__);
@@ -1304,27 +1320,22 @@
         target_qubit_index_list, target_qubit_index_count, control_qubit_index);
 
     GTYPE *d_matrix, *d_matrix_mask_list;
 
     // loop varaibles
     const ITYPE loop_dim = dim >> insert_index_count;
 
-    unsigned int block = loop_dim <= 1024 ? loop_dim : 1024;
-    unsigned int grid = loop_dim / block;
-
     if (target_qubit_index_count <= 10) {
-        if (target_qubit_index_count >= 3) {
-            unsigned int tmp_block = 1ULL << (13 - target_qubit_index_count);
-            block = loop_dim <= tmp_block ? loop_dim : tmp_block;
-        } else {
-            block = loop_dim <= 1024 ? loop_dim : 1024;
-        }
-        grid = loop_dim / block;
-
         if (target_qubit_index_count <= 5) {
+            unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+                static_cast<void (*)(UINT, UINT, UINT, GTYPE*, ITYPE)>(
+                    single_qubit_control_multi_qubit_dense_matrix_gate_const_gpu));
+            unsigned int block =
+                loop_dim <= max_block_size ? loop_dim : max_block_size;
+            unsigned int grid = (loop_dim + block - 1) / block;
             checkCudaErrors(cudaMemcpyToSymbolAsync(matrix_const_gpu, matrix,
                                 sizeof(GTYPE) * matrix_dim * matrix_dim, 0,
                                 cudaMemcpyHostToDevice, *cuda_stream),
                 __FILE__, __LINE__);
             checkCudaErrors(cudaMemcpyToSymbolAsync(matrix_mask_list_gpu,
                                 matrix_mask_list, sizeof(ITYPE) * matrix_dim, 0,
                                 cudaMemcpyHostToDevice, *cuda_stream),
@@ -1336,14 +1347,21 @@
                     cudaMemcpyHostToDevice, *cuda_stream),
                 __FILE__, __LINE__);
 
             single_qubit_control_multi_qubit_dense_matrix_gate_const_gpu<<<grid,
                 block, 0, *cuda_stream>>>(control_qubit_index, control_value,
                 target_qubit_index_count, state_gpu, dim);
         } else {
+            unsigned int max_block_size =
+                get_block_size_to_maximize_occupancy(static_cast<void (*)(
+                        UINT, UINT, UINT, const GTYPE*, GTYPE*, ITYPE)>(
+                    single_qubit_control_multi_qubit_dense_matrix_gate_const_gpu));
+            unsigned int block =
+                loop_dim <= max_block_size ? loop_dim : max_block_size;
+            unsigned int grid = (loop_dim + block - 1) / block;
             checkCudaErrors(cudaMalloc(reinterpret_cast<void**>(&d_matrix),
                                 matrix_dim * matrix_dim * sizeof(GTYPE)),
                 __FILE__, __LINE__);
             checkCudaErrors(cudaMemcpyAsync(d_matrix, matrix,
                                 matrix_dim * matrix_dim * sizeof(GTYPE),
                                 cudaMemcpyHostToDevice, *cuda_stream),
                 __FILE__, __LINE__);
@@ -1500,27 +1518,22 @@
 
     // loop varaibles
     const ITYPE loop_dim =
         dim >> (target_qubit_index_count + control_qubit_index_count);
 
     GTYPE *d_matrix, *d_matrix_mask_list;
 
-    unsigned int block = loop_dim <= 1024 ? loop_dim : 1024;
-    unsigned int grid = loop_dim / block;
-
     if (target_qubit_index_count <= 10) {
-        if (target_qubit_index_count >= 3) {
-            unsigned int tmp_block = 1ULL << (13 - target_qubit_index_count);
-            block = loop_dim <= tmp_block ? loop_dim : tmp_block;
-        } else {
-            block = loop_dim <= 1024 ? loop_dim : 1024;
-        }
-        grid = loop_dim / block;
-
         if (target_qubit_index_count <= 5) {
+            unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+                static_cast<void (*)(ITYPE, UINT, ITYPE, GTYPE*, ITYPE)>(
+                    multi_qubit_control_multi_qubit_dense_matrix_gate_const_gpu));
+            unsigned int block =
+                loop_dim <= max_block_size ? loop_dim : max_block_size;
+            unsigned int grid = (loop_dim + block - 1) / block;
             checkCudaErrors(cudaMemcpyToSymbolAsync(matrix_const_gpu, matrix,
                                 sizeof(GTYPE) * matrix_dim * matrix_dim, 0,
                                 cudaMemcpyHostToDevice, *cuda_stream),
                 __FILE__, __LINE__);
             checkCudaErrors(cudaMemcpyToSymbolAsync(matrix_mask_list_gpu,
                                 matrix_mask_list, sizeof(ITYPE) * matrix_dim, 0,
                                 cudaMemcpyHostToDevice, *cuda_stream),
@@ -1534,14 +1547,21 @@
                 __FILE__, __LINE__);
 
             multi_qubit_control_multi_qubit_dense_matrix_gate_const_gpu<<<grid,
                 block, 0, *cuda_stream>>>(control_mask,
                 target_qubit_index_count, control_qubit_index_count, state_gpu,
                 dim);
         } else {
+            unsigned int max_block_size =
+                get_block_size_to_maximize_occupancy(static_cast<void (*)(
+                        ITYPE, UINT, ITYPE, const GTYPE*, GTYPE*, ITYPE)>(
+                    multi_qubit_control_multi_qubit_dense_matrix_gate_const_gpu));
+            unsigned int block =
+                loop_dim <= max_block_size ? loop_dim : max_block_size;
+            unsigned int grid = (loop_dim + block - 1) / block;
             checkCudaErrors(cudaMalloc(reinterpret_cast<void**>(&d_matrix),
                                 matrix_dim * matrix_dim * sizeof(GTYPE)),
                 __FILE__, __LINE__);
             checkCudaErrors(cudaMemcpyAsync(d_matrix, matrix,
                                 matrix_dim * matrix_dim * sizeof(GTYPE),
                                 cudaMemcpyHostToDevice, *cuda_stream),
                 __FILE__, __LINE__);
@@ -1615,16 +1635,19 @@
 
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     checkCudaErrors(cudaMemcpyToSymbol(
                         matrix_const_gpu, diagonal_matrix, sizeof(GTYPE) * dim),
         __FILE__, __LINE__);
 
-    unsigned int block = dim <= 1024 ? dim : 1024;
-    unsigned int grid = dim / block;
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        static_cast<void (*)(GTYPE*, ITYPE)>(
+            multi_qubit_diagonal_matrix_gate_gpu));
+    unsigned int block = dim <= max_block_size ? dim : max_block_size;
+    unsigned int grid = (dim + block - 1) / block;
 
     multi_qubit_diagonal_matrix_gate_gpu<<<grid, block, 0, *cuda_stream>>>(
         state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     checkCudaErrors(cudaGetLastError(), __FILE__, __LINE__);
     state = reinterpret_cast<void*>(state_gpu);
@@ -1642,16 +1665,19 @@
     checkCudaErrors(
         cudaMalloc((void**)&d_matrix, sizeof(GTYPE) * dim), __FILE__, __LINE__);
     checkCudaErrors(
         cudaMemcpyAsync(d_matrix, diagonal_matrix, sizeof(GTYPE) * dim,
             cudaMemcpyHostToDevice, *cuda_stream),
         __FILE__, __LINE__);
 
-    unsigned int block = dim <= 1024 ? dim : 1024;
-    unsigned int grid = dim / block;
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        static_cast<void (*)(GTYPE*, GTYPE*, ITYPE)>(
+            multi_qubit_diagonal_matrix_gate_gpu));
+    unsigned int block = dim <= max_block_size ? dim : max_block_size;
+    unsigned int grid = (dim + block - 1) / block;
 
     multi_qubit_diagonal_matrix_gate_gpu<<<grid, block, 0, *cuda_stream>>>(
         d_matrix, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     checkCudaErrors(cudaGetLastError(), __FILE__, __LINE__);
     cudaFree(d_matrix);
```

### Comparing `qulacs-0.6.3/src/gpusim/update_ops_named.cu` & `qulacs-0.6.4/src/gpusim/update_ops_named.cu`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #include <cuComplex.h>
 
 #include "cuda_runtime.h"
 #include "device_launch_parameters.h"
-//#include "util.h"
+// #include "util.h"
 #include "update_ops_cuda.h"
 #include "update_ops_cuda_device_functions.h"
 #include "util.cuh"
 #include "util_func.h"
 #include "util_type.h"
 #include "util_type_internal.h"
 
@@ -42,16 +42,18 @@
     int current_device = get_current_device();
     if (device_number != current_device) cudaSetDevice((int)device_number);
 
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     cudaError cudaStatus;
     ITYPE half_dim = dim >> 1;
-    unsigned int block = half_dim <= 1024 ? half_dim : 1024;
-    unsigned int grid = half_dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(H_gate_gpu);
+    unsigned int block = half_dim <= max_block_size ? half_dim : max_block_size;
+    unsigned int grid = (half_dim + block - 1) / block;
 
     H_gate_gpu<<<grid, block, 0, *cuda_stream>>>(
         target_qubit_index, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
     checkCudaErrors(cudaStatus, __FILE__, __LINE__);
@@ -83,16 +85,18 @@
     int current_device = get_current_device();
     if (device_number != current_device) cudaSetDevice(device_number);
 
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     cudaError cudaStatus;
     ITYPE half_dim = dim >> 1;
-    unsigned int block = half_dim <= 1024 ? half_dim : 1024;
-    unsigned int grid = half_dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(X_gate_gpu);
+    unsigned int block = half_dim <= max_block_size ? half_dim : max_block_size;
+    unsigned int grid = (half_dim + block - 1) / block;
 
     X_gate_gpu<<<grid, block, 0, *cuda_stream>>>(
         target_qubit_index, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
     checkCudaErrors(cudaStatus, __FILE__, __LINE__);
@@ -123,16 +127,18 @@
     int current_device = get_current_device();
     if (device_number != current_device) cudaSetDevice(device_number);
 
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     cudaError cudaStatus;
     ITYPE half_dim = dim >> 1;
-    unsigned int block = half_dim <= 1024 ? half_dim : 1024;
-    unsigned int grid = half_dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(Y_gate_gpu);
+    unsigned int block = half_dim <= max_block_size ? half_dim : max_block_size;
+    unsigned int grid = (half_dim + block - 1) / block;
 
     Y_gate_gpu<<<grid, block, 0, *cuda_stream>>>(
         target_qubit_index, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
     checkCudaErrors(cudaStatus, __FILE__, __LINE__);
@@ -156,16 +162,18 @@
     int current_device = get_current_device();
     if (device_number != current_device) cudaSetDevice(device_number);
 
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     cudaError cudaStatus;
     ITYPE half_dim = dim >> 1;
-    unsigned int block = half_dim <= 1024 ? half_dim : 1024;
-    unsigned int grid = half_dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(Z_gate_gpu);
+    unsigned int block = half_dim <= max_block_size ? half_dim : max_block_size;
+    unsigned int grid = (half_dim + block - 1) / block;
 
     Z_gate_gpu<<<grid, block, 0, *cuda_stream>>>(
         target_qubit_index, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
     checkCudaErrors(cudaStatus, __FILE__, __LINE__);
@@ -209,16 +217,18 @@
         large_index = control_qubit_index;
         small_index = target_qubit_index;
     } else {
         large_index = target_qubit_index;
         small_index = control_qubit_index;
     }
 
-    unsigned int block = quad_dim <= 1024 ? quad_dim : 1024;
-    unsigned int grid = quad_dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(CZ_gate_gpu);
+    unsigned int block = quad_dim <= max_block_size ? quad_dim : max_block_size;
+    unsigned int grid = (quad_dim + block - 1) / block;
 
     CZ_gate_gpu<<<grid, block, 0, *cuda_stream>>>(
         large_index, small_index, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
     checkCudaErrors(cudaStatus, __FILE__, __LINE__);
@@ -267,16 +277,18 @@
     int current_device = get_current_device();
     if (device_number != current_device) cudaSetDevice(device_number);
 
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     cudaError cudaStatus;
     ITYPE quad_dim = dim >> 2;
-    unsigned int block = quad_dim <= 1024 ? quad_dim : 1024;
-    unsigned int grid = quad_dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(CNOT_gate_gpu);
+    unsigned int block = quad_dim <= max_block_size ? quad_dim : max_block_size;
+    unsigned int grid = (quad_dim + block - 1) / block;
 
     CNOT_gate_gpu<<<grid, block, 0, *cuda_stream>>>(
         control_qubit_index, target_qubit_index, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
     checkCudaErrors(cudaStatus, __FILE__, __LINE__);
@@ -317,16 +329,18 @@
     if (device_number != current_device) cudaSetDevice(device_number);
 
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     cudaError cudaStatus;
     unsigned int large_index, small_index;
     ITYPE quad_dim = dim >> 2;
-    unsigned int block = quad_dim <= 1024 ? quad_dim : 1024;
-    unsigned int grid = quad_dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(SWAP_gate_gpu);
+    unsigned int block = quad_dim <= max_block_size ? quad_dim : max_block_size;
+    unsigned int grid = (quad_dim + block - 1) / block;
 
     if (target_qubit_index1 > target_qubit_index0) {
         large_index = target_qubit_index1;
         small_index = target_qubit_index0;
     } else {
         large_index = target_qubit_index0;
         small_index = target_qubit_index1;
@@ -360,17 +374,18 @@
     int current_device = get_current_device();
     if (device_number != current_device) cudaSetDevice(device_number);
 
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     cudaError cudaStatus;
     const ITYPE loop_dim = dim >> 1;
-
-    unsigned int block = loop_dim <= 1024 ? loop_dim : 1024;
-    unsigned int grid = loop_dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(P0_gate_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
 
     P0_gate_gpu<<<grid, block, 0, *cuda_stream>>>(
         target_qubit_index, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
     checkCudaErrors(cudaStatus, __FILE__, __LINE__);
@@ -395,16 +410,18 @@
     if (device_number != current_device) cudaSetDevice(device_number);
 
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     cudaError cudaStatus;
     const ITYPE loop_dim = dim >> 1;
 
-    unsigned int block = loop_dim <= 1024 ? loop_dim : 1024;
-    unsigned int grid = loop_dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(P1_gate_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
 
     P1_gate_gpu<<<grid, block, 0, *cuda_stream>>>(
         target_qubit_index, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
     checkCudaErrors(cudaStatus, __FILE__, __LINE__);
@@ -431,16 +448,18 @@
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     cudaError cudaStatus;
     const ITYPE loop_dim = dim;
     const double normalize_factor = sqrt(1. / squared_norm);
     // const double normalize_factor = 1. / norm;
 
-    unsigned int block = loop_dim <= 1024 ? loop_dim : 1024;
-    unsigned int grid = loop_dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(normalize_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
 
     normalize_gpu<<<grid, block, 0, *cuda_stream>>>(
         normalize_factor, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
     checkCudaErrors(cudaStatus, __FILE__, __LINE__);
```

### Comparing `qulacs-0.6.3/src/gpusim/update_ops_single.cu` & `qulacs-0.6.4/src/gpusim/update_ops_single.cu`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #include <cuComplex.h>
 
 #include "cuda_runtime.h"
 #include "device_launch_parameters.h"
-//#include "util.h"
+// #include "util.h"
 #include <assert.h>
 
 #include "update_ops_cuda.h"
 #include "update_ops_cuda_device_functions.h"
 #include "util.cuh"
 #include "util_func.h"
 #include "util_type.h"
@@ -114,16 +114,18 @@
     if (device_number != current_device) cudaSetDevice(device_number);
 
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     cudaError cudaStatus;
 
     ITYPE loop_dim = dim >> 1;
-    unsigned int block = loop_dim <= 1024 ? loop_dim : 1024;
-    unsigned int grid = loop_dim / block;
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        single_qubit_dense_matrix_gate_gpu);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
     GTYPE mat[4];
     for (int i = 0; i < 4; ++i)
         mat[i] = make_cuDoubleComplex(matrix[i].real(), matrix[i].imag());
     single_qubit_dense_matrix_gate_gpu<<<grid, block, 0, *cuda_stream>>>(
         mat[0], mat[1], mat[2], mat[3], target_qubit_index, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
@@ -159,16 +161,18 @@
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     cudaError cudaStatus;
     checkCudaErrors(
         cudaMemcpyToSymbolAsync(matrix_const_gpu, diagonal_matrix,
             sizeof(GTYPE) * 2, 0, cudaMemcpyHostToDevice, *cuda_stream),
         __FILE__, __LINE__);
 
-    unsigned int block = dim <= 1024 ? dim : 1024;
-    unsigned int grid = dim / block;
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        single_qubit_diagonal_matrix_gate_gpu);
+    unsigned int block = dim <= max_block_size ? dim : max_block_size;
+    unsigned int grid = (dim + block - 1) / block;
 
     single_qubit_diagonal_matrix_gate_gpu<<<grid, block, 0, *cuda_stream>>>(
         target_qubit_index, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
     checkCudaErrors(cudaStatus, __FILE__, __LINE__);
@@ -234,16 +238,18 @@
     cudaError cudaStatus;
     checkCudaErrors(
         cudaMemcpyToSymbolAsync(matrix_const_gpu, matrix, sizeof(GTYPE) * 4, 0,
             cudaMemcpyHostToDevice, *cuda_stream),
         __FILE__, __LINE__);
 
     ITYPE quad_dim = dim >> 2;
-    unsigned int block = quad_dim <= 1024 ? quad_dim : 1024;
-    unsigned int grid = quad_dim / block;
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        single_qubit_control_single_qubit_dense_matrix_gate_gpu);
+    unsigned int block = quad_dim <= max_block_size ? quad_dim : max_block_size;
+    unsigned int grid = (quad_dim + block - 1) / block;
 
     single_qubit_control_single_qubit_dense_matrix_gate_gpu<<<grid, block, 0,
         *cuda_stream>>>(
         control_qubit_index, control_value, target_qubit_index, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
@@ -285,16 +291,18 @@
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
     GTYPE phase_gtype;
     cudaError cudaStatus;
 
     phase_gtype = make_cuDoubleComplex(phase.real(), phase.imag());
     ITYPE half_dim = dim >> 1;
-    unsigned int block = half_dim <= 1024 ? half_dim : 1024;
-    unsigned int grid = half_dim / block;
+    unsigned int max_block_size =
+        get_block_size_to_maximize_occupancy(single_qubit_phase_gate_gpu);
+    unsigned int block = half_dim <= max_block_size ? half_dim : max_block_size;
+    unsigned int grid = (half_dim + block - 1) / block;
 
     single_qubit_phase_gate_gpu<<<grid, block, 0, *cuda_stream>>>(
         target_qubit_index, phase_gtype, state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     cudaStatus = cudaGetLastError();
     checkCudaErrors(cudaStatus, __FILE__, __LINE__);
@@ -360,16 +368,18 @@
     // control mask
     ITYPE control_mask = create_control_mask_gsim(control_qubit_index_list,
         control_value_list, control_qubit_index_count);
 
     // loop varaibles
     const ITYPE loop_dim = dim >> insert_index_list_count;
 
-    unsigned int block = loop_dim <= 1024 ? loop_dim : 1024;
-    unsigned int grid = loop_dim / block;
+    unsigned int max_block_size = get_block_size_to_maximize_occupancy(
+        multi_qubit_control_single_qubit_dense_matrix_gate);
+    unsigned int block = loop_dim <= max_block_size ? loop_dim : max_block_size;
+    unsigned int grid = (loop_dim + block - 1) / block;
 
     checkCudaErrors(
         cudaMemcpyToSymbol(matrix_const_gpu, matrix, sizeof(GTYPE) * 4),
         __FILE__, __LINE__);
     checkCudaErrors(cudaMemcpyToSymbol(insert_index_list_gpu, insert_index_list,
                         sizeof(UINT) * insert_index_list_count),
         __FILE__, __LINE__);
```

### Comparing `qulacs-0.6.3/src/gpusim/util.cu` & `qulacs-0.6.4/src/gpusim/util.cu`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #include "cuda_runtime.h"
 #include "device_launch_parameters.h"
-//#include "cuda.h"
-// for using cublas
+// #include "cuda.h"
+//  for using cublas
 #include <assert.h>
 #include <cuComplex.h>
 #include <cublas_v2.h>
 
 #include <algorithm>
 #include <cmath>
 #include <complex>
@@ -178,14 +178,36 @@
                   << state_cpu[i].imag() << '\n';
     }
     std::cout << '\n';
     free(state_cpu);
     state = reinterpret_cast<void*>(state);
 }
 
+// As a result of experience, loop_dim = dim >> (n_qubits/2-2) always performs
+// almost the best. ref:
+// https://github.com/qulacs/qulacs/issues/618#issuecomment-2024279795
+ITYPE get_loop_dim_of_reduction_function(ITYPE dim) {
+    if (dim <= 1ULL << 4) return dim;
+    if (dim <= 1ULL << 6) return 1ULL << 5;
+    if (dim <= 1ULL << 8) return 1ULL << 6;
+    if (dim <= 1ULL << 10) return 1ULL << 7;
+    if (dim <= 1ULL << 12) return 1ULL << 8;
+    if (dim <= 1ULL << 14) return 1ULL << 9;
+    if (dim <= 1ULL << 16) return 1ULL << 10;
+    if (dim <= 1ULL << 18) return 1ULL << 11;
+    if (dim <= 1ULL << 20) return 1ULL << 12;
+    if (dim <= 1ULL << 22) return 1ULL << 13;
+    if (dim <= 1ULL << 24) return 1ULL << 14;
+    if (dim <= 1ULL << 26) return 1ULL << 15;
+    if (dim <= 1ULL << 28) return 1ULL << 16;
+    if (dim <= 1ULL << 30) return 1ULL << 17;
+    if (dim <= 1ULL << 32) return 1ULL << 18;
+    return 1ULL << 18;
+}
+
 ITYPE
 insert_zero_to_basis_index_gsim(ITYPE basis_index, unsigned int qubit_index) {
     ITYPE temp_basis = (basis_index >> qubit_index) << (qubit_index + 1);
     return temp_basis + (basis_index & ((1ULL << qubit_index) - 1));
 }
 
 void get_Pauli_masks_partial_list_gsim(const UINT* target_qubit_index_list,
```

### Comparing `qulacs-0.6.3/src/gpusim/util.cuh` & `qulacs-0.6.4/src/gpusim/util.cuh`

 * *Files 27% similar despite different names*

```diff
@@ -7,31 +7,43 @@
 #include <cstdlib>
 #include <cstring>
 #include <iostream>
 #include <string>
 
 #include "cuda_runtime.h"
 #include "device_launch_parameters.h"
-//#include <sys/time.h>
+// #include <sys/time.h>
 #include <cuComplex.h>
 
 #include "util_type.h"
 #include "util_type_internal.h"
 
-//#include "util_type.h"
+// #include "util_type.h"
 
 inline void checkCudaErrors(
     const cudaError error, std::string filename, int line) {
     if (error != cudaSuccess) {
         printf("Error: %s:%d, ", filename.c_str(), line);
         printf("code: %d, reason: %s\n", error, cudaGetErrorString(error));
         exit(1);
     }
 }
 
+// As a result of the experience, using `cudaOccupancyMaxPotentialBlockSize`
+// does not lose performance. ref:
+// https://github.com/qulacs/qulacs/issues/618#issuecomment-2011658886
+template <typename F>
+inline unsigned int get_block_size_to_maximize_occupancy(F func,
+    unsigned int dynamic_s_mem_size = 0, unsigned int block_size_limit = 0) {
+    int block_size, min_grid_size;
+    cudaOccupancyMaxPotentialBlockSize(&min_grid_size, &block_size, func,
+        dynamic_s_mem_size, block_size_limit);
+    return block_size;
+}
+
 /*
 //inline void memcpy_quantum_state_HostToDevice(CPPCTYPE* state_cpu, GTYPE*
 state_gpu, ITYPE dim){ inline void memcpy_quantum_state_HostToDevice(CPPCTYPE*
 state_cpu, GTYPE* state_gpu, ITYPE dim, void* stream, UINT device_number){
         cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
         int current_device = get_current_device();
         if (device_number != current_device) cudaSetDevice(device_number);
```

### Comparing `qulacs-0.6.3/src/gpusim/util.h` & `qulacs-0.6.4/src/gpusim/util.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/gpusim/util_common.h` & `qulacs-0.6.4/src/gpusim/util_common.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/gpusim/util_func.h` & `qulacs-0.6.4/src/gpusim/util_func.h`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     const void* state_gpu_original, ITYPE dim, void* stream,
     unsigned int device_number);
 DllExport void get_quantum_state_host(void* state_gpu, void* psi_cpu_copy,
     ITYPE dim, void* stream, unsigned int device_number);
 DllExport void print_quantum_state_host(
     void* state, ITYPE dim, unsigned int device_number);
 
+ITYPE get_loop_dim_of_reduction_function(ITYPE dim);
+
 ITYPE
 insert_zero_to_basis_index_gsim(ITYPE basis_index, unsigned int qubit_index);
 void get_Pauli_masks_partial_list_gsim(const UINT* target_qubit_index_list,
     const UINT* Pauli_operator_type_list, UINT target_qubit_index_count,
     ITYPE* bit_flip_mask, ITYPE* phase_flip_mask,
     UINT* global_phase_90rot_count, UINT* pivot_qubit_index);
 void get_Pauli_masks_whole_list_gsim(const UINT* Pauli_operator_type_list,
```

### Comparing `qulacs-0.6.3/src/vqcsim/GradCalculator.cpp` & `qulacs-0.6.4/src/vqcsim/GradCalculator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/vqcsim/boolean_formula.hpp` & `qulacs-0.6.4/src/vqcsim/boolean_formula.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/vqcsim/causalcone_simulator.hpp` & `qulacs-0.6.4/src/vqcsim/causalcone_simulator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/vqcsim/differential.cpp` & `qulacs-0.6.4/src/vqcsim/differential.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/vqcsim/differential.hpp` & `qulacs-0.6.4/src/vqcsim/differential.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/vqcsim/loss_function.cpp` & `qulacs-0.6.4/src/vqcsim/loss_function.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/vqcsim/loss_function.hpp` & `qulacs-0.6.4/src/vqcsim/loss_function.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/vqcsim/optimizer.hpp` & `qulacs-0.6.4/src/vqcsim/optimizer.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/vqcsim/parametric_circuit.cpp` & `qulacs-0.6.4/src/vqcsim/parametric_circuit.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/vqcsim/parametric_circuit.hpp` & `qulacs-0.6.4/src/vqcsim/parametric_circuit.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/vqcsim/parametric_gate.hpp` & `qulacs-0.6.4/src/vqcsim/parametric_gate.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/vqcsim/parametric_gate_factory.cpp` & `qulacs-0.6.4/src/vqcsim/parametric_gate_factory.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/vqcsim/parametric_gate_factory.hpp` & `qulacs-0.6.4/src/vqcsim/parametric_gate_factory.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/vqcsim/parametric_simulator.cpp` & `qulacs-0.6.4/src/vqcsim/parametric_simulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/vqcsim/parametric_simulator.hpp` & `qulacs-0.6.4/src/vqcsim/parametric_simulator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/vqcsim/problem.hpp` & `qulacs-0.6.4/src/vqcsim/problem.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/src/vqcsim/solver.hpp` & `qulacs-0.6.4/src/vqcsim/solver.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_KAK.cpp` & `qulacs-0.6.4/test/cppsim/test_KAK.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_circuit.cpp` & `qulacs-0.6.4/test/cppsim/test_circuit.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_circuit_multicpu.cpp` & `qulacs-0.6.4/test/cppsim/test_circuit_multicpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_circuit_optimize_light.cpp` & `qulacs-0.6.4/test/cppsim/test_circuit_optimize_light.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #include <cppsim/pauli_operator.hpp>
 #include <cppsim/state.hpp>
 #include <cppsim/type.hpp>
 #include <cppsim/utility.hpp>
 #include <csim/constant.hpp>
 #include <unsupported/Eigen/MatrixFunctions>
 #include <utility>
+#include <vqcsim/parametric_circuit.hpp>
 
 #include "../util/util.hpp"
 
 TEST(CircuitTest, CircuitOptimizeLight) {
     const UINT n = 4;
     const UINT dim = 1ULL << n;
 
@@ -140,14 +141,44 @@
         ASSERT_STATE_NEAR(state, test_state, eps);
         ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
         ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
         delete copy_circuit;
     }
 }
 
+// Regression test for #634.
+// This test checks if the optimizer leaves parametric gates as is.
+TEST(CircuitTest, CircuitOptimizeLightParameterUnchanged) {
+    const UINT n = 2;
+    const UINT dim = 1ULL << n;
+
+    QuantumState state(n), test_state(n);
+    state.set_Haar_random_state();
+    test_state.load(&state);
+    ParametricQuantumCircuit circuit(n);
+
+    circuit.add_X_gate(0);
+    circuit.add_parametric_RX_gate(0, 0.1);
+    circuit.add_parametric_RY_gate(0, 0.1);
+    UINT expected_depth = 3;
+    UINT expected_gate_count = 3;
+
+    ParametricQuantumCircuit* copy_circuit = circuit.copy();
+    QuantumCircuitOptimizer qco;
+    qco.optimize_light(copy_circuit);
+    circuit.update_quantum_state(&test_state);
+    copy_circuit->update_quantum_state(&state);
+
+    ASSERT_STATE_NEAR(state, test_state, eps);
+    ASSERT_EQ(copy_circuit->calculate_depth(), expected_depth);
+    ASSERT_EQ(copy_circuit->gate_list.size(), expected_gate_count);
+    ASSERT_EQ(copy_circuit->get_parameter_count(), 2);
+    delete copy_circuit;
+}
+
 TEST(CircuitTest, RandomCircuitOptimizeLight) {
     const UINT n = 5;
     const UINT dim = 1ULL << n;
     const UINT depth = 5;
     Random random;
 
     UINT max_repeat = 3;
```

### Comparing `qulacs-0.6.3/test/cppsim/test_gate.cpp` & `qulacs-0.6.4/test/cppsim/test_gate.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_gate_dm.cpp` & `qulacs-0.6.4/test/cppsim/test_gate_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_gate_multicpu.cpp` & `qulacs-0.6.4/test/cppsim/test_gate_multicpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_hamiltonian.cpp` & `qulacs-0.6.4/test/cppsim/test_hamiltonian.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_hamiltonian_dm.cpp` & `qulacs-0.6.4/test/cppsim/test_hamiltonian_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_hamiltonian_multicpu.cpp` & `qulacs-0.6.4/test/cppsim/test_hamiltonian_multicpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_mpiutil_multicpu.cpp` & `qulacs-0.6.4/test/cppsim/test_mpiutil_multicpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_noise_dm.cpp` & `qulacs-0.6.4/test/cppsim/test_noise_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_noisesimulator.cpp` & `qulacs-0.6.4/test/cppsim/test_noisesimulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_noisyevolution.cpp` & `qulacs-0.6.4/test/cppsim/test_noisyevolution.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_pauli_operator.cpp` & `qulacs-0.6.4/test/cppsim/test_pauli_operator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_simulator.cpp` & `qulacs-0.6.4/test/cppsim/test_simulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_state.cpp` & `qulacs-0.6.4/test/cppsim/test_state.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_state_dm.cpp` & `qulacs-0.6.4/test/cppsim/test_state_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/cppsim/test_state_multicpu.cpp` & `qulacs-0.6.4/test/cppsim/test_state_multicpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/csim/test_memory.cpp` & `qulacs-0.6.4/test/csim/test_memory.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/csim/test_omputil.cpp` & `qulacs-0.6.4/test/csim/test_omputil.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/csim/test_stat.cpp` & `qulacs-0.6.4/test/csim/test_stat.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/csim/test_update_control.cpp` & `qulacs-0.6.4/test/csim/test_update_control.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/csim/test_update_dense.cpp` & `qulacs-0.6.4/test/csim/test_update_dense.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/csim/test_update_dense_double.cpp` & `qulacs-0.6.4/test/csim/test_update_dense_double.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/csim/test_update_diagonal.cpp` & `qulacs-0.6.4/test/csim/test_update_diagonal.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/csim/test_update_diagonal_multi.cpp` & `qulacs-0.6.4/test/csim/test_update_diagonal_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/csim/test_update_named.cpp` & `qulacs-0.6.4/test/csim/test_update_named.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/csim/test_update_pauli.cpp` & `qulacs-0.6.4/test/csim/test_update_pauli.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/gpusim/test_circuit.cpp` & `qulacs-0.6.4/test/gpusim/test_circuit.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/gpusim/test_compat_cpu.cpp` & `qulacs-0.6.4/test/gpusim/test_compat_cpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/gpusim/test_func_memory.cpp` & `qulacs-0.6.4/test/gpusim/test_func_memory.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/gpusim/test_gate.cpp` & `qulacs-0.6.4/test/gpusim/test_gate.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/gpusim/test_hamiltonian.cpp` & `qulacs-0.6.4/test/gpusim/test_hamiltonian.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/gpusim/test_state.cpp` & `qulacs-0.6.4/test/gpusim/test_state.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/gpusim/test_update_control.cpp` & `qulacs-0.6.4/test/gpusim/test_update_control.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/gpusim/test_update_dense.cpp` & `qulacs-0.6.4/test/gpusim/test_update_dense.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/gpusim/test_update_diagonal.cpp` & `qulacs-0.6.4/test/gpusim/test_update_diagonal.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/gpusim/test_update_named.cpp` & `qulacs-0.6.4/test/gpusim/test_update_named.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/gpusim/test_update_pauli.cpp` & `qulacs-0.6.4/test/gpusim/test_update_pauli.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/gpusim/test_util.hpp` & `qulacs-0.6.4/test/gpusim/test_util.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/util/util.hpp` & `qulacs-0.6.4/test/util/util.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -68,16 +68,16 @@
     return vec;
 }
 
 // expand matrix
 static Eigen::MatrixXcd kronecker_product(
     const Eigen::MatrixXcd& lhs, const Eigen::MatrixXcd& rhs) {
     Eigen::MatrixXcd result(lhs.rows() * rhs.rows(), lhs.cols() * rhs.cols());
-    for (int i = 0; i < lhs.cols(); i++) {
-        for (int j = 0; j < lhs.rows(); j++) {
+    for (int i = 0; i < lhs.rows(); i++) {
+        for (int j = 0; j < lhs.cols(); j++) {
             result.block(i * rhs.rows(), j * rhs.cols(), rhs.rows(),
                 rhs.cols()) = lhs(i, j) * rhs;
         }
     }
     return result;
 }
```

### Comparing `qulacs-0.6.3/test/vqcsim/test.cpp` & `qulacs-0.6.4/test/vqcsim/test.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.3/test/vqcsim/test_backprop.cpp` & `qulacs-0.6.4/test/vqcsim/test_backprop.cpp`

 * *Files identical despite different names*

