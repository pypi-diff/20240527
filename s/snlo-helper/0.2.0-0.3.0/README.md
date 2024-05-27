# Comparing `tmp/snlo_helper-0.2.0.tar.gz` & `tmp/snlo_helper-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snlo_helper-0.2.0.tar", last modified: Tue May  7 08:46:42 2024, max compression
+gzip compressed data, was "snlo_helper-0.3.0.tar", last modified: Mon May 27 12:09:19 2024, max compression
```

## Comparing `snlo_helper-0.2.0.tar` & `snlo_helper-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 08:46:42.590736 snlo_helper-0.2.0/
-drwxrwxrwx   0        0        0        0 2024-05-07 08:46:42.481284 snlo_helper-0.2.0/.github/
-drwxrwxrwx   0        0        0        0 2024-05-07 08:46:42.512429 snlo_helper-0.2.0/.github/workflows/
--rw-rw-rw-   0        0        0      925 2024-05-07 08:28:00.000000 snlo_helper-0.2.0/.github/workflows/python-publish.yml
--rw-rw-rw-   0        0        0     1969 2024-05-03 14:47:36.000000 snlo_helper-0.2.0/.gitignore
--rw-rw-rw-   0        0        0      414 2024-05-07 08:36:48.000000 snlo_helper-0.2.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     3437 2024-05-07 08:46:42.590736 snlo_helper-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2733 2024-05-07 08:17:46.000000 snlo_helper-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 08:46:42.512429 snlo_helper-0.2.0/examples/
--rw-rw-rw-   0        0        0     8606 2024-05-07 08:06:54.000000 snlo_helper-0.2.0/examples/get_spectr.py
--rw-rw-rw-   0        0        0      201 2024-05-07 08:04:22.000000 snlo_helper-0.2.0/examples/test.py
--rw-rw-rw-   0        0        0     4424 2024-05-07 08:07:05.000000 snlo_helper-0.2.0/examples/upconversion.py
--rw-rw-rw-   0        0        0     1105 2024-05-07 08:42:20.000000 snlo_helper-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 08:46:42.590736 snlo_helper-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-07 08:46:42.590736 snlo_helper-0.2.0/snlo_helper.egg-info/
--rw-rw-rw-   0        0        0     3437 2024-05-07 08:46:42.000000 snlo_helper-0.2.0/snlo_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2024-05-07 08:46:42.000000 snlo_helper-0.2.0/snlo_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 08:46:42.000000 snlo_helper-0.2.0/snlo_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-07 08:46:42.000000 snlo_helper-0.2.0/snlo_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-07 08:46:42.000000 snlo_helper-0.2.0/snlo_helper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 08:46:42.575108 snlo_helper-0.2.0/snlohelper/
--rw-rw-rw-   0        0        0        0 2024-04-24 08:11:13.000000 snlo_helper-0.2.0/snlohelper/__init__.py
--rw-rw-rw-   0        0        0     4746 2024-05-03 14:47:36.000000 snlo_helper-0.2.0/snlohelper/base_function.py
--rw-rw-rw-   0        0        0     3199 2024-05-03 14:47:36.000000 snlo_helper-0.2.0/snlohelper/focus.py
--rw-rw-rw-   0        0        0     1321 2024-05-06 16:30:12.000000 snlo_helper-0.2.0/snlohelper/functions.py
--rw-rw-rw-   0        0        0     1037 2024-04-24 08:09:00.000000 snlo_helper-0.2.0/snlohelper/import_snlo_file.py
--rw-rw-rw-   0        0        0     1758 2024-05-06 16:29:36.000000 snlo_helper-0.2.0/snlohelper/main_window.py
--rw-rw-rw-   0        0        0      922 2024-05-03 14:47:36.000000 snlo_helper-0.2.0/snlohelper/mix_methods.py
--rw-rw-rw-   0        0        0     1471 2024-05-03 14:47:36.000000 snlo_helper-0.2.0/snlohelper/ref_index.py
--rw-rw-rw-   0        0        0      708 2024-04-25 09:11:35.000000 snlo_helper-0.2.0/snlohelper/snlo.py
--rw-rw-rw-   0        0        0     2729 2024-04-25 09:00:51.000000 snlo_helper-0.2.0/snlohelper/two_d_mix_lp.py
--rw-rw-rw-   0        0        0     2372 2024-04-24 12:06:47.000000 snlo_helper-0.2.0/snlohelper/two_d_mix_sp.py
--rw-rw-rw-   0        0        0     3618 2024-05-03 14:47:36.000000 snlo_helper-0.2.0/snlohelper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:09:19.047900 snlo_helper-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:09:19.043900 snlo_helper-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:09:19.043900 snlo_helper-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-27 12:09:19.047900 snlo_helper-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:09:19.043900 snlo_helper-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/examples/get_spectr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/examples/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/examples/upconversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:09:19.047900 snlo_helper-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:09:19.047900 snlo_helper-0.3.0/snlo_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-27 12:09:19.000000 snlo_helper-0.3.0/snlo_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-27 12:09:19.000000 snlo_helper-0.3.0/snlo_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:09:19.000000 snlo_helper-0.3.0/snlo_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 12:09:19.000000 snlo_helper-0.3.0/snlo_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 12:09:19.000000 snlo_helper-0.3.0/snlo_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:09:19.047900 snlo_helper-0.3.0/snlohelper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/snlohelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/snlohelper/base_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/snlohelper/focus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/snlohelper/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/snlohelper/import_snlo_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/snlohelper/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/snlohelper/mix_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/snlohelper/pw_opo_bb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/snlohelper/q_mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/snlohelper/ref_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/snlohelper/snlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/snlohelper/two_d_mix_lp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/snlohelper/two_d_mix_sp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-27 12:09:08.000000 snlo_helper-0.3.0/snlohelper/utils.py
```

### Comparing `snlo_helper-0.2.0/PKG-INFO` & `snlo_helper-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,69 @@
-Metadata-Version: 2.1
-Name: snlo-helper
-Version: 0.2.0
-Summary: An autoclicker to automatically configure and read SNLO.
-Author: Benedikt Burger
-Project-URL: Repository, https://github.com/BenediktBurger/snlo-helper
-Project-URL: Issues, https://github.com/BenediktBurger/snlo-helper/issues
-Keywords: SNLO,nonlinear optics,simulation
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Utilities
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Requires-Dist: pyautogui
-Requires-Dist: pyperclip
-Provides-Extra: full
-Requires-Dist: numpy; extra == "full"
-
-# SNLO-Helper
-
-SNLO-Helper helps to use [SNLO](https://as-photonics.com/products/snlo/) software for simulation of nonlinear optical processes in crystals.
-
-An autoclicker clicks different buttons and fills fields in order to automate SNLO simulations.
-Afterwards, it can retrieve the results and return them as a dictionary.
-
-Attention:
-- The script does use your mouse and keyboard, so you should not interact with the computer at the same time.
-- The script uses predefined positions of the windows, so **do not move the windows**.
-- The autoclicker can be interrupted by moving the mouse into the top left corner of the screen.
-
-
-Currently it supports the following functions (feel free to add more):
-- Ref. Ind.
-- 2D-mix-LP
-- 2D-mix-SP
-- Focus
-
-
-## Installation
-
-Install it executing `pip install -e .` in this folder or via `pip install git+https://git.rwth-aachen.de/nloqo/snlo-helper.git` to download it in the background and install it.
-
-
-## Usage
-
-### Quick Start
-
-1. Start SNLO on your computer
-2. Import `snlohelper.main_window.MainWindow` as a starting point.
-3. Create an instande `mw = MainWindow`
-4. Open the desired function: `ri = mw.open_function(Functions.REF_INDEX)`
-5. Execute it `no, ne = ri.refractive_indices(Wavelength=1234)`
-
-Here is a small snippet how to do a 2D mix of long pulses:
-```
-from snlohelper.main_window import MainWindow
-
-mw = MainWindow()
-mix = mw.open_two_d_mix_lp()
-mix.configure({"Wavelengths (nm)": [1064.5, None, None]})
-result = mix.run_and_read()
-print(result)
-```
-
-For more examples see the `examples` folder.
-
-
-### General usage
-
-* The `main_window.MainWindow` class manages the main window.
-* For several functions exists a module containing a class, which in turn allows to configure the function, to run the calculation, and to extract the result.
-  1. You start that class, for example `mix = two_d_mix_lp.TwoDMixLp()` or `mix = MainWindow().open_function("2D-Mix-LP")`.
-  2. You can configure it giving a configuration dictionary (the keys correspond to the names) with `mix.configure({"Wavelengths": [1064, None, None]})`. If a value is `None`, it won't be changed.
-  3. You can run it with `mix.run()`
-  4. With `results = mix.read_results()` you can extract the resulting text.
-  5. With `result_dict = mix.interpret_results(results)` you get a dictionary of the result data
-  6. There are convenience methods like `mix.run_and_read` which runs and returns the dictionary, or even `mix.configure_run_read`, which does all of above steps in one.
-
-
-## Contribution
-
-You are welcome to contribute to this library.
-Just open an issue for suggestions or bug reports and open a pull request for code contributions.
+# SNLO-Helper
+
+[![pypi release](https://img.shields.io/pypi/v/snlo-helper.svg)](https://pypi.org/project/snlo-helper/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11125163.svg)](https://doi.org/10.5281/zenodo.11125163)
+[![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)
+
+SNLO-Helper helps to use [SNLO](https://as-photonics.com/products/snlo/) software for simulation of nonlinear optical processes in crystals.
+
+An autoclicker clicks different buttons and fills fields in order to automate SNLO simulations.
+Afterwards, it can retrieve the results and return them as a dictionary.
+
+Attention:
+- The script does use your mouse and keyboard, so you should not interact with the computer at the same time.
+- The script uses predefined positions of the windows, so **do not move the windows**.
+- The autoclicker can be interrupted by moving the mouse into the top left corner of the screen.
+
+
+Currently it supports the following functions (feel free to add more):
+- Ref. Ind.
+- 2D-mix-LP
+- 2D-mix-SP
+- Focus
+
+
+## Installation
+
+Install it executing `pip install -e .` in this folder or via `pip install snlo-helper` to download it in the background and install it.
+
+
+## Usage
+
+### Quick Start
+
+1. Start SNLO on your computer
+2. Import `snlohelper.main_window.MainWindow` as a starting point.
+3. Create an instande `mw = MainWindow`
+4. Open the desired function: `ri = mw.open_function(Functions.REF_INDEX)`
+5. Execute it `no, ne = ri.refractive_indices(Wavelength=1234)`
+
+Here is a small snippet how to do a 2D mix of long pulses:
+```
+from snlohelper.main_window import MainWindow
+
+mw = MainWindow()
+mix = mw.open_two_d_mix_lp()
+mix.configure({"Wavelengths (nm)": [1064.5, None, None]})
+result = mix.run_and_read()
+print(result)
+```
+
+For more examples see the `examples` folder.
+
+
+### General usage
+
+* The `main_window.MainWindow` class manages the main window.
+* For several functions exists a module containing a class, which in turn allows to configure the function, to run the calculation, and to extract the result.
+  1. You start that class, for example `mix = two_d_mix_lp.TwoDMixLp()` or `mix = MainWindow().open_function("2D-Mix-LP")`.
+  2. You can configure it giving a configuration dictionary (the keys correspond to the names) with `mix.configure({"Wavelengths": [1064, None, None]})`. If a value is `None`, it won't be changed.
+  3. You can run it with `mix.run()`
+  4. With `results = mix.read_results()` you can extract the resulting text.
+  5. With `result_dict = mix.interpret_results(results)` you get a dictionary of the result data
+  6. There are convenience methods like `mix.run_and_read` which runs and returns the dictionary, or even `mix.configure_run_read`, which does all of above steps in one.
+
+
+## Contribution
+
+You are welcome to contribute to this library.
+Just open an issue for suggestions or bug reports and open a pull request for code contributions.
```

### Comparing `snlo_helper-0.2.0/snlo_helper.egg-info/PKG-INFO` & `snlo_helper-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,89 @@
-Metadata-Version: 2.1
-Name: snlo-helper
-Version: 0.2.0
-Summary: An autoclicker to automatically configure and read SNLO.
-Author: Benedikt Burger
-Project-URL: Repository, https://github.com/BenediktBurger/snlo-helper
-Project-URL: Issues, https://github.com/BenediktBurger/snlo-helper/issues
-Keywords: SNLO,nonlinear optics,simulation
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Utilities
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Requires-Dist: pyautogui
-Requires-Dist: pyperclip
-Provides-Extra: full
-Requires-Dist: numpy; extra == "full"
-
-# SNLO-Helper
-
-SNLO-Helper helps to use [SNLO](https://as-photonics.com/products/snlo/) software for simulation of nonlinear optical processes in crystals.
-
-An autoclicker clicks different buttons and fills fields in order to automate SNLO simulations.
-Afterwards, it can retrieve the results and return them as a dictionary.
-
-Attention:
-- The script does use your mouse and keyboard, so you should not interact with the computer at the same time.
-- The script uses predefined positions of the windows, so **do not move the windows**.
-- The autoclicker can be interrupted by moving the mouse into the top left corner of the screen.
-
-
-Currently it supports the following functions (feel free to add more):
-- Ref. Ind.
-- 2D-mix-LP
-- 2D-mix-SP
-- Focus
-
-
-## Installation
-
-Install it executing `pip install -e .` in this folder or via `pip install git+https://git.rwth-aachen.de/nloqo/snlo-helper.git` to download it in the background and install it.
-
-
-## Usage
-
-### Quick Start
-
-1. Start SNLO on your computer
-2. Import `snlohelper.main_window.MainWindow` as a starting point.
-3. Create an instande `mw = MainWindow`
-4. Open the desired function: `ri = mw.open_function(Functions.REF_INDEX)`
-5. Execute it `no, ne = ri.refractive_indices(Wavelength=1234)`
-
-Here is a small snippet how to do a 2D mix of long pulses:
-```
-from snlohelper.main_window import MainWindow
-
-mw = MainWindow()
-mix = mw.open_two_d_mix_lp()
-mix.configure({"Wavelengths (nm)": [1064.5, None, None]})
-result = mix.run_and_read()
-print(result)
-```
-
-For more examples see the `examples` folder.
-
-
-### General usage
-
-* The `main_window.MainWindow` class manages the main window.
-* For several functions exists a module containing a class, which in turn allows to configure the function, to run the calculation, and to extract the result.
-  1. You start that class, for example `mix = two_d_mix_lp.TwoDMixLp()` or `mix = MainWindow().open_function("2D-Mix-LP")`.
-  2. You can configure it giving a configuration dictionary (the keys correspond to the names) with `mix.configure({"Wavelengths": [1064, None, None]})`. If a value is `None`, it won't be changed.
-  3. You can run it with `mix.run()`
-  4. With `results = mix.read_results()` you can extract the resulting text.
-  5. With `result_dict = mix.interpret_results(results)` you get a dictionary of the result data
-  6. There are convenience methods like `mix.run_and_read` which runs and returns the dictionary, or even `mix.configure_run_read`, which does all of above steps in one.
-
-
-## Contribution
-
-You are welcome to contribute to this library.
-Just open an issue for suggestions or bug reports and open a pull request for code contributions.
+Metadata-Version: 2.1
+Name: snlo-helper
+Version: 0.3.0
+Summary: An autoclicker to automatically configure and read SNLO.
+Author: Benedikt Burger
+Project-URL: Repository, https://github.com/BenediktBurger/snlo-helper
+Project-URL: Issues, https://github.com/BenediktBurger/snlo-helper/issues
+Keywords: SNLO,nonlinear optics,simulation
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Utilities
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyautogui
+Requires-Dist: pyperclip
+Provides-Extra: full
+Requires-Dist: numpy; extra == "full"
+
+# SNLO-Helper
+
+[![pypi release](https://img.shields.io/pypi/v/snlo-helper.svg)](https://pypi.org/project/snlo-helper/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11125163.svg)](https://doi.org/10.5281/zenodo.11125163)
+[![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)
+
+SNLO-Helper helps to use [SNLO](https://as-photonics.com/products/snlo/) software for simulation of nonlinear optical processes in crystals.
+
+An autoclicker clicks different buttons and fills fields in order to automate SNLO simulations.
+Afterwards, it can retrieve the results and return them as a dictionary.
+
+Attention:
+- The script does use your mouse and keyboard, so you should not interact with the computer at the same time.
+- The script uses predefined positions of the windows, so **do not move the windows**.
+- The autoclicker can be interrupted by moving the mouse into the top left corner of the screen.
+
+
+Currently it supports the following functions (feel free to add more):
+- Ref. Ind.
+- 2D-mix-LP
+- 2D-mix-SP
+- Focus
+
+
+## Installation
+
+Install it executing `pip install -e .` in this folder or via `pip install snlo-helper` to download it in the background and install it.
+
+
+## Usage
+
+### Quick Start
+
+1. Start SNLO on your computer
+2. Import `snlohelper.main_window.MainWindow` as a starting point.
+3. Create an instande `mw = MainWindow`
+4. Open the desired function: `ri = mw.open_function(Functions.REF_INDEX)`
+5. Execute it `no, ne = ri.refractive_indices(Wavelength=1234)`
+
+Here is a small snippet how to do a 2D mix of long pulses:
+```
+from snlohelper.main_window import MainWindow
+
+mw = MainWindow()
+mix = mw.open_two_d_mix_lp()
+mix.configure({"Wavelengths (nm)": [1064.5, None, None]})
+result = mix.run_and_read()
+print(result)
+```
+
+For more examples see the `examples` folder.
+
+
+### General usage
+
+* The `main_window.MainWindow` class manages the main window.
+* For several functions exists a module containing a class, which in turn allows to configure the function, to run the calculation, and to extract the result.
+  1. You start that class, for example `mix = two_d_mix_lp.TwoDMixLp()` or `mix = MainWindow().open_function("2D-Mix-LP")`.
+  2. You can configure it giving a configuration dictionary (the keys correspond to the names) with `mix.configure({"Wavelengths": [1064, None, None]})`. If a value is `None`, it won't be changed.
+  3. You can run it with `mix.run()`
+  4. With `results = mix.read_results()` you can extract the resulting text.
+  5. With `result_dict = mix.interpret_results(results)` you get a dictionary of the result data
+  6. There are convenience methods like `mix.run_and_read` which runs and returns the dictionary, or even `mix.configure_run_read`, which does all of above steps in one.
+
+
+## Contribution
+
+You are welcome to contribute to this library.
+Just open an issue for suggestions or bug reports and open a pull request for code contributions.
```

### Comparing `snlo_helper-0.2.0/snlo_helper.egg-info/SOURCES.txt` & `snlo_helper-0.3.0/snlo_helper.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 CHANGELOG.md
+LICENSE
 README.md
 pyproject.toml
 .github/workflows/python-publish.yml
 examples/get_spectr.py
 examples/test.py
 examples/upconversion.py
 snlo_helper.egg-info/PKG-INFO
@@ -14,12 +15,14 @@
 snlohelper/__init__.py
 snlohelper/base_function.py
 snlohelper/focus.py
 snlohelper/functions.py
 snlohelper/import_snlo_file.py
 snlohelper/main_window.py
 snlohelper/mix_methods.py
+snlohelper/pw_opo_bb.py
+snlohelper/q_mix.py
 snlohelper/ref_index.py
 snlohelper/snlo.py
 snlohelper/two_d_mix_lp.py
 snlohelper/two_d_mix_sp.py
 snlohelper/utils.py
```

### Comparing `snlo_helper-0.2.0/snlohelper/main_window.py` & `snlo_helper-0.3.0/snlohelper/main_window.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,90 @@
-"""
-The SNLO main window
-"""
-
-from typing import Optional, TypeVar
-
-from .utils import gui, scale, get_screenfactors, set_screenfactors, Point
-from .functions import Functions, open_function
-from .base_function import BaseFunction
-from .ref_index import RefractiveIndex
-from .focus import Focus
-from .two_d_mix_lp import TwoDMixLP
-from .two_d_mix_sp import TwoDMixSP
-
-
-function_classes = {
-    Functions.REF_INDEX: RefractiveIndex,
-    Functions.TWOD_MIX_LP: TwoDMixLP,
-    Functions.TWOD_MIX_SP: TwoDMixSP,
-    Functions.FOCUS: Focus,
-}
-
-FunctionClass = TypeVar("FunctionClass")
-
-
-class MainWindow:
-    _close_pos = (95, 14)
-
-    def __init__(self, screenfactors: Optional[Point] = None, **kwargs) -> None:
-        super().__init__(**kwargs)
-        sf = get_screenfactors()
-        if sf is None or screenfactors is not None:
-            set_screenfactors(new_factors=screenfactors)
-
-    def close(self) -> None:
-        gui.click(*scale(self._close_pos))
-
-    def open_function(self, key: str | Functions) -> Optional[BaseFunction]:
-        open_function(key)
-        if key in function_classes:
-            return function_classes[key]()
-
-    def _open_function(self, function_class: type[FunctionClass]) -> FunctionClass:
-        function = function_class()
-        function.open()  # type: ignore
-        return function
-
-    def open_refractive_index(self) -> RefractiveIndex:
-        return self._open_function(RefractiveIndex)
-
-    def open_two_d_mix_lp(self) -> TwoDMixLP:
-        return self._open_function(TwoDMixLP)
-
-    def open_two_d_mix_sp(self) -> TwoDMixSP:
-        return self._open_function(TwoDMixSP)
-
-    def open_focus(self) -> Focus:
-        return self._open_function(Focus)
+# MIT License
+
+# Copyright (c) 2024 Benedikt Burger
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+"""
+The SNLO main window
+"""
+
+from typing import Optional, TypeVar
+
+from .utils import gui, scale, get_screenfactors, set_screenfactors, Point
+from .functions import Functions, open_function
+from .base_function import BaseFunction
+from .ref_index import RefractiveIndex
+from .focus import Focus
+from .two_d_mix_lp import TwoDMixLP
+from .two_d_mix_sp import TwoDMixSP
+from .q_mix import QMix
+from .pw_opo_bb import PW_OPO_BB
+
+
+function_classes = {
+    Functions.REF_INDEX: RefractiveIndex,
+    Functions.QMIX: QMix,
+    Functions.TWOD_MIX_LP: TwoDMixLP,
+    Functions.TWOD_MIX_SP: TwoDMixSP,
+    Functions.PW_OPO_BB: PW_OPO_BB,
+    Functions.FOCUS: Focus,
+}
+
+FunctionClass = TypeVar("FunctionClass")
+
+
+class MainWindow:
+    _close_pos = (95, 14)
+
+    def __init__(self, screenfactors: Optional[Point] = None, **kwargs) -> None:
+        super().__init__(**kwargs)
+        sf = get_screenfactors()
+        if sf is None or screenfactors is not None:
+            set_screenfactors(new_factors=screenfactors)
+
+    def close(self) -> None:
+        gui.click(*scale(self._close_pos))
+
+    def open_function(self, key: str | Functions) -> Optional[BaseFunction]:
+        open_function(key)
+        if key in function_classes:
+            return function_classes[key]()
+
+    def _open_function(self, function_class: type[FunctionClass]) -> FunctionClass:
+        function = function_class()
+        function.open()  # type: ignore
+        return function
+
+    def open_refractive_index(self) -> RefractiveIndex:
+        return self._open_function(RefractiveIndex)
+    
+    def open_q_mix(self) -> QMix:
+        return self._open_function(QMix)
+
+    def open_two_d_mix_lp(self) -> TwoDMixLP:
+        return self._open_function(TwoDMixLP)
+
+    def open_two_d_mix_sp(self) -> TwoDMixSP:
+        return self._open_function(TwoDMixSP)
+    
+    def open_pw_opo_bb(self) -> PW_OPO_BB:
+        return self._open_function(PW_OPO_BB)
+
+    def open_focus(self) -> Focus:
+        return self._open_function(Focus)
```

### Comparing `snlo_helper-0.2.0/snlohelper/two_d_mix_lp.py` & `snlo_helper-0.3.0/snlohelper/two_d_mix_lp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,75 @@
-from .main_window import Functions
-from .mix_methods import MixMethods
-
-
-class TwoDMixLP(MixMethods):
-    """The '2D-mix-LP' method."""
-
-    _function = Functions.TWOD_MIX_LP
-    _accept_pos = (506, 520)
-    _run_pos = (140, 220)
-    _close_pos = (540, 140)
-    _change_inputs_pos = (373, 166)
-    _result_pos = (133, 293)
-
-    # coordinates of the 2DmixLP-function (in FHD standard)
-    _configuration_pos = {
-        "Wavelengths (nm)": [(400, 186), (460, 186), (520, 186)],
-        "Indexes of refraction": [(400, 200), (460, 200), (520, 200)],
-        "Phases at input (rad)": [(400, 213), (460, 213), (520, 213)],
-        "Input face reflectivity (0-1)": [(400, 226), (460, 226), (520, 226)],
-        "Output face reflectivity (0-1)": [(400, 246), (460, 246), (520, 246)],
-        "Crystal loss (1/mm)": [(400, 260), (460, 260), (520, 260)],
-        "Energy/power (J or W)": [(416, 280), (483, 280), (550, 280)],
-        "Pulse duration (fwhm ns)": [(400, 293), (460, 293), (520, 293)],
-        "Beam diam. (fwhm mm)": [(400, 306), (460, 306), (520, 306)],
-        "Supergaussian coeff.": [(400, 326), (460, 326), (520, 326)],
-        "n2 red1 (sq cm/W)": [(400, 340), (460, 340), (520, 340)],
-        "n2 red2 (sq cm/W)": [(400, 360), (460, 360), (520, 360)],
-        "n2 blue (sq cm/W)": [(400, 373), (460, 373), (520, 373)],
-        "beta red1 (cm/W)": [(400, 393), (460, 393), (520, 393)],
-        "beta red2 (cm/W)": [(400, 406), (460, 406), (520, 406)],
-        "beta blue (cm/W)": [(400, 420), (460, 420), (520, 420)],
-        "Walkoff angles (mrad)": [(400, 440), (460, 440), (520, 440)],
-        "Offset in wo dir. (mm)": [(400, 453), (460, 453), (520, 453)],
-        "Rad. curv. (mm/air)": [(400, 473), (460, 473), (520, 473)],
-        "# of integ/grid points": [(400, 486), (460, 486), (520, 486)],
-        "Crystal/grid sizes (mm)": [(400, 500), (460, 500), (520, 500)],
-        "Deff (pm/V)": [(400, 520)],
-        "Delta k (1/mm)": [(400, 533)],
-        "Dist. to image (mm)": [(400, 546)],
-        "# time steps": [(400, 566)],
-    }
-
-    def interpret_results(self, rows: list[str]) -> dict[str, float | list[float]]:
-        """Interpret the results."""
-        return {
-            "Input peak irradiance (W/sq cm)": [float(i) for i in rows[0].split()[5:]],
-            "Input peak fluence (J/sq cm)": [float(i) for i in rows[1].split()[6:]],
-            "Input peak powers (W)": [float(i) for i in rows[2].split()[5:]],
-            "Output peak fluence (J/sq cm)": [float(i) for i in rows[3].split()[6:]],
-            "Output pulse energy (mJ)": [float(i) for i in rows[4].split()[5:]],
-            "So (W/sq cm)": float(rows[5].split()[4]),
-        }
+# MIT License
+
+# Copyright (c) 2024 Benedikt Burger
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+from .main_window import Functions
+from .mix_methods import MixMethods
+
+
+class TwoDMixLP(MixMethods):
+    """The '2D-mix-LP' method."""
+
+    _function = Functions.TWOD_MIX_LP
+    _accept_pos = (506, 520)
+    _run_pos = (140, 220)
+    _close_pos = (540, 140)
+    _change_inputs_pos = (373, 166)
+    _result_pos = (133, 293)
+
+    # coordinates of the 2DmixLP-function (in FHD standard)
+    _configuration_pos = {
+        "Wavelengths (nm)": [(400, 186), (460, 186), (520, 186)],
+        "Indexes of refraction": [(400, 200), (460, 200), (520, 200)],
+        "Phases at input (rad)": [(400, 213), (460, 213), (520, 213)],
+        "Input face reflectivity (0-1)": [(400, 226), (460, 226), (520, 226)],
+        "Output face reflectivity (0-1)": [(400, 246), (460, 246), (520, 246)],
+        "Crystal loss (1/mm)": [(400, 260), (460, 260), (520, 260)],
+        "Energy/power (J or W)": [(416, 280), (483, 280), (550, 280)],
+        "Pulse duration (fwhm ns)": [(400, 293), (460, 293), (520, 293)],
+        "Beam diam. (fwhm mm)": [(400, 306), (460, 306), (520, 306)],
+        "Supergaussian coeff.": [(400, 326), (460, 326), (520, 326)],
+        "n2 red1 (sq cm/W)": [(400, 340), (460, 340), (520, 340)],
+        "n2 red2 (sq cm/W)": [(400, 360), (460, 360), (520, 360)],
+        "n2 blue (sq cm/W)": [(400, 373), (460, 373), (520, 373)],
+        "beta red1 (cm/W)": [(400, 393), (460, 393), (520, 393)],
+        "beta red2 (cm/W)": [(400, 406), (460, 406), (520, 406)],
+        "beta blue (cm/W)": [(400, 420), (460, 420), (520, 420)],
+        "Walkoff angles (mrad)": [(400, 440), (460, 440), (520, 440)],
+        "Offset in wo dir. (mm)": [(400, 453), (460, 453), (520, 453)],
+        "Rad. curv. (mm/air)": [(400, 473), (460, 473), (520, 473)],
+        "# of integ/grid points": [(400, 486), (460, 486), (520, 486)],
+        "Crystal/grid sizes (mm)": [(400, 500), (460, 500), (520, 500)],
+        "Deff (pm/V)": [(400, 520)],
+        "Delta k (1/mm)": [(400, 533)],
+        "Dist. to image (mm)": [(400, 546)],
+        "# time steps": [(400, 566)],
+    }
+
+    def interpret_results(self, rows: list[str]) -> dict[str, float | list[float]]:
+        """Interpret the results."""
+        return {
+            "Input peak irradiance (W/sq cm)": [float(i) for i in rows[0].split()[5:]],
+            "Input peak fluence (J/sq cm)": [float(i) for i in rows[1].split()[6:]],
+            "Input peak powers (W)": [float(i) for i in rows[2].split()[5:]],
+            "Output peak fluence (J/sq cm)": [float(i) for i in rows[3].split()[6:]],
+            "Output pulse energy (mJ)": [float(i) for i in rows[4].split()[5:]],
+            "So (W/sq cm)": float(rows[5].split()[4]),
+        }
```

