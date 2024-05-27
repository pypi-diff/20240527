# Comparing `tmp/oresat_c3-0.4.0.tar.gz` & `tmp/oresat_c3-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat_c3-0.4.0.tar", last modified: Thu May 23 00:28:11 2024, max compression
+gzip compressed data, was "oresat_c3-0.5.0.tar", last modified: Mon May 27 02:23:10 2024, max compression
```

## Comparing `oresat_c3-0.4.0.tar` & `oresat_c3-0.5.0.tar`

### file list

```diff
@@ -1,85 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.918331 oresat_c3-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.906331 oresat_c3-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.906331 oresat_c3-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-23 00:28:11.918331 oresat_c3-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.910331 oresat_c3-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/edl.rst
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/opd.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/state.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.910331 oresat_c3-0.4.0/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/static/comms_ipc.drawio
--rw-r--r--   0 runner    (1001) docker     (127)    33084 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/static/comms_ipc.jpg
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    98849 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/static/opd.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.910331 oresat_c3-0.4.0/oresat_c3/
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 00:28:11.000000 oresat_c3-0.4.0/oresat_c3/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.910331 oresat_c3-0.4.0/oresat_c3/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/drivers/fm24cl64b.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/drivers/max7310.py
--rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/drivers/si41xx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.910331 oresat_c3-0.4.0/oresat_c3/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/protocols/ax25.py
--rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/protocols/edl_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/protocols/edl_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.914331 oresat_c3-0.4.0/oresat_c3/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/services/beacon.py
--rw-r--r--   0 runner    (1001) docker     (127)    29640 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/services/edl.py
--rw-r--r--   0 runner    (1001) docker     (127)    14657 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/services/node_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/services/radios.py
--rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/services/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.914331 oresat_c3-0.4.0/oresat_c3/subsystems/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/subsystems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/subsystems/antennas.py
--rw-r--r--   0 runner    (1001) docker     (127)    15253 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/subsystems/opd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/subsystems/rtc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.914331 oresat_c3-0.4.0/oresat_c3/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/templates/beacon.html
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/templates/keys.html
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/templates/node_manager.html
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/templates/state.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.918331 oresat_c3-0.4.0/oresat_c3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-23 00:28:11.000000 oresat_c3-0.4.0/oresat_c3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-23 00:28:11.000000 oresat_c3-0.4.0/oresat_c3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 00:28:11.000000 oresat_c3-0.4.0/oresat_c3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-23 00:28:11.000000 oresat_c3-0.4.0/oresat_c3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-23 00:28:11.000000 oresat_c3-0.4.0/oresat_c3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 00:28:11.000000 oresat_c3-0.4.0/oresat_c3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.914331 oresat_c3-0.4.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)    14219 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/scripts/edl_cmd_shell.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13336 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/scripts/edl_file_upload.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4214 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/scripts/edl_ping_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 00:28:11.918331 oresat_c3-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.914331 oresat_c3-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.914331 oresat_c3-0.4.0/tests/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/drivers/test_fm23cl64b.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/drivers/test_max7310.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.914331 oresat_c3-0.4.0/tests/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/protocols/test_ax25.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/protocols/test_edl_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/protocols/test_edl_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.914331 oresat_c3-0.4.0/tests/services/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/services/test_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.918331 oresat_c3-0.4.0/tests/subsystems/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/subsystems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/subsystems/test_opd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.497593 oresat_c3-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.481593 oresat_c3-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.485593 oresat_c3-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-27 02:23:10.497593 oresat_c3-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.489593 oresat_c3-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/docs/edl.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/docs/opd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/docs/state.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.489593 oresat_c3-0.5.0/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/docs/static/comms_ipc.drawio
+-rw-r--r--   0 runner    (1001) docker     (127)    33084 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/docs/static/comms_ipc.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/docs/static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    98849 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/docs/static/opd.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.489593 oresat_c3-0.5.0/oresat_c3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 02:23:10.000000 oresat_c3-0.5.0/oresat_c3/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.489593 oresat_c3-0.5.0/oresat_c3/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/drivers/fm24cl64b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/drivers/max7310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/drivers/si41xx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.493593 oresat_c3-0.5.0/oresat_c3/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/protocols/ax25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/protocols/cachestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/protocols/cfdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/protocols/edl_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/protocols/edl_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.493593 oresat_c3-0.5.0/oresat_c3/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/services/beacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28484 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/services/edl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/services/node_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/services/radios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/services/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.493593 oresat_c3-0.5.0/oresat_c3/subsystems/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/subsystems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/subsystems/antennas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16913 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/subsystems/opd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/subsystems/rtc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.493593 oresat_c3-0.5.0/oresat_c3/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/templates/beacon.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/templates/keys.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/templates/node_manager.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/oresat_c3/templates/state.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.497593 oresat_c3-0.5.0/oresat_c3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-27 02:23:10.000000 oresat_c3-0.5.0/oresat_c3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-27 02:23:10.000000 oresat_c3-0.5.0/oresat_c3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 02:23:10.000000 oresat_c3-0.5.0/oresat_c3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-27 02:23:10.000000 oresat_c3-0.5.0/oresat_c3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-27 02:23:10.000000 oresat_c3-0.5.0/oresat_c3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 02:23:10.000000 oresat_c3-0.5.0/oresat_c3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.493593 oresat_c3-0.5.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14216 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/scripts/edl_cmd_shell.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14754 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/scripts/edl_file_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4214 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/scripts/edl_ping_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 02:23:10.497593 oresat_c3-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.493593 oresat_c3-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.497593 oresat_c3-0.5.0/tests/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/tests/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/tests/drivers/test_fm23cl64b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/tests/drivers/test_max7310.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.497593 oresat_c3-0.5.0/tests/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/tests/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/tests/protocols/test_ax25.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10658 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/tests/protocols/test_cachestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/tests/protocols/test_edl_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/tests/protocols/test_edl_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.497593 oresat_c3-0.5.0/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/tests/services/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:10.497593 oresat_c3-0.5.0/tests/subsystems/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/tests/subsystems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-27 02:23:05.000000 oresat_c3-0.5.0/tests/subsystems/test_opd.py
```

### Comparing `oresat_c3-0.4.0/.github/workflows/pypi.yaml` & `oresat_c3-0.5.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/.github/workflows/tests.yaml` & `oresat_c3-0.5.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/.gitignore` & `oresat_c3-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/LICENSE` & `oresat_c3-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/PKG-INFO` & `oresat_c3-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-c3
-Version: 0.4.0
+Version: 0.5.0
 Summary: OreSat C3 OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oresat_c3-0.4.0/README.md` & `oresat_c3-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/docs/Makefile` & `oresat_c3-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/docs/conf.py` & `oresat_c3-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/docs/edl.rst` & `oresat_c3-0.5.0/docs/edl.rst`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/docs/make.bat` & `oresat_c3-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/docs/opd.rst` & `oresat_c3-0.5.0/docs/opd.rst`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/docs/state.rst` & `oresat_c3-0.5.0/docs/state.rst`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/docs/static/comms_ipc.drawio` & `oresat_c3-0.5.0/docs/static/comms_ipc.drawio`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/docs/static/comms_ipc.jpg` & `oresat_c3-0.5.0/docs/static/comms_ipc.jpg`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/docs/static/opd.jpg` & `oresat_c3-0.5.0/docs/static/opd.jpg`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/oresat_c3/__init__.py` & `oresat_c3-0.5.0/oresat_c3/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/oresat_c3/__main__.py` & `oresat_c3-0.5.0/oresat_c3/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     olaf_setup,
     render_olaf_template,
     rest_api,
     set_cpufreq_gov,
 )
 
 from . import C3State, __version__
+from .protocols.cachestore import CacheStore
 from .services.beacon import BeaconService
 from .services.edl import EdlService
 from .services.node_manager import NodeManagerService
 from .services.radios import RadiosService
 from .services.state import StateService
 from .subsystems.rtc import set_system_time_to_rtc_time
 
@@ -116,14 +117,17 @@
     mock_args = [i.lower() for i in args.mock_hw]
     mock_hw = len(mock_args) != 0
 
     # start watchdog thread ASAP
     thread = Thread(target=watchdog, daemon=True)
     thread.start()
 
+    # The C3 needs a special OreSatFileCache that can speak CFDP
+    app.node._fwrite_cache = CacheStore(app.node.fwrite_cache.dir)  # pylint: disable=W0212
+
     app.od["versions"]["sw_version"].value = __version__
     if app.od["versions"]["hw_version"].value == "6.0":
         app.od["hw_id"].value = get_hw_id(mock_hw)
 
     state_service = StateService(config.fram_def, mock_hw)
     radios_service = RadiosService(mock_hw)
     beacon_service = BeaconService(config.beacon_def, radios_service)
```

### Comparing `oresat_c3-0.4.0/oresat_c3/drivers/fm24cl64b.py` & `oresat_c3-0.5.0/oresat_c3/drivers/fm24cl64b.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/oresat_c3/drivers/max7310.py` & `oresat_c3-0.5.0/oresat_c3/drivers/max7310.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/oresat_c3/drivers/si41xx.py` & `oresat_c3-0.5.0/oresat_c3/drivers/si41xx.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/oresat_c3/protocols/ax25.py` & `oresat_c3-0.5.0/oresat_c3/protocols/ax25.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/oresat_c3/protocols/edl_command.py` & `oresat_c3-0.5.0/oresat_c3/protocols/edl_command.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/oresat_c3/protocols/edl_packet.py` & `oresat_c3-0.5.0/oresat_c3/protocols/edl_packet.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/oresat_c3/services/beacon.py` & `oresat_c3-0.5.0/oresat_c3/services/beacon.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/oresat_c3/services/edl.py` & `oresat_c3-0.5.0/oresat_c3/services/edl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 """'EDL Service"""
 
-import struct
 from collections.abc import Iterable
 from datetime import timedelta
 from pathlib import Path
 from queue import Empty, SimpleQueue
 from time import time
 from typing import Any, Optional
 
 import canopen
 from cfdppy import CfdpState, PacketDestination, get_packet_destination
 from cfdppy.exceptions import (
     FsmNotCalledAfterPacketInsertion,
     NoRemoteEntityCfgFound,
     SourceFileDoesNotExist,
+    UnretrievedPdusToBeSent,
 )
-from cfdppy.filestore import HostFilestore
-from cfdppy.handler.crc import CrcHelper
-from cfdppy.handler.dest import DestHandler
-from cfdppy.handler.source import SourceHandler
 from cfdppy.mib import (
     CheckTimerProvider,
     DefaultFaultHandlerBase,
     IndicationCfg,
     LocalEntityCfg,
     RemoteEntityCfg,
     RemoteEntityCfgTable,
@@ -32,28 +28,32 @@
     CfdpUserBase,
     FileSegmentRecvdParams,
     MetadataRecvParams,
     TransactionFinishedParams,
     TransactionId,
     TransactionParams,
 )
-from olaf import MasterNode, NodeStop, OreSatFileCache, Service, logger
-from spacepackets.cfdp import NULL_CHECKSUM_U32, ChecksumType, ConditionCode, TransmissionMode
+from olaf import MasterNode, NodeStop, Service, logger
+from spacepackets.cfdp import ChecksumType, ConditionCode, FaultHandlerCode, TransmissionMode
 from spacepackets.cfdp.defs import DeliveryCode, FileStatus
 from spacepackets.cfdp.pdu import AbstractFileDirectiveBase
 from spacepackets.cfdp.tlv import (
-    FilestoreResponseStatusCode,
+    DirectoryListingResponse,
+    DirectoryOperationMessageType,
     OriginatingTransactionId,
+    ProxyMessageType,
     ProxyPutResponse,
     ProxyPutResponseParams,
 )
 from spacepackets.countdown import Countdown
 from spacepackets.seqcount import SeqCountProvider
 from spacepackets.util import ByteFieldU8
 
+from ..protocols.cachestore import CacheStore
+from ..protocols.cfdp import FixedDestHandler, VfsCrcHelper, VfsSourceHandler
 from ..protocols.edl_command import (
     EdlCommandCode,
     EdlCommandError,
     EdlCommandRequest,
     EdlCommandResponse,
 )
 from ..protocols.edl_packet import SRC_DEST_UNICLOGS, EdlPacket, EdlPacketError, EdlVcid
@@ -75,16 +75,15 @@
     ):
         super().__init__()
 
         self._radios_service = radios_service
         self._node_mgr_service = node_mgr_service
         self._beacon_service = beacon_service
 
-        upload_dir = f"{node.work_base_dir}/upload"
-        self._file_receiver = EdlFileReciever(upload_dir, node.fwrite_cache)
+        self._file_receiver = EdlFileReciever(node.fwrite_cache)
 
         # objs
         edl_rec = node.od["edl"]
         tx_rec = node.od["tx_control"]
         self._flight_mode_obj = node.od["flight_mode"]
         self._seq_num = edl_rec["sequence_count"].value
         self._tx_enable_obj = tx_rec["enable"]
@@ -339,116 +338,14 @@
         response = EdlCommandResponse(request.code, ret)
 
         logger.info(f"EDL command response: {response.code.name}, values: {response.values}")
 
         return response
 
 
-class PrefixedFilestore(HostFilestore):
-    """A HostFilestore modified to only run in a specified directory"""
-
-    def __init__(self, prefix: Path):
-        if not prefix.is_dir():
-            raise NotADirectoryError("prefix must be a directory")
-        self._prefix = prefix
-
-    def read_data(self, file: Path, offset: Optional[int], read_len: Optional[int] = None) -> bytes:
-        return super().read_data(self._prefix.joinpath(file), offset, read_len)
-
-    def file_exists(self, path: Path) -> bool:
-        return super().file_exists(self._prefix.joinpath(path))
-
-    def is_directory(self, path: Path) -> bool:
-        return super().is_directory(self._prefix.joinpath(path))
-
-    def truncate_file(self, file: Path):
-        super().truncate_file(self._prefix.joinpath(file))
-
-    def write_data(self, file: Path, data: bytes, offset: Optional[int]):
-        super().write_data(self._prefix.joinpath(file), data, offset)
-
-    def create_file(self, file: Path) -> FilestoreResponseStatusCode:
-        return super().create_file(self._prefix.joinpath(file))
-
-    def delete_file(self, file: Path) -> FilestoreResponseStatusCode:
-        return super().delete_file(self._prefix.joinpath(file))
-
-    def rename_file(self, old_file: Path, new_file: Path) -> FilestoreResponseStatusCode:
-        return super().rename_file(self._prefix.joinpath(old_file), self._prefix.joinpath(new_file))
-
-    def replace_file(self, replaced_file: Path, source_file: Path) -> FilestoreResponseStatusCode:
-        return super().replace_file(
-            self._prefix.joinpath(replaced_file),
-            self._prefix.joinpath(source_file),
-        )
-
-    def remove_directory(
-        self, dir_name: Path, recursive: bool = False
-    ) -> FilestoreResponseStatusCode:
-        return super().remove_directory(self._prefix.joinpath(dir_name), recursive)
-
-    def create_directory(self, dir_name: Path) -> FilestoreResponseStatusCode:
-        return super().create_directory(self._prefix.joinpath(dir_name))
-
-    def list_directory(
-        self, dir_name: Path, target_file: Path, recursive: bool = False
-    ) -> FilestoreResponseStatusCode:
-        return super().list_directory(self._prefix.joinpath(dir_name), target_file, recursive)
-
-
-class VfsCrcHelper(CrcHelper):
-    """CrcHelper but modified to only use Filestore operations.
-
-    It previously would attempt to open the paths passed to it directly instead of asking the
-    filestore, which failed when using the above PrefixFilestore.
-    """
-
-    def calc_modular_checksum(self, file_path: Path) -> bytes:
-        """Calculates the modular checksum of the file in file_path.
-
-        This was a module level function in cfdppy but it accessed the filesystem directly
-        instead of going through a filestore. It needs to become a CrcHelper method to use the
-        provided filestore.
-        """
-        checksum = 0
-        offset = 0
-        while True:
-            data = self.vfs.read_data(file_path, offset, 4)
-            offset += 4
-            if not data:
-                break
-            checksum += int.from_bytes(data.ljust(4, b"\0"), byteorder="big", signed=False)
-
-        checksum %= 2**32
-        return struct.pack("!I", checksum)
-
-    def calc_for_file(self, file_path: Path, file_sz: int, segment_len: int = 4096) -> bytes:
-        if self.checksum_type == ChecksumType.NULL_CHECKSUM:
-            return NULL_CHECKSUM_U32
-        if self.checksum_type == ChecksumType.MODULAR:
-            return self.calc_modular_checksum(file_path)
-        crc_obj = self.generate_crc_calculator()
-        if segment_len == 0:
-            raise ValueError("Segment length can not be 0")
-        if not self.vfs.file_exists(file_path):
-            raise SourceFileDoesNotExist(file_path)
-        current_offset = 0
-
-        # Calculate the file CRC
-        while current_offset < file_sz:
-            if current_offset + segment_len > file_sz:
-                read_len = file_sz - current_offset
-            else:
-                read_len = segment_len
-            if read_len > 0:
-                crc_obj.update(self.vfs.read_data(file_path, current_offset, read_len))
-            current_offset += read_len
-        return crc_obj.digest()
-
-
 class LogFaults(DefaultFaultHandlerBase):
     """A HaultHandler that only logs the faults and nothing more.
 
     At some point this should be replaced with something more robust.
     """
 
     def notice_of_suspension_cb(self, transaction_id, cond, progress):
@@ -474,26 +371,51 @@
     def provide_check_timer(self, local_entity_id, remote_entity_id, entity_type) -> Countdown:
         return Countdown(timedelta(seconds=5.0))
 
 
 class EdlFileReciever(CfdpUserBase):
     """CFDP receiver for file uploads."""
 
-    def __init__(self, upload_dir: str, fwrite_cache: OreSatFileCache):
-        path = Path(upload_dir)
-        path.mkdir(parents=True, exist_ok=True)
-        super().__init__(vfs=PrefixedFilestore(path))
+    def __init__(self, fwrite_cache: CacheStore):
+        super().__init__(vfs=fwrite_cache)
+
+        self.proxy_responses = {  # FIXME: defaultdict with invalid response
+            ProxyMessageType.PUT_REQUEST: self.proxy_put_response,
+            ProxyMessageType.MSG_TO_USER: self.unimplemented,
+            ProxyMessageType.FS_REQUEST: self.unimplemented,
+            ProxyMessageType.FAULT_HANDLER_OVERRIDE: self.unimplemented,
+            ProxyMessageType.TRANSMISSION_MODE: self.unimplemented,
+            ProxyMessageType.FLOW_LABEL: self.unimplemented,
+            ProxyMessageType.SEGMENTATION_CTRL: self.unimplemented,
+            ProxyMessageType.PUT_RESPONSE: self.unimplemented,
+            ProxyMessageType.FS_RESPONSE: self.unimplemented,
+            ProxyMessageType.PUT_CANCEL: self.unimplemented,
+            ProxyMessageType.CLOSURE_REQUEST: self.unimplemented,
+            DirectoryOperationMessageType.LISTING_REQUEST: self.directory_listing_response,
+            DirectoryOperationMessageType.LISTING_RESPONSE: self.unimplemented,
+            DirectoryOperationMessageType.CUSTOM_LISTING_PARAMETERS: self.unimplemented,
+        }
 
         SOURCE_ID = ByteFieldU8(0)
         DEST_ID = ByteFieldU8(1)
+        fault_handler = LogFaults()
+        # The default setting is NOTICE_OF_CANCELLATION but during that process the positive ack
+        # counter gets reset, meaning we keep retrying the handler forever. This manifests for
+        # example if the final source -> dest ack for FinishedPDU gets dropped. Source considers
+        # the transaction finished, and will refuse to respond, dest will be stuck re-sending the
+        # FinishedPDU every ack_timer interval forever. Setting it to ABANDON_TRANSACTION means it
+        # just resets after the ack counter reaches its count.
+        fault_handler.set_handler(
+            ConditionCode.POSITIVE_ACK_LIMIT_REACHED, FaultHandlerCode.ABANDON_TRANSACTION
+        )
 
         localcfg = LocalEntityCfg(
             local_entity_id=DEST_ID,
             indication_cfg=IndicationCfg(),
-            default_fault_handlers=LogFaults(),
+            default_fault_handlers=fault_handler,
         )
 
         remote_entities = RemoteEntityCfgTable(
             [
                 RemoteEntityCfg(
                     entity_id=SOURCE_ID,
                     max_file_segment_len=None,
@@ -505,30 +427,30 @@
                     crc_on_transmission=False,
                     default_transmission_mode=TransmissionMode.ACKNOWLEDGED,
                     crc_type=ChecksumType.CRC_32,
                 ),
             ]
         )
 
-        self.fwrite_cache = fwrite_cache
-        self.dest = DestHandler(
+        self.dest = FixedDestHandler(
             cfg=localcfg,
             user=self,
             remote_cfg_table=remote_entities,
             check_timer_provider=DefaultCheckTimer(),
         )
         self.dest._cksum_verif_helper = VfsCrcHelper(ChecksumType.NULL_CHECKSUM, self.vfs)
 
-        self.source = SourceHandler(
+        self.source = VfsSourceHandler(
             cfg=localcfg,
             user=self,
             remote_cfg_table=remote_entities,
             check_timer_provider=DefaultCheckTimer(),
             seq_num_provider=SeqCountProvider(16),
         )
+        self.source._crc_helper = VfsCrcHelper(ChecksumType.NULL_CHECKSUM, self.vfs)
 
         self.scheduled_requests: SimpleQueue[PutRequest] = SimpleQueue()
         self.active_requests: dict[TransactionId, TransactionId] = {}
 
     @property
     def state(self) -> CfdpState:
         """Either BUSY or IDLE
@@ -555,24 +477,24 @@
         # pdu.
         if pdu:
             logger.info(f"<--- {pdu}")
 
             if get_packet_destination(pdu) == PacketDestination.DEST_HANDLER:
                 try:
                     self.dest.insert_packet(pdu)
-                except FsmNotCalledAfterPacketInsertion:
+                except Exception:
                     # Usually this exception means the library is being used wrong, so we have
                     # to be careful here. However there is a bug in the presence of dropped packets
                     # where dest._params.last_inserted_packet does not get cleared.
                     logger.exception("dest.state_machine() didn't properly clear inserted packet")
                     self.dest.reset()
             else:
                 try:
                     self.source.insert_packet(pdu)
-                except FsmNotCalledAfterPacketInsertion:
+                except Exception:
                     logger.exception("source.state_machine() didn't properly clear inserted packet")
                     self.source.reset()
 
         if self.dest.state == CfdpState.IDLE and self.source.state == CfdpState.IDLE:
             try:
                 request = self.scheduled_requests.get_nowait()
             except Empty:
@@ -584,27 +506,36 @@
                     # Note that NoRemoteEntityCfgFound indicates that the MIB is missing info on
                     # the requested proxy transfer destination. CFDP doesn't seem to have a
                     # standard set of errors that cover this condition, and the least worst option
                     # resulted in an identical message to missing_file. Not super great, so if
                     # there's a better idea of how to handle this, please change.
                     self.scheduled_requests.put(self.missing_file_response(request))
 
-        self.dest.state_machine()
-        self.source.state_machine()
+        try:
+            self.dest.state_machine()
+            self.source.state_machine()
+        except Exception:
+            logger.exception("state_machine failed to update")
+            self.dest.reset()
+            self.source.reset()
 
         pdus = []
         while self.dest.packets_ready:
             pdus.append(self.dest.get_next_packet().pdu)
         while self.source.packets_ready:
             pdus.append(self.source.get_next_packet().pdu)
 
         for out in pdus:
             logger.info(f"---> {out}")
         return pdus or None
 
+    def unimplemented(self, _source, _tid, _reserved_message) -> PutRequest:
+        """Default method for responding to unimplemented requests"""
+        return None
+
     def missing_file_response(self, invalid: PutRequest) -> PutRequest:
         """Generates a resonse put for when a proxy request tries to access a missing file"""
 
         originating_id = (
             invalid.msgs_to_user[0].to_reserved_msg_tlv().get_originating_transaction_id()
         )
         return PutRequest(
@@ -623,14 +554,66 @@
                         file_status=FileStatus.DISCARDED_FILESTORE_REJECTION,
                     )
                 ).to_generic_msg_to_user_tlv(),
                 OriginatingTransactionId(originating_id).to_generic_msg_to_user_tlv(),
             ],
         )
 
+    def proxy_put_response(self, _source, _tid, reserved_message) -> PutRequest:
+        """Response for a proxy put request"""
+        params = reserved_message.get_proxy_put_request_params()
+        return PutRequest(
+            destination_id=params.dest_entity_id,
+            source_file=Path(params.source_file_as_path),
+            dest_file=Path(params.dest_file_as_path),
+            trans_mode=None,
+            closure_requested=True,
+            msgs_to_user=[
+                OriginatingTransactionId(params.transaction_id).to_generic_msg_to_user_tlv()
+            ],
+        )
+
+    def directory_listing_response(self, source, tid, reserved_message) -> PutRequest:
+        """Response for a directory listing request"""
+        # See CFDP 6.3.4
+        params = reserved_message.get_dir_listing_request_params()
+        self.vfs.list_directory(params.dir_path_as_path, params.dir_file_name_as_path, False)
+        return PutRequest(
+            destination_id=source,
+            source_file=params.dir_file_name_as_path,
+            dest_file=params.dir_file_name_as_path,
+            trans_mode=None,
+            closure_requested=True,
+            msgs_to_user=[
+                DirectoryListingResponse(
+                    listing_success=True,
+                    dir_params=params,
+                ).to_generic_msg_to_user_tlv(),
+                OriginatingTransactionId(tid).to_generic_msg_to_user_tlv(),
+            ],
+        )
+
+    def proxy_request_complete(self, originating_id, params) -> PutRequest:
+        """Indicates that a proxy put request was successful"""
+        return PutRequest(
+            destination_id=originating_id.source_id,
+            source_file=None,
+            dest_file=None,
+            trans_mode=None,
+            # FIXME: upstream bug - DestHandler does not respect closure_requested=None when
+            # trans_mode defaults to ACKNOWLEGED
+            closure_requested=True,
+            msgs_to_user=[
+                ProxyPutResponse(
+                    ProxyPutResponseParams.from_finished_params(params.finished_params)
+                ).to_generic_msg_to_user_tlv(),
+                OriginatingTransactionId(originating_id).to_generic_msg_to_user_tlv(),
+            ],
+        )
+
     def transaction_indication(self, transaction_indication_params: TransactionParams):
         logger.info(f"Indication: Transaction. {transaction_indication_params}")
         t_id = transaction_indication_params.transaction_id
         orig = transaction_indication_params.originating_transaction_id
         if orig is not None:
             self.active_requests[t_id] = orig
 
@@ -638,52 +621,26 @@
         logger.info(f"Indication: EOF Sent for {transaction_id}.")
 
     def transaction_finished_indication(self, params: TransactionFinishedParams):
         logger.info(f"Indication: Transaction Finished. {params}")
         if params.transaction_id in self.active_requests:
             originating_id = self.active_requests.get(params.transaction_id)
             assert originating_id is not None
-            put = PutRequest(
-                destination_id=originating_id.source_id,
-                source_file=None,
-                dest_file=None,
-                trans_mode=None,
-                # FIXME: upstream bug - DestHandler does not respect closure_requested=None when
-                # trans_mode defaults to ACKNOWLEGED
-                closure_requested=True,
-                msgs_to_user=[
-                    ProxyPutResponse(
-                        ProxyPutResponseParams.from_finished_params(params.finished_params)
-                    ).to_generic_msg_to_user_tlv(),
-                    OriginatingTransactionId(originating_id).to_generic_msg_to_user_tlv(),
-                ],
-            )
+            put = self.proxy_request_complete(originating_id, params)
             self.scheduled_requests.put(put)
             del self.active_requests[params.transaction_id]
 
     def metadata_recv_indication(self, params: MetadataRecvParams):
         logger.info(f"Indication: Metadata Recv. {params}")
         for msg in params.msgs_to_user or []:
-            if msg.is_reserved_cfdp_message():
-                reserved = msg.to_reserved_msg_tlv()
-                if reserved.is_cfdp_proxy_operation():
-                    proxyparams = reserved.get_proxy_put_request_params()
-                    put = PutRequest(
-                        destination_id=proxyparams.dest_entity_id,
-                        source_file=Path(proxyparams.source_file_as_path),
-                        dest_file=Path(proxyparams.dest_file_as_path),
-                        trans_mode=None,
-                        closure_requested=None,
-                        msgs_to_user=[
-                            OriginatingTransactionId(
-                                params.transaction_id
-                            ).to_generic_msg_to_user_tlv()
-                        ],
-                    )
-                    self.scheduled_requests.put(put)
+            if r := msg.to_reserved_msg_tlv():  # is None if not a reserved TLV message
+                op = r.get_cfdp_proxy_message_type() or r.get_directory_operation_type()
+                put = self.proxy_responses[op](params.source_id, params.transaction_id, r)
+                self.scheduled_requests.put(put)
+            # Ignore non-reserved messages for now
 
     def file_segment_recv_indication(self, params: FileSegmentRecvdParams):
         logger.info(f"Indication: File Segment Recv. {params}")
 
     def report_indication(self, transaction_id: TransactionId, status_report: Any):
         logger.info(f"Indication: Report for {transaction_id}. {status_report}")
```

### Comparing `oresat_c3-0.4.0/oresat_c3/services/node_manager.py` & `oresat_c3-0.5.0/oresat_c3/services/node_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 class Node(Card):
     """Node data."""
 
     opd_resets: int = 0
     """OPD reset count."""
     last_enable: float = 0.0
     """last enable timeout."""
-    status: NodeState = NodeState.OFF
+    status: NodeState = NodeState.NOT_FOUND
     """Node status."""
 
 
 class NodeManagerService(Service):
     """Node manager service."""
 
     _MAX_CO_RESETS = 3
@@ -116,28 +116,28 @@
         self._nodes_off_obj: canopen.objectdictionary.Variable = None
         self._nodes_booting_obj: canopen.objectdictionary.Variable = None
         self._nodes_on_obj: canopen.objectdictionary.Variable = None
         self._nodes_with_errors_obj: canopen.objectdictionary.Variable = None
         self._nodes_not_found_obj: canopen.objectdictionary.Variable = None
         self._nodes_dead_obj: canopen.objectdictionary.Variable = None
 
-        self.opd.enable()
-
     def on_start(self):
         # local objects
         self._flight_mode_obj = self.node.od["flight_mode"]
         nodes_mgr_rec = self.node.od["node_manager"]
         self._nodes_off_obj = nodes_mgr_rec["nodes_off"]
         self._nodes_booting_obj = nodes_mgr_rec["nodes_booting"]
         self._nodes_on_obj = nodes_mgr_rec["nodes_on"]
         self._nodes_not_found_obj = nodes_mgr_rec["nodes_not_found"]
         self._nodes_with_errors_obj = nodes_mgr_rec["nodes_with_errors"]
         self._nodes_dead_obj = nodes_mgr_rec["nodes_dead"]
         nodes_mgr_rec["total_nodes"].value = len(list(self._data))
 
+        self.opd.enable()
+
         self.node.add_sdo_callbacks("node_manager", "status_json", self._get_status_json, None)
         self.node.add_sdo_callbacks("opd", "status", self._get_opd_status, self._set_opd_status)
         self.node.add_sdo_callbacks(
             "opd",
             "uart_node_select",
             self._get_uart_node_select,
             self._set_uart_node_select,
@@ -151,34 +151,43 @@
                 lambda n=name: self.node_status(n),
                 lambda v, n=name: self._set_node_status(n, v),
             )
 
     def _check_co_nodes_state(self, name: str) -> NodeState:
         """Get a CANopen node's state."""
 
-        next_state = self._data[name].status
+        node = self._data[name]
+        next_state = node.status
+        last_hb = self.node.node_status[name][2]
+
         if next_state == NodeState.DEAD:
+            if monotonic() > last_hb + self._RESET_TIMEOUT_S:
+                # if the node start sending heartbeats again (really only for flatsat)
+                next_state = NodeState.ON
             return next_state
 
-        if self._data[name].processor == "stm32":
+        if node.processor == "stm32":
             timeout = self._STM32_BOOT_TIMEOUT
         else:
             timeout = self._OCTAVO_BOOT_TIMEOUT
 
-        last_hb = self.node.node_status[name][2]
-        if self._data[name].last_enable + timeout > monotonic():
+        if node.last_enable + timeout > monotonic():
             if monotonic() > last_hb + self._RESET_TIMEOUT_S:
                 next_state = NodeState.BOOT
             else:
                 next_state = NodeState.ON
-        elif self._data[name].status == NodeState.ERROR:
+        elif node.status == NodeState.ERROR:
             next_state = NodeState.ERROR
-        elif self._flight_mode_obj.value and monotonic() > (last_hb + self._RESET_TIMEOUT_S):
+        elif (
+            self._flight_mode_obj.value
+            and self.node.bus_state == "NETWORK_UP"
+            and monotonic() > (last_hb + self._RESET_TIMEOUT_S)
+        ):
             logger.error(
-                f"CANopen node {name} has had no heartbeats in " f"{self._RESET_TIMEOUT_S} seconds"
+                f"CANopen node {name} has had no heartbeats in {self._RESET_TIMEOUT_S} seconds"
             )
             next_state = NodeState.ERROR
         else:
             next_state = NodeState.ON
 
         return next_state
 
@@ -203,22 +212,20 @@
         next_state = prev_state
 
         # update status of data on the OPD
         if self.opd.status == OpdState.DEAD:
             next_state = NodeState.DEAD
         else:
             status = self.opd[name].status
-            if status == OpdNodeState.FAULT:
+            if self._data[name].opd_resets >= self._MAX_CO_RESETS:
+                next_state = NodeState.DEAD
+            elif status == OpdNodeState.FAULT:
                 next_state = NodeState.ERROR
             elif status == OpdNodeState.NOT_FOUND:
                 next_state = NodeState.NOT_FOUND
-            elif (
-                prev_state == NodeState.ERROR and self._data[name].opd_resets >= self._MAX_CO_RESETS
-            ):
-                next_state = NodeState.DEAD
             elif status == OpdNodeState.ENABLED:
                 if self._data[name].processor == "stm32" and self.opd[name].in_bootloader_mode:
                     next_state = NodeState.BOOTLOADER
                 elif self._data[name].node_id != 0:  # aka CANopen nodes
                     next_state = self._check_co_nodes_state(name)
                 else:
                     next_state = NodeState.ON
@@ -235,60 +242,62 @@
 
         nodes_off = 0
         nodes_booting = 0
         nodes_on = 0
         nodes_with_errors = 0
         nodes_not_found = 0
         nodes_dead = 0
-        for name in self._data:
+        for name, node in self._data.items():
             if name == "c3":
                 continue
 
-            last_state = self._data[name].status
+            last_state = node.status
             state = self._get_nodes_state(name)
-            if state != last_state:
+            if self._loops != 0 and state != last_state:
                 logger.info(f"node {name} state change {last_state.name} -> {state.name}")
             nodes_off += int(state == NodeState.OFF)
             nodes_booting += int(state == NodeState.BOOT)
             nodes_on += int(state == NodeState.ON)
             nodes_with_errors += int(state == NodeState.ERROR)
             nodes_not_found += int(state == NodeState.NOT_FOUND)
             nodes_dead += int(state == NodeState.DEAD)
-            self._data[name].status = state
+            node.status = state
         self._nodes_off_obj.value = nodes_off
         self._nodes_booting_obj.value = nodes_booting
         self._nodes_on_obj.value = nodes_on
         self._nodes_with_errors_obj.value = nodes_with_errors
         self._nodes_not_found_obj.value = nodes_not_found
         self._nodes_dead_obj.value = nodes_dead
 
         if self.opd.status in [OpdState.DEAD, OpdState.DISABLED]:
             self._loops = -1
             return  # nothing to monitor
 
         if nodes_not_found == len(self._data):
             self._loops = 0
 
-        # reset data with errors and probe for data not found
+        # reset nodes with errors and probe for nodes not found
         for name, info in self._data.items():
             if info.opd_address == 0:
                 continue
 
-            if self._loops % 60 == 0 and self._data[name].status == NodeState.NOT_FOUND:
+            if self._loops % 10 == 0 and self._data[name].status == NodeState.NOT_FOUND:
                 self.opd[name].probe(True)
 
             if info.opd_always_on and info.status == NodeState.OFF:
                 self.enable(name)
 
-            if info.status == NodeState.ERROR:
+            if info.status == NodeState.DEAD and self.opd[name].is_enabled:
+                self.opd[name].disable()  # make sure this is disabled
+            elif info.status == NodeState.ERROR:
                 logger.error(f"resetting node {name}, try {info.opd_resets + 1}")
                 self.opd[name].reset(1)
                 self._data[name].last_enable = monotonic()
                 info.opd_resets += 1
-            else:
+            elif info.status in [NodeState.ON, NodeState.OFF]:
                 info.opd_resets = 0
 
     def enable(self, name: Union[str, int], bootloader_mode: bool = False):
         """
         Enable a OreSat node.
 
         Parameters
@@ -394,14 +403,18 @@
 
     def _get_opd_status(self) -> int:
         return self.opd.status.value
 
     def _set_opd_status(self, value: int):
         if value == 0:
             self.opd.disable()
+            for name, node in self._data.items():
+                if node.opd_address != 0 and node.status != NodeState.NOT_FOUND:
+                    logger.info(f"node {name} state change {node.status.name} -> NOT_FOUND")
+                    node.status = NodeState.NOT_FOUND
         elif value == 1:
             if self.opd.status == OpdState.DISABLED:
                 for node in self._data.values():
                     node.last_enable = monotonic()
             self.opd.enable()
 
     def _get_uart_node_select(self) -> int:
```

### Comparing `oresat_c3-0.4.0/oresat_c3/services/radios.py` & `oresat_c3-0.5.0/oresat_c3/services/radios.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/oresat_c3/services/state.py` & `oresat_c3-0.5.0/oresat_c3/services/state.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/oresat_c3/subsystems/antennas.py` & `oresat_c3-0.5.0/oresat_c3/subsystems/antennas.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/oresat_c3/subsystems/opd.py` & `oresat_c3-0.5.0/oresat_c3/subsystems/opd.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 class OpdNode:
     """
     Base class for all OPD nodes
 
     NOTE: CFC sensor node does not have UART enable pin.
     """
 
-    _RESET_DELAY_S = 0.25
+    _RESET_DELAY_S = 0.5
 
     _TIMEOUT_CONFIG = 1
 
     # these are consistent between all cards
     _NOT_FAULT_PIN = 2
     _ENABLE_PIN = 3
     _CB_RESET_PIN = 4
@@ -74,18 +74,23 @@
         except Max7310Error:
             pass
 
     def configure(self):
         """Configure the MAX7310 for the OPD node."""
 
         inputs = 1 << self._NOT_FAULT_PIN
-        self._max7310.configure(0, 0, inputs, self._TIMEOUT_CONFIG)
-        if self._mock:
-            self._max7310._mock_input_set(self._NOT_FAULT_PIN)  # pylint: disable=W0212
-        self._status = OpdNodeState.DISABLED
+        try:
+            self._max7310.configure(0, 0, inputs, self._TIMEOUT_CONFIG)
+            if self._mock:
+                self._max7310._mock_input_set(self._NOT_FAULT_PIN)  # pylint: disable=W0212
+            self._status = OpdNodeState.DISABLED
+        except Max7310Error as e:
+            logger.error(f"MAX7310 error: {e}")
+            logger.debug(f"OPD node {self.name} (0x{self.addr:02X}) was not configured")
+            self._status = OpdNodeState.FAULT
 
     def probe(self, reset: bool = False) -> bool:
         """
         Probe the OPD for a node (see if it is there). Will automatically call configure the
         MAX7310, if found.
 
         Parameters
@@ -103,25 +108,25 @@
 
         if self._status == OpdNodeState.DEAD:
             return False  # node is dead, no reason to probe
 
         try:
             if self._max7310.is_valid:
                 if self._status == OpdNodeState.NOT_FOUND:
-                    logger.info(f"OPD node {self.name} (0x{self.addr:02X}) was found")
+                    logger.debug(f"OPD node {self.name} (0x{self.addr:02X}) was found")
                     self.configure()
 
                 if reset:
                     self._max7310.reset()
                     self.configure()
 
                 self._status = OpdNodeState.DISABLED
             else:
                 if self._status != OpdNodeState.NOT_FOUND:
-                    logger.info(f"OPD node {self.name} (0x{self.addr:02X}) was lost")
+                    logger.debug(f"OPD node {self.name} (0x{self.addr:02X}) was lost")
                     self._status = OpdNodeState.NOT_FOUND
         except Max7310Error as e:
             logger.error(f"MAX7310 error: {e}")
             logger.debug(f"OPD node {self.name} (0x{self.addr:02X}) was not found")
             self._status = OpdNodeState.NOT_FOUND
 
         return self._status != OpdNodeState.NOT_FOUND
@@ -132,15 +137,15 @@
 
         Returns
         -------
         OpdNodeState
             The node state after disabling the node.
         """
 
-        logger.info(f"enabling OPD node {self.name} (0x{self.addr:02X})")
+        logger.debug(f"enabling OPD node {self.name} (0x{self.addr:02X})")
 
         if self._status == OpdNodeState.NOT_FOUND:
             return self._status  # cannot enable node that is NOT_FOUND
 
         try:
             self._max7310.output_set(self._ENABLE_PIN)
             self._status = OpdNodeState.ENABLED
@@ -155,19 +160,19 @@
 
         Returns
         -------
         OpdNodeState
             The node state after disabling the node.
         """
 
-        logger.info(f"disabling OPD node {self.name} (0x{self.addr:02X})")
+        logger.debug(f"disabling OPD node {self.name} (0x{self.addr:02X})")
 
         try:
-            self._status = OpdNodeState.DISABLED
             self._max7310.output_clear(self._ENABLE_PIN)
+            self._status = OpdNodeState.DISABLED
         except Max7310Error:
             self._status = OpdNodeState.FAULT
 
         return self._status
 
     def reset(self, attempts: int = 3) -> OpdNodeState:
         """
@@ -192,15 +197,15 @@
 
                 if self.fault:
                     self._status = OpdNodeState.FAULT
                 else:
                     self._status = OpdNodeState.ENABLED
                     break
             except Max7310Error:
-                continue
+                self._status = OpdNodeState.FAULT
 
         return self._status
 
     @property
     def name(self) -> str:
         """int: Unique name."""
 
@@ -212,40 +217,48 @@
 
         return self._addr
 
     @property
     def status(self) -> OpdNodeState:
         """OpdNodeState: Status of the OPD node."""
 
+        valid = False
+        try:
+            valid = self._max7310.is_valid
+        except Max7310Error:
+            pass
+
+        if not valid:
+            self._status = OpdNodeState.NOT_FOUND
+        elif self.is_enabled and self.fault:
+            self._status = OpdNodeState.FAULT
         return self._status
 
     @property
     def is_enabled(self) -> bool:
         """bool: The node is enabled."""
 
+        enabled = False
         try:
             enabled = self._max7310.output_status(self._ENABLE_PIN)
-        except Max7310Error as e:
+        except Max7310Error:
             if self._status != OpdNodeState.NOT_FOUND:
                 self._status = OpdNodeState.FAULT
-            raise OpdError(e) from e
-
         return enabled
 
     @property
     def fault(self) -> bool:
         """bool: The OPD fault pin has tripped."""
 
+        fault = True
         try:
             fault = not self._max7310.input_status(self._NOT_FAULT_PIN)
-        except Max7310Error as e:
+        except Max7310Error:
             if self._status != OpdNodeState.NOT_FOUND:
                 self._status = OpdNodeState.FAULT
-            raise OpdError(e) from e
-
         return fault
 
 
 class OpdStm32Node(OpdNode):
     """A STM32-based OPD Node"""
 
     _I2C_SCL_PIN = 0  # i2c bootloader
@@ -294,73 +307,111 @@
             pass
         return super().disable()
 
     def configure(self):
         """Configure the MAX7310 for the OPD node."""
 
         inputs = 1 << self._I2C_SCL_PIN | 1 << self._I2C_SDA_PIN | 1 << self._NOT_FAULT_PIN
-        self._max7310.configure(0, 0, inputs, self._TIMEOUT_CONFIG)
-        if self._mock:
-            self._max7310._mock_input_set(self._NOT_FAULT_PIN)  # pylint: disable=W0212
-        self._status = OpdNodeState.DISABLED
+        try:
+            self._max7310.configure(0, 0, inputs, self._TIMEOUT_CONFIG)
+            if self._mock:
+                self._max7310._mock_input_set(self._NOT_FAULT_PIN)  # pylint: disable=W0212
+            self._status = OpdNodeState.DISABLED
+        except Max7310Error:
+            logger.debug(f"OPD node {self.name} (0x{self.addr:02X}) was not found")
+            self._status = OpdNodeState.FAULT
 
     def enable_uart(self):
         """Connect the node the C3's UART"""
 
-        self._max7310.output_set(self._UART_PIN)
-        logger.info(f"OPD node {self.name} (0x{self.addr:02X}) was connected to UART")
+        try:
+            self._max7310.output_set(self._UART_PIN)
+            logger.debug(f"OPD node {self.name} (0x{self.addr:02X}) was connected to UART")
+        except Max7310Error:
+            self._status = OpdNodeState.FAULT
 
     def disable_uart(self):
         """Disconnect the node from the C3's UART"""
 
-        self._max7310.output_clear(self._UART_PIN)
-        logger.info(f"OPD node {self.name} (0x{self.addr:02X}) was disconnected from UART")
+        try:
+            self._max7310.output_clear(self._UART_PIN)
+            logger.debug(f"OPD node {self.name} (0x{self.addr:02X}) was disconnected from UART")
+        except Max7310Error:
+            self._status = OpdNodeState.FAULT
 
     @property
     def is_uart_enabled(self) -> bool:
         """bool: Check if the UART pin is connected"""
 
-        return self._max7310.output_status(self._UART_PIN)
+        r = False
+        try:
+            r = self._max7310.output_status(self._UART_PIN)
+        except Max7310Error:
+            self._status = OpdNodeState.FAULT
+        return r
 
     @property
     def in_bootloader_mode(self) -> bool:
         """bool: Check if the card is in bootloader mode."""
 
-        return self._max7310.output_status(self._BOOT_PIN)
+        r = False
+        try:
+            r = self._max7310.output_status(self._BOOT_PIN)
+        except Max7310Error:
+            self._status = OpdNodeState.FAULT
+        return r
 
 
 class OpdOctavoNode(OpdNode):
     """A Octavo A8-based OPD Node"""
 
     _SYS_BOOT2 = 0
     _UART_PIN = 7  # connect to C3 UART
 
     def enable(self) -> OpdNodeState:
         """Enable the node"""
 
-        self._max7310.output_set(self._SYS_BOOT2)
-        return super().enable()
+        try:
+            self._max7310.output_set(self._SYS_BOOT2)
+            r = super().enable()
+        except Max7310Error:
+            r = OpdNodeState.FAULT
+        self._status = r
+        return self._status
 
     def enable_uart(self):
         """Connect the node the C3's UART"""
 
-        self._max7310.output_set(self._UART_PIN)
-        logger.info(f"OPD node {self.name} (0x{self.addr:02X}) was connected to UART")
+        try:
+            self._max7310.output_set(self._UART_PIN)
+            logger.debug(f"OPD node {self.name} (0x{self.addr:02X}) was connected to UART")
+        except Max7310Error:
+            self._status = OpdNodeState.FAULT
+        return self._status
 
     def disable_uart(self):
         """Disconnect the node the C3's UART"""
 
-        self._max7310.output_clear(self._UART_PIN)
-        logger.info(f"OPD node {self.name} (0x{self.addr:02X}) was disconnected from UART")
+        try:
+            self._max7310.output_clear(self._UART_PIN)
+            logger.debug(f"OPD node {self.name} (0x{self.addr:02X}) was disconnected from UART")
+        except Max7310Error:
+            self._status = OpdNodeState.FAULT
+        return self._status
 
     @property
     def is_uart_enabled(self) -> bool:
         """bool: Check if the UART pin is connected"""
 
-        return self._max7310.output_status(self._UART_PIN)
+        r = False
+        try:
+            r = self._max7310.output_status(self._UART_PIN)
+        except Max7310Error:
+            self._status = OpdNodeState.FAULT
+        return r
 
 
 class OpdState(IntEnum):
     """OPD subsystem states."""
 
     DISABLED = 0x0
     """OPD subsystem is off."""
```

### Comparing `oresat_c3-0.4.0/oresat_c3/subsystems/rtc.py` & `oresat_c3-0.5.0/oresat_c3/subsystems/rtc.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/oresat_c3/templates/keys.html` & `oresat_c3-0.5.0/oresat_c3/templates/keys.html`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/oresat_c3/templates/node_manager.html` & `oresat_c3-0.5.0/oresat_c3/templates/node_manager.html`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/oresat_c3/templates/state.html` & `oresat_c3-0.5.0/oresat_c3/templates/state.html`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/oresat_c3.egg-info/PKG-INFO` & `oresat_c3-0.5.0/oresat_c3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-c3
-Version: 0.4.0
+Version: 0.5.0
 Summary: OreSat C3 OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oresat_c3-0.4.0/oresat_c3.egg-info/SOURCES.txt` & `oresat_c3-0.5.0/oresat_c3.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 oresat_c3.egg-info/top_level.txt
 oresat_c3/drivers/__init__.py
 oresat_c3/drivers/fm24cl64b.py
 oresat_c3/drivers/max7310.py
 oresat_c3/drivers/si41xx.py
 oresat_c3/protocols/__init__.py
 oresat_c3/protocols/ax25.py
+oresat_c3/protocols/cachestore.py
+oresat_c3/protocols/cfdp.py
 oresat_c3/protocols/edl_command.py
 oresat_c3/protocols/edl_packet.py
 oresat_c3/services/__init__.py
 oresat_c3/services/beacon.py
 oresat_c3/services/edl.py
 oresat_c3/services/node_manager.py
 oresat_c3/services/radios.py
@@ -53,13 +55,14 @@
 scripts/edl_ping_loop.py
 tests/__init__.py
 tests/drivers/__init__.py
 tests/drivers/test_fm23cl64b.py
 tests/drivers/test_max7310.py
 tests/protocols/__init__.py
 tests/protocols/test_ax25.py
+tests/protocols/test_cachestore.py
 tests/protocols/test_edl_command.py
 tests/protocols/test_edl_packet.py
 tests/services/__init__.py
 tests/services/test_state.py
 tests/subsystems/__init__.py
 tests/subsystems/test_opd.py
```

### Comparing `oresat_c3-0.4.0/pyproject.toml` & `oresat_c3-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 write_to = "oresat_c3/_version.py"
 
 [tool.black]
 line_length = 100
 
 [tool.pylama]
 format = "pylint"
-skip = "*/.tox/*,*/.env/,*/.git/*,*/.github/*,*/build/*"
+skip = "*/.tox/*,*/.env/,*/.git/*,*/.github/*,*/build/*,.direnv/*"
 linters = "pycodestyle,pyflakes,pylint,mccabe,mypy,radon"
 # E402:     Module level import not at top of file
 # C901:     Function is too complex
 # C0103:    Arguments are not snake_case naming style or too short
 # E203:     Whitespace before ':' (black does this)
 # R0912:    Too many branches
 # R0915:    Too many statements
```

### Comparing `oresat_c3-0.4.0/scripts/edl_cmd_shell.py` & `oresat_c3-0.5.0/scripts/edl_cmd_shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,15 @@
         print("  <enable> is 0, 1, true, false")
 
     def do_opd_enable(self, arg: str):
         """Do the opd_enable command."""
 
         args = arg.split(" ")
         if len(args) != 2:
-            self.help_opd_sysenable()
+            self.help_opd_enable()
             return
 
         if args[0].startswith("0x"):
             opd_addr = int(args[0], 16)
         else:
             opd_addr = 0
             for name, card in self.configs.cards.items():
```

### Comparing `oresat_c3-0.4.0/scripts/edl_file_upload.py` & `oresat_c3-0.5.0/scripts/edl_file_upload.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 
 import os
 import random
 import signal
 import socket
 import sys
 import time
+import traceback
 from argparse import ArgumentParser
 from datetime import timedelta
 from pathlib import Path
 from queue import Empty, SimpleQueue
 from threading import Lock, Thread
 from typing import Any
 
 from cfdppy import CfdpState, PacketDestination, get_packet_destination
+from cfdppy.exceptions import NoRemoteEntityCfgFound
 from cfdppy.handler.dest import DestHandler
 from cfdppy.handler.source import SourceHandler
 from cfdppy.mib import (
     CheckTimerProvider,
     DefaultFaultHandlerBase,
     IndicationCfg,
     LocalEntityCfg,
@@ -35,15 +37,20 @@
     TransactionFinishedParams,
     TransactionId,
     TransactionParams,
 )
 from olaf import OreSatFile
 from spacepackets.cfdp import CfdpLv
 from spacepackets.cfdp.defs import ChecksumType, ConditionCode, TransmissionMode
-from spacepackets.cfdp.tlv import ProxyPutRequest, ProxyPutRequestParams
+from spacepackets.cfdp.tlv import (
+    DirectoryListingRequest,
+    DirectoryParams,
+    ProxyPutRequest,
+    ProxyPutRequestParams,
+)
 from spacepackets.countdown import Countdown
 from spacepackets.seqcount import SeqCountProvider
 from spacepackets.util import ByteFieldU8
 
 from oresat_c3.protocols.edl_packet import SRC_DEST_ORESAT, EdlPacket
 
 sys.path.insert(0, os.path.abspath(".."))
@@ -125,14 +132,15 @@
     def run(self):
         uplink = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         uplink.connect(self._address)
 
         while True:
             payload = self.queue.get()
             if self._bad_connection and not random.randrange(5):
+                print("---X DROPPED", payload)
                 continue  # simulate dropped packets
             print("--->", payload)
             packet = EdlPacket(payload, self._sequence_number, SRC_DEST_ORESAT)
             message = packet.pack(self._hmac_key)
             uplink.send(message)
             self._sequence_number += 1
             time.sleep(self._delay)
@@ -155,17 +163,18 @@
 
     def run(self):
         downlink = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         downlink.bind(self._address)
 
         while True:
             message = downlink.recv(4096)
+            packet = EdlPacket.unpack(message, self._hmac_key, True).payload
             if self._bad_connection and not random.randrange(5):
+                print("X--- DROPPED", packet)
                 continue  # simulate dropped packets
-            packet = EdlPacket.unpack(message, self._hmac_key, True).payload
             print("<---", packet)
 
             if get_packet_destination(packet) == PacketDestination.DEST_HANDLER:
                 self.dest_queue.put(packet)
             else:
                 self.source_queue.put(packet)
 
@@ -198,15 +207,19 @@
         )
 
         self.lock = Lock()
 
     def run(self):
         while packet := self.downlink.get():
             with self.lock:
-                self.src.insert_packet(packet)
+                try:
+                    self.src.insert_packet(packet)
+                except NoRemoteEntityCfgFound as e:
+                    print(e)
+                    traceback.print_exc()
                 self.src.state_machine()
                 while self.src.packets_ready:
                     pdu = self.src.get_next_packet().pdu
                     self.uplink.put(pdu)
 
     def send_packets(self, put):
         """Sends a PutRequest to the uplink and handles respones.
@@ -255,14 +268,64 @@
                 time.sleep(0.1)
             self.dest.state_machine()
             while self.dest.packets_ready:
                 pdu = self.dest.get_next_packet().pdu
                 self.uplink.put(pdu)
 
 
+def put_request(dest: ByteFieldU8, file_path: str) -> PutRequest:
+    """Creates a simple PutRequest for the file in file_path"""
+    return PutRequest(
+        destination_id=dest,
+        source_file=Path(file_path),
+        dest_file=Path(file_path),
+        trans_mode=None,
+        closure_requested=None,
+    )
+
+
+def proxy_put_request(dest: ByteFieldU8, source: ByteFieldU8, file_path: str) -> PutRequest:
+    """Creates a put request for file_path to be transfered to the cfdp entity in dest"""
+    return PutRequest(
+        destination_id=dest,
+        source_file=None,
+        dest_file=None,
+        trans_mode=None,
+        # FIXME: upstream bug - DestHandler does not respect closure_requested=None when
+        # trans_mode defaults to ACKNOWLEGED
+        closure_requested=True,
+        msgs_to_user=[
+            ProxyPutRequest(
+                ProxyPutRequestParams(
+                    source,
+                    source_file_name=CfdpLv(file_path.encode()),
+                    dest_file_name=CfdpLv(file_path.encode()),
+                )
+            ).to_generic_msg_to_user_tlv()
+        ],
+    )
+
+
+def directory_listing(dest: ByteFieldU8, path: str, result: str) -> PutRequest:
+    """Creates a directory listing put request"""
+    # CFDP 6.3.3
+    return PutRequest(
+        destination_id=dest,
+        source_file=None,
+        dest_file=None,
+        trans_mode=None,
+        closure_requested=True,
+        msgs_to_user=[
+            DirectoryListingRequest(
+                DirectoryParams.from_strs(path, result)
+            ).to_generic_msg_to_user_tlv()
+        ],
+    )
+
+
 def main():
     """Upload a file to the satellite."""
     parser = ArgumentParser()
     parser.add_argument("file_path")
     parser.add_argument(
         "-o", "--host", default="localhost", help="address to use, default is localhost"
     )
@@ -303,20 +366,23 @@
     parser.add_argument("-s", "--buffer-size", type=int, default=950, help="file data buffer size")
     parser.add_argument(
         "-m",
         "--hmac",
         default="",
         help="edl hmac, must be 32 bytes, default all zero",
     )
-    parser.add_argument(
+    command = parser.add_mutually_exclusive_group()
+    command.add_argument(
         "-p",
         "--proxy",
         action="store_true",
         help="Initiate a proxy put request instead of a normal one",
     )
+    command.add_argument("-dr", "--directory", help="Request a directory listing, for example '.'")
+
     args = parser.parse_args()
 
     file_path = args.file_path.split("/")[-1]
     try:
         OreSatFile(file_path)
     except ValueError:
         print("file name must be in card-name_key_unix-time.extension format")
@@ -372,40 +438,18 @@
 
     source = Source(up.queue, down.source_queue, localcfg, remote_entities)
     source.start()
     dest = Dest(up.queue, down.dest_queue, localcfg, remote_entities)
     dest.start()
 
     if args.proxy:
-        put = PutRequest(
-            destination_id=DEST_ID,
-            source_file=None,
-            dest_file=None,
-            trans_mode=None,
-            # FIXME: upstream bug - DestHandler does not respect closure_requested=None when
-            # trans_mode defaults to ACKNOWLEGED
-            closure_requested=True,
-            msgs_to_user=[
-                ProxyPutRequest(
-                    ProxyPutRequestParams(
-                        SOURCE_ID,
-                        source_file_name=CfdpLv(args.file_path.encode()),
-                        dest_file_name=CfdpLv(args.file_path.encode()),
-                    )
-                ).to_generic_msg_to_user_tlv()
-            ],
-        )
+        put = proxy_put_request(DEST_ID, SOURCE_ID, args.file_path)
+    elif args.directory:
+        put = directory_listing(DEST_ID, args.directory, args.file_path)
     else:
-        put = PutRequest(
-            destination_id=DEST_ID,
-            source_file=Path(args.file_path),
-            dest_file=Path(args.file_path),
-            trans_mode=None,
-            closure_requested=None,
-        )
-
+        put = put_request(DEST_ID, args.file_path)
     source.send_packets(put)
     signal.pause()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `oresat_c3-0.4.0/scripts/edl_ping_loop.py` & `oresat_c3-0.5.0/scripts/edl_ping_loop.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/tests/drivers/test_fm23cl64b.py` & `oresat_c3-0.5.0/tests/drivers/test_fm23cl64b.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/tests/drivers/test_max7310.py` & `oresat_c3-0.5.0/tests/drivers/test_max7310.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/tests/protocols/test_ax25.py` & `oresat_c3-0.5.0/tests/protocols/test_ax25.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/tests/protocols/test_edl_command.py` & `oresat_c3-0.5.0/tests/protocols/test_edl_command.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/tests/protocols/test_edl_packet.py` & `oresat_c3-0.5.0/tests/protocols/test_edl_packet.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/tests/services/test_state.py` & `oresat_c3-0.5.0/tests/services/test_state.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.4.0/tests/subsystems/test_opd.py` & `oresat_c3-0.5.0/tests/subsystems/test_opd.py`

 * *Files identical despite different names*

