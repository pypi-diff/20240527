# Comparing `tmp/squidpy-1.4.1.tar.gz` & `tmp/squidpy-1.5.0.tar.gz`

## Comparing `squidpy-1.4.1.tar` & `squidpy-1.5.0.tar`

### file list

```diff
@@ -1,243 +1,244 @@
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 squidpy-1.4.1/.bumpversion.cfg
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 squidpy-1.4.1/.cruft.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 squidpy-1.4.1/.editorconfig
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 squidpy-1.4.1/.gitmodules
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 squidpy-1.4.1/.mypy.ini
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 squidpy-1.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 squidpy-1.4.1/.prettierignore
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 squidpy-1.4.1/.readthedocs.yml
--rw-r--r--   0        0        0     7692 2020-02-02 00:00:00.000000 squidpy-1.4.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 squidpy-1.4.1/MANIFEST.in
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 squidpy-1.4.1/README_pypi.rst
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 squidpy-1.4.1/tox.ini
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 squidpy-1.4.1/.github/.codecov.yml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 squidpy-1.4.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 squidpy-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 squidpy-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 squidpy-1.4.1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 squidpy-1.4.1/.github/workflows/build.yml
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 squidpy-1.4.1/.github/workflows/deployment.yml
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 squidpy-1.4.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 squidpy-1.4.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 squidpy-1.4.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 squidpy-1.4.1/.scripts/ci/download_data.py
--rwxr-xr-x   0        0        0      527 2020-02-02 00:00:00.000000 squidpy-1.4.1/.scripts/ci/install_dependencies.sh
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/Makefile
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/api.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/classes.rst
--rw-r--r--   0        0        0     6329 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/conf.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/index.rst
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/installation.rst
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/make.bat
--rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/references.bib
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/references.rst
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/release_notes.rst
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/utils.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/_ext/typed_returns.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/_static/css/custom.css
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/_static/css/dataframe.css
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/_static/css/nbsphinx.css
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/_static/css/sphinx_gallery.css
--rw-r--r--   0        0        0   911945 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/_static/img/figure1.png
--rw-r--r--   0        0        0    29642 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/_static/img/squidpy_horizontal.png
--rw-r--r--   0        0        0    20146 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/_static/img/squidpy_vertical.png
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/_templates/breadcrumbs.html
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/release/notes-1.0.0.rst
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/release/notes-1.0.1.rst
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/release/notes-1.1.0.rst
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/release/notes-1.1.1.rst
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/release/notes-1.1.2.rst
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/release/notes-1.2.0.rst
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/release/notes-1.2.1.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/release/notes-1.2.2.rst
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/release/notes-1.2.3.rst
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/release/notes-1.3.0.rst
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/release/notes-1.3.1.rst
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/release/notes-1.4.0.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/release/notes-1.4.1.rst
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 squidpy-1.4.1/docs/release/notes-dev.rst
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/__init__.py
--rw-r--r--   0        0        0    14070 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/_docs.py
--rw-r--r--   0        0        0     9618 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/_constants/__init__.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/_constants/_constants.py
--rw-r--r--   0        0        0     6674 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/_constants/_pkg_constants.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/_constants/_utils.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/datasets/_10x_datasets.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/datasets/__init__.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/datasets/_dataset.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/datasets/_dataset.pyi
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/datasets/_image.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/datasets/_image.pyi
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/datasets/_utils.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/gr/__init__.py
--rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/gr/_build.py
--rw-r--r--   0        0        0    31974 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/gr/_ligrec.py
--rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/gr/_nhood.py
--rw-r--r--   0        0        0    19367 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/gr/_ppatterns.py
--rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/gr/_ripley.py
--rw-r--r--   0        0        0    10860 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/gr/_sepal.py
--rw-r--r--   0        0        0    11034 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/gr/_utils.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/im/__init__.py
--rw-r--r--   0        0        0    60127 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/im/_container.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/im/_coords.py
--rw-r--r--   0        0        0     5462 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/im/_feature.py
--rw-r--r--   0        0        0    18604 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/im/_feature_mixin.py
--rw-r--r--   0        0        0     9682 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/im/_io.py
--rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/im/_process.py
--rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/im/_segment.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/pl/__init__.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/pl/_color_utils.py
--rw-r--r--   0        0        0    11779 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/pl/_graph.py
--rw-r--r--   0        0        0    15942 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/pl/_ligrec.py
--rw-r--r--   0        0        0    15744 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/pl/_spatial.py
--rw-r--r--   0        0        0    36118 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/pl/_spatial_utils.py
--rw-r--r--   0        0        0    21664 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/pl/_utils.py
--rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/pl/_var_by_distance.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/pl/_interactive/__init__.py
--rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/pl/_interactive/_controller.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/pl/_interactive/_model.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/pl/_interactive/_utils.py
--rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/pl/_interactive/_view.py
--rw-r--r--   0        0        0    12192 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/pl/_interactive/_widgets.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/pl/_interactive/interactive.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/read/__init__.py
--rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/read/_read.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/read/_utils.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/tl/__init__.py
--rw-r--r--   0        0        0    10966 2020-02-02 00:00:00.000000 squidpy-1.4.1/src/squidpy/tl/_var_by_distance.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/__init__.py
--rw-r--r--   0        0        0    11281 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/conftest.py
--rw-r--r--   0        0        0    35962 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_data/filtered_feature_bc_matrix.h5
--rw-r--r--   0        0        0    15619 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_data/ligrec_no_numba.pickle
--rw-r--r--   0        0        0    87822 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_data/paul15_means.pickle
--rw-r--r--   0        0        0   602117 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_data/test_data.h5ad
--rw-r--r--   0        0        0   229870 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_data/test_img.jpg
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_data/spatial/scalefactors_json.json
--rw-r--r--   0        0        0    20014 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_data/spatial/tissue_hires_image.png
--rw-r--r--   0        0        0   518124 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_data/spatial/tissue_lowres_image.png
--rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_data/spatial/tissue_positions_list.csv
--rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/ContainerShow_axis.png
--rw-r--r--   0        0        0    95400 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/ContainerShow_channel.png
--rw-r--r--   0        0        0    91924 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/ContainerShow_channelwise.png
--rw-r--r--   0        0        0   129565 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/ContainerShow_channelwise_segmentation.png
--rw-r--r--   0        0        0   122974 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/ContainerShow_imshow_kwargs.png
--rw-r--r--   0        0        0   119898 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/ContainerShow_library_id.png
--rw-r--r--   0        0        0    51525 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/ContainerShow_scale_mask_circle_crop.png
--rw-r--r--   0        0        0   140839 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/ContainerShow_segmentation.png
--rw-r--r--   0        0        0    67164 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/ContainerShow_transpose_channelwise_False_False.png
--rw-r--r--   0        0        0   180591 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/ContainerShow_transpose_channelwise_False_True.png
--rw-r--r--   0        0        0   236892 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/ContainerShow_transpose_channelwise_True_False.png
--rw-r--r--   0        0        0    76745 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/ContainerShow_transpose_channelwise_True_True.png
--rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Graph_centrality_scores.png
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Graph_centrality_scores_single.png
--rw-r--r--   0        0        0    31775 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Graph_co_occurrence.png
--rw-r--r--   0        0        0    32008 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Graph_co_occurrence_palette.png
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Graph_interaction.png
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Graph_interaction_dendro.png
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Graph_nhood_enrichment.png
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Graph_nhood_enrichment_ax.png
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Graph_nhood_enrichment_dendro.png
--rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Graph_ripley_f.png
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Graph_ripley_f_nopalette.png
--rw-r--r--   0        0        0     5429 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Graph_ripley_g.png
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Graph_ripley_l.png
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Heatmap_cbar_kwargs.png
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Heatmap_cbar_vmin_vmax.png
--rw-r--r--   0        0        0    19521 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Ligrec_alpha.png
--rw-r--r--   0        0        0    18044 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Ligrec_alpha_none.png
--rw-r--r--   0        0        0    19242 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Ligrec_cmap.png
--rw-r--r--   0        0        0    19252 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Ligrec_dendrogram_both.png
--rw-r--r--   0        0        0    20981 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Ligrec_dendrogram_clusters.png
--rw-r--r--   0        0        0    20530 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Ligrec_dendrogram_pairs.png
--rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Ligrec_kwargs.png
--rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Ligrec_means_range.png
--rw-r--r--   0        0        0    29501 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Ligrec_no_remove_empty_interactions.png
--rw-r--r--   0        0        0    14454 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Ligrec_pvalue_threshold.png
--rw-r--r--   0        0        0    17685 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Ligrec_remove_empty_interactions.png
--rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Ligrec_remove_nonsig_interactions.png
--rw-r--r--   0        0        0    10701 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Ligrec_source_clusters.png
--rw-r--r--   0        0        0    20234 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Ligrec_swap_axes.png
--rw-r--r--   0        0        0    21101 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Ligrec_swap_axes_dedrogram.png
--rw-r--r--   0        0        0    10949 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Ligrec_target_clusters.png
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_add_image.png
--rw-r--r--   0        0        0    21995 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_blending.png
--rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_cat_cmap.png
--rw-r--r--   0        0        0    21738 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_cont_cmap.png
--rw-r--r--   0        0        0     9231 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_corner_case_-200_-200_600_800.png
--rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_corner_case_-200_-200_800_600.png
--rw-r--r--   0        0        0    12504 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_corner_case_-200_-200_800_800.png
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_corner_case_-200_200_600_800.png
--rw-r--r--   0        0        0    12407 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_corner_case_-200_200_800_600.png
--rw-r--r--   0        0        0    15960 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_corner_case_-200_200_800_800.png
--rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_corner_case_200_-200_600_800.png
--rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_corner_case_200_-200_800_600.png
--rw-r--r--   0        0        0    16043 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_corner_case_200_-200_800_800.png
--rw-r--r--   0        0        0    17445 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_corner_case_200_200_600_800.png
--rw-r--r--   0        0        0    16287 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_corner_case_200_200_800_600.png
--rw-r--r--   0        0        0    21234 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_corner_case_200_200_800_800.png
--rw-r--r--   0        0        0    28180 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_crop_center.png
--rw-r--r--   0        0        0    17228 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_crop_corner.png
--rw-r--r--   0        0        0    21848 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_gene_X.png
--rw-r--r--   0        0        0    22045 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_obs_categorical.png
--rw-r--r--   0        0        0    21794 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_obs_continuous.png
--rw-r--r--   0        0        0    25425 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_scalefactor.png
--rw-r--r--   0        0        0    20173 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_simple_canvas.png
--rw-r--r--   0        0        0    18340 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_symbol.png
--rw-r--r--   0        0        0    14849 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/Napari_viewer_canvas.png
--rw-r--r--   0        0        0    51439 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_palette_listed_cmap.png
--rw-r--r--   0        0        0     9002 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_axfig.png
--rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_categorical_alpha.png
--rw-r--r--   0        0        0    93592 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_crop.png
--rw-r--r--   0        0        0    41672 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_crop_graph.png
--rw-r--r--   0        0        0   118281 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_crop_noorigin.png
--rw-r--r--   0        0        0   142407 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_group.png
--rw-r--r--   0        0        0    51931 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_group_multi.png
--rw-r--r--   0        0        0    25974 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_group_outline.png
--rw-r--r--   0        0        0    57879 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_image.png
--rw-r--r--   0        0        0    22237 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_noimage.png
--rw-r--r--   0        0        0    51647 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_non_unique_colors.png
--rw-r--r--   0        0        0    35072 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_nospatial.png
--rw-r--r--   0        0        0    64688 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_novisium.png
--rw-r--r--   0        0        0    48845 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_title_single.png
--rw-r--r--   0        0        0   114278 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_segment.png
--rw-r--r--   0        0        0   247009 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_segment_crop.png
--rw-r--r--   0        0        0    82158 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/SpatialStatic_spatial_segment_group.png
--rw-r--r--   0        0        0    31379 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/var_by_distance_single_anchor_and_gene.png
--rw-r--r--   0        0        0    20962 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/var_by_distance_single_anchor_and_gene_two_categories.png
--rw-r--r--   0        0        0   104786 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/var_by_distance_single_anchor_four_genes_two_categories_two_palettes.png
--rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/_images/var_by_distance_single_anchor_one_gene_two_categories_without_scatter.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/datasets/__init__.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/datasets/test_dataset.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/datasets/test_download_visium_dataset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/graph/__init__.py
--rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/graph/test_ligrec.py
--rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/graph/test_nhood.py
--rw-r--r--   0        0        0     6969 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/graph/test_ppatterns.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/graph/test_ripley.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/graph/test_sepal.py
--rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/graph/test_spatial_neighbors.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/graph/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/image/__init__.py
--rw-r--r--   0        0        0    55061 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/image/test_container.py
--rw-r--r--   0        0        0    10534 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/image/test_features.py
--rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/image/test_io.py
--rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/image/test_processing.py
--rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/image/test_segmentation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/plotting/__init__.py
--rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/plotting/test_graph.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/plotting/test_image.py
--rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/plotting/test_interactive.py
--rw-r--r--   0        0        0     9547 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/plotting/test_spatial_static.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/plotting/test_var_by_distance_plot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/read/__init__.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/read/test_visium.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/tools/__init__.py
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 squidpy-1.4.1/tests/tools/test_var_by_distance.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 squidpy-1.4.1/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 squidpy-1.4.1/LICENSE
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 squidpy-1.4.1/README.rst
--rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 squidpy-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     8847 2020-02-02 00:00:00.000000 squidpy-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 squidpy-1.5.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 squidpy-1.5.0/.cruft.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 squidpy-1.5.0/.editorconfig
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 squidpy-1.5.0/.gitmodules
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 squidpy-1.5.0/.mypy.ini
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 squidpy-1.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 squidpy-1.5.0/.prettierignore
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 squidpy-1.5.0/.readthedocs.yml
+-rw-r--r--   0        0        0     7692 2020-02-02 00:00:00.000000 squidpy-1.5.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 squidpy-1.5.0/MANIFEST.in
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 squidpy-1.5.0/README_pypi.rst
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 squidpy-1.5.0/tox.ini
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 squidpy-1.5.0/.github/.codecov.yml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 squidpy-1.5.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 squidpy-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 squidpy-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 squidpy-1.5.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 squidpy-1.5.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 squidpy-1.5.0/.github/workflows/deployment.yml
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 squidpy-1.5.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 squidpy-1.5.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 squidpy-1.5.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 squidpy-1.5.0/.scripts/ci/download_data.py
+-rwxr-xr-x   0        0        0      527 2020-02-02 00:00:00.000000 squidpy-1.5.0/.scripts/ci/install_dependencies.sh
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/Makefile
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/api.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/classes.rst
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/conf.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/index.rst
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/installation.rst
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/make.bat
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/references.bib
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/references.rst
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/release_notes.rst
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/utils.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/_ext/typed_returns.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/_static/css/custom.css
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/_static/css/dataframe.css
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/_static/css/nbsphinx.css
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/_static/css/sphinx_gallery.css
+-rw-r--r--   0        0        0   911945 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/_static/img/figure1.png
+-rw-r--r--   0        0        0    29642 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/_static/img/squidpy_horizontal.png
+-rw-r--r--   0        0        0    20146 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/_static/img/squidpy_vertical.png
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/_templates/breadcrumbs.html
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/release/notes-1.0.0.rst
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/release/notes-1.0.1.rst
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/release/notes-1.1.0.rst
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/release/notes-1.1.1.rst
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/release/notes-1.1.2.rst
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/release/notes-1.2.0.rst
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/release/notes-1.2.1.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/release/notes-1.2.2.rst
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/release/notes-1.2.3.rst
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/release/notes-1.3.0.rst
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/release/notes-1.3.1.rst
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/release/notes-1.4.0.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/release/notes-1.4.1.rst
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/release/notes-1.5.0.rst
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 squidpy-1.5.0/docs/release/notes-dev.rst
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/__init__.py
+-rw-r--r--   0        0        0    14070 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/_docs.py
+-rw-r--r--   0        0        0     9587 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/_constants/__init__.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/_constants/_constants.py
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/_constants/_pkg_constants.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/_constants/_utils.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/datasets/_10x_datasets.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/datasets/__init__.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/datasets/_dataset.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/datasets/_dataset.pyi
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/datasets/_image.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/datasets/_image.pyi
+-rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/datasets/_utils.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/gr/__init__.py
+-rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/gr/_build.py
+-rw-r--r--   0        0        0    32029 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/gr/_ligrec.py
+-rw-r--r--   0        0        0    13300 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/gr/_nhood.py
+-rw-r--r--   0        0        0    20316 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/gr/_ppatterns.py
+-rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/gr/_ripley.py
+-rw-r--r--   0        0        0    10836 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/gr/_sepal.py
+-rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/gr/_utils.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/im/__init__.py
+-rw-r--r--   0        0        0    60086 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/im/_container.py
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/im/_coords.py
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/im/_feature.py
+-rw-r--r--   0        0        0    18594 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/im/_feature_mixin.py
+-rw-r--r--   0        0        0     9657 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/im/_io.py
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/im/_process.py
+-rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/im/_segment.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/pl/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/pl/_color_utils.py
+-rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/pl/_graph.py
+-rw-r--r--   0        0        0    15892 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/pl/_ligrec.py
+-rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/pl/_spatial.py
+-rw-r--r--   0        0        0    36194 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/pl/_spatial_utils.py
+-rw-r--r--   0        0        0    21629 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/pl/_utils.py
+-rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/pl/_var_by_distance.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/pl/_interactive/__init__.py
+-rw-r--r--   0        0        0    11977 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/pl/_interactive/_controller.py
+-rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/pl/_interactive/_model.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/pl/_interactive/_utils.py
+-rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/pl/_interactive/_view.py
+-rw-r--r--   0        0        0    12212 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/pl/_interactive/_widgets.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/pl/_interactive/interactive.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/read/__init__.py
+-rw-r--r--   0        0        0    10953 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/read/_read.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/read/_utils.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/tl/__init__.py
+-rw-r--r--   0        0        0    10916 2020-02-02 00:00:00.000000 squidpy-1.5.0/src/squidpy/tl/_var_by_distance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/__init__.py
+-rw-r--r--   0        0        0    11125 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/conftest.py
+-rw-r--r--   0        0        0    35962 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_data/filtered_feature_bc_matrix.h5
+-rw-r--r--   0        0        0    15619 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_data/ligrec_no_numba.pickle
+-rw-r--r--   0        0        0    87822 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_data/paul15_means.pickle
+-rw-r--r--   0        0        0   602117 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_data/test_data.h5ad
+-rw-r--r--   0        0        0   229870 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_data/test_img.jpg
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_data/spatial/scalefactors_json.json
+-rw-r--r--   0        0        0    20014 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_data/spatial/tissue_hires_image.png
+-rw-r--r--   0        0        0   518124 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_data/spatial/tissue_lowres_image.png
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_data/spatial/tissue_positions_list.csv
+-rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/ContainerShow_axis.png
+-rw-r--r--   0        0        0    95400 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/ContainerShow_channel.png
+-rw-r--r--   0        0        0    91924 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/ContainerShow_channelwise.png
+-rw-r--r--   0        0        0   129565 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/ContainerShow_channelwise_segmentation.png
+-rw-r--r--   0        0        0   122974 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/ContainerShow_imshow_kwargs.png
+-rw-r--r--   0        0        0   119898 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/ContainerShow_library_id.png
+-rw-r--r--   0        0        0    51525 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/ContainerShow_scale_mask_circle_crop.png
+-rw-r--r--   0        0        0   140839 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/ContainerShow_segmentation.png
+-rw-r--r--   0        0        0    67164 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/ContainerShow_transpose_channelwise_False_False.png
+-rw-r--r--   0        0        0   180591 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/ContainerShow_transpose_channelwise_False_True.png
+-rw-r--r--   0        0        0   236892 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/ContainerShow_transpose_channelwise_True_False.png
+-rw-r--r--   0        0        0    76745 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/ContainerShow_transpose_channelwise_True_True.png
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Graph_centrality_scores.png
+-rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Graph_centrality_scores_single.png
+-rw-r--r--   0        0        0    31775 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Graph_co_occurrence.png
+-rw-r--r--   0        0        0    32008 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Graph_co_occurrence_palette.png
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Graph_interaction.png
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Graph_interaction_dendro.png
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Graph_nhood_enrichment.png
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Graph_nhood_enrichment_ax.png
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Graph_nhood_enrichment_dendro.png
+-rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Graph_ripley_f.png
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Graph_ripley_f_nopalette.png
+-rw-r--r--   0        0        0     5429 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Graph_ripley_g.png
+-rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Graph_ripley_l.png
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Heatmap_cbar_kwargs.png
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Heatmap_cbar_vmin_vmax.png
+-rw-r--r--   0        0        0    19521 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Ligrec_alpha.png
+-rw-r--r--   0        0        0    18044 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Ligrec_alpha_none.png
+-rw-r--r--   0        0        0    19242 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Ligrec_cmap.png
+-rw-r--r--   0        0        0    19252 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Ligrec_dendrogram_both.png
+-rw-r--r--   0        0        0    20981 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Ligrec_dendrogram_clusters.png
+-rw-r--r--   0        0        0    20530 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Ligrec_dendrogram_pairs.png
+-rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Ligrec_kwargs.png
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Ligrec_means_range.png
+-rw-r--r--   0        0        0    29501 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Ligrec_no_remove_empty_interactions.png
+-rw-r--r--   0        0        0    14454 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Ligrec_pvalue_threshold.png
+-rw-r--r--   0        0        0    17685 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Ligrec_remove_empty_interactions.png
+-rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Ligrec_remove_nonsig_interactions.png
+-rw-r--r--   0        0        0    10701 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Ligrec_source_clusters.png
+-rw-r--r--   0        0        0    20234 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Ligrec_swap_axes.png
+-rw-r--r--   0        0        0    21101 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Ligrec_swap_axes_dedrogram.png
+-rw-r--r--   0        0        0    10949 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Ligrec_target_clusters.png
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_add_image.png
+-rw-r--r--   0        0        0    21995 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_blending.png
+-rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_cat_cmap.png
+-rw-r--r--   0        0        0    21738 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_cont_cmap.png
+-rw-r--r--   0        0        0     9231 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_corner_case_-200_-200_600_800.png
+-rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_corner_case_-200_-200_800_600.png
+-rw-r--r--   0        0        0    12504 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_corner_case_-200_-200_800_800.png
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_corner_case_-200_200_600_800.png
+-rw-r--r--   0        0        0    12407 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_corner_case_-200_200_800_600.png
+-rw-r--r--   0        0        0    15960 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_corner_case_-200_200_800_800.png
+-rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_corner_case_200_-200_600_800.png
+-rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_corner_case_200_-200_800_600.png
+-rw-r--r--   0        0        0    16043 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_corner_case_200_-200_800_800.png
+-rw-r--r--   0        0        0    17445 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_corner_case_200_200_600_800.png
+-rw-r--r--   0        0        0    16287 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_corner_case_200_200_800_600.png
+-rw-r--r--   0        0        0    21234 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_corner_case_200_200_800_800.png
+-rw-r--r--   0        0        0    28180 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_crop_center.png
+-rw-r--r--   0        0        0    17228 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_crop_corner.png
+-rw-r--r--   0        0        0    21848 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_gene_X.png
+-rw-r--r--   0        0        0    22045 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_obs_categorical.png
+-rw-r--r--   0        0        0    21794 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_obs_continuous.png
+-rw-r--r--   0        0        0    25425 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_scalefactor.png
+-rw-r--r--   0        0        0    20173 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_simple_canvas.png
+-rw-r--r--   0        0        0    18340 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_symbol.png
+-rw-r--r--   0        0        0    14849 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/Napari_viewer_canvas.png
+-rw-r--r--   0        0        0    51439 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_palette_listed_cmap.png
+-rw-r--r--   0        0        0     9002 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_axfig.png
+-rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_categorical_alpha.png
+-rw-r--r--   0        0        0    93592 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_crop.png
+-rw-r--r--   0        0        0    41672 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_crop_graph.png
+-rw-r--r--   0        0        0   118281 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_crop_noorigin.png
+-rw-r--r--   0        0        0   142407 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_group.png
+-rw-r--r--   0        0        0    51931 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_group_multi.png
+-rw-r--r--   0        0        0    25974 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_group_outline.png
+-rw-r--r--   0        0        0    57879 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_image.png
+-rw-r--r--   0        0        0    22237 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_noimage.png
+-rw-r--r--   0        0        0    51647 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_non_unique_colors.png
+-rw-r--r--   0        0        0    35072 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_nospatial.png
+-rw-r--r--   0        0        0    64688 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_novisium.png
+-rw-r--r--   0        0        0    48845 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_title_single.png
+-rw-r--r--   0        0        0   114278 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_segment.png
+-rw-r--r--   0        0        0   247009 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_segment_crop.png
+-rw-r--r--   0        0        0    82158 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/SpatialStatic_spatial_segment_group.png
+-rw-r--r--   0        0        0    31379 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/var_by_distance_single_anchor_and_gene.png
+-rw-r--r--   0        0        0    20962 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/var_by_distance_single_anchor_and_gene_two_categories.png
+-rw-r--r--   0        0        0   104786 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/var_by_distance_single_anchor_four_genes_two_categories_two_palettes.png
+-rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/_images/var_by_distance_single_anchor_one_gene_two_categories_without_scatter.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/datasets/__init__.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/datasets/test_dataset.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/datasets/test_download_visium_dataset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/graph/__init__.py
+-rw-r--r--   0        0        0    19165 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/graph/test_ligrec.py
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/graph/test_nhood.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/graph/test_ppatterns.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/graph/test_ripley.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/graph/test_sepal.py
+-rw-r--r--   0        0        0     9898 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/graph/test_spatial_neighbors.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/graph/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/image/__init__.py
+-rw-r--r--   0        0        0    54905 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/image/test_container.py
+-rw-r--r--   0        0        0    10572 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/image/test_features.py
+-rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/image/test_io.py
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/image/test_processing.py
+-rw-r--r--   0        0        0    10691 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/image/test_segmentation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/plotting/__init__.py
+-rw-r--r--   0        0        0     8864 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/plotting/test_graph.py
+-rw-r--r--   0        0        0     4745 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/plotting/test_image.py
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/plotting/test_interactive.py
+-rw-r--r--   0        0        0     9509 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/plotting/test_spatial_static.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/plotting/test_var_by_distance_plot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/read/__init__.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/read/test_visium.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/tools/__init__.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 squidpy-1.5.0/tests/tools/test_var_by_distance.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 squidpy-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 squidpy-1.5.0/LICENSE
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 squidpy-1.5.0/README.rst
+-rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 squidpy-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8847 2020-02-02 00:00:00.000000 squidpy-1.5.0/PKG-INFO
```

### Comparing `squidpy-1.4.1/.cruft.json` & `squidpy-1.5.0/.cruft.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7984375%*

 * *Differences: {"'checkout'": "'v0.4.0'",*

 * * "'commit'": "'87a407a65408d75a949c0b54b19fd287475a56f8'",*

 * * "'context'": "{'cookiecutter': {'_copy_without_render': {insert: [(0, "*

 * *              "'.github/workflows/build.yaml'), (1, '.github/workflows/test.yaml')], delete: "*

 * *              '[0]}}}'}*

```diff
@@ -1,14 +1,15 @@
 {
-    "checkout": "v0.3.0",
-    "commit": "8e96abb5c3e2d5078c44713958da672711cf2a48",
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
             "_jinja2_env_vars": {
                 "lstrip_blocks": true,
                 "trim_blocks": true
             },
             "_render_devdocs": false,
```

### Comparing `squidpy-1.4.1/.mypy.ini` & `squidpy-1.5.0/.mypy.ini`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/.pre-commit-config.yaml` & `squidpy-1.5.0/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -3,30 +3,25 @@
     python: python3
 default_stages:
     - commit
     - push
 minimum_pre_commit_version: 2.9.3
 repos:
     - repo: https://github.com/pre-commit/mirrors-mypy
-      rev: v1.8.0
+      rev: v1.10.0
       hooks:
           - id: mypy
             additional_dependencies: [numpy, pandas, types-requests]
             exclude: .scripts/ci/download_data.py|squidpy/datasets/_(dataset|image).py # See https://github.com/pre-commit/mirrors-mypy/issues/33
-    - repo: https://github.com/psf/black
-      rev: 24.1.1
-      hooks:
-          - id: black
-            additional_dependencies: [toml]
     - repo: https://github.com/pre-commit/mirrors-prettier
       rev: v4.0.0-alpha.8
       hooks:
           - id: prettier
     - repo: https://github.com/pre-commit/pre-commit-hooks
-      rev: v4.5.0
+      rev: v4.6.0
       hooks:
           - id: detect-private-key
           - id: check-merge-conflict
           - id: check-ast
           - id: check-symlinks
           - id: check-added-large-files
           - id: check-executables-have-shebangs
@@ -46,24 +41,22 @@
           - id: requirements-txt-fixer
     - repo: https://github.com/jumanjihouse/pre-commit-hooks
       rev: 3.0.0
       hooks:
           - id: script-must-have-extension
             name: Check executable files use .sh extension
             types: [shell, executable]
-    - repo: https://github.com/asottile/blacken-docs
-      rev: 1.16.0
-      hooks:
-          - id: blacken-docs
     - repo: https://github.com/astral-sh/ruff-pre-commit
-      # Ruff version.
-      rev: v0.2.0
+      rev: v0.4.5
       hooks:
           - id: ruff
+            types_or: [python, pyi, jupyter]
             args: [--fix, --exit-non-zero-on-fix]
+          - id: ruff-format
+            types_or: [python, pyi, jupyter]
     - repo: https://github.com/pre-commit/pygrep-hooks
       rev: v1.10.0
       hooks:
           - id: python-no-eval
           - id: python-use-type-annotations
           - id: python-check-blanket-noqa
           - id: rst-backticks
```

### Comparing `squidpy-1.4.1/CONTRIBUTING.rst` & `squidpy-1.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/README_pypi.rst` & `squidpy-1.5.0/README_pypi.rst`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tox.ini` & `squidpy-1.5.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 [pytest]
 python_files = test_*.py
 testpaths = tests/
 xfail_strict = true
 qt_api=pyqt5
-; addopts = -n auto
 
 filterwarnings =
     ignore::UserWarning
-    ignore:Using or importing the ABCs from 'collections':DeprecationWarning
-    ignore:Converting `np.inexact`:DeprecationWarning
-    ignore:the matrix subclass is:PendingDeprecationWarning
-    ignore:Please use:DeprecationWarning:dask_image.*
-    ignore:Auto-removal of grids by:DeprecationWarning:
-    ignore:Support for passing numbers through unit converters:DeprecationWarning
-    ignore:distutils Version classes are deprecated:DeprecationWarning
     ignore::anndata.OldFormatWarning
+    ignore:.*pkg_resources:DeprecationWarning
 
 [coverage:run]
 branch = true
 parallel = true
 source = squidpy
 omit =
     */__init__.py
```

### Comparing `squidpy-1.4.1/.github/workflows/build.yml` & `squidpy-1.5.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/.github/workflows/deployment.yml` & `squidpy-1.5.0/.github/workflows/deployment.yml`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/.github/workflows/lint.yml` & `squidpy-1.5.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/.github/workflows/release.yml` & `squidpy-1.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/.github/workflows/test.yml` & `squidpy-1.5.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/.scripts/ci/download_data.py` & `squidpy-1.5.0/.scripts/ci/download_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 #!/usr/bin/env python3
+from __future__ import annotations
+
 import argparse
 from pathlib import Path
 from typing import Any
 
 _CNT = 0  # increment this when you want to rebuild the CI cache
 _ROOT = Path.home() / ".cache" / "squidpy"
```

### Comparing `squidpy-1.4.1/.scripts/ci/install_dependencies.sh` & `squidpy-1.5.0/.scripts/ci/install_dependencies.sh`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/Makefile` & `squidpy-1.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/api.rst` & `squidpy-1.5.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/conf.py` & `squidpy-1.5.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Configuration file for the Sphinx documentation builder.
-#
+
 # This file only contains a selection of the most common options. For a full
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
+from __future__ import annotations
+
 # -- Path setup --------------------------------------------------------------
 import os
 import sys
 from datetime import datetime
 
 # from importlib.metadata import metadata
 from pathlib import Path
```

### Comparing `squidpy-1.4.1/docs/index.rst` & `squidpy-1.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/make.bat` & `squidpy-1.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/references.bib` & `squidpy-1.5.0/docs/references.bib`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/spelling_wordlist.txt` & `squidpy-1.5.0/docs/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/utils.py` & `squidpy-1.5.0/docs/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+from __future__ import annotations
+
 import os
 import re
 from logging import info, warning
 from pathlib import Path
 from shutil import copytree, rmtree
 from tempfile import TemporaryDirectory
-from typing import Any, Dict, ForwardRef, List, Union
+from typing import Any, ForwardRef
 
 from enchant.tokenize import Filter
 from git import Repo
 from sphinx_gallery.directives import MiniGallery
 
 HERE = Path(__file__).parent
 
 
 def _fetch_notebooks(repo_url: str) -> None:
-    def copy_files(repo_path: Union[str, Path]) -> None:
+    def copy_files(repo_path: str | Path) -> None:
         repo_path = Path(repo_path)
 
         for dirname in ["tutorials", "auto_examples", "gen_modules"]:
             rmtree(dirname, ignore_errors=True)  # locally re-cloning
             copytree(repo_path / "docs" / "source" / dirname, dirname)
 
     def fetch_remote(repo_url: str) -> None:
@@ -26,15 +28,15 @@
         with TemporaryDirectory() as repo_dir:
             ref = "main"
             repo = Repo.clone_from(repo_url, repo_dir, depth=1, branch=ref)
             repo.git.checkout(ref, force=True)
 
             copy_files(repo_dir)
 
-    def fetch_local(repo_path: Union[str, Path]) -> None:
+    def fetch_local(repo_path: str | Path) -> None:
         info(f"Fetching notebooks from local path `{repo_path}`")
         repo_path = Path(repo_path)
         if not repo_path.is_dir():
             raise OSError(f"Path `{repo_path}` is not a directory.")
 
         copy_files(repo_path)
 
@@ -71,15 +73,15 @@
         try:
             return super().run()  # type: ignore[no-any-return]
         except UnboundLocalError:
             # no gallery files
             return []
 
 
-def _get_thumbnails(root: Union[str, Path]) -> dict[str, str]:
+def _get_thumbnails(root: str | Path) -> dict[str, str]:
     res = {}
     root = Path(root)
     thumb_path = Path(__file__).parent.parent.parent / "docs" / "source"
 
     for fname in root.glob("**/*.py"):
         path, name = os.path.split(str(fname)[:-3])
         thumb_fname = f"sphx_glr_{name}_thumb.png"
```

### Comparing `squidpy-1.4.1/docs/_static/css/custom.css` & `squidpy-1.5.0/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/_static/css/dataframe.css` & `squidpy-1.5.0/docs/_static/css/dataframe.css`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/_static/css/nbsphinx.css` & `squidpy-1.5.0/docs/_static/css/nbsphinx.css`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/_static/css/sphinx_gallery.css` & `squidpy-1.5.0/docs/_static/css/sphinx_gallery.css`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/_static/img/figure1.png` & `squidpy-1.5.0/docs/_static/img/figure1.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/_static/img/squidpy_horizontal.png` & `squidpy-1.5.0/docs/_static/img/squidpy_horizontal.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/_static/img/squidpy_vertical.png` & `squidpy-1.5.0/docs/_static/img/squidpy_vertical.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/_templates/autosummary/class.rst` & `squidpy-1.5.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/release/notes-1.0.1.rst` & `squidpy-1.5.0/docs/release/notes-1.0.1.rst`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/release/notes-1.1.0.rst` & `squidpy-1.5.0/docs/release/notes-1.1.0.rst`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/release/notes-1.1.1.rst` & `squidpy-1.5.0/docs/release/notes-1.1.1.rst`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/release/notes-1.2.0.rst` & `squidpy-1.5.0/docs/release/notes-1.2.0.rst`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/release/notes-1.2.1.rst` & `squidpy-1.5.0/docs/release/notes-1.2.1.rst`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/release/notes-1.2.3.rst` & `squidpy-1.5.0/docs/release/notes-1.2.3.rst`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/release/notes-1.3.0.rst` & `squidpy-1.5.0/docs/release/notes-1.3.0.rst`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/docs/release/notes-1.4.0.rst` & `squidpy-1.5.0/docs/release/notes-1.4.0.rst`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/src/squidpy/_docs.py` & `squidpy-1.5.0/src/squidpy/_docs.py`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/src/squidpy/_utils.py` & `squidpy-1.5.0/src/squidpy/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 """Spatial tools general utility functions."""
 
 from __future__ import annotations
 
 import functools
 import inspect
 import warnings
+from collections.abc import Generator, Hashable, Iterable, Sequence
 from contextlib import contextmanager
 from enum import Enum
 from multiprocessing import Manager, cpu_count
 from queue import Queue
 from threading import Thread
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Generator,
-    Hashable,
-    Iterable,
-    Sequence,
-    Union,  # noqa: F401
-)
+from typing import TYPE_CHECKING, Any, Callable
 
 import joblib as jl
 import numpy as np
 
 __all__ = ["singledispatchmethod", "Signal", "SigQueue", "NDArray", "NDArrayA"]
```

### Comparing `squidpy-1.4.1/src/squidpy/_constants/_constants.py` & `squidpy-1.5.0/src/squidpy/_constants/_constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Constants that user deals with."""
 
+from __future__ import annotations
+
 from enum import unique
 
 from squidpy._constants._utils import ModeEnum
 
 
 @unique
 class ImageFeature(ModeEnum):
```

### Comparing `squidpy-1.4.1/src/squidpy/_constants/_pkg_constants.py` & `squidpy-1.5.0/src/squidpy/_constants/_pkg_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Internal constants not exposed to the user."""
 
 from __future__ import annotations
 
-from typing import Any, Callable, Mapping, Optional, Sequence, Union
+from collections.abc import Callable, Mapping, Sequence
+from typing import Any
 
 from anndata import AnnData
 
 from squidpy._constants._constants import Processing, SegmentationBackend
 
 _SEP = "_"
```

### Comparing `squidpy-1.4.1/src/squidpy/_constants/_utils.py` & `squidpy-1.5.0/src/squidpy/_constants/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from abc import ABC, ABCMeta
+from collections.abc import Mapping
 from enum import Enum, EnumMeta
 from functools import wraps
-from typing import Any, Callable, Mapping, Tuple
+from typing import Any, Callable
 
 
 def _pretty_raise_enum(cls: type[ModeEnum], fun: Callable[..., Any]) -> Callable[..., Any]:
     @wraps(fun)
     def wrapper(*args: Any, **kwargs: Any) -> Any:
         try:
             return fun(*args, **kwargs)
@@ -29,15 +30,17 @@
     """Mixin class that formats invalid value when constructing an enum."""
 
     __error_format__ = "Invalid option `{0}` for `{1}`. Valid options are: `{2}`."
 
     @classmethod
     def _format(cls, value: Enum) -> str:
         return cls.__error_format__.format(
-            value, cls.__name__, [m.value for m in cls.__members__.values()]  # type: ignore[attr-defined]
+            value,
+            cls.__name__,
+            [m.value for m in cls.__members__.values()],  # type: ignore[attr-defined]
         )
 
 
 class PrettyEnum(Enum):
     """Enum with a pretty __str__ and __repr__."""
 
     def __repr__(self) -> str:
```

### Comparing `squidpy-1.4.1/src/squidpy/datasets/_10x_datasets.py` & `squidpy-1.5.0/src/squidpy/datasets/_10x_datasets.py`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/src/squidpy/datasets/_dataset.py` & `squidpy-1.5.0/src/squidpy/datasets/_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from copy import copy
 
 from squidpy.datasets._utils import AMetadata
 
 _4i = AMetadata(
     name="four_i",
     doc_header="Pre-processed subset 4i dataset from `Gut et al <https://doi.org/10.1126/science.aar7042>`__.",
```

### Comparing `squidpy-1.4.1/src/squidpy/datasets/_image.py` & `squidpy-1.5.0/src/squidpy/datasets/_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from copy import copy
 
 from squidpy.datasets._utils import ImgMetadata
 
 _vfic = ImgMetadata(
     name="visium_fluo_image_crop",
     doc_header="Cropped Fluorescent image from `10x Genomics Visium dataset "
```

### Comparing `squidpy-1.4.1/src/squidpy/datasets/_utils.py` & `squidpy-1.5.0/src/squidpy/datasets/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from __future__ import annotations
+
 import os
 from abc import ABC, abstractmethod
+from collections.abc import Sequence
 from dataclasses import dataclass, field
 from inspect import Parameter, Signature, signature
 from pathlib import Path
-from typing import Any, Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Union
 
 import anndata
 from anndata import AnnData
 from scanpy import logging as logg
 from scanpy import read
 from scanpy._utils import check_presence_download
 
@@ -18,18 +21,18 @@
 @dataclass(frozen=True)
 class Metadata(ABC):
     """Base class handling metadata."""
 
     name: str
     url: str
 
-    doc_header: Optional[str] = field(default=None, repr=False)
-    path: Optional[PathLike] = field(default=None, repr=False)
-    shape: Optional[tuple[int, int]] = field(default=None, repr=False)
-    library_id: Optional[Union[str, Sequence[str]]] = field(default=None, repr=False)
+    doc_header: str | None = field(default=None, repr=False)
+    path: PathLike | None = field(default=None, repr=False)
+    shape: tuple[int, int] | None = field(default=None, repr=False)
+    library_id: str | Sequence[str] | None = field(default=None, repr=False)
 
     _DOC_FMT = ""
 
     def __post_init__(self) -> None:
         if self.doc_header is None:
             object.__setattr__(self, "doc_header", f"Download `{self.name.title().replace('_', ' ')}` data.")
         if self.path is None:
@@ -62,15 +65,15 @@
             f"    {self._DOC_FMT.format(doc_header=self.doc_header, shape=self.shape)}"
             f'    """\n'
             f"    return {name}.download(path, **kwargs)".replace(" /,", ""),
             globals(),
             glob_ns,
         )
 
-    def download(self, fpath: Optional[PathLike] = None, **kwargs: Any) -> Any:
+    def download(self, fpath: PathLike | None = None, **kwargs: Any) -> Any:
         """Download the dataset into ``fpath``."""
         fpath = str(self.path if fpath is None else fpath)
         if not fpath.endswith(self._extension):
             fpath += self._extension
 
         if os.path.isfile(fpath):
             logg.debug(f"Loading dataset `{self.name}` from `{fpath}`")
```

### Comparing `squidpy-1.4.1/src/squidpy/gr/_build.py` & `squidpy-1.5.0/src/squidpy/gr/_build.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Functions for building graphs from spatial coordinates."""
 
 from __future__ import annotations
 
 import warnings
+from collections.abc import Iterable  # noqa: F401
 from functools import partial
 from itertools import chain
-from typing import Iterable, List, Tuple, Union  # noqa: F401
 
 import numpy as np
 from anndata import AnnData
 from anndata.utils import make_index_unique
 from numba import njit
 from scanpy import logging as logg
 from scipy.sparse import (
```

### Comparing `squidpy-1.4.1/src/squidpy/gr/_ligrec.py` & `squidpy-1.5.0/src/squidpy/gr/_ligrec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Permutation test function as described in CellPhoneDB 2.0."""
 
 from __future__ import annotations
 
 from abc import ABC
 from collections import namedtuple
+from collections.abc import Iterable, Mapping, Sequence
 from functools import partial
 from itertools import product
 from types import MappingProxyType
-from typing import TYPE_CHECKING, Any, Iterable, Literal, Mapping, Sequence, Union
+from typing import TYPE_CHECKING, Any, Literal, Union
 
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from numba import njit, prange  # noqa: F401
 from scanpy import logging as logg
 from scipy.sparse import csc_matrix
@@ -726,15 +727,15 @@
             assert isinstance(means, np.ndarray)
 
         pvalues = np.sum([r.pvalues for r in res if r.pvalues is not None], axis=0) / float(n_perms)
         assert means.shape == pvalues.shape, f"Means and p-values differ in shape: `{means.shape}`, `{pvalues.shape}`."
 
         return TempResult(means=means, pvalues=pvalues)
 
-    groups = data.groupby("clusters")
+    groups = data.groupby("clusters", observed=True)
     clustering = np.array(data["clusters"].values, dtype=np.int32)
 
     mean = groups.mean().values.T  # (n_genes, n_clusters)
     mask = groups.apply(lambda c: ((c > 0).sum() / len(c)) >= threshold).values.T  # (n_genes, n_clusters)
     # (n_cells, n_genes)
     data = np.array(data[data.columns.difference(["clusters"])].values, dtype=np.float64, order="C")
     # all 3 should be C contiguous
@@ -818,15 +819,16 @@
     numba_parallel = (
         (np.prod(res.shape) >= 2**20 or clustering.shape[0] >= 2**15) if numba_parallel is None else numba_parallel  # type: ignore[assignment]
     )
 
     fn_key = f"_test_{n_cls}_{int(return_means)}_{bool(numba_parallel)}"
     if fn_key not in globals():
         exec(
-            compile(_create_template(n_cls, return_means=return_means, parallel=numba_parallel), "", "exec"), globals()  # type: ignore[arg-type]
+            compile(_create_template(n_cls, return_means=return_means, parallel=numba_parallel), "", "exec"),  # type: ignore[arg-type]
+            globals(),
         )
     _test = globals()[fn_key]
 
     if return_means:
         res_means: NDArrayA | None = np.zeros((len(interactions), len(interaction_clusters)), dtype=np.float64)
         test = partial(_test, res_means=res_means)
     else:
```

### Comparing `squidpy-1.4.1/src/squidpy/gr/_nhood.py` & `squidpy-1.5.0/src/squidpy/gr/_nhood.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 """Functions for neighborhood enrichment analysis (permutation test, centralities measures etc.)."""
 
 from __future__ import annotations
 
+from collections.abc import Iterable, Sequence
 from functools import partial
-from typing import (
-    Any,
-    Callable,
-    Iterable,
-    Sequence,
-    Union,  # noqa: F401
-)
+from typing import Any, Callable
 
 import networkx as nx
 import numba.types as nt
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from numba import njit, prange  # noqa: F401
```

### Comparing `squidpy-1.4.1/src/squidpy/gr/_ppatterns.py` & `squidpy-1.5.0/src/squidpy/gr/_ppatterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 """Functions for point patterns spatial statistics."""
 
 from __future__ import annotations
 
+from collections.abc import Iterable, Sequence
 from itertools import chain
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Dict,
-    Iterable,
-    Literal,  # < 3.8
-    Sequence,
-    Union,  # noqa: F401
-)
+from typing import TYPE_CHECKING, Any, Literal
 
 import numba.types as nt
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from numba import njit
 from numpy.random import default_rng
@@ -47,14 +40,15 @@
 
 
 it = nt.int32
 ft = nt.float32
 tt = nt.UniTuple
 ip = np.int32
 fp = np.float32
+bl = nt.boolean
 
 
 @d.dedent
 @inject_docs(key=Key.obsp.spatial_conn(), sp=SpatialAutocorr)
 def spatial_autocorr(
     adata: AnnData | SpatialData,
     connectivity_key: str = Key.obsp.spatial_conn(),
@@ -267,47 +261,63 @@
     if queue is not None:
         queue.put(Signal.FINISH)
 
     return score_perms
 
 
 @njit(
-    ft[:, :, :](tt(it[:], 2), ft[:, :], it[:], ft[:]),
+    ft[:, :, :](tt(it[:], 2), ft[:, :], it[:], ft[:], bl),
     parallel=False,
     fastmath=True,
 )
 def _occur_count(
     clust: tuple[NDArrayA, NDArrayA],
     pw_dist: NDArrayA,
     labs_unique: NDArrayA,
     interval: NDArrayA,
+    same_split: bool,
 ) -> NDArrayA:
     num = labs_unique.shape[0]
     out = np.zeros((num, num, interval.shape[0] - 1), dtype=ft)
 
     for idx in range(interval.shape[0] - 1):
         co_occur = np.zeros((num, num), dtype=ft)
         probs_con = np.zeros((num, num), dtype=ft)
 
-        thres_min = interval[idx]
         thres_max = interval[idx + 1]
         clust_x, clust_y = clust
 
-        idx_x, idx_y = np.nonzero((pw_dist <= thres_max) & (pw_dist > thres_min))
+        # Modified to compute co-occurrence probability ratio over increasing radii sizes as opposed to discrete interval bins
+        # Need pw_dist > 0 to avoid counting a cell with itself as co-occurrence
+        idx_x, idx_y = np.nonzero((pw_dist <= thres_max) & (pw_dist > 0))
         x = clust_x[idx_x]
         y = clust_y[idx_y]
+        # Treat computing co-occurrence using the same split and different splits differently
+        # Pairwise distance matrix for between the same split is symmetric and therefore only needs to be counted once
         for i, j in zip(x, y):
-            co_occur[i, j] += 1
+            if same_split:
+                co_occur[i, j] += 1
+            else:
+                co_occur[i, j] += 1
+                co_occur[j, i] += 1
 
-        probs_matrix = co_occur / np.sum(co_occur)
-        probs = np.sum(probs_matrix, axis=1)
+        # Prevent divison by zero errors when we have low cell counts/small intervals
+        probs_matrix = co_occur / np.sum(co_occur) if np.sum(co_occur) != 0 else np.zeros((num, num), dtype=ft)
+        probs = np.sum(probs_matrix, axis=0)
 
         for c in labs_unique:
-            probs_conditional = co_occur[c] / np.sum(co_occur[c])
-            probs_con[c, :] = probs_conditional / probs
+            probs_conditional = (
+                co_occur[c] / np.sum(co_occur[c]) if np.sum(co_occur[c]) != 0 else np.zeros(num, dtype=ft)
+            )
+            probs_con[c, :] = np.zeros(num, dtype=ft)
+            for i in range(num):
+                if probs[i] == 0:
+                    probs_con[c, i] = 0
+                else:
+                    probs_con[c, i] = probs_conditional[i] / probs[i]
 
         out[:, :, idx] = probs_con
 
     return out
 
 
 def _co_occurrence_helper(
@@ -321,15 +331,15 @@
     out_lst = []
     for t in idx_splits:
         idx_x, idx_y = t
         labs_x = labs_splits[idx_x]
         labs_y = labs_splits[idx_y]
         dist = pairwise_distances(spatial_splits[idx_x], spatial_splits[idx_y])
 
-        out = _occur_count((labs_x, labs_y), dist, labs_unique, interval)
+        out = _occur_count((labs_x, labs_y), dist, labs_unique, interval, idx_x == idx_y)
         out_lst.append(out)
 
         if queue is not None:
             queue.put(Signal.UPDATE)
 
     if queue is not None:
         queue.put(Signal.FINISH)
```

### Comparing `squidpy-1.4.1/src/squidpy/gr/_ripley.py` & `squidpy-1.5.0/src/squidpy/gr/_ripley.py`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/src/squidpy/gr/_sepal.py` & `squidpy-1.5.0/src/squidpy/gr/_sepal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from __future__ import annotations
 
-from typing import (
-    Callable,
-    Literal,  # < 3.8
-    Sequence,
-    Union,  # noqa: F401
-)
+from collections.abc import Sequence
+from typing import Callable, Literal
 
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from numba import njit
 from scanpy import logging as logg
 from scipy.sparse import csr_matrix, issparse, isspmatrix_csr, spmatrix
```

### Comparing `squidpy-1.4.1/src/squidpy/gr/_utils.py` & `squidpy-1.5.0/src/squidpy/gr/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 """Graph utilities."""
 
 from __future__ import annotations
 
+from collections.abc import Hashable, Iterable, Sequence
 from contextlib import contextmanager
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Hashable,
-    Iterable,
-    Sequence,
-    Union,  # noqa: F401
-)
+from typing import TYPE_CHECKING, Any
 
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from anndata._core.views import ArrayView, SparseCSCView, SparseCSRView
 from anndata.utils import make_index_unique
 from pandas import CategoricalDtype
-from pandas.api.types import infer_dtype, is_categorical_dtype
+from pandas.api.types import infer_dtype
 from scanpy import logging as logg
 from scipy.sparse import csc_matrix, csr_matrix, issparse, spmatrix
 
 from squidpy._docs import d
 from squidpy._utils import NDArrayA, _unique_order_preserving
```

### Comparing `squidpy-1.4.1/src/squidpy/im/_container.py` & `squidpy-1.5.0/src/squidpy/im/_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,17 @@
 from __future__ import annotations
 
 import re
+from collections.abc import Iterable, Iterator, Mapping, Sequence
 from copy import copy, deepcopy
 from functools import partial
 from itertools import chain
 from pathlib import Path
 from types import MappingProxyType
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Iterable,
-    Iterator,
-    Literal,
-    Mapping,
-    Sequence,
-    TypeVar,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, Callable, Literal, TypeVar, Union
 
 import dask.array as da
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import validators
 import xarray as xr
@@ -147,15 +137,15 @@
         ------
         ValueError
             If any of the ``imgs`` have more than 1 Z-dimension or if ``library_ids`` are not unique.
         """
         # check that imgs are not already 3d
         imgs = list(imgs)
         for img in imgs:
-            if img.data.dims["z"] > 1:
+            if img.data.sizes["z"] > 1:
                 raise ValueError(
                     f"Currently, can concatenate only images with 1 Z-dimension, found `{img.data.dims['z']}`."
                 )
 
         # check library_ids
         if library_ids is None:
             library_ids = [None] * len(imgs)
@@ -601,18 +591,18 @@
         if scale != 1:
             attrs = data.attrs
             library_ids = data.coords["z"]
             data = data.map(_rescale).assign_coords({"z": library_ids})
             data.attrs = _update_attrs_scale(attrs, scale)
 
         if mask_circle:
-            if data.dims["y"] != data.dims["x"]:
+            if data.sizes["y"] != data.sizes["x"]:
                 raise ValueError(
                     f"Masking circle is only available for square crops, "
-                    f"found crop of shape `{(data.dims['y'], data.dims['x'])}`."
+                    f"found crop of shape `{(data.sizes['y'], data.sizes['x'])}`."
                 )
             c = data.x.shape[0] // 2
             # manually reassign coordinates
             library_ids = data.coords["z"]
             data = data.where((data.x - c) ** 2 + (data.y - c) ** 2 <= c**2, other=cval).assign_coords(
                 {"z": library_ids}
             )
@@ -785,15 +775,15 @@
                         str(e)
                         + " Or specify a key in `adata.obs` containing a mapping from observations to library ids."
                     ) from e
                 else:
                     raise e
         else:
             try:
-                obs_library_ids = adata.obs[library_id]
+                obs_library_ids = list(adata.obs[library_id])
             except KeyError:
                 logg.debug(
                     f"Unable to find library ids in `adata.obs[{library_id!r}]`. "
                     f"Trying in `adata.uns[{spatial_key!r}]`"
                 )
                 library_id = Key.uns.library_id(adata, spatial_key=spatial_key, library_id=library_id)
                 if not isinstance(library_id, str):
@@ -1364,15 +1354,15 @@
         return self._data
 
     @property
     def shape(self) -> tuple[int, int]:
         """Image shape ``(y, x)``."""
         if not len(self):
             return 0, 0
-        return self.data.dims["y"], self.data.dims["x"]
+        return self.data.sizes["y"], self.data.sizes["x"]
 
     def copy(self, deep: bool = False) -> ImageContainer:
         """
         Return a copy of self.
 
         Parameters
         ----------
@@ -1592,16 +1582,15 @@
         inflection = "" if len(self) <= 1 else "s"
         s = f"{self.__class__.__name__} object with {len(self.data.keys())} layer{inflection}:"
         style = "text-indent: 25px; margin-top: 0px; margin-bottom: 0px;"
 
         for i, layer in enumerate(self.data.keys()):
             s += f"<p style={style!r}><strong>{html.escape(str(layer))}</strong>: "
             s += ", ".join(
-                f"<em>{html.escape(str(dim))}</em> ({shape})"
-                for dim, shape in zip(self.data[layer].dims, self.data[layer].shape)
+                f"<em>{html.escape(str(dim))}</em> ({shape})" for dim, shape in self.data[layer].sizes.items()
             )
             s += "</p>"
             if i == 9 and i < len(self) - 1:  # show only first 10 layers
                 s += f"<p style={style!r}>and {len(self) - i  - 1} more...</p>"
                 break
 
         return s
```

### Comparing `squidpy-1.4.1/src/squidpy/im/_coords.py` & `squidpy-1.5.0/src/squidpy/im/_coords.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from collections.abc import Hashable
 from dataclasses import dataclass
-from typing import (
-    Any,
-    Hashable,
-    Union,  # noqa: F401
-)
+from typing import Any
 
 import numpy as np
 
 from squidpy._constants._pkg_constants import Key
 from squidpy._utils import NDArrayA
 from squidpy.gr._utils import _assert_non_negative
```

### Comparing `squidpy-1.4.1/src/squidpy/im/_feature.py` & `squidpy-1.5.0/src/squidpy/im/_feature.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from __future__ import annotations
 
+from collections.abc import Mapping, Sequence
 from types import MappingProxyType
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Mapping,
-    Sequence,
-    Union,  # noqa: F401
-)
+from typing import TYPE_CHECKING, Any
 
 import pandas as pd
 from anndata import AnnData
 from scanpy import logging as logg
 
 from squidpy._constants._constants import ImageFeature
 from squidpy._docs import d, inject_docs
```

### Comparing `squidpy-1.4.1/src/squidpy/im/_feature_mixin.py` & `squidpy-1.5.0/src/squidpy/im/_feature_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,11 @@
 from __future__ import annotations
 
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Dict,
-    Iterable,
-    Protocol,
-    Sequence,
-    Union,
-)
+from collections.abc import Iterable, Sequence
+from typing import TYPE_CHECKING, Any, Callable, Protocol, Union
 
 import numpy as np
 import skimage.measure
 import xarray as xr
 from skimage.feature import graycomatrix, graycoprops
 from skimage.util import img_as_ubyte
 
@@ -326,26 +318,26 @@
         """
 
         def convert_to_full_image_coordinates(x: NDArrayA, y: NDArrayA) -> NDArrayA:
             if not len(y):
                 return np.array([[]], dtype=np.float64)
 
             if self.data.attrs.get("mask_circle", False):
-                if self.data.dims["y"] != self.data.dims["x"]:
-                    raise ValueError(f"Crop is not a square: `{self.data.dims}`.")
-                c = self.data.dims["x"] // 2  # center
+                if self.data.sizes["y"] != self.data.sizes["x"]:
+                    raise ValueError(f"Crop is not a square: `{self.data.sizes}`.")
+                c = self.data.sizes["x"] // 2  # center
                 mask = (x - c) ** 2 + (y - c) ** 2 <= c**2
                 y = y[mask]
                 x = x[mask]
 
             if not len(y):
                 return np.array([[]], dtype=np.float64)  # because of masking, should not happen
 
             coord = self.data.attrs.get(
-                Key.img.coords, CropCoords(x0=0, y0=0, x1=self.data.dims["x"], y1=self.data.dims["y"])
+                Key.img.coords, CropCoords(x0=0, y0=0, x1=self.data.sizes["x"], y1=self.data.sizes["y"])
             )  # fall back to default (i.e no crop) coordinates
             padding = self.data.attrs.get(Key.img.padding, _NULL_PADDING)  # fallback to no padding
             y_slc, x_slc = coord.to_image_coordinates(padding).slice
 
             # relative coordinates
             y = (y - np.min(y)) / (np.max(y) - np.min(y))
             x = (x - np.min(x)) / (np.max(x) - np.min(x))
```

### Comparing `squidpy-1.4.1/src/squidpy/im/_io.py` & `squidpy-1.5.0/src/squidpy/im/_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from __future__ import annotations
 
+from collections.abc import Mapping
 from pathlib import Path
-from typing import (
-    Mapping,
-    Union,  # noqa: F401
-)
 
 import dask.array as da
 import numpy as np
 import xarray as xr
 from dask import delayed
 from PIL import Image
 from scanpy import logging as logg
```

### Comparing `squidpy-1.4.1/src/squidpy/im/_process.py` & `squidpy-1.5.0/src/squidpy/im/_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from __future__ import annotations
 
+from collections.abc import Mapping, Sequence
 from types import MappingProxyType
-from typing import (
-    Any,
-    Callable,
-    Mapping,
-    Sequence,
-    Union,  # noqa: F401
-)
+from typing import Any, Callable
 
 import dask.array as da
 from dask_image.ndfilters import gaussian_filter as dask_gf
 from scanpy import logging as logg
 from scipy.ndimage import gaussian_filter as scipy_gf
 
 from squidpy._constants._constants import Processing
```

### Comparing `squidpy-1.4.1/src/squidpy/im/_segment.py` & `squidpy-1.5.0/src/squidpy/im/_segment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from collections.abc import Mapping, Sequence
 from types import MappingProxyType
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Mapping,
-    Sequence,
-    Union,  # noqa: F401
-)
+from typing import TYPE_CHECKING, Any, Callable
 
 import dask.array as da
 import numpy as np
 from scanpy import logging as logg
 from scipy import ndimage as ndi
 from skimage.feature import peak_local_max
 from skimage.filters import threshold_otsu
```

### Comparing `squidpy-1.4.1/src/squidpy/pl/_color_utils.py` & `squidpy-1.5.0/src/squidpy/pl/_color_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Utils for plotting functions."""
 
 from __future__ import annotations
 
-from typing import Any, Mapping, Optional, Sequence, Union
+from collections.abc import Mapping, Sequence
+from typing import Any, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 from anndata import AnnData
 from cycler import Cycler, cycler
 from matplotlib.colors import ListedColormap, to_hex, to_rgba
 from scanpy import logging as logg
@@ -49,15 +50,15 @@
             return {cat: to_hex(to_rgba(col)[:3] + (alpha,), keep_alpha=True) for cat, col in zip(categories, palette)}
         except KeyError as e:
             logg.error(f"Unable to fetch palette, reason: {e}. Using `None`.")
             return None
 
     len_cat = len(categories)
     if isinstance(palette, str):
-        cmap = plt.get_cmap(palette)
+        cmap = plt.colormaps[palette]
         palette = [to_hex(x, keep_alpha=True) for x in cmap(np.linspace(0, 1, len_cat), alpha=alpha)]
     elif isinstance(palette, ListedColormap):
         palette = [to_hex(x, keep_alpha=True) for x in palette(np.linspace(0, 1, len_cat), alpha=alpha)]
     else:
         raise TypeError(f"Palette is {type(palette)} but should be string or `ListedColormap`.")
 
     return dict(zip(categories, palette))
```

### Comparing `squidpy-1.4.1/src/squidpy/pl/_graph.py` & `squidpy-1.5.0/src/squidpy/pl/_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 """Plotting for graph functions."""
 
 from __future__ import annotations
 
+from collections.abc import Mapping, Sequence
 from pathlib import Path
 from types import MappingProxyType
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Literal,
-    Mapping,
-    Sequence,
-    Union,  # noqa: F401
-)
+from typing import TYPE_CHECKING, Any, Literal
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from anndata import AnnData
 from matplotlib.axes import Axes
@@ -155,15 +149,15 @@
     Returns
     -------
     %(plotting_returns)s
     """
     _assert_categorical_obs(adata, key=cluster_key)
     array = _get_data(adata, cluster_key=cluster_key, func_name="interaction_matrix")
 
-    ad = AnnData(X=array, obs={cluster_key: pd.Categorical(adata.obs[cluster_key].cat.categories)}, dtype=array.dtype)
+    ad = AnnData(X=array, obs={cluster_key: pd.Categorical(adata.obs[cluster_key].cat.categories)})
     _maybe_set_colors(source=adata, target=ad, key=cluster_key, palette=palette)
     if title is None:
         title = "Interaction matrix"
     fig = _heatmap(
         ad,
         key=cluster_key,
         title=title,
@@ -220,15 +214,15 @@
     Returns
     -------
     %(plotting_returns)s
     """
     _assert_categorical_obs(adata, key=cluster_key)
     array = _get_data(adata, cluster_key=cluster_key, func_name="nhood_enrichment")[mode]
 
-    ad = AnnData(X=array, obs={cluster_key: pd.Categorical(adata.obs[cluster_key].cat.categories)}, dtype=array.dtype)
+    ad = AnnData(X=array, obs={cluster_key: pd.Categorical(adata.obs[cluster_key].cat.categories)})
     _maybe_set_colors(source=adata, target=ad, key=cluster_key, palette=palette)
     if title is None:
         title = "Neighborhood enrichment"
     fig = _heatmap(
         ad,
         key=cluster_key,
         title=title,
@@ -311,15 +305,15 @@
         data=res[f"{mode.s}_stat"],
         hue_order=categories,
         palette=palette,
         ax=ax,
         **kwargs,
     )
     if plot_sims:
-        sns.lineplot(y="stats", x="bins", ci="sd", alpha=0.01, color="gray", data=res["sims_stat"], ax=ax)
+        sns.lineplot(y="stats", x="bins", errorbar="sd", alpha=0.01, color="gray", data=res["sims_stat"], ax=ax)
     ax.legend(**legend_kwargs)
     ax.set_ylabel("value")
     ax.set_title(f"Ripley's {mode.s}")
 
     if save is not None:
         save_fig(fig, path=save)
```

### Comparing `squidpy-1.4.1/src/squidpy/pl/_ligrec.py` & `squidpy-1.5.0/src/squidpy/pl/_ligrec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from __future__ import annotations
 
+from collections.abc import Mapping, Sequence
 from pathlib import Path
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Mapping,
-    Sequence,
-    Union,  # noqa: F401
-)
+from typing import TYPE_CHECKING, Any
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scanpy as sc
 from anndata import AnnData
 from matplotlib.axes import Axes
@@ -103,15 +98,15 @@
             ax.set_title(f"significant\n$p={self._alpha}$", y=ymax + 0.25, size="small")
             ax.set(frame_on=False)
 
             l, b, w, h = size_legend_ax.get_position().bounds
             ax.set_position([l + w, b, w, h])
 
     def _plot_colorbar(self, color_legend_ax: Axes, normalize: bool) -> None:
-        cmap = plt.get_cmap(self.cmap)
+        cmap = plt.colormaps[self.cmap]
 
         ColorbarBase(
             color_legend_ax,
             orientation="horizontal",
             cmap=cmap,
             norm=normalize,
             ticks=np.linspace(
@@ -299,15 +294,15 @@
     start, label_ranges = 0, {}
 
     if dendrogram == DendrogramAxis.INTERACTING_CLUSTERS:
         # rows are now cluster combinations, not interacting pairs
         pvals = pvals.T
         means = means.T
 
-    for cls, size in (pvals.groupby(level=0, axis=1)).size().to_dict().items():
+    for cls, size in (pvals.T.groupby(level=0)).size().to_dict().items():
         label_ranges[cls] = (start, start + size - 1)
         start += size
     label_ranges = {k: label_ranges[k] for k in sorted(label_ranges.keys())}
 
     pvals = pvals[label_ranges.keys()]
     pvals = -np.log10(pvals + min(1e-3, alpha if alpha is not None else 1e-3)).fillna(0)
 
@@ -318,15 +313,15 @@
     means.columns = map(_SEP.join, means.columns.to_flat_index())
     means.index = map(_SEP.join, means.index.to_flat_index())
     means = np.log2(means + 1)
 
     var = pd.DataFrame(pvals.columns)
     var = var.set_index(var.columns[0])
 
-    adata = AnnData(pvals.values, obs={"groups": pd.Categorical(pvals.index)}, var=var, dtype=pvals.values.dtype)
+    adata = AnnData(pvals.values, obs={"groups": pd.Categorical(pvals.index)}, var=var)
     adata.obs_names = pvals.index
     minn = np.nanmin(adata.X)
     delta = np.nanmax(adata.X) - minn
     adata.X = (adata.X - minn) / delta
 
     try:
         if dendrogram == DendrogramAxis.BOTH:
```

### Comparing `squidpy-1.4.1/src/squidpy/pl/_spatial.py` & `squidpy-1.5.0/src/squidpy/pl/_spatial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import itertools
+from collections.abc import Mapping, Sequence
 from pathlib import Path
 from types import MappingProxyType
-from typing import Any, Callable, List, Mapping, Optional, Sequence, Tuple, Union
+from typing import Any, Callable
 
 from anndata import AnnData
 from matplotlib.axes import Axes
 from matplotlib.colors import Colormap
 from matplotlib.figure import Figure
 
 from squidpy._constants._constants import ScatterShape
```

### Comparing `squidpy-1.4.1/src/squidpy/pl/_spatial_utils.py` & `squidpy-1.5.0/src/squidpy/pl/_spatial_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,50 +1,37 @@
 from __future__ import annotations
 
 import itertools
+from collections.abc import Mapping, Sequence
 from copy import copy
 from functools import partial
 from numbers import Number
 from types import MappingProxyType
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    List,
-    Literal,
-    Mapping,
-    NamedTuple,
-    Optional,
-    Sequence,
-    Tuple,
-    Type,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, Literal, NamedTuple, Optional, Union
 
 import dask.array as da
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from matplotlib import colors, patheffects, rcParams
 from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
-from matplotlib.cm import get_cmap
 from matplotlib.collections import Collection, PatchCollection
 from matplotlib.colors import (
     ColorConverter,
     Colormap,
     ListedColormap,
     Normalize,
     TwoSlopeNorm,
 )
 from matplotlib.figure import Figure
 from matplotlib.gridspec import GridSpec
 from matplotlib.patches import Circle, Polygon, Rectangle
 from matplotlib_scalebar.scalebar import ScaleBar
 from pandas import CategoricalDtype
-from pandas.core.dtypes.common import is_categorical_dtype
 from scanpy import logging as logg
 from scanpy._settings import settings as sc_settings
 from scanpy.plotting._tools.scatterplots import _add_categorical_legend
 from skimage.color import label2rgb
 from skimage.morphology import erosion, square
 from skimage.segmentation import find_boundaries
 from skimage.util import map_array
@@ -58,15 +45,15 @@
 
 _AvailShapes = Literal["circle", "square", "hex"]
 Palette_t = Optional[Union[str, ListedColormap]]
 _Normalize = Union[Normalize, Sequence[Normalize]]
 _SeqStr = Union[str, Sequence[str]]
 _SeqFloat = Union[float, Sequence[float]]
 _SeqArray = Union[NDArrayA, Sequence[NDArrayA]]
-_CoordTuple = Tuple[int, int, int, int]
+_CoordTuple = tuple[int, int, int, int]
 _FontWeight = Literal["light", "normal", "medium", "semibold", "bold", "heavy", "black"]
 _FontSize = Literal["xx-small", "x-small", "small", "medium", "large", "x-large", "xx-large"]
 
 
 # named tuples
 class FigParams(NamedTuple):
     """Figure params."""
@@ -381,15 +368,15 @@
         adata: AnnData,
         coords: NDArrayA,
         key: str | None,
         values: Sequence[Any] | None,
     ) -> tuple[AnnData, NDArrayA]:
         if key is None or values is None:
             return adata, coords
-        if key not in adata.obs or not is_categorical_dtype(adata.obs[key]):
+        if key not in adata.obs or not isinstance(adata.obs[key].dtype, CategoricalDtype):
             return adata, coords
         try:
             mask = adata.obs[key].isin(values).values
             msg = f"None of `adata.obs[{key}]` are in `{values}`"
             return assert_notempty(adata[mask], msg=msg), coords[mask]
         except KeyError:
             raise KeyError(f"Unable to find `{key!r}` in `adata.obs`.") from None
@@ -464,27 +451,27 @@
     if alt_var is not None and value_to_plot not in adata.obs and value_to_plot not in adata.var_names:
         value_to_plot = adata.var_names[adata.var[alt_var] == value_to_plot][0]
     if use_raw and value_to_plot not in adata.obs:
         color_source_vector = adata.raw.obs_vector(value_to_plot)
     else:
         color_source_vector = adata.obs_vector(value_to_plot, layer=layer)
 
-    if not is_categorical_dtype(color_source_vector):
+    if not isinstance(color_source_vector.dtype, CategoricalDtype):
         return None, color_source_vector, False
 
     color_source_vector = pd.Categorical(color_source_vector)  # convert, e.g., `pd.Series`
     categories = color_source_vector.categories
     if groups is not None:
         color_source_vector = color_source_vector.remove_categories(categories.difference(groups))
 
     color_map = _get_palette(adata, cluster_key=value_to_plot, categories=categories, palette=palette, alpha=alpha)
     if color_map is None:
         raise ValueError("Unable to create color palette.")
     # do not rename categories, as colors need not be unique
-    color_vector = color_source_vector.map(color_map)
+    color_vector = color_source_vector.map(color_map, na_action=None)
     if color_vector.isna().any():
         color_vector = color_vector.add_categories([to_hex(na_color)])
         color_vector = color_vector.fillna(to_hex(na_color))
 
     return color_source_vector, color_vector, True
 
 
@@ -609,15 +596,15 @@
     ax: Axes,
     cax: PatchCollection,
     lib_count: int,
     fig_params: FigParams,
     adata: AnnData,
     coords: NDArrayA,
     value_to_plot: str,
-    color_source_vector: pd.Series[CategoricalDtype],
+    color_source_vector: pd.Series[CategoricalDtype] | None,
     img: NDArrayA | None = None,
     img_cmap: str | None = None,
     img_alpha: float | None = None,
     palette: Palette_t = None,
     alpha: float = 1.0,
     legend_fontsize: int | float | _FontSize | None = None,
     legend_fontweight: int | _FontWeight = "bold",
@@ -642,15 +629,15 @@
 
         if legend_fontoutline is not None:
             path_effect = [patheffects.withStroke(linewidth=legend_fontoutline, foreground="w")]
         else:
             path_effect = []
 
         # Adding legends
-        if is_categorical_dtype(color_source_vector):
+        if color_source_vector is not None and isinstance(color_source_vector.dtype, CategoricalDtype):
             clusters = color_source_vector.categories
             palette = _get_palette(adata, cluster_key=value_to_plot, categories=clusters, palette=palette, alpha=alpha)
             _add_categorical_legend(
                 ax,
                 color_source_vector,
                 palette=palette,
                 scatter_array=coords,
@@ -687,15 +674,15 @@
     cmap_params: CmapParams,
     seg_erosionpx: int | None = None,
     seg_boundaries: bool = False,
     na_color: str | tuple[float, ...] = (0, 0, 0, 0),
 ) -> NDArrayA:
     cell_id = np.array(cell_id)
 
-    if is_categorical_dtype(color_vector):
+    if isinstance(color_vector.dtype, CategoricalDtype):
         if isinstance(na_color, tuple) and len(na_color) == 4 and np.any(color_source_vector.isna()):
             cell_id[color_source_vector.isna()] = 0
         val_im: NDArrayA = map_array(seg, cell_id, color_vector.codes + 1)  # type: ignore[union-attr]
         cols = colors.to_rgba_array(color_vector.categories)  # type: ignore[union-attr]
     else:
         val_im = map_array(seg, cell_id, cell_id)  # replace with same seg id to remove missing segs
         try:
@@ -818,15 +805,18 @@
         axs = ax
     else:
         axs = None
         if ax is None:
             fig, ax = plt.subplots(figsize=figsize, dpi=dpi, constrained_layout=True)
 
     # set cmap and norm
-    cmap = copy(get_cmap(cmap))
+    if cmap is None:
+        cmap = plt.rcParams["image.cmap"]
+    if isinstance(cmap, str):
+        cmap = plt.colormaps[cmap]
     cmap.set_bad("lightgray" if na_color is None else na_color)
 
     if isinstance(norm, Normalize):
         pass
     elif vcenter is None:
         norm = Normalize(vmin=vmin, vmax=vmax)
     else:
```

### Comparing `squidpy-1.4.1/src/squidpy/pl/_utils.py` & `squidpy-1.5.0/src/squidpy/pl/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 from __future__ import annotations
 
 import os
-from copy import copy
+from collections.abc import Mapping, Sequence
 from functools import wraps
 from inspect import signature
 from pathlib import Path
 from types import MappingProxyType
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    List,
-    Mapping,
-    Optional,
-    Sequence,
-    Tuple,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, Callable, Optional, Union
 
 import matplotlib as mpl
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from dask import array as da
 from dask import delayed
@@ -30,15 +20,14 @@
 from matplotlib.figure import Figure
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from numba import njit, prange
 from pandas import CategoricalDtype
 from pandas._libs.lib import infer_dtype
 from pandas.core.dtypes.common import (
     is_bool_dtype,
-    is_categorical_dtype,
     is_integer_dtype,
     is_numeric_dtype,
     is_object_dtype,
     is_string_dtype,
 )
 from scanpy import logging as logg
 from scanpy import settings
@@ -478,15 +467,15 @@
 
 
 def _annotate_heatmap(
     im: mpl.image.AxesImage, valfmt: str = "{x:.2f}", cmap: mpl.colors.Colormap | str = "viridis", **kwargs: Any
 ) -> None:
     # modified from matplotlib's site
     if isinstance(cmap, str):
-        cmap = plt.get_cmap(cmap)
+        cmap = plt.colormaps[cmap]
 
     data = im.get_array()
     kw = {"ha": "center", "va": "center"}
     kw.update(**kwargs)
 
     if isinstance(valfmt, str):
         valfmt = mpl.ticker.StrMethodFormatter(valfmt)
@@ -550,24 +539,25 @@
 
     if method is not None:
         row_order, col_order, _, col_link = _dendrogram(adata.X, method, optimal_ordering=adata.n_obs <= 1500)
     else:
         row_order = col_order = np.arange(len(adata.uns[Key.uns.colors(key)])).tolist()
 
     row_order = row_order[::-1]
-    row_labels = adata.obs[key][row_order]
+    row_labels = adata.obs[key].iloc[row_order]
     data = adata[row_order, col_order].X
 
     row_cmap, col_cmap, row_norm, col_norm, n_cls = _get_cmap_norm(adata, key, order=(row_order, col_order))
 
     row_sm = mpl.cm.ScalarMappable(cmap=row_cmap, norm=row_norm)
     col_sm = mpl.cm.ScalarMappable(cmap=col_cmap, norm=col_norm)
 
     norm = mpl.colors.Normalize(vmin=kwargs.pop("vmin", np.nanmin(data)), vmax=kwargs.pop("vmax", np.nanmax(data)))
-    cont_cmap = copy(plt.get_cmap(cont_cmap))
+    if isinstance(cont_cmap, str):
+        cont_cmap = plt.colormaps[cont_cmap]
     cont_cmap.set_bad(color="grey")
 
     im = ax.imshow(data[::-1], cmap=cont_cmap, norm=norm)
 
     ax.grid(False)
     ax.tick_params(top=False, bottom=False, labeltop=False, labelbottom=False)
     ax.set_xticks([])
```

### Comparing `squidpy-1.4.1/src/squidpy/pl/_var_by_distance.py` & `squidpy-1.5.0/src/squidpy/pl/_var_by_distance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
+from collections.abc import Mapping, Sequence
 from pathlib import Path
 from types import MappingProxyType
-from typing import Any, List, Mapping, Optional, Sequence, Tuple, Union
+from typing import Any
 
 import matplotlib.cm as cm
 import matplotlib.colors as colors
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 from anndata import AnnData
@@ -63,38 +64,45 @@
     order
         Order of the polynomial fit for :func:`seaborn.regplot`.
     show_scatter
         Whether to show a scatter plot underlying the regression line.
     line_palette
         Categorical color palette used in case a covariate is specified.
     scatter_palette
-        Color palette for the scatter plot underlying the `sns.regplot`
-    %(plotting_save)s
+        Color palette for the scatter plot underlying the :func:`seaborn.regplot`.
+    dpi
+        Dots per inch.
+    figsize
+        Size of the figure in inches.
+    save
+        Whether to save the plot.
     title
         Panel titles.
     axis_label
         Panel axis labels.
+    return_ax
+        Whether to return :class:`matplotlib.axes.Axes` object(s).
     regplot_kwargs
-        Kwargs for `sns.regplot`
+        Kwargs for :func:`seaborn.regplot`.
     scatterplot_kwargs
-        Kwargs for `sns.scatter`
+        Kwargs for :func:`matplotlib.pyplot.scatter`.
 
     Returns
     -------
     %(plotting_returns)s
     """
     dpi = rcParams["figure.dpi"] if dpi is None else dpi
     regplot_kwargs = dict(regplot_kwargs)
-    scatterplot_kwargs = dict(regplot_kwargs)
+    scatterplot_kwargs = dict(scatterplot_kwargs)
 
     df = adata.obsm[design_matrix_key]  # get design matrix
     df[var] = np.array(adata[:, var].X.A) if issparse(adata[:, var].X) else np.array(adata[:, var].X)  # add var column
 
     # if several variables are plotted, make a panel grid
-    if isinstance(var, List):
+    if isinstance(var, list):
         fig, grid = _panel_grid(
             hspace=0.25, wspace=0.75 / rcParams["figure.figsize"][0] + 0.02, ncols=4, num_panels=len(var)
         )
         axs = []
     else:
         var = [var]
```

### Comparing `squidpy-1.4.1/src/squidpy/pl/_interactive/_controller.py` & `squidpy-1.5.0/src/squidpy/pl/_interactive/_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import numpy as np
 import pandas as pd
 import xarray as xr
 from anndata import AnnData
 from napari import Viewer
 from napari.layers import Points, Shapes
 from pandas import CategoricalDtype
-from pandas.core.dtypes.common import is_categorical_dtype
 from PyQt5.QtWidgets import QGridLayout, QLabel, QWidget
 from scanpy import logging as logg
 
 from squidpy._docs import d
 from squidpy._utils import NDArrayA, singledispatchmethod
 from squidpy.im import ImageContainer  # type: ignore[attr-defined]
 from squidpy.pl._interactive._model import ImageModel
```

### Comparing `squidpy-1.4.1/src/squidpy/pl/_interactive/_model.py` & `squidpy-1.5.0/src/squidpy/pl/_interactive/_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
+from collections.abc import Sequence
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Sequence
+from typing import TYPE_CHECKING
 
 import numpy as np
 from anndata import AnnData
 
 from squidpy._constants._constants import Symbol
 from squidpy._constants._pkg_constants import Key
 from squidpy._utils import NDArrayA, _unique_order_preserving
```

### Comparing `squidpy-1.4.1/src/squidpy/pl/_interactive/_utils.py` & `squidpy-1.5.0/src/squidpy/pl/_interactive/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from matplotlib.colors import to_hex, to_rgb
 from numba import njit
 from pandas import CategoricalDtype
 from pandas._libs.lib import infer_dtype
-from pandas.core.dtypes.common import is_categorical_dtype
 from scanpy import logging as logg
 from scanpy.plotting._utils import add_colors_for_categorical_sample_annotation
 from scipy.spatial import KDTree
 
 from squidpy._constants._pkg_constants import Key
 from squidpy._utils import NDArrayA
```

### Comparing `squidpy-1.4.1/src/squidpy/pl/_interactive/_view.py` & `squidpy-1.5.0/src/squidpy/pl/_interactive/_view.py`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/src/squidpy/pl/_interactive/_widgets.py` & `squidpy-1.5.0/src/squidpy/pl/_interactive/_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # type: ignore
 from __future__ import annotations
 
 from abc import abstractmethod
-from typing import Any, Iterable, Tuple
+from collections.abc import Iterable
+from typing import Any
 
 import numpy as np
 import pandas as pd
 from deprecated import deprecated
 from napari.layers import Points
 from PyQt5 import QtCore, QtWidgets
 from PyQt5.QtCore import Qt
```

### Comparing `squidpy-1.4.1/src/squidpy/pl/_interactive/interactive.py` & `squidpy-1.5.0/src/squidpy/pl/_interactive/interactive.py`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/src/squidpy/read/_read.py` & `squidpy-1.5.0/src/squidpy/read/_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,14 @@
     obs.rename_axis(None, inplace=True)
     obs.index = obs.index.astype(str).str.cat(obs[fov_key].values, sep="_")
 
     common_index = obs.index.intersection(counts.index)
 
     adata = AnnData(
         csr_matrix(counts.loc[common_index, :].values),
-        dtype=counts.values.dtype,
         obs=obs.loc[common_index, :],
         uns={Key.uns.spatial: {}},
     )
     adata.var_names = counts.columns
 
     adata.obsm[Key.obsm.spatial] = adata.obs[["CenterX_local_px", "CenterY_local_px"]].values
     adata.obsm["spatial_fov"] = adata.obs[["CenterX_global_px", "CenterY_global_px"]].values
```

### Comparing `squidpy-1.4.1/src/squidpy/read/_utils.py` & `squidpy-1.5.0/src/squidpy/read/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Any, Optional, Tuple
+from typing import Any
 
 import numpy as np
-from anndata import AnnData, read_mtx, read_text
+from anndata import AnnData, read_text
 from h5py import File
 from PIL import Image
-from scanpy import read_10x_h5
+from scanpy import read_10x_h5, read_10x_mtx
 
 from squidpy._constants._pkg_constants import Key
 from squidpy._utils import NDArrayA
 from squidpy.datasets._utils import PathLike
 
 
 def _read_counts(
@@ -44,16 +44,16 @@
         return adata, library_id
 
     if library_id is None:
         raise ValueError("Please explicitly specify library id.")
 
     if count_file.endswith((".csv", ".txt")):
         adata = read_text(path / count_file, **kwargs)
-    elif count_file.endswith(".mtx"):
-        adata = read_mtx(path / count_file, **kwargs)
+    elif count_file.endswith(".mtx.gz"):
+        adata = read_10x_mtx(path, **kwargs)
     else:
         raise NotImplementedError("TODO")
 
     adata.uns[Key.uns.spatial] = {library_id: {"metadata": {}}}  # can overwrite
     return adata, library_id
```

### Comparing `squidpy-1.4.1/src/squidpy/tl/_var_by_distance.py` & `squidpy-1.5.0/src/squidpy/tl/_var_by_distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from functools import reduce
 from itertools import product
-from typing import Any, Dict, List, Tuple, Union  # noqa: F401
+from typing import Any
 
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from scanpy import logging as logg
 from sklearn.metrics import DistanceMetric
 from sklearn.neighbors import KDTree
@@ -51,15 +51,15 @@
         Distance metric, defaults to "euclidean".
     %(spatial_key)s
     %(copy)s
 
     Returns
     -------
     If ``copy = True``, returns the design_matrix with the distances to an anchor point
-    Otherwise, stores design_matrix in .obsm
+    Otherwise, stores design_matrix in `.obsm`.
     """
     start = logg.info(f"Creating {design_matrix_key}")
     # list of columns which will be categorical later on
     categorical_columns = [cluster_key]
     # save initial metadata to adata.uns if copy == False
     if not copy:
         adata.uns[design_matrix_key] = _add_metadata(
@@ -69,15 +69,15 @@
     if isinstance(groups, str) or isinstance(groups, np.ndarray):
         anchor: list[Any] = [groups]
     elif isinstance(groups, list):
         anchor = groups
     else:
         raise TypeError(f"Invalid type for groups: {type(groups)}.")
 
-    # prepare batch key for iteration (Nonetype alone in product will result in neutral element)
+    # prepare batch key for iteration (None alone in product will result in neutral element)
     if library_key is None:
         batch = [None]
     else:
         batch = adata.obs[library_key].unique()
         categorical_columns.append(library_key)
 
     batch_design_matrices = {}
@@ -102,15 +102,15 @@
             anchor_col_id = 1
 
         tree = KDTree(
             anchor_coord, metric=DistanceMetric.get_metric(metric)
         )  # build KDTree of anchor point coordinates
         mindist, _ = tree.query(
             batch_coord
-        )  # calculate closest distance from any observation to an observation within anchor point
+        )  # calculate the closest distance from any observation to an observation within anchor point
 
         if isinstance(anchor_var, np.ndarray):  # adjust anchor column name if it is a numpy array
             anchor_var = "custom_anchor"
             anchor = ["custom_anchor"]
         if nan_ids.size != 0:  # in case there were nan coordinates before building the tree, add them back in
             mindist = np.insert(mindist, nan_ids - np.arange(len(nan_ids)), np.nan)
 
@@ -224,46 +224,45 @@
         df = adata.obs[[cluster_key]].copy()
 
     return df
 
 
 def _get_coordinates(adata: AnnData, anchor: str, annotation: str, spatial_key: str) -> tuple[Any, Any, Any]:
     """Get anchor point coordinates and coordinates of all observations, excluding nan values."""
-    # since amount of distances have to match n_obs, the nan id's are stored an inserted after KDTree construction
+    # since amount of distances have to match n_obs, the nan ids are stored an inserted after KDTree construction
     nan_ids, _ = np.split(np.argwhere(np.isnan(adata.obsm[spatial_key])), 2, axis=1)
 
     if nan_ids.size != 0:
         nan_ids = np.unique(nan_ids)
 
     batch_coord = adata.obsm["spatial"][~np.isnan(adata.obsm["spatial"]).any(axis=1)]
 
     if isinstance(anchor, np.ndarray):
         anchor_coord = anchor[~np.isnan(anchor).any(axis=1)]
-        return (anchor, batch_coord, nan_ids)
+        return anchor_coord, batch_coord, nan_ids
 
-    else:
-        anchor_arr = np.array(adata[adata.obs[annotation] == anchor].obsm["spatial"])
-        anchor_coord = anchor_arr[~np.isnan(anchor_arr).any(axis=1)]
-        return (anchor_coord, batch_coord, nan_ids)
+    anchor_arr = np.array(adata[adata.obs[annotation] == anchor].obsm["spatial"])
+    anchor_coord = anchor_arr[~np.isnan(anchor_arr).any(axis=1)]
+    return anchor_coord, batch_coord, nan_ids
 
 
 def _normalize_distances(
     mapping_design_matrix: dict[tuple[Any | None, Any], pd.DataFrame],
     anchor: str | list[str],
     slides: list[str] | list[None],
     mapping_max_distances: dict[tuple[Any | None, Any], float],
-) -> pd.DataFrame:
+) -> list[pd.DataFrame]:
     """Normalize distances to anchor."""
     if not isinstance(anchor, list):
         anchor = [anchor]
 
     # save raw distances, set 0 distances to NaN and smallest non-zero distance to 0 for scaling
     for (_, anchor_point), design_matrix in mapping_design_matrix.items():  # (slide, anchor_point) , design_matrix
         design_matrix[f"{anchor_point}_raw"] = design_matrix[anchor_point]
-        design_matrix[anchor_point].replace(0, np.nan, inplace=True)
+        design_matrix.replace({anchor_point: 0}, np.nan, inplace=True)
         design_matrix.loc[design_matrix[anchor_point].idxmin(), anchor_point] = 0
 
     # for each anchor point, get the slide with the highest maximum distance
     for a in anchor:
         pairs = list(product(slides, [a]))  # get all (slides, anchor) possibilities for given anchor
         mapping_subset = {
             k: mapping_max_distances[k] for k in pairs if k in mapping_max_distances
```

### Comparing `squidpy-1.4.1/tests/conftest.py` & `squidpy-1.5.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import pickle
 import sys
 import warnings
 from abc import ABC, ABCMeta
+from collections.abc import Callable, Mapping, Sequence
 from functools import wraps
 from itertools import product
 from pathlib import Path
-from typing import Callable, Mapping, Optional, Sequence, Tuple
 
 import anndata as ad
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pytest
@@ -80,17 +80,15 @@
 @pytest.fixture()
 def adata() -> AnnData:
     return _adata.copy()
 
 
 @pytest.fixture()
 def adata_palette() -> AnnData:
-    from matplotlib.cm import get_cmap
-
-    cmap = get_cmap("Set1")
+    cmap = plt.colormaps["Set1"]
 
     adata_palette = _adata.copy()
     adata_palette.uns[f"{C_KEY_PALETTE}_colors"] = cmap(range(adata_palette.obs[C_KEY_PALETTE].unique().shape[0]))
     return adata_palette.copy()
 
 
 @pytest.fixture()
@@ -102,15 +100,15 @@
 
     return adata
 
 
 @pytest.fixture()
 def dummy_adata() -> AnnData:
     r = np.random.RandomState(100)
-    adata = AnnData(r.rand(200, 100), obs={"cluster": r.randint(0, 3, 200)}, dtype=float)
+    adata = AnnData(r.rand(200, 100), obs={"cluster": r.randint(0, 3, 200)})
 
     adata.obsm[Key.obsm.spatial] = np.stack([r.randint(0, 500, 200), r.randint(0, 500, 200)], axis=1)
     sq.gr.spatial_neighbors(adata, spatial_key=Key.obsm.spatial, n_rings=2)
 
     return adata
 
 
@@ -127,36 +125,33 @@
             ]
         )
     )
     return AnnData(
         np.zeros((5, 5)),
         obs={"cat": pd.Categorical.from_codes([0, 0, 0, 1, 1], ("a", "b"))},
         obsp={"spatial_connectivities": graph},
-        dtype=float,
     )
 
 
 @pytest.fixture()
 def adata_ripley() -> AnnData:
-    from matplotlib.cm import get_cmap
-
     adata = _adata[_adata.obs.leiden.isin(["0", "2"])].copy()
-    cmap = get_cmap("Set1")
+    cmap = plt.colormaps["Set1"]
 
     adata.uns[f"{C_KEY_PALETTE}_colors"] = cmap(range(adata.obs[C_KEY_PALETTE].unique().shape[0]))
     return adata
 
 
 @pytest.fixture()
 def adata_squaregrid() -> AnnData:
     rng = np.random.default_rng(42)
     coord = rng.integers(0, 10, size=(400, 2))
     coord = np.unique(coord, axis=0)
     counts = rng.integers(0, 10, size=(coord.shape[0], 10))
-    adata = AnnData(counts, dtype=counts.dtype)
+    adata = AnnData(counts)
     adata.obsm["spatial"] = coord
     sc.pp.scale(adata)
     return adata
 
 
 @pytest.fixture(scope="session")
 def paul15() -> AnnData:
@@ -315,24 +310,24 @@
             [4331, 7609],
             [4124, 8208],
             [3780, 7848],
             [3918, 7609],
             [4400, 7729],
         ]
     )
-    adata = AnnData(X=np.ones((visium_coords.shape[0], 3)), dtype=float)
+    adata = AnnData(X=np.ones((visium_coords.shape[0], 3)))
     adata.obsm[Key.obsm.spatial] = visium_coords
     adata.uns[Key.uns.spatial] = {}
     return adata
 
 
 @pytest.fixture()
 def non_visium_adata():
     non_visium_coords = np.array([[1, 0], [3, 0], [5, 6], [0, 4]])
-    adata = AnnData(X=non_visium_coords, dtype=int)
+    adata = AnnData(X=non_visium_coords)
     adata.obsm[Key.obsm.spatial] = non_visium_coords
     return adata
 
 
 def _decorate(fn: Callable, clsname: str, name: str | None = None) -> Callable:
     @wraps(fn)
     def save_and_compare(self, *args, **kwargs):
```

### Comparing `squidpy-1.4.1/tests/_data/filtered_feature_bc_matrix.h5` & `squidpy-1.5.0/tests/_data/filtered_feature_bc_matrix.h5`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_data/ligrec_no_numba.pickle` & `squidpy-1.5.0/tests/_data/ligrec_no_numba.pickle`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_data/paul15_means.pickle` & `squidpy-1.5.0/tests/_data/paul15_means.pickle`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_data/test_data.h5ad` & `squidpy-1.5.0/tests/_data/test_data.h5ad`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_data/test_img.jpg` & `squidpy-1.5.0/tests/_data/test_img.jpg`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_data/spatial/tissue_hires_image.png` & `squidpy-1.5.0/tests/_data/spatial/tissue_hires_image.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_data/spatial/tissue_lowres_image.png` & `squidpy-1.5.0/tests/_data/spatial/tissue_lowres_image.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_data/spatial/tissue_positions_list.csv` & `squidpy-1.5.0/tests/_data/spatial/tissue_positions_list.csv`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/ContainerShow_axis.png` & `squidpy-1.5.0/tests/_images/ContainerShow_axis.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/ContainerShow_channel.png` & `squidpy-1.5.0/tests/_images/ContainerShow_channel.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/ContainerShow_channelwise.png` & `squidpy-1.5.0/tests/_images/ContainerShow_channelwise.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/ContainerShow_channelwise_segmentation.png` & `squidpy-1.5.0/tests/_images/ContainerShow_channelwise_segmentation.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/ContainerShow_imshow_kwargs.png` & `squidpy-1.5.0/tests/_images/ContainerShow_imshow_kwargs.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/ContainerShow_library_id.png` & `squidpy-1.5.0/tests/_images/ContainerShow_library_id.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/ContainerShow_scale_mask_circle_crop.png` & `squidpy-1.5.0/tests/_images/ContainerShow_scale_mask_circle_crop.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/ContainerShow_segmentation.png` & `squidpy-1.5.0/tests/_images/ContainerShow_segmentation.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/ContainerShow_transpose_channelwise_False_False.png` & `squidpy-1.5.0/tests/_images/ContainerShow_transpose_channelwise_False_False.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/ContainerShow_transpose_channelwise_False_True.png` & `squidpy-1.5.0/tests/_images/ContainerShow_transpose_channelwise_False_True.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/ContainerShow_transpose_channelwise_True_False.png` & `squidpy-1.5.0/tests/_images/ContainerShow_transpose_channelwise_True_False.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/ContainerShow_transpose_channelwise_True_True.png` & `squidpy-1.5.0/tests/_images/ContainerShow_transpose_channelwise_True_True.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Graph_centrality_scores.png` & `squidpy-1.5.0/tests/_images/Graph_centrality_scores.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Graph_centrality_scores_single.png` & `squidpy-1.5.0/tests/_images/Graph_centrality_scores_single.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Graph_co_occurrence.png` & `squidpy-1.5.0/tests/_images/Graph_co_occurrence.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Graph_co_occurrence_palette.png` & `squidpy-1.5.0/tests/_images/Graph_co_occurrence_palette.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Graph_interaction.png` & `squidpy-1.5.0/tests/_images/Graph_interaction.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Graph_interaction_dendro.png` & `squidpy-1.5.0/tests/_images/Graph_interaction_dendro.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Graph_nhood_enrichment.png` & `squidpy-1.5.0/tests/_images/Graph_nhood_enrichment.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Graph_nhood_enrichment_ax.png` & `squidpy-1.5.0/tests/_images/Graph_nhood_enrichment_ax.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Graph_nhood_enrichment_dendro.png` & `squidpy-1.5.0/tests/_images/Graph_nhood_enrichment_dendro.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Graph_ripley_f.png` & `squidpy-1.5.0/tests/_images/Graph_ripley_f.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Graph_ripley_f_nopalette.png` & `squidpy-1.5.0/tests/_images/Graph_ripley_f_nopalette.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Graph_ripley_g.png` & `squidpy-1.5.0/tests/_images/Graph_ripley_g.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Graph_ripley_l.png` & `squidpy-1.5.0/tests/_images/Graph_ripley_l.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Heatmap_cbar_kwargs.png` & `squidpy-1.5.0/tests/_images/Heatmap_cbar_kwargs.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Heatmap_cbar_vmin_vmax.png` & `squidpy-1.5.0/tests/_images/Heatmap_cbar_vmin_vmax.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Ligrec_alpha.png` & `squidpy-1.5.0/tests/_images/Ligrec_alpha.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Ligrec_alpha_none.png` & `squidpy-1.5.0/tests/_images/Ligrec_alpha_none.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Ligrec_cmap.png` & `squidpy-1.5.0/tests/_images/Ligrec_cmap.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Ligrec_dendrogram_both.png` & `squidpy-1.5.0/tests/_images/Ligrec_dendrogram_both.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Ligrec_dendrogram_clusters.png` & `squidpy-1.5.0/tests/_images/Ligrec_dendrogram_clusters.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Ligrec_dendrogram_pairs.png` & `squidpy-1.5.0/tests/_images/Ligrec_dendrogram_pairs.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Ligrec_kwargs.png` & `squidpy-1.5.0/tests/_images/Ligrec_kwargs.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Ligrec_means_range.png` & `squidpy-1.5.0/tests/_images/Ligrec_means_range.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Ligrec_no_remove_empty_interactions.png` & `squidpy-1.5.0/tests/_images/Ligrec_no_remove_empty_interactions.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Ligrec_pvalue_threshold.png` & `squidpy-1.5.0/tests/_images/Ligrec_pvalue_threshold.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Ligrec_remove_empty_interactions.png` & `squidpy-1.5.0/tests/_images/Ligrec_remove_empty_interactions.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Ligrec_remove_nonsig_interactions.png` & `squidpy-1.5.0/tests/_images/Ligrec_remove_nonsig_interactions.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Ligrec_source_clusters.png` & `squidpy-1.5.0/tests/_images/Ligrec_source_clusters.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Ligrec_swap_axes.png` & `squidpy-1.5.0/tests/_images/Ligrec_swap_axes.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Ligrec_swap_axes_dedrogram.png` & `squidpy-1.5.0/tests/_images/Ligrec_swap_axes_dedrogram.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Ligrec_target_clusters.png` & `squidpy-1.5.0/tests/_images/Ligrec_target_clusters.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_add_image.png` & `squidpy-1.5.0/tests/_images/Napari_add_image.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_blending.png` & `squidpy-1.5.0/tests/_images/Napari_blending.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_cat_cmap.png` & `squidpy-1.5.0/tests/_images/Napari_cat_cmap.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_cont_cmap.png` & `squidpy-1.5.0/tests/_images/Napari_cont_cmap.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_corner_case_-200_-200_600_800.png` & `squidpy-1.5.0/tests/_images/Napari_corner_case_-200_-200_600_800.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_corner_case_-200_-200_800_600.png` & `squidpy-1.5.0/tests/_images/Napari_corner_case_-200_-200_800_600.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_corner_case_-200_-200_800_800.png` & `squidpy-1.5.0/tests/_images/Napari_corner_case_-200_-200_800_800.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_corner_case_-200_200_600_800.png` & `squidpy-1.5.0/tests/_images/Napari_corner_case_-200_200_600_800.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_corner_case_-200_200_800_600.png` & `squidpy-1.5.0/tests/_images/Napari_corner_case_-200_200_800_600.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_corner_case_-200_200_800_800.png` & `squidpy-1.5.0/tests/_images/Napari_corner_case_-200_200_800_800.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_corner_case_200_-200_600_800.png` & `squidpy-1.5.0/tests/_images/Napari_corner_case_200_-200_600_800.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_corner_case_200_-200_800_600.png` & `squidpy-1.5.0/tests/_images/Napari_corner_case_200_-200_800_600.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_corner_case_200_-200_800_800.png` & `squidpy-1.5.0/tests/_images/Napari_corner_case_200_-200_800_800.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_corner_case_200_200_600_800.png` & `squidpy-1.5.0/tests/_images/Napari_corner_case_200_200_600_800.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_corner_case_200_200_800_600.png` & `squidpy-1.5.0/tests/_images/Napari_corner_case_200_200_800_600.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_corner_case_200_200_800_800.png` & `squidpy-1.5.0/tests/_images/Napari_corner_case_200_200_800_800.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_crop_center.png` & `squidpy-1.5.0/tests/_images/Napari_crop_center.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_crop_corner.png` & `squidpy-1.5.0/tests/_images/Napari_crop_corner.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_gene_X.png` & `squidpy-1.5.0/tests/_images/Napari_gene_X.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_obs_categorical.png` & `squidpy-1.5.0/tests/_images/Napari_obs_categorical.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_obs_continuous.png` & `squidpy-1.5.0/tests/_images/Napari_obs_continuous.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_scalefactor.png` & `squidpy-1.5.0/tests/_images/Napari_scalefactor.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_simple_canvas.png` & `squidpy-1.5.0/tests/_images/Napari_simple_canvas.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_symbol.png` & `squidpy-1.5.0/tests/_images/Napari_symbol.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/Napari_viewer_canvas.png` & `squidpy-1.5.0/tests/_images/Napari_viewer_canvas.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_palette_listed_cmap.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_palette_listed_cmap.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_axfig.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_axfig.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_categorical_alpha.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_categorical_alpha.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_crop.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_crop.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_crop_graph.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_crop_graph.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_crop_noorigin.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_crop_noorigin.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_group.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_group.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_group_multi.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_group_multi.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_group_outline.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_group_outline.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_image.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_image.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_noimage.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_noimage.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_non_unique_colors.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_non_unique_colors.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_nospatial.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_nospatial.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_novisium.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_novisium.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_scatter_title_single.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_scatter_title_single.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_segment.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_segment.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_segment_crop.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_segment_crop.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/SpatialStatic_spatial_segment_group.png` & `squidpy-1.5.0/tests/_images/SpatialStatic_spatial_segment_group.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/var_by_distance_single_anchor_and_gene.png` & `squidpy-1.5.0/tests/_images/var_by_distance_single_anchor_and_gene.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/var_by_distance_single_anchor_and_gene_two_categories.png` & `squidpy-1.5.0/tests/_images/var_by_distance_single_anchor_and_gene_two_categories.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/var_by_distance_single_anchor_four_genes_two_categories_two_palettes.png` & `squidpy-1.5.0/tests/_images/var_by_distance_single_anchor_four_genes_two_categories_two_palettes.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/_images/var_by_distance_single_anchor_one_gene_two_categories_without_scatter.png` & `squidpy-1.5.0/tests/_images/var_by_distance_single_anchor_one_gene_two_categories_without_scatter.png`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/tests/datasets/test_dataset.py` & `squidpy-1.5.0/tests/datasets/test_dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import warnings
 from http.client import RemoteDisconnected
 from pathlib import Path
 from types import FunctionType
 
 import pytest
 import squidpy as sq
```

### Comparing `squidpy-1.4.1/tests/datasets/test_download_visium_dataset.py` & `squidpy-1.5.0/tests/datasets/test_download_visium_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-""""
+""" "
 Tests to make sure the Visium example datasets load.
 """
 
+from __future__ import annotations
+
 import subprocess
 from pathlib import Path
 
 import pytest
 from anndata.tests.helpers import assert_adata_equal
 from scanpy._settings import settings
 from squidpy.datasets import visium
```

### Comparing `squidpy-1.4.1/tests/graph/test_ligrec.py` & `squidpy-1.5.0/tests/graph/test_ligrec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from __future__ import annotations
+
 import sys
+from collections.abc import Mapping, Sequence
 from itertools import product
 from time import time
-from typing import TYPE_CHECKING, Mapping, Optional, Sequence, Tuple
+from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 import pytest
 import scanpy as sc
 from anndata import AnnData
 from pandas.testing import assert_frame_equal
@@ -146,15 +149,15 @@
                     [g[8], g[10]],
                     [g[8], g[11]],
                     [g[9], g[10]],
                     [g[9], g[11]],
                     [g[12], g[13]],
                 ]
             )
-            .applymap(str.upper)
+            .map(str.upper)
             .values,
         )
 
     def test_fdr_axis_works(self, adata: AnnData, interactions: Interactions_t):
         rc = ligrec(
             adata,
             _CK,
@@ -219,15 +222,15 @@
         assert "foobar" not in adata.uns
         assert len(r) == 3
         assert isinstance(r["means"], pd.DataFrame)
         assert isinstance(r["pvalues"], pd.DataFrame)
         assert isinstance(r["metadata"], pd.DataFrame)
 
     @pytest.mark.parametrize("fdr_method", [None, "fdr_bh"])
-    def test_pvals_in_correct_range(self, adata: AnnData, interactions: Interactions_t, fdr_method: Optional[str]):
+    def test_pvals_in_correct_range(self, adata: AnnData, interactions: Interactions_t, fdr_method: str | None):
         r = ligrec(
             adata,
             _CK,
             interactions=interactions,
             n_perms=5,
             copy=True,
             show_progress_bar=False,
```

### Comparing `squidpy-1.4.1/tests/graph/test_nhood.py` & `squidpy-1.5.0/tests/graph/test_nhood.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 import pandas as pd
 import pytest
 from anndata import AnnData
 from squidpy._constants._pkg_constants import Key
 from squidpy.gr import (
     centrality_scores,
@@ -118,44 +120,24 @@
         assert len(adata.obsp["spatial_connectivities"].data) == res.sum()
 
 
 def test_interaction_matrix_values(adata_intmat: AnnData):
     result_weighted = interaction_matrix(adata_intmat, "cat", weights=True, copy=True)
     result_unweighted = interaction_matrix(adata_intmat, "cat", weights=False, copy=True)
 
-    expected_weighted = np.array(
-        [
-            [5, 1],
-            [2, 3],
-        ]
-    )
-    expected_unweighted = np.array(
-        [
-            [4, 1],
-            [2, 2],
-        ]
-    )
+    expected_weighted = np.array([[5, 1], [2, 3]])
+    expected_unweighted = np.array([[4, 1], [2, 2]])
 
     np.testing.assert_array_equal(expected_weighted, result_weighted)
     np.testing.assert_array_equal(expected_unweighted, result_unweighted)
 
 
 def test_interaction_matrix_nan_values(adata_intmat: AnnData):
-    adata_intmat.obs["cat"].iloc[0] = np.nan
+    adata_intmat.obs.loc["0", "cat"] = np.nan
     result_weighted = interaction_matrix(adata_intmat, "cat", weights=True, copy=True)
     result_unweighted = interaction_matrix(adata_intmat, "cat", weights=False, copy=True)
 
-    expected_weighted = np.array(
-        [
-            [2, 1],
-            [2, 3],
-        ]
-    )
-    expected_unweighted = np.array(
-        [
-            [1, 1],
-            [2, 2],
-        ]
-    )
+    expected_weighted = np.array([[2, 1], [2, 3]])
+    expected_unweighted = np.array([[1, 1], [2, 2]])
 
     np.testing.assert_array_equal(expected_weighted, result_weighted)
     np.testing.assert_array_equal(expected_unweighted, result_unweighted)
```

### Comparing `squidpy-1.4.1/tests/graph/test_ppatterns.py` & `squidpy-1.5.0/tests/graph/test_ppatterns.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Any, Literal
 
 import numpy as np
 import pytest
 from anndata import AnnData
 from pandas.testing import assert_frame_equal
 from squidpy._constants._pkg_constants import Key
```

### Comparing `squidpy-1.4.1/tests/graph/test_ripley.py` & `squidpy-1.5.0/tests/graph/test_ripley.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 import pytest
 from anndata import AnnData
 from squidpy._constants._constants import RipleyStat
 from squidpy.gr import ripley
 
 CLUSTER_KEY = "leiden"
```

### Comparing `squidpy-1.4.1/tests/graph/test_sepal.py` & `squidpy-1.5.0/tests/graph/test_sepal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 from anndata import AnnData
 from pandas.testing import assert_frame_equal
 from squidpy.gr import sepal, spatial_neighbors
 
 UNS_KEY = "sepal_score"
```

### Comparing `squidpy-1.4.1/tests/graph/test_spatial_neighbors.py` & `squidpy-1.5.0/tests/graph/test_spatial_neighbors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple
+from __future__ import annotations
 
 import anndata as ad
 import numpy as np
 import pytest
 from anndata import AnnData
 from scipy.sparse import isspmatrix_csr
 from squidpy._constants._pkg_constants import Key
```

### Comparing `squidpy-1.4.1/tests/graph/test_utils.py` & `squidpy-1.5.0/tests/graph/test_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 import pandas as pd
 import pytest
 from anndata import AnnData
 from squidpy._constants._pkg_constants import Key
 from squidpy.gr._utils import _shuffle_group
```

### Comparing `squidpy-1.4.1/tests/image/test_container.py` & `squidpy-1.5.0/tests/image/test_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from __future__ import annotations
+
 import subprocess
 from collections import defaultdict
+from collections.abc import Sequence, Set
 from html.parser import HTMLParser
 from itertools import permutations
 from pathlib import Path
-from typing import Any, List, Optional, Sequence, Set, Tuple, Union
+from typing import Any
 
 import anndata as ad
 import dask.array as da
 import imageio.v3 as iio
 import numpy as np
 import pytest
 import squidpy as sq
@@ -131,15 +134,15 @@
     @pytest.mark.parametrize(
         ("shape1", "shape2"),
         [
             ((100, 200, 3), (100, 200, 1)),
             ((100, 200, 3), (100, 200)),
         ],
     )
-    def test_add_img(self, shape1: Tuple[int, ...], shape2: Tuple[int, ...]):
+    def test_add_img(self, shape1: tuple[int, ...], shape2: tuple[int, ...]):
         img_orig = np.random.randint(low=0, high=255, size=shape1, dtype=np.uint8)
         cont = ImageContainer(img_orig, layer="img_orig")
 
         img_new = np.random.randint(low=0, high=255, size=shape2, dtype=np.uint8)
         cont.add_img(img_new, layer="img_new", channel_dim="mask")
 
         assert "img_orig" in cont
@@ -148,15 +151,15 @@
 
     def test_add_img_invalid_zdim(self, cont: ImageContainer):
         with pytest.raises(ValueError, match=r"Expected image to have `1` Z-dimension\(s\), found `10`."):
             cont.add_img(np.random.normal(size=(*cont.shape, 10, 3)), dims=["y", "x", "z", "channels"])
 
     @pytest.mark.parametrize("ext", ["jpg", "png"])
     @pytest.mark.parametrize("shape", [(100, 200, 3), (100, 200, 1)])
-    def test_load_ext(self, shape: Tuple[int, ...], ext: str, tmpdir):
+    def test_load_ext(self, shape: tuple[int, ...], ext: str, tmpdir):
         fname = tmpdir / f"tmp.{ext}"
 
         if shape == (100, 200, 1):
             img = np.random.randint(256, size=(100, 200), dtype=np.uint8)
             img_orig = Image.fromarray(img)
         else:
             img_orig = np.random.randint(low=0, high=255, size=shape, dtype=np.uint8)
@@ -164,28 +167,28 @@
 
         gt = iio.imread(str(fname))  # because of compression, we load again
         cont = ImageContainer(str(fname))
 
         np.testing.assert_array_equal(cont["image"].values.squeeze(), gt.squeeze())
 
     @pytest.mark.parametrize("shape", [(100, 200, 3), (100, 200, 1), (10, 100, 200, 1)])
-    def test_load_tiff(self, shape: Tuple[int, ...], tmpdir):
+    def test_load_tiff(self, shape: tuple[int, ...], tmpdir):
         img_orig = np.random.randint(low=0, high=255, size=shape, dtype=np.uint8)
         fname = tmpdir / "tmp.tiff"
         tifffile.imwrite(fname, img_orig)
 
         cont = ImageContainer(str(fname))
 
         if len(shape) > 3:  # multi-channel tiff
             np.testing.assert_array_equal(np.squeeze(cont["image"]), img_orig[..., 0].transpose(1, 2, 0))
         else:
             np.testing.assert_array_equal(np.squeeze(cont["image"]), np.squeeze(img_orig))
 
     @pytest.mark.parametrize("dims", [("y", "x", "z", "c"), ("foo", "bar", "faa", "baz")])
-    def test_load_netcdf(self, tmpdir, dims: Tuple[str, ...]):
+    def test_load_netcdf(self, tmpdir, dims: tuple[str, ...]):
         arr = np.random.normal(size=(100, 10, 1, 4))
         ds = xr.Dataset({"quux": xr.DataArray(arr, dims=dims)})
         fname = tmpdir / "tmp.nc"
         ds.to_netcdf(str(fname))
 
         if "foo" in dims:
             with pytest.raises(ValueError, match=r"Expected to find"):
@@ -196,15 +199,15 @@
             assert len(cont) == 1
             assert "quux" in cont
             np.testing.assert_array_equal(cont["quux"], ds["quux"])
 
     @pytest.mark.parametrize(
         "array", [np.zeros((10, 10, 3), dtype=np.uint8), np.random.rand(10, 10, 1).astype(np.float32)]
     )
-    def test_array_dtypes(self, array: Union[np.ndarray, xr.DataArray]):
+    def test_array_dtypes(self, array: np.ndarray | xr.DataArray):
         img = ImageContainer(array)
         np.testing.assert_array_equal(np.squeeze(img["image"].data), np.squeeze(array))
         assert img["image"].data.dtype == array.dtype
 
         img = ImageContainer(xr.DataArray(array))
         np.testing.assert_array_equal(np.squeeze(img["image"].data), np.squeeze(array))
         assert img["image"].data.dtype == array.dtype
@@ -280,27 +283,27 @@
 
         assert len(small_cont_1c) == 0
 
         with pytest.raises(KeyError, match=r"'image'"):
             del small_cont_1c["image"]
 
     @pytest.mark.parametrize("img_key", [None, "hires", "lowres"])
-    def test_read_from_adata(self, adata: AnnData, img_key: Optional[str]):
+    def test_read_from_adata(self, adata: AnnData, img_key: str | None):
         img = sq.im.ImageContainer.from_adata(adata, img_key=img_key)
         if img_key is None:
             img_key = "hires"
         shape = ((100, 100) if img_key == "hires" else (88, 49)) + (1, 3)
 
         assert isinstance(img, ImageContainer)
         assert img_key in img
 
         np.testing.assert_array_equal(img[img_key].shape, shape)
 
     @pytest.mark.parametrize("scale", [None, 42])
-    def test_read_from_adata_scalefactor(self, adata: AnnData, scale: Optional[int]):
+    def test_read_from_adata_scalefactor(self, adata: AnnData, scale: int | None):
         img_key = "lowres"
         library_id = Key.uns.library_id(adata, Key.uns.spatial)
         del adata.uns[Key.uns.spatial][library_id]["scalefactors"][f"tissue_{img_key}_scalef"]
         if scale is None:
             kwargs = {}
             scale = 1.0
         else:
@@ -389,17 +392,15 @@
             assert isinstance(crop["image"].data, da.Array)
             crop.compute()
 
         assert isinstance(crop["image"].data, np.ndarray)
 
     @pytest.mark.parametrize("dy", [-10, 25, 0.3])
     @pytest.mark.parametrize("dx", [-10, 30, 0.5])
-    def test_crop_corner_size(
-        self, small_cont_1c: ImageContainer, dy: Optional[Union[int, float]], dx: Optional[Union[int, float]]
-    ):
+    def test_crop_corner_size(self, small_cont_1c: ImageContainer, dy: int | float | None, dx: int | float | None):
         crop = small_cont_1c.crop_corner(dy, dx, size=20)
         # original coordinates
         ody, odx = max(dy, 0), max(dx, 0)
         ody = int(ody * small_cont_1c.shape[0]) if isinstance(ody, float) else ody
         odx = int(odx * small_cont_1c.shape[1]) if isinstance(odx, float) else odx
 
         # crop coordinates
@@ -427,40 +428,38 @@
     def test_test_crop_corner_cval(self, cval: float):
         shape_img = (50, 50)
         img = ImageContainer(np.zeros(shape_img))
         crop = img.crop_corner(10, 10, cval=cval)
         np.testing.assert_array_equal(crop["image"].data[-10:, -10:], cval)
 
     @pytest.mark.parametrize("size", [(10, 10), (10, 11)])
-    def test_crop_corner_mask_circle(self, small_cont_1c: ImageContainer, size: Tuple[int, int]):
+    def test_crop_corner_mask_circle(self, small_cont_1c: ImageContainer, size: tuple[int, int]):
         if size[0] != size[1]:
             with pytest.raises(ValueError, match=r"Masking circle is only"):
                 small_cont_1c.crop_corner(0, 0, size=size, mask_circle=True, cval=np.nan)
         else:
             crop = small_cont_1c.crop_corner(0, 0, size=20, mask_circle=True, cval=np.nan)
             mask = (crop.data.x - 10) ** 2 + (crop.data.y - 10) ** 2 <= 10**2
 
             assert crop.shape == (20, 20)
             np.testing.assert_array_equal(crop["image"].values[..., 0][~mask.values], np.nan)
 
     @pytest.mark.parametrize("ry", [23, 1.0])
     @pytest.mark.parametrize("rx", [30, 0.5])
-    def test_crop_center_radius(
-        self, small_cont_1c: ImageContainer, ry: Optional[Union[int, float]], rx: Optional[Union[int, float]]
-    ):
+    def test_crop_center_radius(self, small_cont_1c: ImageContainer, ry: int | float | None, rx: int | float | None):
         crop = small_cont_1c.crop_center(0, 0, radius=(ry, rx))
         sy = int(ry * small_cont_1c.shape[0]) if isinstance(ry, float) else ry
         sx = int(rx * small_cont_1c.shape[1]) if isinstance(rx, float) else rx
 
         assert crop.shape == (2 * sy + 1, 2 * sx + 1)
 
     @pytest.mark.parametrize("squeeze", [False, True])
     @pytest.mark.parametrize("as_array", [False, True, "image", ["image", "baz"]])
     def test_equal_crops_as_array(self, small_cont: ImageContainer, as_array: bool, squeeze: bool):
-        def assert_shape(expected: xr.DataArray, actual: Union[np.ndarray, xr.DataArray]):
+        def assert_shape(expected: xr.DataArray, actual: np.ndarray | xr.DataArray):
             expected_shape = list(expected.shape)
             expected_shape[:2] = [11, 11]  # because crop is 11x11
             if squeeze:
                 assert actual.shape == np.squeeze(np.empty(expected_shape)).shape
             else:
                 assert actual.shape == tuple(expected_shape)
 
@@ -513,15 +512,15 @@
                 assert isinstance(crop, np.ndarray)
                 assert crop.shape == (*size, cont[as_array].data.shape[-1])
             else:
                 assert isinstance(crop, ImageContainer)
                 assert crop.shape == size
 
     @pytest.mark.parametrize("n_names", [None, 4])
-    def test_spot_crops_obs_names(self, adata: AnnData, cont: ImageContainer, n_names: Optional[int]):
+    def test_spot_crops_obs_names(self, adata: AnnData, cont: ImageContainer, n_names: int | None):
         obs = adata.obs_names[:n_names] if isinstance(n_names, int) else adata.obs_names
         crops = list(cont.generate_spot_crops(adata, obs_names=obs))
 
         assert len(crops) == len(obs)
         for crop, o in zip(crops, obs):
             assert crop.data.attrs[Key.img.obs] == o
 
@@ -674,15 +673,15 @@
         assert (ry, rx) == (cont.shape[0], 1)
 
         ry, rx = cont._get_size((-1, None))
         assert (ry, rx) == (-1, cont.shape[1])
 
     @pytest.mark.parametrize("sx", [-1, -1.0, 0.5, 10])
     @pytest.mark.parametrize("sy", [-1, -1.0, 0.5, 10])
-    def test_to_pixel_space(self, sy: Union[int, float], sx: Union[int, float]):
+    def test_to_pixel_space(self, sy: int | float, sx: int | float):
         cont = ImageContainer(np.empty((10, 10)))
 
         if (isinstance(sy, float) and sy < 0) or (isinstance(sx, float) and sx < 0):
             with pytest.raises(ValueError, match=r"Expected .* to be in interval `\[0, 1\]`.*"):
                 cont._convert_to_pixel_space((sy, sx))
         else:
             ry, rx = cont._convert_to_pixel_space((sy, sx))
@@ -694,15 +693,15 @@
             if isinstance(sx, int):
                 assert rx == sx
             else:
                 assert rx == int(cont.shape[1] * sx)
 
     @pytest.mark.parametrize("channel", [None, 0])
     @pytest.mark.parametrize("copy", [False, True])
-    def test_apply(self, copy: bool, channel: Optional[int]):
+    def test_apply(self, copy: bool, channel: int | None):
         cont = ImageContainer(np.random.normal(size=(100, 100, 3)))
         orig = cont.copy()
 
         res = cont.apply(lambda arr: arr + 42, channel=channel, copy=copy)
 
         if copy:
             assert isinstance(res, ImageContainer)
@@ -714,31 +713,29 @@
 
         if channel is None:
             np.testing.assert_allclose(data.values, orig["image"].values + 42)
         else:
             np.testing.assert_allclose(data.values[..., 0], orig["image"].values[..., channel] + 42)
 
     @pytest.mark.parametrize("depth", [None, (30, 30, 0)])
-    def test_apply_overlap(self, small_cont: ImageContainer, mocker: MockerFixture, depth: Optional[Tuple[int, ...]]):
+    def test_apply_overlap(self, small_cont: ImageContainer, mocker: MockerFixture, depth: tuple[int, ...] | None):
         if depth is None:
             kwargs = {}
             spy = mocker.spy(da, "map_blocks")
         else:
             kwargs = {"depth": depth}
             spy = mocker.spy(da, "map_overlap")
         _ = small_cont.apply(lambda arr: arr + 1, chunks=15, **kwargs)
 
         spy.assert_called_once()
 
     @pytest.mark.parametrize("copy", [False, True])
     @pytest.mark.parametrize("chunks", [25, (50, 50, 1, 3), "auto"])
     @pytest.mark.parametrize("lazy", [False, True])
-    def test_apply_dask(
-        self, small_cont: ImageContainer, copy: bool, chunks: Union[int, Tuple[int, ...], str], lazy: bool
-    ):
+    def test_apply_dask(self, small_cont: ImageContainer, copy: bool, chunks: int | tuple[int, ...] | str, lazy: bool):
         def func(chunk: np.ndarray) -> np.ndarray:
             if isinstance(chunks, tuple):
                 np.testing.assert_array_equal(chunk.shape, chunks)
             elif isinstance(chunks, int):
                 np.testing.assert_array_equal(chunk.shape, [chunks, chunks, 1, 3])
             return chunk
 
@@ -754,15 +751,15 @@
         if lazy:
             assert isinstance(cont["foo"].data, da.Array)
         else:
             assert isinstance(cont["foo"].data, np.ndarray)
 
     @pytest.mark.parametrize("as_dask", [False, True])
     def test_apply_passes_correct_array_type(self, as_dask: bool):
-        def func(arr: Union[np.ndarray, da.Array]):
+        def func(arr: np.ndarray | da.Array):
             if as_dask:
                 assert isinstance(arr, da.Array)
             else:
                 assert isinstance(arr, np.ndarray)
             assert arr.shape == (100, 100, 1, 3)
             return arr
 
@@ -882,22 +879,20 @@
         # build adata to crop from img
         crop_coords = np.array([[0, 0], [0, 4], [0, 8], [4, 0], [4, 4], [4, 8], [8, 0], [8, 4], [8, 8]])
         # for library_id 1
         adata1 = AnnData(
             np.zeros((len(crop_coords), 1)),
             uns={"spatial": {"1": {"scalefactors": {"spot_diameter_fullres": 5}}}},
             obsm={"spatial": crop_coords},
-            dtype=float,
         )
         # for library_id 2 (with larger scalefactor)
         adata2 = AnnData(
             np.zeros((len(crop_coords), 1)),
             uns={"spatial": {"2": {"scalefactors": {"spot_diameter_fullres": 7}}}},
             obsm={"spatial": crop_coords},
-            dtype=float,
         )
         # concatenate
         adata = ad.concat({"1": adata1, "2": adata2}, uns_merge="unique", label="library_id")
         adata.obs_names_make_unique()
 
         cont1 = ImageContainer(np.zeros((10, 10, 3)) + 1, library_id="1")
         cont2 = ImageContainer(np.zeros((10, 10, 3)) + 2, library_id="2")
@@ -931,15 +926,15 @@
             assert el.shape == (7, 7)
         res = ImageContainer.uncrop(els)
         assert (res.data["image"].sel(z="2").values == cont_comb.data["image"].sel(z="2").values).all()
 
     @pytest.mark.parametrize("channel", [None, 0])
     @pytest.mark.parametrize("copy", [False, True])
     @pytest.mark.parametrize("library_id", [["l1"], ["l2"], ["l1", "l2", "l3"], None])
-    def test_apply(self, copy: bool, channel: Optional[int], library_id: Optional[Union[list[str], str]]):
+    def test_apply(self, copy: bool, channel: int | None, library_id: list[str] | str | None):
         cont = ImageContainer(
             np.random.normal(size=(100, 100, 3, 2)), dims=("y", "x", "z", "channels"), library_id=["l1", "l2", "l3"]
         )
         orig = cont.copy()
 
         if library_id is None:
             library_ids = ["l1", "l2", "l3"]
@@ -974,20 +969,20 @@
                     np.testing.assert_allclose(
                         data.sel(z=lid).values[..., 0], orig["image"].sel(z=lid).values[..., channel]
                     )
 
 
 class TestExplicitDims:
     @pytest.mark.parametrize("dims", list(permutations(["y", "x", "z", "c"])))
-    def test_explicit_dims(self, dims: Tuple[str, str, str, str]):
+    def test_explicit_dims(self, dims: tuple[str, str, str, str]):
         shape = (2, 3, 4, 5)
         img = ImageContainer(np.random.normal(size=shape), dims=dims)
 
         for d, s in zip(dims, shape):
-            assert img.data.dims[d] == s
+            assert img.data.sizes[d] == s
 
     @pytest.mark.parametrize("missing", ["y", "x", "z"])
     @pytest.mark.parametrize("ndim", [2, 3, 4])
     def test_required_dim_missing(self, missing: str, ndim: int):
         shape = (2, 3)
         if ndim >= 3:
             shape += (4,)
@@ -1000,51 +995,51 @@
             "channels",
         )
         dims = dims[:ndim]
 
         if ndim in (2, 3) and missing == "z":
             img = ImageContainer(np.random.normal(size=shape), dims=dims)
             for d, s in zip(dims, shape):
-                assert img.data.dims[d] == s
-            assert img.data.dims["z"] == 1
+                assert img.data.sizes[d] == s
+            assert img.data.sizes["z"] == 1
         else:
             with pytest.raises(ValueError, match=rf"Expected to find `\[{missing!r}\]` dimension\(s\)"):
                 _ = ImageContainer(np.random.normal(size=shape), dims=dims)
 
     @pytest.mark.parametrize("dims", ["z_last", "channels_last", ("x", "y")])
     def test_2D_array(self, dims: str):
         shape = (2, 3)
         img = ImageContainer(np.random.normal(size=shape), dims=dims)
 
         if isinstance(dims, str):
             dims = ("channels", "z", "y", "x")
             shape = (1, 1) + shape
         for d, s in zip(dims, shape):
-            assert img.data.dims[d] == s
+            assert img.data.sizes[d] == s
 
     @pytest.mark.parametrize("dims", ["z_last", "channels_last", ("x", "y", "z"), ("y", "x", "c")])
     def test_3D_array(self, dims: str):
         shape = (2, 3, 4)
         img = ImageContainer(np.random.normal(size=shape), dims=dims)
 
         if isinstance(dims, str):
             dims = (("channels", "z") if dims == "z_last" else ("z", "channels")) + ("y", "x")
             shape = (1,) + shape
         for d, s in zip(dims, shape):
-            assert img.data.dims[d] == s
+            assert img.data.sizes[d] == s
 
     @pytest.mark.parametrize("dims", ["z_last", "channels_last", ("z", "y", "x", "c")])
     def test_4D_array(self, dims: str):
         shape = (2, 3, 4, 5)
         img = ImageContainer(np.random.normal(size=shape), dims=dims)
 
         if isinstance(dims, str):
             dims = (("channels", "z") if dims == "z_last" else ("z", "channels")) + ("y", "x")
         for d, s in zip(dims, shape):
-            assert img.data.dims[d] == s
+            assert img.data.sizes[d] == s
 
 
 class TestLibraryIds:
     def test_empty_container(self):
         img = ImageContainer()
         np.testing.assert_array_equal(img.library_ids, [])
 
@@ -1085,15 +1080,15 @@
         img = ImageContainer(tmp["image"])
 
         np.testing.assert_array_equal(tmp.library_ids, library_id)
         np.testing.assert_array_equal(img.library_ids, library_id)
 
     @pytest.mark.parametrize("library_id", ["a", ["b", "a"], ["c"]])
     @pytest.mark.parametrize("empty", [False, True])
-    def test_get_library_ids(self, empty: bool, library_id: Union[str, Sequence[str]]):
+    def test_get_library_ids(self, empty: bool, library_id: str | Sequence[str]):
         img = ImageContainer()
         if not empty:
             img.add_img(np.random.normal(size=(2, 3, 4, 5)), dims=["z", "y", "x", "c"], library_id=["a", "b"])
 
         if empty:
             np.testing.assert_array_equal(np.ravel([library_id]), img._get_library_ids(library_id))
         else:
@@ -1255,8 +1250,8 @@
         ds.to_zarr(Path(tmpdir))
 
         if dim_name == "z":
             with pytest.raises(ValueError, match=r".*z.*exists"):
                 _ = ImageContainer.load(str(tmpdir))
         else:
             img = ImageContainer.load(str(tmpdir))
-            assert img.data.dims == {"x": 64, "y": 64, "z": 1, dim_name: 3}
+            assert img.data.sizes == {"x": 64, "y": 64, "z": 1, dim_name: 3}
```

### Comparing `squidpy-1.4.1/tests/image/test_features.py` & `squidpy-1.5.0/tests/image/test_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Sequence, Tuple
+from __future__ import annotations
+
+from collections.abc import Sequence
 
 import numpy as np
 import pandas as pd
 import pytest
 from anndata import AnnData
 from pytest_mock import MockerFixture
 from squidpy._constants._constants import ImageFeature
```

### Comparing `squidpy-1.4.1/tests/image/test_io.py` & `squidpy-1.5.0/tests/image/test_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Optional, Tuple, Union
+from __future__ import annotations
 
 import dask.array as da
 import numpy as np
 import pytest
 import tifffile
 import xarray as xr
 from pytest_mock import MockerFixture
@@ -77,15 +77,15 @@
             elif infer_dim == InferDimensions.Z_LAST:
                 np.testing.assert_array_equal(actual_dims, ["channels", "y", "x", "z"])
             else:
                 np.testing.assert_array_equal(actual_dims, ["z", "y", "x", "channels"])
             np.testing.assert_array_equal(actual_shape, shape)
 
     @pytest.mark.parametrize("chunks", [100, (1, 100, 100, 3), "auto", None, {"y": 100, "x": 100}])
-    def test_lazy_load_image(self, chunks: Optional[Union[int, tuple[int, ...], str, dict[str, int]]], tmpdir):
+    def test_lazy_load_image(self, chunks: int | tuple[int, ...] | str | dict[str, int] | None, tmpdir):
         path = str(tmpdir / "img.tiff")
         img = self._create_image(path, (256, 256, 3))
 
         res = _lazy_load_image(path, chunks=chunks)
 
         assert isinstance(res, xr.DataArray)
         assert isinstance(res.data, da.Array)
```

### Comparing `squidpy-1.4.1/tests/image/test_processing.py` & `squidpy-1.5.0/tests/image/test_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Callable, Optional, Sequence, Tuple, Union
+from __future__ import annotations
+
+from collections.abc import Callable, Sequence
 
 import dask.array as da
 import numpy as np
 import pytest
 from pytest_mock import MockerFixture
 from squidpy._constants._pkg_constants import Key
 from squidpy.im import ImageContainer, process
@@ -11,35 +13,35 @@
 class TestProcess:
     def test_invalid_layer(self, small_cont: ImageContainer):
         with pytest.raises(KeyError, match=r"Image layer `foobar` not found in"):
             process(small_cont, layer="foobar")
 
     @pytest.mark.parametrize("dy", [25, 0.3, None])
     @pytest.mark.parametrize("dx", [30, 0.5, None])
-    def test_size(self, small_cont: ImageContainer, dy: Optional[Union[int, float]], dx: Optional[Union[int, float]]):
+    def test_size(self, small_cont: ImageContainer, dy: int | float | None, dx: int | float | None):
         res = process(small_cont, method="smooth", copy=True)
         key = Key.img.process("smooth", "image")
 
         assert res.shape == small_cont.shape
         np.testing.assert_array_equal(res[key].dims, small_cont["image"].dims)
 
     @pytest.mark.parametrize("method", ["smooth", "gray", lambda arr: arr])
-    def test_method(self, small_cont: ImageContainer, method: Union[str, Callable[[np.ndarray], np.ndarray]]):
+    def test_method(self, small_cont: ImageContainer, method: str | Callable[[np.ndarray], np.ndarray]):
         res = process(small_cont, method=method, copy=True)
         key = Key.img.process(method, "image")
 
         assert isinstance(res, ImageContainer)
         assert key in res
         if callable(method):
             np.testing.assert_array_equal(small_cont["image"].values, res[key].values)
         else:
             assert not np.all(np.allclose(small_cont["image"].values, res[key].values))
 
     @pytest.mark.parametrize("method", ["smooth", "gray", lambda arr: arr[..., 0]])
-    def test_channel_dim(self, small_cont: ImageContainer, method: Union[str, Callable[[np.ndarray], np.ndarray]]):
+    def test_channel_dim(self, small_cont: ImageContainer, method: str | Callable[[np.ndarray], np.ndarray]):
         res = process(small_cont, method=method, copy=True, channel_dim="foo")
         key = Key.img.process(method, "image")
 
         assert isinstance(res, ImageContainer)
 
         if method == "smooth":
             np.testing.assert_array_equal(res[key].dims, ["y", "x", "z", "foo"])
@@ -48,15 +50,15 @@
             np.testing.assert_array_equal(res[key].dims, ["y", "x", "z", f"foo_{modifier}"])
 
     def test_gray_not_rgb(self, small_cont_1c: ImageContainer):
         with pytest.raises(ValueError, match=r"Expected channel dimension to be `3`, found `1`."):
             process(small_cont_1c, method="gray")
 
     @pytest.mark.parametrize("key_added", [None, "foo"])
-    def test_key_added(self, small_cont: ImageContainer, key_added: Optional[str]):
+    def test_key_added(self, small_cont: ImageContainer, key_added: str | None):
         res = process(small_cont, method="smooth", copy=False, layer_added=key_added, layer="image")
 
         assert res is None
         assert Key.img.process("smooth", "image", layer_added=key_added)
 
     def test_passing_kwargs(self, small_cont: ImageContainer):
         def func(arr: np.ndarray, sentinel: bool = False) -> np.ndarray:
@@ -83,15 +85,15 @@
         spy.assert_called_once()
         np.testing.assert_array_equal(small_cont["foo"].values, small_cont["image"].values)
 
     @pytest.mark.parametrize("dask_input", [False, True])
     @pytest.mark.parametrize("chunks", [25, (50, 50, 1, 3), "auto"])
     @pytest.mark.parametrize("lazy", [False, True])
     def test_dask_processing(
-        self, small_cont: ImageContainer, dask_input: bool, chunks: Union[int, tuple[int, ...], str], lazy: bool
+        self, small_cont: ImageContainer, dask_input: bool, chunks: int | tuple[int, ...] | str, lazy: bool
     ):
         def func(chunk: np.ndarray):
             if isinstance(chunks, tuple):
                 np.testing.assert_array_equal(chunk.shape, chunks)
             elif isinstance(chunks, int):
                 np.testing.assert_array_equal(chunk.shape, [chunks, chunks, 1, 3])
 
@@ -110,15 +112,15 @@
         else:
             # make sure we didn't accidentally trigger foo's computation
             assert isinstance(small_cont["foo"].data, da.Array if dask_input else np.ndarray)
 
         assert isinstance(small_cont["bar"].data, np.ndarray)
 
     @pytest.mark.parametrize("library_id", [None, "3", ["1", "2"]])
-    def test_library_id(self, cont_4d: ImageContainer, library_id: Optional[Union[str, Sequence[str]]]):
+    def test_library_id(self, cont_4d: ImageContainer, library_id: str | Sequence[str] | None):
         def func(arr: np.ndarray):
             if library_id is None:
                 assert arr.shape == cont_4d["image"].shape
             else:
                 assert arr.shape == cont_4d["image"][..., 0, :].shape
             return arr + 1
```

### Comparing `squidpy-1.4.1/tests/image/test_segmentation.py` & `squidpy-1.5.0/tests/image/test_segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Callable, Optional, Sequence, Tuple, Union
+from __future__ import annotations
+
+from collections.abc import Callable, Sequence
 
 import dask.array as da
 import numpy as np
 import pytest
 from pytest_mock import MockerFixture
 from squidpy._constants._constants import SegmentationBackend
 from squidpy._constants._pkg_constants import Key
@@ -55,15 +57,15 @@
         assert res.shape == img.shape
         assert "image" in res
         assert res["image"].dims == img["image"].dims
 
 
 class TestWatershed:
     @pytest.mark.parametrize("thresh", [None, 0.1, 0.5, 1.0])
-    def test_threshold(self, thresh: Optional[float], mocker: MockerFixture):
+    def test_threshold(self, thresh: float | None, mocker: MockerFixture):
         img = np.zeros((100, 200), dtype=np.float64)
         img[2:10, 2:10] = 1.0
         img[30:34, 10:16] = 1.0
         img = ImageContainer(img, layer="image")
 
         sw = SegmentationWatershed()
         spy = mocker.spy(sw, "_segment")
@@ -79,15 +81,15 @@
 
 class TestHighLevel:
     def test_invalid_layer(self, small_cont: ImageContainer):
         with pytest.raises(KeyError, match=r"Image layer `foobar` not found in"):
             segment(small_cont, layer="foobar")
 
     @pytest.mark.parametrize("method", ["watershed", dummy_segment])
-    def test_method(self, small_cont: ImageContainer, method: Union[str, Callable]):
+    def test_method(self, small_cont: ImageContainer, method: str | Callable):
         res = segment(small_cont, method=method, copy=True)
 
         assert isinstance(res, ImageContainer)
         assert res.shape == small_cont.shape
 
         if callable(method):
             method = SegmentationBackend.CUSTOM.s
@@ -95,15 +97,15 @@
         assert Key.img.segment(method) in res
 
         if method in ("log", "dog", "dog"):
             assert res[Key.img.segment(method)].values.max() <= 1
 
     @pytest.mark.parametrize("dy", [11, 0.5, None])
     @pytest.mark.parametrize("dx", [15, 0.1, None])
-    def test_size(self, small_cont: ImageContainer, dy: Optional[Union[int, float]], dx: Optional[Union[int, float]]):
+    def test_size(self, small_cont: ImageContainer, dy: int | float | None, dx: int | float | None):
         res = segment(small_cont, size=(dy, dx), copy=True)
 
         assert isinstance(res, ImageContainer)
         assert res.shape == small_cont.shape
 
     @pytest.mark.parametrize("channel", [0, 1, 2])
     def test_channel(self, small_cont: ImageContainer, channel: int):
@@ -123,15 +125,15 @@
         n_channels = small_cont["image"].sizes["channels"]
         segment(small_cont, copy=False, layer="image", channel=None, method=func, layer_added="seg")
 
         np.testing.assert_array_equal(small_cont["seg"], np.zeros(small_cont.shape + (1, 1)))
         assert small_cont["seg"].dtype == _SEG_DTYPE
 
     @pytest.mark.parametrize("key_added", [None, "foo"])
-    def test_key_added(self, small_cont: ImageContainer, key_added: Optional[str]):
+    def test_key_added(self, small_cont: ImageContainer, key_added: str | None):
         res = segment(small_cont, copy=False, layer="image", layer_added=key_added)
 
         assert res is None
         assert Key.img.segment("watershed", layer_added=key_added) in small_cont
 
     def test_passing_kwargs(self, small_cont: ImageContainer):
         def func(chunk: np.ndarray, sentinel: bool = False):
@@ -144,15 +146,15 @@
         assert small_cont["bar"].values.dtype == _SEG_DTYPE
         np.testing.assert_array_equal(small_cont["bar"].values, 0)
 
     @pytest.mark.parametrize("dask_input", [False, True])
     @pytest.mark.parametrize("chunks", [25, (50, 50, 1), "auto"])
     @pytest.mark.parametrize("lazy", [False, True])
     def test_dask_segment(
-        self, small_cont: ImageContainer, dask_input: bool, chunks: Union[int, tuple[int, ...], str], lazy: bool
+        self, small_cont: ImageContainer, dask_input: bool, chunks: int | tuple[int, ...] | str, lazy: bool
     ):
         def func(chunk: np.ndarray):
             if isinstance(chunks, tuple):
                 np.testing.assert_array_equal(chunk.shape, [chunks[0] + 2 * d, chunks[1] + 2 * d, 1])
             elif isinstance(chunks, int):
                 np.testing.assert_array_equal(chunk.shape, [chunks + 2 * d, chunks + 2 * d, 1])
 
@@ -212,15 +214,15 @@
                 expected[i, j] = start
                 start += 1
 
         assert small_cont["bar"].values.dtype == _SEG_DTYPE
         np.testing.assert_array_equal(small_cont["bar"].values, expected)
 
     @pytest.mark.parametrize("size", [None, 11])
-    def test_watershed_works(self, size: Optional[int]):
+    def test_watershed_works(self, size: int | None):
         img_orig = np.zeros((100, 200, 30), dtype=np.float64)
         img_orig[2:10, 2:10] = 1.0
         img_orig[30:34, 10:16] = 1.0
 
         cont = ImageContainer(img_orig, layer="image_0")
         segment(
             img=cont,
@@ -235,15 +237,15 @@
         assert np.mean(cont.data["segment"].values[img_orig[:, :, 0] > 0] > 0) > 0.5
 
         # for size=10, "fails with `size=10` due to border effects"
         # the reason why there is no test for it that inside tox, it "works" (i.e. the assertion passes)
         # but outside, the assertion fails, as it should
 
     @pytest.mark.parametrize("library_id", [None, "3", ["1", "2"]])
-    def test_library_id(self, cont_4d: ImageContainer, library_id: Optional[Union[str, Sequence[str]]]):
+    def test_library_id(self, cont_4d: ImageContainer, library_id: str | Sequence[str] | None):
         def func(arr: np.ndarray):
             assert arr.shape == cont_4d.shape + (1,)
             return np.ones(arr[..., 0].shape, dtype=_SEG_DTYPE)
 
         segment(cont_4d, method=func, layer="image", layer_added="image_seg", library_id=library_id, copy=False)
 
         np.testing.assert_array_equal(cont_4d["image"].coords, cont_4d["image_seg"].coords)
```

### Comparing `squidpy-1.4.1/tests/plotting/test_graph.py` & `squidpy-1.5.0/tests/plotting/test_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
+from collections.abc import Mapping
 from copy import deepcopy
-from typing import Mapping
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pytest
 import scanpy as sc
 from anndata import AnnData
```

### Comparing `squidpy-1.4.1/tests/plotting/test_image.py` & `squidpy-1.5.0/tests/plotting/test_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pytest
 import scanpy as sc
 import squidpy as sq
 from anndata import AnnData
```

### Comparing `squidpy-1.4.1/tests/plotting/test_interactive.py` & `squidpy-1.5.0/tests/plotting/test_interactive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from __future__ import annotations
+
 import platform
 import sys
-from typing import Tuple
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pytest
 from anndata import AnnData
 from matplotlib.testing.compare import compare_images
 from scanpy import settings as s
```

### Comparing `squidpy-1.4.1/tests/plotting/test_spatial_static.py` & `squidpy-1.5.0/tests/plotting/test_spatial_static.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import platform
+from collections.abc import Sequence
 from functools import partial
-from typing import Sequence
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pytest
 import scanpy as sc
 from anndata import AnnData
@@ -192,15 +192,15 @@
     def test_tol_plot_spatial_scatter_non_unique_colors(self, adata_hne: AnnData):
         adata_hne.uns["cluster_colors"] = ["#000000"] * len(adata_hne.uns["cluster_colors"])
         pl.spatial_scatter(adata_hne, color="cluster", legend_loc=None)
         self.compare("SpatialStatic_spatial_scatter_non_unique_colors", tolerance=70)
 
     def test_tol_plot_palette_listed_cmap(self, adata_hne: AnnData):
         del adata_hne.uns["cluster_colors"]
-        palette = plt.get_cmap("Set3")
+        palette = plt.colormaps["Set3"]
         assert isinstance(palette, ListedColormap)
         pl.spatial_scatter(adata_hne, color="cluster", palette=palette, legend_loc=None)
         self.compare("SpatialStatic_palette_listed_cmap", tolerance=70)
 
 
 class TestSpatialStaticUtils:
     @staticmethod
@@ -208,17 +208,16 @@
         n_obs = len(library_id) * 2 if isinstance(library_id, list) else 2
         X = np.empty((n_obs, 3))
         if not isinstance(library_id, list) and library_id is not None:
             library_id = [library_id]
         if library_id is not None:
             obs = pd.DataFrame(library_id * 2, columns=[library_key])
             uns = {Key.uns.spatial: {k: None for k in library_id}}
-            return AnnData(X, obs=obs, uns=uns, dtype=X.dtype)
-        else:
-            return AnnData(X, dtype=X.dtype)
+            return AnnData(X, obs=obs, uns=uns)
+        return AnnData(X)
 
     @pytest.mark.parametrize("shape", ["circle", None])
     @pytest.mark.parametrize("library_id", [None, "1", ["1"], ["1", "2"]])
     @pytest.mark.parametrize("library_key", [None, "library_id"])
     def test_get_library_id(self, shape, library_id, library_key):
         adata = TestSpatialStaticUtils._create_anndata(shape, library_id, library_key)
         if not isinstance(library_id, list) and library_id is not None:
```

### Comparing `squidpy-1.4.1/tests/plotting/test_var_by_distance_plot.py` & `squidpy-1.5.0/tests/plotting/test_var_by_distance_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import scanpy as sc
 from anndata import AnnData
 from squidpy import pl, tl
 
 from tests.conftest import PlotTester, PlotTesterMeta
 
 sc.pl.set_rcParams_defaults()
```

### Comparing `squidpy-1.4.1/tests/read/test_visium.py` & `squidpy-1.5.0/tests/read/test_visium.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from anndata.tests.helpers import assert_adata_equal
 from squidpy._constants._pkg_constants import Key
 from squidpy.read import visium
 
 
 def test_read_visium():
     # Test that reading .h5 file works and does not have any global effects.
```

### Comparing `squidpy-1.4.1/tests/tools/test_var_by_distance.py` & `squidpy-1.5.0/tests/tools/test_var_by_distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from __future__ import annotations
 
-from typing import List
-
 import pytest
 from anndata import AnnData
 from squidpy.tl import var_by_distance
 from squidpy.tl._var_by_distance import _normalize_distances
 
 
 class TestVarDist:
```

### Comparing `squidpy-1.4.1/.gitignore` & `squidpy-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/LICENSE` & `squidpy-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/README.rst` & `squidpy-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `squidpy-1.4.1/pyproject.toml` & `squidpy-1.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -113,84 +113,35 @@
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 include-package-data = true
 
 [tool.setuptools_scm]
 
-[tool.black]
-line-length = 120
-target-version = ['py39']
-include = '\.pyi?$'
-exclude = '''
-(
-  /(
-      \.eggs
-    | \.git
-    | \.hg
-    | \.mypy_cache
-    | \.tox
-    | \.venv
-    | _build
-    | buck-out
-    | build
-    | dist
-  )/
-
-)
-'''
-
-[tool.isort]
-profile = "black"
-py_version = "38"
-skip = "docs/source/conf.py,.tox,build"
-line_length = 88
-multi_line_output = 3
-include_trailing_comma = true
-use_parentheses = true
-known_stdlib = "joblib"
-known_bio = "anndata,scanpy"
-known_num = "numpy,numba,scipy,sklearn,statsmodels,pandas,xarray,dask"
-known_plot = "matplotlib,seaborn,napari"
-known_gui = "PyQt5,superqt"
-known_img = "skimage,tifffile,dask_image"
-known_graph = "networkx"
-sections = "FUTURE,STDLIB,THIRDPARTY,BIO,NUM,GUI,PLOT,IMG,GRAPH,FIRSTPARTY,LOCALFOLDER"
-no_lines_before="LOCALFOLDER"
-balanced_wrapping = true
-force_grid_wrap = 0
-length_sort = "1"
-indent = "    "
-from_first = true
-order_by_type = true
-atomic = true
-combine_star = true
-combine_as_imports = true
-honor_noqa = true
-remove_redundant_aliases = true
-only_modified = true
-group_by_package = true
-force_alphabetical_sort_within_sections = true
-lexicographical = true
-
 [tool.hatch.version]
 source = "vcs"
 
 [tool.ruff]
+line-length = 120
 exclude = [
     ".git",
     ".tox",
     "__pycache__",
     "build",
     "docs/_build",
     "dist",
     "setup.py"
 ]
+
+[tool.ruff.format]
+docstring-code-format = true
+
+[tool.ruff.lint]
 ignore = [
-    # line too long -> we accept long comment lines; black gets rid of long code lines
+    # line too long -> we accept long comment lines; formatter gets rid of long code lines
     "E501",
     # Do not assign a lambda expression, use a def -> lambda expression assignments are convenient
     "E731",
     # allow I, O, l as variable names -> I is the identity matrix, i, j, k, l is reasonable indexing notation
     "E741",
     # Missing docstring in public package
     "D104",
@@ -239,35 +190,37 @@
     # "E266",
     # format string does contain unindexed parameters
     # "P101",
     # indentation is not a multiple of 4
     # "E111",
     # "E114",
 ]
-line-length = 120
 select = [
     "I", # isort
     "E", # pycodestyle
     "F", # pyflakes
     "W", # pycodestyle
     # below are not autofixed
     "UP", # pyupgrade
     "C4", # flake8-comprehensions
     "B", # flake8-bugbear
     "BLE", # flake8-blind-except
 ]
-unfixable = ["B", "UP", "C4", "BLE"]
-target-version = "py38"
-[tool.ruff.per-file-ignores]
-    "*/__init__.py" = ["D104", "F401"]
-    "tests/*"= ["D"]
-    "docs/*"= ["D","B"]
-    "squidpy/pl/_ligrec.py"= ["D","B"]
-    "squidpy/_constants/_pkg_constants.py"= ["D101","D102","D106"]
-    "squidpy/_constants/_constants.py"= ["D101"]
-    "squidpy/pl/_interactive/_widgets.py"= ["D"]
-    ".scripts/ci/download_data.py"= ["D","B"]
-    # "squidpy/*.py"= ["RST303"]
+unfixable = ["B", "C4", "BLE"]
+
+[tool.ruff.lint.isort]
+required-imports = ["from __future__ import annotations"]
+
+[tool.ruff.lint.per-file-ignores]
+"*/__init__.py" = ["D104", "F401"]
+"tests/*"= ["D"]
+"docs/*"= ["D","B"]
+"squidpy/pl/_ligrec.py"= ["D","B"]
+"squidpy/_constants/_pkg_constants.py"= ["D101","D102","D106"]
+"squidpy/_constants/_constants.py"= ["D101"]
+"squidpy/pl/_interactive/_widgets.py"= ["D"]
+".scripts/ci/download_data.py"= ["D","B"]
+# "squidpy/*.py"= ["RST303"]
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 # Disallow all relative imports.
 ban-relative-imports = "all"
```

### Comparing `squidpy-1.4.1/PKG-INFO` & `squidpy-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: squidpy
-Version: 1.4.1
+Version: 1.5.0
 Summary: Spatial Single Cell Analysis in Python
 Project-URL: Homepage, https://github.com/scverse/squidpy
 Project-URL: Bug Tracker, https://github.com/scverse/squidpy/issues
 Project-URL: Documentation, https://squidpy.readthedocs.io/en/stable
 Project-URL: Source Code, https://github.com/scverse/squidpy
 Author: Giovanni Palla, Michal Klein, Hannah Spitzer
 Maintainer-email: Giovanni Palla <giovanni.palla@helmholtz-muenchen.de>, Michal Klein <michal.klein@helmholtz-muenchen.de>
```

