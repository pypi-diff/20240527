# Comparing `tmp/finlearn-0.0.44.tar.gz` & `tmp/finlearn-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finlearn-0.0.44.tar", last modified: Sat May  4 21:13:21 2024, max compression
+gzip compressed data, was "finlearn-0.0.45.tar", last modified: Mon May 27 17:08:33 2024, max compression
```

## Comparing `finlearn-0.0.44.tar` & `finlearn-0.0.45.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 21:13:21.503519 finlearn-0.0.44/
--rw-rw-rw-   0        0        0      857 2024-05-04 21:13:21.503519 finlearn-0.0.44/PKG-INFO
--rw-rw-rw-   0        0        0      447 2024-05-04 21:12:01.000000 finlearn-0.0.44/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 21:13:21.455344 finlearn-0.0.44/finlearn/
--rw-rw-rw-   0        0        0       28 2024-03-18 20:53:50.000000 finlearn-0.0.44/finlearn/__init__.py
--rw-rw-rw-   0        0        0     5731 2024-05-04 21:11:50.000000 finlearn-0.0.44/finlearn/plotter.py
-drwxrwxrwx   0        0        0        0 2024-05-04 21:13:21.497351 finlearn-0.0.44/finlearn.egg-info/
--rw-rw-rw-   0        0        0      857 2024-05-04 21:13:20.000000 finlearn-0.0.44/finlearn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-05-04 21:13:21.000000 finlearn-0.0.44/finlearn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 21:13:20.000000 finlearn-0.0.44/finlearn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-04 21:13:20.000000 finlearn-0.0.44/finlearn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-04 21:13:20.000000 finlearn-0.0.44/finlearn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 21:13:21.511541 finlearn-0.0.44/setup.cfg
--rw-rw-rw-   0        0        0     1149 2024-05-04 21:13:09.000000 finlearn-0.0.44/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 17:08:33.883960 finlearn-0.0.45/
+-rw-rw-rw-   0        0        0     1460 2024-05-27 17:08:33.855895 finlearn-0.0.45/PKG-INFO
+-rw-rw-rw-   0        0        0      956 2024-05-27 16:43:26.000000 finlearn-0.0.45/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 17:08:33.734157 finlearn-0.0.45/finlearn/
+-rw-rw-rw-   0        0        0       93 2024-05-27 16:12:19.000000 finlearn-0.0.45/finlearn/__init__.py
+-rw-rw-rw-   0        0        0      733 2024-05-27 16:33:29.000000 finlearn-0.0.45/finlearn/check.py
+-rw-rw-rw-   0        0        0     6134 2024-05-27 16:11:47.000000 finlearn-0.0.45/finlearn/plotter.py
+-rw-rw-rw-   0        0        0     2533 2024-05-27 15:51:15.000000 finlearn-0.0.45/finlearn/time_series.py
+drwxrwxrwx   0        0        0        0 2024-05-27 17:08:33.800984 finlearn-0.0.45/finlearn.egg-info/
+-rw-rw-rw-   0        0        0     1460 2024-05-27 17:08:33.000000 finlearn-0.0.45/finlearn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-05-27 17:08:33.000000 finlearn-0.0.45/finlearn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 17:08:33.000000 finlearn-0.0.45/finlearn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-27 17:08:33.000000 finlearn-0.0.45/finlearn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 17:08:33.000000 finlearn-0.0.45/finlearn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 17:08:33.900600 finlearn-0.0.45/setup.cfg
+-rw-rw-rw-   0        0        0     1203 2024-05-27 16:43:39.000000 finlearn-0.0.45/setup.py
```

### Comparing `finlearn-0.0.44/finlearn/plotter.py` & `finlearn-0.0.45/finlearn/plotter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import plotly.graph_objects as go 
+import pandas as pd
 from plotly.subplots import make_subplots
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
+import seaborn as sns
 import yfinance as yf
 
 class plotter:
     def __init__(self):
         pass
 
     
@@ -116,14 +118,21 @@
       ax.set_ylabel('Price')
       ax.set_title('Candlestick Chart for '+ name)
       ax.xaxis.set_major_locator(mdates.MonthLocator())
       ax.xaxis.set_major_formatter(mdates.DateFormatter('%b %Y'))
       plt.xticks(rotation=45)
       plt.tight_layout()
       plt.show()
-    
+      
+    def heatmap(self, name, start, end):
+      '''Downloading the data from yfinance and then using the sns.heatmap feature to generate the correlation between the various
+      parameters of the stock price data'''
+      
+      data = yf.download(name, start=start, end=end)
+      sns.heatmap(data.corr(), annot=True, cmap="crest")
+      plt.show()
```

### Comparing `finlearn-0.0.44/setup.py` & `finlearn-0.0.45/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from setuptools import setup, find_packages
 
 # Package metadata
 NAME = 'finlearn'
 DESCRIPTION = 'A one-stop package for entire financial analysis and market prediction using Deep Learning'
-VERSION = '0.0.44'
+VERSION = '0.0.45'
 AUTHOR = 'Ankit Dutta'
 AUTHOR_EMAIL = 'ankitduttaiitkgp@gmail.com'
-#URL = 'https://github.com/your_username/your_repository'
+URL = 'https://github.com/ankitdutta428/finlearn'
 LICENSE = 'Apache 2.0'
 
 # Read long description from README file
 with open('README.md', 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 # Define dependencies
 INSTALL_REQUIRES = [
     'plotly',
     'yfinance',
-    'matplotlib'
+    'matplotlib',
+    'pandas',
+    'seaborn',
+    'keras',
+    'datetime'
     # Add more dependencies as needed
 ]
 
 # Define additional classifiers
 CLASSIFIERS = [
     'Programming Language :: Python :: 3',
     # Add more classifiers as needed
```

