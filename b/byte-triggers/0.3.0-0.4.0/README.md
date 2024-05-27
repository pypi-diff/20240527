# Comparing `tmp/byte_triggers-0.3.0.tar.gz` & `tmp/byte_triggers-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byte_triggers-0.3.0.tar", last modified: Wed Apr  3 14:29:28 2024, max compression
+gzip compressed data, was "byte_triggers-0.4.0.tar", last modified: Mon May 27 14:58:46 2024, max compression
```

## Comparing `byte_triggers-0.3.0.tar` & `byte_triggers-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:29:28.240423 byte_triggers-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-03 14:29:28.240423 byte_triggers-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:29:28.232423 byte_triggers-0.3.0/byte_triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:29:28.232423 byte_triggers-0.3.0/byte_triggers/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/commands/sys_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:29:28.236423 byte_triggers-0.3.0/byte_triggers/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/io/_dlportio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/io/_inpout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/io/_linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/lsl.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)    10074 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:29:28.236423 byte_triggers-0.3.0/byte_triggers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/utils/_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/utils/_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/utils/_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/utils/_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/utils/_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/utils/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:29:28.236423 byte_triggers-0.3.0/byte_triggers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-03 14:29:28.000000 byte_triggers-0.3.0/byte_triggers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-03 14:29:28.000000 byte_triggers-0.3.0/byte_triggers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:29:28.000000 byte_triggers-0.3.0/byte_triggers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 14:29:28.000000 byte_triggers-0.3.0/byte_triggers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-03 14:29:28.000000 byte_triggers-0.3.0/byte_triggers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 14:29:28.000000 byte_triggers-0.3.0/byte_triggers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:29:28.240423 byte_triggers-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:58:46.726009 byte_triggers-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-27 14:58:46.726009 byte_triggers-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:58:46.722009 byte_triggers-0.4.0/byte_triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:58:46.722009 byte_triggers-0.4.0/byte_triggers/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/commands/sys_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:58:46.722009 byte_triggers-0.4.0/byte_triggers/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/io/_dlportio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/io/_inpout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/io/_linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/lsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:58:46.726009 byte_triggers-0.4.0/byte_triggers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/utils/_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/utils/_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/utils/_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/utils/_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/byte_triggers/utils/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:58:46.726009 byte_triggers-0.4.0/byte_triggers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-27 14:58:46.000000 byte_triggers-0.4.0/byte_triggers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-27 14:58:46.000000 byte_triggers-0.4.0/byte_triggers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:58:46.000000 byte_triggers-0.4.0/byte_triggers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 14:58:46.000000 byte_triggers-0.4.0/byte_triggers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-27 14:58:46.000000 byte_triggers-0.4.0/byte_triggers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 14:58:46.000000 byte_triggers-0.4.0/byte_triggers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-27 14:58:08.000000 byte_triggers-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:58:46.726009 byte_triggers-0.4.0/setup.cfg
```

### Comparing `byte_triggers-0.3.0/LICENSE` & `byte_triggers-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.3.0/PKG-INFO` & `byte_triggers-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byte_triggers
-Version: 0.3.0
+Version: 0.4.0
 Summary: Provides byte (0 to 255) triggers on serial/parallel ports and on LSL streams.
 Author-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 Maintainer-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 License: MIT License
         
         Copyright (c) 2022 Mathieu Scheltienne
         
@@ -23,71 +23,70 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: documentation, https://fcbg-hnp-meeg.github.io/byte-triggers
-Project-URL: homepage, https://fcbg-hnp-meeg.github.io/byte-triggers
 Project-URL: source, https://github.com/fcbg-hnp-meeg/byte-triggers
 Project-URL: tracker, https://github.com/fcbg-hnp-meeg/byte-triggers/issues
-Keywords: parallel,python,serial,triggers
+Keywords: events,lsl,parallel,python,serial,triggers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mne_lsl
-Requires-Dist: numpy>=1.21
+Requires-Dist: mne_lsl>=1.3.1
+Requires-Dist: numpy>=1.26.4
 Requires-Dist: packaging
 Requires-Dist: psutil
 Requires-Dist: pyparallel; sys_platform == "linux"
 Requires-Dist: pyserial
 Provides-Extra: all
 Requires-Dist: byte_triggers[build]; extra == "all"
 Requires-Dist: byte_triggers[doc]; extra == "all"
 Requires-Dist: byte_triggers[style]; extra == "all"
 Requires-Dist: byte_triggers[test]; extra == "all"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
 Provides-Extra: doc
 Requires-Dist: furo; extra == "doc"
+Requires-Dist: intersphinx_registry; extra == "doc"
 Requires-Dist: matplotlib; extra == "doc"
 Requires-Dist: memory-profiler; extra == "doc"
 Requires-Dist: numpydoc; extra == "doc"
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx-copybutton; extra == "doc"
 Requires-Dist: sphinx-design; extra == "doc"
 Requires-Dist: sphinx-issues; extra == "doc"
 Requires-Dist: sphinx-remove-toctrees; extra == "doc"
 Requires-Dist: sphinxcontrib-bibtex; extra == "doc"
 Provides-Extra: full
 Requires-Dist: byte_triggers[all]; extra == "full"
 Provides-Extra: style
 Requires-Dist: bibclean; extra == "style"
-Requires-Dist: black; extra == "style"
-Requires-Dist: codespell; extra == "style"
+Requires-Dist: codespell[toml]>=2.2.4; extra == "style"
 Requires-Dist: isort; extra == "style"
 Requires-Dist: pydocstyle[toml]; extra == "style"
-Requires-Dist: ruff; extra == "style"
+Requires-Dist: ruff>=0.1.8; extra == "style"
 Requires-Dist: toml-sort; extra == "style"
 Requires-Dist: yamllint; extra == "style"
 Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-timeout; extra == "test"
+Requires-Dist: pytest>=8.0; extra == "test"
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![codecov](https://codecov.io/gh/fcbg-hnp-meeg/byte-triggers/graph/badge.svg?token=rSGaJehUMl)](https://codecov.io/gh/fcbg-hnp-meeg/byte-triggers)
 [![tests](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/pytest.yml)
 [![doc](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/doc.yml/badge.svg?branch=main)](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/doc.yml)
```

### Comparing `byte_triggers-0.3.0/README.md` & `byte_triggers-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.3.0/byte_triggers/_base.py` & `byte_triggers-0.4.0/byte_triggers/_base.py`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.3.0/byte_triggers/io/__init__.py` & `byte_triggers-0.4.0/byte_triggers/io/__init__.py`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.3.0/byte_triggers/io/_dlportio.py` & `byte_triggers-0.4.0/byte_triggers/io/_dlportio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 # This code is heavily based upon winioport.py
 # Provides hardware port access for Python under Windows 95/98/NT/2000
 #
 # Original Author: Dincer Aydin dinceraydin@gmx.net www.dinceraydin.com
 # Merged directly into psychopy by: Mark Hymers <mark.hymers@ynic.york.ac.uk>
 # All bugs are Mark's fault.
```

### Comparing `byte_triggers-0.3.0/byte_triggers/io/_inpout.py` & `byte_triggers-0.4.0/byte_triggers/io/_inpout.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 # We deliberately delay importing the inpout32 or inpoutx64 module until we try
 # to use it - this allows us to import the class on machines
 # which don't have it and then worry about dealing with
 # using the right one later
 
 
@@ -30,17 +29,17 @@
         if isinstance(address, str) and address.startswith("0x"):
             # convert u"0x0378" into 0x0378
             self.base = int(address, 16)
         else:
             self.base = address
 
         if platform.architecture()[0] == "32bit":
-            self.port = getattr(windll, "inpout32")
+            self.port = windll.inpout32
         elif platform.architecture()[0] == "64bit":
-            self.port = getattr(windll, "inpoutx64")
+            self.port = windll.inpoutx64
 
         BYTEMODEMASK = uint8(1 << 5 | 1 << 6 | 1 << 7)
 
         # Put the port into Byte Mode (ECP register)
         _inp = self.port.Inp32(self.base + 0x402)
         self.port.Out32(self.base + 0x402, int((_inp & ~BYTEMODEMASK) | (1 << 5)))
```

### Comparing `byte_triggers-0.3.0/byte_triggers/io/_linux.py` & `byte_triggers-0.4.0/byte_triggers/io/_linux.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 # We deliberately delay importing the pyparallel module until we try
 # to use it - this allows us to import the class on machines
 # which don't have it and then worry about dealing with
 # using the right one later
 
 # This is necessary to stop the local parallel.py masking the module
```

### Comparing `byte_triggers-0.3.0/byte_triggers/lsl.py` & `byte_triggers-0.4.0/byte_triggers/lsl.py`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.3.0/byte_triggers/parallel.py` & `byte_triggers-0.4.0/byte_triggers/parallel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Trigger using an parallel port."""
 
-import threading
 import time
+from concurrent.futures import ThreadPoolExecutor
 from platform import system
 from typing import Optional, Union
-from warnings import warn
 
 from ._base import BaseTrigger
 from .utils._checks import check_type, check_value, ensure_int
 from .utils._docs import copy_doc
 from .utils._imports import import_optional_dependency
 from .utils.logs import logger
 
@@ -43,27 +42,21 @@
     - On Windows::
 
           LPT1 = 0x0378 or 0x03BC
           LPT2 = 0x0278 or 0x0378
           LPT3 = 0x0278
 
     - macOS does not have support for built-in parallel ports.
-
-    .. warning::
-
-        On Linux, the arduino to parallel-port converter works reliably for ~10 minutes
-        after which some sort of overflow occurs and impacts negatively the timing of
-        the triggers. Use at your own discretion.
     """
 
     def __init__(
         self,
         address: Union[int, str],
         port_type: Optional[str] = None,
-        delay: int = 50,
+        delay: int = 10,
     ):
         check_type(address, ("int-like", str), "address")
         if not isinstance(address, str):
             address = ensure_int(address)
         delay = ensure_int(delay, "delay")
         self._delay = delay / 1000.0
         if port_type is None:
@@ -71,22 +64,14 @@
         else:
             check_type(port_type, (str,), "port_type")
             check_value(port_type, ("arduino", "pport"), "port_type")
             self._port_type = port_type
 
         # initialize port
         if self._port_type == "arduino":
-            if system() == "Linux":
-                warn(
-                    "On Linux, the arduino to parallel-port converter works reliably "
-                    "for ~10 minutes, after which some sort of overflow occurs and "
-                    "impacts negatively the timing of the triggers. Use at your own "
-                    "discretion.",
-                    RuntimeWarning,
-                )
             import_optional_dependency(
                 "serial", extra="Install 'pyserial' for ARDUINO support."
             )
             if address == "arduino":
                 self._address = ParallelPortTrigger._search_arduino()
             else:
                 self._address = address
@@ -96,16 +81,18 @@
             if system() == "Linux":
                 import_optional_dependency(
                     "parallel",
                     extra="Install 'pyparallel' for LPT support on Linux.",
                 )
             self._address = address
             self._connect_pport()
-
-        self._signal_off()  # set pins to 0 and define self._offtimer
+        # set pins to 0 and prepare threadpool for resets
+        self._set_data(0)
+        self._executor = ThreadPoolExecutor(max_workers=1)
+        self._future = None
 
     @staticmethod
     def _infer_port_type(address: Union[int, str]) -> str:
         """Infer the type of port from the address."""
         if system() == "Linux":
             if not isinstance(address, str):
                 raise TypeError(
@@ -146,15 +133,15 @@
         """Look for a connected Arduino to LPT converter."""
         from serial.tools import list_ports
 
         for arduino in list_ports.grep(regexp="Arduino"):
             logger.info("Found arduino to LPT on '%s'.", arduino)
             return arduino.device
         else:
-            raise IOError("No arduino card was found.")
+            raise OSError("No arduino card was found.")
 
     def _connect_arduino(self, baud_rate: int = 115200) -> None:
         """Connect to an Arduino to LPT converter."""
         from serial import Serial, SerialException
 
         try:
             self._port = Serial(self._address, baud_rate)
@@ -204,57 +191,53 @@
 
         time.sleep(1)
         logger.info("Connected to parallel port on '%s'.", self._address)
 
     @copy_doc(BaseTrigger.signal)
     def signal(self, value: int) -> None:
         value = super().signal(value)
-        if self._offtimer.is_alive():
+        if self._future is not None and not self._future.done():
             logger.warning(
                 "You are sending a new signal before the end of the "
                 "last signal. Signal ignored. Delay required = %.1f ms.",
                 self.delay,
             )
-        else:
-            self._set_data(value)
-            self._offtimer.start()
+        self._set_data(value)
+        self._future = self._executor.submit(self._signal_off())
 
     def _signal_off(self) -> None:
-        """Reset trigger signal to 0 and reset offtimer.
-
-        The offtimer reset is required because threads are one-call only.
-        """
+        """Reset trigger signal to 0."""
+        time.sleep(self._delay)
         self._set_data(0)
-        self._offtimer = threading.Timer(self._delay, self._signal_off)
 
     def _set_data(self, value: int) -> None:
         """Set data on the pin."""
         if self._port_type == "arduino":
             self._port.write(bytes([value]))
         else:
             self._port.setData(value)
 
     def close(self) -> None:
         """Disconnect the parallel port.
 
-        This method should free the parallel or serial port and let other
-        application or python process use it.
+        This method should free the parallel or serial port and let other application or
+        python process use it.
         """
         if hasattr(self, "_port_type") and self._port_type == "arduino":
             try:
                 self._port.close()
             except Exception:
                 pass
         if hasattr(self, "_port"):
             try:
                 del self._port
             except Exception:
                 pass
 
-    def __del__(self):  # noqa: D105
+    def __del__(self) -> None:  # noqa: D105
         self.close()
 
     # --------------------------------------------------------------------
     @property
     def address(self) -> Union[int, str]:
         """The address of the parallel port on the system.
```

### Comparing `byte_triggers-0.3.0/byte_triggers/utils/_checks.py` & `byte_triggers-0.4.0/byte_triggers/utils/_checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 from ._docs import fill_doc
 
 if TYPE_CHECKING:
-    from typing import Any, Optional
+    from typing import Any, Optional, Union
 
 
 def ensure_int(item: Any, item_name: Optional[str] = None) -> int:
     """Ensure a variable is an integer.
 
     Parameters
     ----------
@@ -36,15 +36,15 @@
     try:
         # someone passing True/False is much more likely to be an error than
         # intentional usage
         if isinstance(item, bool):
             raise TypeError
         item = int(operator.index(item))
     except TypeError:
-        item_name = "Item" if item_name is None else "'%s'" % item_name
+        item_name = "Item" if item_name is None else f"'{item_name}'"
         raise TypeError(f"{item_name} must be an integer, got {type(item)} instead.")
 
     return item
 
 
 class _IntLike:
     @classmethod
@@ -92,81 +92,85 @@
         When the type of the item is not one of the valid options.
     """
     check_types = sum(
         (
             (
                 (type(None),)
                 if type_ is None
-                else (type_,) if not isinstance(type_, str) else _types[type_]
+                else (type_,)
+                if not isinstance(type_, str)
+                else _types[type_]
             )
             for type_ in types
         ),
         (),
     )
 
     if not isinstance(item, check_types):
         type_name = [
             (
                 "None"
                 if cls_ is None
-                else cls_.__name__ if not isinstance(cls_, str) else cls_
+                else cls_.__name__
+                if not isinstance(cls_, str)
+                else cls_
             )
             for cls_ in types
         ]
         if len(type_name) == 1:
             type_name = type_name[0]
         elif len(type_name) == 2:
             type_name = " or ".join(type_name)
         else:
             type_name[-1] = "or " + type_name[-1]
             type_name = ", ".join(type_name)
-        item_name = "Item" if item_name is None else "'%s'" % item_name
+        item_name = "Item" if item_name is None else f"'{item_name}'"
         raise TypeError(
             f"{item_name} must be an instance of {type_name}, got {type(item)} instead."
         )
 
 
 def check_value(
     item: Any,
-    allowed_values: tuple,
+    allowed_values: Union[tuple, dict[Any, Any]],
     item_name: Optional[str] = None,
     extra: Optional[str] = None,
 ) -> None:
     """Check the value of a parameter against a list of valid options.
 
     Parameters
     ----------
     item : object
         Item to check.
-    allowed_values : tuple of objects
-        Allowed values to be checked against.
+    allowed_values : tuple of objects | dict of objects
+        Allowed values to be checked against. If a dictionary, checks against the keys.
     item_name : str | None
         Name of the item to show inside the error message.
     extra : str | None
         Extra string to append to the invalid value sentence, e.g. "when using DC mode".
 
     Raises
     ------
     ValueError
         When the value of the item is not one of the valid options.
     """
     if item not in allowed_values:
-        item_name = "" if item_name is None else " '%s'" % item_name
+        item_name = "" if item_name is None else f" '{item_name}'"
         extra = "" if extra is None else " " + extra
         msg = (
             "Invalid value for the{item_name} parameter{extra}. "
             "{options}, but got {item!r} instead."
         )
         allowed_values = tuple(allowed_values)  # e.g., if a dict was given
         if len(allowed_values) == 1:
-            options = "The only allowed value is %s" % repr(allowed_values[0])
+            options = f"The only allowed value is {repr(allowed_values[0])}"
         elif len(allowed_values) == 2:
-            options = "Allowed values are %s and %s" % (
-                repr(allowed_values[0]),
-                repr(allowed_values[1]),
+            options = (
+                f"Allowed values are {repr(allowed_values[0])} "
+                f"and {repr(allowed_values[1])}"
             )
         else:
             options = "Allowed values are "
             options += ", ".join([f"{repr(v)}" for v in allowed_values[:-1]])
             options += f", and {repr(allowed_values[-1])}"
         raise ValueError(
             msg.format(item_name=item_name, extra=extra, options=options, item=item)
```

### Comparing `byte_triggers-0.3.0/byte_triggers/utils/_fixes.py` & `byte_triggers-0.4.0/byte_triggers/utils/_fixes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """Temporary bug-fixes awaiting an upstream fix."""
 
+from __future__ import annotations  # c.f. PEP 563, PEP 649
+
 import sys
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Any
 
 
 # https://github.com/sphinx-gallery/sphinx-gallery/issues/1112
-class WrapStdOut(object):
+class WrapStdOut:
     """Dynamically wrap to sys.stdout.
 
     This makes packages that monkey-patch sys.stdout (e.g.doctest, sphinx-gallery) work
     properly.
     """
 
-    def __getattr__(self, name: str):  # noqa: D105
+    def __getattr__(self, name: str) -> Any:  # noqa: D105
         # Even more ridiculous than this class, this must be sys.stdout (not
         # just stdout) in order for this to work (tested on OSX and Linux).
         if hasattr(sys.stdout, name):
             return getattr(sys.stdout, name)
         else:
             raise AttributeError(f"'file' object has not attribute '{name}'.")
```

### Comparing `byte_triggers-0.3.0/byte_triggers/utils/_imports.py` & `byte_triggers-0.4.0/byte_triggers/utils/_imports.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 """Handle optional dependency imports.
 
 Inspired from pandas: https://pandas.pydata.org/
 """
 
+from __future__ import annotations  # c.f. PEP 563, PEP 649
+
 import importlib
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from types import ModuleType
+    from typing import Optional
 
 # A mapping from import name to package name (on PyPI) when the package name
 # is different.
-INSTALL_MAPPING = {
+_INSTALL_MAPPING: dict[str, str] = {
     "codespell_lib": "codespell",
     "cv2": "opencv-python",
     "parallel": "pyparallel",
     "pytest_cov": "pytest-cov",
     "serial": "pyserial",
     "sklearn": "scikit-learn",
     "sksparse": "scikit-sparse",
 }
 
 
 def import_optional_dependency(
     name: str,
     extra: str = "",
     raise_error: bool = True,
-):
+) -> Optional[ModuleType]:
     """Import an optional dependency.
 
     By default, if a dependency is missing an ImportError with a nice message will be
     raised.
 
     Parameters
     ----------
@@ -37,19 +44,19 @@
     raise_error : bool
         What to do when a dependency is not found.
         * True : Raise an ImportError.
         * False: Return None.
 
     Returns
     -------
-    module : Optional[ModuleType]
+    module : Module | None
         The imported module when found.
         None is returned when the package is not found and raise_error is False.
     """
-    package_name = INSTALL_MAPPING.get(name)
+    package_name = _INSTALL_MAPPING.get(name)
     install_name = package_name if package_name is not None else name
 
     try:
         module = importlib.import_module(name)
     except ImportError:
         if raise_error:
             raise ImportError(
```

### Comparing `byte_triggers-0.3.0/byte_triggers/utils/config.py` & `byte_triggers-0.4.0/byte_triggers/utils/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations  # c.f. PEP 563, PEP 649
 
 import platform
 import sys
-from functools import partial
+from functools import lru_cache, partial
 from importlib.metadata import requires, version
 from typing import TYPE_CHECKING
 
 import psutil
 from packaging.requirements import Requirement
 
 from ._checks import check_type
 
 if TYPE_CHECKING:
-    from typing import IO, Callable, List, Optional
+    from typing import IO, Callable, Optional
 
 
 def sys_info(fid: Optional[IO] = None, developer: bool = False):
     """Print the system information for debugging.
 
     Parameters
     ----------
@@ -72,22 +72,22 @@
             if len(extra_dependencies) == 0:
                 continue
             out(f"\nOptional '{key}' dependencies\n")
             _list_dependencies_info(out, ljust, package, extra_dependencies)
 
 
 def _list_dependencies_info(
-    out: Callable, ljust: int, package: str, dependencies: List[Requirement]
-):
+    out: Callable, ljust: int, package: str, dependencies: list[Requirement]
+) -> None:
     """List dependencies names and versions."""
     unicode = sys.stdout.encoding.lower().startswith("utf")
     if unicode:
         ljust += 1
 
-    not_found: List[Requirement] = list()
+    not_found: list[Requirement] = list()
     for dep in dependencies:
         if dep.name == package:
             continue
         try:
             version_ = version(dep.name)
         except Exception:
             not_found.append(dep)
@@ -107,14 +107,20 @@
                 from matplotlib import pyplot as plt
 
                 backend = plt.get_backend()
             except Exception:
                 backend = "Not found"
 
             output += f" (backend: {backend})"
+        if dep.name == "pyvista":
+            version_, renderer = _get_gpu_info()
+            if version_ is None:
+                output += " (OpenGL unavailable)"
+            else:
+                output += f" (OpenGL {version_} via {renderer})"
         out(output + "\n")
 
     if len(not_found) != 0:
         not_found = [
             (
                 f"{dep.name} ({str(dep.specifier)})"
                 if len(dep.specifier) != 0
@@ -122,7 +128,19 @@
             )
             for dep in not_found
         ]
         if unicode:
             out(f"✘ Not installed: {', '.join(not_found)}\n")
         else:
             out(f"Not installed: {', '.join(not_found)}\n")
+
+
+@lru_cache(maxsize=1)
+def _get_gpu_info() -> tuple[Optional[str], Optional[str]]:
+    """Get the GPU information."""
+    try:
+        from pyvista import GPUInfo
+
+        gi = GPUInfo()
+        return gi.version, gi.renderer
+    except Exception:
+        return None, None
```

### Comparing `byte_triggers-0.3.0/byte_triggers.egg-info/PKG-INFO` & `byte_triggers-0.4.0/byte_triggers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byte_triggers
-Version: 0.3.0
+Version: 0.4.0
 Summary: Provides byte (0 to 255) triggers on serial/parallel ports and on LSL streams.
 Author-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 Maintainer-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 License: MIT License
         
         Copyright (c) 2022 Mathieu Scheltienne
         
@@ -23,71 +23,70 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: documentation, https://fcbg-hnp-meeg.github.io/byte-triggers
-Project-URL: homepage, https://fcbg-hnp-meeg.github.io/byte-triggers
 Project-URL: source, https://github.com/fcbg-hnp-meeg/byte-triggers
 Project-URL: tracker, https://github.com/fcbg-hnp-meeg/byte-triggers/issues
-Keywords: parallel,python,serial,triggers
+Keywords: events,lsl,parallel,python,serial,triggers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mne_lsl
-Requires-Dist: numpy>=1.21
+Requires-Dist: mne_lsl>=1.3.1
+Requires-Dist: numpy>=1.26.4
 Requires-Dist: packaging
 Requires-Dist: psutil
 Requires-Dist: pyparallel; sys_platform == "linux"
 Requires-Dist: pyserial
 Provides-Extra: all
 Requires-Dist: byte_triggers[build]; extra == "all"
 Requires-Dist: byte_triggers[doc]; extra == "all"
 Requires-Dist: byte_triggers[style]; extra == "all"
 Requires-Dist: byte_triggers[test]; extra == "all"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
 Provides-Extra: doc
 Requires-Dist: furo; extra == "doc"
+Requires-Dist: intersphinx_registry; extra == "doc"
 Requires-Dist: matplotlib; extra == "doc"
 Requires-Dist: memory-profiler; extra == "doc"
 Requires-Dist: numpydoc; extra == "doc"
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx-copybutton; extra == "doc"
 Requires-Dist: sphinx-design; extra == "doc"
 Requires-Dist: sphinx-issues; extra == "doc"
 Requires-Dist: sphinx-remove-toctrees; extra == "doc"
 Requires-Dist: sphinxcontrib-bibtex; extra == "doc"
 Provides-Extra: full
 Requires-Dist: byte_triggers[all]; extra == "full"
 Provides-Extra: style
 Requires-Dist: bibclean; extra == "style"
-Requires-Dist: black; extra == "style"
-Requires-Dist: codespell; extra == "style"
+Requires-Dist: codespell[toml]>=2.2.4; extra == "style"
 Requires-Dist: isort; extra == "style"
 Requires-Dist: pydocstyle[toml]; extra == "style"
-Requires-Dist: ruff; extra == "style"
+Requires-Dist: ruff>=0.1.8; extra == "style"
 Requires-Dist: toml-sort; extra == "style"
 Requires-Dist: yamllint; extra == "style"
 Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-timeout; extra == "test"
+Requires-Dist: pytest>=8.0; extra == "test"
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![codecov](https://codecov.io/gh/fcbg-hnp-meeg/byte-triggers/graph/badge.svg?token=rSGaJehUMl)](https://codecov.io/gh/fcbg-hnp-meeg/byte-triggers)
 [![tests](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/pytest.yml)
 [![doc](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/doc.yml/badge.svg?branch=main)](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/doc.yml)
```

### Comparing `byte_triggers-0.3.0/byte_triggers.egg-info/SOURCES.txt` & `byte_triggers-0.4.0/byte_triggers.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 byte_triggers/__init__.py
 byte_triggers/_base.py
 byte_triggers/_version.py
-byte_triggers/conftest.py
 byte_triggers/lsl.py
 byte_triggers/mock.py
 byte_triggers/parallel.py
 byte_triggers.egg-info/PKG-INFO
 byte_triggers.egg-info/SOURCES.txt
 byte_triggers.egg-info/dependency_links.txt
 byte_triggers.egg-info/entry_points.txt
@@ -21,10 +21,9 @@
 byte_triggers/io/_inpout.py
 byte_triggers/io/_linux.py
 byte_triggers/utils/__init__.py
 byte_triggers/utils/_checks.py
 byte_triggers/utils/_docs.py
 byte_triggers/utils/_fixes.py
 byte_triggers/utils/_imports.py
-byte_triggers/utils/_tests.py
 byte_triggers/utils/config.py
 byte_triggers/utils/logs.py
```

### Comparing `byte_triggers-0.3.0/pyproject.toml` & `byte_triggers-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -15,50 +15,53 @@
   'Programming Language :: Python :: 3 :: Only',
   'Programming Language :: Python :: 3.10',
   'Programming Language :: Python :: 3.11',
   'Programming Language :: Python :: 3.12',
   'Programming Language :: Python :: 3.9',
 ]
 dependencies = [
-  'mne_lsl',
-  'numpy>=1.21',
+  'mne_lsl>=1.3.1',
+  'numpy>=1.26.4',
   'packaging',
   'psutil',
   'pyparallel; sys_platform == "linux"',
   'pyserial',
 ]
 description = 'Provides byte (0 to 255) triggers on serial/parallel ports and on LSL streams.'
 keywords = [
+  'events',
+  'lsl',
   'parallel',
   'python',
   'serial',
   'triggers',
 ]
 license = {file = 'LICENSE'}
 maintainers = [
   {email = 'mathieu.scheltienne@fcbg.ch', name = 'Mathieu Scheltienne'},
 ]
 name = 'byte_triggers'
 readme = 'README.md'
 requires-python = '>=3.9'
-version = '0.3.0'
+version = '0.4.0'
 
 [project.optional-dependencies]
 all = [
   'byte_triggers[build]',
   'byte_triggers[doc]',
   'byte_triggers[style]',
   'byte_triggers[test]',
 ]
 build = [
   'build',
   'twine',
 ]
 doc = [
   'furo',
+  'intersphinx_registry',
   'matplotlib',
   'memory-profiler',
   'numpydoc',
   'sphinx',
   'sphinx-copybutton',
   'sphinx-design',
   'sphinx-issues',
@@ -66,49 +69,40 @@
   'sphinxcontrib-bibtex',
 ]
 full = [
   'byte_triggers[all]',
 ]
 style = [
   'bibclean',
-  'black',
-  'codespell',
+  'codespell[toml]>=2.2.4',
   'isort',
   'pydocstyle[toml]',
-  'ruff',
+  'ruff>=0.1.8',
   'toml-sort',
   'yamllint',
 ]
 test = [
-  'pytest',
   'pytest-cov',
   'pytest-timeout',
+  'pytest>=8.0',
 ]
 
 [project.scripts]
 byte_triggers-sys_info = 'byte_triggers.commands.sys_info:run'
 
 [project.urls]
 documentation = 'https://fcbg-hnp-meeg.github.io/byte-triggers'
-homepage = 'https://fcbg-hnp-meeg.github.io/byte-triggers'
 source = 'https://github.com/fcbg-hnp-meeg/byte-triggers'
 tracker = 'https://github.com/fcbg-hnp-meeg/byte-triggers/issues'
 
-[tool.black]
-extend-exclude = '''
-(
-      __pycache__
-    | .github
-    | setup.py
-    | doc/
-)
-'''
-include = '\.pyi?$'
-line-length = 88
-target-version = ['py39']
+[tool.codespell]
+check-filenames = true
+check-hidden = true
+ignore-words = '.codespellignore'
+skip = 'build,.git,.mypy_cache,.pytest_cache,.venv'
 
 [tool.coverage.report]
 exclude_lines = [
   'if __name__ == .__main__.:',
   'if TYPE_CHECKING:',
   'pragma: no cover',
 ]
@@ -126,42 +120,54 @@
   '**/conftest.py',
   '**/tests/**',
 ]
 
 [tool.isort]
 extend_skip_glob = [
   'doc/*',
-  'setup.py',
 ]
 line_length = 88
 multi_line_output = 3
 profile = 'black'
 py_version = 39
 
 [tool.pydocstyle]
 add_ignore = 'D100,D104,D107'
 convention = 'numpy'
 ignore-decorators = '(copy_doc|property|.*setter|.*getter|pyqtSlot|Slot)'
-match = '^(?!setup|__init__|test_).*\.py'
+match = '^(?!__init__|test_).*\.py'
 match-dir = '^byte_triggers.*'
 
 [tool.pytest.ini_options]
 addopts = '--durations 20 --junit-xml=junit-results.xml --verbose'
-filterwarnings = []
-minversion = '6.0'
+minversion = '8.0'
 
 [tool.ruff]
 extend-exclude = [
-  "doc",
-  "setup.py",
+  'byte_triggers/io',
+  'doc',
 ]
 line-length = 88
+target-version = 'py39'
 
-[tool.ruff.per-file-ignores]
-"__init__.py" = ["F401"]
+[tool.ruff.format]
+docstring-code-format = true
+line-ending = "lf"
+
+[tool.ruff.lint]
+ignore = []
+select = ['A', 'B', 'E', 'F', 'G', 'LOG', 'NPY', 'PIE', 'PT', 'T20', 'UP', 'W']
+
+[tool.ruff.lint.per-file-ignores]
+'*' = [
+  'B904', # 'Within an except clause, raise exceptions with raise ... from ...'
+  'UP007', # 'Use `X | Y` for type annotations', requires python 3.10
+]
+'*.pyi' = ['E501']
+'__init__.py' = ['F401']
 
 [tool.setuptools]
 include-package-data = false
 
 [tool.setuptools.packages.find]
 exclude = ['byte_triggers*tests']
 include = ['byte_triggers*']
```

