# Comparing `tmp/ansys_tools_visualization_interface-0.1.0.tar.gz` & `tmp/ansys_tools_visualization_interface-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_tools_visualization_interface-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_tools_visualization_interface-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_tools_visualization_interface-0.1.0.tar` & `ansys_tools_visualization_interface-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1071 2024-05-10 12:44:04.394506 ansys_tools_visualization_interface-0.1.0/LICENSE
--rw-r--r--   0        0        0     4791 2024-05-10 12:44:04.394506 ansys_tools_visualization_interface-0.1.0/README.rst
--rw-r--r--   0        0        0     2860 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2017 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/__init__.py
--rw-r--r--   0        0        0     1180 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/__init__.py
--rw-r--r--   0        0        0     1857 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/_base.py
--rw-r--r--   0        0        0     1320 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/__init__.py
--rw-r--r--   0        0        0    19373 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/pyvista.py
--rw-r--r--   0        0        0    13630 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/pyvista_interface.py
--rw-r--r--   0        0        0     2803 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_local.py
--rw-r--r--   0        0        0     2555 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_remote.py
--rw-r--r--   0        0        0     5102 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_service.py
--rw-r--r--   0        0        0     1339 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/__init__.py
--rw-r--r--   0        0        0      499 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/+xy.png
--rw-r--r--   0        0        0      487 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/+xz.png
--rw-r--r--   0        0        0      497 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/+yz.png
--rw-r--r--   0        0        0      496 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/-xy.png
--rw-r--r--   0        0        0      484 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/-xz.png
--rw-r--r--   0        0        0      495 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/-yz.png
--rw-r--r--   0        0        0      569 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/designpoint.png
--rw-r--r--   0        0        0      526 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/downarrow.png
--rw-r--r--   0        0        0      725 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/isometric.png
--rw-r--r--   0        0        0      339 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/measurement.png
--rw-r--r--   0        0        0      341 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/ruler.png
--rw-r--r--   0        0        0      451 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/upxarrow.png
--rw-r--r--   0        0        0      442 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/upyarrow.png
--rw-r--r--   0        0        0      428 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/upzarrow.png
--rw-r--r--   0        0        0     2990 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/button.py
--rw-r--r--   0        0        0     4215 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/displace_arrows.py
--rw-r--r--   0        0        0     3742 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/measure.py
--rw-r--r--   0        0        0     3568 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/ruler.py
--rw-r--r--   0        0        0     3326 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/view_button.py
--rw-r--r--   0        0        0     2307 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/widget.py
--rw-r--r--   0        0        0     2342 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/plotter.py
--rw-r--r--   0        0        0     1182 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/types/__init__.py
--rw-r--r--   0        0        0     3174 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/types/edge_plot.py
--rw-r--r--   0        0        0     4908 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/types/mesh_object_plot.py
--rw-r--r--   0        0        0     1187 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/utils/__init__.py
--rw-r--r--   0        0        0     2920 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/utils/clip_plane.py
--rw-r--r--   0        0        0     1641 2024-05-10 12:44:04.398506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/utils/color.py
--rw-r--r--   0        0        0     3825 2024-05-10 12:44:04.402506 ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/utils/logger.py
--rw-r--r--   0        0        0     6568 1970-01-01 00:00:00.000000 ansys_tools_visualization_interface-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4861 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/README.rst
+-rw-r--r--   0        0        0     2858 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2020 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/__init__.py
+-rw-r--r--   0        0        0     1180 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/__init__.py
+-rw-r--r--   0        0        0     1857 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/_base.py
+-rw-r--r--   0        0        0     1320 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/__init__.py
+-rw-r--r--   0        0        0    19281 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/pyvista.py
+-rw-r--r--   0        0        0    13932 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/pyvista_interface.py
+-rw-r--r--   0        0        0     2803 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_local.py
+-rw-r--r--   0        0        0     2555 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_remote.py
+-rw-r--r--   0        0        0     5102 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_service.py
+-rw-r--r--   0        0        0     1339 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/__init__.py
+-rw-r--r--   0        0        0      499 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/+xy.png
+-rw-r--r--   0        0        0      487 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/+xz.png
+-rw-r--r--   0        0        0      497 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/+yz.png
+-rw-r--r--   0        0        0      496 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/-xy.png
+-rw-r--r--   0        0        0      484 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/-xz.png
+-rw-r--r--   0        0        0      495 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/-yz.png
+-rw-r--r--   0        0        0      569 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/designpoint.png
+-rw-r--r--   0        0        0      526 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/downarrow.png
+-rw-r--r--   0        0        0      725 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/isometric.png
+-rw-r--r--   0        0        0      339 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/measurement.png
+-rw-r--r--   0        0        0      341 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/ruler.png
+-rw-r--r--   0        0        0      451 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/upxarrow.png
+-rw-r--r--   0        0        0      442 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/upyarrow.png
+-rw-r--r--   0        0        0      428 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/upzarrow.png
+-rw-r--r--   0        0        0     2990 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/button.py
+-rw-r--r--   0        0        0     4215 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/displace_arrows.py
+-rw-r--r--   0        0        0     3742 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/measure.py
+-rw-r--r--   0        0        0     3568 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/ruler.py
+-rw-r--r--   0        0        0     3326 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/view_button.py
+-rw-r--r--   0        0        0     2311 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/widget.py
+-rw-r--r--   0        0        0     3023 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/plotter.py
+-rw-r--r--   0        0        0     1182 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/types/__init__.py
+-rw-r--r--   0        0        0     3174 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/types/edge_plot.py
+-rw-r--r--   0        0        0     4908 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/types/mesh_object_plot.py
+-rw-r--r--   0        0        0     1187 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/utils/__init__.py
+-rw-r--r--   0        0        0     2920 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/utils/clip_plane.py
+-rw-r--r--   0        0        0     1641 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/utils/color.py
+-rw-r--r--   0        0        0     3825 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/utils/logger.py
+-rw-r--r--   0        0        0     6636 1970-01-01 00:00:00.000000 ansys_tools_visualization_interface-0.2.0/PKG-INFO
```

### Comparing `ansys_tools_visualization_interface-0.1.0/LICENSE` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/utils/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-MIT License
-
-Copyright (c) 2024 Ansys Internal
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+# Copyright (C) 2023 - 2024 ANSYS, Inc. and/or its affiliates.
+# SPDX-License-Identifier: MIT
+#
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+"""Provides the Utils package."""
```

### Comparing `ansys_tools_visualization_interface-0.1.0/README.rst` & `ansys_tools_visualization_interface-0.2.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -27,59 +27,59 @@
    :alt: pre-commit.ci status
 
 .. contents::
 
 Overview
 --------
 
-Visualization Interface tool is a Python API that provides an interface between PyAnsys libraries and
+The Visualization Interface Tool is a Python API that provides an interface between PyAnsys libraries and
 different plotting backends.
 
-Visualization Interface tool offers these main features:
+The Visualization Interface Tool offers these main features:
 
 * Serves as an interface between PyAnsys and other plotting libraries (although only
   `PyVista <https://docs.pyvista.org/version/stable/>`_ is supported currently).
 * Provides out-of-the box picking, viewing, and measuring functionalities.
 * Supplies an extensible class for adding custom functionalities.
 
 Documentation and issues
 ------------------------
 
-Documentation for the latest stable release of Visualization Interface tool is hosted
-at `Visualization Interface tool documentation <https://visualization-interface.tools.docs.pyansys.com/version/dev/>`_.
+Documentation for the latest stable release of the Visualization Interface Tool is hosted
+at `Visualization Interface Tool documentation <https://visualization-interface.tools.docs.pyansys.com/version/stable/index.html>`_.
 
 The documentation has these sections:
 
-- `Getting started <https://visualization-interface.tools.docs.pyansys.com/version/dev/getting_started/index.html>`_: Learn
-  how to install Visualization Interface tool in user mode and quickly begin using it.
-- `User guide <https://visualization-interface.tools.docs.pyansys.com/version/dev/user_guide/index.html>`_: Understand key
-  concepts for implementing Visualization Interface tool in your workflow.
-- `API reference <https://visualization-interface.tools.docs.pyansys.com/version/dev/api/index.html>`_: Understand how to
-  use Python to interact programmatically with Visualization Interface tool.
-- `Examples <visualization-interface.tools.docs.pyansys.com/version/dev/examples/index.html>`_: Explore examples that
-  show how to use Visualization Interface tool to perform many different types of operations.
-- `Contribute <https://visualization-interface.tools.docs.pyansys.com/version/dev/contributing/index.html>`_: Learn how to
-  contribute to the Visualization Interface tool codebase or documentation.
+- `Getting started <https://visualization-interface.tools.docs.pyansys.com/version/stable/getting_started/index.html>`_: Learn
+  how to install the Visualization Interface Tool in user mode and quickly begin using it.
+- `User guide <https://visualization-interface.tools.docs.pyansys.com/version/stable/user_guide/index.html>`_: Understand key
+  concepts for implementing the Visualization Interface Tool in your workflow.
+- `API reference <https://visualization-interface.tools.docs.pyansys.com/version/stable/api/index.html>`_: Understand how to
+  use Python to interact programmatically with the Visualization Interface Tool.
+- `Examples <https://visualization-interface.tools.docs.pyansys.com/version/stable/examples/index.html>`_: Explore examples that
+  show how to use the Visualization Interface Tool to perform many different types of operations.
+- `Contribute <https://visualization-interface.tools.docs.pyansys.com/version/stable/contributing.html>`_: Learn how to
+  contribute to the Visualization Interface Tool codebase or documentation.
 
 In the upper right corner of the documentation's title bar, there is an option
 for switching from viewing the documentation for the latest stable release
 to viewing the documentation for the development version or previously
 released versions.
 
-On the `Visualization Interface tool Issues <https://github.com/ansys/ansys-tools-visualization-interface/issues>`_
+On the `Visualization Interface Tool Issues <https://github.com/ansys/ansys-tools-visualization-interface/issues>`_
 page, you can create issues to report bugs and request new features. On the
 `Discussions <https://discuss.ansys.com/>`_ page on the Ansys Developer portal,
 you can post questions, share ideas, and get community feedback.
 
 If you have general questions about the PyAnsys ecosystem, email
 `pyansys.core@ansys.com <pyansys.core@ansys.com>`_. If your
-question is specific to Visualization Interface tool, ask your
+question is specific to the Visualization Interface Tool, ask your
 question in an issue as described in the previous paragraph.
 
 License
 -------
 
-Visualization Interface tool is licensed under the `MIT License <https://github.com/ansys/ansys-tools-visualization-interface/blob/main/LICENSE>`_.
+The Visualization Interface Tool is licensed under the `MIT License <https://github.com/ansys/ansys-tools-visualization-interface/blob/main/LICENSE>`_.
 
-Visualization Interface tool makes no commercial claim over Ansys whatsoever. This library adds a
+The Visualization Interface Tool makes no commercial claim over Ansys whatsoever. This library adds a
 Python interface for visualizing Ansys results without changing the core behavior or
 license of the original Ansys software.
```

### Comparing `ansys_tools_visualization_interface-0.1.0/pyproject.toml` & `ansys_tools_visualization_interface-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-tools-visualization-interface"
-version = "0.1.0"
+version = "0.2.0"
 description = "A Python visualization interface for PyAnsys libraries"
 readme = "README.rst"
 requires-python = ">=3.9,<4"
 license = { file = "LICENSE" }
 authors = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 maintainers = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 classifiers = [
@@ -28,25 +28,25 @@
     "websockets >= 12.0,<13",
     "trame >= 3.6.0,<4",
     "trame-vtk >= 2.8.7,<3",
     "trame-vuetify >= 2.4.3,<3",
 ]
 
 [project.optional-dependencies]
-tests = ["pytest==8.2.0", "pytest-pyvista==0.1.9", "pytest-cov==5.0.0"]
+tests = ["pytest==8.2.1", "pytest-pyvista==0.1.9", "pytest-cov==5.0.0"]
 doc = [
-    "ansys-sphinx-theme==0.15.2",
+    "ansys-sphinx-theme==0.16.2",
     "jupyter_sphinx==0.5.3",
     "jupytext==1.16.2",
-    "nbsphinx==0.9.3",
+    "nbsphinx==0.9.4",
     "numpydoc==1.7.0",
     "sphinx==7.3.7",
-    "sphinx-autoapi==3.1.0b0",
+    "sphinx-autoapi==3.1.1",
     "sphinx-copybutton==0.5.2",
-    "sphinx_design==0.5.0",
+    "sphinx_design==0.6.0",
     "sphinx-gallery==0.16.0",
     "sphinx-jinja==2.0.2",
 ]
 
 [tool.flit.module]
 name = "ansys.tools.visualization_interface"
```

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/__init__.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,20 +15,19 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-"""Visualization Interface tool is a Python client library for visualizing the results of Ansys simulations."""
+"""Visualization Interface Tool is a Python client library for visualizing the results of Ansys simulations."""
+import importlib.metadata as importlib_metadata
 import os
 
-import pkg_resources
-
-__version__ = pkg_resources.get_distribution("ansys-tools-visualization-interface").version
+__version__ = importlib_metadata.version(__name__.replace(".", "-"))
 
 USE_TRAME: bool = False
 DOCUMENTATION_BUILD: bool = False
 TESTING_MODE: bool = os.environ.get("PYANSYS_VISUALIZER_TESTMODE", "false").lower() == "true"
 
 from ansys.tools.visualization_interface.plotter import Plotter  # noqa: F401, E402
 from ansys.tools.visualization_interface.types.edge_plot import EdgePlot  # noqa: F401, E402
```

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/__init__.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/_base.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/_base.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/__init__.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/pyvista.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/pyvista.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 from ansys.tools.visualization_interface.types.edge_plot import EdgePlot
 from ansys.tools.visualization_interface.types.mesh_object_plot import MeshObjectPlot
 from ansys.tools.visualization_interface.utils.color import Color
 from ansys.tools.visualization_interface.utils.logger import logger
 
 
 class PyVistaBackendInterface(BaseBackend):
-    """Provides the interface for the Visualization Interface tool plotter.
+    """Provides the interface for the Visualization Interface Tool plotter.
 
     This class is intended to be used as a base class for the custom plotters
     in the different PyAnsys libraries. It provides the basic plotter functionalities,
     such as adding objects and enabling widgets and picking capabilities. It also
     provides the ability to show the plotter using the `trame <https://kitware.github.io/trame/index.html>`_
     service.
 
@@ -214,15 +214,15 @@
 
         self._picker_added_actors_map[custom_object.actor.name] = added_actors
 
     def unselect_object(self, custom_object: Union[MeshObjectPlot, EdgePlot]) -> None:
         """Unselect a custom object in the plotter.
 
         This method removes edge highlighting and the label from a plotter actor and removes
-        the object from the Visualization Interface tool object selection.
+        the object from the Visualization Interface Tool object selection.
 
         Parameters
         ----------
         custom_object : Union[MeshObjectPlot, EdgePlot]
             Custom object to unselect.
 
         """
@@ -376,15 +376,15 @@
 
     def show_plotter(self, screenshot: Optional[str] = None) -> None:
         """Show the plotter or start the `trame <https://kitware.github.io/trame/index.html>`_ service.
 
         Parameters
         ----------
         plotter : Plotter
-            Visualization Interface tool plotter with the meshes added.
+            Visualization Interface Tool plotter with the meshes added.
         screenshot : str, default: None
             Path for saving a screenshot of the image that is being represented.
 
         """
         if self._use_trame and _HAS_TRAME:
             visualizer = TrameVisualizer()
             visualizer.set_scene(self._pl)
@@ -496,10 +496,7 @@
         """
         if hasattr(object, "__iter__"):
             logger.debug("Plotting objects in list...")
             self.pv_interface.plot_iter(object, filter, **plotting_options)
         else:
             self.pv_interface.plot(object, filter, **plotting_options)
 
-    def show(self):
-        """Show the rendered scene."""
-        self.pv_interface.show()
```

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/pyvista_interface.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/pyvista_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,16 @@
         show_plane: bool = False,
         **plotter_kwargs,
     ) -> None:
         """Initialize the plotter."""
         # Generate custom scene if ``None`` is provided
         if scene is None:
             scene = pv.Plotter(plotter_kwargs)
-
+        if TESTING_MODE:
+            scene.off_screen = True
         # If required, use a white background with no gradient
         if not color_opts:
             color_opts = dict(color="white")
 
         # Create the scene
         self._scene = scene
         # Scene: assign the background
@@ -326,16 +327,23 @@
 
         # Override Jupyter backend if building docs
         if DOCUMENTATION_BUILD:
             jupyter_backend = "static"
 
         # Enabling anti-aliasing by default on scene
         self.scene.enable_anti_aliasing("ssaa")
+
+        # If screenshot is requested, set off_screen to True for the plotter
+        if kwargs.get("screenshot") is not None:
+            self.scene.off_screen = True
+
+        # If running on testing, set off_screen to True for the plotter
         if TESTING_MODE:
             self.scene.off_screen = True
+
         self.scene.show(jupyter_backend=jupyter_backend, **kwargs)
 
     def set_add_mesh_defaults(self, plotting_options: Optional[Dict]) -> None:
         """Set the default values for the plotting options.
 
         Parameters
         ----------
```

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_local.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_local.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_remote.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_remote.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_service.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_service.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/__init__.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,11 +15,11 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-"""Provides widgets for the Visualization Interface tool plotter."""
+"""Provides widgets for the Visualization Interface Tool plotter."""
 from ansys.tools.visualization_interface.backends.pyvista.widgets.widget import (  # noqa: F401
     PlotterWidget,
 )
```

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/designpoint.png` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/designpoint.png`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/downarrow.png` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/downarrow.png`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/isometric.png` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/isometric.png`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/button.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/button.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/displace_arrows.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/displace_arrows.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/measure.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/measure.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 from vtk import vtkActor, vtkButtonWidget, vtkPNGReader
 
 from ansys.tools.visualization_interface.backends.pyvista.widgets.widget import PlotterWidget
 
 
 class MeasureWidget(PlotterWidget):
-    """Provides the measure widget for the Visualization Interface tool ``Plotter`` class.
+    """Provides the measure widget for the Visualization Interface Tool ``Plotter`` class.
 
     Parameters
     ----------
     plotter_helper : PlotterHelper
         Plotter to add the measure widget to.
 
     """
```

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/ruler.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/ruler.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-"""Provides the ruler widget for the Visualization Interface tool plotter."""
+"""Provides the ruler widget for the Visualization Interface Tool plotter."""
 
 from pathlib import Path
 
 from pyvista import Plotter
 from vtk import vtkActor, vtkButtonWidget, vtkPNGReader
 
 from ansys.tools.visualization_interface.backends.pyvista.widgets.widget import PlotterWidget
 
 
 class Ruler(PlotterWidget):
-    """Provides the ruler widget for the Visualization Interface tool ``Plotter`` class.
+    """Provides the ruler widget for the Visualization Interface Tool ``Plotter`` class.
 
     Parameters
     ----------
     plotter : ~pyvista.Plotter
         Provides the plotter to add the ruler widget to.
 
     """
```

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/view_button.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/view_button.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/widget.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     plotter : ~pyvista.Plotter
         Plotter instance to add the widget to.
 
     Notes
     -----
     These widgets are intended to be used with PyVista plotter objects.
     More specifically, the way in which this abstraction has been built
-    ensures that these widgets can be easily integrated with Visualization Interface tool's
-    widgets.
+    ensures that these widgets can be easily integrated with the Visualization Interface
+    Tool's widgets.
 
     """
 
     def __init__(self, plotter: Plotter):
         """Initialize the ``PlotterWidget`` class."""
         self._plotter: Plotter = plotter
```

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/plotter.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/plotter.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,10 +52,33 @@
         object : Any
             Object to plot.
         plotting_options : dict
             Additional plotting options.
         """
         self._backend.plot(object=object, **plotting_options)
 
-    def show(self):
-        """Show the plotted objects."""
-        self._backend.show()
+    def show(
+        self,
+        object: Any = None,
+        screenshot: str = None,
+        filter: bool = None,
+        **plotting_options
+        ) -> None:
+        """Show the plotted objects.
+
+        Parameters
+        ----------
+        object : Any, optional
+            Object to show, by default None.
+        screenshot : str, optional
+            Path to save a screenshot, by default None.
+        filter : bool, optional
+            Flag to filter the object, by default None.
+        plotting_options : dict
+            Additional plotting options the selected backend accepts.
+        """
+        self._backend.show(
+            object=object,
+            screenshot=screenshot,
+            filter=filter,
+            **plotting_options
+            )
```

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/types/__init__.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/types/edge_plot.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/types/edge_plot.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/types/mesh_object_plot.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/types/mesh_object_plot.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/utils/__init__.py` & `ansys_tools_visualization_interface-0.2.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# Copyright (C) 2023 - 2024 ANSYS, Inc. and/or its affiliates.
-# SPDX-License-Identifier: MIT
-#
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-"""Provides the Utils package."""
+MIT License
+
+Copyright (c) 2024 ANSYS, Inc. and/or its affiliates.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/utils/clip_plane.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/utils/clip_plane.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/utils/color.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/utils/color.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/src/ansys/tools/visualization_interface/utils/logger.py` & `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.1.0/PKG-INFO` & `ansys_tools_visualization_interface-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-tools-visualization-interface
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python visualization interface for PyAnsys libraries
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -17,26 +17,26 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pyvista >= 0.42.0,<1
 Requires-Dist: beartype >= 0.17.0,<1
 Requires-Dist: websockets >= 12.0,<13
 Requires-Dist: trame >= 3.6.0,<4
 Requires-Dist: trame-vtk >= 2.8.7,<3
 Requires-Dist: trame-vuetify >= 2.4.3,<3
-Requires-Dist: ansys-sphinx-theme==0.15.2 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.16.2 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.5.3 ; extra == "doc"
 Requires-Dist: jupytext==1.16.2 ; extra == "doc"
-Requires-Dist: nbsphinx==0.9.3 ; extra == "doc"
+Requires-Dist: nbsphinx==0.9.4 ; extra == "doc"
 Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
 Requires-Dist: sphinx==7.3.7 ; extra == "doc"
-Requires-Dist: sphinx-autoapi==3.1.0b0 ; extra == "doc"
+Requires-Dist: sphinx-autoapi==3.1.1 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
-Requires-Dist: sphinx_design==0.5.0 ; extra == "doc"
+Requires-Dist: sphinx_design==0.6.0 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.16.0 ; extra == "doc"
 Requires-Dist: sphinx-jinja==2.0.2 ; extra == "doc"
-Requires-Dist: pytest==8.2.0 ; extra == "tests"
+Requires-Dist: pytest==8.2.1 ; extra == "tests"
 Requires-Dist: pytest-pyvista==0.1.9 ; extra == "tests"
 Requires-Dist: pytest-cov==5.0.0 ; extra == "tests"
 Provides-Extra: doc
 Provides-Extra: tests
 
 Visualization Interface Tool
 ============================
@@ -67,60 +67,60 @@
    :alt: pre-commit.ci status
 
 .. contents::
 
 Overview
 --------
 
-Visualization Interface tool is a Python API that provides an interface between PyAnsys libraries and
+The Visualization Interface Tool is a Python API that provides an interface between PyAnsys libraries and
 different plotting backends.
 
-Visualization Interface tool offers these main features:
+The Visualization Interface Tool offers these main features:
 
 * Serves as an interface between PyAnsys and other plotting libraries (although only
   `PyVista <https://docs.pyvista.org/version/stable/>`_ is supported currently).
 * Provides out-of-the box picking, viewing, and measuring functionalities.
 * Supplies an extensible class for adding custom functionalities.
 
 Documentation and issues
 ------------------------
 
-Documentation for the latest stable release of Visualization Interface tool is hosted
-at `Visualization Interface tool documentation <https://visualization-interface.tools.docs.pyansys.com/version/dev/>`_.
+Documentation for the latest stable release of the Visualization Interface Tool is hosted
+at `Visualization Interface Tool documentation <https://visualization-interface.tools.docs.pyansys.com/version/stable/index.html>`_.
 
 The documentation has these sections:
 
-- `Getting started <https://visualization-interface.tools.docs.pyansys.com/version/dev/getting_started/index.html>`_: Learn
-  how to install Visualization Interface tool in user mode and quickly begin using it.
-- `User guide <https://visualization-interface.tools.docs.pyansys.com/version/dev/user_guide/index.html>`_: Understand key
-  concepts for implementing Visualization Interface tool in your workflow.
-- `API reference <https://visualization-interface.tools.docs.pyansys.com/version/dev/api/index.html>`_: Understand how to
-  use Python to interact programmatically with Visualization Interface tool.
-- `Examples <visualization-interface.tools.docs.pyansys.com/version/dev/examples/index.html>`_: Explore examples that
-  show how to use Visualization Interface tool to perform many different types of operations.
-- `Contribute <https://visualization-interface.tools.docs.pyansys.com/version/dev/contributing/index.html>`_: Learn how to
-  contribute to the Visualization Interface tool codebase or documentation.
+- `Getting started <https://visualization-interface.tools.docs.pyansys.com/version/stable/getting_started/index.html>`_: Learn
+  how to install the Visualization Interface Tool in user mode and quickly begin using it.
+- `User guide <https://visualization-interface.tools.docs.pyansys.com/version/stable/user_guide/index.html>`_: Understand key
+  concepts for implementing the Visualization Interface Tool in your workflow.
+- `API reference <https://visualization-interface.tools.docs.pyansys.com/version/stable/api/index.html>`_: Understand how to
+  use Python to interact programmatically with the Visualization Interface Tool.
+- `Examples <https://visualization-interface.tools.docs.pyansys.com/version/stable/examples/index.html>`_: Explore examples that
+  show how to use the Visualization Interface Tool to perform many different types of operations.
+- `Contribute <https://visualization-interface.tools.docs.pyansys.com/version/stable/contributing.html>`_: Learn how to
+  contribute to the Visualization Interface Tool codebase or documentation.
 
 In the upper right corner of the documentation's title bar, there is an option
 for switching from viewing the documentation for the latest stable release
 to viewing the documentation for the development version or previously
 released versions.
 
-On the `Visualization Interface tool Issues <https://github.com/ansys/ansys-tools-visualization-interface/issues>`_
+On the `Visualization Interface Tool Issues <https://github.com/ansys/ansys-tools-visualization-interface/issues>`_
 page, you can create issues to report bugs and request new features. On the
 `Discussions <https://discuss.ansys.com/>`_ page on the Ansys Developer portal,
 you can post questions, share ideas, and get community feedback.
 
 If you have general questions about the PyAnsys ecosystem, email
 `pyansys.core@ansys.com <pyansys.core@ansys.com>`_. If your
-question is specific to Visualization Interface tool, ask your
+question is specific to the Visualization Interface Tool, ask your
 question in an issue as described in the previous paragraph.
 
 License
 -------
 
-Visualization Interface tool is licensed under the `MIT License <https://github.com/ansys/ansys-tools-visualization-interface/blob/main/LICENSE>`_.
+The Visualization Interface Tool is licensed under the `MIT License <https://github.com/ansys/ansys-tools-visualization-interface/blob/main/LICENSE>`_.
 
-Visualization Interface tool makes no commercial claim over Ansys whatsoever. This library adds a
+The Visualization Interface Tool makes no commercial claim over Ansys whatsoever. This library adds a
 Python interface for visualizing Ansys results without changing the core behavior or
 license of the original Ansys software.
```

