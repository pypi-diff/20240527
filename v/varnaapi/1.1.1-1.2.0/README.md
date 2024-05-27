# Comparing `tmp/varnaapi-1.1.1.tar.gz` & `tmp/varnaapi-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varnaapi-1.1.1.tar", last modified: Sat Oct 21 13:31:13 2023, max compression
+gzip compressed data, was "varnaapi-1.2.0.tar", last modified: Mon May 27 09:21:35 2024, max compression
```

## Comparing `varnaapi-1.1.1.tar` & `varnaapi-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 htyao     (1001) htyao     (1001)        0 2023-10-21 13:31:13.093656 varnaapi-1.1.1/
--rw-r--r--   0 htyao     (1001) htyao     (1001)    35061 2020-12-04 00:51:39.000000 varnaapi-1.1.1/LICENSE
--rw-r--r--   0 htyao     (1001) htyao     (1001)     5904 2023-10-21 13:31:13.093656 varnaapi-1.1.1/PKG-INFO
--rw-rw-r--   0 htyao     (1001) htyao     (1001)     4921 2023-09-21 21:15:41.000000 varnaapi-1.1.1/README.md
--rw-rw-r--   0 htyao     (1001) htyao     (1001)     1103 2023-10-21 13:27:05.000000 varnaapi-1.1.1/pyproject.toml
--rw-rw-r--   0 htyao     (1001) htyao     (1001)       38 2023-10-21 13:31:13.093656 varnaapi-1.1.1/setup.cfg
-drwxrwxr-x   0 htyao     (1001) htyao     (1001)        0 2023-10-21 13:31:13.085657 varnaapi-1.1.1/src/
-drwxrwxr-x   0 htyao     (1001) htyao     (1001)        0 2023-10-21 13:31:13.093656 varnaapi-1.1.1/src/varnaapi/
--rw-rw-r--   0 htyao     (1001) htyao     (1001)      245 2023-10-21 13:27:05.000000 varnaapi-1.1.1/src/varnaapi/__init__.py
--rw-rw-r--   0 htyao     (1001) htyao     (1001)       44 2023-09-19 19:32:14.000000 varnaapi-1.1.1/src/varnaapi/config-settings-v1.yml
-drwxrwxr-x   0 htyao     (1001) htyao     (1001)        0 2023-10-21 13:31:13.093656 varnaapi-1.1.1/src/varnaapi/extensions/
--rw-rw-r--   0 htyao     (1001) htyao     (1001)        0 2023-09-21 21:18:14.000000 varnaapi-1.1.1/src/varnaapi/extensions/__init__.py
--rw-r--r--   0 htyao     (1001) htyao     (1001)     8669 2023-09-21 22:44:00.000000 varnaapi-1.1.1/src/varnaapi/extensions/pdb.py
--rw-rw-r--   0 htyao     (1001) htyao     (1001)    22436 2023-10-21 13:27:05.000000 varnaapi-1.1.1/src/varnaapi/models.py
--rw-rw-r--   0 htyao     (1001) htyao     (1001)    29745 2023-09-19 21:08:40.000000 varnaapi-1.1.1/src/varnaapi/param.py
--rw-rw-r--   0 htyao     (1001) htyao     (1001)     1453 2023-09-19 21:08:40.000000 varnaapi-1.1.1/src/varnaapi/settings.py
-drwxrwxr-x   0 htyao     (1001) htyao     (1001)        0 2023-10-21 13:31:13.093656 varnaapi-1.1.1/src/varnaapi.egg-info/
--rw-r--r--   0 htyao     (1001) htyao     (1001)     5904 2023-10-21 13:31:13.000000 varnaapi-1.1.1/src/varnaapi.egg-info/PKG-INFO
--rw-rw-r--   0 htyao     (1001) htyao     (1001)      409 2023-10-21 13:31:13.000000 varnaapi-1.1.1/src/varnaapi.egg-info/SOURCES.txt
--rw-rw-r--   0 htyao     (1001) htyao     (1001)        1 2023-10-21 13:31:13.000000 varnaapi-1.1.1/src/varnaapi.egg-info/dependency_links.txt
--rw-rw-r--   0 htyao     (1001) htyao     (1001)       46 2023-10-21 13:31:13.000000 varnaapi-1.1.1/src/varnaapi.egg-info/requires.txt
--rw-rw-r--   0 htyao     (1001) htyao     (1001)        9 2023-10-21 13:31:13.000000 varnaapi-1.1.1/src/varnaapi.egg-info/top_level.txt
+drwxrwxr-x   0 htyao     (1001) htyao     (1001)        0 2024-05-27 09:21:35.254351 varnaapi-1.2.0/
+-rw-r--r--   0 htyao     (1001) htyao     (1001)    35061 2020-12-04 00:51:39.000000 varnaapi-1.2.0/LICENSE
+-rw-r--r--   0 htyao     (1001) htyao     (1001)     6052 2024-05-27 09:21:35.254351 varnaapi-1.2.0/PKG-INFO
+-rw-rw-r--   0 htyao     (1001) htyao     (1001)     4933 2024-05-27 09:16:33.000000 varnaapi-1.2.0/README.md
+-rw-rw-r--   0 htyao     (1001) htyao     (1001)     1215 2024-05-27 09:16:33.000000 varnaapi-1.2.0/pyproject.toml
+-rw-rw-r--   0 htyao     (1001) htyao     (1001)       38 2024-05-27 09:21:35.254351 varnaapi-1.2.0/setup.cfg
+drwxrwxr-x   0 htyao     (1001) htyao     (1001)        0 2024-05-27 09:21:35.254351 varnaapi-1.2.0/src/
+drwxrwxr-x   0 htyao     (1001) htyao     (1001)        0 2024-05-27 09:21:35.254351 varnaapi-1.2.0/src/varnaapi/
+-rw-rw-r--   0 htyao     (1001) htyao     (1001)      255 2024-05-27 09:16:33.000000 varnaapi-1.2.0/src/varnaapi/__init__.py
+-rw-rw-r--   0 htyao     (1001) htyao     (1001)       44 2024-05-25 23:02:51.000000 varnaapi-1.2.0/src/varnaapi/config-settings-v1.yml
+drwxrwxr-x   0 htyao     (1001) htyao     (1001)        0 2024-05-27 09:21:35.254351 varnaapi-1.2.0/src/varnaapi/extensions/
+-rw-rw-r--   0 htyao     (1001) htyao     (1001)        0 2023-09-21 21:18:14.000000 varnaapi-1.2.0/src/varnaapi/extensions/__init__.py
+-rw-r--r--   0 htyao     (1001) htyao     (1001)     8669 2024-05-03 14:51:06.000000 varnaapi-1.2.0/src/varnaapi/extensions/pdb.py
+-rw-rw-r--   0 htyao     (1001) htyao     (1001)    24774 2024-05-27 09:16:26.000000 varnaapi-1.2.0/src/varnaapi/models.py
+-rw-rw-r--   0 htyao     (1001) htyao     (1001)    29745 2024-05-25 23:02:51.000000 varnaapi-1.2.0/src/varnaapi/param.py
+-rw-rw-r--   0 htyao     (1001) htyao     (1001)     1527 2024-05-27 09:16:26.000000 varnaapi-1.2.0/src/varnaapi/settings.py
+drwxrwxr-x   0 htyao     (1001) htyao     (1001)        0 2024-05-27 09:21:35.254351 varnaapi-1.2.0/src/varnaapi.egg-info/
+-rw-r--r--   0 htyao     (1001) htyao     (1001)     6052 2024-05-27 09:21:35.000000 varnaapi-1.2.0/src/varnaapi.egg-info/PKG-INFO
+-rw-rw-r--   0 htyao     (1001) htyao     (1001)      409 2024-05-27 09:21:35.000000 varnaapi-1.2.0/src/varnaapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 htyao     (1001) htyao     (1001)        1 2024-05-27 09:21:35.000000 varnaapi-1.2.0/src/varnaapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 htyao     (1001) htyao     (1001)       72 2024-05-27 09:21:35.000000 varnaapi-1.2.0/src/varnaapi.egg-info/requires.txt
+-rw-rw-r--   0 htyao     (1001) htyao     (1001)        9 2024-05-27 09:21:35.000000 varnaapi-1.2.0/src/varnaapi.egg-info/top_level.txt
```

### Comparing `varnaapi-1.1.1/LICENSE` & `varnaapi-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `varnaapi-1.1.1/PKG-INFO` & `varnaapi-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: varnaapi
-Version: 1.1.1
+Version: 1.2.0
 Summary: Python helper for RNA visualization tool VARNA
 Author-email: Hua-Ting Yao <hua-ting.yao@polytechnique.edu>
-Project-URL: Homepage, https://htyao.gitlab.io/varna-api/
+Project-URL: Homepage, https://amibio.gitlabpages.inria.fr/varna-api
 Project-URL: Source Code, https://gitlab.inria.fr/amibio/varna-api
 Project-URL: VARNA, https://varna.lisn.upsaclay.fr/index.php
+Project-URL: Issues, https://github.com/anthonyhtyao/varnaapi/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colour
 Requires-Dist: deprecated
 Requires-Dist: pyyaml
-Requires-Dist: ipython
 Requires-Dist: platformdirs
+Requires-Dist: drawsvg~=2.0
+Requires-Dist: svgpathtools
+Requires-Dist: ipython
 
 VARNA API is a Python interface for [VARNA](http://varna.lri.fr/index.php) (v3-93), a Java lightweight component and applet for drawing the RNA secondary structure.
 VARNA allows users to produce drawing in a non-iteractive way via command line.
 However, the command line might be massive and complicate in some use cases.
 VARNA API aims to simplify such process.
-The [online documentation](https://htyao.gitlab.io/varna-api/) is available.
+The [online documentation](https://amibio.gitlabpages.inria.fr/varna-api/) is available.
 
 !!! danger "Starting from v1.1.0, VARNA API uses _1-indexed_ to count RNA bases. The change aims to better align with VARNA and ViennaRNA."
 
 ## Example
 
 The command below highlights region 11-21 and adds a non-canonical base pair at position (14,20)
 on secondary structure `((((((.((((((........)))))).((((((.......))))))..))))))`.
```

### Comparing `varnaapi-1.1.1/README.md` & `varnaapi-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 VARNA API is a Python interface for [VARNA](http://varna.lri.fr/index.php) (v3-93), a Java lightweight component and applet for drawing the RNA secondary structure.
 VARNA allows users to produce drawing in a non-iteractive way via command line.
 However, the command line might be massive and complicate in some use cases.
 VARNA API aims to simplify such process.
-The [online documentation](https://htyao.gitlab.io/varna-api/) is available.
+The [online documentation](https://amibio.gitlabpages.inria.fr/varna-api/) is available.
 
 !!! danger "Starting from v1.1.0, VARNA API uses _1-indexed_ to count RNA bases. The change aims to better align with VARNA and ViennaRNA."
 
 ## Example
 
 The command below highlights region 11-21 and adds a non-canonical base pair at position (14,20)
 on secondary structure `((((((.((((((........)))))).((((((.......))))))..))))))`.
```

### Comparing `varnaapi-1.1.1/pyproject.toml` & `varnaapi-1.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 varnaapi = ["*.yml"]
 
 [project]
 name = "varnaapi"
-version = "1.1.1"
+version = "1.2.0"
 authors = [
     {name= "Hua-Ting Yao", email="hua-ting.yao@polytechnique.edu"}
 ]
 description = "Python helper for RNA visualization tool VARNA"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
@@ -27,15 +27,18 @@
     "Topic :: Scientific/Engineering",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "colour",
     "deprecated",
     "pyyaml",
-    "ipython",
-    "platformdirs"
+    "platformdirs",
+    "drawsvg~=2.0",
+    "svgpathtools",
+    "ipython"
 ]
 
 [project.urls]
-"Homepage" = "https://htyao.gitlab.io/varna-api/"
+"Homepage" = "https://amibio.gitlabpages.inria.fr/varna-api"
 "Source Code" = "https://gitlab.inria.fr/amibio/varna-api"
 "VARNA" = "https://varna.lisn.upsaclay.fr/index.php"
+"Issues" = "https://github.com/anthonyhtyao/varnaapi/issues"
```

### Comparing `varnaapi-1.1.1/src/varnaapi/extensions/pdb.py` & `varnaapi-1.2.0/src/varnaapi/extensions/pdb.py`

 * *Files identical despite different names*

### Comparing `varnaapi-1.1.1/src/varnaapi/models.py` & `varnaapi-1.2.0/src/varnaapi/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import re
 import os
 import abc
 from string import ascii_lowercase, ascii_uppercase
 from colour import Color
 import subprocess
+from math import ceil
 from tempfile import NamedTemporaryFile
 from deprecated import deprecated
+from functools import reduce
+
+from IPython.display import display
+from svgpathtools import svg2paths
+from drawsvg.jupyter import JupyterSvgImage
 
-from IPython.display import Image, display, SVG
 
 from varnaapi.param import _VarnaConfig, BasesStyle, _Title, _Highlight, _Annotation, _BPStyle, _ChemProb, _ColorMap
 import varnaapi.settings
 
 
 PARENTHESES_SYSTEMS = [
     ("(", ")"),
@@ -19,14 +24,19 @@
     ("<", ">"),
     ("{", "}")
 ] + [(c1, c2) for c1, c2 in zip(ascii_uppercase, ascii_lowercase)]
 PARENTHESES_OPENING = [c1 for c1, c2 in PARENTHESES_SYSTEMS]
 PARENTHESES_CLOSING = {c2: c1 for c1, c2 in PARENTHESES_SYSTEMS}
 
 
+@deprecated("Class has been renamed 'Structure'")
+def VARNA(*args, **kwargs):
+    return Structure(*args, **kwargs)
+
+
 
 def assert_valid_interval(length, *args):
     if not varnaapi.settings.CONFIG['hackmode']:
         for i in args:
             if i < 1 or i > length:
                 raise Exception("{} out of range".format(args))
 
@@ -75,14 +85,27 @@
             if count == 0:
                 current = 0
         else:
             res[ind+1] = current
     return list(set(res[t] for x in positions for t in (x if isinstance(x, tuple) else (x,)) if res[t]!=0))
 
 
+def _border_of_path(path):
+    """Return max x and y of a svgpathtools path
+    """
+    _, x, _, y = path.bbox()
+    return x, y
+
+
+def _border_of_svg(name):
+    """Return border of given svg filename
+    """
+    paths, _ = svg2paths(name)
+    return reduce(lambda u, v: (max(u[0], v[0]), max(u[1], v[1])), map(_border_of_path, paths), (0, 0))
+
 
 class BasicDraw(_VarnaConfig):
     def __init__(self):
         super().__init__()
 
         self.structure = ""
         self.aux_BPs = []
@@ -91,28 +114,30 @@
         self.bases_styles = {}
         self.annotations = []
         self.chem_prob = []
         self.length = 0
         self.colormap = None
         self.to_flip = []
         self.smart_flip = False
+        self._check_interval = True
 
     def add_aux_BP(self, i:int, j:int, edge5:str='wc', edge3:str='wc', stericity:str='cis', color='blue', thickness:float=1, **kwargs):
         """Add an additional base pair `(i,j)`, possibly defining and using custom style
 
         Args:
             i: 5' position of base pair
             j: 3' position of base pair
             edge5: Edge 5' used for interaction in non-canonical base-pairs, as defined by the Leontis/Westhof classification of base-pairs. Admissible values are __wc__ (Watson/Crick edge), __h__ (Hoogsteen edge) and __s__ (Sugar edge).
             edge3: Edge 3' used for interaction in non-canonical base-pairs. Admissible values are __wc__, __h__ and __s__.
             stericity: Orientation of the strands. Admissible values are __cis__ and __trans__
             color (color): Base-pair color
             thickness: Base-pair thickness
         """
-        assert_valid_interval(self.length, i, j)
+        if self._check_interval:
+            assert_valid_interval(self.length, i, j)
 
         self.aux_BPs.append((i, j, _BPStyle(edge5=edge5, edge3=edge3, stericity=stericity, color=color, thickness=thickness, **kwargs)))
 
     def add_highlight_region(self, i:int, j:int, radius:float=16, fill="#BCFFDD", outline="#6ED86E", **kwargs):
         """Highlights a region by drawing a polygon of predefined radius,
         fill color and outline color around it.
         A region consists in an interval from base `i` to base `j`.
@@ -120,15 +145,16 @@
         Args:
             i: 5'-end of the highlight
             j: 3'-end of the highlight
             radius: Thickness of the highlight
             fill (color): The color used to fill the highlight
             outline (color): The color used to draw the line around the highlight
         """
-        assert_valid_interval(self.length, i, j)
+        if self._check_interval:
+            assert_valid_interval(self.length, i, j)
 
         self.highlight_regions.append((i, j, _Highlight(radius, fill, outline, **kwargs)))
 
     def set_title(self, title:str, color='#000000', size:int=19, **kwargs):
         """Set title displayed at the bottom of the panel with color and font size
         """
         self._title = _Title(title, color, size, **kwargs)
@@ -176,15 +202,16 @@
         Args:
             base: index of the first base of adjacent bases
             glyph: Shape of the annotation chosen from ['arrow', 'dot', 'pin', 'triangle']
             dir: Direction of the annotation chosen from ['in', 'out']
             intensity: Annotation intensity, _i.e._ thickness
             color (color): Color used to draw the annotation
         """
-        assert_valid_interval(self.length, base)
+        if self._check_interval:
+            assert_valid_interval(self.length, base)
         self.chem_prob.append((int(base), _ChemProb(glyph=glyph, dir=dir, intensity=intensity, color=color, **kwargs)))
 
     def add_colormap(self, values, vMin:float=None, vMax:float=None, caption:str="", style="energy", **kwargs):
         """Add color map on bases.
 
         Args:
             values (float list): list of values in float for each base. `0`s are added at the end of the list if the list length is shorter than the number of bases.
@@ -193,15 +220,15 @@
             caption: Color map caption
             style: Color map style, which is one of the following
 
                 - predefined style from
 
                     ['red', 'blue', 'green', 'heat', 'energy', 'bw']
 
-                - customized style in a list of pairs, (value, color)
+                - customized style in dictionary {value: color}
         """
         self.colormap = _ColorMap(values, vMin, vMax, caption, style, **kwargs)
 
     def flip(self, *positions):
         """Flip one or more helices identfied by given positions.
 
         Note: Behind the flip
@@ -225,15 +252,16 @@
             ```
             One can flip the first and third branches by
             >>> v = varnaapi.Structure(structure=dbn)
             >>> v.flip(5, (27,33))
 
         __See Also:__ [BasicDraw.enable_smart_flip][varnaapi.BasicDraw.enable_smart_flip]
         """
-        map(lambda x: assert_valid_interval(self.length, *(x if isinstance(x, tuple) else (x,))), positions)
+        if self._check_interval:
+            map(lambda x: assert_valid_interval(self.length, *(x if isinstance(x, tuple) else (x,))), positions)
         self.to_flip += positions
 
 
     def enable_smart_flip(self, enable:bool=True):
         """Enable to flip positions treating to address points 1-3 in flip().
         When enable, for each branch of exterior loop, VARNA API will send only the 5' most position to flip to VARNA if any position (unpaired included) of the branch is given by flip().
 
@@ -321,43 +349,66 @@
 
     def format_structure(self):
         return self.structure
 
     def _gen_input_cmd(self):
         return []
 
-    def savefig(self, output, show:bool=False):
+    def savefig(self, output):
         """Call VARNA to draw and store the paint in output
 
         Args:
             output: Output file name with extension is either png or svg
-            show: Show the drawing
-
-        Note:
-            The argument `show` is used only in jupyter notebook
         """
         self.output = output
         cmd = self._gen_command()
-        print(cmd)
+        varnaapi.settings.Logger.debug(cmd)
         subprocess.run(cmd)
 
-        if show:
-            if output[-3:] == 'png':
-                display(Image(filename=output))
-            elif output[-3:] == 'svg':
-                display(SVG(filename=output))
+    def _to_svg(self, size=None, full:bool=False):
+        """Convert drawing to svg that can be displayed in jupyter notebook
+
+        Code inspired from drawsvg and svgpathtools
+        """
+        tmp = NamedTemporaryFile(suffix='.svg')
+        self.savefig(tmp.name)
+        # We need to modify some info in svg tag to make it display until VARNA fix it
+        x, y = _border_of_svg(tmp.name)
+        if full:
+            w = "100%"
+            h = "100%"
+        else:
+            if size is None:
+                size = max(100, min(600, max(x, y)))
+            if x > y:
+                w = "{}px".format(size)
+                h = "{}px".format(int(ceil(size*y/x)))
             else:
-                raise Exception("File type should be either png or svg")
+                h = "{}px".format(size)
+                w = "{}px".format(int(ceil(size*x/y)))
+        res = []
+        for line in open(tmp.name).readlines():
+            if line.startswith("<svg"):
+                line = '<svg width="{}" height="{}" version="1.1" viewBox="0 0 {} {}" \n'.format(w, h, int(ceil(x/100)*100), int(ceil(y/100)*100))
+            res.append(line)
+        return "".join(res)
 
-    def show(self, extension='png'):
-        """Show the drawing
-        Equivalent to `savefig(tmp, show=True)` where tmp is a temporary file
+    def show(self, size=None, full=False):
+        """Display drawing (svg format) in jupyter notebook
+
+        Args:
+            size (int): max size (in px) for width or height if given
+            full: if True, set image width to 100%
         """
-        tmp = NamedTemporaryFile(suffix='.'+extension)
-        self.savefig(tmp.name, show=True)
+        svg = self._to_svg(size=size, full=full)
+        display(JupyterSvgImage(svg))
+
+    def _repr_svg_(self):
+        return self._to_svg()
+
 
 class Structure(BasicDraw):
     """Classic VARNA drawing mode. Constructor from given RNA sequence or/and secondary structure.
     If sequence and structure have different size, the larger one is used
     and ` `s or `.`s will be added to sequence or structure to complement.
 
     Args:
@@ -423,17 +474,35 @@
     def _gen_input_cmd(self):
         return ['-sequenceDBN', self.sequence, '-structureDBN', self.format_structure()]
 
     def __repr__(self):
         return repr((self.format_structure(), self.sequence))
 
 
-@deprecated("Class has been renamed 'Structure'")
-def VARNA(*args, **kwargs):
-    return Structure(*args, **kwargs)
+class FileDraw(BasicDraw):
+    """Drawing class with input structure/sequence given by file
+    The simplest input format is dbn format. The file contains two lines: the first line is the sequence and the second one is the structure in dbn.
+    Other supported formats are ct, BPseq, TCoffee, Stockholm, RNAML, as well as Varna session.
+
+    Warning: Position value check disable
+        As input file is passed to VARNA directly without any parsing, the RNA length is unknown.
+        Therefore, all value checks related to position are disable.
+
+    Args:
+        inputfile: path to inputfile
+    """
+    def __init__(self, inputfile):
+        super().__init__()
+        self.inputfile = inputfile
+
+        # Disable interval check
+        self._check_interval = False
+
+    def _gen_input_cmd(self):
+        return ['-i', self.inputfile]
 
 
 class Comparison(BasicDraw):
     """Drawing of two aligned RNAs.
     Unlike classic [Structure][varnaapi.Structure] mode,
     both sequences and structures __MUST__ be specified and have the same size.
     Additionally, the merged secondary structures must currently be without any crossing
```

### Comparing `varnaapi-1.1.1/src/varnaapi/param.py` & `varnaapi-1.2.0/src/varnaapi/param.py`

 * *Files identical despite different names*

### Comparing `varnaapi-1.1.1/src/varnaapi/settings.py` & `varnaapi-1.2.0/src/varnaapi/settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import os
+import logging
 from pathlib import Path
 from importlib.resources import files
 from shutil import copyfile
 import platformdirs
 import yaml
 
 CONFIG_VERSION = 1
 
 CONFIG_ORIGIN = files('varnaapi').joinpath('config-settings-v{}.yml'.format(CONFIG_VERSION))
 CONFIG_DIR = platformdirs.user_config_path('varnaapi', ensure_exists=True)
 CONFIG_USER = Path(CONFIG_DIR, 'config-settings-v{}.yml'.format(CONFIG_VERSION))
 
 CONFIG = {}
 
+
+# Setup logger
+Logger = logging.getLogger("VARNA API")
+
+
+
 def check_settings_exists():
     """Check if configuration file exist, if no create one.
     The function is called when the package is imported
     """
     if not CONFIG_USER.exists():
         copyfile(CONFIG_ORIGIN, CONFIG_USER)
```

### Comparing `varnaapi-1.1.1/src/varnaapi.egg-info/PKG-INFO` & `varnaapi-1.2.0/src/varnaapi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: varnaapi
-Version: 1.1.1
+Version: 1.2.0
 Summary: Python helper for RNA visualization tool VARNA
 Author-email: Hua-Ting Yao <hua-ting.yao@polytechnique.edu>
-Project-URL: Homepage, https://htyao.gitlab.io/varna-api/
+Project-URL: Homepage, https://amibio.gitlabpages.inria.fr/varna-api
 Project-URL: Source Code, https://gitlab.inria.fr/amibio/varna-api
 Project-URL: VARNA, https://varna.lisn.upsaclay.fr/index.php
+Project-URL: Issues, https://github.com/anthonyhtyao/varnaapi/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colour
 Requires-Dist: deprecated
 Requires-Dist: pyyaml
-Requires-Dist: ipython
 Requires-Dist: platformdirs
+Requires-Dist: drawsvg~=2.0
+Requires-Dist: svgpathtools
+Requires-Dist: ipython
 
 VARNA API is a Python interface for [VARNA](http://varna.lri.fr/index.php) (v3-93), a Java lightweight component and applet for drawing the RNA secondary structure.
 VARNA allows users to produce drawing in a non-iteractive way via command line.
 However, the command line might be massive and complicate in some use cases.
 VARNA API aims to simplify such process.
-The [online documentation](https://htyao.gitlab.io/varna-api/) is available.
+The [online documentation](https://amibio.gitlabpages.inria.fr/varna-api/) is available.
 
 !!! danger "Starting from v1.1.0, VARNA API uses _1-indexed_ to count RNA bases. The change aims to better align with VARNA and ViennaRNA."
 
 ## Example
 
 The command below highlights region 11-21 and adds a non-canonical base pair at position (14,20)
 on secondary structure `((((((.((((((........)))))).((((((.......))))))..))))))`.
```

