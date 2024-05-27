# Comparing `tmp/itables-2.1.0rc1.tar.gz` & `tmp/itables-2.1.0rc2.tar.gz`

## Comparing `itables-2.1.0rc1.tar` & `itables-2.1.0rc2.tar`

### file list

```diff
@@ -1,105 +1,112 @@
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 itables-2.1.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 itables-2.1.0rc1/.pylintrc
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 itables-2.1.0rc1/codecov.yml
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 itables-2.1.0rc1/environment.yml
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 itables-2.1.0rc1/.github/workflows/comment-pr.yml
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 itables-2.1.0rc1/.github/workflows/continuous-integration.yml
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 itables-2.1.0rc1/.github/workflows/publish-book.yml
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 itables-2.1.0rc1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 itables-2.1.0rc1/binder/postBuild
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 itables-2.1.0rc1/binder/requirements.txt
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 itables-2.1.0rc1/binder/labconfig/default_setting_overrides.json
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/_config.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/_toc.yml
--rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/advanced_parameters.md
--rw-r--r--   0        0        0    18588 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/changelog.md
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/contributing.md
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/custom_css.md
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/custom_extensions.md
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/developing.md
--rw-r--r--   0        0        0    46135 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/df_example.png
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/downsampling.md
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/extensions.md
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/formatting.md
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/pandas_style.md
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/polars_dataframes.md
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/quarto.md
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/quick_start.md
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/references.md
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/sample_dataframes.md
--rw-r--r--   0        0        0    51851 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/show_df.png
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/supported_editors.md
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/troubleshooting.md
--rw-r--r--   0        0        0    83555 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/images/code.png
--rw-r--r--   0        0        0    98830 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/images/colab.png
--rw-r--r--   0        0        0   110756 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/images/html.png
--rw-r--r--   0        0        0   108275 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/images/lab.png
--rw-r--r--   0        0        0   129198 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/images/notebook.png
--rw-r--r--   0        0        0   107743 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/images/pycharm.png
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/quarto/quarto_html.qmd
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/quarto/quarto_revealjs.qmd
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/package-lock.json
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/package.json
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/dt_for_itables/CHANGELOG.md
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/dt_for_itables/LICENSE
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/dt_for_itables/README.md
--rw-r--r--   0        0        0    23839 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/dt_for_itables/package-lock.json
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/dt_for_itables/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/dt_for_itables/src/index.d.ts
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/dt_for_itables/src/index.js
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/itables_for_streamlit/README.md
--rw-r--r--   0        0        0   708765 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/itables_for_streamlit/package-lock.json
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/itables_for_streamlit/package.json
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/itables_for_streamlit/tsconfig.json
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/itables_for_streamlit/public/index.html
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/itables_for_streamlit/src/index.tsx
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/__init__.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/datatables_format.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/downsample.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/interactive.py
--rw-r--r--   0        0        0    27476 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/javascript.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/options.py
--rw-r--r--   0        0        0    13926 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/sample_dfs.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/shiny.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/streamlit.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/utils.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/version.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/html/datatables_template.html
--rw-r--r--   0        0        0    68898 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/html/dt_bundle.css
--rw-r--r--   0        0        0   505946 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/html/dt_bundle.js
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/html/init_datatables.html
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/html/column_filters/initComplete.js
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/html/column_filters/pre_dt_code.js
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/logo/loading.svg
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/logo/logo.svg
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/logo/text.svg
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/logo/wide.svg
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/logo/with_text.svg
--rw-r--r--   0        0        0    31715 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/samples/countries.csv
--rw-r--r--   0        0        0   420013 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/samples/indicators.csv
--rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/samples/population.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/conftest.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_changelog.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_connected_notebook_is_small.py
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_datatables_format.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_documentation_notebooks_run.py
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_downsample.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_extension_arguments.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_html_in_table_header.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_init.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_javascript.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_json_dumps.py
--rw-r--r--   0        0        0   791362 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_notebook.ipynb
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_pandas_style.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_polars.py
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_sample_dfs.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_sample_python_apps.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_update_samples.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/sample_python_apps/itables_in_a_shiny_app.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/sample_python_apps/itables_in_a_shiny_app_with_tabs.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 itables-2.1.0rc1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 itables-2.1.0rc1/LICENSE
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 itables-2.1.0rc1/README.md
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 itables-2.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 itables-2.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 itables-2.1.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 itables-2.1.0rc2/.pylintrc
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 itables-2.1.0rc2/codecov.yml
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 itables-2.1.0rc2/environment.yml
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 itables-2.1.0rc2/.github/workflows/comment-pr.yml
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 itables-2.1.0rc2/.github/workflows/continuous-integration.yml
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 itables-2.1.0rc2/.github/workflows/publish-book.yml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 itables-2.1.0rc2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 itables-2.1.0rc2/binder/postBuild
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 itables-2.1.0rc2/binder/requirements.txt
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 itables-2.1.0rc2/binder/labconfig/default_setting_overrides.json
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/_config.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/_toc.yml
+-rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/advanced_parameters.md
+-rw-r--r--   0        0        0    18588 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/changelog.md
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/contributing.md
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/custom_css.md
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/custom_extensions.md
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/developing.md
+-rw-r--r--   0        0        0    46135 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/df_example.png
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/downsampling.md
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/extensions.md
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/formatting.md
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/pandas_style.md
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/polars_dataframes.md
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/quarto.md
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/quick_start.md
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/references.md
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/sample_dataframes.md
+-rw-r--r--   0        0        0    51851 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/show_df.png
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/supported_editors.md
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/troubleshooting.md
+-rw-r--r--   0        0        0    83555 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/images/code.png
+-rw-r--r--   0        0        0    98830 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/images/colab.png
+-rw-r--r--   0        0        0   110756 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/images/html.png
+-rw-r--r--   0        0        0   108275 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/images/lab.png
+-rw-r--r--   0        0        0   129198 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/images/notebook.png
+-rw-r--r--   0        0        0   107743 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/images/pycharm.png
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/quarto/quarto_html.qmd
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 itables-2.1.0rc2/docs/quarto/quarto_revealjs.qmd
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/package-lock.json
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/package.json
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/dt_for_itables/CHANGELOG.md
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/dt_for_itables/LICENSE
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/dt_for_itables/README.md
+-rw-r--r--   0        0        0    23839 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/dt_for_itables/package-lock.json
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/dt_for_itables/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/dt_for_itables/src/index.d.ts
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/dt_for_itables/src/index.js
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/itables_for_streamlit/README.md
+-rw-r--r--   0        0        0   708765 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/itables_for_streamlit/package-lock.json
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/itables_for_streamlit/package.json
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/itables_for_streamlit/tsconfig.json
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/itables_for_streamlit/public/index.html
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 itables-2.1.0rc2/packages/itables_for_streamlit/src/index.tsx
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/__init__.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/datatables_format.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/downsample.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/interactive.py
+-rw-r--r--   0        0        0    27476 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/javascript.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/options.py
+-rw-r--r--   0        0        0    13926 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/sample_dfs.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/shiny.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/streamlit.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/utils.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/version.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/html/datatables_template.html
+-rw-r--r--   0        0        0    68898 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/html/dt_bundle.css
+-rw-r--r--   0        0        0   505946 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/html/dt_bundle.js
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/html/init_datatables.html
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/html/column_filters/initComplete.js
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/html/column_filters/pre_dt_code.js
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/itables_for_streamlit/asset-manifest.json
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/itables_for_streamlit/index.html
+-rw-r--r--   0        0        0    71691 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/itables_for_streamlit/static/css/main.45cd49da.css
+-rw-r--r--   0        0        0   152195 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/itables_for_streamlit/static/css/main.45cd49da.css.map
+-rw-r--r--   0        0        0   689965 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/itables_for_streamlit/static/js/main.b98e79fb.js
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/itables_for_streamlit/static/js/main.b98e79fb.js.LICENSE.txt
+-rw-r--r--   0        0        0  3051380 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/itables_for_streamlit/static/js/main.b98e79fb.js.map
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/logo/loading.svg
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/logo/logo.svg
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/logo/text.svg
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/logo/wide.svg
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/logo/with_text.svg
+-rw-r--r--   0        0        0    31715 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/samples/countries.csv
+-rw-r--r--   0        0        0   420013 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/samples/indicators.csv
+-rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 itables-2.1.0rc2/src/itables/samples/population.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/conftest.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_changelog.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_connected_notebook_is_small.py
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_datatables_format.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_documentation_notebooks_run.py
+-rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_downsample.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_extension_arguments.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_html_in_table_header.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_init.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_javascript.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_json_dumps.py
+-rw-r--r--   0        0        0   791362 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_notebook.ipynb
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_pandas_style.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_polars.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_sample_dfs.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_sample_python_apps.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/test_update_samples.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/sample_python_apps/itables_in_a_shiny_app.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 itables-2.1.0rc2/tests/sample_python_apps/itables_in_a_shiny_app_with_tabs.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 itables-2.1.0rc2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 itables-2.1.0rc2/LICENSE
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 itables-2.1.0rc2/README.md
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 itables-2.1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 itables-2.1.0rc2/PKG-INFO
```

### Comparing `itables-2.1.0rc1/.pre-commit-config.yaml` & `itables-2.1.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/.github/workflows/comment-pr.yml` & `itables-2.1.0rc2/.github/workflows/comment-pr.yml`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/.github/workflows/continuous-integration.yml` & `itables-2.1.0rc2/.github/workflows/continuous-integration.yml`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/.github/workflows/publish-book.yml` & `itables-2.1.0rc2/.github/workflows/publish-book.yml`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/.github/workflows/publish.yml` & `itables-2.1.0rc2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/_toc.yml` & `itables-2.1.0rc2/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/advanced_parameters.md` & `itables-2.1.0rc2/docs/advanced_parameters.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/changelog.md` & `itables-2.1.0rc2/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/contributing.md` & `itables-2.1.0rc2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/custom_css.md` & `itables-2.1.0rc2/docs/custom_css.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/custom_extensions.md` & `itables-2.1.0rc2/docs/custom_extensions.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/developing.md` & `itables-2.1.0rc2/docs/developing.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/df_example.png` & `itables-2.1.0rc2/docs/df_example.png`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/downsampling.md` & `itables-2.1.0rc2/docs/downsampling.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/extensions.md` & `itables-2.1.0rc2/docs/extensions.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/formatting.md` & `itables-2.1.0rc2/docs/formatting.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/pandas_style.md` & `itables-2.1.0rc2/docs/pandas_style.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/polars_dataframes.md` & `itables-2.1.0rc2/docs/polars_dataframes.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/quarto.md` & `itables-2.1.0rc2/docs/quarto.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/quick_start.md` & `itables-2.1.0rc2/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/references.md` & `itables-2.1.0rc2/docs/references.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/sample_dataframes.md` & `itables-2.1.0rc2/docs/sample_dataframes.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/show_df.png` & `itables-2.1.0rc2/docs/show_df.png`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/supported_editors.md` & `itables-2.1.0rc2/docs/supported_editors.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/troubleshooting.md` & `itables-2.1.0rc2/docs/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/images/code.png` & `itables-2.1.0rc2/docs/images/code.png`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/images/colab.png` & `itables-2.1.0rc2/docs/images/colab.png`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/images/html.png` & `itables-2.1.0rc2/docs/images/html.png`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/images/lab.png` & `itables-2.1.0rc2/docs/images/lab.png`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/images/notebook.png` & `itables-2.1.0rc2/docs/images/notebook.png`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/images/pycharm.png` & `itables-2.1.0rc2/docs/images/pycharm.png`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/quarto/quarto_html.qmd` & `itables-2.1.0rc2/docs/quarto/quarto_html.qmd`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/docs/quarto/quarto_revealjs.qmd` & `itables-2.1.0rc2/docs/quarto/quarto_revealjs.qmd`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/packages/dt_for_itables/LICENSE` & `itables-2.1.0rc2/packages/dt_for_itables/LICENSE`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/packages/dt_for_itables/README.md` & `itables-2.1.0rc2/packages/dt_for_itables/README.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/packages/dt_for_itables/package-lock.json` & `itables-2.1.0rc2/packages/dt_for_itables/package-lock.json`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/packages/dt_for_itables/package.json` & `itables-2.1.0rc2/packages/dt_for_itables/package.json`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/packages/dt_for_itables/src/index.js` & `itables-2.1.0rc2/packages/dt_for_itables/src/index.js`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/packages/itables_for_streamlit/package-lock.json` & `itables-2.1.0rc2/packages/itables_for_streamlit/package-lock.json`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/packages/itables_for_streamlit/package.json` & `itables-2.1.0rc2/packages/itables_for_streamlit/package.json`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/packages/itables_for_streamlit/src/index.tsx` & `itables-2.1.0rc2/packages/itables_for_streamlit/src/index.tsx`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/datatables_format.py` & `itables-2.1.0rc2/src/itables/datatables_format.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/downsample.py` & `itables-2.1.0rc2/src/itables/downsample.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/javascript.py` & `itables-2.1.0rc2/src/itables/javascript.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/options.py` & `itables-2.1.0rc2/src/itables/options.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/sample_dfs.py` & `itables-2.1.0rc2/src/itables/sample_dfs.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/utils.py` & `itables-2.1.0rc2/src/itables/utils.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/html/datatables_template.html` & `itables-2.1.0rc2/src/itables/html/datatables_template.html`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/html/dt_bundle.css` & `itables-2.1.0rc2/src/itables/html/dt_bundle.css`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/html/dt_bundle.js` & `itables-2.1.0rc2/src/itables/html/dt_bundle.js`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/logo/loading.svg` & `itables-2.1.0rc2/src/itables/logo/loading.svg`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/logo/logo.svg` & `itables-2.1.0rc2/src/itables/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/logo/text.svg` & `itables-2.1.0rc2/src/itables/logo/text.svg`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/logo/wide.svg` & `itables-2.1.0rc2/src/itables/logo/wide.svg`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/logo/with_text.svg` & `itables-2.1.0rc2/src/itables/logo/with_text.svg`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/samples/countries.csv` & `itables-2.1.0rc2/src/itables/samples/countries.csv`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/samples/indicators.csv` & `itables-2.1.0rc2/src/itables/samples/indicators.csv`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/src/itables/samples/population.csv` & `itables-2.1.0rc2/src/itables/samples/population.csv`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/tests/conftest.py` & `itables-2.1.0rc2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/tests/test_changelog.py` & `itables-2.1.0rc2/tests/test_changelog.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/tests/test_connected_notebook_is_small.py` & `itables-2.1.0rc2/tests/test_connected_notebook_is_small.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/tests/test_datatables_format.py` & `itables-2.1.0rc2/tests/test_datatables_format.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/tests/test_documentation_notebooks_run.py` & `itables-2.1.0rc2/tests/test_documentation_notebooks_run.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/tests/test_downsample.py` & `itables-2.1.0rc2/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/tests/test_extension_arguments.py` & `itables-2.1.0rc2/tests/test_extension_arguments.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/tests/test_javascript.py` & `itables-2.1.0rc2/tests/test_javascript.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/tests/test_json_dumps.py` & `itables-2.1.0rc2/tests/test_json_dumps.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/tests/test_notebook.ipynb` & `itables-2.1.0rc2/tests/test_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/tests/test_pandas_style.py` & `itables-2.1.0rc2/tests/test_pandas_style.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/tests/test_polars.py` & `itables-2.1.0rc2/tests/test_polars.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/tests/test_sample_dfs.py` & `itables-2.1.0rc2/tests/test_sample_dfs.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/tests/test_sample_python_apps.py` & `itables-2.1.0rc2/tests/test_sample_python_apps.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/tests/test_update_samples.py` & `itables-2.1.0rc2/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/LICENSE` & `itables-2.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/README.md` & `itables-2.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `itables-2.1.0rc1/pyproject.toml` & `itables-2.1.0rc2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -84,11 +84,11 @@
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
 path = "packages"
 build_cmd = "build"
 npm = ["npm"]
 
 [tool.hatch.build.targets.sdist]
-artifacts = ["src/itables/html/dt_bundle.js", "src/itables/html/dt_bundle.css"]
+artifacts = ["src/itables/html/dt_bundle.js", "src/itables/html/dt_bundle.css", "src/itables/itables_for_streamlit/*"]
 
 [tool.hatch.build.targets.wheel]
-artifacts = ["src/itables/html/dt_bundle.js", "src/itables/html/dt_bundle.css"]
+artifacts = ["src/itables/html/dt_bundle.js", "src/itables/html/dt_bundle.css", "src/itables/itables_for_streamlit/*"]
```

### Comparing `itables-2.1.0rc1/PKG-INFO` & `itables-2.1.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: itables
-Version: 2.1.0rc1
+Version: 2.1.0rc2
 Summary: Pandas and Polar DataFrames as interactive DataTables
 Project-URL: Homepage, https://mwouts.github.io/itables/
 Project-URL: Documentation, https://mwouts.github.io/itables
 Project-URL: Repository, https://github.com/mwouts/itables.git
 Project-URL: Issues, https://github.com/mwouts/itables/issues
 Project-URL: Changelog, https://github.com/mwouts/itables/blob/main/docs/changelog.md
 Author-email: Marc Wouts <marc.wouts@gmail.com>
```

