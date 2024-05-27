# Comparing `tmp/plotly-helper-0.0.8.tar.gz` & `tmp/plotly-helper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plotly-helper-0.0.8.tar", last modified: Mon Aug 30 09:35:02 2021, max compression
+gzip compressed data, was "plotly-helper-0.0.9.tar", last modified: Mon May 27 12:03:38 2024, max compression
```

## Comparing `plotly-helper-0.0.8.tar` & `plotly-helper-0.0.9.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 09:35:02.000000 plotly-helper-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 09:35:02.000000 plotly-helper-0.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      717 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/examples/plot_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)      901 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      140 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/ACKNOWLEDGMENT.md
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 09:35:02.000000 plotly-helper-0.0.8/plotly_helper/
--rw-r--r--   0 runner    (1001) docker     (121)     7750 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/plotly_helper/neuron_viewer.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/plotly_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14802 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/plotly_helper/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3250 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/plotly_helper/object_creator.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/plotly_helper/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/plotly_helper/shapes.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2021-08-30 09:35:02.000000 plotly-helper-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3854 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 09:35:02.000000 plotly-helper-0.0.8/plotly_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-08-30 09:35:01.000000 plotly-helper-0.0.8/plotly_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-08-30 09:35:01.000000 plotly-helper-0.0.8/plotly_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-08-30 09:35:01.000000 plotly-helper-0.0.8/plotly_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      472 2021-08-30 09:35:01.000000 plotly-helper-0.0.8/plotly_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-30 09:35:01.000000 plotly-helper-0.0.8/plotly_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      822 2021-08-30 09:35:02.000000 plotly-helper-0.0.8/plotly_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/COPYING.LESSER
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 09:35:02.000000 plotly-helper-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 09:35:02.000000 plotly-helper-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      536 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (121)      617 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (121)      694 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 09:35:02.000000 plotly-helper-0.0.8/doc/
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 09:35:02.000000 plotly-helper-0.0.8/doc/source/
--rw-r--r--   0 runner    (1001) docker     (121)     4646 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4072 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/doc/source/_common.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 09:35:02.000000 plotly-helper-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      862 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/tests/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (121)    10504 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1691 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/tests/test_neuron_viewer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4215 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/tests/test_object_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-30 09:35:02.000000 plotly-helper-0.0.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)   279908 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/tests/data/neuron.h5
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-30 09:35:02.000000 plotly-helper-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      862 2021-08-30 09:34:37.000000 plotly-helper-0.0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:38.467938 plotly-helper-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:38.463938 plotly-helper-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:38.463938 plotly-helper-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/ACKNOWLEDGMENT.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-27 12:03:38.467938 plotly-helper-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:38.467938 plotly-helper-0.0.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:38.467938 plotly-helper-0.0.9/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/doc/source/_common.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/doc/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:38.467938 plotly-helper-0.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/examples/plot_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:38.467938 plotly-helper-0.0.9/plotly_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/plotly_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/plotly_helper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14952 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/plotly_helper/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/plotly_helper/neuron_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/plotly_helper/object_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/plotly_helper/shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:38.467938 plotly-helper-0.0.9/plotly_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-27 12:03:38.000000 plotly-helper-0.0.9/plotly_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-27 12:03:38.000000 plotly-helper-0.0.9/plotly_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:03:38.000000 plotly-helper-0.0.9/plotly_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 12:03:38.000000 plotly-helper-0.0.9/plotly_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-27 12:03:38.000000 plotly-helper-0.0.9/plotly_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 12:03:38.000000 plotly-helper-0.0.9/plotly_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:03:38.471938 plotly-helper-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:38.467938 plotly-helper-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:03:38.467938 plotly-helper-0.0.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   279908 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/tests/data/neuron.h5
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/tests/test_neuron_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/tests/test_object_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/tests/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-27 12:03:34.000000 plotly-helper-0.0.9/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `plotly-helper-0.0.8/examples/plot_builder.py` & `plotly-helper-0.0.9/examples/plot_builder.py`

 * *Files identical despite different names*

### Comparing `plotly-helper-0.0.8/setup.py` & `plotly-helper-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     author="Blue Brain Project, EPFL",
     description="Package that makes plotly easy",
     url="https://github.com/bluebrain/plotly-helper",
     license="LGPLv3",
     install_requires=[
         'plotly>=3.4.2',
         'numpy>=1.15.4',
-        'neurom>=3.0,<4.0',
+        'neurom>=3.0,<5.0',
         'click>=6.0',
     ],
     extras_require={
         'docs': ['sphinx', 'sphinx-bluebrain-theme'],
     },
     entry_points={
         'console_scripts': ['viewer=plotly_helper.cli:cli']
```

### Comparing `plotly-helper-0.0.8/plotly_helper/neuron_viewer.py` & `plotly-helper-0.0.9/plotly_helper/neuron_viewer.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 NEURON_NAME = 'neuron'
 SOMA_NAME = 'soma'
 
 
 def _neurite_name(neurite, prefix, names):
     '''The neurite name used for the legend'''
     name = str(neurite.type).replace('NeuriteType.', '').replace('_', ' ')
-    return '{} {} {}'.format(prefix, name, names[neurite.type])
+    return f'{prefix} {name} {names[neurite.type]}'
 
 
 # pylint: disable=too-many-locals
 def _make_trace2d(neuron, plane, prefix='', opacity=1., visible=True, style=None, line_width=2):
     '''Create the trace to be plotted'''
     names = defaultdict(int)
-    lines = list()
+    lines = []
     for neurite in iter_neurites(neuron):
         names[neurite.type] += 1
 
         try:
             neurite_color = style[neurite]['color']
         except KeyError:
             neurite_color = TREE_COLOR.get(neurite.root_node.type, 'black')
@@ -45,37 +45,37 @@
             segs = [(s[0][COLS.XYZ], s[1][COLS.XYZ]) for s in iter_segments(section)]
 
             try:
                 colors = style[section]['color']
             except KeyError:
                 colors = neurite_color
 
-            coords = dict()
+            coords = {}
             for i, coord in enumerate('xyz'):
                 coords[coord] = list(chain.from_iterable((p1[i], p2[i], None) for p1, p2 in segs))
 
-            coords = dict(x=coords[plane[0]], y=coords[plane[1]])
+            coords = {'x': coords[plane[0]], 'y': coords[plane[1]]}
             lines.append(go.Scattergl(name=name, visible=visible, opacity=opacity,
                                       showlegend=False,
-                                      line=dict(color=colors, width=line_width),
+                                      line={'color': colors, 'width': line_width},
                                       mode='lines',
                                       **coords))
     return lines
 
 
 # pylint: disable=too-many-locals
 def _make_trace(neuron, plane, prefix='', opacity=1., visible=True, style=None, line_width=2):
     '''Create the trace to be plotted'''
     names = defaultdict(int)
-    lines = list()
+    lines = []
     for neurite in iter_neurites(neuron):
         names[neurite.type] += 1
 
-        coords = dict(x=list(), y=list(), z=list())
-        colors = list()
+        coords = {'x': [], 'y': [], 'z': []}
+        colors = []
 
         try:
             default_color = style[neurite]['color']
         except KeyError:
             default_color = TREE_COLOR.get(neurite.root_node.type, 'black')
 
         for section in iter_sections(neurite):
@@ -92,15 +92,15 @@
                 coords[coord] += list(chain.from_iterable((p1[i], p2[i], None) for p1, p2 in segs)
                                       if coord in plane else
                                       chain.from_iterable((0, 0, None) for _ in segs))
 
         lines.append(go.Scatter3d(name=_neurite_name(neurite, prefix, names),
                                   showlegend=False,
                                   visible=visible, opacity=opacity,
-                                  line=dict(color=colors, width=line_width),
+                                  line={'color': colors, 'width': line_width},
                                   mode='lines',
                                   **coords))
     return lines
 
 
 def _make_soma(neuron):
     ''' Create a 3d surface representing the soma '''
@@ -150,15 +150,15 @@
         self.properties[section]['range'] = slice(start_point, end_point)
         if recursive:
             for child in section.children:
                 self.color_section(child, color, recursive=True)
 
     def get_figure(self):
         '''Build the figure and returns it'''
-        is_3d = (self.helper.plane == 'xyz')
+        is_3d = self.helper.plane == 'xyz'
         if is_3d:
             self.helper.add_data({NEURON_NAME: _make_trace(
                 self.neuron, self.helper.plane, style=self.properties, line_width=self.line_width)})
             self.helper.add_data({SOMA_NAME: _make_soma(self.neuron)})
             # self.helper.add_plane_buttons()
         else:
             self.helper.add_data({NEURON_NAME: _make_trace2d(
```

### Comparing `plotly-helper-0.0.8/plotly_helper/helper.py` & `plotly-helper-0.0.9/plotly_helper/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,43 +14,49 @@
 
 class PlotlyHelper:
     """Class to help creating plotly plots with shapes, buttons and data """
 
     def __init__(self, title, layout=None):
         self.title = title
         self.layout = layout if layout else self._get_standard_layout(title)
-        self.data = list()
-        self.visibility_map = dict()
-        self.updatemenus = list()
-        self.shapes = list()
+        self.data = []
+        self.visibility_map = {}
+        self.updatemenus = []
+        self.shapes = []
         self.nb_objects = 0
-        self.button_group_to_index = dict()
+        self.button_group_to_index = {}
         self.button_group_index = -1
 
     @staticmethod
     def _get_standard_layout(title):
         """ Return a very simple layout with a title and legend's setup """
-        return dict(autosize=True, title=title,
-                    legend=PlotlyHelper._get_legend())
+        return {'autosize': True, 'title': title,
+                'legend': PlotlyHelper._get_legend(),
+                }
 
     @staticmethod
     def _get_legend():
         """ Returns the legend dict already setup for the plot """
-        return dict(x=0.8, y=1, traceorder='normal',
-                    font=dict(family='sans-serif', size=12, color='#000'),
-                    bgcolor='#FFFFFF', bordercolor='#FFFFFF', borderwidth=2)
+        return {'x': 0.8, 'y': 1, 'traceorder': 'normal',
+                'font': {'family': 'sans-serif', 'size': 12, 'color': '#000'},
+                'bgcolor': '#FFFFFF', 'bordercolor': '#FFFFFF', 'borderwidth': 2}
 
     @staticmethod
     def _get_button_skeleton(direction='down'):
         """ Returns the skeleton dict for buttons
 
         Args:
             direction: the direction for the button layout (default=down)
         """
-        return dict(type='dropdown', direction=direction, xanchor='left', active=0, buttons=list())
+        return {'type': 'dropdown',
+                'direction': direction,
+                'xanchor': 'left',
+                'active': 0,
+                'buttons': [],
+                }
 
     def _add_button_group(self, name, direction='down'):
         """ Add a button group to the plot
 
         Args:
             name: the button group name (str)
             direction: the direction for the button layout (default=down)
@@ -70,15 +76,15 @@
             name: the id used to name a group of plotly object (str)
             objs: a list containing the plotly objects included in the group 'name'
 
         Raises:
             ValueError: An error occurs if name shadows a previous entry name
         """
         if name in self.visibility_map:
-            raise ValueError('{} already exists'.format(name))
+            raise ValueError(f'{name} already exists')
         self.visibility_map[name] = range(len(self.data), len(self.data) + len(objs))
 
     def _place_buttons(self, offset=0.01):
         """ Place the buttons using the update menu from plotly """
         y_position = 1
         for group in self.updatemenus:
             group['y'] = y_position
@@ -128,30 +134,30 @@
         Raises:
             TypeError: if obj_groups is not a dict
             TypeError: if an item in obj_groups is not a BaseTraceType
             TypeError: if a key in obj_groups is not a string_type
             ValueError: if an item is empty
         """
         if not isinstance(obj_groups, dict):
-            raise TypeError('can t add {} to helper. Must be a dict'.format(obj_groups))
+            raise TypeError(f"can't add {obj_groups} to helper. Must be a dict")
 
         def _obj_validator(current_obj):
             if not isinstance(current_obj, BaseTraceType):
-                raise TypeError('can t add {} to helper'.format(current_obj))
+                raise TypeError(f"can't add {current_obj} to helper")
 
         for name, obj_group in obj_groups.items():
             if not isinstance(name, str):
-                raise TypeError('bad name {} for object'.format(name))
+                raise TypeError(f'bad name {name} for object')
 
             if not isinstance(obj_group, (list, BaseTraceType)):
-                raise TypeError('bad obj_group {} for name'.format(name))
+                raise TypeError(f'bad obj_group {name} for name')
 
             if isinstance(obj_group, list):
                 if not obj_group:
-                    raise ValueError('{} object is empty'.format(name))
+                    raise ValueError(f'{name} object is empty')
                 for obj in obj_group:
                     _obj_validator(obj)
 
     def add_data(self, obj_groups):
         """ Add plotly data to the plot and update its visibility map
 
         Args:
@@ -181,15 +187,15 @@
 
         Note:
             This function keeps recompute the number of object and visibility_map for all objects
         """
 
         def _remove_visibility(visibility_map, obj_name):
             if obj_name not in visibility_map:
-                raise ValueError('{} must exists'.format(obj_name))
+                raise ValueError(f'{obj_name} must exists')
             to_removed_range = visibility_map.pop(obj_name)
             for c_name, obj_range in self.visibility_map.items():
                 if obj_range[0] > to_removed_range[-1]:
                     c_range = list(visibility_map[c_name])
                     start = c_range[0] - len(to_removed_range)
                     stop = c_range[-1] - len(to_removed_range) + 1
                     visibility_map[c_name] = range(start, stop)
@@ -226,26 +232,26 @@
 
         Notes:
             Buttons are grouped thanks to the groupname variable. If you add some update button
             you need to do it after including all your data.
         """
         self._add_button_group(groupname, direction)
         index = self.button_group_to_index[groupname]
-        self.updatemenus[index]['buttons'].append(dict(label=label, method=method, args=args))
+        self.updatemenus[index]['buttons'].append({'label': label, 'method': method, 'args': args})
 
     def get_fig(self):
         """ Return the final figure
 
         Notes:
             you can use in the plotly.offline.(i)plot functions
         """
         self._place_buttons()
         self.layout['updatemenus'] = self.updatemenus
         self.layout['shapes'] = self.shapes
-        return dict(data=self.data, layout=self.layout)
+        return {'data': self.data, 'layout': self.layout}
 
 
 class PlotlyHelperPlane(PlotlyHelper):
     """ Helper to create plotly figure with plane helpers """
 
     def __init__(self, title, plane):
         self.plane = self._sanitize_plane(plane)
@@ -256,15 +262,15 @@
     def _get_title(title, plane):
         """ Return the title with the correct plane name
 
         Args:
             title: the title for the plot.
             plane: the sanitized plane used for this plot
         """
-        return '{}-{}'.format(title, plane)
+        return f'{title}-{plane}'
 
     @staticmethod
     def _sanitize_plane(plane):
         """ sanitizer for the plane input
 
         Args:
             plane: a string that should be a combination of 'x', 'y' or 'z'
@@ -301,18 +307,21 @@
         Args:
             plane: a string that should be a combination of 'x', 'y' or 'z'
 
         Notes:
             For 2d scene the camera is simply positioned in such a way that for xy plane, the
             x axis is from left to right and y for bottom to up.
         """
-        camera = dict(up=dict(x=0, y=0, z=0), center=dict(x=0, y=0, z=0), eye=dict(x=0, y=0, z=0))
+        camera = {'up': {'x': 0, 'y': 0, 'z': 0},
+                  'center': {'x': 0, 'y': 0, 'z': 0},
+                  'eye': {'x': 0, 'y': 0, 'z': 0},
+                  }
         if plane == 'xyz':
-            camera['up'] = dict(x=0, y=0, z=1)
-            camera['eye'] = dict(x=-1.7428, y=1.0707, z=0.7100, )
+            camera['up'] = {'x': 0, 'y': 0, 'z': 1}
+            camera['eye'] = {'x': -1.7428, 'y': 1.0707, 'z': 0.7100, }
         else:
             unit = {v: np.eye(3)[i] for i, v in enumerate('xyz')}
             sign_cross = np.sum(np.sign(np.cross(unit[plane[0]], unit[plane[1]])))
             camera['eye'][list(set('xyz') - set(plane))[0]] = sign_cross * 2
             camera['up'][plane[1]] = 1
         return camera
 
@@ -325,33 +334,33 @@
 
         Notes:
             For 2d scene the camera is simply positioned in such a way that for xy plane, the
             x axis is from left to right and y for bottom to up.
             The colors for the planes, background etc are set here.
         """
         dragmode = 'zoom' if plane != 'xyz' else 'turntable'
-        scene = dict(xaxis=None, yaxis=None, zaxis=None, aspectmode='data',
-                     dragmode=dragmode, camera=PlotlyHelperPlane._get_camera(plane))
+        scene = {'xaxis': None, 'yaxis': None, 'zaxis': None, 'aspectmode': 'data',
+                 'dragmode': dragmode, 'camera': PlotlyHelperPlane._get_camera(plane)}
         for axis in 'xyz':
             axis_name = axis + 'axis'
-            scene[axis_name] = dict(
-                gridcolor='rgb(255, 255, 255)',
-                zerolinecolor='rgb(255, 255, 255)',
-                showbackground=True,
-                backgroundcolor='rgb(238, 238,238)',
-                visible=True,
-            )
+            scene[axis_name] = {
+                'gridcolor': 'rgb(255, 255, 255)',
+                'zerolinecolor': 'rgb(255, 255, 255)',
+                'showbackground': True,
+                'backgroundcolor': 'rgb(238, 238,238)',
+                'visible': True,
+            }
         return scene
 
     @staticmethod
     def _get_layout_skeleton(title, plane):
         """ Returns a layout skeleton that is camera compliant """
-        layout = dict(autosize=True, title=title,
-                      scene=PlotlyHelperPlane._get_scene(plane),
-                      legend=PlotlyHelperPlane._get_legend())
+        layout = {'autosize': True, 'title': title,
+                  'scene': PlotlyHelperPlane._get_scene(plane),
+                  'legend': PlotlyHelperPlane._get_legend()}
         return layout
 
     def add_plane_buttons(self):
         """ Add the plane buttons to the plot """
         if self.plane == 'xyz':
             self.add_button('3D view', 'relayout', ['scene', PlotlyHelperPlane._get_scene('xyz')],
                             'view', 'right')
```

### Comparing `plotly-helper-0.0.8/plotly_helper/object_creator.py` & `plotly-helper-0.0.9/plotly_helper/object_creator.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,18 +14,18 @@
         showlegend: boolean to add object to the legend
         opacity: set the opacity value (float)
         marker_size: size of marker (set to small value to get lines)
 
     Returns :
         A scatter plot representing points
     """
-    args = dict(visible=visible, marker=dict(size=marker_size, color=color),
-                line=dict(width=width, color=color),
-                x=points[:, 0], y=points[:, 1],
-                showlegend=showlegend, opacity=opacity)
+    args = {'visible': visible, 'marker': {'size': marker_size, 'color': color},
+            'line': {'width': width, 'color': color},
+            'x': points[:, 0], 'y': points[:, 1],
+            'showlegend': showlegend, 'opacity': opacity}
 
     if points.shape[1] == 3:
         scatter_fun = go.Scatter3d
         args['z'] = points[:, 2]
     else:
         scatter_fun = go.Scattergl
 
@@ -45,19 +45,19 @@
         showlegend: boolean to add object to the legend
         opacity: set the opacity value (float)
 
     Returns :
         A scatter plot representing points
     """
     obj = scatter_line(points, name, color, width, visible, showlegend, opacity)
-    marker = dict(
-        line=dict(width=width, color=color),
-        color=color,
-        size=width,
-    )
+    marker = {
+        'line': {'width': width, 'color': color},
+        'color': color,
+        'size': width,
+    }
     obj['marker'] = marker
     obj.mode = 'markers'
     return obj
 
 
 # pylint: disable=redefined-outer-name
 def point(point, name=None, color=None, width=5, visible=True, showlegend=True, opacity=1.0):
```

### Comparing `plotly-helper-0.0.8/plotly_helper/shapes.py` & `plotly-helper-0.0.9/plotly_helper/shapes.py`

 * *Files identical despite different names*

### Comparing `plotly-helper-0.0.8/CONTRIBUTING.md` & `plotly-helper-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `plotly-helper-0.0.8/plotly_helper.egg-info/SOURCES.txt` & `plotly-helper-0.0.9/plotly_helper.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .gitignore
 .pylintrc
 ACKNOWLEDGMENT.md
+AUTHORS.txt
 CONTRIBUTING.md
 COPYING
 COPYING.LESSER
 MANIFEST.in
 README.rst
 setup.py
 tox.ini
```

### Comparing `plotly-helper-0.0.8/COPYING` & `plotly-helper-0.0.9/COPYING`

 * *Files identical despite different names*

### Comparing `plotly-helper-0.0.8/COPYING.LESSER` & `plotly-helper-0.0.9/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `plotly-helper-0.0.8/.github/workflows/run-tox.yml` & `plotly-helper-0.0.9/.github/workflows/run-tox.yml`

 * *Files 26% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.6,3.7]
+        python-version: ['3.8', '3.9', '3.10', '3.11']
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
+
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools
         pip install tox-gh-actions
+
     - name: Run tox
       run: |
         tox
```

### Comparing `plotly-helper-0.0.8/.github/workflows/publish-sdist.yml` & `plotly-helper-0.0.9/.github/workflows/publish-sdist.yml`

 * *Files 22% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 jobs:
   build-n-publish:
     name: Build and publish on PyPI
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@master
-      - name: Set up Python 3.6
+      - name: Set up Python 3.8
         uses: actions/setup-python@v2
         with:
-          python-version: 3.6
+          python-version: 3.8
       - name: Build a source tarball
         run:
             python setup.py sdist
 
       - name: Publish distribution package to PyPI
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `plotly-helper-0.0.8/README.rst` & `plotly-helper-0.0.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
 License
 =======
 
 plotly-helper is licensed under the terms of the GNU Lesser General Public License version 3.
 Refer to COPYING.LESSER and COPYING for details.
 
-Copyright (c) 2018-2021 Blue Brain Project/EPFL
+Copyright (c) 2018-2024 Blue Brain Project/EPFL
```

### Comparing `plotly-helper-0.0.8/doc/Makefile` & `plotly-helper-0.0.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `plotly-helper-0.0.8/doc/source/index.rst` & `plotly-helper-0.0.9/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `plotly-helper-0.0.8/doc/source/conf.py` & `plotly-helper-0.0.9/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `plotly-helper-0.0.8/tests/test_neuron_viewer.py` & `plotly-helper-0.0.9/tests/test_neuron_viewer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 import os
-from mock import patch
+from unittest.mock import patch
 
 from neurom import load_morphology
 from plotly_helper.neuron_viewer import NeuronBuilder
 
-from nose.tools import assert_dict_equal, assert_equal
 PATH = os.path.dirname(__file__)
 
 # patching plotly.offline.plot to avoid the call
 @patch('plotly_helper.neuron_viewer.plot_')
 def test_color_section(_):
     neuron = load_morphology(os.path.join(PATH, '..', 'tests', 'data', 'neuron.h5'))
 
     # Colorize first section of the neurite
     builder = NeuronBuilder(neuron, '3d')
     builder.color_section(neuron.neurites[1].root_node)
-    assert_equal(len(builder.properties.values()), 1)
-    assert_dict_equal(next(iter(builder.properties.values())),
+    assert len(builder.properties.values()) == 1
+    assert (next(iter(builder.properties.values())) ==
                       {'color': 'green', 'range': slice(0, 23, None)})
     builder.plot()
 
     # Colorize alls sections of the neurite
     builder = NeuronBuilder(neuron, '3d')
     section = neuron.neurites[2].root_node
     builder.color_section(section, color='gray', recursive=True)
-    assert_equal(len(builder.properties.values()), 27)
+    assert len(builder.properties.values()) == 27
     builder.plot()
 
     # Colorize only a fraction of the section
     builder = NeuronBuilder(neuron, '3d')
     builder.color_section(neuron.sections[159], color='black', start_point=20, end_point=120)
-    assert_dict_equal(next(iter(builder.properties.values())),
+    assert (next(iter(builder.properties.values())) ==
                       {'color': 'black', 'range': slice(20, 120, None)})
     builder.plot()
 
 
     # 2d
     builder = NeuronBuilder(neuron, 'xy')
     builder.color_section(neuron.neurites[1].root_node)
-    assert_equal(len(builder.properties.values()), 1)
-    assert_dict_equal(next(iter(builder.properties.values())),
+    assert len(builder.properties.values()) == 1
+    assert (next(iter(builder.properties.values())) ==
                       {'color': 'green', 'range': slice(0, 23, None)})
     builder.plot()
```

### Comparing `plotly-helper-0.0.8/tests/test_object_creator.py` & `plotly-helper-0.0.9/tests/test_object_creator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import nose.tools as nt
 import numpy as np
 import numpy.testing as npt
 
 import plotly_helper.object_creator as object_creator
 
 
 def test_create_scatter_line():
@@ -19,15 +18,15 @@
                 'z': np.array([0, 1, 2]),
                 'type': 'scatter3d'}
 
     # can't dict equal with numpy array. Remove and test them and then test the dict.
     npt.assert_array_equal(good_obj.pop('x'), obj.pop('x'))
     npt.assert_array_equal(good_obj.pop('y'), obj.pop('y'))
     npt.assert_array_equal(good_obj.pop('z'), obj.pop('z'))
-    nt.assert_dict_equal(obj, good_obj)
+    assert obj == good_obj
 
 
 def test_scatter_line_2():
     points = np.array([[0, 0, 0], [1, 1, 1], [2, 2, 2]])
     obj = object_creator.scatter_line(points).to_plotly_json()
     good_obj = {'line': {'width': 5},
                 'marker': {'size': 3},
@@ -39,15 +38,15 @@
                 'z': np.array([0, 1, 2]),
                 'type': 'scatter3d'}
 
     # can't dict equal with numpy array. Remove and test them and then test the dict.
     npt.assert_array_equal(good_obj.pop('x'), obj.pop('x'))
     npt.assert_array_equal(good_obj.pop('y'), obj.pop('y'))
     npt.assert_array_equal(good_obj.pop('z'), obj.pop('z'))
-    nt.assert_dict_equal(obj, good_obj)
+    assert obj == good_obj
 
 def test_scatter():
     points = np.array([[0, 0, 0], [1, 1, 1], [2, 2, 2]])
     obj = object_creator.scatter(points).to_plotly_json()
     good_obj = {'mode': 'markers',
                 'line': {'width': 5},
                 'marker': {'line': {'width': 5}, 'size': 5},
@@ -59,15 +58,15 @@
                 'z': np.array([0, 1, 2]),
                 'type': 'scatter3d'}
 
     # can't dict equal with numpy array. Remove and test them and then test the dict.
     npt.assert_array_equal(good_obj.pop('x'), obj.pop('x'))
     npt.assert_array_equal(good_obj.pop('y'), obj.pop('y'))
     npt.assert_array_equal(good_obj.pop('z'), obj.pop('z'))
-    nt.assert_dict_equal(obj, good_obj)
+    assert obj == good_obj
 
 
 def test_point():
     point = np.array([1, 1, 1])
     obj = object_creator.point(point).to_plotly_json()
     good_obj = {'mode': 'markers',
                 'line': {'width': 5},
@@ -80,15 +79,15 @@
                 'z': np.array([1]),
                 'type': 'scatter3d'}
 
     # can't dict equal with numpy array. Remove and test them and then test the dict.
     npt.assert_array_equal(good_obj.pop('x'), obj.pop('x'))
     npt.assert_array_equal(good_obj.pop('y'), obj.pop('y'))
     npt.assert_array_equal(good_obj.pop('z'), obj.pop('z'))
-    nt.assert_dict_equal(obj, good_obj)
+    assert obj == good_obj
 
 
 def test_vector():
     point1 = np.array([1, 1, 1])
     point2 = np.array([2, 2, 2])
 
     obj = object_creator.vector(point1, point2).to_plotly_json()
@@ -102,8 +101,8 @@
                 'z': np.array([1, 2]),
                 'type': 'scatter3d'}
 
     # can't dict equal with numpy array. Remove and test them and then test the dict.
     npt.assert_array_equal(good_obj.pop('x'), obj.pop('x'))
     npt.assert_array_equal(good_obj.pop('y'), obj.pop('y'))
     npt.assert_array_equal(good_obj.pop('z'), obj.pop('z'))
-    nt.assert_dict_equal(obj, good_obj)
+    assert obj == good_obj
```

### Comparing `plotly-helper-0.0.8/tests/data/neuron.h5` & `plotly-helper-0.0.9/tests/data/neuron.h5`

 * *Files identical despite different names*

### Comparing `plotly-helper-0.0.8/tox.ini` & `plotly-helper-0.0.9/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 [base]
 name = plotly_helper
 testdeps =
-    mock
-    nose
+    pytest
 
 [tox]
 envlist =
     {py36,py37,py38}
     check-dist
     lint
     docs
     coverage
 
 [testenv]
 deps = {[base]testdeps}
-commands = nosetests tests
+allowlist_externals = pytest
+commands = pytest tests
 
 [testenv:lint]
 deps =
-     {[base]testdeps}
-     pycodestyle
-     pylint
+    {[base]testdeps}
+    pycodestyle
+    pylint
 commands =
     pycodestyle {[base]name} --exclude tests
     pylint {[base]name} --ignore tests
 
 [testenv:coverage]
 deps =
     {[base]testdeps}
-    coverage
+    pytest-cov
+    coverage[toml]
 commands =
-    coverage run --source {[base]name} {envbindir}/nosetests
-    coverage report --show-missing
+    python -m pytest -vs --cov={[base]name} tests {posargs}
     coverage xml
+    coverage html
 
 [testenv:docs]
 changedir = doc
 extras = docs
 deps = sphinx
 commands = make html
-whitelist_externals = make
+allowlist_externals = make
 
 # E731: do not assign a lambda expression, use a def
 # W503: line break after binary operator
 # W504: line break before binary operator
 [pycodestyle]
 ignore = E731,W503,W504
 max-line-length = 100
```

