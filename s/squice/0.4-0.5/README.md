# Comparing `tmp/squice-0.4.tar.gz` & `tmp/squice-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squice-0.4.tar", last modified: Sun May 26 10:27:53 2024, max compression
+gzip compressed data, was "squice-0.5.tar", last modified: Mon May 27 17:25:22 2024, max compression
```

## Comparing `squice-0.4.tar` & `squice-0.5.tar`

### file list

```diff
@@ -1,65 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.611633 squice-0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.599633 squice-0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.603633 squice-0.4/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-26 10:27:47.000000 squice-0.4/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.607633 squice-0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-26 10:27:47.000000 squice-0.4/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-26 10:27:47.000000 squice-0.4/.github/workflows/lint_style.yml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-26 10:27:47.000000 squice-0.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-26 10:27:47.000000 squice-0.4/.github/workflows/pydoctor.yml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-26 10:27:47.000000 squice-0.4/.github/workflows/pytest_app.yml
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-26 10:27:47.000000 squice-0.4/.github/workflows/pytest_lib.yml
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-26 10:27:47.000000 squice-0.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-26 10:27:47.000000 squice-0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-26 10:27:47.000000 squice-0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-26 10:27:47.000000 squice-0.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-26 10:27:47.000000 squice-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-26 10:27:53.611633 squice-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-26 10:27:47.000000 squice-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.607633 squice-0.4/app/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-26 10:27:47.000000 squice-0.4/app/home.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.607633 squice-0.4/app/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-26 10:27:47.000000 squice-0.4/app/pages/2_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-26 10:27:47.000000 squice-0.4/app/pages/3_use_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-26 10:27:47.000000 squice-0.4/app/pages/4_about.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.607633 squice-0.4/app/static/
--rw-r--r--   0 runner    (1001) docker     (127)   183520 2024-05-26 10:27:47.000000 squice-0.4/app/static/squice.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.603633 squice-0.4/app/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.607633 squice-0.4/app/tests/use_cases/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-26 10:27:47.000000 squice-0.4/app/tests/use_cases/test_add_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-26 10:27:47.000000 squice-0.4/citation.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-26 10:27:47.000000 squice-0.4/dev.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.607633 squice-0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-26 10:27:47.000000 squice-0.4/docs/docs.md
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-26 10:27:47.000000 squice-0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-26 10:27:47.000000 squice-0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-26 10:27:47.000000 squice-0.4/requirements_lib.txt
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-26 10:27:53.611633 squice-0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.607633 squice-0.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-26 10:27:47.000000 squice-0.4/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.607633 squice-0.4/src/squice/
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-26 10:27:47.000000 squice-0.4/src/squice/DataLoaders.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:47.000000 squice-0.4/src/squice/ModulePredict.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-26 10:27:47.000000 squice-0.4/src/squice/MtxDisplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-26 10:27:47.000000 squice-0.4/src/squice/MtxInterpolator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:47.000000 squice-0.4/src/squice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.611633 squice-0.4/src/squice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-26 10:27:53.000000 squice-0.4/src/squice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-26 10:27:53.000000 squice-0.4/src/squice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 10:27:53.000000 squice-0.4/src/squice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 10:27:53.000000 squice-0.4/src/squice.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.607633 squice-0.4/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:47.000000 squice-0.4/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.607633 squice-0.4/src/tests/speed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:47.000000 squice-0.4/src/tests/speed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.607633 squice-0.4/src/tests/speed/data/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-26 10:27:47.000000 squice-0.4/src/tests/speed/data/speed_data.npy
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-26 10:27:47.000000 squice-0.4/src/tests/speed/data/speed_log.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-26 10:27:47.000000 squice-0.4/src/tests/speed/help_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-26 10:27:47.000000 squice-0.4/src/tests/speed/test_dataloaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.607633 squice-0.4/src/tests/utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:47.000000 squice-0.4/src/tests/utility/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:27:53.611633 squice-0.4/src/tests/utility/data/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-26 10:27:47.000000 squice-0.4/src/tests/utility/data/data1.npy
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-26 10:27:47.000000 squice-0.4/src/tests/utility/data/data3d.npy
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-26 10:27:47.000000 squice-0.4/src/tests/utility/test_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.317177 squice-0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.305177 squice-0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.309177 squice-0.5/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-27 17:25:16.000000 squice-0.5/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.309177 squice-0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-27 17:25:16.000000 squice-0.5/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-27 17:25:16.000000 squice-0.5/.github/workflows/lint_style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-27 17:25:16.000000 squice-0.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-27 17:25:16.000000 squice-0.5/.github/workflows/pydoctor.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-27 17:25:16.000000 squice-0.5/.github/workflows/pytest_app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-27 17:25:16.000000 squice-0.5/.github/workflows/pytest_lib.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-27 17:25:16.000000 squice-0.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-27 17:25:16.000000 squice-0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-27 17:25:16.000000 squice-0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-27 17:25:16.000000 squice-0.5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-27 17:25:16.000000 squice-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-27 17:25:22.317177 squice-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-27 17:25:16.000000 squice-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.309177 squice-0.5/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-27 17:25:16.000000 squice-0.5/app/home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.309177 squice-0.5/app/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-05-27 17:25:16.000000 squice-0.5/app/pages/2_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-27 17:25:16.000000 squice-0.5/app/pages/4_about.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.309177 squice-0.5/app/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   183520 2024-05-27 17:25:16.000000 squice-0.5/app/static/squice.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.305177 squice-0.5/app/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.313177 squice-0.5/app/tests/use_cases/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 17:25:16.000000 squice-0.5/app/tests/use_cases/test_add_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-27 17:25:16.000000 squice-0.5/citation.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-27 17:25:16.000000 squice-0.5/dev.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.313177 squice-0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-27 17:25:16.000000 squice-0.5/docs/docs.md
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-27 17:25:16.000000 squice-0.5/matrix (1).npy
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-27 17:25:16.000000 squice-0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-27 17:25:16.000000 squice-0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-27 17:25:16.000000 squice-0.5/requirements_lib.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-27 17:25:22.317177 squice-0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.313177 squice-0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 17:25:16.000000 squice-0.5/src/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:16.000000 squice-0.5/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.313177 squice-0.5/src/squice/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-27 17:25:16.000000 squice-0.5/src/squice/BinaryFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-27 17:25:16.000000 squice-0.5/src/squice/DataLoaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-27 17:25:16.000000 squice-0.5/src/squice/GridMaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-27 17:25:16.000000 squice-0.5/src/squice/Matrix3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:16.000000 squice-0.5/src/squice/ModulePredict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-27 17:25:16.000000 squice-0.5/src/squice/MtxDisplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-27 17:25:16.000000 squice-0.5/src/squice/MtxInterpolator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11412 2024-05-27 17:25:16.000000 squice-0.5/src/squice/SpaceTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-05-27 17:25:16.000000 squice-0.5/src/squice/VectorThree.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:16.000000 squice-0.5/src/squice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79087 2024-05-27 17:25:16.000000 squice-0.5/src/squice/_interpolator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.317177 squice-0.5/src/squice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-27 17:25:22.000000 squice-0.5/src/squice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-27 17:25:22.000000 squice-0.5/src/squice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 17:25:22.000000 squice-0.5/src/squice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 17:25:22.000000 squice-0.5/src/squice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.313177 squice-0.5/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:16.000000 squice-0.5/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.313177 squice-0.5/src/tests/speed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:16.000000 squice-0.5/src/tests/speed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.317177 squice-0.5/src/tests/speed/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-27 17:25:16.000000 squice-0.5/src/tests/speed/data/speed_data.npy
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-27 17:25:16.000000 squice-0.5/src/tests/speed/data/speed_log.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-27 17:25:16.000000 squice-0.5/src/tests/speed/help_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-27 17:25:16.000000 squice-0.5/src/tests/speed/test_dataloaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.317177 squice-0.5/src/tests/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:16.000000 squice-0.5/src/tests/utility/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.317177 squice-0.5/src/tests/utility/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-27 17:25:16.000000 squice-0.5/src/tests/utility/data/data1.npy
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-27 17:25:16.000000 squice-0.5/src/tests/utility/data/data3d.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-27 17:25:16.000000 squice-0.5/src/tests/utility/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-27 17:25:16.000000 squice-0.5/src/tests/utility/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-27 17:25:16.000000 squice-0.5/tmp
```

### Comparing `squice-0.4/.github/scripts/release.py` & `squice-0.5/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `squice-0.4/.github/workflows/docker.yml` & `squice-0.5/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `squice-0.4/.github/workflows/lint_style.yml` & `squice-0.5/.github/workflows/lint_style.yml`

 * *Files identical despite different names*

### Comparing `squice-0.4/.github/workflows/pydoctor.yml` & `squice-0.5/.github/workflows/pydoctor.yml`

 * *Files identical despite different names*

### Comparing `squice-0.4/.github/workflows/pytest_app.yml` & `squice-0.5/.github/workflows/pytest_app.yml`

 * *Files identical despite different names*

### Comparing `squice-0.4/.github/workflows/pytest_lib.yml` & `squice-0.5/.github/workflows/pytest_lib.yml`

 * *Files identical despite different names*

### Comparing `squice-0.4/.gitignore` & `squice-0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `squice-0.4/Dockerfile` & `squice-0.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `squice-0.4/LICENSE` & `squice-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `squice-0.4/PKG-INFO` & `squice-0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squice
-Version: 0.4
+Version: 0.5
 Summary: Example library for scientific software.
 Home-page: https://github.com/RachelAlcraft/squice
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/RachelAlcraft/squice/issues
 Project-URL: Documentation, https://rachelalcraft.github.io/squice
 Project-URL: Application demo, https://squice.streamlit.app
```

### Comparing `squice-0.4/README.md` & `squice-0.5/README.md`

 * *Files identical despite different names*

### Comparing `squice-0.4/app/static/squice.png` & `squice-0.5/app/static/squice.png`

 * *Files identical despite different names*

### Comparing `squice-0.4/dev.md` & `squice-0.5/dev.md`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 ## Load dev environment
 source .env-sq-lib/bin/activate
 (deactivate to exit venv)
 pip install --upgrade pip
 pip install -r requirements_lib.txt --upgrade
 ```
 
+To install the lib locally while developing
+```
+pip install .
+```
+
 ## Pre-commit
 
 The pre-commit hook shyuld run on check in to format files as per standards.
 ```
 pre-commit run --all-files
 black ./ --check --line-length 88 --diff
 black ./ --line-length 88
```

### Comparing `squice-0.4/setup.cfg` & `squice-0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `squice-0.4/src/squice/DataLoaders.py` & `squice-0.5/src/squice/DataLoaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                 v.append(strv)
             vec_slicesb.append(v)
         self.numa = len(vec_slicesb)
         self.numb = len(vec_slicesb[0])
         self.filedata = self.filedata.replace("]", "")
         self.filedata = self.filedata.replace("[", "")
         self.numc = int(len(self.filedata.split(",")) / (self.numa * self.numb))
-        self.mtx = np.fromstring(self.filedata, dtype=int, sep=",").reshape(
+        self.mtx = np.fromstring(self.filedata, dtype=float, sep=",").reshape(
             [self.numa, self.numb, self.numc]
         )
 
 
 ####################################################################################
 class NumpyFile(DataLoader):
     """Class to load a file of numerical data from numpy serislisation format"""
```

### Comparing `squice-0.4/src/squice.egg-info/PKG-INFO` & `squice-0.5/src/squice.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squice
-Version: 0.4
+Version: 0.5
 Summary: Example library for scientific software.
 Home-page: https://github.com/RachelAlcraft/squice
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/RachelAlcraft/squice/issues
 Project-URL: Documentation, https://rachelalcraft.github.io/squice
 Project-URL: Application demo, https://squice.streamlit.app
```

### Comparing `squice-0.4/src/squice.egg-info/SOURCES.txt` & `squice-0.5/src/squice.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 .gitignore
 .pre-commit-config.yaml
 Dockerfile
 LICENSE
 README.md
 citation.cff
 dev.md
+matrix (1).npy
 pyproject.toml
 requirements.txt
 requirements_lib.txt
 setup.cfg
+tmp
 .github/scripts/release.py
 .github/workflows/docker.yml
 .github/workflows/lint_style.yml
 .github/workflows/publish.yml
 .github/workflows/pydoctor.yml
 .github/workflows/pytest_app.yml
 .github/workflows/pytest_lib.yml
 .github/workflows/release.yml
 app/home.py
 app/pages/2_example.py
-app/pages/3_use_template.py
 app/pages/4_about.py
 app/static/squice.png
 app/tests/use_cases/test_add_curve.py
 docs/docs.md
 src/README.md
+src/__init__.py
+src/squice/BinaryFile.py
 src/squice/DataLoaders.py
+src/squice/GridMaker.py
+src/squice/Matrix3d.py
 src/squice/ModulePredict.py
 src/squice/MtxDisplay.py
 src/squice/MtxInterpolator.py
+src/squice/SpaceTransform.py
+src/squice/VectorThree.py
 src/squice/__init__.py
+src/squice/_interpolator.py
 src/squice.egg-info/PKG-INFO
 src/squice.egg-info/SOURCES.txt
 src/squice.egg-info/dependency_links.txt
 src/squice.egg-info/top_level.txt
 src/tests/__init__.py
 src/tests/speed/__init__.py
 src/tests/speed/help_speed.py
 src/tests/speed/test_dataloaders.py
 src/tests/speed/data/speed_data.npy
 src/tests/speed/data/speed_log.csv
 src/tests/utility/__init__.py
 src/tests/utility/test_loader.py
+src/tests/utility/test_slice.py
 src/tests/utility/data/data1.npy
 src/tests/utility/data/data3d.npy
```

### Comparing `squice-0.4/src/tests/speed/data/speed_log.csv` & `squice-0.5/src/tests/speed/data/speed_log.csv`

 * *Files identical despite different names*

### Comparing `squice-0.4/src/tests/speed/help_speed.py` & `squice-0.5/src/tests/speed/help_speed.py`

 * *Files identical despite different names*

### Comparing `squice-0.4/src/tests/speed/test_dataloaders.py` & `squice-0.5/src/tests/speed/test_dataloaders.py`

 * *Files identical despite different names*

### Comparing `squice-0.4/src/tests/utility/test_loader.py` & `squice-0.5/src/tests/utility/test_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         assert npf.mtx[0][0][0] == 1, npf.mtx[0][0][0]
 
 
 def test_numpynow_tabs_and_lines():
     print(f"Testing utility: {inspect.stack()[0][3]}")
     datas = []
     datas.append(
-        "[[[1,2],[3,4],[3,4]], \t[[5,6],[7,8],[7,8]], \n[[5,6],[7,8],[7,8]],\t [[5,6],[7,8],[7,8]\n]]"
+        "[[[1.0,2],[3,4],[3,4]], \t[[5,6],[7,8],[7,8]], \n[[5,6],[7,8],[7,8]],\t [[5,6],[7,8],[7,8]\n]]"
     )
 
     for dt in datas:
         print(dt)
         npf = cc.NumpyNow(dt)
         npf.load()
         assert npf.mtx[0][0][0] == 1, npf.mtx[0][0][0]
```

