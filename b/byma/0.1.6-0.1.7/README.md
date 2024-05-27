# Comparing `tmp/byma-0.1.6.tar.gz` & `tmp/byma-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byma-0.1.6.tar", last modified: Fri Apr 26 06:00:23 2024, max compression
+gzip compressed data, was "byma-0.1.7.tar", last modified: Mon May 27 20:30:35 2024, max compression
```

## Comparing `byma-0.1.6.tar` & `byma-0.1.7.tar`

### file list

```diff
@@ -1,103 +1,107 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.794084 byma-0.1.6/
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-26 06:00:11.000000 byma-0.1.6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1616 2024-04-26 06:00:11.000000 byma-0.1.6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      522 2024-04-26 06:00:11.000000 byma-0.1.6/CHANGELOG.txt
--rwxrwxrwx   0 root         (0) root         (0)     1836 2024-04-26 06:00:11.000000 byma-0.1.6/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-26 06:00:11.000000 byma-0.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3433 2024-04-26 06:00:23.794084 byma-0.1.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2538 2024-04-26 06:00:11.000000 byma-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.783084 byma-0.1.6/byma/
--rw-rw-rw-   0 root         (0) root         (0)     1384 2024-04-26 06:00:11.000000 byma-0.1.6/byma/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-26 06:00:23.000000 byma-0.1.6/byma/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.784085 byma-0.1.6/byma/interface/
--rw-rw-rw-   0 root         (0) root         (0)     2612 2024-04-26 06:00:11.000000 byma-0.1.6/byma/interface/BaseInterface.py
--rw-rw-rw-   0 root         (0) root         (0)     3589 2024-04-26 06:00:11.000000 byma-0.1.6/byma/interface/NonlinearHeat.py
--rw-rw-rw-   0 root         (0) root         (0)    11496 2024-04-26 06:00:11.000000 byma-0.1.6/byma/interface/Time.py
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-26 06:00:11.000000 byma-0.1.6/byma/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.785085 byma-0.1.6/byma/iteral/
--rw-rw-rw-   0 root         (0) root         (0)      187 2024-04-26 06:00:11.000000 byma-0.1.6/byma/iteral/Iteral.py
--rw-rw-rw-   0 root         (0) root         (0)     5149 2024-04-26 06:00:11.000000 byma-0.1.6/byma/iteral/Newton.py
--rw-rw-rw-   0 root         (0) root         (0)     4872 2024-04-26 06:00:11.000000 byma-0.1.6/byma/iteral/OrthogonalSubspace.py
--rw-rw-rw-   0 root         (0) root         (0)      142 2024-04-26 06:00:11.000000 byma-0.1.6/byma/iteral/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.785085 byma-0.1.6/byma/iteral/stationary/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 06:00:11.000000 byma-0.1.6/byma/iteral/stationary/OrthogonalSubspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.786085 byma-0.1.6/byma/nuby/
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-26 06:00:11.000000 byma-0.1.6/byma/nuby/Bifurcation.py
--rw-rw-rw-   0 root         (0) root         (0)     7951 2024-04-26 06:00:11.000000 byma-0.1.6/byma/nuby/Continuation.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-26 06:00:11.000000 byma-0.1.6/byma/nuby/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2024-04-26 06:00:11.000000 byma-0.1.6/byma/nuby/_nuby.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.787084 byma-0.1.6/byma/numy/
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-26 06:00:11.000000 byma-0.1.6/byma/numy/Numy.py
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-26 06:00:11.000000 byma-0.1.6/byma/numy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-26 06:00:11.000000 byma-0.1.6/byma/numy/_numy.py
--rw-rw-rw-   0 root         (0) root         (0)     3576 2024-04-26 06:00:11.000000 byma-0.1.6/byma/numy/integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.787084 byma-0.1.6/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-26 06:00:11.000000 byma-0.1.6/byma/pyplot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6292 2024-04-26 06:00:11.000000 byma-0.1.6/byma/pyplot/plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.794084 byma-0.1.6/byma.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3433 2024-04-26 06:00:23.000000 byma-0.1.6/byma.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2012 2024-04-26 06:00:23.000000 byma-0.1.6/byma.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 06:00:23.000000 byma-0.1.6/byma.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-26 06:00:23.000000 byma-0.1.6/byma.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.788085 byma-0.1.6/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-26 06:00:11.000000 byma-0.1.6/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-26 06:00:11.000000 byma-0.1.6/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-26 06:00:11.000000 byma-0.1.6/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.788085 byma-0.1.6/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.789085 byma-0.1.6/docs/source/autoapi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.789085 byma-0.1.6/docs/source/autoapi/OrthogonalSubspace/
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/OrthogonalSubspace/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.789085 byma-0.1.6/docs/source/autoapi/byma/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.789085 byma-0.1.6/docs/source/autoapi/byma/_version/
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/_version/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      834 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.789085 byma-0.1.6/docs/source/autoapi/byma/interface/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.790084 byma-0.1.6/docs/source/autoapi/byma/interface/BaseInterface/
--rw-rw-rw-   0 root         (0) root         (0)     1551 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/interface/BaseInterface/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.790084 byma-0.1.6/docs/source/autoapi/byma/interface/NonlinearHeat/
--rw-rw-rw-   0 root         (0) root         (0)     2105 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.790084 byma-0.1.6/docs/source/autoapi/byma/interface/Time/
--rw-rw-rw-   0 root         (0) root         (0)     6246 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/interface/Time/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     9425 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/interface/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.790084 byma-0.1.6/docs/source/autoapi/byma/iteral/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.790084 byma-0.1.6/docs/source/autoapi/byma/iteral/Iteral/
--rw-rw-rw-   0 root         (0) root         (0)      289 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/iteral/Iteral/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.791084 byma-0.1.6/docs/source/autoapi/byma/iteral/Newton/
--rw-rw-rw-   0 root         (0) root         (0)     1912 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/iteral/Newton/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.791084 byma-0.1.6/docs/source/autoapi/byma/iteral/OrthogonalSubspace/
--rw-rw-rw-   0 root         (0) root         (0)     2111 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      405 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/iteral/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.791084 byma-0.1.6/docs/source/autoapi/byma/nuby/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.791084 byma-0.1.6/docs/source/autoapi/byma/nuby/Bifurcation/
--rw-rw-rw-   0 root         (0) root         (0)      301 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.791084 byma-0.1.6/docs/source/autoapi/byma/nuby/Continuation/
--rw-rw-rw-   0 root         (0) root         (0)     4607 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/nuby/Continuation/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.792084 byma-0.1.6/docs/source/autoapi/byma/nuby/_nuby/
--rw-rw-rw-   0 root         (0) root         (0)     4840 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/nuby/_nuby/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5112 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/nuby/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.792084 byma-0.1.6/docs/source/autoapi/byma/numy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.792084 byma-0.1.6/docs/source/autoapi/byma/numy/Numy/
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/numy/Numy/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.792084 byma-0.1.6/docs/source/autoapi/byma/numy/_numy/
--rw-rw-rw-   0 root         (0) root         (0)     1858 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/numy/_numy/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2116 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/numy/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.792084 byma-0.1.6/docs/source/autoapi/byma/numy/integration/
--rw-rw-rw-   0 root         (0) root         (0)     1620 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/numy/integration/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.793084 byma-0.1.6/docs/source/autoapi/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     3599 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/pyplot/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.793084 byma-0.1.6/docs/source/autoapi/byma/pyplot/plots/
--rw-rw-rw-   0 root         (0) root         (0)     3544 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/byma/pyplot/plots/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      278 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/autoapi/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3805 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2203 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.793084 byma-0.1.6/docs/source/user/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/user/Installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/user/index.rst
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/user/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-26 06:00:11.000000 byma-0.1.6/docs/source/user/whatisbyma.rst
--rwxrwxrwx   0 root         (0) root         (0)     1005 2024-04-26 06:00:11.000000 byma-0.1.6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-26 06:00:11.000000 byma-0.1.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 06:00:23.794084 byma-0.1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1021 2024-04-26 06:00:11.000000 byma-0.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:00:23.794084 byma-0.1.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 06:00:11.000000 byma-0.1.6/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.109779 byma-0.1.7/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-05-27 20:30:22.000000 byma-0.1.7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2024-05-27 20:30:22.000000 byma-0.1.7/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      623 2024-05-27 20:30:22.000000 byma-0.1.7/CHANGELOG.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1836 2024-05-27 20:30:22.000000 byma-0.1.7/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-27 20:30:22.000000 byma-0.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3433 2024-05-27 20:30:35.108778 byma-0.1.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2538 2024-05-27 20:30:22.000000 byma-0.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.094776 byma-0.1.7/byma/
+-rw-rw-rw-   0 root         (0) root         (0)     1384 2024-05-27 20:30:22.000000 byma-0.1.7/byma/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-05-27 20:30:34.000000 byma-0.1.7/byma/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.096776 byma-0.1.7/byma/interface/
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2024-05-27 20:30:22.000000 byma-0.1.7/byma/interface/BaseInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2024-05-27 20:30:22.000000 byma-0.1.7/byma/interface/NonlinearHeat.py
+-rw-rw-rw-   0 root         (0) root         (0)    11496 2024-05-27 20:30:22.000000 byma-0.1.7/byma/interface/Time.py
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-05-27 20:30:22.000000 byma-0.1.7/byma/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.097777 byma-0.1.7/byma/iteral/
+-rw-rw-rw-   0 root         (0) root         (0)     8604 2024-05-27 20:30:22.000000 byma-0.1.7/byma/iteral/GradientDescent.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2024-05-27 20:30:22.000000 byma-0.1.7/byma/iteral/Iteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     6420 2024-05-27 20:30:22.000000 byma-0.1.7/byma/iteral/NesterovMethod.py
+-rw-rw-rw-   0 root         (0) root         (0)     5149 2024-05-27 20:30:22.000000 byma-0.1.7/byma/iteral/Newton.py
+-rw-rw-rw-   0 root         (0) root         (0)     4832 2024-05-27 20:30:22.000000 byma-0.1.7/byma/iteral/OrthogonalSubspace.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2024-05-27 20:30:22.000000 byma-0.1.7/byma/iteral/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.098777 byma-0.1.7/byma/nuby/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-27 20:30:22.000000 byma-0.1.7/byma/nuby/Bifurcation.py
+-rw-rw-rw-   0 root         (0) root         (0)     7951 2024-05-27 20:30:22.000000 byma-0.1.7/byma/nuby/Continuation.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-05-27 20:30:22.000000 byma-0.1.7/byma/nuby/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-05-27 20:30:22.000000 byma-0.1.7/byma/nuby/_nuby.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.099777 byma-0.1.7/byma/numy/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-05-27 20:30:22.000000 byma-0.1.7/byma/numy/Numy.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-05-27 20:30:22.000000 byma-0.1.7/byma/numy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      167 2024-05-27 20:30:22.000000 byma-0.1.7/byma/numy/_numy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3576 2024-05-27 20:30:22.000000 byma-0.1.7/byma/numy/integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.100777 byma-0.1.7/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-27 20:30:22.000000 byma-0.1.7/byma/pyplot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6292 2024-05-27 20:30:22.000000 byma-0.1.7/byma/pyplot/plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.108778 byma-0.1.7/byma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3433 2024-05-27 20:30:35.000000 byma-0.1.7/byma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2143 2024-05-27 20:30:35.000000 byma-0.1.7/byma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 20:30:35.000000 byma-0.1.7/byma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-27 20:30:35.000000 byma-0.1.7/byma.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.100777 byma-0.1.7/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-05-27 20:30:22.000000 byma-0.1.7/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-27 20:30:22.000000 byma-0.1.7/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-27 20:30:22.000000 byma-0.1.7/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.101777 byma-0.1.7/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.101777 byma-0.1.7/docs/source/autoapi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.101777 byma-0.1.7/docs/source/autoapi/OrthogonalSubspace/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/OrthogonalSubspace/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.101777 byma-0.1.7/docs/source/autoapi/byma/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.102777 byma-0.1.7/docs/source/autoapi/byma/_version/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/_version/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      849 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.102777 byma-0.1.7/docs/source/autoapi/byma/interface/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.102777 byma-0.1.7/docs/source/autoapi/byma/interface/BaseInterface/
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/interface/BaseInterface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.102777 byma-0.1.7/docs/source/autoapi/byma/interface/NonlinearHeat/
+-rw-rw-rw-   0 root         (0) root         (0)     2086 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.103778 byma-0.1.7/docs/source/autoapi/byma/interface/Time/
+-rw-rw-rw-   0 root         (0) root         (0)     6226 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/interface/Time/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9459 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/interface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.103778 byma-0.1.7/docs/source/autoapi/byma/iteral/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.103778 byma-0.1.7/docs/source/autoapi/byma/iteral/GradientDescent/
+-rw-rw-rw-   0 root         (0) root         (0)     3809 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/iteral/GradientDescent/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.103778 byma-0.1.7/docs/source/autoapi/byma/iteral/Iteral/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/iteral/Iteral/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.104778 byma-0.1.7/docs/source/autoapi/byma/iteral/NesterovMethod/
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/iteral/NesterovMethod/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.104778 byma-0.1.7/docs/source/autoapi/byma/iteral/Newton/
+-rw-rw-rw-   0 root         (0) root         (0)     3365 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/iteral/Newton/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.104778 byma-0.1.7/docs/source/autoapi/byma/iteral/OrthogonalSubspace/
+-rw-rw-rw-   0 root         (0) root         (0)     3588 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      509 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/iteral/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.104778 byma-0.1.7/docs/source/autoapi/byma/nuby/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.105778 byma-0.1.7/docs/source/autoapi/byma/nuby/Bifurcation/
+-rw-rw-rw-   0 root         (0) root         (0)      278 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.105778 byma-0.1.7/docs/source/autoapi/byma/nuby/Continuation/
+-rw-rw-rw-   0 root         (0) root         (0)     7798 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/nuby/Continuation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.105778 byma-0.1.7/docs/source/autoapi/byma/nuby/_nuby/
+-rw-rw-rw-   0 root         (0) root         (0)     4840 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/nuby/_nuby/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5104 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/nuby/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.105778 byma-0.1.7/docs/source/autoapi/byma/numy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.105778 byma-0.1.7/docs/source/autoapi/byma/numy/Numy/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/numy/Numy/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.106778 byma-0.1.7/docs/source/autoapi/byma/numy/_numy/
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/numy/_numy/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2108 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/numy/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.106778 byma-0.1.7/docs/source/autoapi/byma/numy/integration/
+-rw-rw-rw-   0 root         (0) root         (0)     4818 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/numy/integration/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.106778 byma-0.1.7/docs/source/autoapi/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     3579 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/pyplot/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.106778 byma-0.1.7/docs/source/autoapi/byma/pyplot/plots/
+-rw-rw-rw-   0 root         (0) root         (0)     3522 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/byma/pyplot/plots/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/autoapi/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3805 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.107778 byma-0.1.7/docs/source/user/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/user/Installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/user/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/user/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-27 20:30:22.000000 byma-0.1.7/docs/source/user/whatisbyma.rst
+-rwxrwxrwx   0 root         (0) root         (0)     1005 2024-05-27 20:30:22.000000 byma-0.1.7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-27 20:30:22.000000 byma-0.1.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 20:30:35.109779 byma-0.1.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2024-05-27 20:30:22.000000 byma-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 20:30:35.108778 byma-0.1.7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 20:30:22.000000 byma-0.1.7/tests/__init__.py
```

### Comparing `byma-0.1.6/.gitlab-ci.yml` & `byma-0.1.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/CHANGELOG.txt` & `byma-0.1.7/CHANGELOG.txt`

 * *Files 18% similar despite different names*

```diff
@@ -20,7 +20,13 @@
     - Fully Initialize auto-documentation 
 
 0.1.3 (10/04/2024)
 -------------------
 - Patch: Reoganization interal method
 - Major: 
     - New sub-package numy
+
+0.1.7 (10/04/2024)
+-------------------
+- Major: 
+    - Nesterov Method
+    - GradientDescent Method
```

### Comparing `byma-0.1.6/LICENSE.md` & `byma-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/PKG-INFO` & `byma-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
 Project-URL: documentation, https://bytemath.gitlab.io/python/ByMa/index.html
 Project-URL: source, https://gitlab.com/ByteMath/python/ByMa
 Project-URL: download, https://pypi.org/project/byma/#files
```

### Comparing `byma-0.1.6/README.md` & `byma-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/byma/__init__.py` & `byma-0.1.7/byma/__init__.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/byma/interface/BaseInterface.py` & `byma-0.1.7/byma/interface/BaseInterface.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/byma/interface/NonlinearHeat.py` & `byma-0.1.7/byma/interface/NonlinearHeat.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/byma/interface/Time.py` & `byma-0.1.7/byma/interface/Time.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/byma/iteral/Newton.py` & `byma-0.1.7/byma/iteral/Newton.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/byma/iteral/OrthogonalSubspace.py` & `byma-0.1.7/byma/iteral/OrthogonalSubspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-from scipy.linalg import lu, inv, solve
 from scipy.sparse import csc_matrix
 from scipy.sparse.linalg import splu
 from numpy.linalg import qr
 from ..interface.BaseInterface import BaseInterface as bs
 from .Iteral import Iteral as Int
 import scipy.sparse as sp
```

### Comparing `byma-0.1.6/byma/nuby/Continuation.py` & `byma-0.1.7/byma/nuby/Continuation.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/byma/numy/integration.py` & `byma-0.1.7/byma/numy/integration.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/byma/pyplot/plots.py` & `byma-0.1.7/byma/pyplot/plots.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/byma.egg-info/PKG-INFO` & `byma-0.1.7/byma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
 Project-URL: documentation, https://bytemath.gitlab.io/python/ByMa/index.html
 Project-URL: source, https://gitlab.com/ByteMath/python/ByMa
 Project-URL: download, https://pypi.org/project/byma/#files
```

### Comparing `byma-0.1.6/byma.egg-info/SOURCES.txt` & `byma-0.1.7/byma.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 byma.egg-info/SOURCES.txt
 byma.egg-info/dependency_links.txt
 byma.egg-info/top_level.txt
 byma/interface/BaseInterface.py
 byma/interface/NonlinearHeat.py
 byma/interface/Time.py
 byma/interface/__init__.py
+byma/iteral/GradientDescent.py
 byma/iteral/Iteral.py
+byma/iteral/NesterovMethod.py
 byma/iteral/Newton.py
 byma/iteral/OrthogonalSubspace.py
 byma/iteral/__init__.py
-byma/iteral/stationary/OrthogonalSubspace.py
 byma/nuby/Bifurcation.py
 byma/nuby/Continuation.py
 byma/nuby/__init__.py
 byma/nuby/_nuby.py
 byma/numy/Numy.py
 byma/numy/__init__.py
 byma/numy/_numy.py
@@ -42,15 +43,17 @@
 docs/source/autoapi/byma/index.rst
 docs/source/autoapi/byma/_version/index.rst
 docs/source/autoapi/byma/interface/index.rst
 docs/source/autoapi/byma/interface/BaseInterface/index.rst
 docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
 docs/source/autoapi/byma/interface/Time/index.rst
 docs/source/autoapi/byma/iteral/index.rst
+docs/source/autoapi/byma/iteral/GradientDescent/index.rst
 docs/source/autoapi/byma/iteral/Iteral/index.rst
+docs/source/autoapi/byma/iteral/NesterovMethod/index.rst
 docs/source/autoapi/byma/iteral/Newton/index.rst
 docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst
 docs/source/autoapi/byma/nuby/index.rst
 docs/source/autoapi/byma/nuby/Bifurcation/index.rst
 docs/source/autoapi/byma/nuby/Continuation/index.rst
 docs/source/autoapi/byma/nuby/_nuby/index.rst
 docs/source/autoapi/byma/numy/index.rst
```

### Comparing `byma-0.1.6/docs/Makefile` & `byma-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/docs/make.bat` & `byma-0.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/docs/source/autoapi/byma/index.rst` & `byma-0.1.7/docs/source/autoapi/byma/index.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-:py:mod:`byma`
-==============
+byma
+====
 
 .. py:module:: byma
 
 .. autoapi-nested-parse::
 
    ByMa: A scientific computing package for Python
    ================================================
@@ -23,18 +23,18 @@
     interface                    --- Interface functions
     numy                         --- Basic Numerical Methods functions
 
 
 
 Subpackages
 -----------
+
 .. toctree::
-   :titlesonly:
-   :maxdepth: 3
+   :maxdepth: 1
 
-   interface/index.rst
-   iteral/index.rst
-   nuby/index.rst
-   numy/index.rst
-   pyplot/index.rst
+   /autoapi/byma/interface/index
+   /autoapi/byma/iteral/index
+   /autoapi/byma/nuby/index
+   /autoapi/byma/numy/index
+   /autoapi/byma/pyplot/index
```

### Comparing `byma-0.1.6/docs/source/autoapi/byma/interface/BaseInterface/index.rst` & `byma-0.1.7/docs/source/autoapi/byma/interface/BaseInterface/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-:py:mod:`byma.interface.BaseInterface`
-======================================
+byma.interface.BaseInterface
+============================
 
 .. py:module:: byma.interface.BaseInterface
 
 
-Module Contents
----------------
-
 Classes
-~~~~~~~
+-------
 
 .. autoapisummary::
 
    byma.interface.BaseInterface.BaseInterface
 
 
-
+Module Contents
+---------------
 
 .. py:class:: BaseInterface(default_cls, default_opts, **kwargs)
 
-
    Defines a base interface
 
+
    .. py:method:: set_defaults(default_cls, default_opts={})
       :staticmethod:
 
+
       Decorator for setting default interface and parameters.
 
       Parameters
       ----------
       default_cls : obj
           The default class instance.
       default_opts : dict, optional
@@ -36,30 +35,33 @@
 
       Returns
       -------
       callable
           A decorator function that sets default interface and parameters.
 
 
+
    .. py:method:: opts(**kwargs)
       :staticmethod:
 
+
       Method for setting options for the interface.
 
       Parameters
       ----------
       kwargs : dict
           Additional keyword arguments.
 
       Returns
       -------
       dict
           A dictionary containing updated interface and parameters.
 
 
+
    .. py:method:: check_none()
 
       Check if any of the arguments are None.
 
       Parameters
       ----------
       *args : tuple
```

### Comparing `byma-0.1.6/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst` & `byma-0.1.7/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-:py:mod:`byma.interface.NonlinearHeat`
-======================================
+byma.interface.NonlinearHeat
+============================
 
 .. py:module:: byma.interface.NonlinearHeat
 
 
-Module Contents
----------------
-
 Classes
-~~~~~~~
+-------
 
 .. autoapisummary::
 
    byma.interface.NonlinearHeat.NonlinearHeat
 
 
-
+Module Contents
+---------------
 
 .. py:class:: NonlinearHeat
 
-
    Damped stationary heat equation with discretization using finite difference method.
 
    The equation is given by:
 
    .. math::
        u_{xx} + \mu(u - \frac{1}{3}u^3)   x \in [0,1]
        u(0) = 1, u(1) = 0
@@ -38,14 +35,15 @@
 
    - `GL1(x, mu)`: Checks if x is a zero of the right-hand side.
    - `fGL1(u, n, mu)`: Computes the resulting sparse matrix.
    - `linGL1(n)`: Computes a 1d float vector for the linearized version.
    - `JacGL1(u, n, mu)`: Computes the Jacobian matrix.
 
 
+
    .. py:method:: GL1(x, mu)
 
       Computes the finite difference method for the damped stationary heat equation.
 
       Parameters
       ----------
       x : numpy.ndarray
@@ -56,14 +54,15 @@
       Returns
       -------
       numpy.ndarray
           Result of the computation.
 
 
 
+
    .. py:method:: fGL1(**kwargs)
 
       Computes the resulting sparse matrix for the damped stationary heat equation.
 
       Parameters
       ----------
       **kwargs : dict
@@ -72,14 +71,15 @@
       Returns
       -------
       numpy.ndarray
           Resulting sparse matrix.
 
 
 
+
    .. py:method:: linGL1(n, **kwargs)
 
       Computes a 1D float vector for the linearized version of the heat equation.
 
       Parameters
       ----------
       n : int
@@ -88,14 +88,15 @@
       Returns
       -------
       numpy.ndarray
           1D float vector.
 
 
 
+
    .. py:method:: JacGL1(**kwargs)
 
       Computes the Jacobian matrix for the damped stationary heat equation.
 
       Parameters
       ----------
       **kwargs : dict
```

### Comparing `byma-0.1.6/docs/source/autoapi/byma/interface/Time/index.rst` & `byma-0.1.7/docs/source/autoapi/byma/interface/Time/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-:py:mod:`byma.interface.Time`
-=============================
+byma.interface.Time
+===================
 
 .. py:module:: byma.interface.Time
 
 .. autoapi-nested-parse::
 
    Time Module
    ===========
@@ -59,60 +59,59 @@
    Acknowledgement
    ===================
 
    This module has been made by taking inspiration and multiple parts of the code from the `timebudget` package.
 
 
 
-Module Contents
----------------
-
 Classes
-~~~~~~~
+-------
 
 .. autoapisummary::
 
    byma.interface.Time.TimeRecorder
 
 
-
 Functions
-~~~~~~~~~
+---------
 
 .. autoapisummary::
 
    byma.interface.Time.annotate
    byma.interface.Time.time
    byma.interface.Time.set_quiet
    byma.interface.Time.read_data
 
 
+Module Contents
+---------------
 
 .. py:class:: TimeRecorder(quiet_mode: bool = False)
 
-
    .. py:method:: reset()
 
       Clear all recorded time statistics.
 
 
+
    .. py:method:: start(block_name: str)
 
       Record the start time of a code block.
 
       Parameters:
       -----------
       block_name : str
           Name of the code block.
           
       Examples:
       ---------
       >>> recorder.start("my_block")
 
 
+
    .. py:method:: end(block_name: str, quiet: Optional[bool] = None) -> float
 
       Record the end time of a code block and calculate the elapsed time.
 
       Parameters:
       -----------
       block_name : str
@@ -126,14 +125,15 @@
           Elapsed time in milliseconds.
           
       Examples:
       ---------
       >>> elapsed_time = recorder.end("my_block")
 
 
+
    .. py:method:: report(percent_of: str = None, reset: bool = False)
 
       Generate and print a report of recorded time statistics.
 
       Parameters:
       -----------
       percent_of : str, optional
```

### Comparing `byma-0.1.6/docs/source/autoapi/byma/interface/index.rst` & `byma-0.1.7/docs/source/autoapi/byma/interface/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,67 +1,66 @@
-:py:mod:`byma.interface`
-========================
+byma.interface
+==============
 
 .. py:module:: byma.interface
 
 .. autoapi-nested-parse::
 
    BaseInterface Module
    ====================
 
    This module provides a base interface for defining default classes and options. It includes functionality for setting default parameters, updating interface options, and retrieving updated options.
 
 
 
 Submodules
 ----------
+
 .. toctree::
-   :titlesonly:
    :maxdepth: 1
 
-   BaseInterface/index.rst
-   NonlinearHeat/index.rst
-   Time/index.rst
-
+   /autoapi/byma/interface/BaseInterface/index
+   /autoapi/byma/interface/NonlinearHeat/index
+   /autoapi/byma/interface/Time/index
 
-Package Contents
-----------------
 
 Classes
-~~~~~~~
+-------
 
 .. autoapisummary::
 
    byma.interface.BaseInterface
    byma.interface.NonlinearHeat
    byma.interface.TimeRecorder
    byma.interface.TimeRecorder
 
 
-
 Functions
-~~~~~~~~~
+---------
 
 .. autoapisummary::
 
    byma.interface.annotate
    byma.interface.time
    byma.interface.set_quiet
    byma.interface.read_data
 
 
+Package Contents
+----------------
 
 .. py:class:: BaseInterface(default_cls, default_opts, **kwargs)
 
-
    Defines a base interface
 
+
    .. py:method:: set_defaults(default_cls, default_opts={})
       :staticmethod:
 
+
       Decorator for setting default interface and parameters.
 
       Parameters
       ----------
       default_cls : obj
           The default class instance.
       default_opts : dict, optional
@@ -69,30 +68,33 @@
 
       Returns
       -------
       callable
           A decorator function that sets default interface and parameters.
 
 
+
    .. py:method:: opts(**kwargs)
       :staticmethod:
 
+
       Method for setting options for the interface.
 
       Parameters
       ----------
       kwargs : dict
           Additional keyword arguments.
 
       Returns
       -------
       dict
           A dictionary containing updated interface and parameters.
 
 
+
    .. py:method:: check_none()
 
       Check if any of the arguments are None.
 
       Parameters
       ----------
       *args : tuple
@@ -110,15 +112,14 @@
 
 
 
 
 
 .. py:class:: NonlinearHeat
 
-
    Damped stationary heat equation with discretization using finite difference method.
 
    The equation is given by:
 
    .. math::
        u_{xx} + \mu(u - \frac{1}{3}u^3)   x \in [0,1]
        u(0) = 1, u(1) = 0
@@ -133,14 +134,15 @@
 
    - `GL1(x, mu)`: Checks if x is a zero of the right-hand side.
    - `fGL1(u, n, mu)`: Computes the resulting sparse matrix.
    - `linGL1(n)`: Computes a 1d float vector for the linearized version.
    - `JacGL1(u, n, mu)`: Computes the Jacobian matrix.
 
 
+
    .. py:method:: GL1(x, mu)
 
       Computes the finite difference method for the damped stationary heat equation.
 
       Parameters
       ----------
       x : numpy.ndarray
@@ -151,14 +153,15 @@
       Returns
       -------
       numpy.ndarray
           Result of the computation.
 
 
 
+
    .. py:method:: fGL1(**kwargs)
 
       Computes the resulting sparse matrix for the damped stationary heat equation.
 
       Parameters
       ----------
       **kwargs : dict
@@ -167,14 +170,15 @@
       Returns
       -------
       numpy.ndarray
           Resulting sparse matrix.
 
 
 
+
    .. py:method:: linGL1(n, **kwargs)
 
       Computes a 1D float vector for the linearized version of the heat equation.
 
       Parameters
       ----------
       n : int
@@ -183,14 +187,15 @@
       Returns
       -------
       numpy.ndarray
           1D float vector.
 
 
 
+
    .. py:method:: JacGL1(**kwargs)
 
       Computes the Jacobian matrix for the damped stationary heat equation.
 
       Parameters
       ----------
       **kwargs : dict
@@ -202,34 +207,35 @@
           Jacobian matrix.
 
 
 
 
 .. py:class:: TimeRecorder(quiet_mode: bool = False)
 
-
    .. py:method:: reset()
 
       Clear all recorded time statistics.
 
 
+
    .. py:method:: start(block_name: str)
 
       Record the start time of a code block.
 
       Parameters:
       -----------
       block_name : str
           Name of the code block.
           
       Examples:
       ---------
       >>> recorder.start("my_block")
 
 
+
    .. py:method:: end(block_name: str, quiet: Optional[bool] = None) -> float
 
       Record the end time of a code block and calculate the elapsed time.
 
       Parameters:
       -----------
       block_name : str
@@ -243,14 +249,15 @@
           Elapsed time in milliseconds.
           
       Examples:
       ---------
       >>> elapsed_time = recorder.end("my_block")
 
 
+
    .. py:method:: report(percent_of: str = None, reset: bool = False)
 
       Generate and print a report of recorded time statistics.
 
       Parameters:
       -----------
       percent_of : str, optional
@@ -350,34 +357,35 @@
    Examples:
    ---------
    >>> data = read_data('timings.h5', ['Block1'])
 
 
 .. py:class:: TimeRecorder(quiet_mode: bool = False)
 
-
    .. py:method:: reset()
 
       Clear all recorded time statistics.
 
 
+
    .. py:method:: start(block_name: str)
 
       Record the start time of a code block.
 
       Parameters:
       -----------
       block_name : str
           Name of the code block.
           
       Examples:
       ---------
       >>> recorder.start("my_block")
 
 
+
    .. py:method:: end(block_name: str, quiet: Optional[bool] = None) -> float
 
       Record the end time of a code block and calculate the elapsed time.
 
       Parameters:
       -----------
       block_name : str
@@ -391,14 +399,15 @@
           Elapsed time in milliseconds.
           
       Examples:
       ---------
       >>> elapsed_time = recorder.end("my_block")
 
 
+
    .. py:method:: report(percent_of: str = None, reset: bool = False)
 
       Generate and print a report of recorded time statistics.
 
       Parameters:
       -----------
       percent_of : str, optional
```

### Comparing `byma-0.1.6/docs/source/autoapi/byma/iteral/Newton/index.rst` & `byma-0.1.7/docs/source/autoapi/byma/iteral/Newton/index.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,103 @@
-:py:mod:`byma.iteral.Newton`
-============================
+byma.iteral.Newton
+==================
 
 .. py:module:: byma.iteral.Newton
 
 
-Module Contents
----------------
+Classes
+-------
+
+.. autoapisummary::
+
+   byma.iteral.Newton.bs
+   byma.iteral.Newton.Int
 
 
 Functions
-~~~~~~~~~
+---------
 
 .. autoapisummary::
 
    byma.iteral.Newton.newton
 
 
+Module Contents
+---------------
+
+.. py:class:: bs(default_cls, default_opts, **kwargs)
+
+   Defines a base interface
+
+
+   .. py:method:: set_defaults(default_cls, default_opts={})
+      :staticmethod:
+
+
+      Decorator for setting default interface and parameters.
+
+      Parameters
+      ----------
+      default_cls : obj
+          The default class instance.
+      default_opts : dict, optional
+          Default options for the interface (default is an empty dictionary).
+
+      Returns
+      -------
+      callable
+          A decorator function that sets default interface and parameters.
+
+
+
+   .. py:method:: opts(**kwargs)
+      :staticmethod:
+
+
+      Method for setting options for the interface.
+
+      Parameters
+      ----------
+      kwargs : dict
+          Additional keyword arguments.
+
+      Returns
+      -------
+      dict
+          A dictionary containing updated interface and parameters.
+
+
+
+   .. py:method:: check_none()
+
+      Check if any of the arguments are None.
+
+      Parameters
+      ----------
+      *args : tuple
+          Arbitrary number of arguments to check.
+
+      Returns
+      -------
+      bool
+          True if any argument is None, False otherwise.
+
+      Raises
+      ------
+      ValueError
+          If any argument is None, raises ValueError with the names of the None arguments.
+
+
+
+
+
+.. py:class:: Int
+
+   Defines default options for the Iterative methods sub-package
+
 
 .. py:function:: newton(x, f, df, **kwargs)
 
    Perform Newton iterations to find the root of a given function.
 
    Parameters
    ----------
```

### Comparing `byma-0.1.6/docs/source/autoapi/byma/nuby/Continuation/index.rst` & `byma-0.1.7/docs/source/autoapi/byma/nuby/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,65 @@
-:py:mod:`byma.nuby.Continuation`
-================================
+byma.nuby
+=========
 
-.. py:module:: byma.nuby.Continuation
+.. py:module:: byma.nuby
 
+.. autoapi-nested-parse::
 
-Module Contents
----------------
+   ``byma.nuby``
+   ================
+
+   The ByMa numerical bifurcation functions rely on 
+
+   Functions present in byma.nuby are listed below.
+
+
+   Continuation
+   --------------------------
+
+      step
+      cont
+      
+
+   Exceptions
+   ----------
+
+      NuByError
+
+
+
+Submodules
+----------
+
+.. toctree::
+   :maxdepth: 1
+
+   /autoapi/byma/nuby/Bifurcation/index
+   /autoapi/byma/nuby/Continuation/index
+
+
+Classes
+-------
+
+.. autoapisummary::
+
+   byma.nuby.Bifurcation
 
 
 Functions
-~~~~~~~~~
+---------
 
 .. autoapisummary::
 
-   byma.nuby.Continuation.step
-   byma.nuby.Continuation.cont
+   byma.nuby.step
+   byma.nuby.cont
 
 
+Package Contents
+----------------
 
 .. py:function:: step(x, f, df, dfmu, dx, dmu, **kwargs)
 
    Perform one step of the continuation.
 
    :param x: array_like
        Current state.
@@ -102,7 +141,12 @@
        >>> # Perform continuation from start value to target value
        >>> start = 0.0
        >>> target = 1.0
        >>> result = cont(x0, dx0, start, df, dfmu, target=target, maxit_con=1000, method='normal', mode='full')
        >>> print(result)
 
 
+.. py:class:: Bifurcation
+
+   Defines default options for the Bifurcation package
+
+
```

### Comparing `byma-0.1.6/docs/source/autoapi/byma/nuby/_nuby/index.rst` & `byma-0.1.7/docs/source/autoapi/byma/nuby/_nuby/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/docs/source/autoapi/byma/numy/_numy/index.rst` & `byma-0.1.7/docs/source/autoapi/byma/numy/_numy/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/docs/source/autoapi/byma/numy/index.rst` & `byma-0.1.7/docs/source/autoapi/byma/numy/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-:py:mod:`byma.numy`
-===================
+byma.numy
+=========
 
 .. py:module:: byma.numy
 
 .. autoapi-nested-parse::
 
    ``byma.numy``
    ================
@@ -24,46 +24,43 @@
 
       NuMyError
 
 
 
 Submodules
 ----------
+
 .. toctree::
-   :titlesonly:
    :maxdepth: 1
 
-   Numy/index.rst
-   integration/index.rst
-
+   /autoapi/byma/numy/Numy/index
+   /autoapi/byma/numy/integration/index
 
-Package Contents
-----------------
 
 Classes
-~~~~~~~
+-------
 
 .. autoapisummary::
 
    byma.numy.Numy
 
 
-
 Functions
-~~~~~~~~~
+---------
 
 .. autoapisummary::
 
    byma.numy.euler
 
 
+Package Contents
+----------------
 
 .. py:class:: Numy
 
-
    Defines default options for the numerical methods sub-package
 
 
 .. py:function:: euler(start=0, T=1, dt=0.01, x0=None, f=None, df=None, **kwargs)
 
    Euler integration method.
```

### Comparing `byma-0.1.6/docs/source/autoapi/byma/pyplot/index.rst` & `byma-0.1.7/docs/source/autoapi/byma/pyplot/plots/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,25 @@
-:py:mod:`byma.pyplot`
-=====================
+byma.pyplot.plots
+=================
 
-.. py:module:: byma.pyplot
-
-
-Submodules
-----------
-.. toctree::
-   :titlesonly:
-   :maxdepth: 1
-
-   plots/index.rst
-
-
-Package Contents
-----------------
+.. py:module:: byma.pyplot.plots
 
 
 Functions
-~~~~~~~~~
+---------
 
 .. autoapisummary::
 
-   byma.pyplot.plot_scale
-   byma.pyplot.plot
-   byma.pyplot.plot_numerical_error
+   byma.pyplot.plots.plot_scale
+   byma.pyplot.plots.plot
+   byma.pyplot.plots.plot_numerical_error
 
 
+Module Contents
+---------------
 
 .. py:function:: plot_scale(x, y, label, scale, style={})
 
    Plot data with specified scale and style.
 
    Parameters
    ================
```

### Comparing `byma-0.1.6/docs/source/autoapi/byma/pyplot/plots/index.rst` & `byma-0.1.7/docs/source/autoapi/byma/pyplot/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,34 @@
-:py:mod:`byma.pyplot.plots`
-===========================
+byma.pyplot
+===========
 
-.. py:module:: byma.pyplot.plots
+.. py:module:: byma.pyplot
 
 
-Module Contents
----------------
+Submodules
+----------
+
+.. toctree::
+   :maxdepth: 1
+
+   /autoapi/byma/pyplot/plots/index
 
 
 Functions
-~~~~~~~~~
+---------
 
 .. autoapisummary::
 
-   byma.pyplot.plots.plot_scale
-   byma.pyplot.plots.plot
-   byma.pyplot.plots.plot_numerical_error
+   byma.pyplot.plot_scale
+   byma.pyplot.plot
+   byma.pyplot.plot_numerical_error
 
 
+Package Contents
+----------------
 
 .. py:function:: plot_scale(x, y, label, scale, style={})
 
    Plot data with specified scale and style.
 
    Parameters
    ================
```

### Comparing `byma-0.1.6/docs/source/conf.py` & `byma-0.1.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/docs/source/index.rst` & `byma-0.1.7/docs/source/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 
 
 .. toctree::
    :maxdepth: 5
    :hidden:
 
    User Guide <user/index>
-   API reference <reference/index>
-   Building from source <building/index>
-   release
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
@@ -32,15 +29,14 @@
 `Source Repository <https://gitlab.com/ByteMath/python/ByMa>`_ |
 `Issue Tracker <https://gitlab.com/ByteMath/python/ByMa/-/issues>`_ |
 
 
 .. grid:: 2
 
     .. grid-item-card::
-        :img-top: ../source/_static/index-images/getting_started.svg
 
         Getting started
         ^^^^^^^^^^^^^^^
 
         New to ByMa? Check out the Absolute Beginner's Guide. It contains an
         introduction to ByMa's main concepts and links to additional tutorials.
 
@@ -50,15 +46,14 @@
             :expand:
             :color: secondary
             :click-parent:
 
             To the absolute beginner's guide
 
     .. grid-item-card::
-        :img-top: ../source/_static/index-images/user_guide.svg
 
         User guide
         ^^^^^^^^^^
 
         The user guide provides in-depth information on the
         key concepts of ByMa with useful background information and explanation.
 
@@ -68,15 +63,14 @@
             :expand:
             :color: secondary
             :click-parent:
 
             To the user guide
 
     .. grid-item-card::
-        :img-top: ../source/_static/index-images/api.svg
 
         API reference
         ^^^^^^^^^^^^^
 
         The reference guide contains a detailed description of the functions,
         modules, and objects included in ByMa. The reference describes how the
         methods work and which parameters can be used. It assumes that you have an
```

### Comparing `byma-0.1.6/pyproject.toml` & `byma-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `byma-0.1.6/setup.py` & `byma-0.1.7/setup.py`

 * *Files identical despite different names*

