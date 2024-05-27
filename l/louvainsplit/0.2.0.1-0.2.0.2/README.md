# Comparing `tmp/louvainsplit-0.2.0.1.tar.gz` & `tmp/louvainsplit-0.2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "louvainsplit-0.2.0.1.tar", last modified: Mon May 27 01:26:13 2024, max compression
+gzip compressed data, was "louvainsplit-0.2.0.2.tar", last modified: Mon May 27 01:43:06 2024, max compression
```

## Comparing `louvainsplit-0.2.0.1.tar` & `louvainsplit-0.2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 01:26:13.745212 louvainsplit-0.2.0.1/
--rw-rw-rw-   0        0        0     1119 2024-05-26 14:11:51.000000 louvainsplit-0.2.0.1/LICENCE
--rw-rw-rw-   0        0        0     5332 2024-05-27 01:26:13.737215 louvainsplit-0.2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4439 2024-05-27 01:19:46.000000 louvainsplit-0.2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 01:26:13.719210 louvainsplit-0.2.0.1/louvainsplit/
--rw-rw-rw-   0        0        0      160 2024-05-26 14:22:35.000000 louvainsplit-0.2.0.1/louvainsplit/__init__.py
--rw-rw-rw-   0        0        0     1347 2024-05-26 14:22:48.000000 louvainsplit-0.2.0.1/louvainsplit/feature_extraction.py
--rw-rw-rw-   0        0        0      819 2024-05-26 14:22:59.000000 louvainsplit-0.2.0.1/louvainsplit/louvain_algorithm.py
-drwxrwxrwx   0        0        0        0 2024-05-27 01:26:13.734209 louvainsplit-0.2.0.1/louvainsplit/tests/
--rw-rw-rw-   0        0        0        0 2024-05-26 14:21:04.000000 louvainsplit-0.2.0.1/louvainsplit/tests/__init__.py
--rw-rw-rw-   0        0        0      555 2024-05-26 14:23:19.000000 louvainsplit-0.2.0.1/louvainsplit/tests/test_louvain_algorithm.py
-drwxrwxrwx   0        0        0        0 2024-05-27 01:26:13.735209 louvainsplit-0.2.0.1/louvainsplit.egg-info/
--rw-rw-rw-   0        0        0     5332 2024-05-27 01:26:13.000000 louvainsplit-0.2.0.1/louvainsplit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2024-05-27 01:26:13.000000 louvainsplit-0.2.0.1/louvainsplit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 01:26:13.000000 louvainsplit-0.2.0.1/louvainsplit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-27 01:26:13.000000 louvainsplit-0.2.0.1/louvainsplit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-27 01:26:13.000000 louvainsplit-0.2.0.1/louvainsplit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 01:26:13.745212 louvainsplit-0.2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1231 2024-05-27 01:26:00.000000 louvainsplit-0.2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:43:06.786962 louvainsplit-0.2.0.2/
+-rw-rw-rw-   0        0        0     1119 2024-05-26 14:11:51.000000 louvainsplit-0.2.0.2/LICENCE
+-rw-rw-rw-   0        0        0     5295 2024-05-27 01:43:06.784960 louvainsplit-0.2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4402 2024-05-27 01:41:51.000000 louvainsplit-0.2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 01:43:06.744962 louvainsplit-0.2.0.2/louvainsplit/
+-rw-rw-rw-   0        0        0      160 2024-05-26 14:22:35.000000 louvainsplit-0.2.0.2/louvainsplit/__init__.py
+-rw-rw-rw-   0        0        0     1347 2024-05-26 14:22:48.000000 louvainsplit-0.2.0.2/louvainsplit/feature_extraction.py
+-rw-rw-rw-   0        0        0      819 2024-05-26 14:22:59.000000 louvainsplit-0.2.0.2/louvainsplit/louvain_algorithm.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:43:06.782975 louvainsplit-0.2.0.2/louvainsplit/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-26 14:21:04.000000 louvainsplit-0.2.0.2/louvainsplit/tests/__init__.py
+-rw-rw-rw-   0        0        0      555 2024-05-26 14:23:19.000000 louvainsplit-0.2.0.2/louvainsplit/tests/test_louvain_algorithm.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:43:06.783961 louvainsplit-0.2.0.2/louvainsplit.egg-info/
+-rw-rw-rw-   0        0        0     5295 2024-05-27 01:43:06.000000 louvainsplit-0.2.0.2/louvainsplit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2024-05-27 01:43:06.000000 louvainsplit-0.2.0.2/louvainsplit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 01:43:06.000000 louvainsplit-0.2.0.2/louvainsplit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-27 01:43:06.000000 louvainsplit-0.2.0.2/louvainsplit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-27 01:43:06.000000 louvainsplit-0.2.0.2/louvainsplit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 01:43:06.786962 louvainsplit-0.2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1231 2024-05-27 01:42:08.000000 louvainsplit-0.2.0.2/setup.py
```

### Comparing `louvainsplit-0.2.0.1/LICENCE` & `louvainsplit-0.2.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `louvainsplit-0.2.0.1/PKG-INFO` & `louvainsplit-0.2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: louvainsplit
-Version: 0.2.0.1
+Version: 0.2.0.2
 Summary: Efficient graph partitioning using LouvainSplit algorithm
 Home-page: https://github.com/mehrdaddjavadi/louvainsplit
 Author: Mehrdad Javadi
 Author-email: mehrdaddjavadi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -64,34 +64,32 @@
 Louvain Algorithm Integration: Utilizes the Louvain algorithm for efficient community detection based on cosine similarities of node feature vectors.
 
 ## Functions and Methods
 construct_feature_pyramid(graph, num_levels)
 Constructs a feature pyramid representation of the input graph.
 
 Parameters:
+
 graph: A NetworkX graph object.
 num_levels: The number of levels in the feature pyramid.
 Returns: A list of tensors representing the feature pyramid.
 extract_basic_features(graph)
 Extracts basic features from the input graph.
 
-Parameters:
 graph: A NetworkX graph object.
 Returns: A list of basic features [num_nodes, num_edges, avg_degree clustering_coefficient].
 extract_abstract_features(graph, level)
 Extracts abstract features from the input graph at the specified level.
 
-Parameters:
 graph: A NetworkX graph object.
 level: The granularity level for feature extraction.
 Returns: A tensor of abstract features.
 louvain_algorithm(feature_pyramid, num_clusters, similarity_measure='cosine')
 Applies the Louvain algorithm to partition the graph based on the feature pyramid.
 
-Parameters:
 feature_pyramid: A list of tensors representing the feature pyramid.
 num_clusters: The number of clusters to partition the graph into.
 similarity_measure: The similarity measure to use (cosine is currently supported).
 Returns: A list of partitions, where each partition is a list of node indices.
```

### Comparing `louvainsplit-0.2.0.1/README.md` & `louvainsplit-0.2.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,34 +40,32 @@
 Louvain Algorithm Integration: Utilizes the Louvain algorithm for efficient community detection based on cosine similarities of node feature vectors.
 
 ## Functions and Methods
 construct_feature_pyramid(graph, num_levels)
 Constructs a feature pyramid representation of the input graph.
 
 Parameters:
+
 graph: A NetworkX graph object.
 num_levels: The number of levels in the feature pyramid.
 Returns: A list of tensors representing the feature pyramid.
 extract_basic_features(graph)
 Extracts basic features from the input graph.
 
-Parameters:
 graph: A NetworkX graph object.
 Returns: A list of basic features [num_nodes, num_edges, avg_degree clustering_coefficient].
 extract_abstract_features(graph, level)
 Extracts abstract features from the input graph at the specified level.
 
-Parameters:
 graph: A NetworkX graph object.
 level: The granularity level for feature extraction.
 Returns: A tensor of abstract features.
 louvain_algorithm(feature_pyramid, num_clusters, similarity_measure='cosine')
 Applies the Louvain algorithm to partition the graph based on the feature pyramid.
 
-Parameters:
 feature_pyramid: A list of tensors representing the feature pyramid.
 num_clusters: The number of clusters to partition the graph into.
 similarity_measure: The similarity measure to use (cosine is currently supported).
 Returns: A list of partitions, where each partition is a list of node indices.
```

### Comparing `louvainsplit-0.2.0.1/louvainsplit/feature_extraction.py` & `louvainsplit-0.2.0.2/louvainsplit/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `louvainsplit-0.2.0.1/louvainsplit/louvain_algorithm.py` & `louvainsplit-0.2.0.2/louvainsplit/louvain_algorithm.py`

 * *Files identical despite different names*

### Comparing `louvainsplit-0.2.0.1/louvainsplit/tests/test_louvain_algorithm.py` & `louvainsplit-0.2.0.2/louvainsplit/tests/test_louvain_algorithm.py`

 * *Files identical despite different names*

### Comparing `louvainsplit-0.2.0.1/louvainsplit.egg-info/PKG-INFO` & `louvainsplit-0.2.0.2/louvainsplit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: louvainsplit
-Version: 0.2.0.1
+Version: 0.2.0.2
 Summary: Efficient graph partitioning using LouvainSplit algorithm
 Home-page: https://github.com/mehrdaddjavadi/louvainsplit
 Author: Mehrdad Javadi
 Author-email: mehrdaddjavadi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -64,34 +64,32 @@
 Louvain Algorithm Integration: Utilizes the Louvain algorithm for efficient community detection based on cosine similarities of node feature vectors.
 
 ## Functions and Methods
 construct_feature_pyramid(graph, num_levels)
 Constructs a feature pyramid representation of the input graph.
 
 Parameters:
+
 graph: A NetworkX graph object.
 num_levels: The number of levels in the feature pyramid.
 Returns: A list of tensors representing the feature pyramid.
 extract_basic_features(graph)
 Extracts basic features from the input graph.
 
-Parameters:
 graph: A NetworkX graph object.
 Returns: A list of basic features [num_nodes, num_edges, avg_degree clustering_coefficient].
 extract_abstract_features(graph, level)
 Extracts abstract features from the input graph at the specified level.
 
-Parameters:
 graph: A NetworkX graph object.
 level: The granularity level for feature extraction.
 Returns: A tensor of abstract features.
 louvain_algorithm(feature_pyramid, num_clusters, similarity_measure='cosine')
 Applies the Louvain algorithm to partition the graph based on the feature pyramid.
 
-Parameters:
 feature_pyramid: A list of tensors representing the feature pyramid.
 num_clusters: The number of clusters to partition the graph into.
 similarity_measure: The similarity measure to use (cosine is currently supported).
 Returns: A list of partitions, where each partition is a list of node indices.
```

### Comparing `louvainsplit-0.2.0.1/setup.py` & `louvainsplit-0.2.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='louvainsplit',
-    version='0.2.0.1',
+    version='0.2.0.2',
     description='Efficient graph partitioning using LouvainSplit algorithm',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Mehrdad Javadi',
     author_email='mehrdaddjavadi@gmail.com',
     url='https://github.com/mehrdaddjavadi/louvainsplit',
     packages=find_packages(),
```

