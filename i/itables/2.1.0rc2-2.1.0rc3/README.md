# Comparing `tmp/itables-2.1.0rc2.tar.gz` & `tmp/itables-2.1.0rc3.tar.gz`

## Comparing `itables-2.1.0rc2.tar` & `itables-2.1.0rc3.tar`

### file list

```diff
@@ -1,112 +1,117 @@
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 itables-2.1.0rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 itables-2.1.0rc2/.pylintrc
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 itables-2.1.0rc2/codecov.yml
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 itables-2.1.0rc2/environment.yml
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 itables-2.1.0rc2/.github/workflows/comment-pr.yml
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 itables-2.1.0rc2/.github/workflows/continuous-integration.yml
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 itables-2.1.0rc2/.github/workflows/publish-book.yml
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 itables-2.1.0rc2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 itables-2.1.0rc2/binder/postBuild
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 itables-2.1.0rc2/binder/requirements.txt
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 itables-2.1.0rc2/binder/labconfig/default_setting_overrides.json
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/_config.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/_toc.yml
--rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/advanced_parameters.md
--rw-r--r--   0        0        0    18588 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/changelog.md
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/contributing.md
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/custom_css.md
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/custom_extensions.md
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/developing.md
--rw-r--r--   0        0        0    46135 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/df_example.png
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/downsampling.md
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/extensions.md
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/formatting.md
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/pandas_style.md
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/polars_dataframes.md
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/quarto.md
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/quick_start.md
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/references.md
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/sample_dataframes.md
--rw-r--r--   0        0        0    51851 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/show_df.png
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/supported_editors.md
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/troubleshooting.md
--rw-r--r--   0        0        0    83555 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/images/code.png
--rw-r--r--   0        0        0    98830 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/images/colab.png
--rw-r--r--   0        0        0   110756 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/images/html.png
--rw-r--r--   0        0        0   108275 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/images/lab.png
--rw-r--r--   0        0        0   129198 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/images/notebook.png
--rw-r--r--   0        0        0   107743 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/images/pycharm.png
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/quarto/quarto_html.qmd
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/quarto/quarto_revealjs.qmd
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/package-lock.json
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/package.json
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/dt_for_itables/CHANGELOG.md
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/dt_for_itables/LICENSE
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/dt_for_itables/README.md
--rw-r--r--   0        0        0    23839 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/dt_for_itables/package-lock.json
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/dt_for_itables/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/dt_for_itables/src/index.d.ts
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/dt_for_itables/src/index.js
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/itables_for_streamlit/README.md
--rw-r--r--   0        0        0   708765 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/itables_for_streamlit/package-lock.json
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/itables_for_streamlit/package.json
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/itables_for_streamlit/tsconfig.json
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/itables_for_streamlit/public/index.html
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/itables_for_streamlit/src/index.tsx
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/__init__.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/datatables_format.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/downsample.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/interactive.py
--rw-r--r--   0        0        0    27476 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/javascript.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/options.py
--rw-r--r--   0        0        0    13926 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/sample_dfs.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/shiny.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/streamlit.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/utils.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/version.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/html/datatables_template.html
--rw-r--r--   0        0        0    68898 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/html/dt_bundle.css
--rw-r--r--   0        0        0   505946 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/html/dt_bundle.js
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/html/init_datatables.html
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/html/column_filters/initComplete.js
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/html/column_filters/pre_dt_code.js
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/itables_for_streamlit/asset-manifest.json
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/itables_for_streamlit/index.html
--rw-r--r--   0        0        0    71691 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/itables_for_streamlit/static/css/main.45cd49da.css
--rw-r--r--   0        0        0   152195 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/itables_for_streamlit/static/css/main.45cd49da.css.map
--rw-r--r--   0        0        0   689965 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/itables_for_streamlit/static/js/main.b98e79fb.js
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/itables_for_streamlit/static/js/main.b98e79fb.js.LICENSE.txt
--rw-r--r--   0        0        0  3051380 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/itables_for_streamlit/static/js/main.b98e79fb.js.map
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/logo/loading.svg
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/logo/logo.svg
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/logo/text.svg
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/logo/wide.svg
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/logo/with_text.svg
--rw-r--r--   0        0        0    31715 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/samples/countries.csv
--rw-r--r--   0        0        0   420013 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/samples/indicators.csv
--rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/samples/population.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/conftest.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_changelog.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_connected_notebook_is_small.py
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_datatables_format.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_documentation_notebooks_run.py
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_downsample.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_extension_arguments.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_html_in_table_header.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_init.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_javascript.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_json_dumps.py
--rw-r--r--   0        0        0   791362 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_notebook.ipynb
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_pandas_style.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_polars.py
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_sample_dfs.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_sample_python_apps.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_update_samples.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/sample_python_apps/itables_in_a_shiny_app.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/sample_python_apps/itables_in_a_shiny_app_with_tabs.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 itables-2.1.0rc2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 itables-2.1.0rc2/LICENSE
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 itables-2.1.0rc2/README.md
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 itables-2.1.0rc2/pyproject.toml
--rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 itables-2.1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 itables-2.1.0rc3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 itables-2.1.0rc3/.pylintrc
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 itables-2.1.0rc3/codecov.yml
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 itables-2.1.0rc3/environment.yml
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 itables-2.1.0rc3/.github/workflows/comment-pr.yml
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 itables-2.1.0rc3/.github/workflows/continuous-integration.yml
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 itables-2.1.0rc3/.github/workflows/publish-book.yml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 itables-2.1.0rc3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 itables-2.1.0rc3/binder/postBuild
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 itables-2.1.0rc3/binder/requirements.txt
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 itables-2.1.0rc3/binder/labconfig/default_setting_overrides.json
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/_config.yml
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/_toc.yml
+-rw-r--r--   0        0        0     6355 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/advanced_parameters.md
+-rw-r--r--   0        0        0    18588 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/changelog.md
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/contributing.md
+-rw-r--r--   0        0        0     4804 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/custom_css.md
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/custom_extensions.md
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/dash.md
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/developing.md
+-rw-r--r--   0        0        0    46135 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/df_example.png
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/downsampling.md
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/extensions.md
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/formatting.md
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/html_export.md
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/ipywidgets.md
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/pandas_style.md
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/polars_dataframes.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/quarto.md
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/quick_start.md
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/references.md
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/sample_dataframes.md
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/shiny.md
+-rw-r--r--   0        0        0    51851 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/show_df.png
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/streamlit.md
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/supported_editors.md
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/troubleshooting.md
+-rw-r--r--   0        0        0    83555 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/images/code.png
+-rw-r--r--   0        0        0    98830 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/images/colab.png
+-rw-r--r--   0        0        0   110756 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/images/html.png
+-rw-r--r--   0        0        0   108275 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/images/lab.png
+-rw-r--r--   0        0        0   129198 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/images/notebook.png
+-rw-r--r--   0        0        0   107743 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/images/pycharm.png
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/quarto/quarto_html.qmd
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 itables-2.1.0rc3/docs/quarto/quarto_revealjs.qmd
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 itables-2.1.0rc3/packages/package-lock.json
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 itables-2.1.0rc3/packages/package.json
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 itables-2.1.0rc3/packages/dt_for_itables/CHANGELOG.md
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 itables-2.1.0rc3/packages/dt_for_itables/LICENSE
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 itables-2.1.0rc3/packages/dt_for_itables/README.md
+-rw-r--r--   0        0        0    23839 2020-02-02 00:00:00.000000 itables-2.1.0rc3/packages/dt_for_itables/package-lock.json
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 itables-2.1.0rc3/packages/dt_for_itables/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 itables-2.1.0rc3/packages/dt_for_itables/src/index.d.ts
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 itables-2.1.0rc3/packages/dt_for_itables/src/index.js
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 itables-2.1.0rc3/packages/itables_for_streamlit/README.md
+-rw-r--r--   0        0        0   708765 2020-02-02 00:00:00.000000 itables-2.1.0rc3/packages/itables_for_streamlit/package-lock.json
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 itables-2.1.0rc3/packages/itables_for_streamlit/package.json
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 itables-2.1.0rc3/packages/itables_for_streamlit/tsconfig.json
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 itables-2.1.0rc3/packages/itables_for_streamlit/public/index.html
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 itables-2.1.0rc3/packages/itables_for_streamlit/src/index.tsx
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/__init__.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/datatables_format.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/downsample.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/interactive.py
+-rw-r--r--   0        0        0    27989 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/javascript.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/options.py
+-rw-r--r--   0        0        0    13926 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/sample_dfs.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/shiny.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/streamlit.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/utils.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/version.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/html/datatables_template.html
+-rw-r--r--   0        0        0    68898 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/html/dt_bundle.css
+-rw-r--r--   0        0        0   505946 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/html/dt_bundle.js
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/html/init_datatables.html
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/html/column_filters/initComplete.js
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/html/column_filters/pre_dt_code.js
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/itables_for_streamlit/asset-manifest.json
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/itables_for_streamlit/index.html
+-rw-r--r--   0        0        0    71691 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/itables_for_streamlit/static/css/main.45cd49da.css
+-rw-r--r--   0        0        0   152195 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/itables_for_streamlit/static/css/main.45cd49da.css.map
+-rw-r--r--   0        0        0   689965 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/itables_for_streamlit/static/js/main.b98e79fb.js
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/itables_for_streamlit/static/js/main.b98e79fb.js.LICENSE.txt
+-rw-r--r--   0        0        0  3051380 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/itables_for_streamlit/static/js/main.b98e79fb.js.map
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/logo/loading.svg
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/logo/logo.svg
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/logo/text.svg
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/logo/wide.svg
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/logo/with_text.svg
+-rw-r--r--   0        0        0    31715 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/samples/countries.csv
+-rw-r--r--   0        0        0   420013 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/samples/indicators.csv
+-rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 itables-2.1.0rc3/src/itables/samples/population.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/conftest.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/test_changelog.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/test_connected_notebook_is_small.py
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/test_datatables_format.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/test_documentation_notebooks_run.py
+-rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/test_downsample.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/test_extension_arguments.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/test_html_in_table_header.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/test_init.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/test_javascript.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/test_json_dumps.py
+-rw-r--r--   0        0        0   791362 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/test_notebook.ipynb
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/test_pandas_style.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/test_polars.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/test_sample_dfs.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/test_sample_python_apps.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/test_update_samples.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/sample_python_apps/itables_in_a_shiny_app.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 itables-2.1.0rc3/tests/sample_python_apps/itables_in_a_shiny_app_with_tabs.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 itables-2.1.0rc3/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 itables-2.1.0rc3/LICENSE
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 itables-2.1.0rc3/README.md
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 itables-2.1.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 itables-2.1.0rc3/PKG-INFO
```

### Comparing `itables-2.1.0rc2/.pre-commit-config.yaml` & `itables-2.1.0rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/.github/workflows/comment-pr.yml` & `itables-2.1.0rc3/.github/workflows/comment-pr.yml`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/.github/workflows/continuous-integration.yml` & `itables-2.1.0rc3/.github/workflows/continuous-integration.yml`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/.github/workflows/publish-book.yml` & `itables-2.1.0rc3/.github/workflows/publish-book.yml`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/.github/workflows/publish.yml` & `itables-2.1.0rc3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/_toc.yml` & `itables-2.1.0rc3/docs/_toc.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 format: jb-book
 root: quick_start
 parts:
-  - caption: How to use DataTables
+  - caption: ITables in Notebooks
     chapters:
     - file: advanced_parameters
-    - file: formatting
     - file: custom_css
+    - file: formatting
+    - file: pandas_style
     - file: extensions
     - file: custom_extensions
-  - caption: ITables
+    - file: quarto
+    - file: downsampling
+    - file: references
+    - file: supported_editors
+  - caption: ITables in Applications
+    chapters:
+      - file: html_export
+      - file: dash
+      - file: shiny
+      - file: streamlit
+      - file: ipywidgets
+  - caption: Contributing to ITables
     chapters:
-      - file: supported_editors
-      - file: quarto
-      - file: downsampling
-      - file: references
       - file: contributing
       - file: developing
       - file: troubleshooting
       - file: changelog
   - caption: Example DataFrames
     chapters:
     - file: sample_dataframes
     - file: polars_dataframes
-    - file: pandas_style
```

### Comparing `itables-2.1.0rc2/docs/advanced_parameters.md` & `itables-2.1.0rc3/docs/advanced_parameters.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     format_version: 0.13
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
-# The DataTables Arguments
+# Advanced Parameters
 
 ITables is a wrapper for the Javascript [DataTables](https://datatables.net/) library, which has a great [documentation](https://datatables.net/), a huge collection of [examples](https://datatables.net/examples/index), and a useful [forum](https://datatables.net/forums/).
 
 Below we give a series of examples of how the DataTables examples can be ported to Python with `itables`.
 
 As always, we initialize the `itables` library with
```

### Comparing `itables-2.1.0rc2/docs/changelog.md` & `itables-2.1.0rc3/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/custom_css.md` & `itables-2.1.0rc3/docs/custom_css.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     format_version: 0.13
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
-# Styling
+# Table Style and CSS
 
 As usual, we initialize ITables with `init_notebook_mode`, and we create two sample DataFrames:
 
 ```{code-cell}
 :tags: [hide-input]
 
 import pandas as pd
@@ -109,15 +109,15 @@
 
 (style)=
 ## The style argument
 
 The `show` function has a `style` argument that determines the
 style for that particular table.
 
-The default value for `style` is `table-layout:auto;width:auto;margin:auto;caption-side:bottom`.
+The default value for `style` is `"table-layout:auto;width:auto;margin:auto;caption-side:bottom"`. When `scrollX` is `True`, `margin:auto` gets replaced with `margin:0` to avoid misaligned headers.
 Without `width:auto`, tables with few columns still take the full notebook width in Jupyter.
 Using `margin:auto` makes non-wide tables centered in Jupyter.
 
 ## Position and width
 
 You can set a specific width or position for a table using with the `style` argument of the show function:
```

### Comparing `itables-2.1.0rc2/docs/custom_extensions.md` & `itables-2.1.0rc3/docs/custom_extensions.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/developing.md` & `itables-2.1.0rc3/docs/developing.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/df_example.png` & `itables-2.1.0rc3/docs/df_example.png`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/downsampling.md` & `itables-2.1.0rc3/docs/downsampling.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/extensions.md` & `itables-2.1.0rc3/docs/extensions.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     format_version: 0.13
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
-# DataTables Extensions
+# Download Buttons and Other Extensions
 
 DataTables comes with a series of [extensions](https://datatables.net/extensions/), which are supported by ITables since v2.0.
 A selection of these extensions are included in ITables.
 
 As usual, we activate ITables with:
 
 ```{code-cell}
@@ -99,14 +99,19 @@
         {"extend": "csvHtml5", "title": "Countries"},
         {"extend": "excelHtml5", "title": "Countries"},
     ],
 )
 ```
 
 ```{warning}
+At the moment, the CSV and Excel buttons don't work well with large tables in some browsers.
+Please subscribe to [#251](https://github.com/mwouts/itables/issues/251) if you wish to receive updates on this.
+```
+
+```{warning}
 The PDF button is not included in ITables' DataTable bundle. This is because the required PDF libraries
 have a large footprint on the bundle size. Still, you can add it to your custom bundle, see the next chapter.
 ```
 
 ## SearchPanes
 
 [SearchPanes](https://datatables.net/extensions/searchpanes/) is an extension that lets you select rows based on
```

### Comparing `itables-2.1.0rc2/docs/formatting.md` & `itables-2.1.0rc3/docs/formatting.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     format_version: 0.13
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
-# Formatting
+# Cell Formatting
 
 ## Formatting with Pandas
 
 `itables` builds the HTML representation of your Pandas dataframes using Pandas itself, so
 you can use [Pandas' formatting options](https://pandas.pydata.org/pandas-docs/stable/user_guide/options.html).
 For instance, you can change the precision used to display floating numbers:
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 --- jupytext: formats: md:myst notebook_metadata_filter: -
 jupytext.text_representation.jupytext_version text_representation: extension:
 .md format_name: myst format_version: 0.13 kernelspec: display_name: itables
-language: python name: itables --- # Formatting ## Formatting with Pandas
+language: python name: itables --- # Cell Formatting ## Formatting with Pandas
 `itables` builds the HTML representation of your Pandas dataframes using Pandas
 itself, so you can use [Pandas' formatting options](https://pandas.pydata.org/
 pandas-docs/stable/user_guide/options.html). For instance, you can change the
 precision used to display floating numbers: ```{code-cell} from itables import
 init_notebook_mode, show from itables.sample_dfs import get_countries
 init_notebook_mode(all_interactive=True) ``` ```{code-cell} import math import
 pandas as pd with pd.option_context("display.float_format", "{:,.2f}".format):
```

### Comparing `itables-2.1.0rc2/docs/pandas_style.md` & `itables-2.1.0rc3/docs/pandas_style.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,19 +8,34 @@
     format_version: 0.13
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
-# Pandas Style examples
+# Using Pandas Style
 
 Starting with `itables>=1.6.0`, ITables provides support for
 [Pandas Style](https://pandas.pydata.org/docs/user_guide/style.html).
 
+```{note}
+Unlike Pandas or Polar DataFrames, `Styler` objects are rendered directly using their
+`to_html` method, rather than passing the underlying table data to the DataTables
+library.
+
+Because of this, the rendering of the table might differ slightly from the rendering of the
+corresponding DataFrame. In particular,
+- The downsampling is not available - please pay attention to the size of the table being rendered
+- Sorting of numbers will not work if the column contains NaNs.
+```
+
+```{warning}
+Pandas Style objects can't be used with the [Streamlit extension](streamlit.md) for ITables.
+```
+
 ```{code-cell}
 import numpy as np
 import pandas as pd
 
 from itables import init_notebook_mode
 
 init_notebook_mode(all_interactive=True)
@@ -79,18 +94,7 @@
         "sin": ["The sinus of {:.6f} is {:.6f}".format(t, np.sin(t)) for t in x],
         "cos": ["The cosinus of {:.6f} is {:.6f}".format(t, np.cos(t)) for t in x],
     },
     index=df.index,
 )
 s.set_tooltips(ttips).set_caption("With tooltips")
 ```
-
-```{note}
-Unlike Pandas or Polar DataFrames, `Styler` objects are rendered directly using their
-`to_html` method, rather than passing the underlying table data to the DataTables
-library.
-
-Because of this, the rendering of the table might differ slightly from the rendering of the
-corresponding DataFrame. In particular,
-- The downsampling is not available - please pay attention to the size of the table being rendered
-- Sorting of numbers will not work if the column contains NaNs.
-```
```

### Comparing `itables-2.1.0rc2/docs/polars_dataframes.md` & `itables-2.1.0rc3/docs/polars_dataframes.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/quick_start.md` & `itables-2.1.0rc3/docs/quick_start.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 ![CI](https://github.com/mwouts/itables/actions/workflows/continuous-integration.yml/badge.svg?branch=main)
 [![codecov.io](https://codecov.io/github/mwouts/itables/coverage.svg?branch=main)](https://codecov.io/github/mwouts/itables?branch=main)
 [![Pypi](https://img.shields.io/pypi/v/itables.svg)](https://pypi.python.org/pypi/itables)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/itables.svg)](https://anaconda.org/conda-forge/itables)
 [![pyversions](https://img.shields.io/pypi/pyversions/itables.svg)](https://pypi.python.org/pypi/itables)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-<a class="github-button" href="https://github.com/mwouts/itables" data-icon="octicon-star" data-show-count="true" aria-label="Star mwouts/itables on GitHub">Star</a>
-<script async defer src="https://buttons.github.io/buttons.js"></script>
+<a class="github-button" href="https://github.com/mwouts/itables" data-icon="octicon-star" data-show-count="true"></a>
+<script src="https://buttons.github.io/buttons.js"></script>
 
 This packages changes how Pandas and Polars DataFrames are rendered in Jupyter Notebooks.
 With `itables` you can display your tables as interactive [DataTables](https://datatables.net/)
 that you can sort, paginate, scroll or filter.
 
 ITables is just about how tables are displayed. You can turn it on and off in just two lines,
 with no other impact on your data workflow.
@@ -45,17 +45,17 @@
 ```
 
 or
 ```shell
 conda install itables -c conda-forge
 ```
 
-## Activate ITables
+## Activate ITables in a Notebook
 
-Activate the interactive mode for all series and dataframes with
+Activate the interactive mode in notebook-like environment with `init_notebook_mode`:
 
 ```{code-cell}
 from itables import init_notebook_mode
 
 init_notebook_mode(all_interactive=True)
 ```
 
@@ -66,14 +66,24 @@
 ```{code-cell}
 from itables.sample_dfs import get_countries
 
 df = get_countries(html=False)
 df
 ```
 
+If you prefer to render only certain tables using `itables`, or want
+to pass [advanced parameters](advanced_parameters.md) along with the
+DataFrame, use `show`:
+
+```{code-cell}
+from itables import show
+
+show(df, lengthMenu=[2, 5, 10, 25, 50, 100, 250])
+```
+
 ## Offline mode versus connected mode
 
 ITables use two Javascript libraries:
 [jQuery](https://jquery.com/) and [DataTables](https://datatables.net/).
 
 By default `itables` works offline. No internet connection is required
 as the two libraries are embedded into the notebook itself
@@ -81,21 +91,10 @@
 
 In some contexts (Jupyter Book, Jupyter Colab, etc...) you might
 prefer to load the libraries dynamically from the internet.
 To do so, add the argument `connected=True` when you
 execute `init_notebook_mode`. This will also make your notebook lighter by
 about [700kB](https://github.com/mwouts/itables/blob/main/tests/test_connected_notebook_is_small.py).
 
-## Using ITables for specific tables only
-
-If you prefer to render only certain series or dataframes using `itables`,
-then call `init_notebook_mode(all_interactive=False)` then `show`:
-
-```{code-cell}
-from itables import show
-
-show(df, lengthMenu=[2, 5, 10, 25, 50, 100, 250])
-```
-
 ## Try ITables on Binder
 
-You can run our examples notebooks directly on [![Lab](https://img.shields.io/badge/Binder-JupyterLab-blue.svg)](https://mybinder.org/v2/gh/mwouts/itables/main?urlpath=lab/tree/docs/quick_start.md), without having to install anything on your side.
+You can run the examples above (or any other documentation page) directly on ![Lab](https://img.shields.io/badge/Binder-JupyterLab-blue.svg), without having to install anything on your end - just click on the rocket icon at the top of the page.
```

#### html2text {}

```diff
@@ -7,40 +7,41 @@
 github/mwouts/itables/coverage.svg?branch=main)](https://codecov.io/github/
 mwouts/itables?branch=main) [![Pypi](https://img.shields.io/pypi/v/
 itables.svg)](https://pypi.python.org/pypi/itables) [![Conda Version](https://
 img.shields.io/conda/vn/conda-forge/itables.svg)](https://anaconda.org/conda-
 forge/itables) [![pyversions](https://img.shields.io/pypi/pyversions/
 itables.svg)](https://pypi.python.org/pypi/itables) [![Code style: black]
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
-github.com/psf/black) _S_t_a_r
+github.com/psf/black)
 This packages changes how Pandas and Polars DataFrames are rendered in Jupyter
 Notebooks. With `itables` you can display your tables as interactive
 [DataTables](https://datatables.net/) that you can sort, paginate, scroll or
 filter. ITables is just about how tables are displayed. You can turn it on and
 off in just two lines, with no other impact on your data workflow. The
 `itables` package depends only on `numpy`, `pandas` and `IPython` which you
 must already have if you work with Pandas in Jupyter (add `polars`, `pyarrow`
 if you work with Polars DataFrames). # Quick Start ## Installation Install the
 `itables` package with either ```shell pip install itables ``` or ```shell
-conda install itables -c conda-forge ``` ## Activate ITables Activate the
-interactive mode for all series and dataframes with ```{code-cell} from itables
-import init_notebook_mode init_notebook_mode(all_interactive=True) ``` After
-this, any Pandas or Polars DataFrame, or Series, is displayed as an interactive
-[DataTables](https://datatables.net/), which lets you explore, filter or sort
-your data. ```{code-cell} from itables.sample_dfs import get_countries df =
-get_countries(html=False) df ``` ## Offline mode versus connected mode ITables
-use two Javascript libraries: [jQuery](https://jquery.com/) and [DataTables]
-(https://datatables.net/). By default `itables` works offline. No internet
-connection is required as the two libraries are embedded into the notebook
-itself when you execute `init_notebook_mode`. In some contexts (Jupyter Book,
-Jupyter Colab, etc...) you might prefer to load the libraries dynamically from
-the internet. To do so, add the argument `connected=True` when you execute
-`init_notebook_mode`. This will also make your notebook lighter by about
-[700kB](https://github.com/mwouts/itables/blob/main/tests/
-test_connected_notebook_is_small.py). ## Using ITables for specific tables only
-If you prefer to render only certain series or dataframes using `itables`, then
-call `init_notebook_mode(all_interactive=False)` then `show`: ```{code-cell}
-from itables import show show(df, lengthMenu=[2, 5, 10, 25, 50, 100, 250]) ```
-## Try ITables on Binder You can run our examples notebooks directly on [![Lab]
-(https://img.shields.io/badge/Binder-JupyterLab-blue.svg)](https://
-mybinder.org/v2/gh/mwouts/itables/main?urlpath=lab/tree/docs/quick_start.md),
-without having to install anything on your side.
+conda install itables -c conda-forge ``` ## Activate ITables in a Notebook
+Activate the interactive mode in notebook-like environment with
+`init_notebook_mode`: ```{code-cell} from itables import init_notebook_mode
+init_notebook_mode(all_interactive=True) ``` After this, any Pandas or Polars
+DataFrame, or Series, is displayed as an interactive [DataTables](https://
+datatables.net/), which lets you explore, filter or sort your data. ```{code-
+cell} from itables.sample_dfs import get_countries df = get_countries
+(html=False) df ``` If you prefer to render only certain tables using
+`itables`, or want to pass [advanced parameters](advanced_parameters.md) along
+with the DataFrame, use `show`: ```{code-cell} from itables import show show
+(df, lengthMenu=[2, 5, 10, 25, 50, 100, 250]) ``` ## Offline mode versus
+connected mode ITables use two Javascript libraries: [jQuery](https://
+jquery.com/) and [DataTables](https://datatables.net/). By default `itables`
+works offline. No internet connection is required as the two libraries are
+embedded into the notebook itself when you execute `init_notebook_mode`. In
+some contexts (Jupyter Book, Jupyter Colab, etc...) you might prefer to load
+the libraries dynamically from the internet. To do so, add the argument
+`connected=True` when you execute `init_notebook_mode`. This will also make
+your notebook lighter by about [700kB](https://github.com/mwouts/itables/blob/
+main/tests/test_connected_notebook_is_small.py). ## Try ITables on Binder You
+can run the examples above (or any other documentation page) directly on ![Lab]
+(https://img.shields.io/badge/Binder-JupyterLab-blue.svg), without having to
+install anything on your end - just click on the rocket icon at the top of the
+page.
```

### Comparing `itables-2.1.0rc2/docs/references.md` & `itables-2.1.0rc3/docs/references.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/sample_dataframes.md` & `itables-2.1.0rc3/docs/sample_dataframes.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/show_df.png` & `itables-2.1.0rc3/docs/show_df.png`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/supported_editors.md` & `itables-2.1.0rc3/docs/supported_editors.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Supported Editors
 
-`itables` has been tested in many development environments.
+ITables has been tested in the following environments
 
 ## Jupyter Notebook
 
 Try it on [![Notebook](https://img.shields.io/badge/Binder-JupyterNotebook-blue.svg)](https://mybinder.org/v2/gh/mwouts/itables/main?filepath=docs/quick_start.md)
 
 ![](images/notebook.png)
 
@@ -44,33 +44,7 @@
 ![](images/pycharm.png)
 
 ## Quarto
 
 ITables works well with Quarto - check out our `html` and `revealjs` [examples](quarto.md).
 
 <iframe src=quarto_revealjs.html width="750px" height="500px"></iframe>
-
-# Exporting a DataFrame to an HTML table
-
-To get the HTML representation of a Pandas DataFrame `df` as an interactive [DataTable](https://datatables.net/), you can use `to_html_datatable` as below:
-```python
-from itables import to_html_datatable
-from itables.sample_dfs import get_countries
-
-df = get_countries()
-html = to_html_datatable(df)
-```
-
-# Using ITables in Shiny
-
-You can use ITables in Web applications generated with [Shiny](https://shiny.rstudio.com/py/) for Python with e.g.
-```python
-from shiny import ui
-
-from itables.shiny import DT
-
-ui.HTML(DT(df))
-```
-
-See also our [tested examples](https://github.com/mwouts/itables/tree/main/tests/sample_python_apps).
-
-ITables won't work in Dash because jQuery is not usable in Dash (see the [Dash FAQ](https://dash.plotly.com/faqs)).
```

### Comparing `itables-2.1.0rc2/docs/troubleshooting.md` & `itables-2.1.0rc3/docs/troubleshooting.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,16 @@
   display_name: itables
   language: python
   name: itables
 ---
 
 # Troubleshooting
 
+## Loading takes forever?
+
 ```{code-cell}
 :tags: [hide-input]
 
 import pandas as pd
 
 from itables import show
 
@@ -36,21 +38,25 @@
 
 ```{tip}
 If you change the value of the `connected` argument in
 the `init_notebook_mode` cell, you need to re-execute all the cells
 that display interactive tables.
 ```
 
+## Trust your notebook
+
 It could also be that your notebook is not _trusted_. This happens when you
 have not run the notebook in full yourself (e.g. the notebook was sent to you with outputs,
 or the notebook was created by a tool like `papermill`). In that case, JavaScript
 code cannot run (and the interactive tables won't display)
 until you tell Jupyter that you trust the notebook content
 (run "Trust Notebook" in View / Activate Command Palette).
 
+## Check ITables' version
+
 If the above does not help, please check out the [ChangeLog](changelog.md)
 and decide whether you should upgrade `itables`. You can tell the version
 of ITables that you are using by looking at the loading message (from ITables v2.0.1 on)
 or by running this code snippet:
 ```python
 import itables as it
```

### Comparing `itables-2.1.0rc2/docs/images/code.png` & `itables-2.1.0rc3/docs/images/code.png`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/images/colab.png` & `itables-2.1.0rc3/docs/images/colab.png`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/images/html.png` & `itables-2.1.0rc3/docs/images/html.png`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/images/lab.png` & `itables-2.1.0rc3/docs/images/lab.png`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/images/notebook.png` & `itables-2.1.0rc3/docs/images/notebook.png`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/images/pycharm.png` & `itables-2.1.0rc3/docs/images/pycharm.png`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/quarto/quarto_html.qmd` & `itables-2.1.0rc3/docs/quarto/quarto_html.qmd`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/docs/quarto/quarto_revealjs.qmd` & `itables-2.1.0rc3/docs/quarto/quarto_revealjs.qmd`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/packages/dt_for_itables/LICENSE` & `itables-2.1.0rc3/packages/dt_for_itables/LICENSE`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/packages/dt_for_itables/README.md` & `itables-2.1.0rc3/packages/dt_for_itables/README.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/packages/dt_for_itables/package-lock.json` & `itables-2.1.0rc3/packages/dt_for_itables/package-lock.json`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/packages/dt_for_itables/package.json` & `itables-2.1.0rc3/packages/dt_for_itables/package.json`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/packages/dt_for_itables/src/index.js` & `itables-2.1.0rc3/packages/dt_for_itables/src/index.js`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/packages/itables_for_streamlit/package-lock.json` & `itables-2.1.0rc3/packages/itables_for_streamlit/package-lock.json`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/packages/itables_for_streamlit/package.json` & `itables-2.1.0rc3/packages/itables_for_streamlit/package.json`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/packages/itables_for_streamlit/src/index.tsx` & `itables-2.1.0rc3/packages/itables_for_streamlit/src/index.tsx`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/datatables_format.py` & `itables-2.1.0rc3/src/itables/datatables_format.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/downsample.py` & `itables-2.1.0rc3/src/itables/downsample.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/javascript.py` & `itables-2.1.0rc3/src/itables/javascript.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,16 @@
 
     display(HTML(read_package_file("html/init_datatables.html")))
 
     if not connected:
         display(HTML(generate_init_offline_itables_html(dt_bundle)))
 
 
-def get_animated_logo():
-    if not opt.display_logo_when_loading:
+def get_animated_logo(display_logo_when_loading):
+    if not display_logo_when_loading:
         return ""
     return f"""<div style="float:left; margin-right: 10px;">
 <a href=https://mwouts.github.io/itables/>{read_package_file("logo/loading.svg")}</a>
 </div>
 """
 
 
@@ -132,28 +132,37 @@
     dt_css = dt_bundle.with_suffix(".css").read_text()
     dt64 = b64encode(dt_src.encode("utf-8")).decode("ascii")
 
     id = "itables_init_notebook_mode_" + str(uuid.uuid4()).replace("-", "_")
 
     return f"""<style>{dt_css}</style>
 <div id="{id}" style="vertical-align:middle; text-align:left">
-{get_animated_logo()}<div>
+{get_animated_logo(opt.display_logo_when_loading)}<div>
 This is the <code>init_notebook_mode</code> cell from ITables v{itables_version}<br>
 (you should not see this message - is your notebook <it>trusted</it>?)
 </div>
 </div>
 <script>
 window.{DATATABLES_SRC_FOR_ITABLES} = "data:text/javascript;base64,{dt64}";
 document.querySelectorAll("#{id}").forEach(e => e.remove());
 </script>
 """
 
 
 def _table_header(
-    df, table_id, show_index, classes, style, tags, footer, column_filters, connected
+    df,
+    table_id,
+    show_index,
+    classes,
+    style,
+    tags,
+    footer,
+    column_filters,
+    connected,
+    display_logo_when_loading,
 ):
     """This function returns the HTML table header. Rows are not included."""
     # Generate table head using pandas.to_html(), see issue 63
     pattern = re.compile(r".*<thead>(.*)</thead>", flags=re.MULTILINE | re.DOTALL)
     try:
         html_header = df.head(0).to_html(escape=False)
     except AttributeError:
@@ -166,15 +175,15 @@
         thead = thead.replace("<th></th>", "", 1)
 
     itables_source = (
         "the internet" if connected else "the <code>init_notebook_mode</code> cell"
     )
     tbody = f"""<tr>
 <td style="vertical-align:middle; text-align:left">
-{get_animated_logo()}<div>
+{get_animated_logo(display_logo_when_loading)}<div>
 Loading ITables v{itables_version} from {itables_source}...
 (need <a href=https://mwouts.github.io/itables/troubleshooting.html>help</a>?)</td>
 </div>
 </tr>"""
 
     if style:
         style = 'style="{}"'.format(style)
@@ -398,15 +407,24 @@
         try:
             df = df.set_index(pd.RangeIndex(len(df.index)))
         except AttributeError:
             # Polars DataFrames
             pass
 
     table_header = _table_header(
-        df, tableId, showIndex, classes, style, tags, footer, column_filters, connected
+        df,
+        tableId,
+        showIndex,
+        classes,
+        style,
+        tags,
+        footer,
+        column_filters,
+        connected=connected,
+        display_logo_when_loading=kwargs.pop("display_logo_when_loading"),
     )
 
     # Export the table data to JSON and include this in the HTML
     if showIndex:
         df = safe_reset_index(df)
 
     # When the header has an extra column, we add
@@ -439,39 +457,42 @@
 
     if isinstance(values, list):
         for i, value in enumerate(values):
             _raise_if_javascript_code(value, f"{context}/{i}")
         return
 
 
-def get_itables_extension_arguments(df, caption=None, **kwargs):
+def get_itables_extension_arguments(df, caption=None, scrollX=True, **kwargs):
     """
     This function returns two dictionaries that are JSON
     serializable and can be passed to the itables extensions.
     The first dict contains the arguments to be passed to the
     DataTable constructor, while the second one contains other
     parameters to be used outside of the constructor.
     """
     # Pandas style objects are not supported
     if pd_style is not None and isinstance(df, pd_style.Styler):
         raise NotImplementedError(
             "Pandas style objects can't be used with the extension"
         )
 
+    kwargs["scrollX"] = scrollX
+
     set_default_options(
         kwargs,
         use_to_html=False,
         context="the streamlit extension",
         not_available=[
             "tags",
             "dt_url",
             "pre_dt_code",
             "use_to_html",
             "footer",
             "column_filters",
+            "display_logo_when_loading",
         ],
     )
 
     # Javascript code is not supported in the extension
     _raise_if_javascript_code(kwargs)
 
     # These options are used here, not in DataTable
@@ -592,20 +613,23 @@
             and (not use_to_html or (option not in _OPTIONS_NOT_AVAILABLE_WITH_TO_HTML))
             and option not in kwargs
             and not option.startswith("__")
             and option
             not in {
                 "dt_bundle",
                 "find_package_file",
-                "display_logo_when_loading",
                 "UNPKG_DT_BUNDLE_URL",
             }
         ):
             kwargs[option] = getattr(opt, option)
 
+    if kwargs.get("scrollX", False):
+        # column headers are misaligned if we let margin:auto
+        kwargs["style"] = kwargs["style"].replace(";margin:auto;", ";margin:0;")
+
     for name, value in kwargs.items():
         if value is None:
             raise ValueError(
                 "Please don't pass an option with a value equal to None ('{}=None')".format(
                     name
                 )
             )
```

### Comparing `itables-2.1.0rc2/src/itables/options.py` & `itables-2.1.0rc3/src/itables/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,18 @@
 """Default DataTables classes. See https://datatables.net/manual/styling/classes"""
 classes = "display nowrap"
 
 """Default table style. Use
 - 'table-layout:auto' to compute the layout automatically
 - 'width:auto' to fit the table width to its content
 - 'margin:auto' to center the table.
-Combine multiple options using ';'."""
+Combine multiple options using ';'.
+
+NB: When scrollX=true, the default is changed to "margin:0;caption-side:bottom"
+"""
 style = "table-layout:auto;width:auto;margin:auto;caption-side:bottom"
 
 """Additional tags like e.g. caption"""
 tags = ""
 
 """Maximum bytes before downsampling a table"""
 maxBytes = "64KB"
```

### Comparing `itables-2.1.0rc2/src/itables/sample_dfs.py` & `itables-2.1.0rc3/src/itables/sample_dfs.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/utils.py` & `itables-2.1.0rc3/src/itables/utils.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/html/datatables_template.html` & `itables-2.1.0rc3/src/itables/html/datatables_template.html`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/html/dt_bundle.css` & `itables-2.1.0rc3/src/itables/html/dt_bundle.css`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/html/dt_bundle.js` & `itables-2.1.0rc3/src/itables/html/dt_bundle.js`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/itables_for_streamlit/static/css/main.45cd49da.css` & `itables-2.1.0rc3/src/itables/itables_for_streamlit/static/css/main.45cd49da.css`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/itables_for_streamlit/static/css/main.45cd49da.css.map` & `itables-2.1.0rc3/src/itables/itables_for_streamlit/static/css/main.45cd49da.css.map`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/itables_for_streamlit/static/js/main.b98e79fb.js` & `itables-2.1.0rc3/src/itables/itables_for_streamlit/static/js/main.b98e79fb.js`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/itables_for_streamlit/static/js/main.b98e79fb.js.LICENSE.txt` & `itables-2.1.0rc3/src/itables/itables_for_streamlit/static/js/main.b98e79fb.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/itables_for_streamlit/static/js/main.b98e79fb.js.map` & `itables-2.1.0rc3/src/itables/itables_for_streamlit/static/js/main.b98e79fb.js.map`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/logo/loading.svg` & `itables-2.1.0rc3/src/itables/logo/loading.svg`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/logo/logo.svg` & `itables-2.1.0rc3/src/itables/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/logo/text.svg` & `itables-2.1.0rc3/src/itables/logo/text.svg`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/logo/wide.svg` & `itables-2.1.0rc3/src/itables/logo/wide.svg`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/logo/with_text.svg` & `itables-2.1.0rc3/src/itables/logo/with_text.svg`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/samples/countries.csv` & `itables-2.1.0rc3/src/itables/samples/countries.csv`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/samples/indicators.csv` & `itables-2.1.0rc3/src/itables/samples/indicators.csv`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/src/itables/samples/population.csv` & `itables-2.1.0rc3/src/itables/samples/population.csv`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/tests/conftest.py` & `itables-2.1.0rc3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/tests/test_changelog.py` & `itables-2.1.0rc3/tests/test_changelog.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/tests/test_connected_notebook_is_small.py` & `itables-2.1.0rc3/tests/test_connected_notebook_is_small.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/tests/test_datatables_format.py` & `itables-2.1.0rc3/tests/test_datatables_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         show_index=False,
         classes="",
         style="",
         tags="",
         footer=False,
         column_filters=False,
         connected=False,
+        display_logo_when_loading=False,
     )
     column_count = _column_count_in_header(table_header)
     actual = datatables_rows(df, count=column_count)
     if isinstance(expected, str):
         assert actual == expected
     else:
         assert actual == json.dumps(expected)
```

### Comparing `itables-2.1.0rc2/tests/test_documentation_notebooks_run.py` & `itables-2.1.0rc3/tests/test_documentation_notebooks_run.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/tests/test_downsample.py` & `itables-2.1.0rc3/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/tests/test_extension_arguments.py` & `itables-2.1.0rc3/tests/test_extension_arguments.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,21 @@
 
 def test_get_itables_extension_arguments(df):
     try:
         ext_args = get_itables_extension_arguments(df)
     except NotImplementedError as e:
         pytest.skip(str(e))
 
-    assert set(ext_args["dt_args"]) <= {"data", "columns", "layout", "order"}, set(
-        ext_args["dt_args"]
-    )
+    assert set(ext_args["dt_args"]) <= {
+        "data",
+        "columns",
+        "layout",
+        "order",
+        "scrollX",
+    }, set(ext_args["dt_args"])
     assert isinstance(ext_args["dt_args"]["data"], list)
     assert isinstance(ext_args["dt_args"]["columns"], list)
 
     assert set(ext_args["other_args"]) <= {
         "classes",
         "style",
         "caption",
```

### Comparing `itables-2.1.0rc2/tests/test_javascript.py` & `itables-2.1.0rc3/tests/test_javascript.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/tests/test_json_dumps.py` & `itables-2.1.0rc3/tests/test_json_dumps.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/tests/test_notebook.ipynb` & `itables-2.1.0rc3/tests/test_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/tests/test_pandas_style.py` & `itables-2.1.0rc3/tests/test_pandas_style.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/tests/test_polars.py` & `itables-2.1.0rc3/tests/test_polars.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/tests/test_sample_dfs.py` & `itables-2.1.0rc3/tests/test_sample_dfs.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/tests/test_sample_python_apps.py` & `itables-2.1.0rc3/tests/test_sample_python_apps.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/tests/test_update_samples.py` & `itables-2.1.0rc3/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/LICENSE` & `itables-2.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/README.md` & `itables-2.1.0rc3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -52,17 +52,16 @@
 Thanks to this the interactive tables will work even without a connection to the internet.
 
 If you prefer to load the libraries dynamically (and keep the notebook lighter), use `connected=True` when you
 execute `init_notebook_mode`.
 
 ## Supported environments
 
-`itables` has been tested in the following editors:
-- Jupyter Notebook
-- Jupyter Lab
-- Jupyter nbconvert (i.e. the tables are still interactive in the HTML export of a notebook)
-- Jupyter Book
-- Google Colab
-- VS Code (for both Jupyter Notebooks and Python scripts)
-- PyCharm (for Jupyter Notebooks)
-- Quarto
-- Shiny for Python
+ITables works in all the usual Jupyter Notebook environments, including Jupyter Notebook, Jupyter Lab, Jupyter nbconvert (i.e. the tables are still interactive in the HTML export of a notebook), Jupyter Book, Google Colab and Kaggle.
+
+You can also use ITables in [Quarto](https://mwouts.github.io/itables/quarto.html) HTML documents, and in RISE presentations.
+
+ITables works well in VS Code, both in Jupyter Notebooks and in interactive Python sessions.
+
+Last but not least, ITables is also available in
+[Streamlit](https://mwouts.github.io/itables/streamlit.html) or
+[Shiny](https://mwouts.github.io/itables/shiny.html) applications.
```

### Comparing `itables-2.1.0rc2/pyproject.toml` & `itables-2.1.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc2/PKG-INFO` & `itables-2.1.0rc3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: itables
-Version: 2.1.0rc2
+Version: 2.1.0rc3
 Summary: Pandas and Polar DataFrames as interactive DataTables
 Project-URL: Homepage, https://mwouts.github.io/itables/
 Project-URL: Documentation, https://mwouts.github.io/itables
 Project-URL: Repository, https://github.com/mwouts/itables.git
 Project-URL: Issues, https://github.com/mwouts/itables/issues
 Project-URL: Changelog, https://github.com/mwouts/itables/blob/main/docs/changelog.md
 Author-email: Marc Wouts <marc.wouts@gmail.com>
@@ -132,17 +132,16 @@
 Thanks to this the interactive tables will work even without a connection to the internet.
 
 If you prefer to load the libraries dynamically (and keep the notebook lighter), use `connected=True` when you
 execute `init_notebook_mode`.
 
 ## Supported environments
 
-`itables` has been tested in the following editors:
-- Jupyter Notebook
-- Jupyter Lab
-- Jupyter nbconvert (i.e. the tables are still interactive in the HTML export of a notebook)
-- Jupyter Book
-- Google Colab
-- VS Code (for both Jupyter Notebooks and Python scripts)
-- PyCharm (for Jupyter Notebooks)
-- Quarto
-- Shiny for Python
+ITables works in all the usual Jupyter Notebook environments, including Jupyter Notebook, Jupyter Lab, Jupyter nbconvert (i.e. the tables are still interactive in the HTML export of a notebook), Jupyter Book, Google Colab and Kaggle.
+
+You can also use ITables in [Quarto](https://mwouts.github.io/itables/quarto.html) HTML documents, and in RISE presentations.
+
+ITables works well in VS Code, both in Jupyter Notebooks and in interactive Python sessions.
+
+Last but not least, ITables is also available in
+[Streamlit](https://mwouts.github.io/itables/streamlit.html) or
+[Shiny](https://mwouts.github.io/itables/shiny.html) applications.
```

