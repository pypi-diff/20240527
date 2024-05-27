# Comparing `tmp/cellcharter-0.2.0.tar.gz` & `tmp/cellcharter-0.2.1.tar.gz`

## Comparing `cellcharter-0.2.0.tar` & `cellcharter-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 cellcharter-0.2.0/.codecov.yaml
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 cellcharter-0.2.0/.cruft.json
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 cellcharter-0.2.0/.editorconfig
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 cellcharter-0.2.0/.flake8
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 cellcharter-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 cellcharter-0.2.0/.pre-commit-config.yaml.rej
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 cellcharter-0.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 cellcharter-0.2.0/.readthedocs.yaml.rej
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cellcharter-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cellcharter-0.2.0/README.md.rej
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 cellcharter-0.2.0/pyproject.toml.rej
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 cellcharter-0.2.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 cellcharter-0.2.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 cellcharter-0.2.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 cellcharter-0.2.0/.github/workflows/build.yaml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cellcharter-0.2.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 cellcharter-0.2.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/_utils.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/_constants/_pkg_constants.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/datasets/__init__.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/datasets/_dataset.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/gr/__init__.py
--rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/gr/_aggr.py
--rw-r--r--   0        0        0     7288 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/gr/_build.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/gr/_group.py
--rw-r--r--   0        0        0    12682 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/gr/_nhood.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/gr/_utils.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/pl/__init__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/pl/_autok.py
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/pl/_group.py
--rw-r--r--   0        0        0     7997 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/pl/_nhood.py
--rw-r--r--   0        0        0     8546 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/pl/_shape.py
--rw-r--r--   0        0        0    12194 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/pl/_utils.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/tl/__init__.py
--rw-r--r--   0        0        0    15332 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/tl/_autok.py
--rw-r--r--   0        0        0    12816 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/tl/_gmm.py
--rw-r--r--   0        0        0    16599 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/tl/_shape.py
--rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/tl/_trvae.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 cellcharter-0.2.0/src/cellcharter/tl/_utils.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 cellcharter-0.2.0/.gitignore
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 cellcharter-0.2.0/LICENSE
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 cellcharter-0.2.0/README.md
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 cellcharter-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6725 2020-02-02 00:00:00.000000 cellcharter-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 cellcharter-0.2.1/.codecov.yaml
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 cellcharter-0.2.1/.cruft.json
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 cellcharter-0.2.1/.editorconfig
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 cellcharter-0.2.1/.flake8
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 cellcharter-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 cellcharter-0.2.1/.pre-commit-config.yaml.rej
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 cellcharter-0.2.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 cellcharter-0.2.1/.readthedocs.yaml.rej
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cellcharter-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 cellcharter-0.2.1/README.md.rej
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cellcharter-0.2.1/pyproject.toml.rej
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 cellcharter-0.2.1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 cellcharter-0.2.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 cellcharter-0.2.1/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 cellcharter-0.2.1/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 cellcharter-0.2.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 cellcharter-0.2.1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 cellcharter-0.2.1/.github/workflows/test.yaml.rej
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/_utils.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/_constants/_pkg_constants.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/datasets/__init__.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/datasets/_dataset.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/gr/__init__.py
+-rw-r--r--   0        0        0     6017 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/gr/_aggr.py
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/gr/_build.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/gr/_group.py
+-rw-r--r--   0        0        0    13020 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/gr/_nhood.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/gr/_utils.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/pl/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/pl/_autok.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/pl/_group.py
+-rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/pl/_nhood.py
+-rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/pl/_shape.py
+-rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/pl/_utils.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/tl/__init__.py
+-rw-r--r--   0        0        0    15332 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/tl/_autok.py
+-rw-r--r--   0        0        0    12816 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/tl/_gmm.py
+-rw-r--r--   0        0        0    16677 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/tl/_shape.py
+-rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/tl/_trvae.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 cellcharter-0.2.1/src/cellcharter/tl/_utils.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 cellcharter-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 cellcharter-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 cellcharter-0.2.1/README.md
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 cellcharter-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 cellcharter-0.2.1/PKG-INFO
```

### Comparing `cellcharter-0.2.0/.cruft.json` & `cellcharter-0.2.1/.cruft.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7901041666666667%*

 * *Differences: {"'checkout'": "'v0.4.0'",*

 * * "'commit'": "'87a407a65408d75a949c0b54b19fd287475a56f8'",*

 * * "'context'": "{'cookiecutter': {'_copy_without_render': {insert: [(0, "*

 * *              "'.github/workflows/build.yaml'), (1, '.github/workflows/test.yaml')], delete: [0]}, "*

 * *              "'_render_devdocs': False, '_jinja2_env_vars': OrderedDict([('lstrip_blocks', True), "*

 * *              "('trim_blocks', True)])}}"}*

```diff
@@ -1,16 +1,22 @@
 {
-    "checkout": "v0.2.22",
-    "commit": "605f95714130c960bce12eab98a4e023e8932249",
+    "checkout": "v0.4.0",
+    "commit": "87a407a65408d75a949c0b54b19fd287475a56f8",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
-                ".github/workflows/**.yaml",
+                ".github/workflows/build.yaml",
+                ".github/workflows/test.yaml",
                 "docs/_templates/autosummary/**.rst"
             ],
+            "_jinja2_env_vars": {
+                "lstrip_blocks": true,
+                "trim_blocks": true
+            },
+            "_render_devdocs": false,
             "_template": "https://github.com/scverse/cookiecutter-scverse",
             "author_email": "marco.varrone@unil.ch",
             "author_full_name": "Marco Varrone",
             "github_user": "marcovarrone",
             "license": "BSD 3-Clause License",
             "package_name": "cellcharter",
             "project_description": "A Python package for the identification, characterization and comparison of spatial clusters from spatial -omics data.",
```

### Comparing `cellcharter-0.2.0/.flake8` & `cellcharter-0.2.1/.flake8`

 * *Files identical despite different names*

### Comparing `cellcharter-0.2.0/.pre-commit-config.yaml` & `cellcharter-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cellcharter-0.2.0/.readthedocs.yaml.rej` & `cellcharter-0.2.1/.readthedocs.yaml.rej`

 * *Files identical despite different names*

### Comparing `cellcharter-0.2.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `cellcharter-0.2.1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `cellcharter-0.2.0/.github/workflows/build.yaml` & `cellcharter-0.2.1/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `cellcharter-0.2.0/.github/workflows/test.yaml` & `cellcharter-0.2.1/.github/workflows/test.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,17 @@
           - os: ubuntu-latest
             python: "3.9"
           - os: ubuntu-latest
             python: "3.10"
           - os: ubuntu-latest
             python: "3.10"
             pip-flags: "--pre"
+            name: PRE-RELEASE DEPENDENCIES
+
+    name: ${{ matrix.name }} Python ${{ matrix.python }}
 
     env:
       OS: ${{ matrix.os }}
       PYTHON: ${{ matrix.python }}
 
     steps:
       - uses: actions/checkout@v3
@@ -52,10 +55,13 @@
           pip install ${{ matrix.pip-flags }} ".[dev,test]"
       - name: Test
         env:
           MPLBACKEND: agg
           PLATFORM: ${{ matrix.os }}
           DISPLAY: :42
         run: |
-          pytest -v --cov --color=yes
+          coverage run -m pytest -v --color=yes
+      - name: Report coverage
+        run: |
+          coverage report
       - name: Upload coverage
         uses: codecov/codecov-action@v3
```

### Comparing `cellcharter-0.2.0/src/cellcharter/datasets/_dataset.py` & `cellcharter-0.2.1/src/cellcharter/datasets/_dataset.py`

 * *Files identical despite different names*

### Comparing `cellcharter-0.2.0/src/cellcharter/gr/_aggr.py` & `cellcharter-0.2.1/src/cellcharter/gr/_aggr.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Optional, Union
 
 import numpy as np
 import scipy.sparse as sps
 from anndata import AnnData
 from scipy.sparse import spdiags
 from squidpy._constants._pkg_constants import Key as sqKey
+from squidpy._docs import d
 from tqdm.auto import tqdm
 
 from cellcharter._constants._pkg_constants import Key
 from cellcharter._utils import str2list
 
 
 def _aggregate_mean(adj, x):
@@ -72,23 +73,21 @@
 def _aggregate_neighbors(
     adj: sps.spmatrix,
     X: np.ndarray,
     nhood_layers: list,
     aggregations: Optional[Union[str, list]] = "mean",
     disable_tqdm: bool = True,
 ) -> np.ndarray:
-
     adj = adj.astype(bool)
     adj = _setdiag(adj, 0)
     adj_hop = adj.copy()
     adj_visited = _setdiag(adj.copy(), 1)
 
     Xs = []
     for i in tqdm(range(0, max(nhood_layers) + 1), disable=disable_tqdm):
-
         if i in nhood_layers:
             if i == 0:
                 Xs.append(X)
             else:
                 if i > 1:
                     adj_hop, adj_visited = _hop(adj_hop, adj, adj_visited)
                 adj_hop_norm = _normalize(adj_hop)
@@ -98,14 +97,15 @@
                     Xs.append(x)
     if sps.issparse(X):
         return sps.hstack(Xs)
     else:
         return np.hstack(Xs)
 
 
+@d.dedent
 def aggregate_neighbors(
     adata: AnnData,
     n_layers: Union[int, list],
     aggregations: Optional[Union[str, list]] = "mean",
     connectivity_key: Optional[str] = None,
     use_rep: Optional[str] = None,
     sample_key: Optional[str] = None,
```

### Comparing `cellcharter-0.2.0/src/cellcharter/gr/_build.py` & `cellcharter-0.2.1/src/cellcharter/gr/_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
 import numpy as np
 import pandas as pd
 import scipy.sparse as sps
 from anndata import AnnData
 from scipy.sparse import csr_matrix
-from squidpy._constants._constants import CoordType, Transform
 from squidpy._constants._pkg_constants import Key
-from squidpy._docs import inject_docs
+from squidpy._docs import d
 from squidpy.gr._utils import _assert_connectivity_key
 
 
-@inject_docs(t=Transform, c=CoordType)
+@d.dedent
 def remove_long_links(
     adata: AnnData,
     distance_percentile: float = 99.0,
     connectivity_key: str | None = None,
     distances_key: str | None = None,
     neighs_key: str | None = None,
     copy: bool = False,
@@ -71,14 +70,15 @@
 
     if copy:
         return conns, dists
     else:
         adata.uns[neighs_key]["params"]["radius"] = threshold
 
 
+@d.dedent
 def remove_intra_cluster_links(
     adata: AnnData,
     cluster_key: str,
     connectivity_key: str | None = None,
     distances_key: str | None = None,
     copy: bool = False,
 ) -> tuple[csr_matrix, csr_matrix] | None:
@@ -114,14 +114,15 @@
     distances_key = Key.obsp.spatial_dist(distances_key)
     _assert_connectivity_key(adata, connectivity_key)
     _assert_connectivity_key(adata, distances_key)
 
     conns = adata.obsp[connectivity_key].copy() if copy else adata.obsp[connectivity_key]
     dists = adata.obsp[distances_key].copy() if copy else adata.obsp[distances_key]
 
+    # ToDo: compute inter_cluster_mask only on conns and apply mask to both matrices
     for matrix in [conns, dists]:
         target_clusters = np.array(adata.obs[cluster_key][matrix.indices])
         source_clusters = np.array(
             adata.obs[cluster_key][np.repeat(np.arange(matrix.indptr.shape[0] - 1), np.diff(matrix.indptr))]
         )
 
         inter_cluster_mask = (source_clusters != target_clusters).astype(int)
@@ -142,14 +143,15 @@
 
     labels[small_components_idxs] = -1
     labels[~small_components_idxs] = pd.factorize(labels[~small_components_idxs])[0] + count
 
     return labels, (n_components - len(small_components))
 
 
+@d.dedent
 def connected_components(
     adata: AnnData,
     cluster_key: str = None,
     min_cells: int = 250,
     connectivity_key: str = None,
     out_key: str = "component",
     copy: bool = False,
```

### Comparing `cellcharter-0.2.0/src/cellcharter/gr/_group.py` & `cellcharter-0.2.1/src/cellcharter/gr/_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import numpy as np
 import pandas as pd
 from anndata import AnnData
+from squidpy._docs import d
 
 
 def _proportion(adata, id_key, val_key, normalize=True):
     df = pd.pivot(adata.obs[[id_key, val_key]].value_counts().reset_index(), index=id_key, columns=val_key)
     df[df.isna()] = 0
     df.columns = df.columns.droplevel(0)
     if normalize:
@@ -20,14 +21,15 @@
 
     if log:
         enrichment = np.log2(enrichment)
     enrichment = enrichment.fillna(enrichment.min())
     return enrichment
 
 
+@d.dedent
 def enrichment(
     adata: AnnData,
     group_key: str,
     label_key: str,
     log: bool = True,
     observed_expected: bool = False,
     copy: bool = False,
@@ -52,16 +54,16 @@
     -------
     If ``copy = True``, returns a :class:`dict` with the following keys:
         - ``'enrichment'`` - the enrichment values.
         - ``'observed'`` - the observed proportions (if `observed_expected is True`).
         - ``'expected'`` - the expected proportions (if `observed_expected is True`).
 
     Otherwise, modifies the ``adata`` with the following keys:
-        - :attr:`anndata.AnnData.uns` ``['{cluster_key}_nhood_enrichment']`` - the above mentioned dict.
-        - :attr:`anndata.AnnData.uns` ``['{cluster_key}_nhood_enrichment']['params']`` - the parameters used.
+        - :attr:`anndata.AnnData.uns` ``['{group_key}_{label_key}_nhood_enrichment']`` - the above mentioned dict.
+        - :attr:`anndata.AnnData.uns` ``['{group_key}_{label_key}_nhood_enrichment']['params']`` - the parameters used.
     """
     observed = _proportion(adata, id_key=label_key, val_key=group_key).reindex().T
     observed[observed.isna()] = 0
     expected = adata.obs[group_key].value_counts() / adata.shape[0]
 
     enrichment = _enrichment(observed, expected, log=log)
```

### Comparing `cellcharter-0.2.0/src/cellcharter/gr/_nhood.py` & `cellcharter-0.2.1/src/cellcharter/gr/_nhood.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from itertools import combinations
 
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from joblib import Parallel, delayed
 from squidpy._constants._pkg_constants import Key
+from squidpy._docs import d
 from squidpy.gr._utils import _assert_categorical_obs, _assert_connectivity_key
 from tqdm.auto import tqdm
 
 from cellcharter.gr import remove_intra_cluster_links
 
 
 def _observed_n_clusters_links(adj, labels, symmetric=True):
@@ -129,14 +130,15 @@
 
     if observed_expected:
         result["observed"] = observed
         result["expected"] = expected
     return result
 
 
+@d.dedent
 def nhood_enrichment(
     adata: AnnData,
     cluster_key: str,
     connectivity_key: str | None = None,
     log_fold_change: bool = False,
     only_inter: bool = True,
     symmetric: bool = False,
@@ -232,18 +234,20 @@
     adata.obs["condition"] = pd.Categorical(adata.obs[library_key].isin(subsamples_perm).astype(int))
     result = diff_nhood_enrichment(adata, cluster_key=cluster_key, condition_key="condition", pvalues=False, copy=True)[
         "0_1"
     ]["enrichment"]
     return result
 
 
+@d.dedent
 def diff_nhood_enrichment(
     adata: AnnData,
     cluster_key: str,
     condition_key: str,
+    condition_groups: tuple[str, str] | None = None,
     library_key: str | None = "library_id",
     pvalues: bool = False,
     n_perms: int = 1000,
     n_jobs: int | None = None,
     copy: bool = False,
     **nhood_kwargs,
 ) -> dict | None:
@@ -281,15 +285,15 @@
         - ``'enrichment'`` - the differential neighborhood enrichment.
         - ``'pvalue'`` - the enrichment pvalues (if `pvalues is True`).
 
     """
     _assert_categorical_obs(adata, key=cluster_key)
     _assert_categorical_obs(adata, key=condition_key)
 
-    conditions = adata.obs[condition_key].cat.categories
+    conditions = adata.obs[condition_key].cat.categories if condition_groups is None else condition_groups
 
     if "observed_expected" in nhood_kwargs:
         warnings.warn(
             "The `observed_expected` can be used only in `pl.nhood_enrichment`, hence it will be ignored.", stacklevel=2
         )
 
     enrichments = {}
@@ -299,16 +303,19 @@
             cluster_key=cluster_key,
             copy=True,
             **nhood_kwargs,
         )["enrichment"]
 
     result = {}
 
-    for condition1, condition2 in combinations(conditions, 2):
+    condition_pairs = combinations(conditions, 2) if condition_groups is None else [condition_groups]
+
+    for condition1, condition2 in condition_pairs:
         observed = enrichments[condition1] - enrichments[condition2]
+        observed = observed.loc[enrichments[condition1].index, enrichments[condition1].columns]
         result_key = f"{condition1}_{condition2}"
         result[result_key] = {"enrichment": observed}
         if pvalues:
             samples1 = adata[adata.obs[condition_key] == condition1].obs[library_key].unique()
             samples2 = adata[adata.obs[condition_key] == condition2].obs[library_key].unique()
 
             samples_perms = np.random.choice(
```

### Comparing `cellcharter-0.2.0/src/cellcharter/pl/_autok.py` & `cellcharter-0.2.1/src/cellcharter/pl/_autok.py`

 * *Files identical despite different names*

### Comparing `cellcharter-0.2.0/src/cellcharter/pl/_group.py` & `cellcharter-0.2.1/src/cellcharter/pl/_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 
 from pathlib import Path
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 from anndata import AnnData
+from squidpy._docs import d
 from squidpy.gr._utils import _assert_categorical_obs
 from squidpy.pl._color_utils import Palette_t, _get_palette, _maybe_set_colors
 
 try:
-    from matplotlib import colormaps as cm
+    from matplotlib.colormaps import get_cmap
 except ImportError:
-    from matplotlib import cm
+    from matplotlib.pyplot import get_cmap
 
 from cellcharter.gr._group import _proportion
 from cellcharter.pl._utils import _dotplot
 
 
+@d.dedent
 def proportion(
     adata: AnnData,
     group_key: str,
     label_key: str,
     groups: list | None = None,
     labels: list | None = None,
     rotation_xlabel: int = 45,
@@ -86,14 +88,15 @@
     handles, labels = ax.get_legend_handles_labels()
     lgd = ax.legend(handles[::-1], labels[::-1], loc="center left", ncol=ncols, bbox_to_anchor=(1.0, 0.5))
 
     if save:
         plt.savefig(save, bbox_extra_artists=(lgd, lgd), bbox_inches="tight")
 
 
+@d.dedent
 def enrichment(
     adata: AnnData,
     group_key: str,
     label_key: str,
     size_threshold: float | None = None,
     color_threshold: float = 1,
     legend_title: str | None = None,
@@ -139,15 +142,15 @@
         Keyword arguments for :func:`matplotlib.pyplot.scatter`.
     """
     if f"{group_key}_{label_key}_enrichment" not in adata.uns:
         raise ValueError("Run cellcharter.gr.enrichment first.")
 
     if palette is None:
         palette = matplotlib.colors.LinearSegmentedColormap.from_list(
-            "", [cm.get_cmap("coolwarm")(0), matplotlib.colors.to_rgb("darkgrey"), cm.get_cmap("coolwarm")(255)]
+            "", [get_cmap("coolwarm")(0), matplotlib.colors.to_rgb("darkgrey"), get_cmap("coolwarm")(255)]
         )
 
     enrichment = adata.uns[f"{group_key}_{label_key}_enrichment"]["enrichment"]
 
     if labels is not None:
         enrichment = enrichment.loc[:, labels]
```

### Comparing `cellcharter-0.2.0/src/cellcharter/pl/_nhood.py` & `cellcharter-0.2.1/src/cellcharter/pl/_nhood.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from matplotlib import rcParams
 from matplotlib.axes import Axes
+from squidpy._docs import d
 from squidpy.gr._utils import _assert_categorical_obs
 from squidpy.pl._color_utils import Palette_t, _maybe_set_colors
 from squidpy.pl._graph import _get_data
 from squidpy.pl._spatial_utils import _panel_grid
 
 from cellcharter.pl._utils import _heatmap
 
@@ -81,20 +82,23 @@
         dpi=dpi,
         cbar_kwargs=cbar_kwargs,
         ax=ax,
         **kwargs,
     )
 
 
+@d.dedent
 def nhood_enrichment(
     adata: AnnData,
     cluster_key: str,
     row_groups: list[str] | None = None,
     col_groups: list[str] | None = None,
+    min_freq: float | None = None,
     annotate: bool = False,
+    transpose: bool = False,
     method: str | None = None,
     title: str | None = "Neighborhood enrichment",
     cmap: str = "bwr",
     palette: Palette_t = None,
     cbar_kwargs: Mapping[str, Any] = MappingProxyType({}),
     figsize: tuple[float, float] | None = None,
     dpi: int | None = None,
@@ -127,17 +131,24 @@
         Keyword arguments for :func:`matplotlib.pyplot.text`.
 
     Returns
     -------
     %(plotting_returns)s
     """
     _assert_categorical_obs(adata, key=cluster_key)
-    nhood_enrichment_values = _get_data(adata, cluster_key=cluster_key, func_name="nhood_enrichment")
-    enrichment = nhood_enrichment_values["enrichment"]
-    enrichment[np.isinf(enrichment)] = np.nan
+    nhood_enrichment_values = _get_data(adata, cluster_key=cluster_key, func_name="nhood_enrichment").copy()
+    nhood_enrichment_values["enrichment"][np.isinf(nhood_enrichment_values["enrichment"])] = np.nan
+
+    if transpose:
+        nhood_enrichment_values["enrichment"] = nhood_enrichment_values["enrichment"].T
+
+    if min_freq is not None:
+        frequency = adata.obs[cluster_key].value_counts(normalize=True)
+        nhood_enrichment_values["enrichment"].loc[frequency[frequency < min_freq].index] = np.nan
+        nhood_enrichment_values["enrichment"].loc[:, frequency[frequency < min_freq].index] = np.nan
 
     _plot_nhood_enrichment(
         adata,
         nhood_enrichment_values,
         cluster_key,
         row_groups=row_groups,
         col_groups=col_groups,
@@ -155,14 +166,15 @@
         **kwargs,
     )
 
     if save is not None:
         plt.savefig(save, bbox_inches="tight")
 
 
+@d.dedent
 def diff_nhood_enrichment(
     adata: AnnData,
     cluster_key: str,
     condition_key: str,
     condition_groups: list[str] | None = None,
     hspace: float = 0.25,
     wspace: float | None = None,
@@ -220,17 +232,17 @@
         figsize=nhood_kwargs.get("dpi", figsize),
     )
 
     axs = [plt.subplot(grid[c]) for c in range(n_combinations)]
 
     for i, (condition1, condition2) in enumerate(combinations(conditions, 2)):
         if f"{condition1}_{condition2}" not in adata.uns[f"{cluster_key}_{condition_key}_diff_nhood_enrichment"]:
-            nhood_enrichment_values = adata.uns[f"{cluster_key}_{condition_key}_diff_nhood_enrichment"][
-                f"{condition2}_{condition1}"
-            ]
+            nhood_enrichment_values = dict(
+                adata.uns[f"{cluster_key}_{condition_key}_diff_nhood_enrichment"][f"{condition2}_{condition1}"]
+            )
             nhood_enrichment_values["enrichment"] = -nhood_enrichment_values["enrichment"]
         else:
             nhood_enrichment_values = adata.uns[f"{cluster_key}_{condition_key}_diff_nhood_enrichment"][
                 f"{condition1}_{condition2}"
             ]
 
         _plot_nhood_enrichment(
```

### Comparing `cellcharter-0.2.0/src/cellcharter/pl/_shape.py` & `cellcharter-0.2.1/src/cellcharter/pl/_shape.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,84 @@
 from __future__ import annotations
 
+import warnings
 from itertools import combinations
+from pathlib import Path
 
 import anndata as ad
 import geopandas
-import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 import spatialdata as sd
+import spatialdata_plot  # noqa: F401
 from anndata import AnnData
 from scipy.stats import ttest_ind
-from spatialdata_plot.pl.utils import _get_colors_for_categorical_obs
+from squidpy._docs import d
 
 from ._utils import adjust_box_widths
 
 
 def plot_boundaries(
     adata: AnnData,
     sample: str,
     library_key: str = "sample",
     component_key: str = "component",
     alpha_boundary: float = 0.5,
     show_cells: bool = True,
+    save: str | Path | None = None,
+) -> None:
+    """
+    Plot the boundaries of the clusters.
+
+    Parameters
+    ----------
+    %(adata)s
+    sample
+        Sample to plot.
+    library_key
+        Key in :attr:`anndata.AnnData.obs` where the sample labels are stored.
+    component_key
+        Key in :attr:`anndata.AnnData.obs` where the component labels are stored.
+    alpha_boundary
+        Transparency of the boundaries.
+    show_cells
+        Whether to show the cells or not.
+
+    Returns
+    -------
+    %(plotting_returns)s
+    """
+    # Print warning and call boundaries
+    warnings.warn(
+        "plot_boundaries is deprecated and will be removed in the next release. " "Please use `boundaries` instead.",
+        FutureWarning,
+        stacklevel=2,
+    )
+    boundaries(
+        adata=adata,
+        sample=sample,
+        library_key=library_key,
+        component_key=component_key,
+        alpha_boundary=alpha_boundary,
+        show_cells=show_cells,
+        save=save,
+    )
+
+
+@d.dedent
+def boundaries(
+    adata: AnnData,
+    sample: str,
+    library_key: str = "sample",
+    component_key: str = "component",
+    alpha_boundary: float = 0.5,
+    show_cells: bool = True,
+    save: str | Path | None = None,
 ) -> None:
     """
     Plot the boundaries of the clusters.
 
     Parameters
     ----------
     %(adata)s
@@ -52,72 +103,134 @@
 
     boundaries = {
         cluster: boundary
         for cluster, boundary in adata.uns[f"shape_{component_key}"]["boundary"].items()
         if cluster in clusters
     }
     gdf = geopandas.GeoDataFrame(geometry=list(boundaries.values()))
-    # adata.obs[cluster_key] = pd.Categorical(adata.obs[cluster_key])
     adata.obs.loc[adata.obs[component_key] == -1, component_key] = np.nan
     adata.obs.index = "cell_" + adata.obs.index
     adata.obs["instance_id"] = adata.obs.index
     adata.obs["region"] = "cells"
 
     xy = adata.obsm["spatial"]
     cell_circles = sd.models.ShapesModel.parse(xy, geometry=0, radius=3000, index=adata.obs["instance_id"])
 
     obs = pd.DataFrame(list(boundaries.keys()), columns=[component_key], index=np.arange(len(boundaries)).astype(str))
     adata_obs = ad.AnnData(X=pd.DataFrame(index=obs.index, columns=adata.var_names), obs=obs)
     adata_obs.obs["region"] = "clusters"
-    adata_obs.index = "cell_" + adata_obs.obs.index
-    adata_obs.obs["instance_id"] = adata_obs.obs.index
+    adata_obs.index = "cluster_" + adata_obs.obs.index
+    adata_obs.obs["instance_id"] = np.arange(len(boundaries))
     adata_obs.obs[component_key] = pd.Categorical(adata_obs.obs[component_key])
 
     adata = ad.concat((adata, adata_obs), join="outer")
 
     adata.obs["region"] = adata.obs["region"].astype("category")
-    adata.obs[component_key] = adata.obs[component_key].astype("category")
 
     table = sd.models.TableModel.parse(
         adata, region_key="region", region=["clusters", "cells"], instance_key="instance_id"
     )
 
     shapes = {
         "clusters": sd.models.ShapesModel.parse(gdf),
         "cells": sd.models.ShapesModel.parse(cell_circles),
     }
-    adata.obs["instance_id"] = pd.Categorical(adata.obs["instance_id"])
 
     sdata = sd.SpatialData(shapes=shapes, table=table)
 
     ax = plt.gca()
     if show_cells:
-        sdata.pl.render_shapes(elements="cells", color=component_key).pl.show(ax=ax, legend_loc=False)
-    else:
-        sdata.table.uns[f"{component_key}_colors"] = _get_colors_for_categorical_obs(
-            adata.obs["component"].cat.categories
-        )
+        try:
+            sdata.pl.render_shapes(elements="cells", color=component_key).pl.show(ax=ax, legend_loc=None)
+        except TypeError:  # TODO: remove after spatialdata-plot issue  #256 is fixed
+            warnings.warn(
+                "Until the next spatialdata_plot release, the cells that do not belong to any component will be displayed with a random color instead of grey.",
+                stacklevel=2,
+            )
+            sdata.tables["table"].obs[component_key] = sdata.tables["table"].obs[component_key].cat.add_categories([-1])
+            sdata.tables["table"].obs[component_key] = sdata.tables["table"].obs[component_key].fillna(-1)
+            sdata.pl.render_shapes(elements="cells", color=component_key).pl.show(ax=ax, legend_loc=None)
 
     sdata.pl.render_shapes(
         elements="clusters",
         color=component_key,
         fill_alpha=alpha_boundary,
-        palette=mpl.colors.ListedColormap(sdata.table.uns[f"{component_key}_colors"]),
     ).pl.show(ax=ax)
-    plt.show()
+
+    if save is not None:
+        plt.savefig(save, bbox_inches="tight")
 
 
 def plot_shape_metrics(
     adata: AnnData,
     condition_key: str,
     condition_groups: list[str] | None = None,
     cluster_key: str | None = None,
     cluster_id: list[str] | None = None,
     component_key: str = "component",
     metrics: str | tuple[str] | list[str] = ("linearity", "curl"),
+    figsize: tuple[float, float] = (8, 7),
+    title: str | None = None,
+) -> None:
+    """
+    Boxplots of the shape metrics between two conditions.
+
+    Parameters
+    ----------
+    %(adata)s
+    condition_key
+        Key in :attr:`anndata.AnnData.obs` where the condition labels are stored.
+    condition_groups
+        List of two conditions to compare. If None, all pairwise comparisons are made.
+    cluster_key
+        Key in :attr:`anndata.AnnData.obs` where the cluster labels are stored. This is used to filter the clusters to plot.
+    cluster_id
+        List of clusters to plot. If None, all clusters are plotted.
+    component_key
+        Key in :attr:`anndata.AnnData.obs` where the component labels are stored.
+    metrics
+        List of metrics to plot. Available metrics are ``linearity``, ``curl``, ``elongation``, ``purity``.
+    figsize
+        Figure size.
+    title
+        Title of the plot.
+
+    Returns
+    -------
+    %(plotting_returns)s
+    """
+    # Print warning and call shape_metrics
+    warnings.warn(
+        "plot_shape_metrics is deprecated and will be removed in the next release. "
+        "Please use `shape_metrics` instead.",
+        FutureWarning,
+        stacklevel=2,
+    )
+    shape_metrics(
+        adata=adata,
+        condition_key=condition_key,
+        condition_groups=condition_groups,
+        cluster_key=cluster_key,
+        cluster_id=cluster_id,
+        component_key=component_key,
+        metrics=metrics,
+        figsize=figsize,
+        title=title,
+    )
+
+
+@d.dedent
+def shape_metrics(
+    adata: AnnData,
+    condition_key: str,
+    condition_groups: list[str] | None = None,
+    cluster_key: str | None = None,
+    cluster_id: list[str] | None = None,
+    component_key: str = "component",
+    metrics: str | tuple[str] | list[str] = ("linearity", "curl"),
     figsize: tuple[float, float] = (8, 7),
     title: str | None = None,
 ) -> None:
     """
     Boxplots of the shape metrics between two conditions.
 
     Parameters
```

### Comparing `cellcharter-0.2.0/src/cellcharter/pl/_utils.py` & `cellcharter-0.2.1/src/cellcharter/pl/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 from matplotlib.patches import PathPatch
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from scanpy.pl._dotplot import DotPlot
 from scipy.cluster import hierarchy as sch
 from squidpy._constants._pkg_constants import Key
 from squidpy.pl._color_utils import Palette_t
 
+try:
+    from matplotlib import colormaps as cm
+except ImportError:
+    from matplotlib import cm
+
 
 def _get_cmap_norm(
     adata: AnnData,
     key: str,
     order: tuple[list[int], list[int]] | None | None = None,
 ) -> tuple[mcolors.ListedColormap, mcolors.ListedColormap, mcolors.BoundaryNorm, mcolors.BoundaryNorm, int]:
     n_rows = n_cols = adata.obs[key].nunique()
@@ -102,15 +107,15 @@
     row_sm = mpl.cm.ScalarMappable(cmap=row_cmap, norm=row_norm)
     col_sm = mpl.cm.ScalarMappable(cmap=col_cmap, norm=col_norm)
 
     vmin = kwargs.pop("vmin", np.nanmin(data))
     vmax = kwargs.pop("vmax", np.nanmax(data))
     vcenter = kwargs.pop("vcenter", 0)
     norm = mpl.colors.TwoSlopeNorm(vcenter=vcenter, vmin=vmin, vmax=vmax)
-    cont_cmap = copy(plt.get_cmap(cont_cmap))
+    cont_cmap = copy(cm.get_cmap(cont_cmap))
     cont_cmap.set_bad(color="grey")
 
     annot = np.round(data[::-1], n_digits).astype(str) if annotate else None
     if "significant" in adata.layers:
         significant = adata.layers["significant"].astype(str)
         annot = np.char.add(np.empty_like(data[::-1], dtype=str), significant[row_order[:, None], col_order][::-1])
```

### Comparing `cellcharter-0.2.0/src/cellcharter/tl/_autok.py` & `cellcharter-0.2.1/src/cellcharter/tl/_autok.py`

 * *Files identical despite different names*

### Comparing `cellcharter-0.2.0/src/cellcharter/tl/_gmm.py` & `cellcharter-0.2.1/src/cellcharter/tl/_gmm.py`

 * *Files identical despite different names*

### Comparing `cellcharter-0.2.0/src/cellcharter/tl/_shape.py` & `cellcharter-0.2.1/src/cellcharter/tl/_shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from anndata import AnnData
 from matplotlib.path import Path
 from rasterio import features
 from scipy.spatial import Delaunay
 from shapely import geometry
 from shapely.ops import polygonize, unary_union
 from skimage.morphology import skeletonize
+from squidpy._docs import d
 
 
 def _alpha_shape(coords, alpha):
     """
     Compute the alpha shape (concave hull) of a set of points.
 
     Adapted from `here <https://web.archive.org/web/20200726174718/http://blog.thehumangeo.com/2014/05/12/drawing-boundaries-in-python/>`_.
@@ -77,14 +78,15 @@
                 if isinstance(difference, geometry.Polygon):
                     boundary = difference
             except Exception:  # noqa: B902
                 pass
     return component, boundary
 
 
+@d.dedent
 def boundaries(
     adata: AnnData,
     cluster_key: str = "component",
     min_hole_area_ratio: float = 0.1,
     alpha_start: int = 2000,
     copy: bool = False,
 ) -> None | dict[int, geometry.Polygon]:
@@ -228,14 +230,15 @@
         scale_factor = height / poly.bounds[2]
     else:
         scale_factor = height / poly.bounds[3]
     poly = shapely.affinity.scale(poly, scale_factor, scale_factor, origin=(0, 0, 0))
     return features.rasterize([poly], out_shape=(height, int(height * (maxx - minx) / (maxy - miny)))), scale_factor
 
 
+@d.dedent
 def linearity(
     adata: AnnData,
     cluster_key: str = "component",
     out_key: str = "linearity",
     height: int = 1000,
     min_ratio: float = 0.05,
     copy: bool = False,
@@ -287,14 +290,15 @@
 
     # get major/minor axis measurements
     minor_axis = min(mbr_lengths)
     major_axis = max(mbr_lengths)
     return 1 - minor_axis / major_axis
 
 
+@d.dedent
 def elongation(
     adata: AnnData,
     cluster_key: str = "component",
     out_key: str = "elongation",
     copy: bool = False,
 ) -> None | dict[int, float]:
     """
@@ -345,14 +349,15 @@
     _, length = _axes(boundary)
     if fibre_length < length:
         return 0
     else:
         return 1 - length / fibre_length
 
 
+@d.dedent
 def curl(
     adata: AnnData,
     cluster_key: str = "component",
     out_key: str = "curl",
     copy: bool = False,
 ) -> None | dict[int, float]:
     """
@@ -380,14 +385,15 @@
         curl_score[cluster] = _curl(boundary)
 
     if copy:
         return curl_score
     adata.uns[f"shape_{cluster_key}"][out_key] = curl_score
 
 
+@d.dedent
 def purity(
     adata: AnnData,
     cluster_key: str = "component",
     library_key: str = "sample",
     out_key: str = "purity",
     exterior: bool = False,
     copy: bool = False,
```

### Comparing `cellcharter-0.2.0/src/cellcharter/tl/_trvae.py` & `cellcharter-0.2.1/src/cellcharter/tl/_trvae.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,26 +77,25 @@
         """
 
         def __init__(
             self,
             adata: AnnData,
             condition_key: str = None,
             conditions: Optional[list] = None,
-            hidden_layer_sizes: list = [256, 64],
+            hidden_layer_sizes: list | tuple = (256, 64),
             latent_dim: int = 10,
             dr_rate: float = 0.05,
             use_mmd: bool = True,
             mmd_on: str = "z",
             mmd_boundary: Optional[int] = None,
             recon_loss: Optional[str] = "mse",
             beta: float = 1,
             use_bn: bool = False,
             use_ln: bool = True,
         ):
-
             self.adata = adata
 
             self.condition_key_ = condition_key
 
             if conditions is None:
                 if condition_key is not None:
                     self.conditions_ = adata.obs[condition_key].unique().tolist()
@@ -117,15 +116,15 @@
             self.use_ln_ = use_ln
 
             self.input_dim_ = adata.n_vars
 
             self.model = trVAE(
                 self.input_dim_,
                 self.conditions_,
-                self.hidden_layer_sizes_,
+                list(self.hidden_layer_sizes_),
                 self.latent_dim_,
                 self.dr_rate_,
                 self.use_mmd_,
                 self.mmd_on_,
                 self.mmd_boundary_,
                 self.recon_loss_,
                 self.beta_,
```

### Comparing `cellcharter-0.2.0/src/cellcharter/tl/_utils.py` & `cellcharter-0.2.1/src/cellcharter/tl/_utils.py`

 * *Files identical despite different names*

### Comparing `cellcharter-0.2.0/LICENSE` & `cellcharter-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cellcharter-0.2.0/README.md` & `cellcharter-0.2.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 **A Python package for the identification, characterization and comparison of spatial clusters from spatial -omics data.**
 
 ---
 
 <p align="center">
   <a href="https://cellcharter.readthedocs.io/en/latest/" target="_blank">Documentation</a> •
   <a href="https://cellcharter.readthedocs.io/en/latest/notebooks/codex_mouse_spleen.html" target="_blank">Examples</a> •
-  <a href="https://www.biorxiv.org/content/10.1101/2023.01.10.523386v1" target="_blank">Paper</a>
+  <a href="https://doi.org/10.1038/s41588-023-01588-4" target="_blank">Paper</a> •
+  <a href="https://www.biorxiv.org/content/10.1101/2023.01.10.523386v2" target="_blank">Preprint</a>
 </p>
 
 [![Tests][badge-tests]][link-tests]
 [![Documentation][badge-docs]][link-docs]
 
 [badge-tests]: https://img.shields.io/github/actions/workflow/status/CSOgroup/cellcharter/test.yaml?branch=main
 [link-tests]: https://github.com/CSOgroup/cellcharter/actions/workflows/test.yml
@@ -41,33 +42,42 @@
 Please refer to the [documentation][link-docs]. In particular, the
 
 -   [API documentation][link-api].
 -   [Tutorials][link-tutorial]
 
 ## Installation
 
-CellCharter uses Python < 3.11 and [PyTorch](https://pytorch.org) <= 1.12.1. If you are planning to use a GPU, make sure to download and install the correct version of PyTorch first.
-
-In CellCharter, only the dimensionality reduction and batch correction step is dependent on the data type. In particular, it uses:
-
--   [scVI](https://github.com/scverse/scvi-tools) for spatial transcriptomics data such as 10x Visium and Xenium, Nanostring CosMx, Vizgen MERSCOPE, Stereo-seq, DBiT-seq, MERFISH and seqFISH data.
--   A modified version of [scArches](https://github.com/theislab/scarches)'s TRVAE model for spatial proteomics data such as Akoya CODEX, Lunaphore COMET, CyCIF, IMC and MIBI-TOF data.
-
-By installing CellCharter without specifying the type of data, as in the following code, it will install without any of the two models.
+1. Create a conda or pyenv environment
+2. Install Python <= 3.10 and [PyTorch](https://pytorch.org) <= 1.12.1. If you are planning to use a GPU, make sure to download and install the correct version of PyTorch first.
+3. Install the library used for dimensionality reduction and batch effect removal according the data type you are planning to analyze:
+    - [scVI](https://github.com/scverse/scvi-tools) for spatial transcriptomics and/or epigenomics data such as 10x Visium and Xenium, Nanostring CosMx, Vizgen MERSCOPE, Stereo-seq, DBiT-seq, MERFISH and seqFISH data.
+    - A modified version of [scArches](https://github.com/theislab/scarches)'s TRVAE model for spatial proteomics data such as Akoya CODEX, Lunaphore COMET, CyCIF, IMC and MIBI-TOF data.
+4. Install CellCharter using pip:
 
 ```bash
 pip install cellcharter
 ```
 
-However, you can include in the installation the type of data (transcriptomics and/or proteomics) you are planning to analyze, and it will install the required dependencies.
+We suggest using `mamba` to install the dependencies.
+Installing the latest version of the dependencies (in particular `scvi-tools` and `spatialdata`) may lead to dependency conflicts.
+However, this should not be a problem because CellCharter doesn't use any of the mismatching features.
+
+We report here an example of an installation aimed at analyzing spatial transcriptomics data (and thus installing `scvi-tools`).
+This example is based on a Linux CentOS 7 system with an NVIDIA A100 GPU.
 
 ```bash
-pip install cellcharter[transcriptomics]
+conda create -n cellcharter-env -c conda-forge python=3.10 mamba
+conda activate cellcharter-env
+mamba install pytorch==1.12.1 torchvision==0.13.1 torchaudio==0.12.1 cudatoolkit=11.6 -c pytorch -c conda-forge
+pip install pyro-ppl==1.8.6 scvi-tools==0.20.3
+pip install cellcharter
 ```
 
+Note: a different system may require different commands to install PyTorch and JAX. Refer to their respective documentation for more details.
+
 ## Contribution
 
 If you found a bug or you want to propose a new feature, please use the [issue tracker][issue-tracker].
 
 [issue-tracker]: https://github.com/CSOgroup/cellcharter/issues
 [link-docs]: https://cellcharter.readthedocs.io
 [link-api]: https://cellcharter.readthedocs.io/en/latest/api.html
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
         [https://github.com/CSOgroup/cellcharter/raw/main/docs/_static/
 cellcharter.png]**A Python package for the identification, characterization and
         comparison of spatial clusters from spatial -omics data.** ---
-                     _D_o_c_u_m_e_n_t_a_t_i_o_n â¢ _E_x_a_m_p_l_e_s â¢ _P_a_p_e_r
+               _D_o_c_u_m_e_n_t_a_t_i_o_n â¢ _E_x_a_m_p_l_e_s â¢ _P_a_p_e_r â¢ _P_r_e_p_r_i_n_t
 [![Tests][badge-tests]][link-tests] [![Documentation][badge-docs]][link-docs]
 [badge-tests]: https://img.shields.io/github/actions/workflow/status/CSOgroup/
  cellcharter/test.yaml?branch=main [link-tests]: https://github.com/CSOgroup/
  cellcharter/actions/workflows/test.yml [badge-docs]: https://img.shields.io/
                             readthedocs/cellcharter
 ## Background
 Spatial clustering determines cellular niches characterized by specific
@@ -16,27 +16,36 @@
                              spatial_clusters.png]
 CellCharter is able to automatically identify spatial clusters, and offers a
 suite of approaches for cluster characterization and comparison.
         [https://github.com/CSOgroup/cellcharter/raw/main/docs/_static/
                            cellcharter_workflow.png]
 ## Getting started Please refer to the [documentation][link-docs]. In
 particular, the - [API documentation][link-api]. - [Tutorials][link-tutorial]
-## Installation CellCharter uses Python < 3.11 and [PyTorch](https://
-pytorch.org) <= 1.12.1. If you are planning to use a GPU, make sure to download
-and install the correct version of PyTorch first. In CellCharter, only the
-dimensionality reduction and batch correction step is dependent on the data
-type. In particular, it uses: - [scVI](https://github.com/scverse/scvi-tools)
-for spatial transcriptomics data such as 10x Visium and Xenium, Nanostring
-CosMx, Vizgen MERSCOPE, Stereo-seq, DBiT-seq, MERFISH and seqFISH data. - A
-modified version of [scArches](https://github.com/theislab/scarches)'s TRVAE
-model for spatial proteomics data such as Akoya CODEX, Lunaphore COMET, CyCIF,
-IMC and MIBI-TOF data. By installing CellCharter without specifying the type of
-data, as in the following code, it will install without any of the two models.
-```bash pip install cellcharter ``` However, you can include in the
-installation the type of data (transcriptomics and/or proteomics) you are
-planning to analyze, and it will install the required dependencies. ```bash pip
-install cellcharter[transcriptomics] ``` ## Contribution If you found a bug or
-you want to propose a new feature, please use the [issue tracker][issue-
-tracker]. [issue-tracker]: https://github.com/CSOgroup/cellcharter/issues
-[link-docs]: https://cellcharter.readthedocs.io [link-api]: https://
-cellcharter.readthedocs.io/en/latest/api.html [link-tutorial]: https://
-cellcharter.readthedocs.io/en/latest/notebooks/codex_mouse_spleen.html
+## Installation 1. Create a conda or pyenv environment 2. Install Python <=
+3.10 and [PyTorch](https://pytorch.org) <= 1.12.1. If you are planning to use a
+GPU, make sure to download and install the correct version of PyTorch first. 3.
+Install the library used for dimensionality reduction and batch effect removal
+according the data type you are planning to analyze: - [scVI](https://
+github.com/scverse/scvi-tools) for spatial transcriptomics and/or epigenomics
+data such as 10x Visium and Xenium, Nanostring CosMx, Vizgen MERSCOPE, Stereo-
+seq, DBiT-seq, MERFISH and seqFISH data. - A modified version of [scArches]
+(https://github.com/theislab/scarches)'s TRVAE model for spatial proteomics
+data such as Akoya CODEX, Lunaphore COMET, CyCIF, IMC and MIBI-TOF data. 4.
+Install CellCharter using pip: ```bash pip install cellcharter ``` We suggest
+using `mamba` to install the dependencies. Installing the latest version of the
+dependencies (in particular `scvi-tools` and `spatialdata`) may lead to
+dependency conflicts. However, this should not be a problem because CellCharter
+doesn't use any of the mismatching features. We report here an example of an
+installation aimed at analyzing spatial transcriptomics data (and thus
+installing `scvi-tools`). This example is based on a Linux CentOS 7 system with
+an NVIDIA A100 GPU. ```bash conda create -n cellcharter-env -c conda-forge
+python=3.10 mamba conda activate cellcharter-env mamba install pytorch==1.12.1
+torchvision==0.13.1 torchaudio==0.12.1 cudatoolkit=11.6 -c pytorch -c conda-
+forge pip install pyro-ppl==1.8.6 scvi-tools==0.20.3 pip install cellcharter
+``` Note: a different system may require different commands to install PyTorch
+and JAX. Refer to their respective documentation for more details. ##
+Contribution If you found a bug or you want to propose a new feature, please
+use the [issue tracker][issue-tracker]. [issue-tracker]: https://github.com/
+CSOgroup/cellcharter/issues [link-docs]: https://cellcharter.readthedocs.io
+[link-api]: https://cellcharter.readthedocs.io/en/latest/api.html [link-
+tutorial]: https://cellcharter.readthedocs.io/en/latest/notebooks/
+codex_mouse_spleen.html
```

### Comparing `cellcharter-0.2.0/pyproject.toml` & `cellcharter-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 exclude = [
   "docs*",
   "tests*",
 ]
 
 [project]
 name = "cellcharter"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Python package for the identification, characterization and comparison of spatial clusters from spatial -omics data."
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
 license = {file = "LICENSE"}
 authors = [
     {name = "CSO group"},
 ]
@@ -28,30 +28,30 @@
     "anndata",
     "scikit-learn",
     "squidpy",
     # for debug logging (referenced from the issue template)
     "session-info",
     "pycave",
     "spatialdata",
-    "spatialdata-plot",
+    "spatialdata-plot >= 0.1.0",
     "rasterio",
     "sknw",
+    "matplotlib < 3.9.0",
 ]
 
 [project.optional-dependencies]
 dev = [
-    # CLI for bumping the version number
     "pre-commit",
     "twine>=4.0.2"
 ]
 doc = [
     "docutils>=0.8,!=0.18.*,!=0.19.*",
     "sphinx>=4",
     "sphinx-book-theme>=1.0.0",
-    "myst-nb",
+    "myst-nb>=1.1.0",
     "sphinxcontrib-bibtex>=1.0.0",
     "sphinx-autodoc-typehints",
     "sphinxext-opengraph",
     # For notebooks
     "ipykernel",
     "ipython",
     "sphinx-copybutton",
```

### Comparing `cellcharter-0.2.0/PKG-INFO` & `cellcharter-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: cellcharter
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package for the identification, characterization and comparison of spatial clusters from spatial -omics data.
 Project-URL: Documentation, https://cellcharter.readthedocs.io/
 Project-URL: Source, https://github.com/CSOgroup/cellcharter
 Project-URL: Home-page, https://github.com/CSOgroup/cellcharter
 Author: CSO group
 Maintainer-email: Marco Varrone <marco.varrone@unil.ch>
 License: BSD 3-Clause License
@@ -35,30 +35,31 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
 Requires-Python: <3.11,>=3.8
 Requires-Dist: anndata
+Requires-Dist: matplotlib<3.9.0
 Requires-Dist: pycave
 Requires-Dist: rasterio
 Requires-Dist: scikit-learn
 Requires-Dist: session-info
 Requires-Dist: sknw
 Requires-Dist: spatialdata
-Requires-Dist: spatialdata-plot
+Requires-Dist: spatialdata-plot>=0.1.0
 Requires-Dist: squidpy
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: twine>=4.0.2; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: docutils!=0.18.*,!=0.19.*,>=0.8; extra == 'doc'
 Requires-Dist: ipykernel; extra == 'doc'
 Requires-Dist: ipython; extra == 'doc'
-Requires-Dist: myst-nb; extra == 'doc'
+Requires-Dist: myst-nb>=1.1.0; extra == 'doc'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'doc'
 Requires-Dist: sphinx-book-theme>=1.0.0; extra == 'doc'
 Requires-Dist: sphinx-copybutton; extra == 'doc'
 Requires-Dist: sphinx>=4; extra == 'doc'
 Requires-Dist: sphinxcontrib-bibtex>=1.0.0; extra == 'doc'
 Requires-Dist: sphinxext-opengraph; extra == 'doc'
 Provides-Extra: proteomics
@@ -76,15 +77,16 @@
 **A Python package for the identification, characterization and comparison of spatial clusters from spatial -omics data.**
 
 ---
 
 <p align="center">
   <a href="https://cellcharter.readthedocs.io/en/latest/" target="_blank">Documentation</a> •
   <a href="https://cellcharter.readthedocs.io/en/latest/notebooks/codex_mouse_spleen.html" target="_blank">Examples</a> •
-  <a href="https://www.biorxiv.org/content/10.1101/2023.01.10.523386v1" target="_blank">Paper</a>
+  <a href="https://doi.org/10.1038/s41588-023-01588-4" target="_blank">Paper</a> •
+  <a href="https://www.biorxiv.org/content/10.1101/2023.01.10.523386v2" target="_blank">Preprint</a>
 </p>
 
 [![Tests][badge-tests]][link-tests]
 [![Documentation][badge-docs]][link-docs]
 
 [badge-tests]: https://img.shields.io/github/actions/workflow/status/CSOgroup/cellcharter/test.yaml?branch=main
 [link-tests]: https://github.com/CSOgroup/cellcharter/actions/workflows/test.yml
@@ -113,33 +115,42 @@
 Please refer to the [documentation][link-docs]. In particular, the
 
 -   [API documentation][link-api].
 -   [Tutorials][link-tutorial]
 
 ## Installation
 
-CellCharter uses Python < 3.11 and [PyTorch](https://pytorch.org) <= 1.12.1. If you are planning to use a GPU, make sure to download and install the correct version of PyTorch first.
-
-In CellCharter, only the dimensionality reduction and batch correction step is dependent on the data type. In particular, it uses:
-
--   [scVI](https://github.com/scverse/scvi-tools) for spatial transcriptomics data such as 10x Visium and Xenium, Nanostring CosMx, Vizgen MERSCOPE, Stereo-seq, DBiT-seq, MERFISH and seqFISH data.
--   A modified version of [scArches](https://github.com/theislab/scarches)'s TRVAE model for spatial proteomics data such as Akoya CODEX, Lunaphore COMET, CyCIF, IMC and MIBI-TOF data.
-
-By installing CellCharter without specifying the type of data, as in the following code, it will install without any of the two models.
+1. Create a conda or pyenv environment
+2. Install Python <= 3.10 and [PyTorch](https://pytorch.org) <= 1.12.1. If you are planning to use a GPU, make sure to download and install the correct version of PyTorch first.
+3. Install the library used for dimensionality reduction and batch effect removal according the data type you are planning to analyze:
+    - [scVI](https://github.com/scverse/scvi-tools) for spatial transcriptomics and/or epigenomics data such as 10x Visium and Xenium, Nanostring CosMx, Vizgen MERSCOPE, Stereo-seq, DBiT-seq, MERFISH and seqFISH data.
+    - A modified version of [scArches](https://github.com/theislab/scarches)'s TRVAE model for spatial proteomics data such as Akoya CODEX, Lunaphore COMET, CyCIF, IMC and MIBI-TOF data.
+4. Install CellCharter using pip:
 
 ```bash
 pip install cellcharter
 ```
 
-However, you can include in the installation the type of data (transcriptomics and/or proteomics) you are planning to analyze, and it will install the required dependencies.
+We suggest using `mamba` to install the dependencies.
+Installing the latest version of the dependencies (in particular `scvi-tools` and `spatialdata`) may lead to dependency conflicts.
+However, this should not be a problem because CellCharter doesn't use any of the mismatching features.
+
+We report here an example of an installation aimed at analyzing spatial transcriptomics data (and thus installing `scvi-tools`).
+This example is based on a Linux CentOS 7 system with an NVIDIA A100 GPU.
 
 ```bash
-pip install cellcharter[transcriptomics]
+conda create -n cellcharter-env -c conda-forge python=3.10 mamba
+conda activate cellcharter-env
+mamba install pytorch==1.12.1 torchvision==0.13.1 torchaudio==0.12.1 cudatoolkit=11.6 -c pytorch -c conda-forge
+pip install pyro-ppl==1.8.6 scvi-tools==0.20.3
+pip install cellcharter
 ```
 
+Note: a different system may require different commands to install PyTorch and JAX. Refer to their respective documentation for more details.
+
 ## Contribution
 
 If you found a bug or you want to propose a new feature, please use the [issue tracker][issue-tracker].
 
 [issue-tracker]: https://github.com/CSOgroup/cellcharter/issues
 [link-docs]: https://cellcharter.readthedocs.io
 [link-api]: https://cellcharter.readthedocs.io/en/latest/api.html
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cellcharter Version: 0.2.0 Summary: A Python
+Metadata-Version: 2.3 Name: cellcharter Version: 0.2.1 Summary: A Python
 package for the identification, characterization and comparison of spatial
 clusters from spatial -omics data. Project-URL: Documentation, https://
 cellcharter.readthedocs.io/ Project-URL: Source, https://github.com/CSOgroup/
 cellcharter Project-URL: Home-page, https://github.com/CSOgroup/cellcharter
 Author: CSO group Maintainer-email: Marco Varrone
 unil.ch> License: BSD 3-Clause License Copyright (c) 2022, Marco Varrone All
 rights reserved. Redistribution and use in source and binary forms, with or
@@ -21,33 +21,34 @@
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. License-
 File: LICENSE Requires-Python: <3.11,>=3.8 Requires-Dist: anndata Requires-
-Dist: pycave Requires-Dist: rasterio Requires-Dist: scikit-learn Requires-Dist:
-session-info Requires-Dist: sknw Requires-Dist: spatialdata Requires-Dist:
-spatialdata-plot Requires-Dist: squidpy Provides-Extra: dev Requires-Dist: pre-
-commit; extra == 'dev' Requires-Dist: twine>=4.0.2; extra == 'dev' Provides-
-Extra: doc Requires-Dist: docutils!=0.18.*,!=0.19.*,>=0.8; extra == 'doc'
-Requires-Dist: ipykernel; extra == 'doc' Requires-Dist: ipython; extra == 'doc'
-Requires-Dist: myst-nb; extra == 'doc' Requires-Dist: sphinx-autodoc-typehints;
-extra == 'doc' Requires-Dist: sphinx-book-theme>=1.0.0; extra == 'doc'
-Requires-Dist: sphinx-copybutton; extra == 'doc' Requires-Dist: sphinx>=4;
-extra == 'doc' Requires-Dist: sphinxcontrib-bibtex>=1.0.0; extra == 'doc'
-Requires-Dist: sphinxext-opengraph; extra == 'doc' Provides-Extra: proteomics
-Requires-Dist: scarches; extra == 'proteomics' Provides-Extra: test Requires-
-Dist: pytest; extra == 'test' Requires-Dist: pytest-cov; extra == 'test'
-Provides-Extra: transcriptomics Requires-Dist: scvi-tools; extra ==
-'transcriptomics' Description-Content-Type: text/markdown
+Dist: matplotlib<3.9.0 Requires-Dist: pycave Requires-Dist: rasterio Requires-
+Dist: scikit-learn Requires-Dist: session-info Requires-Dist: sknw Requires-
+Dist: spatialdata Requires-Dist: spatialdata-plot>=0.1.0 Requires-Dist: squidpy
+Provides-Extra: dev Requires-Dist: pre-commit; extra == 'dev' Requires-Dist:
+twine>=4.0.2; extra == 'dev' Provides-Extra: doc Requires-Dist:
+docutils!=0.18.*,!=0.19.*,>=0.8; extra == 'doc' Requires-Dist: ipykernel; extra
+== 'doc' Requires-Dist: ipython; extra == 'doc' Requires-Dist: myst-nb>=1.1.0;
+extra == 'doc' Requires-Dist: sphinx-autodoc-typehints; extra == 'doc'
+Requires-Dist: sphinx-book-theme>=1.0.0; extra == 'doc' Requires-Dist: sphinx-
+copybutton; extra == 'doc' Requires-Dist: sphinx>=4; extra == 'doc' Requires-
+Dist: sphinxcontrib-bibtex>=1.0.0; extra == 'doc' Requires-Dist: sphinxext-
+opengraph; extra == 'doc' Provides-Extra: proteomics Requires-Dist: scarches;
+extra == 'proteomics' Provides-Extra: test Requires-Dist: pytest; extra ==
+'test' Requires-Dist: pytest-cov; extra == 'test' Provides-Extra:
+transcriptomics Requires-Dist: scvi-tools; extra == 'transcriptomics'
+Description-Content-Type: text/markdown
         [https://github.com/CSOgroup/cellcharter/raw/main/docs/_static/
 cellcharter.png]**A Python package for the identification, characterization and
         comparison of spatial clusters from spatial -omics data.** ---
-                     _D_o_c_u_m_e_n_t_a_t_i_o_n â¢ _E_x_a_m_p_l_e_s â¢ _P_a_p_e_r
+               _D_o_c_u_m_e_n_t_a_t_i_o_n â¢ _E_x_a_m_p_l_e_s â¢ _P_a_p_e_r â¢ _P_r_e_p_r_i_n_t
 [![Tests][badge-tests]][link-tests] [![Documentation][badge-docs]][link-docs]
 [badge-tests]: https://img.shields.io/github/actions/workflow/status/CSOgroup/
  cellcharter/test.yaml?branch=main [link-tests]: https://github.com/CSOgroup/
  cellcharter/actions/workflows/test.yml [badge-docs]: https://img.shields.io/
                             readthedocs/cellcharter
 ## Background
 Spatial clustering determines cellular niches characterized by specific
@@ -58,27 +59,36 @@
                              spatial_clusters.png]
 CellCharter is able to automatically identify spatial clusters, and offers a
 suite of approaches for cluster characterization and comparison.
         [https://github.com/CSOgroup/cellcharter/raw/main/docs/_static/
                            cellcharter_workflow.png]
 ## Getting started Please refer to the [documentation][link-docs]. In
 particular, the - [API documentation][link-api]. - [Tutorials][link-tutorial]
-## Installation CellCharter uses Python < 3.11 and [PyTorch](https://
-pytorch.org) <= 1.12.1. If you are planning to use a GPU, make sure to download
-and install the correct version of PyTorch first. In CellCharter, only the
-dimensionality reduction and batch correction step is dependent on the data
-type. In particular, it uses: - [scVI](https://github.com/scverse/scvi-tools)
-for spatial transcriptomics data such as 10x Visium and Xenium, Nanostring
-CosMx, Vizgen MERSCOPE, Stereo-seq, DBiT-seq, MERFISH and seqFISH data. - A
-modified version of [scArches](https://github.com/theislab/scarches)'s TRVAE
-model for spatial proteomics data such as Akoya CODEX, Lunaphore COMET, CyCIF,
-IMC and MIBI-TOF data. By installing CellCharter without specifying the type of
-data, as in the following code, it will install without any of the two models.
-```bash pip install cellcharter ``` However, you can include in the
-installation the type of data (transcriptomics and/or proteomics) you are
-planning to analyze, and it will install the required dependencies. ```bash pip
-install cellcharter[transcriptomics] ``` ## Contribution If you found a bug or
-you want to propose a new feature, please use the [issue tracker][issue-
-tracker]. [issue-tracker]: https://github.com/CSOgroup/cellcharter/issues
-[link-docs]: https://cellcharter.readthedocs.io [link-api]: https://
-cellcharter.readthedocs.io/en/latest/api.html [link-tutorial]: https://
-cellcharter.readthedocs.io/en/latest/notebooks/codex_mouse_spleen.html
+## Installation 1. Create a conda or pyenv environment 2. Install Python <=
+3.10 and [PyTorch](https://pytorch.org) <= 1.12.1. If you are planning to use a
+GPU, make sure to download and install the correct version of PyTorch first. 3.
+Install the library used for dimensionality reduction and batch effect removal
+according the data type you are planning to analyze: - [scVI](https://
+github.com/scverse/scvi-tools) for spatial transcriptomics and/or epigenomics
+data such as 10x Visium and Xenium, Nanostring CosMx, Vizgen MERSCOPE, Stereo-
+seq, DBiT-seq, MERFISH and seqFISH data. - A modified version of [scArches]
+(https://github.com/theislab/scarches)'s TRVAE model for spatial proteomics
+data such as Akoya CODEX, Lunaphore COMET, CyCIF, IMC and MIBI-TOF data. 4.
+Install CellCharter using pip: ```bash pip install cellcharter ``` We suggest
+using `mamba` to install the dependencies. Installing the latest version of the
+dependencies (in particular `scvi-tools` and `spatialdata`) may lead to
+dependency conflicts. However, this should not be a problem because CellCharter
+doesn't use any of the mismatching features. We report here an example of an
+installation aimed at analyzing spatial transcriptomics data (and thus
+installing `scvi-tools`). This example is based on a Linux CentOS 7 system with
+an NVIDIA A100 GPU. ```bash conda create -n cellcharter-env -c conda-forge
+python=3.10 mamba conda activate cellcharter-env mamba install pytorch==1.12.1
+torchvision==0.13.1 torchaudio==0.12.1 cudatoolkit=11.6 -c pytorch -c conda-
+forge pip install pyro-ppl==1.8.6 scvi-tools==0.20.3 pip install cellcharter
+``` Note: a different system may require different commands to install PyTorch
+and JAX. Refer to their respective documentation for more details. ##
+Contribution If you found a bug or you want to propose a new feature, please
+use the [issue tracker][issue-tracker]. [issue-tracker]: https://github.com/
+CSOgroup/cellcharter/issues [link-docs]: https://cellcharter.readthedocs.io
+[link-api]: https://cellcharter.readthedocs.io/en/latest/api.html [link-
+tutorial]: https://cellcharter.readthedocs.io/en/latest/notebooks/
+codex_mouse_spleen.html
```

