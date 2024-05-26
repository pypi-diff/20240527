# Comparing `tmp/itables-2.0.1.tar.gz` & `tmp/itables-2.1.0rc1.tar.gz`

## Comparing `itables-2.0.1.tar` & `itables-2.1.0rc1.tar`

### file list

```diff
@@ -1,93 +1,105 @@
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 itables-2.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 itables-2.0.1/.pylintrc
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 itables-2.0.1/codecov.yml
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 itables-2.0.1/environment.yml
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 itables-2.0.1/.github/workflows/comment-pr.yml
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 itables-2.0.1/.github/workflows/continuous-integration.yml
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 itables-2.0.1/.github/workflows/publish-book.yml
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 itables-2.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 itables-2.0.1/binder/postBuild
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 itables-2.0.1/binder/requirements.txt
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 itables-2.0.1/binder/labconfig/default_setting_overrides.json
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 itables-2.0.1/docs/_config.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 itables-2.0.1/docs/_toc.yml
--rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 itables-2.0.1/docs/advanced_parameters.md
--rw-r--r--   0        0        0    17944 2020-02-02 00:00:00.000000 itables-2.0.1/docs/changelog.md
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 itables-2.0.1/docs/contributing.md
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 itables-2.0.1/docs/custom_css.md
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 itables-2.0.1/docs/custom_extensions.md
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 itables-2.0.1/docs/developing.md
--rw-r--r--   0        0        0    46135 2020-02-02 00:00:00.000000 itables-2.0.1/docs/df_example.png
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 itables-2.0.1/docs/downsampling.md
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 itables-2.0.1/docs/extensions.md
--rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 itables-2.0.1/docs/formatting.md
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 itables-2.0.1/docs/pandas_style.md
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 itables-2.0.1/docs/polars_dataframes.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 itables-2.0.1/docs/quarto.md
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 itables-2.0.1/docs/quick_start.md
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 itables-2.0.1/docs/references.md
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 itables-2.0.1/docs/sample_dataframes.md
--rw-r--r--   0        0        0    51851 2020-02-02 00:00:00.000000 itables-2.0.1/docs/show_df.png
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 itables-2.0.1/docs/supported_editors.md
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 itables-2.0.1/docs/troubleshooting.md
--rw-r--r--   0        0        0    83555 2020-02-02 00:00:00.000000 itables-2.0.1/docs/images/code.png
--rw-r--r--   0        0        0    98830 2020-02-02 00:00:00.000000 itables-2.0.1/docs/images/colab.png
--rw-r--r--   0        0        0   110756 2020-02-02 00:00:00.000000 itables-2.0.1/docs/images/html.png
--rw-r--r--   0        0        0   108275 2020-02-02 00:00:00.000000 itables-2.0.1/docs/images/lab.png
--rw-r--r--   0        0        0   129198 2020-02-02 00:00:00.000000 itables-2.0.1/docs/images/notebook.png
--rw-r--r--   0        0        0   107743 2020-02-02 00:00:00.000000 itables-2.0.1/docs/images/pycharm.png
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 itables-2.0.1/docs/quarto/quarto_html.qmd
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 itables-2.0.1/docs/quarto/quarto_revealjs.qmd
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 itables-2.0.1/itables/__init__.py
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 itables-2.0.1/itables/datatables_format.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 itables-2.0.1/itables/downsample.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 itables-2.0.1/itables/interactive.py
--rw-r--r--   0        0        0    23228 2020-02-02 00:00:00.000000 itables-2.0.1/itables/javascript.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 itables-2.0.1/itables/options.py
--rw-r--r--   0        0        0    13910 2020-02-02 00:00:00.000000 itables-2.0.1/itables/sample_dfs.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 itables-2.0.1/itables/shiny.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 itables-2.0.1/itables/utils.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 itables-2.0.1/itables/version.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 itables-2.0.1/itables/dt_for_itables/LICENSE
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 itables-2.0.1/itables/dt_for_itables/README.md
--rw-r--r--   0        0        0    68898 2020-02-02 00:00:00.000000 itables-2.0.1/itables/dt_for_itables/dt_bundle.css
--rw-r--r--   0        0        0   505621 2020-02-02 00:00:00.000000 itables-2.0.1/itables/dt_for_itables/dt_bundle.js
--rw-r--r--   0        0        0    23839 2020-02-02 00:00:00.000000 itables-2.0.1/itables/dt_for_itables/package-lock.json
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 itables-2.0.1/itables/dt_for_itables/package.json
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 itables-2.0.1/itables/dt_for_itables/src.js
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 itables-2.0.1/itables/html/datatables_template.html
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 itables-2.0.1/itables/html/init_datatables.html
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 itables-2.0.1/itables/html/column_filters/initComplete.js
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 itables-2.0.1/itables/html/column_filters/pre_dt_code.js
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 itables-2.0.1/itables/logo/loading.svg
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 itables-2.0.1/itables/logo/logo.svg
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 itables-2.0.1/itables/logo/text.svg
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 itables-2.0.1/itables/logo/wide.svg
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 itables-2.0.1/itables/logo/with_text.svg
--rw-r--r--   0        0        0    31715 2020-02-02 00:00:00.000000 itables-2.0.1/itables/samples/countries.csv
--rw-r--r--   0        0        0   420013 2020-02-02 00:00:00.000000 itables-2.0.1/itables/samples/indicators.csv
--rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 itables-2.0.1/itables/samples/population.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itables-2.0.1/tests/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 itables-2.0.1/tests/conftest.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 itables-2.0.1/tests/test_changelog.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 itables-2.0.1/tests/test_connected_notebook_is_small.py
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 itables-2.0.1/tests/test_datatables_format.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 itables-2.0.1/tests/test_documentation_notebooks_run.py
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 itables-2.0.1/tests/test_downsample.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 itables-2.0.1/tests/test_html_in_table_header.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 itables-2.0.1/tests/test_init.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 itables-2.0.1/tests/test_javascript.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 itables-2.0.1/tests/test_json_dumps.py
--rw-r--r--   0        0        0   791362 2020-02-02 00:00:00.000000 itables-2.0.1/tests/test_notebook.ipynb
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 itables-2.0.1/tests/test_pandas_style.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 itables-2.0.1/tests/test_polars.py
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 itables-2.0.1/tests/test_sample_dfs.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 itables-2.0.1/tests/test_sample_python_apps.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 itables-2.0.1/tests/test_update_samples.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 itables-2.0.1/tests/sample_python_apps/itables_in_a_shiny_app.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 itables-2.0.1/tests/sample_python_apps/itables_in_a_shiny_app_with_tabs.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 itables-2.0.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 itables-2.0.1/LICENSE
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 itables-2.0.1/README.md
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 itables-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     6518 2020-02-02 00:00:00.000000 itables-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 itables-2.1.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 itables-2.1.0rc1/.pylintrc
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 itables-2.1.0rc1/codecov.yml
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 itables-2.1.0rc1/environment.yml
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 itables-2.1.0rc1/.github/workflows/comment-pr.yml
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 itables-2.1.0rc1/.github/workflows/continuous-integration.yml
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 itables-2.1.0rc1/.github/workflows/publish-book.yml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 itables-2.1.0rc1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 itables-2.1.0rc1/binder/postBuild
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 itables-2.1.0rc1/binder/requirements.txt
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 itables-2.1.0rc1/binder/labconfig/default_setting_overrides.json
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/_config.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/_toc.yml
+-rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/advanced_parameters.md
+-rw-r--r--   0        0        0    18588 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/changelog.md
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/contributing.md
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/custom_css.md
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/custom_extensions.md
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/developing.md
+-rw-r--r--   0        0        0    46135 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/df_example.png
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/downsampling.md
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/extensions.md
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/formatting.md
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/pandas_style.md
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/polars_dataframes.md
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/quarto.md
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/quick_start.md
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/references.md
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/sample_dataframes.md
+-rw-r--r--   0        0        0    51851 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/show_df.png
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/supported_editors.md
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/troubleshooting.md
+-rw-r--r--   0        0        0    83555 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/images/code.png
+-rw-r--r--   0        0        0    98830 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/images/colab.png
+-rw-r--r--   0        0        0   110756 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/images/html.png
+-rw-r--r--   0        0        0   108275 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/images/lab.png
+-rw-r--r--   0        0        0   129198 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/images/notebook.png
+-rw-r--r--   0        0        0   107743 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/images/pycharm.png
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/quarto/quarto_html.qmd
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 itables-2.1.0rc1/docs/quarto/quarto_revealjs.qmd
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/package-lock.json
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/package.json
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/dt_for_itables/CHANGELOG.md
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/dt_for_itables/LICENSE
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/dt_for_itables/README.md
+-rw-r--r--   0        0        0    23839 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/dt_for_itables/package-lock.json
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/dt_for_itables/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/dt_for_itables/src/index.d.ts
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/dt_for_itables/src/index.js
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/itables_for_streamlit/README.md
+-rw-r--r--   0        0        0   708765 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/itables_for_streamlit/package-lock.json
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/itables_for_streamlit/package.json
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/itables_for_streamlit/tsconfig.json
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/itables_for_streamlit/public/index.html
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 itables-2.1.0rc1/packages/itables_for_streamlit/src/index.tsx
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/__init__.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/datatables_format.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/downsample.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/interactive.py
+-rw-r--r--   0        0        0    27476 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/javascript.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/options.py
+-rw-r--r--   0        0        0    13926 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/sample_dfs.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/shiny.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/streamlit.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/utils.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/version.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/html/datatables_template.html
+-rw-r--r--   0        0        0    68898 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/html/dt_bundle.css
+-rw-r--r--   0        0        0   505946 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/html/dt_bundle.js
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/html/init_datatables.html
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/html/column_filters/initComplete.js
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/html/column_filters/pre_dt_code.js
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/logo/loading.svg
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/logo/logo.svg
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/logo/text.svg
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/logo/wide.svg
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/logo/with_text.svg
+-rw-r--r--   0        0        0    31715 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/samples/countries.csv
+-rw-r--r--   0        0        0   420013 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/samples/indicators.csv
+-rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 itables-2.1.0rc1/src/itables/samples/population.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_changelog.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_connected_notebook_is_small.py
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_datatables_format.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_documentation_notebooks_run.py
+-rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_downsample.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_extension_arguments.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_html_in_table_header.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_init.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_javascript.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_json_dumps.py
+-rw-r--r--   0        0        0   791362 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_notebook.ipynb
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_pandas_style.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_polars.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_sample_dfs.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_sample_python_apps.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/test_update_samples.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/sample_python_apps/itables_in_a_shiny_app.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 itables-2.1.0rc1/tests/sample_python_apps/itables_in_a_shiny_app_with_tabs.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 itables-2.1.0rc1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 itables-2.1.0rc1/LICENSE
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 itables-2.1.0rc1/README.md
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 itables-2.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 itables-2.1.0rc1/PKG-INFO
```

### Comparing `itables-2.0.1/.pre-commit-config.yaml` & `itables-2.1.0rc1/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # Install pre-commit hooks via
 # pre-commit install
 
 repos:
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
     - id: check-json
     - id: check-yaml
     - id: end-of-file-fixer
     - id: trailing-whitespace
 
   - repo: https://github.com/timothycrosley/isort
     rev: 5.13.2
     hooks:
     - id: isort
       args: ["--profile", "black", "--filter-files"]
 
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 24.4.2
     hooks:
     - id: black
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.1
+    rev: v0.4.5
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/mwouts/jupytext
-    rev: v1.14.5
+    rev: v1.16.2
     hooks:
     - id: jupytext
       exclude: dt_for_itables/
       types: ["markdown"]
       args: ["--pipe", "isort {} --treat-comment-as-code '# %%' --profile black", "--pipe", "black", "--check", "ruff check {} --ignore E402"]
       additional_dependencies:
-        - black==22.3.0 # Matches hook
-        - ruff==0.3.1
+        - black==24.4.2 # Matches hook
+        - ruff==0.4.3
         - isort==5.13.2
```

### Comparing `itables-2.0.1/.github/workflows/comment-pr.yml` & `itables-2.1.0rc1/.github/workflows/comment-pr.yml`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/.github/workflows/continuous-integration.yml` & `itables-2.1.0rc1/.github/workflows/continuous-integration.yml`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/.github/workflows/publish-book.yml` & `itables-2.1.0rc1/.github/workflows/publish-book.yml`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/.github/workflows/publish.yml` & `itables-2.1.0rc1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/docs/_toc.yml` & `itables-2.1.0rc1/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/docs/advanced_parameters.md` & `itables-2.1.0rc1/docs/advanced_parameters.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 jupytext:
   formats: md:myst
+  notebook_metadata_filter: -jupytext.text_representation.jupytext_version
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.5
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
 # The DataTables Arguments
```

### Comparing `itables-2.0.1/docs/changelog.md` & `itables-2.1.0rc1/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 ITables ChangeLog
 =================
 
+2.1.0-dev (2024-05-??)
+------------------
+
+**Changed**
+- ITables now uses the `src` layout ([#246](https://github.com/mwouts/itables/issues/246)) - many thanks to [Mahendra Paipuri](https://github.com/mahendrapaipuri) for his help on this topic!
+- We have updated `dt_for_itables`' dependencies to `datatables.net-dt==2.0.7` and `datatables.net-select-dt==2.0.2` ([#273](https://github.com/mwouts/itables/pull/273))
+- We have updated the pre-commit hooks used in the project ([#268](https://github.com/mwouts/itables/pull/268))
+
+**Added**
+- We have added a streamlit component for ITables ([#270](https://github.com/mwouts/itables/pull/270))
+
+
 2.0.1 (2024-04-30)
 ------------------
 
 **Added**
 - We have added a logo for ITables ([#257](https://github.com/mwouts/itables/issues/257))
 - The _loading_ message gives more information, including the version of ITables and where DataTables is loaded from ([#258](https://github.com/mwouts/itables/issues/258))
```

### Comparing `itables-2.0.1/docs/contributing.md` & `itables-2.1.0rc1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/docs/custom_css.md` & `itables-2.1.0rc1/docs/custom_css.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 jupytext:
   formats: md:myst
+  notebook_metadata_filter: -jupytext.text_representation.jupytext_version
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.5
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
 # Styling
```

### Comparing `itables-2.0.1/docs/custom_extensions.md` & `itables-2.1.0rc1/docs/custom_extensions.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 jupytext:
   formats: md:myst
+  notebook_metadata_filter: -jupytext.text_representation.jupytext_version
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.5
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
 # Custom Extensions
@@ -49,26 +49,34 @@
 
 ## Creating a custom DataTables bundle
 
 To use custom extensions in the offline mode, you will need
 to create a bundle of jQuery, DataTables, and the desired extensions.
 
 To do so, make a copy of
-[`itables/dt_for_itables`](https://github.com/mwouts/itables/tree/main/itables/dt_for_itables):
+[`packages/dt_for_itables`](https://github.com/mwouts/itables/tree/main/packages/dt_for_itables):
 ```bash
-$ ls itables/dt_for_itables/
-package.json  package-lock.json  README.md  src.js
+$ tree
+```
+```
+.
+├── LICENSE
+├── package.json
+├── package-lock.json
+├── README.md
+└── src
+    └── index.js
 ```
 
-Add or remove the desired extensions in `package.json` and `src.js`. To do this,
+Add or remove the desired extensions in `package.json` and `src/index.js`. To do this,
 you can use the [DataTables download](https://datatables.net/download/) page and
 follow the instructions for the _NPM_ download method.
 
 For instance, say you want to bundle the PDF export button. Change
-`src.js` to this code:
+`src/index.js` to this code:
 ```javascript
 import JSZip from 'jszip';
 import jQuery from 'jquery';
 import pdfMake from 'pdfmake';
 import DataTable from 'datatables.net-dt';
 import 'datatables.net-dt/css/dataTables.dataTables.min.css';
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `itables-2.0.1/docs/developing.md` & `itables-2.1.0rc1/docs/developing.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/docs/df_example.png` & `itables-2.1.0rc1/docs/df_example.png`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/docs/downsampling.md` & `itables-2.1.0rc1/docs/downsampling.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 jupytext:
   formats: md:myst
+  notebook_metadata_filter: -jupytext.text_representation.jupytext_version
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.5
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
 # Downsampling
```

### Comparing `itables-2.0.1/docs/extensions.md` & `itables-2.1.0rc1/docs/extensions.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 jupytext:
   formats: md:myst
+  notebook_metadata_filter: -jupytext.text_representation.jupytext_version
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.5
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
 # DataTables Extensions
```

### Comparing `itables-2.0.1/docs/formatting.md` & `itables-2.1.0rc1/docs/formatting.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 jupytext:
   formats: md:myst
+  notebook_metadata_filter: -jupytext.text_representation.jupytext_version
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.5
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
 # Formatting
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
---- jupytext: formats: md:myst text_representation: extension: .md format_name:
-myst format_version: 0.13 jupytext_version: 1.14.5 kernelspec: display_name:
-itables language: python name: itables --- # Formatting ## Formatting with
-Pandas `itables` builds the HTML representation of your Pandas dataframes using
-Pandas itself, so you can use [Pandas' formatting options](https://
-pandas.pydata.org/pandas-docs/stable/user_guide/options.html). For instance,
-you can change the precision used to display floating numbers: ```{code-cell}
-from itables import init_notebook_mode, show from itables.sample_dfs import
-get_countries init_notebook_mode(all_interactive=True) ``` ```{code-cell}
-import math import pandas as pd with pd.option_context("display.float_format",
-"{:,.2f}".format): show(pd.Series([i * math.pi for i in range(1, 6)])) ``` Or
-you can use a custom formatter: ```{code-cell} with pd.option_context
-("display.float_format", "${:,.2f}".format): show(pd.Series([i * math.pi for i
-in range(1, 6)])) ``` ## Formatting with Javascript Numbers are formatted using
-Pandas, then are converted back to float to ensure they come in the right order
-when sorted. Therefore, to achieve a particular formatting you might have to
-resort to the [`columns.render` option](https://datatables.net/examples/
-advanced_init/column_render.html) of DataTables. For instance, this [example]
-(https://datatables.net/forums/discussion/61407/how-to-apply-a-numeric-format-
-to-a-column) can be ported like this: ```{code-cell} from itables import
+--- jupytext: formats: md:myst notebook_metadata_filter: -
+jupytext.text_representation.jupytext_version text_representation: extension:
+.md format_name: myst format_version: 0.13 kernelspec: display_name: itables
+language: python name: itables --- # Formatting ## Formatting with Pandas
+`itables` builds the HTML representation of your Pandas dataframes using Pandas
+itself, so you can use [Pandas' formatting options](https://pandas.pydata.org/
+pandas-docs/stable/user_guide/options.html). For instance, you can change the
+precision used to display floating numbers: ```{code-cell} from itables import
+init_notebook_mode, show from itables.sample_dfs import get_countries
+init_notebook_mode(all_interactive=True) ``` ```{code-cell} import math import
+pandas as pd with pd.option_context("display.float_format", "{:,.2f}".format):
+show(pd.Series([i * math.pi for i in range(1, 6)])) ``` Or you can use a custom
+formatter: ```{code-cell} with pd.option_context("display.float_format", "$
+{:,.2f}".format): show(pd.Series([i * math.pi for i in range(1, 6)])) ``` ##
+Formatting with Javascript Numbers are formatted using Pandas, then are
+converted back to float to ensure they come in the right order when sorted.
+Therefore, to achieve a particular formatting you might have to resort to the
+[`columns.render` option](https://datatables.net/examples/advanced_init/
+column_render.html) of DataTables. For instance, this [example](https://
+datatables.net/forums/discussion/61407/how-to-apply-a-numeric-format-to-a-
+column) can be ported like this: ```{code-cell} from itables import
 JavascriptCode show( pd.Series([i * math.pi * 1e4 for i in range(1, 6)]),
 columnDefs=[ { "targets": "_all", "render": JavascriptCode
 ("$.fn.dataTable.render.number(',', '.', 3, '$')"), } ], ) ``` ## Colors based
 on cell values You can use Javascript callbacks to set the cell or row style
 depending on the cell content. The example below, in which we color in red the
 cells with negative numbers, is directly inspired by the corresponding
 DataTables [example](https://datatables.net/reference/option/
```

### Comparing `itables-2.0.1/docs/pandas_style.md` & `itables-2.1.0rc1/docs/pandas_style.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 jupytext:
   formats: md:myst
+  notebook_metadata_filter: -jupytext.text_representation.jupytext_version
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.5
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
 # Pandas Style examples
```

### Comparing `itables-2.0.1/docs/polars_dataframes.md` & `itables-2.1.0rc1/docs/polars_dataframes.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 jupytext:
   formats: md:myst
+  notebook_metadata_filter: -jupytext.text_representation.jupytext_version
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.5
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
 # Polars dataframes
```

### Comparing `itables-2.0.1/docs/quarto.md` & `itables-2.1.0rc1/docs/quarto.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 jupytext:
   formats: md:myst
+  notebook_metadata_filter: -jupytext.text_representation.jupytext_version
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.5
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
 # Quarto
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
---- jupytext: formats: md:myst text_representation: extension: .md format_name:
-myst format_version: 0.13 jupytext_version: 1.14.5 kernelspec: display_name:
-itables language: python name: itables --- # Quarto ITables works well with the
+--- jupytext: formats: md:myst notebook_metadata_filter: -
+jupytext.text_representation.jupytext_version text_representation: extension:
+.md format_name: myst format_version: 0.13 kernelspec: display_name: itables
+language: python name: itables --- # Quarto ITables works well with the
 `revealjs` and `html` outputs formats of [Quarto](https://quarto.org). ## HTML
 Presentations See this _r_e_v_e_a_l_j_s_ _p_r_e_s_e_n_t_a_t_i_o_n, or download the _s_o_u_r_c_e_ _f_i_l_e and
 render it with `quarto render`: ## HTML reports See this _H_T_M_L_ _r_e_p_o_r_t, or
 download the _s_o_u_r_c_e_ _f_i_l_e and render it with `quarto render`:
```

### Comparing `itables-2.0.1/docs/quick_start.md` & `itables-2.1.0rc1/docs/quick_start.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ---
 jupytext:
   formats: md:myst
+  notebook_metadata_filter: -jupytext.text_representation.jupytext_version
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.5
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
-![ITables Logo](../itables/logo/text.svg)
+![ITables Logo](../src/itables/logo/text.svg)
 
 ![CI](https://github.com/mwouts/itables/actions/workflows/continuous-integration.yml/badge.svg?branch=main)
 [![codecov.io](https://codecov.io/github/mwouts/itables/coverage.svg?branch=main)](https://codecov.io/github/mwouts/itables?branch=main)
 [![Pypi](https://img.shields.io/pypi/v/itables.svg)](https://pypi.python.org/pypi/itables)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/itables.svg)](https://anaconda.org/conda-forge/itables)
 [![pyversions](https://img.shields.io/pypi/pyversions/itables.svg)](https://pypi.python.org/pypi/itables)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
---- jupytext: formats: md:myst text_representation: extension: .md format_name:
-myst format_version: 0.13 jupytext_version: 1.14.5 kernelspec: display_name:
-itables language: python name: itables --- ![ITables Logo](../itables/logo/
+--- jupytext: formats: md:myst notebook_metadata_filter: -
+jupytext.text_representation.jupytext_version text_representation: extension:
+.md format_name: myst format_version: 0.13 kernelspec: display_name: itables
+language: python name: itables --- ![ITables Logo](../src/itables/logo/
 text.svg) ![CI](https://github.com/mwouts/itables/actions/workflows/continuous-
 integration.yml/badge.svg?branch=main) [![codecov.io](https://codecov.io/
 github/mwouts/itables/coverage.svg?branch=main)](https://codecov.io/github/
 mwouts/itables?branch=main) [![Pypi](https://img.shields.io/pypi/v/
 itables.svg)](https://pypi.python.org/pypi/itables) [![Conda Version](https://
 img.shields.io/conda/vn/conda-forge/itables.svg)](https://anaconda.org/conda-
 forge/itables) [![pyversions](https://img.shields.io/pypi/pyversions/
```

### Comparing `itables-2.0.1/docs/references.md` & `itables-2.1.0rc1/docs/references.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/docs/sample_dataframes.md` & `itables-2.1.0rc1/docs/sample_dataframes.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 jupytext:
   formats: md:myst
+  notebook_metadata_filter: -jupytext.text_representation.jupytext_version
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.5
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
 # Sample dataframes
```

### Comparing `itables-2.0.1/docs/show_df.png` & `itables-2.1.0rc1/docs/show_df.png`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/docs/supported_editors.md` & `itables-2.1.0rc1/docs/supported_editors.md`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/docs/troubleshooting.md` & `itables-2.1.0rc1/docs/troubleshooting.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 jupytext:
   formats: md:myst
+  notebook_metadata_filter: -jupytext.text_representation.jupytext_version
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.14.5
 kernelspec:
   display_name: itables
   language: python
   name: itables
 ---
 
 # Troubleshooting
```

### Comparing `itables-2.0.1/docs/images/code.png` & `itables-2.1.0rc1/docs/images/code.png`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/docs/images/colab.png` & `itables-2.1.0rc1/docs/images/colab.png`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/docs/images/html.png` & `itables-2.1.0rc1/docs/images/html.png`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/docs/images/lab.png` & `itables-2.1.0rc1/docs/images/lab.png`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/docs/images/notebook.png` & `itables-2.1.0rc1/docs/images/notebook.png`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/docs/images/pycharm.png` & `itables-2.1.0rc1/docs/images/pycharm.png`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/docs/quarto/quarto_html.qmd` & `itables-2.1.0rc1/docs/quarto/quarto_html.qmd`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/docs/quarto/quarto_revealjs.qmd` & `itables-2.1.0rc1/docs/quarto/quarto_revealjs.qmd`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/itables/datatables_format.py` & `itables-2.1.0rc1/src/itables/datatables_format.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,29 +12,34 @@
     pl = None
 
 
 JS_MAX_SAFE_INTEGER = 2**53 - 1
 JS_MIN_SAFE_INTEGER = -(2**53 - 1)
 
 
-def _format_column(x):
+def _format_column(x, pure_json=False):
     dtype_kind = x.dtype.kind
     if dtype_kind in ["b", "i", "s"]:
         return x
 
     try:
         x = fmt.format_array(x._values, None, justify="all", leading_space=False)
     except TypeError:
         # Older versions of Pandas don't have 'leading_space'
         x = fmt.format_array(x._values, None, justify="all")
     if dtype_kind == "f":
         try:
-            return np.array(x).astype(float)
+            x = np.array(x).astype(float)
         except ValueError:
             pass
+        if pure_json:
+            # While JavaScript accept these values,
+            # JSON (in the streamlit component)
+            # cannot encode non-finite float values
+            x = [f if np.isfinite(f) else str(f) for f in x]
 
     return x
 
 
 def generate_encoder(warn_on_unexpected_types=True):
     class TableValuesEncoder(json.JSONEncoder):
         def default(self, obj):
@@ -70,51 +75,61 @@
     """Older versions of Pandas don't have df.isetitem"""
     try:
         df.isetitem(i, value)
     except AttributeError:
         df.iloc[:, i] = value
 
 
-def datatables_rows(df, count=None, warn_on_unexpected_types=False):
+def datatables_rows(df, count=None, warn_on_unexpected_types=False, pure_json=False):
     """Format the values in the table and return the data, row by row, as requested by DataTables"""
     # We iterate over columns using an index rather than the column name
     # to avoid an issue in case of duplicated column names #89
     if count is None or len(df.columns) == count:
         empty_columns = []
     else:
         # When the header requires more columns (#141), we append empty columns on the left
         missing_columns = count - len(df.columns)
         assert missing_columns > 0
         empty_columns = [[None] * len(df)] * missing_columns
 
     try:
         # Pandas DataFrame
-        data = list(zip(*(empty_columns + [_format_column(x) for _, x in df.items()])))
+        data = list(
+            zip(
+                *(empty_columns + [_format_column(x, pure_json) for _, x in df.items()])
+            )
+        )
         has_bigints = any(
             x.dtype.kind == "i"
             and ((x > JS_MAX_SAFE_INTEGER).any() or (x < JS_MIN_SAFE_INTEGER).any())
             for _, x in df.items()
         )
-        js = json.dumps(data, cls=generate_encoder(warn_on_unexpected_types))
+        js = json.dumps(
+            data,
+            cls=generate_encoder(warn_on_unexpected_types),
+            allow_nan=not pure_json,
+        )
     except AttributeError:
         # Polars DataFrame
         data = list(df.iter_rows())
         import polars as pl
 
         has_bigints = any(
             x.dtype in [pl.Int64, pl.UInt64]
             and ((x > JS_MAX_SAFE_INTEGER).any() or (x < JS_MIN_SAFE_INTEGER).any())
             for x in (df[col] for col in df.columns)
         )
-        js = json.dumps(data, cls=generate_encoder(False))
+        js = json.dumps(data, cls=generate_encoder(False), allow_nan=not pure_json)
 
     if has_bigints:
-        js = n_suffix_for_bigints(js)
+        js = n_suffix_for_bigints(js, pure_json=pure_json)
 
     return js
 
 
-def n_suffix_for_bigints(js):
+def n_suffix_for_bigints(js, pure_json=False):
     def n_suffix(matchobj):
+        if pure_json:
+            return '"' + matchobj.group(1) + '"' + matchobj.group(2)
         return 'BigInt("' + matchobj.group(1) + '")' + matchobj.group(2)
 
     return re.sub(r"(-?\d{16,})(,|])", n_suffix, js)
```

### Comparing `itables-2.0.1/itables/downsample.py` & `itables-2.1.0rc1/src/itables/downsample.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/itables/javascript.py` & `itables-2.1.0rc1/src/itables/javascript.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 _OPTIONS_NOT_AVAILABLE_WITH_TO_HTML = {
     "tags",
     "footer",
     "column_filters",
     "maxBytes",
     "maxRows",
     "maxColumns",
-    "warn_on_dom",
     "warn_on_unexpected_types",
 }
 _ORIGINAL_DATAFRAME_REPR_HTML = pd.DataFrame._repr_html_
 _ORIGINAL_DATAFRAME_STYLE_REPR_HTML = (
     None if pd_style is None else pd_style.Styler._repr_html_
 )
 _ORIGINAL_POLARS_DATAFRAME_REPR_HTML = pl.DataFrame._repr_html_
@@ -301,30 +300,36 @@
     df=None,
     caption=None,
     tableId=None,
     connected=True,
     use_to_html=False,
     **kwargs,
 ):
+    """
+    Return the HTML representation of the given
+    dataframe as an interactive datatable
+    """
+
     check_table_id(tableId)
+
     if "import_jquery" in kwargs:
         raise TypeError(
             "The argument 'import_jquery' was removed in ITables v2.0. "
             "Please pass a custom 'dt_url' instead."
         )
+
     if use_to_html or (pd_style is not None and isinstance(df, pd_style.Styler)):
         return to_html_datatable_using_to_html(
             df=df,
             caption=caption,
             tableId=tableId,
             connected=connected,
             **kwargs,
         )
 
-    """Return the HTML representation of the given dataframe as an interactive datatable"""
     set_default_options(kwargs, use_to_html=False)
 
     # These options are used here, not in DataTable
     classes = kwargs.pop("classes")
     style = kwargs.pop("style")
     tags = kwargs.pop("tags")
 
@@ -362,15 +367,20 @@
     if downsampling_warning and "fnInfoCallback" not in kwargs:
         kwargs["fnInfoCallback"] = JavascriptFunction(
             "function (oSettings, iStart, iEnd, iMax, iTotal, sPre) {{ return sPre + ' ({warning})'; }}".format(
                 warning=downsampling_warning
             )
         )
 
-    _adjust_layout(df, kwargs, downsampling_warning)
+    _adjust_layout(
+        df,
+        kwargs,
+        downsampling_warning=downsampling_warning,
+        warn_on_dom=kwargs.pop("warn_on_dom"),
+    )
 
     footer = kwargs.pop("footer")
     column_filters = kwargs.pop("column_filters")
     if column_filters == "header":
         pass
     elif column_filters == "footer":
         footer = True
@@ -414,28 +424,157 @@
         data=dt_data,
         kwargs=kwargs,
         connected=connected,
         column_filters=column_filters,
     )
 
 
+def _raise_if_javascript_code(values, context=""):
+    if isinstance(values, (JavascriptCode, JavascriptFunction)):
+        raise TypeError(f"Javascript code can't be passed to the extension: {context}")
+
+    if isinstance(values, dict):
+        for key, value in values.items():
+            _raise_if_javascript_code(value, f"{context}/{key}")
+        return
+
+    if isinstance(values, list):
+        for i, value in enumerate(values):
+            _raise_if_javascript_code(value, f"{context}/{i}")
+        return
+
+
+def get_itables_extension_arguments(df, caption=None, **kwargs):
+    """
+    This function returns two dictionaries that are JSON
+    serializable and can be passed to the itables extensions.
+    The first dict contains the arguments to be passed to the
+    DataTable constructor, while the second one contains other
+    parameters to be used outside of the constructor.
+    """
+    # Pandas style objects are not supported
+    if pd_style is not None and isinstance(df, pd_style.Styler):
+        raise NotImplementedError(
+            "Pandas style objects can't be used with the extension"
+        )
+
+    set_default_options(
+        kwargs,
+        use_to_html=False,
+        context="the streamlit extension",
+        not_available=[
+            "tags",
+            "dt_url",
+            "pre_dt_code",
+            "use_to_html",
+            "footer",
+            "column_filters",
+        ],
+    )
+
+    # Javascript code is not supported in the extension
+    _raise_if_javascript_code(kwargs)
+
+    # These options are used here, not in DataTable
+    classes = kwargs.pop("classes")
+    style = kwargs.pop("style")
+    showIndex = kwargs.pop("showIndex")
+
+    if isinstance(df, (np.ndarray, np.generic)):
+        df = pd.DataFrame(df)
+
+    if isinstance(df, (pd.Series, pl.Series)):
+        df = df.to_frame()
+
+    if showIndex == "auto":
+        try:
+            showIndex = df.index.name is not None or not isinstance(
+                df.index, pd.RangeIndex
+            )
+        except AttributeError:
+            # Polars DataFrame
+            showIndex = False
+
+    maxBytes = kwargs.pop("maxBytes", 0)
+    maxRows = kwargs.pop("maxRows", 0)
+    maxColumns = kwargs.pop("maxColumns", pd.get_option("display.max_columns") or 0)
+    warn_on_unexpected_types = kwargs.pop("warn_on_unexpected_types", False)
+
+    df, downsampling_warning = downsample(
+        df, max_rows=maxRows, max_columns=maxColumns, max_bytes=maxBytes
+    )
+
+    _adjust_layout(
+        df,
+        kwargs,
+        downsampling_warning=downsampling_warning,
+        warn_on_dom=kwargs.pop("warn_on_dom"),
+    )
+
+    if isinstance(classes, list):
+        classes = " ".join(classes)
+
+    if not showIndex:
+        try:
+            df = df.set_index(pd.RangeIndex(len(df.index)))
+        except AttributeError:
+            # Polars DataFrames
+            pass
+
+    if showIndex:
+        df = safe_reset_index(df)
+
+    if isinstance(df.columns, pd.MultiIndex):
+        columns = [
+            {"title": "<br>".join(str(level) or "&nbsp" for level in col)}
+            for col in df.columns
+        ]
+    else:
+        columns = [{"title": str(col)} for col in df.columns]
+
+    try:
+        data_json = ""
+        data_json = datatables_rows(df, None, warn_on_unexpected_types, pure_json=True)
+        data = json.loads(data_json)
+    except (ValueError, json.JSONDecodeError) as e:
+        raise NotImplementedError(
+            f"This dataframe can't be serialized to JSON:\n{e}\n{data_json}"
+        )
+
+    return {
+        "dt_args": {"columns": columns, "data": data, **kwargs},
+        "other_args": {
+            "classes": classes,
+            "style": style,
+            "caption": caption,
+            "downsampling_warning": downsampling_warning,
+        },
+    }
+
+
 def check_table_id(table_id):
     """Make sure that the table_id is a valid HTML id.
 
     See also https://stackoverflow.com/questions/70579/html-valid-id-attribute-values
     """
     if table_id is not None:
         if not re.match(r"[A-Za-z][-A-Za-z0-9_.]*", table_id):
             raise ValueError(
                 "The id name must contain at least one character, "
                 f"cannot start with a number, and must not contain whitespaces ({table_id})"
             )
 
 
-def set_default_options(kwargs, use_to_html):
+def set_default_options(kwargs, use_to_html, context=None, not_available=()):
+    args_not_available = set(kwargs).intersection(not_available)
+    if args_not_available:
+        raise TypeError(
+            f"In the context of {context}, "
+            f"these options are not available: {args_not_available}"
+        )
     if use_to_html:
         options_not_available = set(kwargs).intersection(
             _OPTIONS_NOT_AVAILABLE_WITH_TO_HTML
         )
         if options_not_available:
             raise TypeError(
                 "These options are not available when using df.to_html: {}".format(
@@ -445,15 +584,16 @@
 
     # layout is updated using the arguments passed on to show
     kwargs["layout"] = {**getattr(opt, "layout"), **kwargs.get("layout", {})}
 
     # Default options
     for option in dir(opt):
         if (
-            (not use_to_html or (option not in _OPTIONS_NOT_AVAILABLE_WITH_TO_HTML))
+            option not in not_available
+            and (not use_to_html or (option not in _OPTIONS_NOT_AVAILABLE_WITH_TO_HTML))
             and option not in kwargs
             and not option.startswith("__")
             and option
             not in {
                 "dt_bundle",
                 "find_package_file",
                 "display_logo_when_loading",
@@ -495,15 +635,17 @@
             showIndex = df.index.name is not None or not isinstance(
                 df.index, pd.RangeIndex
             )
         except AttributeError:
             # Polars DataFrame
             showIndex = False
 
-    _adjust_layout(df, kwargs, downsampling_warning="")
+    _adjust_layout(
+        df, kwargs, downsampling_warning="", warn_on_dom=kwargs.pop("warn_on_dom")
+    )
 
     tableId = (
         tableId
         # default UUID in Pandas styler objects has uuid_len=5
         or str(uuid.uuid4())[:5]
     )
     if pd_style is not None and isinstance(df, pd_style.Styler):
@@ -658,19 +800,19 @@
 
     if isinstance(min_rows, (int, float)):
         return min_rows
 
     return min_rows[0]
 
 
-def _adjust_layout(df, kwargs, downsampling_warning):
+def _adjust_layout(df, kwargs, *, downsampling_warning, warn_on_dom):
     has_default_layout = kwargs["layout"] == DEFAULT_LAYOUT
 
     if "dom" in kwargs:
-        if opt.warn_on_dom:
+        if warn_on_dom:
             warnings.warn(
                 "The 'dom' argument has been deprecated in DataTables==2.0.",
                 DeprecationWarning,
             )
         if not has_default_layout:
             raise ValueError("You cannot pass both 'dom' and 'layout'")
         del kwargs["layout"]
```

### Comparing `itables-2.0.1/itables/options.py` & `itables-2.1.0rc1/src/itables/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,11 +57,11 @@
 """Should a warning appear when the deprecated 'dom' is used?"""
 warn_on_dom = True
 
 """The DataTables URL for the connected mode"""
 dt_url = UNPKG_DT_BUNDLE_URL
 
 """The DataTable bundle for the offline mode"""
-dt_bundle = find_package_file("dt_for_itables/dt_bundle.js")
+dt_bundle = find_package_file("html/dt_bundle.js")
 
 """Display the ITables animated logo when loading"""
 display_logo_when_loading = True
```

### Comparing `itables-2.0.1/itables/sample_dfs.py` & `itables-2.1.0rc1/src/itables/sample_dfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,19 +82,19 @@
 
 def get_df_complex_index():
     df = get_countries()
     df = df.reset_index().set_index(["region", "country"])
     df.columns = pd.MultiIndex.from_arrays(
         [
             [
-                "code"
-                if col == "code"
-                else "localisation"
-                if col in ["longitude", "latitude"]
-                else "data"
+                (
+                    "code"
+                    if col == "code"
+                    else "localisation" if col in ["longitude", "latitude"] else "data"
+                )
                 for col in df.columns
             ],
             df.columns,
         ],
         names=["category", "detail"],
     )
     return df
```

### Comparing `itables-2.0.1/itables/utils.py` & `itables-2.1.0rc1/src/itables/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from io import open
 from pathlib import Path
 
-UNPKG_DT_BUNDLE_URL = "https://www.unpkg.com/dt_for_itables@2.0.5/dt_bundle.js"
+UNPKG_DT_BUNDLE_URL = "https://www.unpkg.com/dt_for_itables@2.0.7/dt_bundle.js"
 UNPKG_DT_BUNDLE_CSS = UNPKG_DT_BUNDLE_URL.replace(".js", ".css")
 
 
 def find_package_file(*path):
     """Return the full path to a file from the itables package"""
     current_path = Path(__file__).parent
     return Path(current_path, *path)
```

### Comparing `itables-2.0.1/itables/dt_for_itables/LICENSE` & `itables-2.1.0rc1/packages/dt_for_itables/LICENSE`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/itables/dt_for_itables/README.md` & `itables-2.1.0rc1/packages/dt_for_itables/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 and some of its extensions for [ITables](https://github.com/mwouts/itables/).
 
 # How to compile the bundle
 
 Run the following commands:
 ```bash
 npm install
-npm run build
+npm run build:js
 ```
 
 # How to update the dependencies
 
 Run
 ```bash
 npm update
```

### Comparing `itables-2.0.1/itables/dt_for_itables/dt_bundle.css` & `itables-2.1.0rc1/src/itables/html/dt_bundle.css`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/itables/dt_for_itables/dt_bundle.js` & `itables-2.1.0rc1/src/itables/html/dt_bundle.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,37 +1,37 @@
-var No = Object.create;
-var _a = Object.defineProperty;
-var Eo = Object.getOwnPropertyDescriptor;
-var Oo = Object.getOwnPropertyNames;
-var Ro = Object.getPrototypeOf,
-    Lo = Object.prototype.hasOwnProperty;
+var Eo = Object.create;
+var Ca = Object.defineProperty;
+var Oo = Object.getOwnPropertyDescriptor;
+var Ro = Object.getOwnPropertyNames;
+var Lo = Object.getPrototypeOf,
+    zo = Object.prototype.hasOwnProperty;
 var Wr = (t => typeof require < "u" ? require : typeof Proxy < "u" ? new Proxy(t, {
     get: (e, r) => (typeof require < "u" ? require : e)[r]
 }) : t)(function(t) {
     if (typeof require < "u") return require.apply(this, arguments);
     throw Error('Dynamic require of "' + t + '" is not supported')
 });
-var Ca = (t, e) => () => (e || t((e = {
+var Ta = (t, e) => () => (e || t((e = {
     exports: {}
 }).exports, e), e.exports);
-var zo = (t, e, r, n) => {
+var jo = (t, e, r, n) => {
     if (e && typeof e == "object" || typeof e == "function")
-        for (let s of Oo(e)) !Lo.call(t, s) && s !== r && _a(t, s, {
+        for (let s of Ro(e)) !zo.call(t, s) && s !== r && Ca(t, s, {
             get: () => e[s],
-            enumerable: !(n = Eo(e, s)) || n.enumerable
+            enumerable: !(n = Oo(e, s)) || n.enumerable
         });
     return t
 };
-var ne = (t, e, r) => (r = t != null ? No(Ro(t)) : {}, zo(e || !t || !t.__esModule ? _a(r, "default", {
+var ne = (t, e, r) => (r = t != null ? Eo(Lo(t)) : {}, jo(e || !t || !t.__esModule ? Ca(r, "default", {
     value: t,
     enumerable: !0
 }) : r, t));
-var ka = Ca((Ta, ii) => {
+var Sa = Ta((ka, ai) => {
     (function(t) {
-        typeof Ta == "object" && typeof ii < "u" ? ii.exports = t() : typeof define == "function" && define.amd ? define([], t) : (typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : this).JSZip = t()
+        typeof ka == "object" && typeof ai < "u" ? ai.exports = t() : typeof define == "function" && define.amd ? define([], t) : (typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : this).JSZip = t()
     })(function() {
         return function t(e, r, n) {
             function s(c, p) {
                 if (!r[c]) {
                     if (!e[c]) {
                         var b = typeof Wr == "function" && Wr;
                         if (!p && b) return b(c, !0);
@@ -3106,30 +3106,30 @@
                     for (M.heap_len = 0, M.heap_max = w, pt = 0; pt < bt; pt++) gt[2 * pt] !== 0 ? (M.heap[++M.heap_len] = zt = pt, M.depth[pt] = 0) : gt[2 * pt + 1] = 0;
                     for (; M.heap_len < 2;) gt[2 * (rt = M.heap[++M.heap_len] = zt < 2 ? ++zt : 0)] = 1, M.depth[rt] = 0, M.opt_len--, xt && (M.static_len -= Ct[2 * rt + 1]);
                     for (Y.max_code = zt, pt = M.heap_len >> 1; 1 <= pt; pt--) Bt(M, gt, pt);
                     for (rt = bt; pt = M.heap[1], M.heap[1] = M.heap[M.heap_len--], Bt(M, gt, 1), mt = M.heap[1], M.heap[--M.heap_max] = pt, M.heap[--M.heap_max] = mt, gt[2 * rt] = gt[2 * pt] + gt[2 * mt], M.depth[rt] = (M.depth[pt] >= M.depth[mt] ? M.depth[pt] : M.depth[mt]) + 1, gt[2 * pt + 1] = gt[2 * mt + 1] = rt, M.heap[1] = rt++, Bt(M, gt, 1), 2 <= M.heap_len;);
                     M.heap[--M.heap_max] = M.heap[1],
                         function(Ut, pe) {
                             var sr, we, Ye, te, be, Oe, de = pe.dyn_tree,
-                                tn = pe.max_code,
+                                en = pe.max_code,
                                 gr = pe.stat_desc.static_tree,
-                                en = pe.stat_desc.has_stree,
-                                rn = pe.stat_desc.extra_bits,
-                                nn = pe.stat_desc.extra_base,
+                                rn = pe.stat_desc.has_stree,
+                                nn = pe.stat_desc.extra_bits,
+                                an = pe.stat_desc.extra_base,
                                 Te = pe.stat_desc.max_length,
                                 je = 0;
                             for (te = 0; te <= k; te++) Ut.bl_count[te] = 0;
-                            for (de[2 * Ut.heap[Ut.heap_max] + 1] = 0, sr = Ut.heap_max + 1; sr < w; sr++) Te < (te = de[2 * de[2 * (we = Ut.heap[sr]) + 1] + 1] + 1) && (te = Te, je++), de[2 * we + 1] = te, tn < we || (Ut.bl_count[te]++, be = 0, nn <= we && (be = rn[we - nn]), Oe = de[2 * we], Ut.opt_len += Oe * (te + be), en && (Ut.static_len += Oe * (gr[2 * we + 1] + be)));
+                            for (de[2 * Ut.heap[Ut.heap_max] + 1] = 0, sr = Ut.heap_max + 1; sr < w; sr++) Te < (te = de[2 * de[2 * (we = Ut.heap[sr]) + 1] + 1] + 1) && (te = Te, je++), de[2 * we + 1] = te, en < we || (Ut.bl_count[te]++, be = 0, an <= we && (be = nn[we - an]), Oe = de[2 * we], Ut.opt_len += Oe * (te + be), rn && (Ut.static_len += Oe * (gr[2 * we + 1] + be)));
                             if (je !== 0) {
                                 do {
                                     for (te = Te - 1; Ut.bl_count[te] === 0;) te--;
                                     Ut.bl_count[te]--, Ut.bl_count[te + 1] += 2, Ut.bl_count[Te]--, je -= 2
                                 } while (0 < je);
                                 for (te = Te; te !== 0; te--)
-                                    for (we = Ut.bl_count[te]; we !== 0;) tn < (Ye = Ut.heap[--sr]) || (de[2 * Ye + 1] !== te && (Ut.opt_len += (te - de[2 * Ye + 1]) * de[2 * Ye], de[2 * Ye + 1] = te), we--)
+                                    for (we = Ut.bl_count[te]; we !== 0;) en < (Ye = Ut.heap[--sr]) || (de[2 * Ye + 1] !== te && (Ut.opt_len += (te - de[2 * Ye + 1]) * de[2 * Ye], de[2 * Ye + 1] = te), we--)
                             }
                         }(M, Y), Tt(gt, zt, M.bl_count)
                 }
 
                 function D(M, Y, pt) {
                     var mt, rt, gt = -1,
                         Ct = Y[1],
@@ -3304,22 +3304,22 @@
                         }
                     })(typeof self > "u" ? n === void 0 ? this : n : self)
                 }).call(this, typeof global < "u" ? global : typeof self < "u" ? self : typeof window < "u" ? window : {})
             }, {}]
         }, {}, [10])(10)
     })
 });
-var ie = Ca((Sa, hn) => {
+var ie = Ta((Da, pn) => {
     (function(t, e) {
         "use strict";
-        typeof hn == "object" && typeof hn.exports == "object" ? hn.exports = t.document ? e(t, !0) : function(r) {
+        typeof pn == "object" && typeof pn.exports == "object" ? pn.exports = t.document ? e(t, !0) : function(r) {
             if (!r.document) throw new Error("jQuery requires a window with a document");
             return e(r)
         } : e(t)
-    })(typeof window < "u" ? window : Sa, function(t, e) {
+    })(typeof window < "u" ? window : Da, function(t, e) {
         "use strict";
         var r = [],
             n = Object.getPrototypeOf,
             s = r.slice,
             a = r.flat ? function(i) {
                 return r.flat.call(i)
             } : function(i) {
@@ -3526,29 +3526,29 @@
         var R = F,
             L = l;
         (function() {
             var i, d, v, x, A, I = L,
                 E, $, U, Q, dt, ft = u.expando,
                 it = 0,
                 wt = 0,
-                Et = dn(),
-                Gt = dn(),
-                Mt = dn(),
-                le = dn(),
+                Et = un(),
+                Gt = un(),
+                Mt = un(),
+                le = un(),
                 se = function(V, K) {
                     return V === K && (A = !0), 0
                 },
                 Me = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",
                 Ve = "(?:\\\\[\\da-fA-F]{1,6}" + g + "?|\\\\[^\\r\\n\\f]|[\\w-]|[^\0-\\x7f])+",
                 qt = "\\[" + g + "*(" + Ve + ")(?:" + g + "*([*^$|!~]?=)" + g + `*(?:'((?:\\\\.|[^\\\\'])*)'|"((?:\\\\.|[^\\\\"])*)"|(` + Ve + "))|)" + g + "*\\]",
                 dr = ":(" + Ve + `)(?:\\((('((?:\\\\.|[^\\\\'])*)'|"((?:\\\\.|[^\\\\"])*)")|((?:\\\\.|[^\\\\()[\\]]|` + qt + ")*)|.*)\\)|)",
                 Xt = new RegExp(g + "+", "g"),
                 re = new RegExp("^" + g + "*," + g + "*"),
                 Mr = new RegExp("^" + g + "*([>+~]|" + g + ")" + g + "*"),
-                Yn = new RegExp(g + "|>"),
+                Qn = new RegExp(g + "|>"),
                 He = new RegExp(dr),
                 Vr = new RegExp("^" + Ve + "$"),
                 We = {
                     ID: new RegExp("^#(" + Ve + ")"),
                     CLASS: new RegExp("^\\.(" + Ve + ")"),
                     TAG: new RegExp("^(" + Ve + "|[*])"),
                     ATTR: new RegExp("^" + qt),
@@ -3556,31 +3556,31 @@
                     CHILD: new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" + g + "*(even|odd|(([+-]|)(\\d*)n|)" + g + "*(?:([+-]|)" + g + "*(\\d+)|))" + g + "*\\)|)", "i"),
                     bool: new RegExp("^(?:" + Me + ")$", "i"),
                     needsContext: new RegExp("^" + g + "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + g + "*((?:-\\d)?\\d*)" + g + "*\\)|)(?=[^-]|$)", "i")
                 },
                 Qe = /^(?:input|select|textarea|button)$/i,
                 Je = /^h\d$/i,
                 Se = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
-                Qn = /[+~]/,
-                Xe = new RegExp("\\\\[\\da-fA-F]{1,6}" + g + "?|\\\\([^\\r\\n\\f])", "g"),
-                $e = function(V, K) {
+                Jn = /[+~]/,
+                $e = new RegExp("\\\\[\\da-fA-F]{1,6}" + g + "?|\\\\([^\\r\\n\\f])", "g"),
+                Ze = function(V, K) {
                     var nt = "0x" + V.slice(1) - 65536;
                     return K || (nt < 0 ? String.fromCharCode(nt + 65536) : String.fromCharCode(nt >> 10 | 55296, nt & 1023 | 56320))
                 },
-                So = function() {
+                Do = function() {
                     tr()
                 },
-                Do = cn(function(V) {
+                Ao = fn(function(V) {
                     return V.disabled === !0 && q(V, "fieldset")
                 }, {
                     dir: "parentNode",
                     next: "legend"
                 });
 
-            function Ao() {
+            function Io() {
                 try {
                     return E.activeElement
                 } catch {}
             }
             try {
                 I.apply(r = s.call(R.childNodes), R.childNodes), r[R.childNodes.length].nodeType
             } catch {
@@ -3606,31 +3606,31 @@
                                     if (St.id === ct) return I.call(nt, St), nt
                                 } else return nt;
                             else if (Ot && (St = Ot.getElementById(ct)) && Yt.contains(K, St) && St.id === ct) return I.call(nt, St), nt
                         } else {
                             if (Dt[2]) return I.apply(nt, K.getElementsByTagName(V)), nt;
                             if ((ct = Dt[3]) && K.getElementsByClassName) return I.apply(nt, K.getElementsByClassName(ct)), nt
                         } if (!le[V + " "] && (!Q || !Q.test(V))) {
-                        if (Nt = V, Ot = K, Ht === 1 && (Yn.test(V) || Mr.test(V))) {
-                            for (Ot = Qn.test(V) && Jn(K.parentNode) || K, (Ot != K || !w.scope) && ((Pt = K.getAttribute("id")) ? Pt = u.escapeSelector(Pt) : K.setAttribute("id", Pt = ft)), Vt = Hr(V), _t = Vt.length; _t--;) Vt[_t] = (Pt ? "#" + Pt : ":scope") + " " + un(Vt[_t]);
+                        if (Nt = V, Ot = K, Ht === 1 && (Qn.test(V) || Mr.test(V))) {
+                            for (Ot = Jn.test(V) && ti(K.parentNode) || K, (Ot != K || !w.scope) && ((Pt = K.getAttribute("id")) ? Pt = u.escapeSelector(Pt) : K.setAttribute("id", Pt = ft)), Vt = Hr(V), _t = Vt.length; _t--;) Vt[_t] = (Pt ? "#" + Pt : ":scope") + " " + cn(Vt[_t]);
                             Nt = Vt.join(",")
                         }
                         try {
                             return I.apply(nt, Ot.querySelectorAll(Nt)), nt
                         } catch {
                             le(V, !0)
                         } finally {
                             Pt === ft && K.removeAttribute("id")
                         }
                     }
                 }
-                return xa(V.replace(_, "$1"), K, nt, lt)
+                return _a(V.replace(_, "$1"), K, nt, lt)
             }
 
-            function dn() {
+            function un() {
                 var V = [];
 
                 function K(nt, lt) {
                     return V.push(nt + " ") > d.cacheLength && delete K[V.shift()], K[nt + " "] = lt
                 }
                 return K
             }
@@ -3646,70 +3646,70 @@
                 } catch {
                     return !1
                 } finally {
                     K.parentNode && K.parentNode.removeChild(K), K = null
                 }
             }
 
-            function Io(V) {
+            function Po(V) {
                 return function(K) {
                     return q(K, "input") && K.type === V
                 }
             }
 
-            function Po(V) {
+            function Fo(V) {
                 return function(K) {
                     return (q(K, "input") || q(K, "button")) && K.type === V
                 }
             }
 
-            function ya(V) {
+            function wa(V) {
                 return function(K) {
-                    return "form" in K ? K.parentNode && K.disabled === !1 ? "label" in K ? "label" in K.parentNode ? K.parentNode.disabled === V : K.disabled === V : K.isDisabled === V || K.isDisabled !== !V && Do(K) === V : K.disabled === V : "label" in K ? K.disabled === V : !1
+                    return "form" in K ? K.parentNode && K.disabled === !1 ? "label" in K ? "label" in K.parentNode ? K.parentNode.disabled === V : K.disabled === V : K.isDisabled === V || K.isDisabled !== !V && Ao(K) === V : K.disabled === V : "label" in K ? K.disabled === V : !1
                 }
             }
 
             function ur(V) {
                 return Le(function(K) {
                     return K = +K, Le(function(nt, lt) {
                         for (var ct, _t = V([], nt.length, K), St = _t.length; St--;) nt[ct = _t[St]] && (nt[ct] = !(lt[ct] = nt[ct]))
                     })
                 })
             }
 
-            function Jn(V) {
+            function ti(V) {
                 return V && typeof V.getElementsByTagName < "u" && V
             }
 
             function tr(V) {
                 var K, nt = V ? V.ownerDocument || V : R;
-                return nt == E || nt.nodeType !== 9 || !nt.documentElement || (E = nt, $ = E.documentElement, U = !u.isXMLDoc(E), dt = $.matches || $.webkitMatchesSelector || $.msMatchesSelector, $.msMatchesSelector && R != E && (K = E.defaultView) && K.top !== K && K.addEventListener("unload", So), w.getById = Cr(function(lt) {
+                return nt == E || nt.nodeType !== 9 || !nt.documentElement || (E = nt, $ = E.documentElement, U = !u.isXMLDoc(E), dt = $.matches || $.webkitMatchesSelector || $.msMatchesSelector, $.msMatchesSelector && R != E && (K = E.defaultView) && K.top !== K && K.addEventListener("unload", Do), w.getById = Cr(function(lt) {
                     return $.appendChild(lt).id = u.expando, !E.getElementsByName || !E.getElementsByName(u.expando).length
                 }), w.disconnectedMatch = Cr(function(lt) {
                     return dt.call(lt, "*")
                 }), w.scope = Cr(function() {
                     return E.querySelectorAll(":scope")
                 }), w.cssHas = Cr(function() {
                     try {
                         return E.querySelector(":has(*,:jqfake)"), !1
                     } catch {
                         return !0
                     }
                 }), w.getById ? (d.filter.ID = function(lt) {
-                    var ct = lt.replace(Xe, $e);
+                    var ct = lt.replace($e, Ze);
                     return function(_t) {
                         return _t.getAttribute("id") === ct
                     }
                 }, d.find.ID = function(lt, ct) {
                     if (typeof ct.getElementById < "u" && U) {
                         var _t = ct.getElementById(lt);
                         return _t ? [_t] : []
                     }
                 }) : (d.filter.ID = function(lt) {
-                    var ct = lt.replace(Xe, $e);
+                    var ct = lt.replace($e, Ze);
                     return function(_t) {
                         var St = typeof _t.getAttributeNode < "u" && _t.getAttributeNode("id");
                         return St && St.value === ct
                     }
                 }, d.find.ID = function(lt, ct) {
                     if (typeof ct.getElementById < "u" && U) {
                         var _t, St, Pt, Dt = ct.getElementById(lt);
@@ -3783,27 +3783,27 @@
                     },
                     "~": {
                         dir: "previousSibling"
                     }
                 },
                 preFilter: {
                     ATTR: function(V) {
-                        return V[1] = V[1].replace(Xe, $e), V[3] = (V[3] || V[4] || V[5] || "").replace(Xe, $e), V[2] === "~=" && (V[3] = " " + V[3] + " "), V.slice(0, 4)
+                        return V[1] = V[1].replace($e, Ze), V[3] = (V[3] || V[4] || V[5] || "").replace($e, Ze), V[2] === "~=" && (V[3] = " " + V[3] + " "), V.slice(0, 4)
                     },
                     CHILD: function(V) {
                         return V[1] = V[1].toLowerCase(), V[1].slice(0, 3) === "nth" ? (V[3] || Yt.error(V[0]), V[4] = +(V[4] ? V[5] + (V[6] || 1) : 2 * (V[3] === "even" || V[3] === "odd")), V[5] = +(V[7] + V[8] || V[3] === "odd")) : V[3] && Yt.error(V[0]), V
                     },
                     PSEUDO: function(V) {
                         var K, nt = !V[6] && V[2];
                         return We.CHILD.test(V[0]) ? null : (V[3] ? V[2] = V[4] || V[5] || "" : nt && He.test(nt) && (K = Hr(nt, !0)) && (K = nt.indexOf(")", nt.length - K) - nt.length) && (V[0] = V[0].slice(0, K), V[2] = nt.slice(0, K)), V.slice(0, 3))
                     }
                 },
                 filter: {
                     TAG: function(V) {
-                        var K = V.replace(Xe, $e).toLowerCase();
+                        var K = V.replace($e, Ze).toLowerCase();
                         return V === "*" ? function() {
                             return !0
                         } : function(nt) {
                             return q(nt, K)
                         }
                     },
                     CLASS: function(V) {
@@ -3861,34 +3861,34 @@
                         }) : lt
                     }
                 },
                 pseudos: {
                     not: Le(function(V) {
                         var K = [],
                             nt = [],
-                            lt = ni(V.replace(_, "$1"));
+                            lt = ii(V.replace(_, "$1"));
                         return lt[ft] ? Le(function(ct, _t, St, Pt) {
                             for (var Dt, Vt = lt(ct, null, Pt, []), Nt = ct.length; Nt--;)(Dt = Vt[Nt]) && (ct[Nt] = !(_t[Nt] = Dt))
                         }) : function(ct, _t, St) {
                             return K[0] = ct, lt(K, null, St, nt), K[0] = null, !nt.pop()
                         }
                     }),
                     has: Le(function(V) {
                         return function(K) {
                             return Yt(V, K).length > 0
                         }
                     }),
                     contains: Le(function(V) {
-                        return V = V.replace(Xe, $e),
+                        return V = V.replace($e, Ze),
                             function(K) {
                                 return (K.textContent || u.text(K)).indexOf(V) > -1
                             }
                     }),
                     lang: Le(function(V) {
-                        return Vr.test(V || "") || Yt.error("unsupported lang: " + V), V = V.replace(Xe, $e).toLowerCase(),
+                        return Vr.test(V || "") || Yt.error("unsupported lang: " + V), V = V.replace($e, Ze).toLowerCase(),
                             function(K) {
                                 var nt;
                                 do
                                     if (nt = U ? K.lang : K.getAttribute("xml:lang") || K.getAttribute("lang")) return nt = nt.toLowerCase(), nt === V || nt.indexOf(V + "-") === 0; while ((K = K.parentNode) && K.nodeType === 1);
                                 return !1
                             }
                     }),
@@ -3896,18 +3896,18 @@
                         var K = t.location && t.location.hash;
                         return K && K.slice(1) === V.id
                     },
                     root: function(V) {
                         return V === $
                     },
                     focus: function(V) {
-                        return V === Ao() && E.hasFocus() && !!(V.type || V.href || ~V.tabIndex)
+                        return V === Io() && E.hasFocus() && !!(V.type || V.href || ~V.tabIndex)
                     },
-                    enabled: ya(!1),
-                    disabled: ya(!0),
+                    enabled: wa(!1),
+                    disabled: wa(!0),
                     checked: function(V) {
                         return q(V, "input") && !!V.checked || q(V, "option") && !!V.selected
                     },
                     selected: function(V) {
                         return V.parentNode && V.parentNode.selectedIndex, V.selected === !0
                     },
                     empty: function(V) {
@@ -3961,22 +3961,22 @@
             }, d.pseudos.nth = d.pseudos.eq;
             for (i in {
                     radio: !0,
                     checkbox: !0,
                     file: !0,
                     password: !0,
                     image: !0
-                }) d.pseudos[i] = Io(i);
+                }) d.pseudos[i] = Po(i);
             for (i in {
                     submit: !0,
                     reset: !0
-                }) d.pseudos[i] = Po(i);
+                }) d.pseudos[i] = Fo(i);
 
-            function wa() {}
-            wa.prototype = d.filters = d.pseudos, d.setFilters = new wa;
+            function xa() {}
+            xa.prototype = d.filters = d.pseudos, d.setFilters = new xa;
 
             function Hr(V, K) {
                 var nt, lt, ct, _t, St, Pt, Dt, Vt = Gt[V + " "];
                 if (Vt) return K ? 0 : Vt.slice(0);
                 for (St = V, Pt = [], Dt = d.preFilter; St;) {
                     (!nt || (lt = re.exec(St))) && (lt && (St = St.slice(lt[0].length) || St), Pt.push(ct = [])), nt = !1, (lt = Mr.exec(St)) && (nt = lt.shift(), ct.push({
                         value: nt,
@@ -3988,20 +3988,20 @@
                         matches: lt
                     }), St = St.slice(nt.length));
                     if (!nt) break
                 }
                 return K ? St.length : St ? Yt.error(V) : Gt(V, Pt).slice(0)
             }
 
-            function un(V) {
+            function cn(V) {
                 for (var K = 0, nt = V.length, lt = ""; K < nt; K++) lt += V[K].value;
                 return lt
             }
 
-            function cn(V, K, nt) {
+            function fn(V, K, nt) {
                 var lt = K.dir,
                     ct = K.next,
                     _t = ct || lt,
                     St = nt && _t === "parentNode",
                     Pt = wt++;
                 return K.first ? function(Dt, Vt, Nt) {
                     for (; Dt = Dt[lt];)
@@ -4019,75 +4019,75 @@
                                 else {
                                     if ((Ot = Ht[_t]) && Ot[0] === it && Ot[1] === Pt) return Ft[2] = Ot[2];
                                     if (Ht[_t] = Ft, Ft[2] = V(Dt, Vt, Nt)) return !0
                                 } return !1
                 }
             }
 
-            function ti(V) {
+            function ei(V) {
                 return V.length > 1 ? function(K, nt, lt) {
                     for (var ct = V.length; ct--;)
                         if (!V[ct](K, nt, lt)) return !1;
                     return !0
                 } : V[0]
             }
 
-            function Fo(V, K, nt) {
+            function Bo(V, K, nt) {
                 for (var lt = 0, ct = K.length; lt < ct; lt++) Yt(V, K[lt], nt);
                 return nt
             }
 
-            function fn(V, K, nt, lt, ct) {
+            function hn(V, K, nt, lt, ct) {
                 for (var _t, St = [], Pt = 0, Dt = V.length, Vt = K != null; Pt < Dt; Pt++)(_t = V[Pt]) && (!nt || nt(_t, lt, ct)) && (St.push(_t), Vt && K.push(Pt));
                 return St
             }
 
-            function ei(V, K, nt, lt, ct, _t) {
-                return lt && !lt[ft] && (lt = ei(lt)), ct && !ct[ft] && (ct = ei(ct, _t)), Le(function(St, Pt, Dt, Vt) {
+            function ri(V, K, nt, lt, ct, _t) {
+                return lt && !lt[ft] && (lt = ri(lt)), ct && !ct[ft] && (ct = ri(ct, _t)), Le(function(St, Pt, Dt, Vt) {
                     var Nt, Ot, Ht, Ft, ee = [],
                         ge = [],
                         ue = Pt.length,
-                        De = St || Fo(K || "*", Dt.nodeType ? [Dt] : Dt, []),
-                        Ue = V && (St || !K) ? fn(De, ee, V, Dt, Vt) : De;
+                        De = St || Bo(K || "*", Dt.nodeType ? [Dt] : Dt, []),
+                        Ue = V && (St || !K) ? hn(De, ee, V, Dt, Vt) : De;
                     if (nt ? (Ft = ct || (St ? V : ue || lt) ? [] : Pt, nt(Ue, Ft, Dt, Vt)) : Ft = Ue, lt)
-                        for (Nt = fn(Ft, ge), lt(Nt, [], Dt, Vt), Ot = Nt.length; Ot--;)(Ht = Nt[Ot]) && (Ft[ge[Ot]] = !(Ue[ge[Ot]] = Ht));
+                        for (Nt = hn(Ft, ge), lt(Nt, [], Dt, Vt), Ot = Nt.length; Ot--;)(Ht = Nt[Ot]) && (Ft[ge[Ot]] = !(Ue[ge[Ot]] = Ht));
                     if (St) {
                         if (ct || V) {
                             if (ct) {
                                 for (Nt = [], Ot = Ft.length; Ot--;)(Ht = Ft[Ot]) && Nt.push(Ue[Ot] = Ht);
                                 ct(null, Ft = [], Nt, Vt)
                             }
                             for (Ot = Ft.length; Ot--;)(Ht = Ft[Ot]) && (Nt = ct ? c.call(St, Ht) : ee[Ot]) > -1 && (St[Nt] = !(Pt[Nt] = Ht))
                         }
-                    } else Ft = fn(Ft === Pt ? Ft.splice(ue, Ft.length) : Ft), ct ? ct(null, Pt, Ft, Vt) : I.apply(Pt, Ft)
+                    } else Ft = hn(Ft === Pt ? Ft.splice(ue, Ft.length) : Ft), ct ? ct(null, Pt, Ft, Vt) : I.apply(Pt, Ft)
                 })
             }
 
-            function ri(V) {
-                for (var K, nt, lt, ct = V.length, _t = d.relative[V[0].type], St = _t || d.relative[" "], Pt = _t ? 1 : 0, Dt = cn(function(Ot) {
+            function ni(V) {
+                for (var K, nt, lt, ct = V.length, _t = d.relative[V[0].type], St = _t || d.relative[" "], Pt = _t ? 1 : 0, Dt = fn(function(Ot) {
                         return Ot === K
-                    }, St, !0), Vt = cn(function(Ot) {
+                    }, St, !0), Vt = fn(function(Ot) {
                         return c.call(K, Ot) > -1
                     }, St, !0), Nt = [function(Ot, Ht, Ft) {
                         var ee = !_t && (Ft || Ht != v) || ((K = Ht).nodeType ? Dt(Ot, Ht, Ft) : Vt(Ot, Ht, Ft));
                         return K = null, ee
                     }]; Pt < ct; Pt++)
-                    if (nt = d.relative[V[Pt].type]) Nt = [cn(ti(Nt), nt)];
+                    if (nt = d.relative[V[Pt].type]) Nt = [fn(ei(Nt), nt)];
                     else {
                         if (nt = d.filter[V[Pt].type].apply(null, V[Pt].matches), nt[ft]) {
                             for (lt = ++Pt; lt < ct && !d.relative[V[lt].type]; lt++);
-                            return ei(Pt > 1 && ti(Nt), Pt > 1 && un(V.slice(0, Pt - 1).concat({
+                            return ri(Pt > 1 && ei(Nt), Pt > 1 && cn(V.slice(0, Pt - 1).concat({
                                 value: V[Pt - 2].type === " " ? "*" : ""
-                            })).replace(_, "$1"), nt, Pt < lt && ri(V.slice(Pt, lt)), lt < ct && ri(V = V.slice(lt)), lt < ct && un(V))
+                            })).replace(_, "$1"), nt, Pt < lt && ni(V.slice(Pt, lt)), lt < ct && ni(V = V.slice(lt)), lt < ct && cn(V))
                         }
                         Nt.push(nt)
-                    } return ti(Nt)
+                    } return ei(Nt)
             }
 
-            function Bo(V, K) {
+            function No(V, K) {
                 var nt = K.length > 0,
                     lt = V.length > 0,
                     ct = function(_t, St, Pt, Dt, Vt) {
                         var Nt, Ot, Ht, Ft = 0,
                             ee = "0",
                             ge = _t && [],
                             ue = [],
@@ -4106,54 +4106,54 @@
                             nt && ((Nt = !Ht && Nt) && Ft--, _t && ge.push(Nt))
                         }
                         if (Ft += ee, nt && ee !== Ft) {
                             for (Ot = 0; Ht = K[Ot++];) Ht(ge, ue, St, Pt);
                             if (_t) {
                                 if (Ft > 0)
                                     for (; ee--;) ge[ee] || ue[ee] || (ue[ee] = et.call(Dt));
-                                ue = fn(ue)
+                                ue = hn(ue)
                             }
                             I.apply(Dt, ue), Vt && !_t && ue.length > 0 && Ft + K.length > 1 && u.uniqueSort(Dt)
                         }
                         return Vt && (it = Tr, v = De), ge
                     };
                 return nt ? Le(ct) : ct
             }
 
-            function ni(V, K) {
+            function ii(V, K) {
                 var nt, lt = [],
                     ct = [],
                     _t = Mt[V + " "];
                 if (!_t) {
-                    for (K || (K = Hr(V)), nt = K.length; nt--;) _t = ri(K[nt]), _t[ft] ? lt.push(_t) : ct.push(_t);
-                    _t = Mt(V, Bo(ct, lt)), _t.selector = V
+                    for (K || (K = Hr(V)), nt = K.length; nt--;) _t = ni(K[nt]), _t[ft] ? lt.push(_t) : ct.push(_t);
+                    _t = Mt(V, No(ct, lt)), _t.selector = V
                 }
                 return _t
             }
 
-            function xa(V, K, nt, lt) {
+            function _a(V, K, nt, lt) {
                 var ct, _t, St, Pt, Dt, Vt = typeof V == "function" && V,
                     Nt = !lt && Hr(V = Vt.selector || V);
                 if (nt = nt || [], Nt.length === 1) {
                     if (_t = Nt[0] = Nt[0].slice(0), _t.length > 2 && (St = _t[0]).type === "ID" && K.nodeType === 9 && U && d.relative[_t[1].type]) {
-                        if (K = (d.find.ID(St.matches[0].replace(Xe, $e), K) || [])[0], K) Vt && (K = K.parentNode);
+                        if (K = (d.find.ID(St.matches[0].replace($e, Ze), K) || [])[0], K) Vt && (K = K.parentNode);
                         else return nt;
                         V = V.slice(_t.shift().value.length)
                     }
                     for (ct = We.needsContext.test(V) ? 0 : _t.length; ct-- && (St = _t[ct], !d.relative[Pt = St.type]);)
-                        if ((Dt = d.find[Pt]) && (lt = Dt(St.matches[0].replace(Xe, $e), Qn.test(_t[0].type) && Jn(K.parentNode) || K))) {
-                            if (_t.splice(ct, 1), V = lt.length && un(_t), !V) return I.apply(nt, lt), nt;
+                        if ((Dt = d.find[Pt]) && (lt = Dt(St.matches[0].replace($e, Ze), Jn.test(_t[0].type) && ti(K.parentNode) || K))) {
+                            if (_t.splice(ct, 1), V = lt.length && cn(_t), !V) return I.apply(nt, lt), nt;
                             break
                         }
                 }
-                return (Vt || ni(V, Nt))(lt, K, !U, nt, !K || Qn.test(V) && Jn(K.parentNode) || K), nt
+                return (Vt || ii(V, Nt))(lt, K, !U, nt, !K || Jn.test(V) && ti(K.parentNode) || K), nt
             }
             w.sortStable = ft.split("").sort(se).join("") === ft, tr(), w.sortDetached = Cr(function(V) {
                 return V.compareDocumentPosition(E.createElement("fieldset")) & 1
-            }), u.find = Yt, u.expr[":"] = u.expr.pseudos, u.unique = u.uniqueSort, Yt.compile = ni, Yt.select = xa, Yt.setDocument = tr, Yt.tokenize = Hr, Yt.escape = u.escapeSelector, Yt.getText = u.text, Yt.isXML = u.isXMLDoc, Yt.selectors = u.expr, Yt.support = u.support, Yt.uniqueSort = u.uniqueSort
+            }), u.find = Yt, u.expr[":"] = u.expr.pseudos, u.unique = u.uniqueSort, Yt.compile = ii, Yt.select = _a, Yt.setDocument = tr, Yt.tokenize = Hr, Yt.escape = u.escapeSelector, Yt.getText = u.text, Yt.isXML = u.isXMLDoc, Yt.selectors = u.expr, Yt.support = u.support, Yt.uniqueSort = u.uniqueSort
         })();
         var X = function(i, d, v) {
                 for (var x = [], A = v !== void 0;
                     (i = i[d]) && i.nodeType !== 9;)
                     if (i.nodeType === 1) {
                         if (A && u(i).is(v)) break;
                         x.push(i)
@@ -4685,25 +4685,25 @@
         var Ye = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
             te = new RegExp("^(?:([+-])=|)(" + Ye + ")([a-z%]*)$", "i"),
             be = ["Top", "Right", "Bottom", "Left"],
             Oe = F.documentElement,
             de = function(i) {
                 return u.contains(i.ownerDocument, i)
             },
-            tn = {
+            en = {
                 composed: !0
             };
         Oe.getRootNode && (de = function(i) {
-            return u.contains(i.ownerDocument, i) || i.getRootNode(tn) === i.ownerDocument
+            return u.contains(i.ownerDocument, i) || i.getRootNode(en) === i.ownerDocument
         });
         var gr = function(i, d) {
             return i = d || i, i.style.display === "none" || i.style.display === "" && de(i) && u.css(i, "display") === "none"
         };
 
-        function en(i, d, v, x) {
+        function rn(i, d, v, x) {
             var A, I, E = 20,
                 $ = x ? function() {
                     return x.cur()
                 } : function() {
                     return u.css(i, d, "")
                 },
                 U = $(),
@@ -4711,25 +4711,25 @@
                 dt = i.nodeType && (u.cssNumber[d] || Q !== "px" && +U) && te.exec(u.css(i, d));
             if (dt && dt[3] !== Q) {
                 for (U = U / 2, Q = Q || dt[3], dt = +U || 1; E--;) u.style(i, d, dt + Q), (1 - I) * (1 - (I = $() / U || .5)) <= 0 && (E = 0), dt = dt / I;
                 dt = dt * 2, u.style(i, d, dt + Q), v = v || []
             }
             return v && (dt = +dt || +U || 0, A = v[1] ? dt + (v[1] + 1) * v[2] : +v[2], x && (x.unit = Q, x.start = dt, x.end = A)), A
         }
-        var rn = {};
+        var nn = {};
 
-        function nn(i) {
+        function an(i) {
             var d, v = i.ownerDocument,
                 x = i.nodeName,
-                A = rn[x];
-            return A || (d = v.body.appendChild(v.createElement(x)), A = u.css(d, "display"), d.parentNode.removeChild(d), A === "none" && (A = "block"), rn[x] = A, A)
+                A = nn[x];
+            return A || (d = v.body.appendChild(v.createElement(x)), A = u.css(d, "display"), d.parentNode.removeChild(d), A === "none" && (A = "block"), nn[x] = A, A)
         }
 
         function Te(i, d) {
-            for (var v, x, A = [], I = 0, E = i.length; I < E; I++) x = i[I], x.style && (v = x.style.display, d ? (v === "none" && (A[I] = bt.get(x, "display") || null, A[I] || (x.style.display = "")), x.style.display === "" && gr(x) && (A[I] = nn(x))) : v !== "none" && (A[I] = "none", bt.set(x, "display", v)));
+            for (var v, x, A = [], I = 0, E = i.length; I < E; I++) x = i[I], x.style && (v = x.style.display, d ? (v === "none" && (A[I] = bt.get(x, "display") || null, A[I] || (x.style.display = "")), x.style.display === "" && gr(x) && (A[I] = an(x))) : v !== "none" && (A[I] = "none", bt.set(x, "display", v)));
             for (I = 0; I < E; I++) A[I] != null && (i[I].style.display = A[I]);
             return i
         }
         u.fn.extend({
             show: function() {
                 return Te(this, !0)
             },
@@ -4739,16 +4739,16 @@
             toggle: function(i) {
                 return typeof i == "boolean" ? i ? this.show() : this.hide() : this.each(function() {
                     gr(this) ? u(this).show() : u(this).hide()
                 })
             }
         });
         var je = /^(?:checkbox|radio)$/i,
-            Gi = /<([a-z][^\/\0>\x20\t\r\n\f]*)/i,
-            Xi = /^$|^module$|\/(?:java|ecma)script/i;
+            Xi = /<([a-z][^\/\0>\x20\t\r\n\f]*)/i,
+            $i = /^$|^module$|\/(?:java|ecma)script/i;
         (function() {
             var i = F.createDocumentFragment(),
                 d = i.appendChild(F.createElement("div")),
                 v = F.createElement("input");
             v.setAttribute("type", "radio"), v.setAttribute("checked", "checked"), v.setAttribute("name", "t"), d.appendChild(v), w.checkClone = d.cloneNode(!0).cloneNode(!0).lastChild.checked, d.innerHTML = "<textarea>x</textarea>", w.noCloneChecked = !!d.cloneNode(!0).lastChild.defaultValue, d.innerHTML = "<option></option>", w.option = !!d.lastChild
         })();
         var ke = {
@@ -4761,53 +4761,53 @@
         ke.tbody = ke.tfoot = ke.colgroup = ke.caption = ke.thead, ke.th = ke.td, w.option || (ke.optgroup = ke.option = [1, "<select multiple='multiple'>", "</select>"]);
 
         function ve(i, d) {
             var v;
             return typeof i.getElementsByTagName < "u" ? v = i.getElementsByTagName(d || "*") : typeof i.querySelectorAll < "u" ? v = i.querySelectorAll(d || "*") : v = [], d === void 0 || d && q(i, d) ? u.merge([i], v) : v
         }
 
-        function Ln(i, d) {
+        function zn(i, d) {
             for (var v = 0, x = i.length; v < x; v++) bt.set(i[v], "globalEval", !d || bt.get(d[v], "globalEval"))
         }
-        var qs = /<|&#?\w+;/;
+        var Gs = /<|&#?\w+;/;
 
-        function $i(i, d, v, x, A) {
+        function Zi(i, d, v, x, A) {
             for (var I, E, $, U, Q, dt, ft = d.createDocumentFragment(), it = [], wt = 0, Et = i.length; wt < Et; wt++)
                 if (I = i[wt], I || I === 0)
                     if (f(I) === "object") u.merge(it, I.nodeType ? [I] : I);
-                    else if (!qs.test(I)) it.push(d.createTextNode(I));
+                    else if (!Gs.test(I)) it.push(d.createTextNode(I));
             else {
-                for (E = E || ft.appendChild(d.createElement("div")), $ = (Gi.exec(I) || ["", ""])[1].toLowerCase(), U = ke[$] || ke._default, E.innerHTML = U[1] + u.htmlPrefilter(I) + U[2], dt = U[0]; dt--;) E = E.lastChild;
+                for (E = E || ft.appendChild(d.createElement("div")), $ = (Xi.exec(I) || ["", ""])[1].toLowerCase(), U = ke[$] || ke._default, E.innerHTML = U[1] + u.htmlPrefilter(I) + U[2], dt = U[0]; dt--;) E = E.lastChild;
                 u.merge(it, E.childNodes), E = ft.firstChild, E.textContent = ""
             }
             for (ft.textContent = "", wt = 0; I = it[wt++];) {
                 if (x && u.inArray(I, x) > -1) {
                     A && A.push(I);
                     continue
                 }
-                if (Q = de(I), E = ve(ft.appendChild(I), "script"), Q && Ln(E), v)
-                    for (dt = 0; I = E[dt++];) Xi.test(I.type || "") && v.push(I)
+                if (Q = de(I), E = ve(ft.appendChild(I), "script"), Q && zn(E), v)
+                    for (dt = 0; I = E[dt++];) $i.test(I.type || "") && v.push(I)
             }
             return ft
         }
-        var Zi = /^([^.]*)(?:\.(.+)|)/;
+        var Ki = /^([^.]*)(?:\.(.+)|)/;
 
         function yr() {
             return !0
         }
 
         function wr() {
             return !1
         }
 
-        function zn(i, d, v, x, A, I) {
+        function jn(i, d, v, x, A, I) {
             var E, $;
             if (typeof d == "object") {
                 typeof v != "string" && (x = x || v, v = void 0);
-                for ($ in d) zn(i, $, v, x, d[$], I);
+                for ($ in d) jn(i, $, v, x, d[$], I);
                 return i
             }
             if (x == null && A == null ? (A = v, x = v = void 0) : A == null && (typeof v == "string" ? (A = x, x = void 0) : (A = x, x = v, v = void 0)), A === !1) A = wr;
             else if (!A) return i;
             return I === 1 && (E = A, A = function(U) {
                 return u().off(U), E.apply(this, arguments)
             }, A.guid = E.guid || (E.guid = u.guid++)), i.each(function() {
@@ -4817,30 +4817,30 @@
         u.event = {
             global: {},
             add: function(i, d, v, x, A) {
                 var I, E, $, U, Q, dt, ft, it, wt, Et, Gt, Mt = bt.get(i);
                 if (Ct(i))
                     for (v.handler && (I = v, v = I.handler, A = I.selector), A && u.find.matchesSelector(Oe, A), v.guid || (v.guid = u.guid++), (U = Mt.events) || (U = Mt.events = Object.create(null)), (E = Mt.handle) || (E = Mt.handle = function(le) {
                             return typeof u < "u" && u.event.triggered !== le.type ? u.event.dispatch.apply(i, arguments) : void 0
-                        }), d = (d || "").match(Bt) || [""], Q = d.length; Q--;) $ = Zi.exec(d[Q]) || [], wt = Gt = $[1], Et = ($[2] || "").split(".").sort(), wt && (ft = u.event.special[wt] || {}, wt = (A ? ft.delegateType : ft.bindType) || wt, ft = u.event.special[wt] || {}, dt = u.extend({
+                        }), d = (d || "").match(Bt) || [""], Q = d.length; Q--;) $ = Ki.exec(d[Q]) || [], wt = Gt = $[1], Et = ($[2] || "").split(".").sort(), wt && (ft = u.event.special[wt] || {}, wt = (A ? ft.delegateType : ft.bindType) || wt, ft = u.event.special[wt] || {}, dt = u.extend({
                         type: wt,
                         origType: Gt,
                         data: x,
                         handler: v,
                         guid: v.guid,
                         selector: A,
                         needsContext: A && u.expr.match.needsContext.test(A),
                         namespace: Et.join(".")
                     }, I), (it = U[wt]) || (it = U[wt] = [], it.delegateCount = 0, (!ft.setup || ft.setup.call(i, x, Et, E) === !1) && i.addEventListener && i.addEventListener(wt, E)), ft.add && (ft.add.call(i, dt), dt.handler.guid || (dt.handler.guid = v.guid)), A ? it.splice(it.delegateCount++, 0, dt) : it.push(dt), u.event.global[wt] = !0)
             },
             remove: function(i, d, v, x, A) {
                 var I, E, $, U, Q, dt, ft, it, wt, Et, Gt, Mt = bt.hasData(i) && bt.get(i);
                 if (!(!Mt || !(U = Mt.events))) {
                     for (d = (d || "").match(Bt) || [""], Q = d.length; Q--;) {
-                        if ($ = Zi.exec(d[Q]) || [], wt = Gt = $[1], Et = ($[2] || "").split(".").sort(), !wt) {
+                        if ($ = Ki.exec(d[Q]) || [], wt = Gt = $[1], Et = ($[2] || "").split(".").sort(), !wt) {
                             for (wt in U) u.event.remove(i, wt + d[Q], v, x, !0);
                             continue
                         }
                         for (ft = u.event.special[wt] || {}, wt = (x ? ft.delegateType : ft.bindType) || wt, it = U[wt] || [], $ = $[2] && new RegExp("(^|\\.)" + Et.join("\\.(?:.*\\.|)") + "(\\.|$)"), E = I = it.length; I--;) dt = it[I], (A || Gt === dt.origType) && (!v || v.guid === dt.guid) && (!$ || $.test(dt.namespace)) && (!x || x === dt.selector || x === "**" && dt.selector) && (it.splice(I, 1), dt.selector && it.delegateCount--, ft.remove && ft.remove.call(i, dt));
                         E && !it.length && ((!ft.teardown || ft.teardown.call(i, Et, Mt.handle) === !1) && u.removeEvent(i, wt, Mt.handle), delete U[wt])
                     }
                     u.isEmptyObject(U) && bt.remove(i, "handle events")
@@ -4904,34 +4904,34 @@
             special: {
                 load: {
                     noBubble: !0
                 },
                 click: {
                     setup: function(i) {
                         var d = this || i;
-                        return je.test(d.type) && d.click && q(d, "input") && an(d, "click", !0), !1
+                        return je.test(d.type) && d.click && q(d, "input") && sn(d, "click", !0), !1
                     },
                     trigger: function(i) {
                         var d = this || i;
-                        return je.test(d.type) && d.click && q(d, "input") && an(d, "click"), !0
+                        return je.test(d.type) && d.click && q(d, "input") && sn(d, "click"), !0
                     },
                     _default: function(i) {
                         var d = i.target;
                         return je.test(d.type) && d.click && q(d, "input") && bt.get(d, "click") || q(d, "a")
                     }
                 },
                 beforeunload: {
                     postDispatch: function(i) {
                         i.result !== void 0 && i.originalEvent && (i.originalEvent.returnValue = i.result)
                     }
                 }
             }
         };
 
-        function an(i, d, v) {
+        function sn(i, d, v) {
             if (!v) {
                 bt.get(i, d) === void 0 && u.event.add(i, d, yr);
                 return
             }
             bt.set(i, d, !1), u.event.add(i, d, {
                 namespace: !1,
                 handler: function(x) {
@@ -5008,19 +5008,19 @@
                         I = u.event.fix(x);
                     I.type = x.type === "focusin" ? "focus" : "blur", I.isSimulated = !0, A(x), I.target === I.currentTarget && A(I)
                 } else u.event.simulate(d, x.target, u.event.fix(x))
             }
             u.event.special[i] = {
                 setup: function() {
                     var x;
-                    if (an(this, i, !0), F.documentMode) x = bt.get(this, d), x || this.addEventListener(d, v), bt.set(this, d, (x || 0) + 1);
+                    if (sn(this, i, !0), F.documentMode) x = bt.get(this, d), x || this.addEventListener(d, v), bt.set(this, d, (x || 0) + 1);
                     else return !1
                 },
                 trigger: function() {
-                    return an(this, i), !0
+                    return sn(this, i), !0
                 },
                 teardown: function() {
                     var x;
                     if (F.documentMode) x = bt.get(this, d) - 1, x ? bt.set(this, d, x) : (this.removeEventListener(d, v), bt.remove(this, d));
                     else return !1
                 },
                 _default: function(x) {
@@ -5055,104 +5055,104 @@
                         I = v.relatedTarget,
                         E = v.handleObj;
                     return (!I || I !== A && !u.contains(A, I)) && (v.type = E.origType, x = E.handler.apply(this, arguments), v.type = d), x
                 }
             }
         }), u.fn.extend({
             on: function(i, d, v, x) {
-                return zn(this, i, d, v, x)
+                return jn(this, i, d, v, x)
             },
             one: function(i, d, v, x) {
-                return zn(this, i, d, v, x, 1)
+                return jn(this, i, d, v, x, 1)
             },
             off: function(i, d, v) {
                 var x, A;
                 if (i && i.preventDefault && i.handleObj) return x = i.handleObj, u(i.delegateTarget).off(x.namespace ? x.origType + "." + x.namespace : x.origType, x.selector, x.handler), this;
                 if (typeof i == "object") {
                     for (A in i) this.off(A, d, i[A]);
                     return this
                 }
                 return (d === !1 || typeof d == "function") && (v = d, d = void 0), v === !1 && (v = wr), this.each(function() {
                     u.event.remove(this, i, v, d)
                 })
             }
         });
-        var Gs = /<script|<style|<link/i,
-            Xs = /checked\s*(?:[^=]|=\s*.checked.)/i,
-            $s = /^\s*<!\[CDATA\[|\]\]>\s*$/g;
+        var Xs = /<script|<style|<link/i,
+            $s = /checked\s*(?:[^=]|=\s*.checked.)/i,
+            Zs = /^\s*<!\[CDATA\[|\]\]>\s*$/g;
 
-        function Ki(i, d) {
+        function Yi(i, d) {
             return q(i, "table") && q(d.nodeType !== 11 ? d : d.firstChild, "tr") && u(i).children("tbody")[0] || i
         }
 
-        function Zs(i) {
+        function Ks(i) {
             return i.type = (i.getAttribute("type") !== null) + "/" + i.type, i
         }
 
-        function Ks(i) {
+        function Ys(i) {
             return (i.type || "").slice(0, 5) === "true/" ? i.type = i.type.slice(5) : i.removeAttribute("type"), i
         }
 
-        function Yi(i, d) {
+        function Qi(i, d) {
             var v, x, A, I, E, $, U;
             if (d.nodeType === 1) {
                 if (bt.hasData(i) && (I = bt.get(i), U = I.events, U)) {
                     bt.remove(d, "handle events");
                     for (A in U)
                         for (v = 0, x = U[A].length; v < x; v++) u.event.add(d, A, U[A][v])
                 }
                 zt.hasData(i) && (E = zt.access(i), $ = u.extend({}, E), zt.set(d, $))
             }
         }
 
-        function Ys(i, d) {
+        function Qs(i, d) {
             var v = d.nodeName.toLowerCase();
             v === "input" && je.test(i.type) ? d.checked = i.checked : (v === "input" || v === "textarea") && (d.defaultValue = i.defaultValue)
         }
 
         function xr(i, d, v, x) {
             d = a(d);
             var A, I, E, $, U, Q, dt = 0,
                 ft = i.length,
                 it = ft - 1,
                 wt = d[0],
                 Et = k(wt);
-            if (Et || ft > 1 && typeof wt == "string" && !w.checkClone && Xs.test(wt)) return i.each(function(Gt) {
+            if (Et || ft > 1 && typeof wt == "string" && !w.checkClone && $s.test(wt)) return i.each(function(Gt) {
                 var Mt = i.eq(Gt);
                 Et && (d[0] = wt.call(this, Gt, Mt.html())), xr(Mt, d, v, x)
             });
-            if (ft && (A = $i(d, i[0].ownerDocument, !1, i, x), I = A.firstChild, A.childNodes.length === 1 && (A = I), I || x)) {
-                for (E = u.map(ve(A, "script"), Zs), $ = E.length; dt < ft; dt++) U = A, dt !== it && (U = u.clone(U, !0, !0), $ && u.merge(E, ve(U, "script"))), v.call(i[dt], U, dt);
+            if (ft && (A = Zi(d, i[0].ownerDocument, !1, i, x), I = A.firstChild, A.childNodes.length === 1 && (A = I), I || x)) {
+                for (E = u.map(ve(A, "script"), Ks), $ = E.length; dt < ft; dt++) U = A, dt !== it && (U = u.clone(U, !0, !0), $ && u.merge(E, ve(U, "script"))), v.call(i[dt], U, dt);
                 if ($)
-                    for (Q = E[E.length - 1].ownerDocument, u.map(E, Ks), dt = 0; dt < $; dt++) U = E[dt], Xi.test(U.type || "") && !bt.access(U, "globalEval") && u.contains(Q, U) && (U.src && (U.type || "").toLowerCase() !== "module" ? u._evalUrl && !U.noModule && u._evalUrl(U.src, {
+                    for (Q = E[E.length - 1].ownerDocument, u.map(E, Ys), dt = 0; dt < $; dt++) U = E[dt], $i.test(U.type || "") && !bt.access(U, "globalEval") && u.contains(Q, U) && (U.src && (U.type || "").toLowerCase() !== "module" ? u._evalUrl && !U.noModule && u._evalUrl(U.src, {
                         nonce: U.nonce || U.getAttribute("nonce")
-                    }, Q) : o(U.textContent.replace($s, ""), U, Q))
+                    }, Q) : o(U.textContent.replace(Zs, ""), U, Q))
             }
             return i
         }
 
-        function Qi(i, d, v) {
+        function Ji(i, d, v) {
             for (var x, A = d ? u.filter(d, i) : i, I = 0;
-                (x = A[I]) != null; I++) !v && x.nodeType === 1 && u.cleanData(ve(x)), x.parentNode && (v && de(x) && Ln(ve(x, "script")), x.parentNode.removeChild(x));
+                (x = A[I]) != null; I++) !v && x.nodeType === 1 && u.cleanData(ve(x)), x.parentNode && (v && de(x) && zn(ve(x, "script")), x.parentNode.removeChild(x));
             return i
         }
         u.extend({
             htmlPrefilter: function(i) {
                 return i
             },
             clone: function(i, d, v) {
                 var x, A, I, E, $ = i.cloneNode(!0),
                     U = de(i);
                 if (!w.noCloneChecked && (i.nodeType === 1 || i.nodeType === 11) && !u.isXMLDoc(i))
-                    for (E = ve($), I = ve(i), x = 0, A = I.length; x < A; x++) Ys(I[x], E[x]);
+                    for (E = ve($), I = ve(i), x = 0, A = I.length; x < A; x++) Qs(I[x], E[x]);
                 if (d)
                     if (v)
-                        for (I = I || ve(i), E = E || ve($), x = 0, A = I.length; x < A; x++) Yi(I[x], E[x]);
-                    else Yi(i, $);
-                return E = ve($, "script"), E.length > 0 && Ln(E, !U && ve(i, "script")), $
+                        for (I = I || ve(i), E = E || ve($), x = 0, A = I.length; x < A; x++) Qi(I[x], E[x]);
+                    else Qi(i, $);
+                return E = ve($, "script"), E.length > 0 && zn(E, !U && ve(i, "script")), $
             },
             cleanData: function(i) {
                 for (var d, v, x, A = u.event.special, I = 0;
                     (v = i[I]) !== void 0; I++)
                     if (Ct(v)) {
                         if (d = v[bt.expando]) {
                             if (d.events)
@@ -5160,38 +5160,38 @@
                             v[bt.expando] = void 0
                         }
                         v[zt.expando] && (v[zt.expando] = void 0)
                     }
             }
         }), u.fn.extend({
             detach: function(i) {
-                return Qi(this, i, !0)
+                return Ji(this, i, !0)
             },
             remove: function(i) {
-                return Qi(this, i)
+                return Ji(this, i)
             },
             text: function(i) {
                 return Y(this, function(d) {
                     return d === void 0 ? u.text(this) : this.empty().each(function() {
                         (this.nodeType === 1 || this.nodeType === 11 || this.nodeType === 9) && (this.textContent = d)
                     })
                 }, null, i, arguments.length)
             },
             append: function() {
                 return xr(this, arguments, function(i) {
                     if (this.nodeType === 1 || this.nodeType === 11 || this.nodeType === 9) {
-                        var d = Ki(this, i);
+                        var d = Yi(this, i);
                         d.appendChild(i)
                     }
                 })
             },
             prepend: function() {
                 return xr(this, arguments, function(i) {
                     if (this.nodeType === 1 || this.nodeType === 11 || this.nodeType === 9) {
-                        var d = Ki(this, i);
+                        var d = Yi(this, i);
                         d.insertBefore(i, d.firstChild)
                     }
                 })
             },
             before: function() {
                 return xr(this, arguments, function(i) {
                     this.parentNode && this.parentNode.insertBefore(i, this)
@@ -5214,15 +5214,15 @@
             },
             html: function(i) {
                 return Y(this, function(d) {
                     var v = this[0] || {},
                         x = 0,
                         A = this.length;
                     if (d === void 0 && v.nodeType === 1) return v.innerHTML;
-                    if (typeof d == "string" && !Gs.test(d) && !ke[(Gi.exec(d) || ["", ""])[1].toLowerCase()]) {
+                    if (typeof d == "string" && !Xs.test(d) && !ke[(Xi.exec(d) || ["", ""])[1].toLowerCase()]) {
                         d = u.htmlPrefilter(d);
                         try {
                             for (; x < A; x++) v = this[x] || {}, v.nodeType === 1 && (u.cleanData(ve(v, !1)), v.innerHTML = d);
                             v = 0
                         } catch {}
                     }
                     v && this.empty().append(d)
@@ -5243,28 +5243,28 @@
             replaceAll: "replaceWith"
         }, function(i, d) {
             u.fn[i] = function(v) {
                 for (var x, A = [], I = u(v), E = I.length - 1, $ = 0; $ <= E; $++) x = $ === E ? this : this.clone(!0), u(I[$])[d](x), l.apply(A, x.get());
                 return this.pushStack(A)
             }
         });
-        var jn = new RegExp("^(" + Ye + ")(?!px)[a-z%]+$", "i"),
-            Mn = /^--/,
-            sn = function(i) {
+        var Mn = new RegExp("^(" + Ye + ")(?!px)[a-z%]+$", "i"),
+            Vn = /^--/,
+            on = function(i) {
                 var d = i.ownerDocument.defaultView;
                 return (!d || !d.opener) && (d = t), d.getComputedStyle(i)
             },
-            Ji = function(i, d, v) {
+            ta = function(i, d, v) {
                 var x, A, I = {};
                 for (A in d) I[A] = i.style[A], i.style[A] = d[A];
                 x = v.call(i);
                 for (A in d) i.style[A] = I[A];
                 return x
             },
-            Qs = new RegExp(be.join("|"), "i");
+            Js = new RegExp(be.join("|"), "i");
         (function() {
             function i() {
                 if (Q) {
                     U.style.cssText = "position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0", Q.style.cssText = "position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%", Oe.appendChild(U).appendChild(Q);
                     var dt = t.getComputedStyle(Q);
                     v = dt.top !== "1%", $ = d(dt.marginLeft) === 12, Q.style.right = "60%", I = d(dt.right) === 36, x = d(dt.width) === 36, Q.style.position = "absolute", A = d(Q.offsetWidth / 3) === 12, Oe.removeChild(U), Q = null
                 }
@@ -5295,81 +5295,81 @@
                     var dt, ft, it, wt;
                     return E == null && (dt = F.createElement("table"), ft = F.createElement("tr"), it = F.createElement("div"), dt.style.cssText = "position:absolute;left:-11111px;border-collapse:separate", ft.style.cssText = "box-sizing:content-box;border:1px solid", ft.style.height = "1px", it.style.height = "9px", it.style.display = "block", Oe.appendChild(dt).appendChild(ft).appendChild(it), wt = t.getComputedStyle(ft), E = parseInt(wt.height, 10) + parseInt(wt.borderTopWidth, 10) + parseInt(wt.borderBottomWidth, 10) === ft.offsetHeight, Oe.removeChild(dt)), E
                 }
             }))
         })();
 
         function Rr(i, d, v) {
-            var x, A, I, E, $ = Mn.test(d),
+            var x, A, I, E, $ = Vn.test(d),
                 U = i.style;
-            return v = v || sn(i), v && (E = v.getPropertyValue(d) || v[d], $ && E && (E = E.replace(_, "$1") || void 0), E === "" && !de(i) && (E = u.style(i, d)), !w.pixelBoxStyles() && jn.test(E) && Qs.test(d) && (x = U.width, A = U.minWidth, I = U.maxWidth, U.minWidth = U.maxWidth = U.width = E, E = v.width, U.width = x, U.minWidth = A, U.maxWidth = I)), E !== void 0 ? E + "" : E
+            return v = v || on(i), v && (E = v.getPropertyValue(d) || v[d], $ && E && (E = E.replace(_, "$1") || void 0), E === "" && !de(i) && (E = u.style(i, d)), !w.pixelBoxStyles() && Mn.test(E) && Js.test(d) && (x = U.width, A = U.minWidth, I = U.maxWidth, U.minWidth = U.maxWidth = U.width = E, E = v.width, U.width = x, U.minWidth = A, U.maxWidth = I)), E !== void 0 ? E + "" : E
         }
 
-        function ta(i, d) {
+        function ea(i, d) {
             return {
                 get: function() {
                     if (i()) {
                         delete this.get;
                         return
                     }
                     return (this.get = d).apply(this, arguments)
                 }
             }
         }
-        var ea = ["Webkit", "Moz", "ms"],
-            ra = F.createElement("div").style,
-            na = {};
+        var ra = ["Webkit", "Moz", "ms"],
+            na = F.createElement("div").style,
+            ia = {};
 
-        function Js(i) {
-            for (var d = i[0].toUpperCase() + i.slice(1), v = ea.length; v--;)
-                if (i = ea[v] + d, i in ra) return i
+        function to(i) {
+            for (var d = i[0].toUpperCase() + i.slice(1), v = ra.length; v--;)
+                if (i = ra[v] + d, i in na) return i
         }
 
-        function Vn(i) {
-            var d = u.cssProps[i] || na[i];
-            return d || (i in ra ? i : na[i] = Js(i) || i)
+        function Hn(i) {
+            var d = u.cssProps[i] || ia[i];
+            return d || (i in na ? i : ia[i] = to(i) || i)
         }
-        var to = /^(none|table(?!-c[ea]).+)/,
-            eo = {
+        var eo = /^(none|table(?!-c[ea]).+)/,
+            ro = {
                 position: "absolute",
                 visibility: "hidden",
                 display: "block"
             },
-            ia = {
+            aa = {
                 letterSpacing: "0",
                 fontWeight: "400"
             };
 
-        function aa(i, d, v) {
+        function sa(i, d, v) {
             var x = te.exec(d);
             return x ? Math.max(0, x[2] - (v || 0)) + (x[3] || "px") : d
         }
 
-        function Hn(i, d, v, x, A, I) {
+        function Wn(i, d, v, x, A, I) {
             var E = d === "width" ? 1 : 0,
                 $ = 0,
                 U = 0,
                 Q = 0;
             if (v === (x ? "border" : "content")) return 0;
             for (; E < 4; E += 2) v === "margin" && (Q += u.css(i, v + be[E], !0, A)), x ? (v === "content" && (U -= u.css(i, "padding" + be[E], !0, A)), v !== "margin" && (U -= u.css(i, "border" + be[E] + "Width", !0, A))) : (U += u.css(i, "padding" + be[E], !0, A), v !== "padding" ? U += u.css(i, "border" + be[E] + "Width", !0, A) : $ += u.css(i, "border" + be[E] + "Width", !0, A));
             return !x && I >= 0 && (U += Math.max(0, Math.ceil(i["offset" + d[0].toUpperCase() + d.slice(1)] - I - U - $ - .5)) || 0), U + Q
         }
 
-        function sa(i, d, v) {
-            var x = sn(i),
+        function oa(i, d, v) {
+            var x = on(i),
                 A = !w.boxSizingReliable() || v,
                 I = A && u.css(i, "boxSizing", !1, x) === "border-box",
                 E = I,
                 $ = Rr(i, d, x),
                 U = "offset" + d[0].toUpperCase() + d.slice(1);
-            if (jn.test($)) {
+            if (Mn.test($)) {
                 if (!v) return $;
                 $ = "auto"
             }
-            return (!w.boxSizingReliable() && I || !w.reliableTrDimensions() && q(i, "tr") || $ === "auto" || !parseFloat($) && u.css(i, "display", !1, x) === "inline") && i.getClientRects().length && (I = u.css(i, "boxSizing", !1, x) === "border-box", E = U in i, E && ($ = i[U])), $ = parseFloat($) || 0, $ + Hn(i, d, v || (I ? "border" : "content"), E, x, $) + "px"
+            return (!w.boxSizingReliable() && I || !w.reliableTrDimensions() && q(i, "tr") || $ === "auto" || !parseFloat($) && u.css(i, "display", !1, x) === "inline") && i.getClientRects().length && (I = u.css(i, "boxSizing", !1, x) === "border-box", E = U in i, E && ($ = i[U])), $ = parseFloat($) || 0, $ + Wn(i, d, v || (I ? "border" : "content"), E, x, $) + "px"
         }
         u.extend({
             cssHooks: {
                 opacity: {
                     get: function(i, d) {
                         if (d) {
                             var v = Rr(i, "opacity");
@@ -5407,67 +5407,67 @@
                 strokeMiterlimit: !0,
                 strokeOpacity: !0
             },
             cssProps: {},
             style: function(i, d, v, x) {
                 if (!(!i || i.nodeType === 3 || i.nodeType === 8 || !i.style)) {
                     var A, I, E, $ = gt(d),
-                        U = Mn.test(d),
+                        U = Vn.test(d),
                         Q = i.style;
-                    if (U || (d = Vn($)), E = u.cssHooks[d] || u.cssHooks[$], v !== void 0) {
-                        if (I = typeof v, I === "string" && (A = te.exec(v)) && A[1] && (v = en(i, d, A), I = "number"), v == null || v !== v) return;
+                    if (U || (d = Hn($)), E = u.cssHooks[d] || u.cssHooks[$], v !== void 0) {
+                        if (I = typeof v, I === "string" && (A = te.exec(v)) && A[1] && (v = rn(i, d, A), I = "number"), v == null || v !== v) return;
                         I === "number" && !U && (v += A && A[3] || (u.cssNumber[$] ? "" : "px")), !w.clearCloneStyle && v === "" && d.indexOf("background") === 0 && (Q[d] = "inherit"), (!E || !("set" in E) || (v = E.set(i, v, x)) !== void 0) && (U ? Q.setProperty(d, v) : Q[d] = v)
                     } else return E && "get" in E && (A = E.get(i, !1, x)) !== void 0 ? A : Q[d]
                 }
             },
             css: function(i, d, v, x) {
                 var A, I, E, $ = gt(d),
-                    U = Mn.test(d);
-                return U || (d = Vn($)), E = u.cssHooks[d] || u.cssHooks[$], E && "get" in E && (A = E.get(i, !0, v)), A === void 0 && (A = Rr(i, d, x)), A === "normal" && d in ia && (A = ia[d]), v === "" || v ? (I = parseFloat(A), v === !0 || isFinite(I) ? I || 0 : A) : A
+                    U = Vn.test(d);
+                return U || (d = Hn($)), E = u.cssHooks[d] || u.cssHooks[$], E && "get" in E && (A = E.get(i, !0, v)), A === void 0 && (A = Rr(i, d, x)), A === "normal" && d in aa && (A = aa[d]), v === "" || v ? (I = parseFloat(A), v === !0 || isFinite(I) ? I || 0 : A) : A
             }
         }), u.each(["height", "width"], function(i, d) {
             u.cssHooks[d] = {
                 get: function(v, x, A) {
-                    if (x) return to.test(u.css(v, "display")) && (!v.getClientRects().length || !v.getBoundingClientRect().width) ? Ji(v, eo, function() {
-                        return sa(v, d, A)
-                    }) : sa(v, d, A)
+                    if (x) return eo.test(u.css(v, "display")) && (!v.getClientRects().length || !v.getBoundingClientRect().width) ? ta(v, ro, function() {
+                        return oa(v, d, A)
+                    }) : oa(v, d, A)
                 },
                 set: function(v, x, A) {
-                    var I, E = sn(v),
+                    var I, E = on(v),
                         $ = !w.scrollboxSize() && E.position === "absolute",
                         U = $ || A,
                         Q = U && u.css(v, "boxSizing", !1, E) === "border-box",
-                        dt = A ? Hn(v, d, A, Q, E) : 0;
-                    return Q && $ && (dt -= Math.ceil(v["offset" + d[0].toUpperCase() + d.slice(1)] - parseFloat(E[d]) - Hn(v, d, "border", !1, E) - .5)), dt && (I = te.exec(x)) && (I[3] || "px") !== "px" && (v.style[d] = x, x = u.css(v, d)), aa(v, x, dt)
+                        dt = A ? Wn(v, d, A, Q, E) : 0;
+                    return Q && $ && (dt -= Math.ceil(v["offset" + d[0].toUpperCase() + d.slice(1)] - parseFloat(E[d]) - Wn(v, d, "border", !1, E) - .5)), dt && (I = te.exec(x)) && (I[3] || "px") !== "px" && (v.style[d] = x, x = u.css(v, d)), sa(v, x, dt)
                 }
             }
-        }), u.cssHooks.marginLeft = ta(w.reliableMarginLeft, function(i, d) {
-            if (d) return (parseFloat(Rr(i, "marginLeft")) || i.getBoundingClientRect().left - Ji(i, {
+        }), u.cssHooks.marginLeft = ea(w.reliableMarginLeft, function(i, d) {
+            if (d) return (parseFloat(Rr(i, "marginLeft")) || i.getBoundingClientRect().left - ta(i, {
                 marginLeft: 0
             }, function() {
                 return i.getBoundingClientRect().left
             })) + "px"
         }), u.each({
             margin: "",
             padding: "",
             border: "Width"
         }, function(i, d) {
             u.cssHooks[i + d] = {
                 expand: function(v) {
                     for (var x = 0, A = {}, I = typeof v == "string" ? v.split(" ") : [v]; x < 4; x++) A[i + be[x] + d] = I[x] || I[x - 2] || I[0];
                     return A
                 }
-            }, i !== "margin" && (u.cssHooks[i + d].set = aa)
+            }, i !== "margin" && (u.cssHooks[i + d].set = sa)
         }), u.fn.extend({
             css: function(i, d) {
                 return Y(this, function(v, x, A) {
                     var I, E, $ = {},
                         U = 0;
                     if (Array.isArray(x)) {
-                        for (I = sn(v), E = x.length; U < E; U++) $[x[U]] = u.css(v, x[U], !1, I);
+                        for (I = on(v), E = x.length; U < E; U++) $[x[U]] = u.css(v, x[U], !1, I);
                         return $
                     }
                     return A !== void 0 ? u.style(v, x, A) : u.css(v, x)
                 }, i, d, arguments.length > 1)
             }
         });
 
@@ -5490,15 +5490,15 @@
         }, me.prototype.init.prototype = me.prototype, me.propHooks = {
             _default: {
                 get: function(i) {
                     var d;
                     return i.elem.nodeType !== 1 || i.elem[i.prop] != null && i.elem.style[i.prop] == null ? i.elem[i.prop] : (d = u.css(i.elem, i.prop, ""), !d || d === "auto" ? 0 : d)
                 },
                 set: function(i) {
-                    u.fx.step[i.prop] ? u.fx.step[i.prop](i) : i.elem.nodeType === 1 && (u.cssHooks[i.prop] || i.elem.style[Vn(i.prop)] != null) ? u.style(i.elem, i.prop, i.now + i.unit) : i.elem[i.prop] = i.now
+                    u.fx.step[i.prop] ? u.fx.step[i.prop](i) : i.elem.nodeType === 1 && (u.cssHooks[i.prop] || i.elem.style[Hn(i.prop)] != null) ? u.style(i.elem, i.prop, i.now + i.unit) : i.elem[i.prop] = i.now
                 }
             }
         }, me.propHooks.scrollTop = me.propHooks.scrollLeft = {
             set: function(i) {
                 i.elem.nodeType && i.elem.parentNode && (i.elem[i.prop] = i.now)
             }
         }, u.easing = {
@@ -5506,57 +5506,57 @@
                 return i
             },
             swing: function(i) {
                 return .5 - Math.cos(i * Math.PI) / 2
             },
             _default: "swing"
         }, u.fx = me.prototype.init, u.fx.step = {};
-        var _r, on, ro = /^(?:toggle|show|hide)$/,
-            no = /queueHooks$/;
+        var _r, ln, no = /^(?:toggle|show|hide)$/,
+            io = /queueHooks$/;
 
-        function Wn() {
-            on && (F.hidden === !1 && t.requestAnimationFrame ? t.requestAnimationFrame(Wn) : t.setTimeout(Wn, u.fx.interval), u.fx.tick())
+        function Un() {
+            ln && (F.hidden === !1 && t.requestAnimationFrame ? t.requestAnimationFrame(Un) : t.setTimeout(Un, u.fx.interval), u.fx.tick())
         }
 
-        function oa() {
+        function la() {
             return t.setTimeout(function() {
                 _r = void 0
             }), _r = Date.now()
         }
 
-        function ln(i, d) {
+        function dn(i, d) {
             var v, x = 0,
                 A = {
                     height: i
                 };
             for (d = d ? 1 : 0; x < 4; x += 2 - d) v = be[x], A["margin" + v] = A["padding" + v] = i;
             return d && (A.opacity = A.width = i), A
         }
 
-        function la(i, d, v) {
+        function da(i, d, v) {
             for (var x, A = (Re.tweeners[d] || []).concat(Re.tweeners["*"]), I = 0, E = A.length; I < E; I++)
                 if (x = A[I].call(v, d, i)) return x
         }
 
-        function io(i, d, v) {
+        function ao(i, d, v) {
             var x, A, I, E, $, U, Q, dt, ft = "width" in d || "height" in d,
                 it = this,
                 wt = {},
                 Et = i.style,
                 Gt = i.nodeType && gr(i),
                 Mt = bt.get(i, "fxshow");
             v.queue || (E = u._queueHooks(i, "fx"), E.unqueued == null && (E.unqueued = 0, $ = E.empty.fire, E.empty.fire = function() {
                 E.unqueued || $()
             }), E.unqueued++, it.always(function() {
                 it.always(function() {
                     E.unqueued--, u.queue(i, "fx").length || E.empty.fire()
                 })
             }));
             for (x in d)
-                if (A = d[x], ro.test(A)) {
+                if (A = d[x], no.test(A)) {
                     if (delete d[x], I = I || A === "toggle", A === (Gt ? "hide" : "show"))
                         if (A === "show" && Mt && Mt[x] !== void 0) Gt = !0;
                         else continue;
                     wt[x] = Mt && Mt[x] || u.style(i, x)
                 } if (U = !u.isEmptyObject(d), !(!U && u.isEmptyObject(wt))) {
                 ft && i.nodeType === 1 && (v.overflow = [Et.overflow, Et.overflowX, Et.overflowY], Q = Mt && Mt.display, Q == null && (Q = bt.get(i, "display")), dt = u.css(i, "display"), dt === "none" && (Q ? dt = Q : (Te([i], !0), Q = i.style.display || Q, dt = u.css(i, "display"), Te([i]))), (dt === "inline" || dt === "inline-block" && Q != null) && u.css(i, "float") === "none" && (U || (it.done(function() {
                     Et.display = Q
@@ -5564,19 +5564,19 @@
                     Et.overflow = v.overflow[0], Et.overflowX = v.overflow[1], Et.overflowY = v.overflow[2]
                 })), U = !1;
                 for (x in wt) U || (Mt ? "hidden" in Mt && (Gt = Mt.hidden) : Mt = bt.access(i, "fxshow", {
                     display: Q
                 }), I && (Mt.hidden = !Gt), Gt && Te([i], !0), it.done(function() {
                     Gt || Te([i]), bt.remove(i, "fxshow");
                     for (x in wt) u.style(i, x, wt[x])
-                })), U = la(Gt ? Mt[x] : 0, x, it), x in Mt || (Mt[x] = U.start, Gt && (U.end = U.start, U.start = 0))
+                })), U = da(Gt ? Mt[x] : 0, x, it), x in Mt || (Mt[x] = U.start, Gt && (U.end = U.start, U.start = 0))
             }
         }
 
-        function ao(i, d) {
+        function so(i, d) {
             var v, x, A, I, E;
             for (v in i)
                 if (x = gt(v), A = d[x], I = i[v], Array.isArray(I) && (A = I[1], I = i[v] = I[0]), v !== x && (i[x] = I, delete i[v]), E = u.cssHooks[x], E && "expand" in E) {
                     I = E.expand(I), delete i[x];
                     for (v in I) v in i || (i[v] = I[v], d[v] = A)
                 } else d[x] = A
         }
@@ -5585,27 +5585,27 @@
             var x, A, I = 0,
                 E = Re.prefilters.length,
                 $ = u.Deferred().always(function() {
                     delete U.elem
                 }),
                 U = function() {
                     if (A) return !1;
-                    for (var ft = _r || oa(), it = Math.max(0, Q.startTime + Q.duration - ft), wt = it / Q.duration || 0, Et = 1 - wt, Gt = 0, Mt = Q.tweens.length; Gt < Mt; Gt++) Q.tweens[Gt].run(Et);
+                    for (var ft = _r || la(), it = Math.max(0, Q.startTime + Q.duration - ft), wt = it / Q.duration || 0, Et = 1 - wt, Gt = 0, Mt = Q.tweens.length; Gt < Mt; Gt++) Q.tweens[Gt].run(Et);
                     return $.notifyWith(i, [Q, Et, it]), Et < 1 && Mt ? it : (Mt || $.notifyWith(i, [Q, 1, 0]), $.resolveWith(i, [Q]), !1)
                 },
                 Q = $.promise({
                     elem: i,
                     props: u.extend({}, d),
                     opts: u.extend(!0, {
                         specialEasing: {},
                         easing: u.easing._default
                     }, v),
                     originalProperties: d,
                     originalOptions: v,
-                    startTime: _r || oa(),
+                    startTime: _r || la(),
                     duration: v.duration,
                     tweens: [],
                     createTween: function(ft, it) {
                         var wt = u.Tween(i, Q.opts, ft, it, Q.opts.specialEasing[ft] || Q.opts.easing);
                         return Q.tweens.push(wt), wt
                     },
                     stop: function(ft) {
@@ -5613,34 +5613,34 @@
                             wt = ft ? Q.tweens.length : 0;
                         if (A) return this;
                         for (A = !0; it < wt; it++) Q.tweens[it].run(1);
                         return ft ? ($.notifyWith(i, [Q, 1, 0]), $.resolveWith(i, [Q, ft])) : $.rejectWith(i, [Q, ft]), this
                     }
                 }),
                 dt = Q.props;
-            for (ao(dt, Q.opts.specialEasing); I < E; I++)
+            for (so(dt, Q.opts.specialEasing); I < E; I++)
                 if (x = Re.prefilters[I].call(Q, i, dt, Q.opts), x) return k(x.stop) && (u._queueHooks(Q.elem, Q.opts.queue).stop = x.stop.bind(x)), x;
-            return u.map(dt, la, Q), k(Q.opts.start) && Q.opts.start.call(i, Q), Q.progress(Q.opts.progress).done(Q.opts.done, Q.opts.complete).fail(Q.opts.fail).always(Q.opts.always), u.fx.timer(u.extend(U, {
+            return u.map(dt, da, Q), k(Q.opts.start) && Q.opts.start.call(i, Q), Q.progress(Q.opts.progress).done(Q.opts.done, Q.opts.complete).fail(Q.opts.fail).always(Q.opts.always), u.fx.timer(u.extend(U, {
                 elem: i,
                 anim: Q,
                 queue: Q.opts.queue
             })), Q
         }
         u.Animation = u.extend(Re, {
                 tweeners: {
                     "*": [function(i, d) {
                         var v = this.createTween(i, d);
-                        return en(v.elem, i, te.exec(d), v), v
+                        return rn(v.elem, i, te.exec(d), v), v
                     }]
                 },
                 tweener: function(i, d) {
                     k(i) ? (d = i, i = ["*"]) : i = i.match(Bt);
                     for (var v, x = 0, A = i.length; x < A; x++) v = i[x], Re.tweeners[v] = Re.tweeners[v] || [], Re.tweeners[v].unshift(d)
                 },
-                prefilters: [io],
+                prefilters: [ao],
                 prefilter: function(i, d) {
                     d ? Re.prefilters.unshift(i) : Re.prefilters.push(i)
                 }
             }), u.speed = function(i, d, v) {
                 var x = i && typeof i == "object" ? u.extend({}, i) : {
                     complete: v || !v && d || k(i) && i,
                     duration: i,
@@ -5672,15 +5672,15 @@
                     return typeof i != "string" && (v = d, d = i, i = void 0), d && this.queue(i || "fx", []), this.each(function() {
                         var A = !0,
                             I = i != null && i + "queueHooks",
                             E = u.timers,
                             $ = bt.get(this);
                         if (I) $[I] && $[I].stop && x($[I]);
                         else
-                            for (I in $) $[I] && $[I].stop && no.test(I) && x($[I]);
+                            for (I in $) $[I] && $[I].stop && io.test(I) && x($[I]);
                         for (I = E.length; I--;) E[I].elem === this && (i == null || E[I].queue === i) && (E[I].anim.stop(v), A = !1, E.splice(I, 1));
                         (A || !v) && u.dequeue(this, i)
                     })
                 },
                 finish: function(i) {
                     return i !== !1 && (i = i || "fx"), this.each(function() {
                         var d, v = bt.get(this),
@@ -5692,20 +5692,20 @@
                         for (d = 0; d < E; d++) x[d] && x[d].finish && x[d].finish.call(this);
                         delete v.finish
                     })
                 }
             }), u.each(["toggle", "show", "hide"], function(i, d) {
                 var v = u.fn[d];
                 u.fn[d] = function(x, A, I) {
-                    return x == null || typeof x == "boolean" ? v.apply(this, arguments) : this.animate(ln(d, !0), x, A, I)
+                    return x == null || typeof x == "boolean" ? v.apply(this, arguments) : this.animate(dn(d, !0), x, A, I)
                 }
             }), u.each({
-                slideDown: ln("show"),
-                slideUp: ln("hide"),
-                slideToggle: ln("toggle"),
+                slideDown: dn("show"),
+                slideUp: dn("hide"),
+                slideToggle: dn("toggle"),
                 fadeIn: {
                     opacity: "show"
                 },
                 fadeOut: {
                     opacity: "hide"
                 },
                 fadeToggle: {
@@ -5719,17 +5719,17 @@
                 var i, d = 0,
                     v = u.timers;
                 for (_r = Date.now(); d < v.length; d++) i = v[d], !i() && v[d] === i && v.splice(d--, 1);
                 v.length || u.fx.stop(), _r = void 0
             }, u.fx.timer = function(i) {
                 u.timers.push(i), u.fx.start()
             }, u.fx.interval = 13, u.fx.start = function() {
-                on || (on = !0, Wn())
+                ln || (ln = !0, Un())
             }, u.fx.stop = function() {
-                on = null
+                ln = null
             }, u.fx.speeds = {
                 slow: 600,
                 fast: 200,
                 _default: 400
             }, u.fn.delay = function(i, d) {
                 return i = u.fx && u.fx.speeds[i] || i, d = d || "fx", this.queue(d, function(v, x) {
                     var A = t.setTimeout(v, i);
@@ -5740,30 +5740,30 @@
             },
             function() {
                 var i = F.createElement("input"),
                     d = F.createElement("select"),
                     v = d.appendChild(F.createElement("option"));
                 i.type = "checkbox", w.checkOn = i.value !== "", w.optSelected = v.selected, i = F.createElement("input"), i.value = "t", i.type = "radio", w.radioValue = i.value === "t"
             }();
-        var da, Lr = u.expr.attrHandle;
+        var ua, Lr = u.expr.attrHandle;
         u.fn.extend({
             attr: function(i, d) {
                 return Y(this, u.attr, i, d, arguments.length > 1)
             },
             removeAttr: function(i) {
                 return this.each(function() {
                     u.removeAttr(this, i)
                 })
             }
         }), u.extend({
             attr: function(i, d, v) {
                 var x, A, I = i.nodeType;
                 if (!(I === 3 || I === 8 || I === 2)) {
                     if (typeof i.getAttribute > "u") return u.prop(i, d, v);
-                    if ((I !== 1 || !u.isXMLDoc(i)) && (A = u.attrHooks[d.toLowerCase()] || (u.expr.match.bool.test(d) ? da : void 0)), v !== void 0) {
+                    if ((I !== 1 || !u.isXMLDoc(i)) && (A = u.attrHooks[d.toLowerCase()] || (u.expr.match.bool.test(d) ? ua : void 0)), v !== void 0) {
                         if (v === null) {
                             u.removeAttr(i, d);
                             return
                         }
                         return A && "set" in A && (x = A.set(i, v, d)) !== void 0 ? x : (i.setAttribute(d, v + ""), v)
                     }
                     return A && "get" in A && (x = A.get(i, d)) !== null ? x : (x = u.find.attr(i, d), x ?? void 0)
@@ -5781,27 +5781,27 @@
             },
             removeAttr: function(i, d) {
                 var v, x = 0,
                     A = d && d.match(Bt);
                 if (A && i.nodeType === 1)
                     for (; v = A[x++];) i.removeAttribute(v)
             }
-        }), da = {
+        }), ua = {
             set: function(i, d, v) {
                 return d === !1 ? u.removeAttr(i, v) : i.setAttribute(v, v), v
             }
         }, u.each(u.expr.match.bool.source.match(/\w+/g), function(i, d) {
             var v = Lr[d] || u.find.attr;
             Lr[d] = function(x, A, I) {
                 var E, $, U = A.toLowerCase();
                 return I || ($ = Lr[U], Lr[U] = E, E = v(x, A, I) != null ? U : null, Lr[U] = $), E
             }
         });
-        var so = /^(?:input|select|textarea|button)$/i,
-            oo = /^(?:a|area)$/i;
+        var oo = /^(?:input|select|textarea|button)$/i,
+            lo = /^(?:a|area)$/i;
         u.fn.extend({
             prop: function(i, d) {
                 return Y(this, u.prop, i, d, arguments.length > 1)
             },
             removeProp: function(i) {
                 return this.each(function() {
                     delete this[u.propFix[i] || i]
@@ -5812,15 +5812,15 @@
                 var x, A, I = i.nodeType;
                 if (!(I === 3 || I === 8 || I === 2)) return (I !== 1 || !u.isXMLDoc(i)) && (d = u.propFix[d] || d, A = u.propHooks[d]), v !== void 0 ? A && "set" in A && (x = A.set(i, v, d)) !== void 0 ? x : i[d] = v : A && "get" in A && (x = A.get(i, d)) !== null ? x : i[d]
             },
             propHooks: {
                 tabIndex: {
                     get: function(i) {
                         var d = u.find.attr(i, "tabindex");
-                        return d ? parseInt(d, 10) : so.test(i.nodeName) || oo.test(i.nodeName) && i.href ? 0 : -1
+                        return d ? parseInt(d, 10) : oo.test(i.nodeName) || lo.test(i.nodeName) && i.href ? 0 : -1
                     }
                 }
             },
             propFix: {
                 for: "htmlFor",
                 class: "className"
             }
@@ -5842,69 +5842,69 @@
             return d.join(" ")
         }
 
         function lr(i) {
             return i.getAttribute && i.getAttribute("class") || ""
         }
 
-        function Un(i) {
+        function qn(i) {
             return Array.isArray(i) ? i : typeof i == "string" ? i.match(Bt) || [] : []
         }
         u.fn.extend({
             addClass: function(i) {
                 var d, v, x, A, I, E;
                 return k(i) ? this.each(function($) {
                     u(this).addClass(i.call(this, $, lr(this)))
-                }) : (d = Un(i), d.length ? this.each(function() {
+                }) : (d = qn(i), d.length ? this.each(function() {
                     if (x = lr(this), v = this.nodeType === 1 && " " + or(x) + " ", v) {
                         for (I = 0; I < d.length; I++) A = d[I], v.indexOf(" " + A + " ") < 0 && (v += A + " ");
                         E = or(v), x !== E && this.setAttribute("class", E)
                     }
                 }) : this)
             },
             removeClass: function(i) {
                 var d, v, x, A, I, E;
                 return k(i) ? this.each(function($) {
                     u(this).removeClass(i.call(this, $, lr(this)))
-                }) : arguments.length ? (d = Un(i), d.length ? this.each(function() {
+                }) : arguments.length ? (d = qn(i), d.length ? this.each(function() {
                     if (x = lr(this), v = this.nodeType === 1 && " " + or(x) + " ", v) {
                         for (I = 0; I < d.length; I++)
                             for (A = d[I]; v.indexOf(" " + A + " ") > -1;) v = v.replace(" " + A + " ", " ");
                         E = or(v), x !== E && this.setAttribute("class", E)
                     }
                 }) : this) : this.attr("class", "")
             },
             toggleClass: function(i, d) {
                 var v, x, A, I, E = typeof i,
                     $ = E === "string" || Array.isArray(i);
                 return k(i) ? this.each(function(U) {
                     u(this).toggleClass(i.call(this, U, lr(this), d), d)
-                }) : typeof d == "boolean" && $ ? d ? this.addClass(i) : this.removeClass(i) : (v = Un(i), this.each(function() {
+                }) : typeof d == "boolean" && $ ? d ? this.addClass(i) : this.removeClass(i) : (v = qn(i), this.each(function() {
                     if ($)
                         for (I = u(this), A = 0; A < v.length; A++) x = v[A], I.hasClass(x) ? I.removeClass(x) : I.addClass(x);
                     else(i === void 0 || E === "boolean") && (x = lr(this), x && bt.set(this, "__className__", x), this.setAttribute && this.setAttribute("class", x || i === !1 ? "" : bt.get(this, "__className__") || ""))
                 }))
             },
             hasClass: function(i) {
                 var d, v, x = 0;
                 for (d = " " + i + " "; v = this[x++];)
                     if (v.nodeType === 1 && (" " + or(lr(v)) + " ").indexOf(d) > -1) return !0;
                 return !1
             }
         });
-        var lo = /\r/g;
+        var uo = /\r/g;
         u.fn.extend({
             val: function(i) {
                 var d, v, x, A = this[0];
                 return arguments.length ? (x = k(i), this.each(function(I) {
                     var E;
                     this.nodeType === 1 && (x ? E = i.call(this, I, u(this).val()) : E = i, E == null ? E = "" : typeof E == "number" ? E += "" : Array.isArray(E) && (E = u.map(E, function($) {
                         return $ == null ? "" : $ + ""
                     })), d = u.valHooks[this.type] || u.valHooks[this.nodeName.toLowerCase()], (!d || !("set" in d) || d.set(this, E, "value") === void 0) && (this.value = E))
-                })) : A ? (d = u.valHooks[A.type] || u.valHooks[A.nodeName.toLowerCase()], d && "get" in d && (v = d.get(A, "value")) !== void 0 ? v : (v = A.value, typeof v == "string" ? v.replace(lo, "") : v ?? "")) : void 0
+                })) : A ? (d = u.valHooks[A.type] || u.valHooks[A.nodeName.toLowerCase()], d && "get" in d && (v = d.get(A, "value")) !== void 0 ? v : (v = A.value, typeof v == "string" ? v.replace(uo, "") : v ?? "")) : void 0
             }
         }), u.extend({
             valHooks: {
                 option: {
                     get: function(i) {
                         var d = u.find.attr(i, "value");
                         return d ?? or(u.text(i))
@@ -5935,46 +5935,46 @@
                     if (Array.isArray(d)) return i.checked = u.inArray(u(i).val(), d) > -1
                 }
             }, w.checkOn || (u.valHooks[this].get = function(i) {
                 return i.getAttribute("value") === null ? "on" : i.value
             })
         });
         var zr = t.location,
-            ua = {
+            ca = {
                 guid: Date.now()
             },
-            qn = /\?/;
+            Gn = /\?/;
         u.parseXML = function(i) {
             var d, v;
             if (!i || typeof i != "string") return null;
             try {
                 d = new t.DOMParser().parseFromString(i, "text/xml")
             } catch {}
             return v = d && d.getElementsByTagName("parsererror")[0], (!d || v) && u.error("Invalid XML: " + (v ? u.map(v.childNodes, function(x) {
                 return x.textContent
             }).join(`
 `) : i)), d
         };
-        var ca = /^(?:focusinfocus|focusoutblur)$/,
-            fa = function(i) {
+        var fa = /^(?:focusinfocus|focusoutblur)$/,
+            ha = function(i) {
                 i.stopPropagation()
             };
         u.extend(u.event, {
             trigger: function(i, d, v, x) {
                 var A, I, E, $, U, Q, dt, ft, it = [v || F],
                     wt = m.call(i, "type") ? i.type : i,
                     Et = m.call(i, "namespace") ? i.namespace.split(".") : [];
-                if (I = ft = E = v = v || F, !(v.nodeType === 3 || v.nodeType === 8) && !ca.test(wt + u.event.triggered) && (wt.indexOf(".") > -1 && (Et = wt.split("."), wt = Et.shift(), Et.sort()), U = wt.indexOf(":") < 0 && "on" + wt, i = i[u.expando] ? i : new u.Event(wt, typeof i == "object" && i), i.isTrigger = x ? 2 : 3, i.namespace = Et.join("."), i.rnamespace = i.namespace ? new RegExp("(^|\\.)" + Et.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, i.result = void 0, i.target || (i.target = v), d = d == null ? [i] : u.makeArray(d, [i]), dt = u.event.special[wt] || {}, !(!x && dt.trigger && dt.trigger.apply(v, d) === !1))) {
+                if (I = ft = E = v = v || F, !(v.nodeType === 3 || v.nodeType === 8) && !fa.test(wt + u.event.triggered) && (wt.indexOf(".") > -1 && (Et = wt.split("."), wt = Et.shift(), Et.sort()), U = wt.indexOf(":") < 0 && "on" + wt, i = i[u.expando] ? i : new u.Event(wt, typeof i == "object" && i), i.isTrigger = x ? 2 : 3, i.namespace = Et.join("."), i.rnamespace = i.namespace ? new RegExp("(^|\\.)" + Et.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, i.result = void 0, i.target || (i.target = v), d = d == null ? [i] : u.makeArray(d, [i]), dt = u.event.special[wt] || {}, !(!x && dt.trigger && dt.trigger.apply(v, d) === !1))) {
                     if (!x && !dt.noBubble && !P(v)) {
-                        for ($ = dt.delegateType || wt, ca.test($ + wt) || (I = I.parentNode); I; I = I.parentNode) it.push(I), E = I;
+                        for ($ = dt.delegateType || wt, fa.test($ + wt) || (I = I.parentNode); I; I = I.parentNode) it.push(I), E = I;
                         E === (v.ownerDocument || F) && it.push(E.defaultView || E.parentWindow || t)
                     }
                     for (A = 0;
                         (I = it[A++]) && !i.isPropagationStopped();) ft = I, i.type = A > 1 ? $ : dt.bindType || wt, Q = (bt.get(I, "events") || Object.create(null))[i.type] && bt.get(I, "handle"), Q && Q.apply(I, d), Q = U && I[U], Q && Q.apply && Ct(I) && (i.result = Q.apply(I, d), i.result === !1 && i.preventDefault());
-                    return i.type = wt, !x && !i.isDefaultPrevented() && (!dt._default || dt._default.apply(it.pop(), d) === !1) && Ct(v) && U && k(v[wt]) && !P(v) && (E = v[U], E && (v[U] = null), u.event.triggered = wt, i.isPropagationStopped() && ft.addEventListener(wt, fa), v[wt](), i.isPropagationStopped() && ft.removeEventListener(wt, fa), u.event.triggered = void 0, E && (v[U] = E)), i.result
+                    return i.type = wt, !x && !i.isDefaultPrevented() && (!dt._default || dt._default.apply(it.pop(), d) === !1) && Ct(v) && U && k(v[wt]) && !P(v) && (E = v[U], E && (v[U] = null), u.event.triggered = wt, i.isPropagationStopped() && ft.addEventListener(wt, ha), v[wt](), i.isPropagationStopped() && ft.removeEventListener(wt, ha), u.event.triggered = void 0, E && (v[U] = E)), i.result
                 }
             },
             simulate: function(i, d, v) {
                 var x = u.extend(new u.Event, v, {
                     type: i,
                     isSimulated: !0
                 });
@@ -5987,113 +5987,113 @@
                 })
             },
             triggerHandler: function(i, d) {
                 var v = this[0];
                 if (v) return u.event.trigger(i, d, v, !0)
             }
         });
-        var uo = /\[\]$/,
-            ha = /\r?\n/g,
-            co = /^(?:submit|button|image|reset|file)$/i,
-            fo = /^(?:input|select|textarea|keygen)/i;
+        var co = /\[\]$/,
+            pa = /\r?\n/g,
+            fo = /^(?:submit|button|image|reset|file)$/i,
+            ho = /^(?:input|select|textarea|keygen)/i;
 
-        function Gn(i, d, v, x) {
+        function Xn(i, d, v, x) {
             var A;
             if (Array.isArray(d)) u.each(d, function(I, E) {
-                v || uo.test(i) ? x(i, E) : Gn(i + "[" + (typeof E == "object" && E != null ? I : "") + "]", E, v, x)
+                v || co.test(i) ? x(i, E) : Xn(i + "[" + (typeof E == "object" && E != null ? I : "") + "]", E, v, x)
             });
             else if (!v && f(d) === "object")
-                for (A in d) Gn(i + "[" + A + "]", d[A], v, x);
+                for (A in d) Xn(i + "[" + A + "]", d[A], v, x);
             else x(i, d)
         }
         u.param = function(i, d) {
             var v, x = [],
                 A = function(I, E) {
                     var $ = k(E) ? E() : E;
                     x[x.length] = encodeURIComponent(I) + "=" + encodeURIComponent($ ?? "")
                 };
             if (i == null) return "";
             if (Array.isArray(i) || i.jquery && !u.isPlainObject(i)) u.each(i, function() {
                 A(this.name, this.value)
             });
             else
-                for (v in i) Gn(v, i[v], d, A);
+                for (v in i) Xn(v, i[v], d, A);
             return x.join("&")
         }, u.fn.extend({
             serialize: function() {
                 return u.param(this.serializeArray())
             },
             serializeArray: function() {
                 return this.map(function() {
                     var i = u.prop(this, "elements");
                     return i ? u.makeArray(i) : this
                 }).filter(function() {
                     var i = this.type;
-                    return this.name && !u(this).is(":disabled") && fo.test(this.nodeName) && !co.test(i) && (this.checked || !je.test(i))
+                    return this.name && !u(this).is(":disabled") && ho.test(this.nodeName) && !fo.test(i) && (this.checked || !je.test(i))
                 }).map(function(i, d) {
                     var v = u(this).val();
                     return v == null ? null : Array.isArray(v) ? u.map(v, function(x) {
                         return {
                             name: d.name,
-                            value: x.replace(ha, `\r
+                            value: x.replace(pa, `\r
 `)
                         }
                     }) : {
                         name: d.name,
-                        value: v.replace(ha, `\r
+                        value: v.replace(pa, `\r
 `)
                     }
                 }).get()
             }
         });
-        var ho = /%20/g,
-            po = /#.*$/,
-            bo = /([?&])_=[^&]*/,
-            vo = /^(.*?):[ \t]*([^\r\n]*)$/mg,
-            mo = /^(?:about|app|app-storage|.+-extension|file|res|widget):$/,
-            go = /^(?:GET|HEAD)$/,
-            yo = /^\/\//,
-            pa = {},
-            Xn = {},
-            ba = "*/".concat("*"),
-            $n = F.createElement("a");
-        $n.href = zr.href;
+        var po = /%20/g,
+            bo = /#.*$/,
+            vo = /([?&])_=[^&]*/,
+            mo = /^(.*?):[ \t]*([^\r\n]*)$/mg,
+            go = /^(?:about|app|app-storage|.+-extension|file|res|widget):$/,
+            yo = /^(?:GET|HEAD)$/,
+            wo = /^\/\//,
+            ba = {},
+            $n = {},
+            va = "*/".concat("*"),
+            Zn = F.createElement("a");
+        Zn.href = zr.href;
 
-        function va(i) {
+        function ma(i) {
             return function(d, v) {
                 typeof d != "string" && (v = d, d = "*");
                 var x, A = 0,
                     I = d.toLowerCase().match(Bt) || [];
                 if (k(v))
                     for (; x = I[A++];) x[0] === "+" ? (x = x.slice(1) || "*", (i[x] = i[x] || []).unshift(v)) : (i[x] = i[x] || []).push(v)
             }
         }
 
-        function ma(i, d, v, x) {
+        function ga(i, d, v, x) {
             var A = {},
-                I = i === Xn;
+                I = i === $n;
 
             function E($) {
                 var U;
                 return A[$] = !0, u.each(i[$] || [], function(Q, dt) {
                     var ft = dt(d, v, x);
                     if (typeof ft == "string" && !I && !A[ft]) return d.dataTypes.unshift(ft), E(ft), !1;
                     if (I) return !(U = ft)
                 }), U
             }
             return E(d.dataTypes[0]) || !A["*"] && E("*")
         }
 
-        function Zn(i, d) {
+        function Kn(i, d) {
             var v, x, A = u.ajaxSettings.flatOptions || {};
             for (v in d) d[v] !== void 0 && ((A[v] ? i : x || (x = {}))[v] = d[v]);
             return x && u.extend(!0, i, x), i
         }
 
-        function wo(i, d, v) {
+        function xo(i, d, v) {
             for (var x, A, I, E, $ = i.contents, U = i.dataTypes; U[0] === "*";) U.shift(), x === void 0 && (x = i.mimeType || d.getResponseHeader("Content-Type"));
             if (x) {
                 for (A in $)
                     if ($[A] && $[A].test(x)) {
                         U.unshift(A);
                         break
                     }
@@ -6108,15 +6108,15 @@
                     E || (E = A)
                 }
                 I = I || E
             }
             if (I) return I !== U[0] && U.unshift(I), v[I]
         }
 
-        function xo(i, d, v, x) {
+        function _o(i, d, v, x) {
             var A, I, E, $, U, Q = {},
                 dt = i.dataTypes.slice();
             if (dt[1])
                 for (E in i.converters) Q[E.toLowerCase()] = i.converters[E];
             for (I = dt.shift(); I;)
                 if (i.responseFields[I] && (v[i.responseFields[I]] = d), !U && x && i.dataFilter && (d = i.dataFilter(d, i.dataType)), U = I, I = dt.shift(), I) {
                     if (I === "*") I = U;
@@ -6147,21 +6147,21 @@
         u.extend({
             active: 0,
             lastModified: {},
             etag: {},
             ajaxSettings: {
                 url: zr.href,
                 type: "GET",
-                isLocal: mo.test(zr.protocol),
+                isLocal: go.test(zr.protocol),
                 global: !0,
                 processData: !0,
                 async: !0,
                 contentType: "application/x-www-form-urlencoded; charset=UTF-8",
                 accepts: {
-                    "*": ba,
+                    "*": va,
                     text: "text/plain",
                     html: "text/html",
                     xml: "application/xml, text/xml",
                     json: "application/json, text/javascript"
                 },
                 contents: {
                     xml: /\bxml\b/,
@@ -6181,18 +6181,18 @@
                 },
                 flatOptions: {
                     url: !0,
                     context: !0
                 }
             },
             ajaxSetup: function(i, d) {
-                return d ? Zn(Zn(i, u.ajaxSettings), d) : Zn(u.ajaxSettings, i)
+                return d ? Kn(Kn(i, u.ajaxSettings), d) : Kn(u.ajaxSettings, i)
             },
-            ajaxPrefilter: va(pa),
-            ajaxTransport: va(Xn),
+            ajaxPrefilter: ma(ba),
+            ajaxTransport: ma($n),
             ajax: function(i, d) {
                 typeof i == "object" && (d = i, i = void 0), d = d || {};
                 var v, x, A, I, E, $, U, Q, dt, ft, it = u.ajaxSetup({}, d),
                     wt = it.context || it,
                     Et = it.context && (wt.nodeType || wt.jquery) ? u(wt) : u.event,
                     Gt = u.Deferred(),
                     Mt = u.Callbacks("once memory"),
@@ -6202,15 +6202,15 @@
                     Ve = "canceled",
                     qt = {
                         readyState: 0,
                         getResponseHeader: function(Xt) {
                             var re;
                             if (U) {
                                 if (!I)
-                                    for (I = {}; re = vo.exec(A);) I[re[1].toLowerCase() + " "] = (I[re[1].toLowerCase() + " "] || []).concat(re[2]);
+                                    for (I = {}; re = mo.exec(A);) I[re[1].toLowerCase() + " "] = (I[re[1].toLowerCase() + " "] || []).concat(re[2]);
                                 re = I[Xt.toLowerCase() + " "]
                             }
                             return re == null ? null : re.join(", ")
                         },
                         getAllResponseHeaders: function() {
                             return U ? A : null
                         },
@@ -6229,43 +6229,43 @@
                             return this
                         },
                         abort: function(Xt) {
                             var re = Xt || Ve;
                             return v && v.abort(re), dr(0, re), this
                         }
                     };
-                if (Gt.promise(qt), it.url = ((i || it.url || zr.href) + "").replace(yo, zr.protocol + "//"), it.type = d.method || d.type || it.method || it.type, it.dataTypes = (it.dataType || "*").toLowerCase().match(Bt) || [""], it.crossDomain == null) {
+                if (Gt.promise(qt), it.url = ((i || it.url || zr.href) + "").replace(wo, zr.protocol + "//"), it.type = d.method || d.type || it.method || it.type, it.dataTypes = (it.dataType || "*").toLowerCase().match(Bt) || [""], it.crossDomain == null) {
                     $ = F.createElement("a");
                     try {
-                        $.href = it.url, $.href = $.href, it.crossDomain = $n.protocol + "//" + $n.host != $.protocol + "//" + $.host
+                        $.href = it.url, $.href = $.href, it.crossDomain = Zn.protocol + "//" + Zn.host != $.protocol + "//" + $.host
                     } catch {
                         it.crossDomain = !0
                     }
                 }
-                if (it.data && it.processData && typeof it.data != "string" && (it.data = u.param(it.data, it.traditional)), ma(pa, it, d, qt), U) return qt;
-                Q = u.event && it.global, Q && u.active++ === 0 && u.event.trigger("ajaxStart"), it.type = it.type.toUpperCase(), it.hasContent = !go.test(it.type), x = it.url.replace(po, ""), it.hasContent ? it.data && it.processData && (it.contentType || "").indexOf("application/x-www-form-urlencoded") === 0 && (it.data = it.data.replace(ho, "+")) : (ft = it.url.slice(x.length), it.data && (it.processData || typeof it.data == "string") && (x += (qn.test(x) ? "&" : "?") + it.data, delete it.data), it.cache === !1 && (x = x.replace(bo, "$1"), ft = (qn.test(x) ? "&" : "?") + "_=" + ua.guid++ + ft), it.url = x + ft), it.ifModified && (u.lastModified[x] && qt.setRequestHeader("If-Modified-Since", u.lastModified[x]), u.etag[x] && qt.setRequestHeader("If-None-Match", u.etag[x])), (it.data && it.hasContent && it.contentType !== !1 || d.contentType) && qt.setRequestHeader("Content-Type", it.contentType), qt.setRequestHeader("Accept", it.dataTypes[0] && it.accepts[it.dataTypes[0]] ? it.accepts[it.dataTypes[0]] + (it.dataTypes[0] !== "*" ? ", " + ba + "; q=0.01" : "") : it.accepts["*"]);
+                if (it.data && it.processData && typeof it.data != "string" && (it.data = u.param(it.data, it.traditional)), ga(ba, it, d, qt), U) return qt;
+                Q = u.event && it.global, Q && u.active++ === 0 && u.event.trigger("ajaxStart"), it.type = it.type.toUpperCase(), it.hasContent = !yo.test(it.type), x = it.url.replace(bo, ""), it.hasContent ? it.data && it.processData && (it.contentType || "").indexOf("application/x-www-form-urlencoded") === 0 && (it.data = it.data.replace(po, "+")) : (ft = it.url.slice(x.length), it.data && (it.processData || typeof it.data == "string") && (x += (Gn.test(x) ? "&" : "?") + it.data, delete it.data), it.cache === !1 && (x = x.replace(vo, "$1"), ft = (Gn.test(x) ? "&" : "?") + "_=" + ca.guid++ + ft), it.url = x + ft), it.ifModified && (u.lastModified[x] && qt.setRequestHeader("If-Modified-Since", u.lastModified[x]), u.etag[x] && qt.setRequestHeader("If-None-Match", u.etag[x])), (it.data && it.hasContent && it.contentType !== !1 || d.contentType) && qt.setRequestHeader("Content-Type", it.contentType), qt.setRequestHeader("Accept", it.dataTypes[0] && it.accepts[it.dataTypes[0]] ? it.accepts[it.dataTypes[0]] + (it.dataTypes[0] !== "*" ? ", " + va + "; q=0.01" : "") : it.accepts["*"]);
                 for (dt in it.headers) qt.setRequestHeader(dt, it.headers[dt]);
                 if (it.beforeSend && (it.beforeSend.call(wt, qt, it) === !1 || U)) return qt.abort();
-                if (Ve = "abort", Mt.add(it.complete), qt.done(it.success), qt.fail(it.error), v = ma(Xn, it, d, qt), !v) dr(-1, "No Transport");
+                if (Ve = "abort", Mt.add(it.complete), qt.done(it.success), qt.fail(it.error), v = ga($n, it, d, qt), !v) dr(-1, "No Transport");
                 else {
                     if (qt.readyState = 1, Q && Et.trigger("ajaxSend", [qt, it]), U) return qt;
                     it.async && it.timeout > 0 && (E = t.setTimeout(function() {
                         qt.abort("timeout")
                     }, it.timeout));
                     try {
                         U = !1, v.send(se, dr)
                     } catch (Xt) {
                         if (U) throw Xt;
                         dr(-1, Xt)
                     }
                 }
 
-                function dr(Xt, re, Mr, Yn) {
+                function dr(Xt, re, Mr, Qn) {
                     var He, Vr, We, Qe, Je, Se = re;
-                    U || (U = !0, E && t.clearTimeout(E), v = void 0, A = Yn || "", qt.readyState = Xt > 0 ? 4 : 0, He = Xt >= 200 && Xt < 300 || Xt === 304, Mr && (Qe = wo(it, qt, Mr)), !He && u.inArray("script", it.dataTypes) > -1 && u.inArray("json", it.dataTypes) < 0 && (it.converters["text script"] = function() {}), Qe = xo(it, Qe, qt, He), He ? (it.ifModified && (Je = qt.getResponseHeader("Last-Modified"), Je && (u.lastModified[x] = Je), Je = qt.getResponseHeader("etag"), Je && (u.etag[x] = Je)), Xt === 204 || it.type === "HEAD" ? Se = "nocontent" : Xt === 304 ? Se = "notmodified" : (Se = Qe.state, Vr = Qe.data, We = Qe.error, He = !We)) : (We = Se, (Xt || !Se) && (Se = "error", Xt < 0 && (Xt = 0))), qt.status = Xt, qt.statusText = (re || Se) + "", He ? Gt.resolveWith(wt, [Vr, Se, qt]) : Gt.rejectWith(wt, [qt, Se, We]), qt.statusCode(le), le = void 0, Q && Et.trigger(He ? "ajaxSuccess" : "ajaxError", [qt, it, He ? Vr : We]), Mt.fireWith(wt, [qt, Se]), Q && (Et.trigger("ajaxComplete", [qt, it]), --u.active || u.event.trigger("ajaxStop")))
+                    U || (U = !0, E && t.clearTimeout(E), v = void 0, A = Qn || "", qt.readyState = Xt > 0 ? 4 : 0, He = Xt >= 200 && Xt < 300 || Xt === 304, Mr && (Qe = xo(it, qt, Mr)), !He && u.inArray("script", it.dataTypes) > -1 && u.inArray("json", it.dataTypes) < 0 && (it.converters["text script"] = function() {}), Qe = _o(it, Qe, qt, He), He ? (it.ifModified && (Je = qt.getResponseHeader("Last-Modified"), Je && (u.lastModified[x] = Je), Je = qt.getResponseHeader("etag"), Je && (u.etag[x] = Je)), Xt === 204 || it.type === "HEAD" ? Se = "nocontent" : Xt === 304 ? Se = "notmodified" : (Se = Qe.state, Vr = Qe.data, We = Qe.error, He = !We)) : (We = Se, (Xt || !Se) && (Se = "error", Xt < 0 && (Xt = 0))), qt.status = Xt, qt.statusText = (re || Se) + "", He ? Gt.resolveWith(wt, [Vr, Se, qt]) : Gt.rejectWith(wt, [qt, Se, We]), qt.statusCode(le), le = void 0, Q && Et.trigger(He ? "ajaxSuccess" : "ajaxError", [qt, it, He ? Vr : We]), Mt.fireWith(wt, [qt, Se]), Q && (Et.trigger("ajaxComplete", [qt, it]), --u.active || u.event.trigger("ajaxStop")))
                 }
                 return qt
             },
             getJSON: function(i, d, v) {
                 return u.get(i, d, v, "json")
             },
             getScript: function(i, d) {
@@ -6332,15 +6332,15 @@
         }, u.expr.pseudos.visible = function(i) {
             return !!(i.offsetWidth || i.offsetHeight || i.getClientRects().length)
         }, u.ajaxSettings.xhr = function() {
             try {
                 return new t.XMLHttpRequest
             } catch {}
         };
-        var _o = {
+        var Co = {
                 0: 200,
                 1223: 204
             },
             jr = u.ajaxSettings.xhr();
         w.cors = !!jr && "withCredentials" in jr, w.ajax = jr = !!jr, u.ajaxTransport(function(i) {
             var d, v;
             if (w.cors || jr && !i.crossDomain) return {
@@ -6348,15 +6348,15 @@
                     var I, E = i.xhr();
                     if (E.open(i.type, i.url, i.async, i.username, i.password), i.xhrFields)
                         for (I in i.xhrFields) E[I] = i.xhrFields[I];
                     i.mimeType && E.overrideMimeType && E.overrideMimeType(i.mimeType), !i.crossDomain && !x["X-Requested-With"] && (x["X-Requested-With"] = "XMLHttpRequest");
                     for (I in x) E.setRequestHeader(I, x[I]);
                     d = function($) {
                         return function() {
-                            d && (d = v = E.onload = E.onerror = E.onabort = E.ontimeout = E.onreadystatechange = null, $ === "abort" ? E.abort() : $ === "error" ? typeof E.status != "number" ? A(0, "error") : A(E.status, E.statusText) : A(_o[E.status] || E.status, E.statusText, (E.responseType || "text") !== "text" || typeof E.responseText != "string" ? {
+                            d && (d = v = E.onload = E.onerror = E.onabort = E.ontimeout = E.onreadystatechange = null, $ === "abort" ? E.abort() : $ === "error" ? typeof E.status != "number" ? A(0, "error") : A(E.status, E.statusText) : A(Co[E.status] || E.status, E.statusText, (E.responseType || "text") !== "text" || typeof E.responseText != "string" ? {
                                 binary: E.response
                             } : {
                                 text: E.responseText
                             }, E.getAllResponseHeaders()))
                         }
                     }, E.onload = d(), v = E.onerror = E.ontimeout = d("error"), E.onabort !== void 0 ? E.onabort = v : E.onreadystatechange = function() {
                         E.readyState === 4 && t.setTimeout(function() {
@@ -6403,39 +6403,39 @@
                     },
                     abort: function() {
                         v && v()
                     }
                 }
             }
         });
-        var ga = [],
-            Kn = /(=)\?(?=&|$)|\?\?/;
+        var ya = [],
+            Yn = /(=)\?(?=&|$)|\?\?/;
         u.ajaxSetup({
             jsonp: "callback",
             jsonpCallback: function() {
-                var i = ga.pop() || u.expando + "_" + ua.guid++;
+                var i = ya.pop() || u.expando + "_" + ca.guid++;
                 return this[i] = !0, i
             }
         }), u.ajaxPrefilter("json jsonp", function(i, d, v) {
-            var x, A, I, E = i.jsonp !== !1 && (Kn.test(i.url) ? "url" : typeof i.data == "string" && (i.contentType || "").indexOf("application/x-www-form-urlencoded") === 0 && Kn.test(i.data) && "data");
-            if (E || i.dataTypes[0] === "jsonp") return x = i.jsonpCallback = k(i.jsonpCallback) ? i.jsonpCallback() : i.jsonpCallback, E ? i[E] = i[E].replace(Kn, "$1" + x) : i.jsonp !== !1 && (i.url += (qn.test(i.url) ? "&" : "?") + i.jsonp + "=" + x), i.converters["script json"] = function() {
+            var x, A, I, E = i.jsonp !== !1 && (Yn.test(i.url) ? "url" : typeof i.data == "string" && (i.contentType || "").indexOf("application/x-www-form-urlencoded") === 0 && Yn.test(i.data) && "data");
+            if (E || i.dataTypes[0] === "jsonp") return x = i.jsonpCallback = k(i.jsonpCallback) ? i.jsonpCallback() : i.jsonpCallback, E ? i[E] = i[E].replace(Yn, "$1" + x) : i.jsonp !== !1 && (i.url += (Gn.test(i.url) ? "&" : "?") + i.jsonp + "=" + x), i.converters["script json"] = function() {
                 return I || u.error(x + " was not called"), I[0]
             }, i.dataTypes[0] = "json", A = t[x], t[x] = function() {
                 I = arguments
             }, v.always(function() {
-                A === void 0 ? u(t).removeProp(x) : t[x] = A, i[x] && (i.jsonpCallback = d.jsonpCallback, ga.push(x)), I && k(A) && A(I[0]), I = A = void 0
+                A === void 0 ? u(t).removeProp(x) : t[x] = A, i[x] && (i.jsonpCallback = d.jsonpCallback, ya.push(x)), I && k(A) && A(I[0]), I = A = void 0
             }), "script"
         }), w.createHTMLDocument = function() {
             var i = F.implementation.createHTMLDocument("").body;
             return i.innerHTML = "<form></form><form></form>", i.childNodes.length === 2
         }(), u.parseHTML = function(i, d, v) {
             if (typeof i != "string") return [];
             typeof d == "boolean" && (v = d, d = !1);
             var x, A, I;
-            return d || (w.createHTMLDocument ? (d = F.implementation.createHTMLDocument(""), x = d.createElement("base"), x.href = F.location.href, d.head.appendChild(x)) : d = F), A = at.exec(i), I = !v && [], A ? [d.createElement(A[1])] : (A = $i([i], d, I), I && I.length && u(I).remove(), u.merge([], A.childNodes))
+            return d || (w.createHTMLDocument ? (d = F.implementation.createHTMLDocument(""), x = d.createElement("base"), x.href = F.location.href, d.head.appendChild(x)) : d = F), A = at.exec(i), I = !v && [], A ? [d.createElement(A[1])] : (A = Zi([i], d, I), I && I.length && u(I).remove(), u.merge([], A.childNodes))
         }, u.fn.load = function(i, d, v) {
             var x, A, I, E = this,
                 $ = i.indexOf(" ");
             return $ > -1 && (x = or(i.slice($)), i = i.slice(0, $)), k(d) ? (v = d, d = void 0) : d && typeof d == "object" && (A = "POST"), E.length > 0 && u.ajax({
                 url: i,
                 type: A || "GET",
                 dataType: "html",
@@ -6505,16 +6505,16 @@
                 return Y(this, function(A, I, E) {
                     var $;
                     if (P(A) ? $ = A : A.nodeType === 9 && ($ = A.defaultView), E === void 0) return $ ? $[d] : A[I];
                     $ ? $.scrollTo(v ? $.pageXOffset : E, v ? E : $.pageYOffset) : A[I] = E
                 }, i, x, arguments.length)
             }
         }), u.each(["top", "left"], function(i, d) {
-            u.cssHooks[d] = ta(w.pixelPosition, function(v, x) {
-                if (x) return x = Rr(v, d), jn.test(x) ? u(v).position()[d] + "px" : x
+            u.cssHooks[d] = ea(w.pixelPosition, function(v, x) {
+                if (x) return x = Rr(v, d), Mn.test(x) ? u(v).position()[d] + "px" : x
             })
         }), u.each({
             Height: "height",
             Width: "width"
         }, function(i, d) {
             u.each({
                 padding: "inner" + i,
@@ -6551,64 +6551,64 @@
                 return this.on("mouseenter", i).on("mouseleave", d || i)
             }
         }), u.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "), function(i, d) {
             u.fn[d] = function(v, x) {
                 return arguments.length > 0 ? this.on(d, null, v, x) : this.trigger(d)
             }
         });
-        var Co = /^[\s\uFEFF\xA0]+|([^\s\uFEFF\xA0])[\s\uFEFF\xA0]+$/g;
+        var To = /^[\s\uFEFF\xA0]+|([^\s\uFEFF\xA0])[\s\uFEFF\xA0]+$/g;
         u.proxy = function(i, d) {
             var v, x, A;
             if (typeof d == "string" && (v = i[d], d = i, i = v), !!k(i)) return x = s.call(arguments, 2), A = function() {
                 return i.apply(d || this, x.concat(s.call(arguments)))
             }, A.guid = i.guid = i.guid || u.guid++, A
         }, u.holdReady = function(i) {
             i ? u.readyWait++ : u.ready(!0)
         }, u.isArray = Array.isArray, u.parseJSON = JSON.parse, u.nodeName = q, u.isFunction = k, u.isWindow = P, u.camelCase = gt, u.type = f, u.now = Date.now, u.isNumeric = function(i) {
             var d = u.type(i);
             return (d === "number" || d === "string") && !isNaN(i - parseFloat(i))
         }, u.trim = function(i) {
-            return i == null ? "" : (i + "").replace(Co, "$1")
+            return i == null ? "" : (i + "").replace(To, "$1")
         }, typeof define == "function" && define.amd && define("jquery", [], function() {
             return u
         });
-        var To = t.jQuery,
-            ko = t.$;
+        var ko = t.jQuery,
+            So = t.$;
         return u.noConflict = function(i) {
-            return t.$ === u && (t.$ = ko), i && t.jQuery === u && (t.jQuery = To), u
+            return t.$ === u && (t.$ = So), i && t.jQuery === u && (t.jQuery = ko), u
         }, typeof e > "u" && (t.jQuery = t.$ = u), u
     })
 });
-var Us = ne(ka()),
-    Gl = ne(ie());
-var Dl = ne(ie(), 1);
-var ja = ne(ie(), 1);
-var W = ja.default,
+var qs = ne(Sa()),
+    Xl = ne(ie());
+var Al = ne(ie(), 1);
+var Ma = ne(ie(), 1);
+var W = Ma.default,
     vt = function(t, e) {
         if (vt.factory(t, e)) return vt;
         if (this instanceof vt) return W(t).DataTable(e);
         e = t;
         var r = this,
             n = e === void 0,
             s = this.length;
         return n && (e = {}), this.api = function() {
             return new Wt(this)
         }, this.each(function() {
             var a = {},
-                l = s > 1 ? Oa(a, e, !0) : e,
+                l = s > 1 ? Ra(a, e, !0) : e,
                 c = 0,
                 p, b = this.getAttribute("id"),
                 m = !1,
                 y = vt.defaults,
                 T = W(this);
             if (this.nodeName.toLowerCase() != "table") {
                 Pe(null, 0, "Non-table node initialisation (" + this.nodeName + ")", 2);
                 return
             }
-            W(this).trigger("options.dt", l), Da(y), Ua(y.column), er(y, y, !0), er(y.column, y.column, !0), er(y, W.extend(l, T.data()), !0);
+            W(this).trigger("options.dt", l), Aa(y), qa(y.column), er(y, y, !0), er(y.column, y.column, !0), er(y, W.extend(l, T.data()), !0);
             var w = vt.settings;
             for (c = 0, p = w.length; c < p; c++) {
                 var k = w[c];
                 if (k.nTable == this || k.nTHead && k.nTHead.parentNode == this || k.nTFoot && k.nTFoot.parentNode == this) {
                     var P = l.bRetrieve !== void 0 ? l.bRetrieve : y.bRetrieve,
                         F = l.bDestroy !== void 0 ? l.bDestroy : y.bDestroy;
                     if (n || P) return k.oInstance;
@@ -6630,46 +6630,46 @@
                 sInstance: b,
                 sTableId: b,
                 colgroup: W("<colgroup>").prependTo(this),
                 fastData: function(Z, g, _) {
                     return Ne(h, Z, g, _)
                 }
             });
-            h.nTable = this, h.oInit = l, w.push(h), h.api = new Wt(h), h.oInstance = r.length === 1 ? r : T.dataTable(), Da(l), l.aLengthMenu && !l.iDisplayLength && (l.iDisplayLength = Array.isArray(l.aLengthMenu[0]) ? l.aLengthMenu[0][0] : W.isPlainObject(l.aLengthMenu[0]) ? l.aLengthMenu[0].value : l.aLengthMenu[0]), l = Oa(W.extend(!0, {}, y), l), nr(h.oFeatures, l, ["bPaginate", "bLengthChange", "bFilter", "bSort", "bSortMulti", "bInfo", "bProcessing", "bAutoWidth", "bSortClasses", "bServerSide", "bDeferRender"]), nr(h, l, ["ajax", "fnFormatNumber", "sServerMethod", "aaSorting", "aaSortingFixed", "aLengthMenu", "sPaginationType", "iStateDuration", "bSortCellsTop", "iTabIndex", "sDom", "fnStateLoadCallback", "fnStateSaveCallback", "renderer", "searchDelay", "rowId", "caption", "layout", ["iCookieDuration", "iStateDuration"],
+            h.nTable = this, h.oInit = l, w.push(h), h.api = new Wt(h), h.oInstance = r.length === 1 ? r : T.dataTable(), Aa(l), l.aLengthMenu && !l.iDisplayLength && (l.iDisplayLength = Array.isArray(l.aLengthMenu[0]) ? l.aLengthMenu[0][0] : W.isPlainObject(l.aLengthMenu[0]) ? l.aLengthMenu[0].value : l.aLengthMenu[0]), l = Ra(W.extend(!0, {}, y), l), nr(h.oFeatures, l, ["bPaginate", "bLengthChange", "bFilter", "bSort", "bSortMulti", "bInfo", "bProcessing", "bAutoWidth", "bSortClasses", "bServerSide", "bDeferRender"]), nr(h, l, ["ajax", "fnFormatNumber", "sServerMethod", "aaSorting", "aaSortingFixed", "aLengthMenu", "sPaginationType", "iStateDuration", "bSortCellsTop", "iTabIndex", "sDom", "fnStateLoadCallback", "fnStateSaveCallback", "renderer", "searchDelay", "rowId", "caption", "layout", ["iCookieDuration", "iStateDuration"],
                 ["oSearch", "oPreviousSearch"],
                 ["aoSearchCols", "aoPreSearchCols"],
                 ["iDisplayLength", "_iDisplayLength"]
             ]), nr(h.oScroll, l, [
                 ["sScrollX", "sX"],
                 ["sScrollXInner", "sXInner"],
                 ["sScrollY", "sY"],
                 ["bScrollCollapse", "bCollapse"]
-            ]), nr(h.oLanguage, l, "fnInfoCallback"), Ae(h, "aoDrawCallback", l.fnDrawCallback), Ae(h, "aoStateSaveParams", l.fnStateSaveParams), Ae(h, "aoStateLoadParams", l.fnStateLoadParams), Ae(h, "aoStateLoaded", l.fnStateLoaded), Ae(h, "aoRowCallback", l.fnRowCallback), Ae(h, "aoRowCreatedCallback", l.fnCreatedRow), Ae(h, "aoHeaderCallback", l.fnHeaderCallback), Ae(h, "aoFooterCallback", l.fnFooterCallback), Ae(h, "aoInitComplete", l.fnInitComplete), Ae(h, "aoPreDrawCallback", l.fnPreDrawCallback), h.rowIdFn = Ir(l.rowId), qo(h);
+            ]), nr(h.oLanguage, l, "fnInfoCallback"), Ae(h, "aoDrawCallback", l.fnDrawCallback), Ae(h, "aoStateSaveParams", l.fnStateSaveParams), Ae(h, "aoStateLoadParams", l.fnStateLoadParams), Ae(h, "aoStateLoaded", l.fnStateLoaded), Ae(h, "aoRowCallback", l.fnRowCallback), Ae(h, "aoRowCreatedCallback", l.fnCreatedRow), Ae(h, "aoHeaderCallback", l.fnHeaderCallback), Ae(h, "aoFooterCallback", l.fnFooterCallback), Ae(h, "aoInitComplete", l.fnInitComplete), Ae(h, "aoPreDrawCallback", l.fnPreDrawCallback), h.rowIdFn = Ir(l.rowId), Go(h);
             var o = h.oClasses;
             W.extend(o, vt.ext.classes, l.oClasses), T.addClass(o.table), h.oFeatures.bPaginate || (l.iDisplayStart = 0), h.iInitDisplayStart === void 0 && (h.iInitDisplayStart = l.iDisplayStart, h._iDisplayStart = l.iDisplayStart);
             var f = h.oLanguage;
             W.extend(!0, f, l.oLanguage), f.sUrl ? (W.ajax({
                 dataType: "json",
                 url: f.sUrl,
                 success: function(Z) {
-                    er(y.oLanguage, Z), W.extend(!0, f, Z, h.oInit.oLanguage), Zt(h, null, "i18n", [h], !0), vn(h)
+                    er(y.oLanguage, Z), W.extend(!0, f, Z, h.oInit.oLanguage), Zt(h, null, "i18n", [h], !0), mn(h)
                 },
                 error: function() {
-                    Pe(h, 0, "i18n file loading error", 21), vn(h)
+                    Pe(h, 0, "i18n file loading error", 21), mn(h)
                 }
             }), m = !0) : Zt(h, null, "i18n", [h]);
             var C = [],
                 B = this.getElementsByTagName("thead"),
-                u = Ya(h, B[0]);
+                u = Qa(h, B[0]);
             if (l.aoColumns) C = l.aoColumns;
             else if (u.length)
                 for (c = 0, p = u[0].length; c < p; c++) C.push(null);
-            for (c = 0, p = C.length; c < p; c++) qa(h);
-            $o(h, l.aoColumnDefs, C, u, function(Z, g) {
-                ui(h, Z, g)
+            for (c = 0, p = C.length; c < p; c++) Ga(h);
+            Zo(h, l.aoColumnDefs, C, u, function(Z, g) {
+                ci(h, Z, g)
             });
             var z = T.children("tbody").find("tr").eq(0);
             if (z.length) {
                 var q = function(Z, g) {
                     return Z.getAttribute("data-" + g) !== null ? g : null
                 };
                 W(z[0]).children("th, td").each(function(Z, g) {
@@ -6678,38 +6678,38 @@
                         var S = q(g, "sort") || q(g, "order"),
                             N = q(g, "filter") || q(g, "search");
                         (S !== null || N !== null) && (_.mData = {
                             _: Z + ".display",
                             sort: S !== null ? Z + ".@data-" + S : void 0,
                             type: S !== null ? Z + ".@data-" + S : void 0,
                             filter: N !== null ? Z + ".@data-" + N : void 0
-                        }, _._isArrayHost = !0, ui(h, Z))
+                        }, _._isArrayHost = !0, ci(h, Z))
                     }
                 })
             }
             var et = h.oFeatures,
                 O = function() {
                     if (l.aaSorting === void 0) {
                         var Z = h.aaSorting;
                         for (c = 0, p = Z.length; c < p; c++) Z[c][1] = h.aoColumns[c].asSorting[0]
                     }
-                    fi(h), Ae(h, "aoDrawCallback", function() {
-                        (h.bSorted || Be(h) === "ssp" || et.bDeferRender) && fi(h)
+                    hi(h), Ae(h, "aoDrawCallback", function() {
+                        (h.bSorted || Be(h) === "ssp" || et.bDeferRender) && hi(h)
                     });
                     var g = T.children("caption");
                     h.caption && (g.length === 0 && (g = W("<caption/>").appendTo(T)), g.html(h.caption)), g.length && (g[0]._captionSide = g.css("caption-side"), h.captionNode = g[0]), B.length === 0 && (B = W("<thead/>").appendTo(T)), h.nTHead = B[0], W("tr", B).addClass(o.thead.row);
                     var _ = T.children("tbody");
                     _.length === 0 && (_ = W("<tbody/>").insertAfter(B)), h.nTBody = _[0];
                     var S = T.children("tfoot");
                     if (S.length === 0 && (S = W("<tfoot/>").appendTo(T)), h.nTFoot = S[0], W("tr", S).addClass(o.tfoot.row), l.aaData)
                         for (c = 0; c < l.aaData.length; c++) br(h, l.aaData[c]);
-                    else Be(h) == "dom" && _i(h, W(h.nTBody).children("tr"));
-                    h.aiDisplay = h.aiDisplayMaster.slice(), h.bInitialised = !0, m === !1 && vn(h)
+                    else Be(h) == "dom" && Ci(h, W(h.nTBody).children("tr"));
+                    h.aiDisplay = h.aiDisplayMaster.slice(), h.bInitialised = !0, m === !1 && mn(h)
                 };
-            Ae(h, "aoDrawCallback", In), l.bStateSave ? (et.bStateSave = !0, fl(h, l, O)) : O()
+            Ae(h, "aoDrawCallback", Pn), l.bStateSave ? (et.bStateSave = !0, hl(h, l, O)) : O()
         }), r = null, this
     };
 vt.ext = oe = {
     buttons: {},
     classes: {},
     builder: "-source-",
     errMode: "alert",
@@ -6807,44 +6807,44 @@
     paging: {
         active: "current",
         button: "dt-paging-button",
         container: "dt-paging",
         disabled: "disabled"
     }
 });
-var oe, Wt, It, Qt, ai = {},
-    jo = /[\r\n\u2028]/g,
-    pi = /<([^>]*>)/g,
-    Mo = Math.pow(2, 28),
-    Vo = /^\d{2,4}[./-]\d{1,2}[./-]\d{1,2}([T ]{1}\d{1,2}[:.]\d{2}([.:]\d{2})?)?$/,
-    Ho = new RegExp("(\\" + ["/", ".", "*", "+", "?", "|", "(", ")", "[", "]", "{", "}", "\\", "$", "^", "-"].join("|\\") + ")", "g"),
-    bi = /['\u00A0,$£€¥%\u2009\u202F\u20BD\u20a9\u20BArfkɃΞ]/gi,
-    Ze = function(t) {
+var oe, Wt, It, Qt, si = {},
+    Mo = /[\r\n\u2028]/g,
+    bi = /<([^>]*>)/g,
+    Vo = Math.pow(2, 28),
+    Ho = /^\d{2,4}[./-]\d{1,2}[./-]\d{1,2}([T ]{1}\d{1,2}[:.]\d{2}([.:]\d{2})?)?$/,
+    Wo = new RegExp("(\\" + ["/", ".", "*", "+", "?", "|", "(", ")", "[", "]", "{", "}", "\\", "$", "^", "-"].join("|\\") + ")", "g"),
+    vi = /['\u00A0,$£€¥%\u2009\u202F\u20BD\u20a9\u20BArfkɃΞ]/gi,
+    Ke = function(t) {
         return !t || t === !0 || t === "-"
     },
-    Ma = function(t) {
+    Va = function(t) {
         var e = parseInt(t, 10);
         return !isNaN(e) && isFinite(t) ? e : null
     },
-    Va = function(t, e) {
-        return ai[e] || (ai[e] = new RegExp(ci(e), "g")), typeof t == "string" && e !== "." ? t.replace(/\./g, "").replace(ai[e], ".") : t
+    Ha = function(t, e) {
+        return si[e] || (si[e] = new RegExp(fi(e), "g")), typeof t == "string" && e !== "." ? t.replace(/\./g, "").replace(si[e], ".") : t
     },
-    vi = function(t, e, r) {
+    mi = function(t, e, r) {
         var n = typeof t,
             s = n === "string";
-        return n === "number" || n === "bigint" || Ze(t) ? !0 : (e && s && (t = Va(t, e)), r && s && (t = t.replace(bi, "")), !isNaN(parseFloat(t)) && isFinite(t))
+        return n === "number" || n === "bigint" || Ke(t) ? !0 : (e && s && (t = Ha(t, e)), r && s && (t = t.replace(vi, "")), !isNaN(parseFloat(t)) && isFinite(t))
     },
-    Wo = function(t) {
-        return Ze(t) || typeof t == "string"
+    Uo = function(t) {
+        return Ke(t) || typeof t == "string"
     },
-    Ha = function(t, e, r) {
-        if (Ze(t)) return !0;
+    Wa = function(t, e, r) {
+        if (Ke(t)) return !0;
         if (typeof t == "string" && t.match(/<(input|select)/i)) return null;
-        var n = Wo(t);
-        return n && vi(hr(t), e, r) ? !0 : null
+        var n = Uo(t);
+        return n && mi(hr(t), e, r) ? !0 : null
     },
     xe = function(t, e, r) {
         var n = [],
             s = 0,
             a = t.length;
         if (r !== void 0)
             for (; s < a; s++) t[s] && t[s][e] && n.push(t[s][e][r]);
@@ -6865,71 +6865,71 @@
     cr = function(t, e) {
         var r = [],
             n;
         e === void 0 ? (e = 0, n = t) : (n = e, e = t);
         for (var s = e; s < n; s++) r.push(s);
         return r
     },
-    Wa = function(t) {
+    Ua = function(t) {
         for (var e = [], r = 0, n = t.length; r < n; r++) t[r] && e.push(t[r]);
         return e
     },
     hr = function(t) {
-        if (t.length > Mo) throw new Error("Exceeded max str len");
+        if (t.length > Vo) throw new Error("Exceeded max str len");
         var e;
-        t = t.replace(pi, "");
+        t = t.replace(bi, "");
         do e = t, t = t.replace(/<script/i, ""); while (t !== e);
         return e
     },
     Dr = function(t) {
         return Array.isArray(t) && (t = t.join(",")), typeof t == "string" ? t.replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;").replace(/"/g, "&quot;") : t
     },
-    mn = function(t, e) {
+    gn = function(t, e) {
         if (typeof t != "string") return t;
         var r = t.normalize("NFD");
         return r.length !== t.length ? (e === !0 ? t + " " : "") + r.replace(/[\u0300-\u036f]/g, "") : r
     },
-    Uo = function(t) {
+    qo = function(t) {
         if (t.length < 2) return !0;
         for (var e = t.slice().sort(), r = e[0], n = 1, s = e.length; n < s; n++) {
             if (e[n] === r) return !1;
             r = e[n]
         }
         return !0
     },
     pr = function(t) {
         if (Array.from && Set) return Array.from(new Set(t));
-        if (Uo(t)) return t.slice();
+        if (qo(t)) return t.slice();
         var e = [],
             r, n, s = t.length,
             a, l = 0;
         t: for (n = 0; n < s; n++) {
             for (r = t[n], a = 0; a < l; a++)
                 if (e[a] === r) continue t;
             e.push(r), l++
         }
         return e
     },
-    mi = function(t, e) {
+    gi = function(t, e) {
         if (Array.isArray(e))
-            for (var r = 0; r < e.length; r++) mi(t, e[r]);
+            for (var r = 0; r < e.length; r++) gi(t, e[r]);
         else t.push(e);
         return t
     };
 
 function Ar(t, e) {
     e && e.split(" ").forEach(function(r) {
         r && t.classList.add(r)
     })
 }
 vt.util = {
     diacritics: function(t, e) {
         var r = typeof t;
-        if (r !== "function") return mn(t, e);
-        mn = t
+        if (r !== "function") return gn(t, e);
+        gn = t
     },
     debounce: function(t, e) {
         var r;
         return function() {
             var n = this,
                 s = arguments;
             clearTimeout(r), r = setTimeout(function() {
@@ -6946,25 +6946,25 @@
                 c = arguments;
             n && l < n + r ? (clearTimeout(s), s = setTimeout(function() {
                 n = void 0, t.apply(a, c)
             }, r)) : (n = l, t.apply(a, c))
         }
     },
     escapeRegex: function(t) {
-        return t.replace(Ho, "\\$1")
+        return t.replace(Wo, "\\$1")
     },
     set: function(t) {
         if (W.isPlainObject(t)) return vt.util.set(t._);
         if (t === null) return function() {};
         if (typeof t == "function") return function(r, n, s) {
             t(r, "set", n, s)
         };
         if (typeof t == "string" && (t.indexOf(".") !== -1 || t.indexOf("[") !== -1 || t.indexOf("(") !== -1)) {
             var e = function(r, n, s) {
-                for (var a = Ia(s), l, c = a[a.length - 1], p, b, m, y, T = 0, w = a.length - 1; T < w; T++) {
+                for (var a = Pa(s), l, c = a[a.length - 1], p, b, m, y, T = 0, w = a.length - 1; T < w; T++) {
                     if (a[T] === "__proto__" || a[T] === "constructor") throw new Error("Cannot set prototype values");
                     if (p = a[T].match(Ur), b = a[T].match(kr), p) {
                         if (a[T] = a[T].replace(Ur, ""), r[a[T]] = [], l = a.slice(), l.splice(0, T + 1), y = l.join("."), Array.isArray(n))
                             for (var k = 0, P = n.length; k < P; k++) m = {}, e(m, n[k], y), r[a[T]].push(m);
                         else r[a[T]] = n;
                         return
                     } else b && (a[T] = a[T].replace(kr, ""), r = r[a[T]](n));
@@ -6996,15 +6996,15 @@
             if (typeof t == "function") return function(n, s, a, l) {
                 return t(n, s, a, l)
             };
             if (typeof t == "string" && (t.indexOf(".") !== -1 || t.indexOf("[") !== -1 || t.indexOf("(") !== -1)) {
                 var r = function(n, s, a) {
                     var l, c, p, b;
                     if (a !== "")
-                        for (var m = Ia(a), y = 0, T = m.length; y < T; y++) {
+                        for (var m = Pa(a), y = 0, T = m.length; y < T; y++) {
                             if (l = m[y].match(Ur), c = m[y].match(kr), l) {
                                 if (m[y] = m[y].replace(Ur, ""), m[y] !== "" && (n = n[m[y]]), p = [], m.splice(0, y + 1), b = m.join("."), Array.isArray(n))
                                     for (var w = 0, k = n.length; w < k; w++) p.push(r(n[w], s, b));
                                 var P = l[0].substring(1, l[0].length - 1);
                                 n = P === "" ? p : p.join(P);
                                 break
                             } else if (c) {
@@ -7040,48 +7040,48 @@
             return
         } else if (e === "string" || Array.isArray(t)) return Dr(t);
         return t
     },
     unique: pr
 };
 
-function Cn(t) {
+function Tn(t) {
     var e = "a aa ai ao as b fn i m o s ",
         r, n, s = {};
     W.each(t, function(a) {
-        r = a.match(/^([^A-Z]+?)([A-Z])/), r && e.indexOf(r[1] + " ") !== -1 && (n = a.replace(r[0], r[2].toLowerCase()), s[n] = a, r[1] === "o" && Cn(t[a]))
+        r = a.match(/^([^A-Z]+?)([A-Z])/), r && e.indexOf(r[1] + " ") !== -1 && (n = a.replace(r[0], r[2].toLowerCase()), s[n] = a, r[1] === "o" && Tn(t[a]))
     }), t._hungarianMap = s
 }
 
 function er(t, e, r) {
-    t._hungarianMap || Cn(t);
+    t._hungarianMap || Tn(t);
     var n;
     W.each(e, function(s) {
         n = t._hungarianMap[s], n !== void 0 && (r || e[n] === void 0) && (n.charAt(0) === "o" ? (e[n] || (e[n] = {}), W.extend(!0, e[n], e[s]), er(t[n], e[n], r)) : e[n] = e[s])
     })
 }
 var ye = function(t, e, r) {
     t[e] !== void 0 && (t[r] = t[e])
 };
 
-function Da(t) {
+function Aa(t) {
     ye(t, "ordering", "bSort"), ye(t, "orderMulti", "bSortMulti"), ye(t, "orderClasses", "bSortClasses"), ye(t, "orderCellsTop", "bSortCellsTop"), ye(t, "order", "aaSorting"), ye(t, "orderFixed", "aaSortingFixed"), ye(t, "paging", "bPaginate"), ye(t, "pagingType", "sPaginationType"), ye(t, "pageLength", "iDisplayLength"), ye(t, "searching", "bFilter"), typeof t.sScrollX == "boolean" && (t.sScrollX = t.sScrollX ? "100%" : ""), typeof t.scrollX == "boolean" && (t.scrollX = t.scrollX ? "100%" : "");
     var e = t.aoSearchCols;
     if (e)
         for (var r = 0, n = e.length; r < n; r++) e[r] && er(vt.models.oSearch, e[r]);
     t.serverSide && !t.searchDelay && (t.searchDelay = 400)
 }
 
-function Ua(t) {
+function qa(t) {
     ye(t, "orderable", "bSortable"), ye(t, "orderData", "aDataSort"), ye(t, "orderSequence", "asSorting"), ye(t, "orderDataType", "sortDataType");
     var e = t.aDataSort;
     typeof e == "number" && !Array.isArray(e) && (t.aDataSort = [e])
 }
 
-function qo(t) {
+function Go(t) {
     if (!vt.__browser) {
         var e = {};
         vt.__browser = e;
         var r = W("<div/>").css({
                 position: "fixed",
                 top: 0,
                 left: -1 * window.pageXOffset,
@@ -7101,33 +7101,33 @@
             n = r.children(),
             s = n.children();
         e.barWidth = n[0].offsetWidth - n[0].clientWidth, e.bScrollbarLeft = Math.round(s.offset().left) !== 1, r.remove()
     }
     W.extend(t.oBrowser, vt.__browser), t.oScroll.iBarWidth = vt.__browser.barWidth
 }
 
-function qa(t) {
+function Ga(t) {
     var e = vt.defaults.column,
         r = t.aoColumns.length,
         n = W.extend({}, vt.models.oColumn, e, {
             aDataSort: e.aDataSort ? e.aDataSort : [r],
             mData: e.mData ? e.mData : r,
             idx: r,
             searchFixed: {},
             colEl: W("<col>").attr("data-dt-column", r)
         });
     t.aoColumns.push(n);
     var s = t.aoPreSearchCols;
     s[r] = W.extend({}, vt.models.oSearch, s[r])
 }
 
-function ui(t, e, r) {
+function ci(t, e, r) {
     var n = t.aoColumns[e];
     if (r != null) {
-        Ua(r), er(vt.defaults.column, r, !0), r.mDataProp !== void 0 && !r.mData && (r.mData = r.mDataProp), r.sType && (n._sManualType = r.sType), r.className && !r.sClass && (r.sClass = r.className);
+        qa(r), er(vt.defaults.column, r, !0), r.mDataProp !== void 0 && !r.mData && (r.mData = r.mDataProp), r.sType && (n._sManualType = r.sType), r.className && !r.sClass && (r.sClass = r.className);
         var s = n.sClass;
         W.extend(n, r), nr(n, r, "sWidth", "sWidthOrig"), s !== n.sClass && (n.sClass = s + " " + n.sClass), r.iDataSort !== void 0 && (n.aDataSort = [r.iDataSort]), nr(n, r, "aDataSort")
     }
     var a = n.mData,
         l = Ir(a);
     if (n.mRender && Array.isArray(n.mRender)) {
         var c = n.mRender.slice(),
@@ -7142,104 +7142,104 @@
         var w = l(m, y, void 0, T);
         return n._render && y ? n._render(w, y, m, T) : w
     }, n.fnSetData = function(m, y, T) {
         return fr(a)(m, y, T)
     }, typeof a != "number" && !n._isArrayHost && (t._rowReadObject = !0), t.oFeatures.bSort || (n.bSortable = !1)
 }
 
-function Tn(t) {
-    ol(t), Go(t);
+function kn(t) {
+    ll(t), Xo(t);
     var e = t.oScroll;
-    (e.sY !== "" || e.sX !== "") && ts(t), Zt(t, null, "column-sizing", [t])
+    (e.sY !== "" || e.sX !== "") && es(t), Zt(t, null, "column-sizing", [t])
 }
 
-function Go(t) {
+function Xo(t) {
     for (var e = t.aoColumns, r = 0; r < e.length; r++) {
-        var n = Ga(t, [r], !1, !1);
+        var n = Xa(t, [r], !1, !1);
         e[r].colEl.css("width", n)
     }
 }
 
-function gi(t, e) {
-    var r = yi(t, "bVisible");
+function yi(t, e) {
+    var r = wi(t, "bVisible");
     return typeof r[e] == "number" ? r[e] : null
 }
 
 function $r(t, e) {
-    var r = yi(t, "bVisible"),
+    var r = wi(t, "bVisible"),
         n = r.indexOf(e);
     return n !== -1 ? n : null
 }
 
-function kn(t) {
+function Sn(t) {
     var e = t.aoHeader,
         r = t.aoColumns,
         n = 0;
     if (e.length)
         for (var s = 0, a = e[0].length; s < a; s++) r[s].bVisible && W(e[0][s].cell).css("display") !== "none" && n++;
     return n
 }
 
-function yi(t, e) {
+function wi(t, e) {
     var r = [];
     return t.aoColumns.map(function(n, s) {
         n[e] && r.push(s)
     }), r
 }
 
-function wi(t) {
+function xi(t) {
     var e = t.aoColumns,
         r = t.aoData,
         n = vt.ext.type.detect,
         s, a, l, c, p, b, m, y, T;
     for (s = 0, a = e.length; s < a; s++) {
         if (m = e[s], T = [], !m.sType && m._sManualType) m.sType = m._sManualType;
         else if (!m.sType) {
             for (l = 0, c = n.length; l < c; l++) {
-                for (p = 0, b = r.length; p < b && !(r[p] && (T[p] === void 0 && (T[p] = Ne(t, p, s, "type")), y = n[l](T[p], t), !y && l !== n.length - 2 || y === "html" && !Ze(T[p]))); p++);
+                for (p = 0, b = r.length; p < b && !(r[p] && (T[p] === void 0 && (T[p] = Ne(t, p, s, "type")), y = n[l](T[p], t), !y && l !== n.length - 2 || y === "html" && !Ke(T[p]))); p++);
                 if (y) {
                     m.sType = y;
                     break
                 }
             }
             m.sType || (m.sType = "string")
         }
         var w = oe.type.className[m.sType];
-        w && (Aa(t.aoHeader, s, w), Aa(t.aoFooter, s, w));
+        w && (Ia(t.aoHeader, s, w), Ia(t.aoFooter, s, w));
         var k = oe.type.render[m.sType];
-        k && !m._render && (m._render = vt.util.get(k), Xo(t, s))
+        k && !m._render && (m._render = vt.util.get(k), $o(t, s))
     }
 }
 
-function Xo(t, e) {
+function $o(t, e) {
     for (var r = t.aoData, n = 0; n < r.length; n++)
         if (r[n].nTr) {
             var s = Ne(t, n, e, "display");
-            r[n].displayData[e] = s, gn(r[n].anCells[e], s)
+            r[n].displayData[e] = s, yn(r[n].anCells[e], s)
         }
 }
 
-function Aa(t, e, r) {
+function Ia(t, e, r) {
     t.forEach(function(n) {
         n[e] && n[e].unique && Ar(n[e].cell, r)
     })
 }
 
-function $o(t, e, r, n, s) {
+function Zo(t, e, r, n, s) {
     var a, l, c, p, b, m, y, T = t.aoColumns;
     if (r)
         for (a = 0, l = r.length; a < l; a++) r[a] && r[a].name && (T[a].sName = r[a].name);
     if (e)
         for (a = e.length - 1; a >= 0; a--) {
             y = e[a];
             var w = y.target !== void 0 ? y.target : y.targets !== void 0 ? y.targets : y.aTargets;
             for (Array.isArray(w) || (w = [w]), c = 0, p = w.length; c < p; c++) {
                 var k = w[c];
                 if (typeof k == "number" && k >= 0) {
-                    for (; T.length <= k;) qa(t);
+                    for (; T.length <= k;) Ga(t);
                     s(k, y)
                 } else if (typeof k == "number" && k < 0) s(T.length + k, y);
                 else if (typeof k == "string")
                     for (b = 0, m = T.length; b < m; b++) k === "_all" ? s(b, y) : k.indexOf(":name") !== -1 ? T[b].sName === k.replace(":name", "") && s(b, y) : n.forEach(function(P) {
                         if (P[b]) {
                             var F = W(P[b].cell);
                             k.match(/^[a-z][\w-]*$/i) && (k = "." + k), F.is(k) && s(b, y)
@@ -7247,16 +7247,16 @@
                     })
             }
         }
     if (r)
         for (a = 0, l = r.length; a < l; a++) s(a, r[a])
 }
 
-function Ga(t, e, r, n) {
-    Array.isArray(e) || (e = xi(e));
+function Xa(t, e, r, n) {
+    Array.isArray(e) || (e = _i(e));
     for (var s = 0, a, l = t.aoColumns, c = 0, p = e.length; c < p; c++) {
         var b = l[e[c]],
             m = r ? b.sWidthOrig : b.sWidth;
         if (!(!n && b.bVisible === !1)) {
             if (m == null) return null;
             if (typeof m == "number") a = "px", s += m;
             else {
@@ -7264,15 +7264,15 @@
                 y && (s += y[1] * 1, a = y.length === 3 ? y[2] : "px")
             }
         }
     }
     return s + a
 }
 
-function xi(t) {
+function _i(t) {
     var e = W(t).closest("[data-dt-column]").attr("data-dt-column");
     return e ? e.split(",").map(function(r) {
         return r * 1
     }) : []
 }
 
 function br(t, e, r, n) {
@@ -7281,21 +7281,21 @@
             src: r ? "dom" : "data",
             idx: s
         });
     a._aData = e, t.aoData.push(a);
     for (var l = t.aoColumns, c = 0, p = l.length; c < p; c++) l[c].sType = null;
     t.aiDisplayMaster.push(s);
     var b = t.rowIdFn(e);
-    return b !== void 0 && (t.aIds[b] = a), (r || !t.oFeatures.bDeferRender) && $a(t, s, r, n), s
+    return b !== void 0 && (t.aIds[b] = a), (r || !t.oFeatures.bDeferRender) && Za(t, s, r, n), s
 }
 
-function _i(t, e) {
+function Ci(t, e) {
     var r;
     return e instanceof W || (e = W(e)), e.map(function(n, s) {
-        return r = Xa(t, s), br(t, r.data, s, r.cells)
+        return r = $a(t, s), br(t, r.data, s, r.cells)
     })
 }
 
 function Ne(t, e, r, n) {
     n === "search" ? n = "filter" : n === "order" && (n = "sort");
     var s = t.aoData[e];
     if (s) {
@@ -7316,68 +7316,68 @@
             var m = vt.ext.type.search;
             m[l.sType] && (b = m[l.sType](b))
         }
         return b
     }
 }
 
-function Zo(t, e, r, n) {
+function Ko(t, e, r, n) {
     var s = t.aoColumns[r],
         a = t.aoData[e]._aData;
     s.fnSetData(a, n, {
         settings: t,
         row: e,
         col: r
     })
 }
 
-function gn(t, e) {
+function yn(t, e) {
     e && typeof e == "object" && e.nodeName ? W(t).empty().append(e) : t.innerHTML = e
 }
 var Ur = /\[.*?\]$/,
     kr = /\(\)$/;
 
-function Ia(t) {
+function Pa(t) {
     var e = t.match(/(\\.|[^.])+/g) || [""];
     return e.map(function(r) {
         return r.replace(/\\\./g, ".")
     })
 }
 var Ir = vt.util.get,
     fr = vt.util.set;
 
-function Pa(t) {
+function Fa(t) {
     return xe(t.aoData, "_aData")
 }
 
-function Ci(t) {
+function Ti(t) {
     t.aoData.length = 0, t.aiDisplayMaster.length = 0, t.aiDisplay.length = 0, t.aIds = {}
 }
 
-function Sn(t, e, r, n) {
+function Dn(t, e, r, n) {
     var s = t.aoData[e],
         a, l;
-    if (s._aSortData = null, s._aFilterData = null, s.displayData = null, r === "dom" || (!r || r === "auto") && s.src === "dom") s._aData = Xa(t, s, n, n === void 0 ? void 0 : s._aData).data;
+    if (s._aSortData = null, s._aFilterData = null, s.displayData = null, r === "dom" || (!r || r === "auto") && s.src === "dom") s._aData = $a(t, s, n, n === void 0 ? void 0 : s._aData).data;
     else {
         var c = s.anCells,
-            p = Ti(t, e);
+            p = ki(t, e);
         if (c)
-            if (n !== void 0) gn(c[n], p[n]);
+            if (n !== void 0) yn(c[n], p[n]);
             else
-                for (a = 0, l = c.length; a < l; a++) gn(c[a], p[a])
+                for (a = 0, l = c.length; a < l; a++) yn(c[a], p[a])
     }
     var b = t.aoColumns;
     if (n !== void 0) b[n].sType = null, b[n].maxLenString = null;
     else {
         for (a = 0, l = b.length; a < l; a++) b[a].sType = null, b[a].maxLenString = null;
-        Za(t, s)
+        Ka(t, s)
     }
 }
 
-function Xa(t, e, r, n) {
+function $a(t, e, r, n) {
     var s = [],
         a = e.firstChild,
         l, c, p = 0,
         b, m = t.aoColumns,
         y = t._rowReadObject;
     n = n !== void 0 ? n : y ? {} : [];
     var T = function(o, f) {
@@ -7411,73 +7411,73 @@
     }
     return {
         data: n,
         cells: s
     }
 }
 
-function Ti(t, e) {
+function ki(t, e) {
     let r = t.aoData[e],
         n = t.aoColumns;
     if (!r.displayData) {
         r.displayData = [];
         for (var s = 0, a = n.length; s < a; s++) r.displayData.push(Ne(t, e, s, "display"))
     }
     return r.displayData
 }
 
-function $a(t, e, r, n) {
+function Za(t, e, r, n) {
     var s = t.aoData[e],
         a = s._aData,
         l = [],
         c, p, b, m, y, T, w = t.oClasses.tbody.row;
     if (s.nTr === null) {
-        for (c = r || document.createElement("tr"), s.nTr = c, s.anCells = l, Ar(c, w), c._DT_RowIndex = e, Za(t, s), m = 0, y = t.aoColumns.length; m < y; m++) {
+        for (c = r || document.createElement("tr"), s.nTr = c, s.anCells = l, Ar(c, w), c._DT_RowIndex = e, Ka(t, s), m = 0, y = t.aoColumns.length; m < y; m++) {
             b = t.aoColumns[m], T = !(r && n[m]), p = T ? document.createElement(b.sCellType) : n[m], p || Pe(t, 0, "Incorrect column count", 18), p._DT_CellIndex = {
                 row: e,
                 column: m
             }, l.push(p);
-            var k = Ti(t, e);
-            (T || (b.mRender || b.mData !== m) && (!W.isPlainObject(b.mData) || b.mData._ !== m + ".display")) && gn(p, k[m]), b.bVisible && T ? c.appendChild(p) : !b.bVisible && !T && p.parentNode.removeChild(p), b.fnCreatedCell && b.fnCreatedCell.call(t.oInstance, p, Ne(t, e, m), a, e, m)
+            var k = ki(t, e);
+            (T || (b.mRender || b.mData !== m) && (!W.isPlainObject(b.mData) || b.mData._ !== m + ".display")) && yn(p, k[m]), b.bVisible && T ? c.appendChild(p) : !b.bVisible && !T && p.parentNode.removeChild(p), b.fnCreatedCell && b.fnCreatedCell.call(t.oInstance, p, Ne(t, e, m), a, e, m)
         }
         Zt(t, "aoRowCreatedCallback", "row-created", [c, a, e, l])
     } else Ar(s.nTr, w)
 }
 
-function Za(t, e) {
+function Ka(t, e) {
     var r = e.nTr,
         n = e._aData;
     if (r) {
         var s = t.rowIdFn(n);
         if (s && (r.id = s), n.DT_RowClass) {
             var a = n.DT_RowClass.split(" ");
             e.__rowc = e.__rowc ? pr(e.__rowc.concat(a)) : a, W(r).removeClass(e.__rowc.join(" ")).addClass(n.DT_RowClass)
         }
         n.DT_RowAttr && W(r).attr(n.DT_RowAttr), n.DT_RowData && W(r).data(n.DT_RowData)
     }
 }
 
-function Fa(t, e) {
+function Ba(t, e) {
     var r = t.oClasses,
         n = t.aoColumns,
         s, a, l, c = e === "header" ? t.nTHead : t.nTFoot,
         p = e === "header" ? "sTitle" : e;
     if (c) {
         if ((e === "header" || xe(t.aoColumns, p).join("")) && (l = W("tr", c), l.length || (l = W("<tr/>").appendTo(c)), l.length === 1)) {
             var b = W("td, th", l);
             for (s = b.length, a = n.length; s < a; s++) W("<th/>").html(n[s][p] || "").appendTo(l)
         }
-        var m = Ya(t, c, !0);
+        var m = Qa(t, c, !0);
         e === "header" ? t.aoHeader = m : t.aoFooter = m, W(c).children("tr").attr("role", "row"), W(c).children("tr").children("th, td").each(function() {
-            xn(t, e)(t, W(this), r)
+            _n(t, e)(t, W(this), r)
         })
     }
 }
 
-function Ka(t, e, r) {
+function Ya(t, e, r) {
     var n, s, a, l = [],
         c = [],
         p = t.aoColumns,
         b = p.length,
         m, y;
     if (e) {
         for (r || (r = cr(b).filter(function(k) {
@@ -7500,27 +7500,27 @@
                         rowspan: m,
                         title: w.length ? w.html() : W(a).html()
                     }
                 } return c
     }
 }
 
-function yn(t, e) {
-    for (var r = Ka(t, e), n, s, a = 0; a < e.length; a++) {
+function wn(t, e) {
+    for (var r = Ya(t, e), n, s, a = 0; a < e.length; a++) {
         if (n = e[a].row, n)
             for (; s = n.firstChild;) n.removeChild(s);
         for (var l = 0; l < r[a].length; l++) {
             var c = r[a][l];
             c && W(c.cell).appendTo(n).attr("rowspan", c.rowspan).attr("colspan", c.colspan)
         }
     }
 }
 
 function Fr(t, e) {
-    Qo(t);
+    Jo(t);
     var r = Zt(t, "aoPreDrawCallback", "preDraw", [t]);
     if (r.indexOf(!1) !== -1) {
         Fe(t, !1);
         return
     }
     var n = [],
         s = 0,
@@ -7528,50 +7528,50 @@
         l = t.aiDisplay,
         c = t._iDisplayStart,
         p = t.fnDisplayEnd(),
         b = t.aoColumns,
         m = W(t.nTBody);
     if (t.bDrawing = !0, !a) t.iDraw++;
     else if (!t.bDestroying && !e) {
-        t.iDraw === 0 && m.empty().append(Ba(t)), Jo(t);
+        t.iDraw === 0 && m.empty().append(Na(t)), tl(t);
         return
     }
     if (l.length !== 0)
         for (var y = a ? 0 : c, T = a ? t.aoData.length : p, w = y; w < T; w++) {
             var k = l[w],
                 P = t.aoData[k];
-            P.nTr === null && $a(t, k);
+            P.nTr === null && Za(t, k);
             for (var F = P.nTr, h = 0; h < b.length; h++) {
                 var o = b[h],
                     f = P.anCells[h];
                 Ar(f, oe.type.className[o.sType]), Ar(f, o.sClass), Ar(f, t.oClasses.tbody.cell)
             }
             Zt(t, "aoRowCallback", null, [F, P._aData, s, w, k]), n.push(F), s++
-        } else n[0] = Ba(t);
-    Zt(t, "aoHeaderCallback", "header", [W(t.nTHead).children("tr")[0], Pa(t), c, p, l]), Zt(t, "aoFooterCallback", "footer", [W(t.nTFoot).children("tr")[0], Pa(t), c, p, l]), m[0].replaceChildren ? m[0].replaceChildren.apply(m[0], n) : (m.children().detach(), m.append(W(n))), W(t.nTableWrapper).toggleClass("dt-empty-footer", W("tr", t.nTFoot).length === 0), Zt(t, "aoDrawCallback", "draw", [t], !0), t.bSorted = !1, t.bFiltered = !1, t.bDrawing = !1
+        } else n[0] = Na(t);
+    Zt(t, "aoHeaderCallback", "header", [W(t.nTHead).children("tr")[0], Fa(t), c, p, l]), Zt(t, "aoFooterCallback", "footer", [W(t.nTFoot).children("tr")[0], Fa(t), c, p, l]), m[0].replaceChildren ? m[0].replaceChildren.apply(m[0], n) : (m.children().detach(), m.append(W(n))), W(t.nTableWrapper).toggleClass("dt-empty-footer", W("tr", t.nTFoot).length === 0), Zt(t, "aoDrawCallback", "draw", [t], !0), t.bSorted = !1, t.bFiltered = !1, t.bDrawing = !1
 }
 
 function Pr(t, e, r) {
     var n = t.oFeatures,
         s = n.bSort,
         a = n.bFilter;
-    (r === void 0 || r === !0) && (s && Di(t), a ? Gr(t, t.oPreviousSearch) : t.aiDisplay = t.aiDisplayMaster.slice()), e !== !0 && (t._iDisplayStart = 0), t._drawHold = e, Fr(t), t._drawHold = !1
+    (r === void 0 || r === !0) && (s && Ai(t), a ? Gr(t, t.oPreviousSearch) : t.aiDisplay = t.aiDisplayMaster.slice()), e !== !0 && (t._iDisplayStart = 0), t._drawHold = e, Fr(t), t._drawHold = !1
 }
 
-function Ba(t) {
+function Na(t) {
     var e = t.oLanguage,
         r = e.sZeroRecords,
         n = Be(t);
     return t.iDraw < 1 && n === "ssp" || t.iDraw <= 1 && n === "ajax" ? r = e.sLoadingRecords : e.sEmptyTable && t.fnRecordsTotal() === 0 && (r = e.sEmptyTable), W("<tr/>").append(W("<td />", {
-        colSpan: kn(t),
+        colSpan: Sn(t),
         class: t.oClasses.empty.row
     }).html(r))[0]
 }
 
-function Na(t, e, r) {
+function Ea(t, e, r) {
     var n = {};
     W.each(e, function(p, b) {
         if (b !== null) {
             var m = p.replace(/([A-Z])/g, " $1").split(" ");
             n[m[0]] || (n[m[0]] = {});
             var y = m.length === 1 ? "full" : m[1].toLowerCase(),
                 T = n[m[0]],
@@ -7602,19 +7602,19 @@
     s.sort(function(p, b) {
         var m = p.name.replace(/[^0-9]/g, "") * 1,
             y = b.name.replace(/[^0-9]/g, "") * 1;
         return y - m
     }), r === "bottom" && s.reverse();
     for (var a = [], l = 0, c = s.length; l < c; l++) s[l].val.full && (a.push({
         full: s[l].val.full
-    }), Ea(t, a[a.length - 1]), delete s[l].val.full), Object.keys(s[l].val).length && (a.push(s[l].val), Ea(t, a[a.length - 1]));
+    }), Oa(t, a[a.length - 1]), delete s[l].val.full), Object.keys(s[l].val).length && (a.push(s[l].val), Oa(t, a[a.length - 1]));
     return a
 }
 
-function Ea(t, e) {
+function Oa(t, e) {
     var r = function(s, a) {
             return oe.features[s] || Pe(t, 0, "Unknown feature: " + s), oe.features[s].apply(this, [t, a])
         },
         n = function(s) {
             for (var a = e[s].contents, l = 0, c = a.length; l < c; l++)
                 if (a[l]) {
                     if (typeof a[l] == "string") a[l] = r(a[l], null);
@@ -7627,62 +7627,62 @@
                 } else continue
         };
     W.each(e, function(s) {
         n(s)
     })
 }
 
-function Ko(t) {
+function Yo(t) {
     var e = t.oClasses,
         r = W(t.nTable),
         n = W("<div/>").attr({
             id: t.sTableId + "_wrapper",
             class: e.container
         }).insertBefore(r);
-    if (t.nTableWrapper = n[0], t.sDom) Yo(t, t.sDom, n);
+    if (t.nTableWrapper = n[0], t.sDom) Qo(t, t.sDom, n);
     else {
-        var s = Na(t, t.layout, "top"),
-            a = Na(t, t.layout, "bottom"),
-            l = xn(t, "layout");
+        var s = Ea(t, t.layout, "top"),
+            a = Ea(t, t.layout, "bottom"),
+            l = _n(t, "layout");
         s.forEach(function(c) {
             l(t, n, c)
         }), l(t, n, {
             full: {
                 table: !0,
-                contents: [Ja(t)]
+                contents: [ts(t)]
             }
         }), a.forEach(function(c) {
             l(t, n, c)
         })
     }
-    sl(t)
+    ol(t)
 }
 
-function Yo(t, e, r) {
+function Qo(t, e, r) {
     for (var n = e.match(/(".*?")|('.*?')|./g), s, a, l, c, p, b = 0; b < n.length; b++) {
         if (s = null, a = n[b], a == "<") {
             if (l = W("<div/>"), c = n[b + 1], c[0] == "'" || c[0] == '"') {
                 p = c.replace(/['"]/g, "");
                 var m = "",
                     y;
                 if (p.indexOf(".") != -1) {
                     var T = p.split(".");
                     m = T[0], y = T[1]
                 } else p[0] == "#" ? m = p : y = p;
                 l.attr("id", m.substring(1)).addClass(y), b++
             }
             r.append(l), r = l
-        } else a == ">" ? r = r.parent() : a == "t" ? s = Ja(t) : vt.ext.feature.forEach(function(w) {
+        } else a == ">" ? r = r.parent() : a == "t" ? s = ts(t) : vt.ext.feature.forEach(function(w) {
             a == w.cFeature && (s = w.fnInit(t))
         });
         s && r.append(s)
     }
 }
 
-function Ya(t, e, r) {
+function Qa(t, e, r) {
     var n = t.aoColumns,
         s = W(e).children("tr"),
         a, l, c, p, b, m, y, T, w, k, P = e && e.nodeName.toLowerCase() === "thead",
         F = [],
         h, o = function(z, q, et) {
             for (var O = z[q]; O[et];) et++;
             return et
@@ -7690,15 +7690,15 @@
     for (c = 0, m = s.length; c < m; c++) F.push([]);
     for (c = 0, m = s.length; c < m; c++)
         for (a = s[c], T = 0, l = a.firstChild; l;) {
             if (l.nodeName.toUpperCase() == "TD" || l.nodeName.toUpperCase() == "TH") {
                 var f = [];
                 if (w = l.getAttribute("colspan") * 1, k = l.getAttribute("rowspan") * 1, w = !w || w === 0 || w === 1 ? 1 : w, k = !k || k === 0 || k === 1 ? 1 : k, y = o(F, c, T), h = w === 1, r) {
                     if (h) {
-                        ui(t, y, W(l).data());
+                        ci(t, y, W(l).data());
                         var C = n[y],
                             B = l.getAttribute("width") || null,
                             u = l.style.width.match(/width:\s*(\d+[pxem%]+)/);
                         u && (B = u[1]), C.sWidthOrig = C.sWidth || B, P ? (C.sTitle !== null && !C.autoTitle && (l.innerHTML = C.sTitle), !C.sTitle && h && (C.sTitle = hr(l.innerHTML), C.autoTitle = !0)) : C.footer && (l.innerHTML = C.footer), C.ariaTitle || (C.ariaTitle = W(l).attr("aria-label") || C.sTitle), C.className && W(l).addClass(C.className)
                     }
                     W("span.dt-column-title", l).length === 0 && W("<span>").addClass("dt-column-title").append(l.childNodes).appendTo(l), P && W("span.dt-column-order", l).length === 0 && W("<span>").addClass("dt-column-order").appendTo(l)
                 }
@@ -7712,26 +7712,26 @@
                 l.setAttribute("data-dt-column", pr(f).join(","))
             }
             l = l.nextSibling
         }
     return F
 }
 
-function Qo(t) {
+function Jo(t) {
     var e = Be(t) == "ssp",
         r = t.iInitDisplayStart;
     r !== void 0 && r !== -1 && (t._iDisplayStart = e ? r : r >= t.fnRecordsDisplay() ? 0 : r, t.iInitDisplayStart = -1)
 }
 
-function ki(t, e, r) {
+function Si(t, e, r) {
     var n, s = t.ajax,
         a = t.oInstance,
         l = function(m) {
             var y = t.jqXHR ? t.jqXHR.status : null;
-            (m === null || typeof y == "number" && y == 204) && (m = {}, Dn(t, m, []));
+            (m === null || typeof y == "number" && y == 204) && (m = {}, An(t, m, []));
             var T = m.error || m.sError;
             T && Pe(t, 0, T), t.json = m, Zt(t, null, "xhr", [t, m, t.jqXHR], !0), r(m)
         };
     if (W.isPlainObject(s) && s.data) {
         n = s.data;
         var c = typeof n == "function" ? n(e, t) : n;
         e = typeof n == "function" && c ? c : W.extend(!0, e, c), delete s.data
@@ -7751,21 +7751,21 @@
     if (W.isPlainObject(s) && W.extend(p, s), t.oAjaxData = e, Zt(t, null, "preXhr", [t, e, p], !0), typeof s == "function") t.jqXHR = s.call(a, e, l, t);
     else if (s.url === "") {
         var b = {};
         vt.util.set(s.dataSrc)(b, []), l(b)
     } else t.jqXHR = W.ajax(p), n && (s.data = n)
 }
 
-function Jo(t) {
-    t.iDraw++, Fe(t, !0), ki(t, tl(t), function(e) {
-        el(t, e)
+function tl(t) {
+    t.iDraw++, Fe(t, !0), Si(t, el(t), function(e) {
+        rl(t, e)
     })
 }
 
-function tl(t) {
+function el(t) {
     var e = t.aoColumns,
         r = t.oFeatures,
         n = t.oPreviousSearch,
         s = t.aoPreSearchCols,
         a = function(l, c) {
             return typeof e[l][c] == "function" ? "function" : e[l][c]
         };
@@ -7785,15 +7785,15 @@
                             name: p,
                             term: l.searchFixed[p].toString()
                         }
                     })
                 }
             }
         }),
-        order: An(t).map(function(l) {
+        order: In(t).map(function(l) {
             return {
                 column: l.col,
                 dir: l.dir,
                 name: a(l.col, "sName")
             }
         }),
         start: t._iDisplayStart,
@@ -7807,143 +7807,149 @@
                     term: t.searchFixed[l].toString()
                 }
             })
         }
     }
 }
 
-function el(t, e) {
-    var r = Dn(t, e),
-        n = si(t, "draw", e),
-        s = si(t, "recordsTotal", e),
-        a = si(t, "recordsFiltered", e);
+function rl(t, e) {
+    var r = An(t, e),
+        n = oi(t, "draw", e),
+        s = oi(t, "recordsTotal", e),
+        a = oi(t, "recordsFiltered", e);
     if (n !== void 0) {
         if (n * 1 < t.iDraw) return;
         t.iDraw = n * 1
     }
-    r || (r = []), Ci(t), t._iRecordsTotal = parseInt(s, 10), t._iRecordsDisplay = parseInt(a, 10);
+    r || (r = []), Ti(t), t._iRecordsTotal = parseInt(s, 10), t._iRecordsDisplay = parseInt(a, 10);
     for (var l = 0, c = r.length; l < c; l++) br(t, r[l]);
-    t.aiDisplay = t.aiDisplayMaster.slice(), Fr(t, !0), wn(t), Fe(t, !1)
+    t.aiDisplay = t.aiDisplayMaster.slice(), Fr(t, !0), xn(t), Fe(t, !1)
 }
 
-function Dn(t, e, r) {
+function An(t, e, r) {
     var n = "data";
     if (W.isPlainObject(t.ajax) && t.ajax.dataSrc !== void 0) {
         var s = t.ajax.dataSrc;
         typeof s == "string" || typeof s == "function" ? n = s : s.data !== void 0 && (n = s.data)
     }
     if (!r) return n === "data" ? e.aaData || e[n] : n !== "" ? Ir(n)(e) : e;
     fr(n)(e, r)
 }
 
-function si(t, e, r) {
+function oi(t, e, r) {
     var n = W.isPlainObject(t.ajax) ? t.ajax.dataSrc : null;
     if (n && n[e]) return Ir(n[e])(r);
     var s = "";
     return e === "draw" ? s = "sEcho" : e === "recordsTotal" ? s = "iTotalRecords" : e === "recordsFiltered" && (s = "iTotalDisplayRecords"), r[s] !== void 0 ? r[s] : r[e]
 }
 
 function Gr(t, e) {
     var r = t.aoPreSearchCols;
-    if (wi(t), Be(t) != "ssp") {
-        al(t), t.aiDisplay = t.aiDisplayMaster.slice(), pn(t.aiDisplay, t, e.search, e), W.each(t.searchFixed, function(a, l) {
-            pn(t.aiDisplay, t, l, {})
+    if (xi(t), Be(t) != "ssp") {
+        sl(t), t.aiDisplay = t.aiDisplayMaster.slice(), bn(t.aiDisplay, t, e.search, e), W.each(t.searchFixed, function(a, l) {
+            bn(t.aiDisplay, t, l, {})
         });
         for (var n = 0; n < r.length; n++) {
             var s = r[n];
-            pn(t.aiDisplay, t, s.search, s, n), W.each(t.aoColumns[n].searchFixed, function(a, l) {
-                pn(t.aiDisplay, t, l, {}, n)
+            bn(t.aiDisplay, t, s.search, s, n), W.each(t.aoColumns[n].searchFixed, function(a, l) {
+                bn(t.aiDisplay, t, l, {}, n)
             })
         }
-        rl(t)
+        nl(t)
     }
     t.bFiltered = !0, Zt(t, null, "search", [t])
 }
 
-function rl(t) {
+function nl(t) {
     for (var e = vt.ext.search, r = t.aiDisplay, n, s, a = 0, l = e.length; a < l; a++) {
         for (var c = [], p = 0, b = r.length; p < b; p++) s = r[p], n = t.aoData[s], e[a](t, n._aFilterData, s, n._aData, p) && c.push(s);
         r.length = 0, r.push.apply(r, c)
     }
 }
 
-function pn(t, e, r, n, s) {
-    if (r !== "")
-        for (var a = 0, l = typeof r == "function" ? r : null, c = r instanceof RegExp ? r : l ? null : nl(r, n); a < t.length;) {
-            var p = e.aoData[t[a]],
-                b = s === void 0 ? p._sFilterRow : p._aFilterData[s];
-            (l && !l(b, p._aData, t[a], s) || c && !c.test(b)) && (t.splice(a, 1), a--), a++
+function bn(t, e, r, n, s) {
+    if (r !== "") {
+        var a = 0,
+            l = [],
+            c = typeof r == "function" ? r : null,
+            p = r instanceof RegExp ? r : c ? null : il(r, n);
+        for (a = 0; a < t.length; a++) {
+            var b = e.aoData[t[a]],
+                m = s === void 0 ? b._sFilterRow : b._aFilterData[s];
+            (c && c(m, b._aData, t[a], s) || p && p.test(m)) && l.push(t[a])
         }
+        for (t.length = l.length, a = 0; a < l.length; a++) t[a] = l[a]
+    }
 }
 
-function nl(t, e) {
+function il(t, e) {
     var r = [],
         n = W.extend({}, {
             boundary: !1,
             caseInsensitive: !0,
             exact: !1,
             regex: !1,
             smart: !0
         }, e);
-    if (typeof t != "string" && (t = t.toString()), t = mn(t), n.exact) return new RegExp("^" + ci(t) + "$", n.caseInsensitive ? "i" : "");
-    if (t = n.regex ? t : ci(t), n.smart) {
+    if (typeof t != "string" && (t = t.toString()), t = gn(t), n.exact) return new RegExp("^" + fi(t) + "$", n.caseInsensitive ? "i" : "");
+    if (t = n.regex ? t : fi(t), n.smart) {
         var s = t.match(/!?["\u201C][^"\u201D]+["\u201D]|[^ ]+/g) || [""],
             a = s.map(function(p) {
                 var b = !1,
                     m;
                 return p.charAt(0) === "!" && (b = !0, p = p.substring(1)), p.charAt(0) === '"' ? (m = p.match(/^"(.*)"$/), p = m ? m[1] : p) : p.charAt(0) === "\u201C" && (m = p.match(/^\u201C(.*)\u201D$/), p = m ? m[1] : p), b && (p.length > 1 && r.push("(?!" + p + ")"), p = ""), p.replace(/"/g, "")
             }),
             l = r.length ? r.join("") : "",
             c = n.boundary ? "\\b" : "";
         t = "^(?=.*?" + c + a.join(")(?=.*?" + c) + ")(" + l + ".)*$"
     }
     return new RegExp(t, n.caseInsensitive ? "i" : "")
 }
-var ci = vt.util.escapeRegex,
-    bn = W("<div>")[0],
-    il = bn.textContent !== void 0;
+var fi = vt.util.escapeRegex,
+    vn = W("<div>")[0],
+    al = vn.textContent !== void 0;
 
-function al(t) {
+function sl(t) {
     for (var e = t.aoColumns, r = t.aoData, n, s, a, l, c, p, b = !1, m = 0; m < r.length; m++)
         if (r[m] && (p = r[m], !p._aFilterData)) {
-            for (l = [], s = 0, a = e.length; s < a; s++) n = e[s], n.bSearchable ? (c = Ne(t, m, s, "filter"), c === null && (c = ""), typeof c != "string" && c.toString && (c = c.toString())) : c = "", c.indexOf && c.indexOf("&") !== -1 && (bn.innerHTML = c, c = il ? bn.textContent : bn.innerText), c.replace && (c = c.replace(/[\r\n\u2028]/g, "")), l.push(c);
+            for (l = [], s = 0, a = e.length; s < a; s++) n = e[s], n.bSearchable ? (c = Ne(t, m, s, "filter"), c === null && (c = ""), typeof c != "string" && c.toString && (c = c.toString())) : c = "", c.indexOf && c.indexOf("&") !== -1 && (vn.innerHTML = c, c = al ? vn.textContent : vn.innerText), c.replace && (c = c.replace(/[\r\n\u2028]/g, "")), l.push(c);
             p._aFilterData = l, p._sFilterRow = l.join("  "), b = !0
         } return b
 }
 
-function vn(t) {
+function mn(t) {
     var e, r = t.iInitDisplayStart;
     if (!t.bInitialised) {
         setTimeout(function() {
-            vn(t)
+            mn(t)
         }, 200);
         return
     }
-    Fa(t, "header"), Fa(t, "footer"), yn(t, t.aoHeader), yn(t, t.aoFooter), Ko(t), dl(t), es(t), Fe(t, !0), Zt(t, null, "preInit", [t], !0), Pr(t);
+    Ba(t, "header"), Ba(t, "footer"), wn(t, t.aoHeader), wn(t, t.aoFooter), Yo(t), ul(t), rs(t), Fe(t, !0), Zt(t, null, "preInit", [t], !0), Pr(t);
     var n = Be(t);
-    n != "ssp" && (n == "ajax" ? ki(t, {}, function(s) {
-        var a = Dn(t, s);
+    n != "ssp" && (n == "ajax" ? Si(t, {}, function(s) {
+        var a = An(t, s);
         for (e = 0; e < a.length; e++) br(t, a[e]);
-        t.iInitDisplayStart = r, Pr(t), Fe(t, !1), wn(t)
-    }, t) : (wn(t), Fe(t, !1)))
+        t.iInitDisplayStart = r, Pr(t), Fe(t, !1), xn(t)
+    }, t) : (xn(t), Fe(t, !1)))
 }
 
-function wn(t) {
+function xn(t) {
     if (!t._bInitComplete) {
         var e = [t, t.json];
-        t._bInitComplete = !0, Tn(t), Zt(t, null, "plugin-init", e, !0), Zt(t, "aoInitComplete", "init", e, !0)
+        t._bInitComplete = !0, kn(t), Zt(t, null, "plugin-init", e, !0), Zt(t, "aoInitComplete", "init", e, !0)
     }
 }
 
-function Qa(t, e) {
+function Ja(t, e) {
     var r = parseInt(e, 10);
-    t._iDisplayLength = r, as(t), Zt(t, null, "length", [t, r])
+    t._iDisplayLength = r, ss(t), Zt(t, null, "length", [t, r])
 }
 
-function Si(t, e, r) {
+function Di(t, e, r) {
     var n = t._iDisplayStart,
         s = t._iDisplayLength,
         a = t.fnRecordsDisplay();
     if (a === 0 || s === -1) n = 0;
     else if (typeof e == "number") n = e * s, n > a && (n = 0);
     else if (e == "first") n = 0;
     else if (e == "previous") n = s >= 0 ? n - s : 0, n < 0 && (n = 0);
@@ -7953,33 +7959,34 @@
         if (e === "ellipsis") return;
         Pe(t, 0, "Unknown paging action: " + e, 5)
     }
     var l = t._iDisplayStart !== n;
     return t._iDisplayStart = n, Zt(t, null, l ? "page" : "page-nc", [t]), l && r && Fr(t), l
 }
 
-function sl(t) {
-    var e = t.nTable;
+function ol(t) {
+    var e = t.nTable,
+        r = t.oScroll.sX !== "" || t.oScroll.sY !== "";
     if (t.oFeatures.bProcessing) {
-        var r = W("<div/>", {
+        var n = W("<div/>", {
             id: t.sTableId + "_processing",
             class: t.oClasses.processing.container,
             role: "status"
-        }).html(t.oLanguage.sProcessing).append("<div><div></div><div></div><div></div><div></div></div>").insertBefore(e);
-        W(e).on("processing.dt.DT", function(n, s, a) {
-            r.css("display", a ? "block" : "none")
+        }).html(t.oLanguage.sProcessing).append("<div><div></div><div></div><div></div><div></div></div>");
+        r ? n.prependTo(W("div.dt-scroll", t.nTableWrapper)) : n.insertBefore(e), W(e).on("processing.dt.DT", function(s, a, l) {
+            n.css("display", l ? "block" : "none")
         })
     }
 }
 
 function Fe(t, e) {
     Zt(t, null, "processing", [t, e])
 }
 
-function Ja(t) {
+function ts(t) {
     var e = W(t.nTable),
         r = t.oScroll;
     if (r.sX === "" && r.sY === "") return t.nTable;
     var n = r.sX,
         s = r.sY,
         a = t.oClasses.scrolling,
         l = t.captionNode,
@@ -8028,18 +8035,18 @@
         h = m ? k[2] : null;
     return W(F).on("scroll.DT", function() {
         var o = this.scrollLeft;
         P.scrollLeft = o, m && (h.scrollLeft = o)
     }), W("th, td", P).on("focus", function() {
         var o = P.scrollLeft;
         F.scrollLeft = o, m && (F.scrollLeft = o)
-    }), W(F).css("max-height", s), r.bCollapse || W(F).css("height", s), t.nScrollHead = P, t.nScrollBody = F, t.nScrollFoot = h, t.aoDrawCallback.push(ts), w[0]
+    }), W(F).css("max-height", s), r.bCollapse || W(F).css("height", s), t.nScrollHead = P, t.nScrollBody = F, t.nScrollFoot = h, t.aoDrawCallback.push(es), w[0]
 }
 
-function ts(t) {
+function es(t) {
     var e = t.oScroll,
         r = e.iBarWidth,
         n = W(t.nScrollHead),
         s = n.children("div"),
         a = s.children("table"),
         l = t.nScrollBody,
         c = W(l),
@@ -8048,21 +8055,21 @@
         m = b.children("table"),
         y = W(t.nTHead),
         T = W(t.nTable),
         w = t.nTFoot && W("th, td", t.nTFoot).length ? W(t.nTFoot) : null,
         k = t.oBrowser,
         P, F, h = l.scrollHeight > l.clientHeight;
     if (t.scrollBarVis !== h && t.scrollBarVis !== void 0) {
-        t.scrollBarVis = h, Tn(t);
+        t.scrollBarVis = h, kn(t);
         return
     } else t.scrollBarVis = h;
     if (T.children("thead, tfoot").remove(), P = y.clone().prependTo(T), P.find("th, td").removeAttr("tabindex"), P.find("[id]").removeAttr("id"), w && (F = w.clone().prependTo(T), F.find("[id]").removeAttr("id")), t.aiDisplay.length)
-        for (var o = T.find("tbody tr").eq(0).find("th, td").map(function(et) {
+        for (var o = T.children("tbody").eq(0).children("tr").eq(0).children("th, td").map(function(et) {
                 return {
-                    idx: gi(t, et),
+                    idx: yi(t, et),
                     width: W(this).outerWidth()
                 }
             }), f = 0; f < o.length; f++) {
             var C = t.aoColumns[o[f].idx].colEl[0],
                 B = C.style.width.replace("px", "");
             B !== o[f].width && (C.style.width = o[f].width + "px")
         }
@@ -8073,44 +8080,44 @@
     });
     var u = Math.floor(T.height()) > l.clientHeight || c.css("overflow-y") == "scroll",
         z = "padding" + (k.bScrollbarLeft ? "Left" : "Right"),
         q = T.outerWidth();
     a.css("width", rr(q)), s.css("width", rr(q)).css(z, u ? r + "px" : "0px"), w && (m.css("width", rr(q)), b.css("width", rr(q)).css(z, u ? r + "px" : "0px")), T.children("colgroup").prependTo(T), c.trigger("scroll"), (t.bSorted || t.bFiltered) && !t._drawHold && (l.scrollTop = 0)
 }
 
-function ol(t) {
+function ll(t) {
     if (t.oFeatures.bAutoWidth) {
         var e = t.nTable,
             r = t.aoColumns,
             n = t.oScroll,
             s = n.sY,
             a = n.sX,
             l = n.sXInner,
-            c = yi(t, "bVisible"),
+            c = wi(t, "bVisible"),
             p = e.getAttribute("width"),
             b = e.parentNode,
             m, y, T, w = e.style.width;
         w && w.indexOf("%") !== -1 && (p = w), Zt(t, null, "column-calc", {
             visible: c
         }, !1);
         var k = W(e.cloneNode()).css("visibility", "hidden").removeAttr("id");
         k.append("<tbody>");
         var P = W("<tr/>").appendTo(k.find("tbody"));
         for (k.append(W(t.nTHead).clone()).append(W(t.nTFoot).clone()), k.find("tfoot th, tfoot td").css("width", ""), k.find("thead th, thead td").each(function() {
-                var et = Ga(t, this, !0, !1);
+                var et = Xa(t, this, !0, !1);
                 et ? (this.style.width = et, a && W(this).append(W("<div/>").css({
                     width: et,
                     margin: 0,
                     padding: 0,
                     border: 0,
                     height: 1
                 }))) : this.style.width = ""
             }), m = 0; m < c.length; m++) {
             T = c[m], y = r[T];
-            var F = ll(t, T),
+            var F = dl(t, T),
                 h = oe.type.className[y.sType],
                 o = F + y.sContentPadding,
                 f = F.indexOf("<") === -1 ? document.createTextNode(o) : o;
             W("<td/>").addClass(h).addClass(y.sClass).append(f).appendTo(P)
         }
         W("[name]", k).removeAttr("name");
         var C = W("<div/>").css(a || s ? {
@@ -8127,81 +8134,83 @@
         for (m = 0; m < c.length; m++) {
             var z = u[m].getBoundingClientRect().width;
             B += z, r[c[m]].sWidth = rr(z)
         }
         if (e.style.width = rr(B), C.remove(), p && (e.style.width = rr(p)), (p || a) && !t._reszEvt) {
             var q = function() {
                 W(window).on("resize.DT-" + t.sInstance, vt.util.throttle(function() {
-                    t.bDestroying || Tn(t)
+                    t.bDestroying || kn(t)
                 }))
             };
             q(), t._reszEvt = !0
         }
     }
 }
 
-function ll(t, e) {
+function dl(t, e) {
     var r = t.aoColumns[e];
     if (!r.maxLenString) {
         for (var n, s = "", a = -1, l = 0, c = t.aiDisplayMaster.length; l < c; l++) {
             var p = t.aiDisplayMaster[l],
-                b = Ti(t, p)[e],
+                b = ki(t, p)[e],
                 m = b && typeof b == "object" && b.nodeType ? b.innerHTML : b + "";
             m = m.replace(/id=".*?"/g, "").replace(/name=".*?"/g, ""), n = hr(m).replace(/&nbsp;/g, " "), n.length > a && (s = m, a = n.length)
         }
         r.maxLenString = s
     }
     return r.maxLenString
 }
 
 function rr(t) {
     return t === null ? "0px" : typeof t == "number" ? t < 0 ? "0px" : t + "px" : t.match(/\d$/) ? t + "px" : t
 }
 
-function es(t) {
+function rs(t) {
     var e = t.aoColumns;
     for (t.colgroup.empty(), Ie = 0; Ie < e.length; Ie++) e[Ie].bVisible && t.colgroup.append(e[Ie].colEl)
 }
 
-function dl(t) {
+function ul(t) {
     var e = t.nTHead,
         r = e.querySelectorAll("tr"),
         n = t.bSortCellsTop,
         s = ':not([data-dt-order="disable"]):not([data-dt-order="icon-only"])';
-    n === !0 ? e = r[0] : n === !1 && (e = r[r.length - 1]), rs(t, e, e === t.nTHead ? "tr" + s + " th" + s + ", tr" + s + " td" + s : "th" + s + ", td" + s);
+    n === !0 ? e = r[0] : n === !1 && (e = r[r.length - 1]), ns(t, e, e === t.nTHead ? "tr" + s + " th" + s + ", tr" + s + " td" + s : "th" + s + ", td" + s);
     var a = [];
     qr(t, a, t.aaSorting), t.aaSorting = a
 }
 
-function rs(t, e, r, n, s) {
-    is(e, r, function(a) {
+function ns(t, e, r, n, s) {
+    as(e, r, function(a) {
         var l = !1,
-            c = n === void 0 ? xi(a.target) : [n];
+            c = n === void 0 ? _i(a.target) : [n];
         if (c.length) {
             for (var p = 0, b = c.length; p < b; p++) {
-                var m = ul(t, c[p], p, a.shiftKey);
+                var m = cl(t, c[p], p, a.shiftKey);
                 if (m !== !1 && (l = !0), t.aaSorting.length === 1 && t.aaSorting[0][1] === "") break
             }
             l && (Fe(t, !0), setTimeout(function() {
-                Di(t), ns(t, t.aiDisplay), Fe(t, !1), Pr(t, !1, !1), s && s()
+                Ai(t), is(t, t.aiDisplay), Fe(t, !1), Pr(t, !1, !1), s && s()
             }, 0))
         }
     })
 }
 
-function ns(t, e) {
-    var r = t.aiDisplayMaster,
-        n = {},
-        s = {},
-        a;
-    for (a = 0; a < r.length; a++) n[r[a]] = a;
-    for (a = 0; a < e.length; a++) s[e[a]] = n[e[a]];
-    e.sort(function(l, c) {
-        return s[l] - s[c]
-    })
+function is(t, e) {
+    if (!(e.length < 2)) {
+        var r = t.aiDisplayMaster,
+            n = {},
+            s = {},
+            a;
+        for (a = 0; a < r.length; a++) n[r[a]] = a;
+        for (a = 0; a < e.length; a++) s[e[a]] = n[e[a]];
+        e.sort(function(l, c) {
+            return s[l] - s[c]
+        })
+    }
 }
 
 function qr(t, e, r) {
     var n = function(a) {
         if (W.isPlainObject(a)) {
             if (a.idx !== void 0) e.push([a.idx, a.dir]);
             else if (a.name) {
@@ -8213,15 +8222,15 @@
     };
     if (W.isPlainObject(r)) n(r);
     else if (r.length && typeof r[0] == "number") n(r);
     else if (r.length)
         for (var s = 0; s < r.length; s++) n(r[s])
 }
 
-function An(t) {
+function In(t) {
     var e, r, n, s = [],
         a = vt.ext.type.order,
         l = t.aoColumns,
         c, p, b, m, y = t.aaSortingFixed,
         T = W.isPlainObject(y),
         w = [];
     if (!t.oFeatures.bSort) return s;
@@ -8235,33 +8244,33 @@
                 type: b,
                 formatter: a[b + "-pre"],
                 sorter: a[b + "-" + w[e][1]]
             });
     return s
 }
 
-function Di(t, e, r) {
+function Ai(t, e, r) {
     var n, s, a, l = [],
         c = vt.ext.type.order,
         p = t.aoData,
         b, m = t.aiDisplayMaster,
         y;
-    if (wi(t), e !== void 0) {
+    if (xi(t), e !== void 0) {
         var T = t.aoColumns[e];
         y = [{
             src: e,
             col: e,
             dir: r,
             index: 0,
             type: T.sType,
             formatter: c[T.sType + "-pre"],
             sorter: c[T.sType + "-" + r]
         }], m = m.slice()
-    } else y = An(t);
-    for (n = 0, s = y.length; n < s; n++) b = y[n], cl(t, b.col);
+    } else y = In(t);
+    for (n = 0, s = y.length; n < s; n++) b = y[n], fl(t, b.col);
     if (Be(t) != "ssp" && y.length !== 0) {
         for (n = 0, a = m.length; n < a; n++) l[n] = n;
         y.length && y[0].dir === "desc" && l.reverse(), m.sort(function(w, k) {
             var P, F, h, o, f, C = y.length,
                 B = p[w]._aSortData,
                 u = p[k]._aSortData;
             for (h = 0; h < C; h++)
@@ -8272,51 +8281,51 @@
         })
     } else y.length === 0 && m.sort(function(w, k) {
         return w < k ? -1 : w > k ? 1 : 0
     });
     return e === void 0 && (t.bSorted = !0, Zt(t, null, "order", [t, y])), m
 }
 
-function ul(t, e, r, n) {
+function cl(t, e, r, n) {
     var s = t.aoColumns[e],
         a = t.aaSorting,
         l = s.asSorting,
         c, p = function(m, y) {
             var T = m._idx;
             return T === void 0 && (T = l.indexOf(m[1])), T + 1 < l.length ? T + 1 : y ? null : 0
         };
     if (!s.bSortable) return !1;
     if (typeof a[0] == "number" && (a = t.aaSorting = [a]), (n || r) && t.oFeatures.bSortMulti) {
         var b = xe(a, "0").indexOf(e);
         b !== -1 ? (c = p(a[b], !0), c === null && a.length === 1 && (c = 0), c === null ? a.splice(b, 1) : (a[b][1] = l[c], a[b]._idx = c)) : n ? (a.push([e, l[0], 0]), a[a.length - 1]._idx = 0) : (a.push([e, a[0][1], 0]), a[a.length - 1]._idx = 0)
     } else a.length && a[0][0] == e ? (c = p(a[0]), a.length = 1, a[0][1] = l[c], a[0]._idx = c) : (a.length = 0, a.push([e, l[0]]), a[0]._idx = 0)
 }
 
-function fi(t) {
+function hi(t) {
     var e = t.aLastSort,
         r = t.oClasses.order.position,
-        n = An(t),
+        n = In(t),
         s = t.oFeatures,
         a, l, c;
     if (s.bSort && s.bSortClasses) {
         for (a = 0, l = e.length; a < l; a++) c = e[a].src, W(xe(t.aoData, "anCells", c)).removeClass(r + (a < 2 ? a + 1 : 3));
         for (a = 0, l = n.length; a < l; a++) c = n[a].src, W(xe(t.aoData, "anCells", c)).addClass(r + (a < 2 ? a + 1 : 3))
     }
     t.aLastSort = n
 }
 
-function cl(t, e) {
+function fl(t, e) {
     var r = t.aoColumns[e],
         n = vt.ext.order[r.sSortDataType],
         s;
     n && (s = n.call(t.oInstance, t, e, $r(t, e)));
     for (var a, l, c = vt.ext.type.order[r.sType + "-pre"], p = t.aoData, b = 0; b < p.length; b++) p[b] && (a = p[b], a._aSortData || (a._aSortData = []), (!a._aSortData[e] || n) && (l = n ? s[b] : Ne(t, b, e, "sort"), a._aSortData[e] = c ? c(l, t) : l))
 }
 
-function In(t) {
+function Pn(t) {
     if (!t._bLoadingState) {
         var e = {
             time: +new Date,
             start: t._iDisplayStart,
             length: t._iDisplayLength,
             order: W.extend(!0, [], t.aaSorting),
             search: W.extend({}, t.oPreviousSearch),
@@ -8327,27 +8336,27 @@
                 }
             })
         };
         t.oSavedState = e, Zt(t, "aoStateSaveParams", "stateSaveParams", [t, e]), t.oFeatures.bStateSave && !t.bDestroying && t.fnStateSaveCallback.call(t.oInstance, t, e)
     }
 }
 
-function fl(t, e, r) {
+function hl(t, e, r) {
     if (!t.oFeatures.bStateSave) {
         r();
         return
     }
     var n = function(a) {
-            hi(t, a, r)
+            pi(t, a, r)
         },
         s = t.fnStateLoadCallback.call(t.oInstance, t, n);
-    return s !== void 0 && hi(t, s, r), !0
+    return s !== void 0 && pi(t, s, r), !0
 }
 
-function hi(t, e, r) {
+function pi(t, e, r) {
     var n, s, a = t.aoColumns;
     t._bLoadingState = !0;
     var l = t._bInitComplete ? new vt.Api(t) : null;
     if (!e || !e.time) {
         t._bLoadingState = !1, r();
         return
     }
@@ -8361,15 +8370,15 @@
         t._bLoadingState = !1, r();
         return
     }
     if (e.columns && a.length !== e.columns.length) {
         t._bLoadingState = !1, r();
         return
     }
-    if (t.oLoadedState = W.extend(!0, {}, e), Zt(t, null, "stateLoadInit", [t, e], !0), e.length !== void 0 && (l ? l.page.len(e.length) : t._iDisplayLength = e.length), e.start !== void 0 && (l === null ? (t._iDisplayStart = e.start, t.iInitDisplayStart = e.start) : Si(t, e.start / t._iDisplayLength)), e.order !== void 0 && (t.aaSorting = [], W.each(e.order, function(m, y) {
+    if (t.oLoadedState = W.extend(!0, {}, e), Zt(t, null, "stateLoadInit", [t, e], !0), e.length !== void 0 && (l ? l.page.len(e.length) : t._iDisplayLength = e.length), e.start !== void 0 && (l === null ? (t._iDisplayStart = e.start, t.iInitDisplayStart = e.start) : Di(t, e.start / t._iDisplayLength)), e.order !== void 0 && (t.aaSorting = [], W.each(e.order, function(m, y) {
             t.aaSorting.push(y[0] >= a.length ? [0, y[1]] : y)
         })), e.search !== void 0 && W.extend(t.oPreviousSearch, e.search), e.columns) {
         for (n = 0, s = e.columns.length; n < s; n++) {
             var b = e.columns[n];
             b.visible !== void 0 && (l ? l.column(n).visible(b.visible, !1) : a[n].bVisible = b.visible), b.search !== void 0 && W.extend(t.aoPreSearchCols[n], b.search)
         }
         l && l.columns.adjust()
@@ -8396,21 +8405,21 @@
             Array.isArray(a) ? nr(t, e, a[0], a[1]) : nr(t, e, a)
         });
         return
     }
     n === void 0 && (n = r), e[r] !== void 0 && (t[n] = e[r])
 }
 
-function Oa(t, e, r) {
+function Ra(t, e, r) {
     var n;
     for (var s in e) Object.prototype.hasOwnProperty.call(e, s) && (n = e[s], W.isPlainObject(n) ? (W.isPlainObject(t[s]) || (t[s] = {}), W.extend(!0, t[s], n)) : r && s !== "data" && s !== "aaData" && Array.isArray(n) ? t[s] = n.slice() : t[s] = n);
     return t
 }
 
-function is(t, e, r) {
+function as(t, e, r) {
     W(t).on("click.DT", e, function(n) {
         r(n)
     }).on("keypress.DT", e, function(n) {
         n.which === 13 && (n.preventDefault(), r(n))
     }).on("selectstart.DT", e, function() {
         return !1
     })
@@ -8428,43 +8437,43 @@
         var l = W.Event(r + ".dt"),
             c = W(t.nTable);
         l.dt = t.api, c[s ? "trigger" : "triggerHandler"](l, n), s && c.parents("body").length === 0 && W("body").trigger(l, n), a.push(l.result)
     }
     return a
 }
 
-function as(t) {
+function ss(t) {
     var e = t._iDisplayStart,
         r = t.fnDisplayEnd(),
         n = t._iDisplayLength;
     e >= r && (e = r - n), e -= e % n, (n === -1 || e < 0) && (e = 0), t._iDisplayStart = e
 }
 
-function xn(t, e) {
+function _n(t, e) {
     var r = t.renderer,
         n = vt.ext.renderer[e];
     return W.isPlainObject(r) && r[e] ? n[r[e]] || n._ : typeof r == "string" && n[r] || n._
 }
 
 function Be(t) {
     return t.oFeatures.bServerSide ? "ssp" : t.ajax ? "ajax" : "dom"
 }
 
-function Ai(t, e, r) {
+function Ii(t, e, r) {
     var n = t.fnFormatNumber,
         s = t._iDisplayStart + 1,
         a = t._iDisplayLength,
         l = t.fnRecordsDisplay(),
         c = t.fnRecordsTotal(),
         p = a === -1;
     return e.replace(/_START_/g, n.call(t, s)).replace(/_END_/g, n.call(t, t.fnDisplayEnd())).replace(/_MAX_/g, n.call(t, c)).replace(/_TOTAL_/g, n.call(t, l)).replace(/_PAGE_/g, n.call(t, p ? 1 : Math.ceil(s / a))).replace(/_PAGES_/g, n.call(t, p ? 1 : Math.ceil(l / a))).replace(/_ENTRIES_/g, t.api.i18n("entries", "", r)).replace(/_ENTRIES-MAX_/g, t.api.i18n("entries", "", c)).replace(/_ENTRIES-TOTAL_/g, t.api.i18n("entries", "", l))
 }
-var Ii = [],
+var Pi = [],
     fe = Array.prototype,
-    hl = function(t) {
+    pl = function(t) {
         var e, r, n = vt.settings,
             s = xe(n, "nTable");
         if (t) {
             if (t.nTable && t.oFeatures) return [t];
             if (t.nodeName && t.nodeName.toLowerCase() === "table") return e = s.indexOf(t), e !== -1 ? [n[e]] : null;
             if (t && typeof t.settings == "function") return t.settings().toArray();
             typeof t == "string" ? r = W(t).get() : t instanceof W && (r = t.get())
@@ -8473,25 +8482,25 @@
             return r.includes(s[l])
         })
     };
 Wt = function(t, e) {
     if (!(this instanceof Wt)) return new Wt(t, e);
     var r = [],
         n = function(l) {
-            var c = hl(l);
+            var c = pl(l);
             c && r.push.apply(r, c)
         };
     if (Array.isArray(t))
         for (var s = 0, a = t.length; s < a; s++) n(t[s]);
     else n(t);
     this.context = r.length > 1 ? pr(r) : r, e && this.push.apply(this, e), this.selector = {
         rows: null,
         cols: null,
         opts: null
-    }, Wt.extend(this, this, Ii)
+    }, Wt.extend(this, this, Pi)
 };
 vt.Api = Wt;
 W.extend(Wt.prototype, {
     any: function() {
         return this.count() !== 0
     },
     context: [],
@@ -8527,15 +8536,15 @@
             a, l, c, p, b, m = this.context,
             y, T, w, k = this.selector;
         for (typeof t == "string" && (n = r, r = e, e = t, t = !1), l = 0, c = m.length; l < c; l++) {
             var P = new Wt(m[l]);
             if (e === "table") a = r.call(P, m[l], l), a !== void 0 && s.push(a);
             else if (e === "columns" || e === "rows") a = r.call(P, m[l], this[l], l), a !== void 0 && s.push(a);
             else if (e === "every" || e === "column" || e === "column-rows" || e === "row" || e === "cell")
-                for (T = this[l], e === "column-rows" && (y = Pn(m[l], k.opts)), p = 0, b = T.length; p < b; p++) w = T[p], e === "cell" ? a = r.call(P, m[l], w.row, w.column, l, p) : a = r.call(P, m[l], w, l, p, y), a !== void 0 && s.push(a)
+                for (T = this[l], e === "column-rows" && (y = Fn(m[l], k.opts)), p = 0, b = T.length; p < b; p++) w = T[p], e === "cell" ? a = r.call(P, m[l], w.row, w.column, l, p) : a = r.call(P, m[l], w, l, p, y), a !== void 0 && s.push(a)
         }
         if (s.length || n) {
             var F = new Wt(m, t ? s.concat.apply([], s) : s),
                 h = F.selector;
             return h.rows = k.rows, h.cols = k.cols, h.opts = k.opts, F
         }
         return this
@@ -8575,44 +8584,44 @@
     },
     unique: function() {
         return new Wt(this.context, pr(this.toArray()))
     },
     unshift: fe.unshift
 });
 
-function pl(t, e, r) {
+function bl(t, e, r) {
     return function() {
         var n = e.apply(t || this, arguments);
         return Wt.extend(n, n, r.methodExt), n
     }
 }
 
-function bl(t, e) {
+function vl(t, e) {
     for (var r = 0, n = t.length; r < n; r++)
         if (t[r].name === e) return t[r];
     return null
 }
-window.__apiStruct = Ii;
+window.__apiStruct = Pi;
 Wt.extend = function(t, e, r) {
     if (!(!r.length || !e || !(e instanceof Wt) && !e.__dt_wrapper)) {
         var n, s, a;
-        for (n = 0, s = r.length; n < s; n++) a = r[n], a.name !== "__proto__" && (e[a.name] = a.type === "function" ? pl(t, a.val, a) : a.type === "object" ? {} : a.val, e[a.name].__dt_wrapper = !0, Wt.extend(t, e[a.name], a.propExt))
+        for (n = 0, s = r.length; n < s; n++) a = r[n], a.name !== "__proto__" && (e[a.name] = a.type === "function" ? bl(t, a.val, a) : a.type === "object" ? {} : a.val, e[a.name].__dt_wrapper = !0, Wt.extend(t, e[a.name], a.propExt))
     }
 };
 Wt.register = It = function(t, e) {
     if (Array.isArray(t)) {
         for (var r = 0, n = t.length; r < n; r++) Wt.register(t[r], e);
         return
     }
     var s, a, l = t.split("."),
-        c = Ii,
+        c = Pi,
         p, b;
     for (s = 0, a = l.length; s < a; s++) {
         b = l[s].indexOf("()") !== -1, p = b ? l[s].replace("()", "") : l[s];
-        var m = bl(c, p);
+        var m = vl(c, p);
         m || (m = {
             name: p,
             val: {},
             methodExt: [],
             propExt: [],
             type: "object"
         }, c.push(m)), s === a - 1 ? (m.val = e, m.type = typeof e == "function" ? "function" : W.isPlainObject(e) ? "object" : "other") : c = b ? m.methodExt : m.propExt
@@ -8620,19 +8629,19 @@
 };
 Wt.registerPlural = Qt = function(t, e, r) {
     Wt.register(t, r), Wt.register(e, function() {
         var n = r.apply(this, arguments);
         return n === this ? this : n instanceof Wt ? n.length ? Array.isArray(n[0]) ? new Wt(n.context, n[0]) : n[0] : void 0 : n
     })
 };
-var ss = function(t, e) {
+var os = function(t, e) {
     if (Array.isArray(t)) {
         var r = [];
         return t.forEach(function(s) {
-            var a = ss(s, e);
+            var a = os(s, e);
             r.push.apply(r, a)
         }), r.filter(function(s) {
             return s
         })
     }
     if (typeof t == "number") return [e[t]];
     var n = e.map(function(s) {
@@ -8640,15 +8649,15 @@
     });
     return W(n).filter(t).map(function() {
         var s = n.indexOf(this);
         return e[s]
     }).toArray()
 };
 It("tables()", function(t) {
-    return t != null ? new Wt(ss(t, this.context)) : this
+    return t != null ? new Wt(os(t, this.context)) : this
 });
 It("table()", function(t) {
     var e = this.tables(t),
         r = e.context;
     return r.length ? new Wt(r[0]) : e
 });
 [
@@ -8666,15 +8675,15 @@
 [
     ["header", "aoHeader"],
     ["footer", "aoFooter"]
 ].forEach(function(t) {
     It("table()." + t[0] + ".structure()", function(e) {
         var r = this.columns(e).indexes().flatten(),
             n = this.context[0];
-        return Ka(n, n[t[1]], r)
+        return Ya(n, n[t[1]], r)
     })
 });
 Qt("tables().containers()", "table().container()", function() {
     return this.iterator("table", function(t) {
         return t.nTableWrapper
     }, 1)
 });
@@ -8707,15 +8716,15 @@
 It("draw()", function(t) {
     return this.iterator("table", function(e) {
         t === "page" ? Fr(e) : (typeof t == "string" && (t = t !== "full-hold"), Pr(e, t === !1))
     })
 });
 It("page()", function(t) {
     return t === void 0 ? this.page.info().page : this.iterator("table", function(e) {
-        Si(e, t)
+        Di(e, t)
     })
 });
 It("page.info()", function() {
     if (this.context.length !== 0) {
         var t = this.context[0],
             e = t._iDisplayStart,
             r = t.oFeatures.bPaginate ? t._iDisplayLength : -1,
@@ -8731,83 +8740,83 @@
             recordsDisplay: n,
             serverSide: Be(t) === "ssp"
         }
     }
 });
 It("page.len()", function(t) {
     return t === void 0 ? this.context.length !== 0 ? this.context[0]._iDisplayLength : void 0 : this.iterator("table", function(e) {
-        Qa(e, t)
+        Ja(e, t)
     })
 });
-var os = function(t, e, r) {
+var ls = function(t, e, r) {
     if (r) {
         var n = new Wt(t);
         n.one("draw", function() {
             r(n.ajax.json())
         })
     }
     if (Be(t) == "ssp") Pr(t, e);
     else {
         Fe(t, !0);
         var s = t.jqXHR;
-        s && s.readyState !== 4 && s.abort(), ki(t, {}, function(a) {
-            Ci(t);
-            for (var l = Dn(t, a), c = 0, p = l.length; c < p; c++) br(t, l[c]);
-            Pr(t, e), wn(t), Fe(t, !1)
+        s && s.readyState !== 4 && s.abort(), Si(t, {}, function(a) {
+            Ti(t);
+            for (var l = An(t, a), c = 0, p = l.length; c < p; c++) br(t, l[c]);
+            Pr(t, e), xn(t), Fe(t, !1)
         })
     }
 };
 It("ajax.json()", function() {
     var t = this.context;
     if (t.length > 0) return t[0].json
 });
 It("ajax.params()", function() {
     var t = this.context;
     if (t.length > 0) return t[0].oAjaxData
 });
 It("ajax.reload()", function(t, e) {
     return this.iterator("table", function(r) {
-        os(r, e === !1, t)
+        ls(r, e === !1, t)
     })
 });
 It("ajax.url()", function(t) {
     var e = this.context;
     return t === void 0 ? e.length === 0 ? void 0 : (e = e[0], W.isPlainObject(e.ajax) ? e.ajax.url : e.ajax) : this.iterator("table", function(r) {
         W.isPlainObject(r.ajax) ? r.ajax.url = t : r.ajax = t
     })
 });
 It("ajax.url().load()", function(t, e) {
     return this.iterator("table", function(r) {
-        os(r, e === !1, t)
+        ls(r, e === !1, t)
     })
 });
-var Pi = function(t, e, r, n, s) {
+var Fi = function(t, e, r, n, s) {
         var a = [],
             l, c, p, b, m, y, T = typeof e;
         for ((!e || T === "string" || T === "function" || e.length === void 0) && (e = [e]), p = 0, b = e.length; p < b; p++)
             for (c = e[p] && e[p].split && !e[p].match(/[[(:]/) ? e[p].split(",") : [e[p]], m = 0, y = c.length; m < y; m++) l = r(typeof c[m] == "string" ? c[m].trim() : c[m]), l = l.filter(function(k) {
                 return k != null
             }), l && l.length && (a = a.concat(l));
         var w = oe.selector[t];
         if (w.length)
             for (p = 0, b = w.length; p < b; p++) a = w[p](n, s, a);
         return pr(a)
     },
-    Fi = function(t) {
+    Bi = function(t) {
         return t || (t = {}), t.filter && t.search === void 0 && (t.search = t.filter), W.extend({
             search: "none",
             order: "current",
             page: "all"
         }, t)
     },
-    Bi = function(t) {
+    Ni = function(t) {
         let e = new Wt(t.context[0]);
         return t.length && e.push(t[0]), e.selector = t.selector, e.length && e[0].length > 1 && e[0].splice(1), e
     },
-    Pn = function(t, e) {
+    Fn = function(t, e) {
         var r, n, s, a = [],
             l = t.aiDisplay,
             c = t.aiDisplayMaster,
             p = e.search,
             b = e.order,
             m = e.page;
         if (m == "current")
@@ -8821,27 +8830,27 @@
                 c.forEach(function(w) {
                     Object.prototype.hasOwnProperty.call(y, w) || a.push(w)
                 })
             }
         } else if (b == "index" || b == "original")
             for (r = 0, n = t.aoData.length; r < n; r++) t.aoData[r] && (p == "none" ? a.push(r) : (s = l.indexOf(r), (s === -1 && p == "removed" || s >= 0 && p == "applied") && a.push(r)));
         else if (typeof b == "number") {
-            var T = Di(t, b, "asc");
+            var T = Ai(t, b, "asc");
             if (p === "none") a = T;
             else
                 for (r = 0; r < T.length; r++) s = l.indexOf(T[r]), (s === -1 && p == "removed" || s >= 0 && p == "applied") && a.push(T[r])
         }
         return a
     },
-    vl = function(t, e, r) {
+    ml = function(t, e, r) {
         var n, s = function(l) {
-                var c = Ma(l),
+                var c = Va(l),
                     p = t.aoData;
                 if (c !== null && !r) return [c];
-                if (n || (n = Pn(t, r)), c !== null && n.indexOf(c) !== -1) return [c];
+                if (n || (n = Fn(t, r)), c !== null && n.indexOf(c) !== -1) return [c];
                 if (l == null || l === "") return n;
                 if (typeof l == "function") return n.map(function(k) {
                     var P = p[k];
                     return l(k, P._aData, P.nTr) ? k : null
                 });
                 if (l.nodeName) {
                     var b = l._DT_RowIndex,
@@ -8851,26 +8860,26 @@
                     var y = W(l).closest("*[data-dt-row]");
                     return y.length ? [y.data("dt-row")] : []
                 }
                 if (typeof l == "string" && l.charAt(0) === "#") {
                     var T = t.aIds[l.replace(/^#/, "")];
                     if (T !== void 0) return [T.idx]
                 }
-                var w = Wa(Xr(t.aoData, n, "nTr"));
+                var w = Ua(Xr(t.aoData, n, "nTr"));
                 return W(w).filter(l).map(function() {
                     return this._DT_RowIndex
                 }).toArray()
             },
-            a = Pi("row", e, s, t, r);
-        return (r.order === "current" || r.order === "applied") && ns(t, a), a
+            a = Fi("row", e, s, t, r);
+        return (r.order === "current" || r.order === "applied") && is(t, a), a
     };
 It("rows()", function(t, e) {
-    t === void 0 ? t = "" : W.isPlainObject(t) && (e = t, t = ""), e = Fi(e);
+    t === void 0 ? t = "" : W.isPlainObject(t) && (e = t, t = ""), e = Bi(e);
     var r = this.iterator("table", function(n) {
-        return vl(n, t, e)
+        return ml(n, t, e)
     }, 1);
     return r.selector.rows = t, r.selector.opts = e, r
 });
 It("rows().nodes()", function() {
     return this.iterator("row", function(t, e) {
         return t.aoData[e].nTr || void 0
     }, 1)
@@ -8884,15 +8893,15 @@
     return this.iterator("row", function(e, r) {
         var n = e.aoData[r];
         return t === "search" ? n._aFilterData : n._aSortData
     }, 1)
 });
 Qt("rows().invalidate()", "row().invalidate()", function(t) {
     return this.iterator("row", function(e, r) {
-        Sn(e, r, t)
+        Dn(e, r, t)
     })
 });
 Qt("rows().indexes()", "row().index()", function() {
     return this.iterator("row", function(t, e) {
         return e
     }, 1)
 });
@@ -8905,101 +8914,105 @@
     return new Wt(r, e)
 });
 Qt("rows().remove()", "row().remove()", function() {
     return this.iterator("row", function(t, e) {
         var r = t.aoData,
             n = r[e],
             s = t.aiDisplayMaster.indexOf(e);
-        s !== -1 && t.aiDisplayMaster.splice(s, 1), t._iRecordsDisplay > 0 && t._iRecordsDisplay--, as(t);
+        s !== -1 && t.aiDisplayMaster.splice(s, 1), t._iRecordsDisplay > 0 && t._iRecordsDisplay--, ss(t);
         var a = t.rowIdFn(n._aData);
         a !== void 0 && delete t.aIds[a], r[e] = null
     }), this
 });
 It("rows.add()", function(t) {
     var e = this.iterator("table", function(n) {
             var s, a, l, c = [];
-            for (a = 0, l = t.length; a < l; a++) s = t[a], s.nodeName && s.nodeName.toUpperCase() === "TR" ? c.push(_i(n, s)[0]) : c.push(br(n, s));
+            for (a = 0, l = t.length; a < l; a++) s = t[a], s.nodeName && s.nodeName.toUpperCase() === "TR" ? c.push(Ci(n, s)[0]) : c.push(br(n, s));
             return c
         }, 1),
         r = this.rows(-1);
     return r.pop(), r.push.apply(r, e), r
 });
 It("row()", function(t, e) {
-    return Bi(this.rows(t, e))
+    return Ni(this.rows(t, e))
 });
 It("row().data()", function(t) {
     var e = this.context;
     if (t === void 0) return e.length && this.length && this[0].length ? e[0].aoData[this[0]]._aData : void 0;
     var r = e[0].aoData[this[0]];
-    return r._aData = t, Array.isArray(t) && r.nTr && r.nTr.id && fr(e[0].rowId)(t, r.nTr.id), Sn(e[0], this[0], "data"), this
+    return r._aData = t, Array.isArray(t) && r.nTr && r.nTr.id && fr(e[0].rowId)(t, r.nTr.id), Dn(e[0], this[0], "data"), this
 });
 It("row().node()", function() {
     var t = this.context;
-    return t.length && this.length && this[0].length && t[0].aoData[this[0]].nTr || null
+    if (t.length && this.length && this[0].length) {
+        var e = t[0].aoData[this[0]];
+        if (e && e.nTr) return e.nTr
+    }
+    return null
 });
 It("row.add()", function(t) {
     t instanceof W && t.length && (t = t[0]);
     var e = this.iterator("table", function(r) {
-        return t.nodeName && t.nodeName.toUpperCase() === "TR" ? _i(r, t)[0] : br(r, t)
+        return t.nodeName && t.nodeName.toUpperCase() === "TR" ? Ci(r, t)[0] : br(r, t)
     });
     return this.row(e[0])
 });
 W(document).on("plugin-init.dt", function(t, e) {
     var r = new Wt(e);
     r.on("stateSaveParams.DT", function(n, s, a) {
         for (var l = s.rowIdFn, c = s.aiDisplayMaster, p = [], b = 0; b < c.length; b++) {
             var m = c[b],
                 y = s.aoData[m];
             y._detailsShow && p.push("#" + l(y._aData))
         }
         a.childRows = p
     }), r.on("stateLoaded.DT", function(n, s, a) {
-        Ra(r, a)
-    }), Ra(r, r.state.loaded())
+        La(r, a)
+    }), La(r, r.state.loaded())
 });
-var Ra = function(t, e) {
+var La = function(t, e) {
         e && e.childRows && t.rows(e.childRows.map(function(r) {
-            return r.replace(/(?<!\\):/g, "\\:")
+            return r.replace(/([^:\\]*(?:\\.[^:\\]*)*):/g, "$1\\:")
         })).every(function() {
             Zt(t.settings()[0], null, "requestChild", [this])
         })
     },
-    ml = function(t, e, r, n) {
+    gl = function(t, e, r, n) {
         var s = [],
             a = function(l, c) {
                 if (Array.isArray(l) || l instanceof W) {
                     for (var p = 0, b = l.length; p < b; p++) a(l[p], c);
                     return
                 }
                 if (l.nodeName && l.nodeName.toLowerCase() === "tr") l.setAttribute("data-dt-row", e.idx), s.push(l);
                 else {
                     var m = W("<tr><td></td></tr>").attr("data-dt-row", e.idx).addClass(c);
-                    W("td", m).addClass(c).html(l)[0].colSpan = kn(t), s.push(m[0])
+                    W("td", m).addClass(c).html(l)[0].colSpan = Sn(t), s.push(m[0])
                 }
             };
         a(r, n), e._details && e._details.detach(), e._details = W(s), e._detailsShow && e._details.insertAfter(e.nTr)
     },
-    ls = vt.util.throttle(function(t) {
-        In(t[0])
+    ds = vt.util.throttle(function(t) {
+        Pn(t[0])
     }, 500),
-    Ni = function(t, e) {
+    Ei = function(t, e) {
         var r = t.context;
         if (r.length) {
             var n = r[0].aoData[e !== void 0 ? e : t[0]];
-            n && n._details && (n._details.remove(), n._detailsShow = void 0, n._details = void 0, W(n.nTr).removeClass("dt-hasChild"), ls(r))
+            n && n._details && (n._details.remove(), n._detailsShow = void 0, n._details = void 0, W(n.nTr).removeClass("dt-hasChild"), ds(r))
         }
     },
-    ds = function(t, e) {
+    us = function(t, e) {
         var r = t.context;
         if (r.length && t.length) {
             var n = r[0].aoData[t[0]];
-            n._details && (n._detailsShow = e, e ? (n._details.insertAfter(n.nTr), W(n.nTr).addClass("dt-hasChild")) : (n._details.detach(), W(n.nTr).removeClass("dt-hasChild")), Zt(r[0], null, "childRow", [e, t.row(t[0])]), gl(r[0]), ls(r))
+            n._details && (n._detailsShow = e, e ? (n._details.insertAfter(n.nTr), W(n.nTr).addClass("dt-hasChild")) : (n._details.detach(), W(n.nTr).removeClass("dt-hasChild")), Zt(r[0], null, "childRow", [e, t.row(t[0])]), yl(r[0]), ds(r))
         }
     },
-    gl = function(t) {
+    yl = function(t) {
         var e = new Wt(t),
             r = ".dt.DT_details",
             n = "draw" + r,
             s = "column-sizing" + r,
             a = "destroy" + r,
             l = t.aoData;
         e.off(n + " " + s + " " + a), xe(l, "_details").length > 0 && (e.on(n, function(c, p) {
@@ -9007,139 +9020,139 @@
                 page: "current"
             }).eq(0).each(function(b) {
                 var m = l[b];
                 m._detailsShow && m._details.insertAfter(m.nTr)
             })
         }), e.on(s, function(c, p) {
             if (t === p)
-                for (var b, m = kn(p), y = 0, T = l.length; y < T; y++) b = l[y], b && b._details && b._details.each(function() {
+                for (var b, m = Sn(p), y = 0, T = l.length; y < T; y++) b = l[y], b && b._details && b._details.each(function() {
                     var w = W(this).children("td");
                     w.length == 1 && w.attr("colspan", m)
                 })
         }), e.on(a, function(c, p) {
             if (t === p)
-                for (var b = 0, m = l.length; b < m; b++) l[b] && l[b]._details && Ni(e, b)
+                for (var b = 0, m = l.length; b < m; b++) l[b] && l[b]._details && Ei(e, b)
         }))
     },
-    yl = "",
-    Zr = yl + "row().child",
-    Fn = Zr + "()";
-It(Fn, function(t, e) {
+    wl = "",
+    Zr = wl + "row().child",
+    Bn = Zr + "()";
+It(Bn, function(t, e) {
     var r = this.context;
-    return t === void 0 ? r.length && this.length && r[0].aoData[this[0]] ? r[0].aoData[this[0]]._details : void 0 : (t === !0 ? this.child.show() : t === !1 ? Ni(this) : r.length && this.length && ml(r[0], r[0].aoData[this[0]], t, e), this)
+    return t === void 0 ? r.length && this.length && r[0].aoData[this[0]] ? r[0].aoData[this[0]]._details : void 0 : (t === !0 ? this.child.show() : t === !1 ? Ei(this) : r.length && this.length && gl(r[0], r[0].aoData[this[0]], t, e), this)
 });
-It([Zr + ".show()", Fn + ".show()"], function() {
-    return ds(this, !0), this
+It([Zr + ".show()", Bn + ".show()"], function() {
+    return us(this, !0), this
 });
-It([Zr + ".hide()", Fn + ".hide()"], function() {
-    return ds(this, !1), this
+It([Zr + ".hide()", Bn + ".hide()"], function() {
+    return us(this, !1), this
 });
-It([Zr + ".remove()", Fn + ".remove()"], function() {
-    return Ni(this), this
+It([Zr + ".remove()", Bn + ".remove()"], function() {
+    return Ei(this), this
 });
 It(Zr + ".isShown()", function() {
     var t = this.context;
     return t.length && this.length && t[0].aoData[this[0]]._detailsShow || !1
 });
-var wl = /^([^:]+):(name|title|visIdx|visible)$/,
-    Ei = function(t, e, r, n, s, a) {
+var xl = /^([^:]+):(name|title|visIdx|visible)$/,
+    Oi = function(t, e, r, n, s, a) {
         for (var l = [], c = 0, p = s.length; c < p; c++) l.push(Ne(t, s[c], e, a));
         return l
     },
-    us = function(t, e, r) {
+    cs = function(t, e, r) {
         var n = t.aoHeader,
             s = r !== void 0 ? r : t.bSortCellsTop ? 0 : n.length - 1;
         return n[s][e].cell
     },
-    xl = function(t, e, r) {
+    _l = function(t, e, r) {
         var n = t.aoColumns,
             s = xe(n, "sName"),
             a = xe(n, "sTitle"),
             l = vt.util.get("[].[].cell")(t.aoHeader),
-            c = pr(mi([], l)),
+            c = pr(gi([], l)),
             p = function(b) {
-                var m = Ma(b);
+                var m = Va(b);
                 if (b === "") return cr(n.length);
                 if (m !== null) return [m >= 0 ? m : n.length + m];
                 if (typeof b == "function") {
-                    var y = Pn(t, r);
+                    var y = Fn(t, r);
                     return n.map(function(h, o) {
-                        return b(o, Ei(t, o, 0, 0, y), us(t, o)) ? o : null
+                        return b(o, Oi(t, o, 0, 0, y), cs(t, o)) ? o : null
                     })
                 }
-                var T = typeof b == "string" ? b.match(wl) : "";
+                var T = typeof b == "string" ? b.match(xl) : "";
                 if (T) switch (T[2]) {
                     case "visIdx":
                     case "visible":
                         var w = parseInt(T[1], 10);
                         if (w < 0) {
                             var k = n.map(function(h, o) {
                                 return h.bVisible ? o : null
                             });
                             return [k[k.length + w]]
                         }
-                        return [gi(t, w)];
+                        return [yi(t, w)];
                     case "name":
                         return s.map(function(h, o) {
                             return h === T[1] ? o : null
                         });
                     case "title":
                         return a.map(function(h, o) {
                             return h === T[1] ? o : null
                         });
                     default:
                         return []
                 }
                 if (b.nodeName && b._DT_CellIndex) return [b._DT_CellIndex.column];
                 var P = W(c).filter(b).map(function() {
-                    return xi(this)
+                    return _i(this)
                 }).toArray();
                 if (P.length || !b.nodeName) return P;
                 var F = W(b).closest("*[data-dt-column]");
                 return F.length ? [F.data("dt-column")] : []
             };
-        return Pi("column", e, p, t, r)
+        return Fi("column", e, p, t, r)
     },
-    _l = function(t, e, r) {
+    Cl = function(t, e, r) {
         var n = t.aoColumns,
             s = n[e],
             a = t.aoData,
             l, c, p, b;
         if (r === void 0) return s.bVisible;
         if (s.bVisible === r) return !1;
         if (r) {
             var m = xe(n, "bVisible").indexOf(!0, e + 1);
             for (c = 0, p = a.length; c < p; c++) a[c] && (b = a[c].nTr, l = a[c].anCells, b && b.insertBefore(l[e], l[m] || null))
         } else W(xe(t.aoData, "anCells", e)).detach();
-        return s.bVisible = r, es(t), !0
+        return s.bVisible = r, rs(t), !0
     };
 It("columns()", function(t, e) {
-    t === void 0 ? t = "" : W.isPlainObject(t) && (e = t, t = ""), e = Fi(e);
+    t === void 0 ? t = "" : W.isPlainObject(t) && (e = t, t = ""), e = Bi(e);
     var r = this.iterator("table", function(n) {
-        return xl(n, t, e)
+        return _l(n, t, e)
     }, 1);
     return r.selector.cols = t, r.selector.opts = e, r
 });
 Qt("columns().header()", "column().header()", function(t) {
     return this.iterator("column", function(e, r) {
-        return us(e, r, t)
+        return cs(e, r, t)
     }, 1)
 });
 Qt("columns().footer()", "column().footer()", function(t) {
     return this.iterator("column", function(e, r) {
         var n = e.aoFooter;
         return n.length ? e.aoFooter[t !== void 0 ? t : 0][r].cell : null
     }, 1)
 });
 Qt("columns().data()", "column().data()", function() {
-    return this.iterator("column-rows", Ei, 1)
+    return this.iterator("column-rows", Oi, 1)
 });
 Qt("columns().render()", "column().render()", function(t) {
     return this.iterator("column-rows", function(e, r, n, s, a) {
-        return Ei(e, r, n, s, a, t)
+        return Oi(e, r, n, s, a, t)
     }, 1)
 });
 Qt("columns().dataSrc()", "column().dataSrc()", function() {
     return this.iterator("column", function(t, e) {
         return t.aoColumns[e].mData
     }, 1)
 });
@@ -9164,26 +9177,26 @@
         var s = W("span.dt-column-title", this.column(n).header(e));
         return t !== void 0 ? (s.html(t), this) : s.html()
     }, 1)
 });
 Qt("columns().types()", "column().type()", function() {
     return this.iterator("column", function(t, e) {
         var r = t.aoColumns[e].sType;
-        return r || wi(t), r
+        return r || xi(t), r
     }, 1)
 });
 Qt("columns().visible()", "column().visible()", function(t, e) {
     var r = this,
         n = [],
         s = this.iterator("column", function(a, l) {
             if (t === void 0) return a.aoColumns[l].bVisible;
-            _l(a, l, t) && n.push(l)
+            Cl(a, l, t) && n.push(l)
         });
     return t !== void 0 && this.iterator("table", function(a) {
-        yn(a, a.aoHeader), yn(a, a.aoFooter), a.aiDisplay.length || W(a.nTBody).find("td[colspan]").attr("colspan", kn(a)), In(a), r.iterator("column", function(l, c) {
+        wn(a, a.aoHeader), wn(a, a.aoFooter), a.aiDisplay.length || W(a.nTBody).find("td[colspan]").attr("colspan", Sn(a)), Pn(a), r.iterator("column", function(l, c) {
             n.includes(c) && Zt(l, null, "column-visibility", [l, c, t, e])
         }), n.length && (e === void 0 || e) && r.columns.adjust()
     }), s
 });
 Qt("columns().widths()", "column().width()", function() {
     var t = this.columns(":visible").count(),
         e = W("<tr>").html("<td>" + Array(t).join("</td><td>") + "</td>");
@@ -9199,32 +9212,32 @@
 Qt("columns().indexes()", "column().index()", function(t) {
     return this.iterator("column", function(e, r) {
         return t === "visible" ? $r(e, r) : r
     }, 1)
 });
 It("columns.adjust()", function() {
     return this.iterator("table", function(t) {
-        Tn(t)
+        kn(t)
     }, 1)
 });
 It("column.index()", function(t, e) {
     if (this.context.length !== 0) {
         var r = this.context[0];
-        if (t === "fromVisible" || t === "toData") return gi(r, e);
+        if (t === "fromVisible" || t === "toData") return yi(r, e);
         if (t === "fromData" || t === "toVisible") return $r(r, e)
     }
 });
 It("column()", function(t, e) {
-    return Bi(this.columns(t, e))
+    return Ni(this.columns(t, e))
 });
-var Cl = function(t, e, r) {
+var Tl = function(t, e, r) {
     var n = t.aoData,
-        s = Pn(t, r),
-        a = Wa(Xr(n, s, "anCells")),
-        l = W(mi([], a)),
+        s = Fn(t, r),
+        a = Ua(Xr(n, s, "anCells")),
+        l = W(gi([], a)),
         c, p = t.aoColumns.length,
         b, m, y, T, w, k, P = function(F) {
             var h = typeof F == "function";
             if (F == null || h) {
                 for (b = [], m = 0, y = s.length; m < y; m++)
                     for (c = s[m], T = 0; T < p; T++) w = {
                         row: c,
@@ -9240,19 +9253,19 @@
                 }
             }).toArray();
             return o.length || !F.nodeName ? o : (k = W(F).closest("*[data-dt-row]"), k.length ? [{
                 row: k.data("dt-row"),
                 column: k.data("dt-column")
             }] : [])
         };
-    return Pi("cell", e, P, t, r)
+    return Fi("cell", e, P, t, r)
 };
 It("cells()", function(t, e, r) {
     if (W.isPlainObject(t) && (t.row === void 0 ? (r = t, t = null) : (r = e, e = null)), W.isPlainObject(e) && (r = e, e = null), e == null) return this.iterator("table", function(T) {
-        return Cl(T, t, Fi(r))
+        return Tl(T, t, Bi(r))
     });
     var n = r ? {
             page: r.page,
             order: r.order,
             search: r.search
         } : {},
         s = this.columns(e, n),
@@ -9301,37 +9314,37 @@
             column: r,
             columnVisible: $r(t, r)
         }
     }, 1)
 });
 Qt("cells().invalidate()", "cell().invalidate()", function(t) {
     return this.iterator("cell", function(e, r, n) {
-        Sn(e, r, t, n)
+        Dn(e, r, t, n)
     })
 });
 It("cell()", function(t, e, r) {
-    return Bi(this.cells(t, e, r))
+    return Ni(this.cells(t, e, r))
 });
 It("cell().data()", function(t) {
     var e = this.context,
         r = this[0];
-    return t === void 0 ? e.length && r.length ? Ne(e[0], r[0].row, r[0].column) : void 0 : (Zo(e[0], r[0].row, r[0].column, t), Sn(e[0], r[0].row, "data", r[0].column), this)
+    return t === void 0 ? e.length && r.length ? Ne(e[0], r[0].row, r[0].column) : void 0 : (Ko(e[0], r[0].row, r[0].column, t), Dn(e[0], r[0].row, "data", r[0].column), this)
 });
 It("order()", function(t, e) {
     var r = this.context,
         n = Array.prototype.slice.call(arguments);
     return t === void 0 ? r.length !== 0 ? r[0].aaSorting : void 0 : (typeof t == "number" ? t = [
         [t, e]
     ] : n.length > 1 && (t = n), this.iterator("table", function(s) {
         s.aaSorting = Array.isArray(t) ? t.slice() : t
     }))
 });
 It("order.listener()", function(t, e, r) {
     return this.iterator("table", function(n) {
-        rs(n, t, {}, e, r)
+        ns(n, t, {}, e, r)
     })
 });
 It("order.fixed()", function(t) {
     if (!t) {
         var e = this.context,
             r = e.length ? e[0].aaSortingFixed : void 0;
         return Array.isArray(r) ? {
@@ -9345,15 +9358,15 @@
 It(["columns().order()", "column().order()"], function(t) {
     var e = this;
     return t ? this.iterator("table", function(r, n) {
         r.aaSorting = e[n].map(function(s) {
             return [s, t]
         })
     }) : this.iterator("column", function(r, n) {
-        for (var s = An(r), a = 0, l = s.length; a < l; a++)
+        for (var s = In(r), a = 0, l = s.length; a < l; a++)
             if (s[a].col === n) return s[a].dir;
         return null
     }, 1)
 });
 Qt("columns().orderable()", "column().orderable()", function(t) {
     return this.iterator("column", function(e, r) {
         var n = e.aoColumns[r];
@@ -9414,28 +9427,28 @@
     });
     return t !== void 0 && e === void 0 ? r[0] : r
 });
 It("state()", function(t, e) {
     if (!t) return this.context.length ? this.context[0].oSavedState : null;
     var r = W.extend(!0, {}, t);
     return this.iterator("table", function(n) {
-        e !== !1 && (r.time = +new Date + 100), hi(n, r, function() {})
+        e !== !1 && (r.time = +new Date + 100), pi(n, r, function() {})
     })
 });
 It("state.clear()", function() {
     return this.iterator("table", function(t) {
         t.fnStateSaveCallback.call(t.oInstance, t, {})
     })
 });
 It("state.loaded()", function() {
     return this.context.length ? this.context[0].oLoadedState : null
 });
 It("state.save()", function() {
     return this.iterator("table", function(t) {
-        In(t)
+        Pn(t)
     })
 });
 vt.use = function(t, e) {
     e === "lib" || t.fn ? W = t : e == "win" || t.document ? (window = t, document = t.document) : (e === "datetime" || t.type === "DateTime") && (vt.DateTime = t)
 };
 vt.factory = function(t, e) {
     var r = !1;
@@ -9479,15 +9492,15 @@
         }).join(" ");
         var n = W(this.tables().nodes());
         return n[e].apply(n, r), this
     })
 });
 It("clear()", function() {
     return this.iterator("table", function(t) {
-        Ci(t)
+        Ti(t)
     })
 });
 It("error()", function(t) {
     return this.iterator("table", function(e) {
         Pe(e, 0, t)
     })
 });
@@ -9526,15 +9539,15 @@
             c = W(n),
             p = W(s),
             b = W(e.nTableWrapper),
             m = e.aoData.map(function(F) {
                 return F ? F.nTr : null
             }),
             y = r.order;
-        e.bDestroying = !0, Zt(e, "aoDestroyCallback", "destroy", [e], !0), t || new Wt(e).columns().visible(!0), b.off(".DT").find(":not(tbody *)").off(".DT"), W(window).off(".DT-" + e.sInstance), n != a.parentNode && (c.children("thead").detach(), c.append(a)), l && n != l.parentNode && (c.children("tfoot").detach(), c.append(l)), e.colgroup.remove(), e.aaSorting = [], e.aaSortingFixed = [], fi(e), W("th, td", a).removeClass(y.canAsc + " " + y.canDesc + " " + y.isAsc + " " + y.isDesc).css("width", ""), p.children().detach(), p.append(m);
+        e.bDestroying = !0, Zt(e, "aoDestroyCallback", "destroy", [e], !0), t || new Wt(e).columns().visible(!0), b.off(".DT").find(":not(tbody *)").off(".DT"), W(window).off(".DT-" + e.sInstance), n != a.parentNode && (c.children("thead").detach(), c.append(a)), l && n != l.parentNode && (c.children("tfoot").detach(), c.append(l)), e.colgroup.remove(), e.aaSorting = [], e.aaSortingFixed = [], hi(e), W("th, td", a).removeClass(y.canAsc + " " + y.canDesc + " " + y.isAsc + " " + y.isDesc).css("width", ""), p.children().detach(), p.append(m);
         var T = e.nTableWrapper.parentNode,
             w = e.nTableWrapper.nextSibling,
             k = t ? "remove" : "detach";
         c[k](), b[k](), !t && T && (T.insertBefore(n, w), c.css("width", e.sDestroyWidth).removeClass(r.table));
         var P = vt.settings.indexOf(e);
         P !== -1 && vt.settings.splice(P, 1)
     })
@@ -9550,15 +9563,15 @@
     })
 });
 It("i18n()", function(t, e, r) {
     var n = this.context[0],
         s = Ir(t)(n.oLanguage);
     return s === void 0 && (s = e), W.isPlainObject(s) && (s = r !== void 0 && s[r] !== void 0 ? s[r] : s._), typeof s == "string" ? s.replace("%d", r) : s
 });
-vt.version = "2.0.5";
+vt.version = "2.0.7";
 vt.settings = [];
 vt.models = {};
 vt.models.oSearch = {
     caseInsensitive: !0,
     search: "",
     regex: !1,
     smart: !0,
@@ -9711,15 +9724,15 @@
     sScrollXInner: "",
     sScrollY: "",
     sServerMethod: "GET",
     renderer: null,
     rowId: "DT_RowId",
     caption: null
 };
-Cn(vt.defaults);
+Tn(vt.defaults);
 vt.defaults.column = {
     aDataSort: null,
     iDataSort: -1,
     ariaTitle: "",
     asSorting: ["asc", "desc", ""],
     bSearchable: !0,
     bSortable: !0,
@@ -9733,15 +9746,15 @@
     sDefaultContent: null,
     sName: "",
     sSortDataType: "std",
     sTitle: null,
     sType: null,
     sWidth: null
 };
-Cn(vt.defaults.column);
+Tn(vt.defaults.column);
 vt.models.oSettings = {
     oFeatures: {
         bAutoWidth: null,
         bDeferRender: null,
         bFilter: null,
         bInfo: !0,
         bLengthChange: !0,
@@ -9853,16 +9866,16 @@
     oPlugins: {},
     rowIdFn: null,
     rowId: null,
     caption: "",
     captionNode: null,
     colgroup: null
 };
-var Tl = vt.ext.pager;
-W.extend(Tl, {
+var kl = vt.ext.pager;
+W.extend(kl, {
     simple: function() {
         return ["previous", "next"]
     },
     full: function() {
         return ["first", "previous", "next", "last"]
     },
     numbers: function() {
@@ -9876,15 +9889,15 @@
     },
     first_last: function() {
         return ["first", "last"]
     },
     first_last_numbers: function() {
         return ["first", "numbers", "last"]
     },
-    _numbers: bs,
+    _numbers: vs,
     numbers_length: 7
 });
 W.extend(!0, vt.ext.renderer, {
     pagingButton: {
         _: function(t, e, r, n, s) {
             var a = t.oClasses.paging,
                 l = [a.button],
@@ -9901,44 +9914,44 @@
     },
     pagingContainer: {
         _: function(t, e) {
             return e
         }
     }
 });
-var Bn = function(t, e) {
+var Nn = function(t, e) {
     return function(r) {
-        return Ze(r) || typeof r != "string" || (r = r.replace(jo, " "), t && (r = hr(r)), e && (r = mn(r, !1))), r
+        return Ke(r) || typeof r != "string" || (r = r.replace(Mo, " "), t && (r = hr(r)), e && (r = gn(r, !1))), r
     }
 };
 
-function cs(t) {
+function fs(t) {
     return t.replace(/[\W]/g, "_")
 }
 
-function La(t, e, r, n, s) {
+function za(t, e, r, n, s) {
     return window.moment ? t[e](s) : window.luxon ? t[r](s) : n ? t[n](s) : t
 }
-var za = !1;
+var ja = !1;
 
-function _n(t, e, r) {
+function Cn(t, e, r) {
     var n;
     if (window.moment) {
         if (n = window.moment.utc(t, e, r, !0), !n.isValid()) return null
     } else if (window.luxon) {
         if (n = e && typeof t == "string" ? window.luxon.DateTime.fromFormat(t, e) : window.luxon.DateTime.fromISO(t), !n.isValid) return null;
         n.setLocale(r)
-    } else e ? (za || alert("DataTables warning: Formatted date without Moment.js or Luxon - https://datatables.net/tn/17"), za = !0) : n = new Date(t);
+    } else e ? (ja || alert("DataTables warning: Formatted date without Moment.js or Luxon - https://datatables.net/tn/17"), ja = !0) : n = new Date(t);
     return n
 }
 
-function oi(t) {
+function li(t) {
     return function(e, r, n, s) {
         arguments.length === 0 ? (n = "en", r = null, e = null) : arguments.length === 1 ? (n = "en", r = e, e = null) : arguments.length === 2 && (n = r, r = e, e = null);
-        var a = "datetime" + (r ? "-" + cs(r) : "");
+        var a = "datetime" + (r ? "-" + fs(r) : "");
         return vt.ext.type.order[a] || vt.type(a, {
                 detect: function(l) {
                     return l === a ? a : !1
                 },
                 order: {
                     pre: function(l) {
                         return l.valueOf()
@@ -9949,51 +9962,51 @@
             function(l, c) {
                 if (l == null)
                     if (s === "--now") {
                         var p = new Date;
                         l = new Date(Date.UTC(p.getFullYear(), p.getMonth(), p.getDate(), p.getHours(), p.getMinutes(), p.getSeconds()))
                     } else l = "";
                 if (c === "type") return a;
-                if (l === "") return c !== "sort" ? "" : _n("0000-01-01 00:00:00", null, n);
+                if (l === "") return c !== "sort" ? "" : Cn("0000-01-01 00:00:00", null, n);
                 if (r !== null && e === r && c !== "sort" && c !== "type" && !(l instanceof Date)) return l;
-                var b = _n(l, e, n);
+                var b = Cn(l, e, n);
                 if (b === null) return l;
                 if (c === "sort") return b;
-                var m = r === null ? La(b, "toDate", "toJSDate", "")[t]() : La(b, "format", "toFormat", "toISOString", r);
+                var m = r === null ? za(b, "toDate", "toJSDate", "")[t]() : za(b, "format", "toFormat", "toISOString", r);
                 return c === "display" ? Dr(m) : m
             }
     }
 }
-var fs = ",",
-    hs = ".";
+var hs = ",",
+    ps = ".";
 if (window.Intl !== void 0) try {
-    for (Sr = new Intl.NumberFormat().formatToParts(100000.1), Ie = 0; Ie < Sr.length; Ie++) Sr[Ie].type === "group" ? fs = Sr[Ie].value : Sr[Ie].type === "decimal" && (hs = Sr[Ie].value)
+    for (Sr = new Intl.NumberFormat().formatToParts(100000.1), Ie = 0; Ie < Sr.length; Ie++) Sr[Ie].type === "group" ? hs = Sr[Ie].value : Sr[Ie].type === "decimal" && (ps = Sr[Ie].value)
 } catch {}
 var Sr, Ie;
 vt.datetime = function(t, e) {
-    var r = "datetime-detect-" + cs(t);
+    var r = "datetime-detect-" + fs(t);
     e || (e = "en"), vt.ext.type.order[r] || vt.type(r, {
         detect: function(n) {
-            var s = _n(n, t, e);
+            var s = Cn(n, t, e);
             return n === "" || s ? r : !1
         },
         order: {
             pre: function(n) {
-                return _n(n, t, e) || 0
+                return Cn(n, t, e) || 0
             }
         },
         className: "dt-right"
     })
 };
 vt.render = {
-    date: oi("toLocaleDateString"),
-    datetime: oi("toLocaleString"),
-    time: oi("toLocaleTimeString"),
+    date: li("toLocaleDateString"),
+    datetime: li("toLocaleString"),
+    time: li("toLocaleTimeString"),
     number: function(t, e, r, n, s) {
-        return t == null && (t = fs), e == null && (e = hs), {
+        return t == null && (t = hs), e == null && (e = ps), {
             display: function(a) {
                 if (typeof a != "number" && typeof a != "string" || a === "" || a === null) return a;
                 var l = a < 0 ? "-" : "",
                     c = parseFloat(a),
                     p = Math.abs(c);
                 if (p >= 1e11 || p < 1e-4 && p !== 0) {
                     var b = c.toExponential(r).split(/e\+?/);
@@ -10057,102 +10070,102 @@
 };
 vt.type("string", {
     detect: function() {
         return "string"
     },
     order: {
         pre: function(t) {
-            return Ze(t) ? "" : typeof t == "string" ? t.toLowerCase() : t.toString ? t.toString() : ""
+            return Ke(t) ? "" : typeof t == "string" ? t.toLowerCase() : t.toString ? t.toString() : ""
         }
     },
-    search: Bn(!1, !0)
+    search: Nn(!1, !0)
 });
 vt.type("html", {
     detect: function(t) {
-        return Ze(t) || typeof t == "string" && t.indexOf("<") !== -1 ? "html" : null
+        return Ke(t) || typeof t == "string" && t.indexOf("<") !== -1 ? "html" : null
     },
     order: {
         pre: function(t) {
-            return Ze(t) ? "" : t.replace ? hr(t).trim().toLowerCase() : t + ""
+            return Ke(t) ? "" : t.replace ? hr(t).trim().toLowerCase() : t + ""
         }
     },
-    search: Bn(!0, !0)
+    search: Nn(!0, !0)
 });
 vt.type("date", {
     className: "dt-type-date",
     detect: function(t) {
-        if (t && !(t instanceof Date) && !Vo.test(t)) return null;
+        if (t && !(t instanceof Date) && !Ho.test(t)) return null;
         var e = Date.parse(t);
-        return e !== null && !isNaN(e) || Ze(t) ? "date" : null
+        return e !== null && !isNaN(e) || Ke(t) ? "date" : null
     },
     order: {
         pre: function(t) {
             var e = Date.parse(t);
             return isNaN(e) ? -1 / 0 : e
         }
     }
 });
 vt.type("html-num-fmt", {
     className: "dt-type-numeric",
     detect: function(t, e) {
         var r = e.oLanguage.sDecimal;
-        return Ha(t, r, !0) ? "html-num-fmt" : null
+        return Wa(t, r, !0) ? "html-num-fmt" : null
     },
     order: {
         pre: function(t, e) {
             var r = e.oLanguage.sDecimal;
-            return Nn(t, r, pi, bi)
+            return En(t, r, bi, vi)
         }
     },
-    search: Bn(!0, !0)
+    search: Nn(!0, !0)
 });
 vt.type("html-num", {
     className: "dt-type-numeric",
     detect: function(t, e) {
         var r = e.oLanguage.sDecimal;
-        return Ha(t, r) ? "html-num" : null
+        return Wa(t, r) ? "html-num" : null
     },
     order: {
         pre: function(t, e) {
             var r = e.oLanguage.sDecimal;
-            return Nn(t, r, pi)
+            return En(t, r, bi)
         }
     },
-    search: Bn(!0, !0)
+    search: Nn(!0, !0)
 });
 vt.type("num-fmt", {
     className: "dt-type-numeric",
     detect: function(t, e) {
         var r = e.oLanguage.sDecimal;
-        return vi(t, r, !0) ? "num-fmt" : null
+        return mi(t, r, !0) ? "num-fmt" : null
     },
     order: {
         pre: function(t, e) {
             var r = e.oLanguage.sDecimal;
-            return Nn(t, r, bi)
+            return En(t, r, vi)
         }
     }
 });
 vt.type("num", {
     className: "dt-type-numeric",
     detect: function(t, e) {
         var r = e.oLanguage.sDecimal;
-        return vi(t, r) ? "num" : null
+        return mi(t, r) ? "num" : null
     },
     order: {
         pre: function(t, e) {
             var r = e.oLanguage.sDecimal;
-            return Nn(t, r)
+            return En(t, r)
         }
     }
 });
-var Nn = function(t, e, r, n) {
+var En = function(t, e, r, n) {
     if (t !== 0 && (!t || t === "-")) return -1 / 0;
     var s = typeof t;
-    return s === "number" || s === "bigint" ? t : (e && (t = Va(t, e)), t.replace && (r && (t = t.replace(r, "")), n && (t = t.replace(n, ""))), t * 1)
+    return s === "number" || s === "bigint" ? t : (e && (t = Ha(t, e)), t.replace && (r && (t = t.replace(r, "")), n && (t = t.replace(n, ""))), t * 1)
 };
 W.extend(!0, vt.ext.renderer, {
     footer: {
         _: function(t, e, r) {
             e.addClass(r.tfoot.cell)
         }
     },
@@ -10220,49 +10233,49 @@
     return e = W.extend({
         callback: r.fnInfoCallback,
         empty: r.sInfoEmpty,
         postfix: r.sInfoPostFix,
         search: r.sInfoFiltered,
         text: r.sInfo
     }, e), t.aoDrawCallback.push(function(a) {
-        kl(a, e, s)
+        Sl(a, e, s)
     }), t._infoEl || (s.attr({
         "aria-live": "polite",
         id: n + "_info",
         role: "status"
     }), W(t.nTable).attr("aria-describedby", n + "_info"), t._infoEl = s), s
 }, "i");
 
-function kl(t, e, r) {
+function Sl(t, e, r) {
     var n = t._iDisplayStart + 1,
         s = t.fnDisplayEnd(),
         a = t.fnRecordsTotal(),
         l = t.fnRecordsDisplay(),
         c = l ? e.text : e.empty;
-    l !== a && (c += " " + e.search), c += e.postfix, c = Ai(t, c), e.callback && (c = e.callback.call(t.oInstance, t, n, s, a, l, c)), r.html(c), Zt(t, null, "info", [t, r[0], c])
+    l !== a && (c += " " + e.search), c += e.postfix, c = Ii(t, c), e.callback && (c = e.callback.call(t.oInstance, t, n, s, a, l, c)), r.html(c), Zt(t, null, "info", [t, r[0], c])
 }
-var li = 0;
+var di = 0;
 vt.feature.register("search", function(t, e) {
     if (!t.oFeatures.bFilter) return null;
     var r = t.oClasses.search,
         n = t.sTableId,
         s = t.oLanguage,
         a = t.oPreviousSearch,
         l = '<input type="search" class="' + r.input + '"/>';
     e = W.extend({
         placeholder: s.sSearchPlaceholder,
         text: s.sSearch
-    }, e), e.text.indexOf("_INPUT_") === -1 && (e.text += "_INPUT_"), e.text = Ai(t, e.text);
+    }, e), e.text.indexOf("_INPUT_") === -1 && (e.text += "_INPUT_"), e.text = Ii(t, e.text);
     var c = e.text.match(/_INPUT_$/),
         p = e.text.match(/^_INPUT_/),
         b = e.text.replace(/_INPUT_/, ""),
         m = "<label>" + e.text + "</label>";
     p ? m = "_INPUT_<label>" + b + "</label>" : c && (m = "<label>" + b + "</label>_INPUT_");
     var y = W("<div>").addClass(r.container).append(m.replace(/_INPUT_/, l));
-    y.find("label").attr("for", "dt-search-" + li), y.find("input").attr("id", "dt-search-" + li), li++;
+    y.find("label").attr("for", "dt-search-" + di), y.find("input").attr("id", "dt-search-" + di), di++;
     var T = function(P) {
             var F = this.value;
             a.return && P.key !== "Enter" || F != a.search && (a.search = F, Gr(t, a), t._iDisplayStart = 0, Fr(t))
         },
         w = t.searchDelay !== null ? t.searchDelay : 0,
         k = W("input", y).val(a.search).attr("placeholder", e.placeholder).on("keyup.DT search.DT input.DT paste.DT cut.DT", w ? vt.util.debounce(T, w) : T).on("mouseup.DT", function(P) {
             setTimeout(function() {
@@ -10280,49 +10293,49 @@
     e = W.extend({
         buttons: vt.ext.pager.numbers_length,
         type: t.sPaginationType,
         boundaryNumbers: !0
     }, e), e.numbers && (e.buttons = e.numbers);
     var r = W("<div/>").addClass(t.oClasses.paging.container + " paging_" + e.type),
         n = function() {
-            ps(t, r, e)
+            bs(t, r, e)
         };
     return t.aoDrawCallback.push(n), W(t.nTable).on("column-sizing.dt.DT", n), r
 }, "p");
 
-function ps(t, e, r) {
+function bs(t, e, r) {
     if (t._bInitComplete) {
         for (var n = vt.ext.pager[r.type], s = t.oLanguage.oAria.paginate || {}, a = t._iDisplayStart, l = t._iDisplayLength, c = t.fnRecordsDisplay(), p = l === -1, b = p ? 0 : Math.ceil(a / l), m = p ? 1 : Math.ceil(c / l), y = n().map(function(f) {
-                return f === "numbers" ? bs(b, m, r.buttons, r.boundaryNumbers) : f
+                return f === "numbers" ? vs(b, m, r.buttons, r.boundaryNumbers) : f
             }).flat(), T = [], w = 0; w < y.length; w++) {
             var k = y[w],
-                P = Sl(t, k, b, m),
-                F = xn(t, "pagingButton")(t, k, P.display, P.active, P.disabled);
+                P = Dl(t, k, b, m),
+                F = _n(t, "pagingButton")(t, k, P.display, P.active, P.disabled);
             W(F.clicker).attr({
                 "aria-controls": t.sTableId,
                 "aria-disabled": P.disabled ? "true" : null,
                 "aria-current": P.active ? "page" : null,
                 "aria-label": s[k],
                 "data-dt-idx": k,
                 tabIndex: P.disabled ? -1 : t.iTabIndex
-            }), typeof k != "number" && W(F.clicker).addClass(k), is(F.clicker, {
+            }), typeof k != "number" && W(F.clicker).addClass(k), as(F.clicker, {
                 action: k
             }, function(f) {
-                f.preventDefault(), Si(t, f.data.action, !0)
+                f.preventDefault(), Di(t, f.data.action, !0)
             }), T.push(F.display)
         }
-        var h = xn(t, "pagingContainer")(t, T),
+        var h = _n(t, "pagingContainer")(t, T),
             o = e.find(document.activeElement).data("dt-idx");
-        e.empty().append(h), o !== void 0 && e.find("[data-dt-idx=" + o + "]").trigger("focus"), T.length && r.numbers > 1 && W(e).height() >= W(T[0]).outerHeight() * 2 - 10 && ps(t, e, W.extend({}, r, {
+        e.empty().append(h), o !== void 0 && e.find("[data-dt-idx=" + o + "]").trigger("focus"), T.length && r.numbers > 1 && W(e).height() >= W(T[0]).outerHeight() * 2 - 10 && bs(t, e, W.extend({}, r, {
             numbers: r.numbers - 2
         }))
     }
 }
 
-function Sl(t, e, r, n) {
+function Dl(t, e, r, n) {
     var s = t.oLanguage.oPaginate,
         a = {
             display: "",
             active: !1,
             disabled: !1
         };
     switch (e) {
@@ -10344,22 +10357,22 @@
         default:
             typeof e == "number" && (a.display = t.fnFormatNumber(e + 1), r === e && (a.active = !0));
             break
     }
     return a
 }
 
-function bs(t, e, r, n) {
+function vs(t, e, r, n) {
     var s = [],
         a = Math.floor(r / 2),
         l = n ? 2 : 1,
         c = n ? 1 : 0;
     return e <= r ? s = cr(0, e) : r === 1 ? s = [t] : r === 3 ? t <= 1 ? s = [0, 1, "ellipsis"] : t >= e - 2 ? (s = cr(e - 2, e), s.unshift("ellipsis")) : s = ["ellipsis", t, "ellipsis"] : t <= a ? (s = cr(0, r - l), s.push("ellipsis"), n && s.push(e - 1)) : t >= e - 1 - a ? (s = cr(e - (r - l), e), s.unshift("ellipsis"), n && s.unshift(0)) : (s = cr(t - a + l, t + a - c), s.push("ellipsis"), s.unshift("ellipsis"), n && (s.push(e - 1), s.unshift(0))), s
 }
-var di = 0;
+var ui = 0;
 vt.feature.register("pageLength", function(t, e) {
     var r = t.oFeatures;
     if (!r.bPaginate || !r.bLengthChange) return null;
     e = W.extend({
         menu: t.aLengthMenu,
         text: t.oLanguage.sLengthMenu
     }, e);
@@ -10383,25 +10396,25 @@
         h.nodeType === Node.TEXT_NODE && k.push({
             el: h,
             text: h.textContent
         })
     });
     var P = function(h) {
             k.forEach(function(o) {
-                o.el.textContent = Ai(t, o.text, h)
+                o.el.textContent = Ii(t, o.text, h)
             })
         },
         F = W("<select/>", {
             name: s + "_length",
             "aria-controls": s,
             class: n.select
         });
     for (p = 0; p < l.length; p++) F[0][p] = new Option(typeof c[p] == "number" ? t.fnFormatNumber(c[p]) : c[p], l[p]);
-    return w.find("label").attr("for", "dt-length-" + di), F.attr("id", "dt-length-" + di), di++, w.find("span").replaceWith(F), W("select", w).val(t._iDisplayLength).on("change.DT", function() {
-        Qa(t, W(this).val()), Fr(t)
+    return w.find("label").attr("for", "dt-length-" + ui), F.attr("id", "dt-length-" + ui), ui++, w.find("span").replaceWith(F), W("select", w).val(t._iDisplayLength).on("change.DT", function() {
+        Ja(t, W(this).val()), Fr(t)
     }), W(t.nTable).on("length.dt.DT", function(h, o, f) {
         t === o && (W("select", w).val(f), P(f))
     }), P(t._iDisplayLength), w
 }, "l");
 W.fn.dataTable = vt;
 vt.$ = W;
 W.fn.dataTableSettings = vt.settings;
@@ -10409,42 +10422,42 @@
 W.fn.DataTable = function(t) {
     return W(this).dataTable(t).api()
 };
 W.each(vt, function(t, e) {
     W.fn.DataTable[t] = e
 });
 var st = vt;
-var Ke = st;
-var Nl = ne(ie(), 1);
-var ys = ne(ie(), 1);
-var ht = ys.default,
-    Al = 0,
+var qe = st;
+var El = ne(ie(), 1);
+var ws = ne(ie(), 1);
+var ht = ws.default,
     Il = 0,
+    Pl = 0,
     _e = st.ext.buttons,
-    Oi = null;
+    Ri = null;
 
-function Ri(t, e, r) {
+function Li(t, e, r) {
     ht.fn.animate ? t.stop().fadeIn(e, r) : (t.css("display", "block"), r && r.call(t))
 }
 
-function Li(t, e, r) {
+function zi(t, e, r) {
     ht.fn.animate ? t.stop().fadeOut(e, r) : (t.css("display", "none"), r && r.call(t))
 }
 var Jt = function(t, e) {
     if (!st.versionCheck("2")) throw "Warning: Buttons requires DataTables 2 or newer";
     if (!(this instanceof Jt)) return function(r) {
         return new Jt(r, t).container()
     };
     typeof e > "u" && (e = {}), e === !0 && (e = {}), Array.isArray(e) && (e = {
         buttons: e
     }), this.c = ht.extend(!0, {}, Jt.defaults, e), e.buttons && (this.c.buttons = e.buttons), this.s = {
         dt: new st.Api(t),
         buttons: [],
         listenKeys: "",
-        namespace: "dtb" + Al++
+        namespace: "dtb" + Il++
     }, this.dom = {
         container: ht("<" + this.c.dom.container.tag + "/>").addClass(this.c.dom.container.className)
     }, this._constructor()
 };
 ht.extend(Jt.prototype, {
     action: function(t, e) {
         var r = this._nodeToButton(t);
@@ -10641,15 +10654,15 @@
                     et.preventDefault(), !y.hasClass(b.disabled) && t.action && w(et, c, y, t), P && y.trigger("blur")
                 }).on("keypress.dtb", function(et) {
                     et.keyCode === 13 && (et.preventDefault(), !y.hasClass(b.disabled) && t.action && w(et, c, y, t))
                 }), k.toLowerCase() === "a" && y.attr("href", "#"), k.toLowerCase() === "button" && y.attr("type", "button"), b.liner.tag) {
                 var F = ht("<" + b.liner.tag + "/>").html(p(t.text)).addClass(b.liner.className);
                 b.liner.tag.toLowerCase() === "a" && F.attr("href", "#"), y.append(F), l = F
             } else y.html(p(t.text)), l = y;
-            t.enabled === !1 && y.addClass(b.disabled), t.className && y.addClass(t.className), t.titleAttr && y.attr("title", p(t.titleAttr)), t.attr && y.attr(t.attr), t.namespace || (t.namespace = ".dt-button-" + Il++), t.config !== void 0 && t.config.split && (t.split = t.config.split)
+            t.enabled === !1 && y.addClass(b.disabled), t.className && y.addClass(t.className), t.titleAttr && y.attr("title", p(t.titleAttr)), t.attr && y.attr(t.attr), t.namespace || (t.namespace = ".dt-button-" + Pl++), t.config !== void 0 && t.config.split && (t.split = t.config.split)
         }
         var h = this.c.dom.buttonContainer,
             o;
         h && h.tag ? o = ht("<" + h.tag + "/>").addClass(h.className).append(y) : o = y, this._addKey(t), this.c.buttonCreated && (o = this.c.buttonCreated(t, o));
         var f;
         if (r) {
             var C = e ? ht.extend(!0, this.c.dom.split, this.c.dom.collection.split) : this.c.dom.split,
@@ -10787,15 +10800,15 @@
                 popoverTitle: "",
                 rightAlignClassName: "dt-button-right",
                 tag: s.dom.collection.container.tag
             }, r),
             c = l.tag + "." + l.containerClassName.replace(/ /g, "."),
             p = e.node(),
             b = function() {
-                a = !0, Li(ht(c), l.fade, function() {
+                a = !0, zi(ht(c), l.fade, function() {
                     ht(this).detach()
                 }), ht(n.buttons('[aria-haspopup="dialog"][aria-expanded="true"]').nodes()).attr("aria-expanded", "false"), ht("div.dt-button-background").off("click.dtb-collection"), Jt.background(!1, l.backgroundClassName, l.fade, p), ht(window).off("resize.resize.dtb-collection"), ht("body").off(".dtb-collection"), n.off("buttons-action.b-internal"), n.off("destroy")
             };
         if (t === !1) {
             b();
             return
         }
@@ -10804,15 +10817,15 @@
         var y = ht(".dt-button", t).length,
             T = "";
         y === 3 ? T = "dtb-b3" : y === 2 ? T = "dtb-b2" : y === 1 && (T = "dtb-b1");
         var w = ht("<" + l.tag + "/>").addClass(l.containerClassName).addClass(l.collectionLayout).addClass(l.splitAlignClass).addClass(T).css("display", "none").attr({
             "aria-modal": !0,
             role: "dialog"
         });
-        t = ht(t).addClass(l.contentClassName).attr("role", "menu").appendTo(w), p.attr("aria-expanded", "true"), p.parents("body")[0] !== document.body && (p = document.body.lastChild), l.popoverTitle ? w.prepend('<div class="dt-button-collection-title">' + l.popoverTitle + "</div>") : l.collectionTitle && w.prepend('<div class="dt-button-collection-title">' + l.collectionTitle + "</div>"), l.closeButton && w.prepend('<div class="dtb-popover-close">&times;</div>').addClass("dtb-collection-closeable"), Ri(w.insertAfter(p), l.fade);
+        t = ht(t).addClass(l.contentClassName).attr("role", "menu").appendTo(w), p.attr("aria-expanded", "true"), p.parents("body")[0] !== document.body && (p = document.body.lastChild), l.popoverTitle ? w.prepend('<div class="dt-button-collection-title">' + l.popoverTitle + "</div>") : l.collectionTitle && w.prepend('<div class="dt-button-collection-title">' + l.collectionTitle + "</div>"), l.closeButton && w.prepend('<div class="dtb-popover-close">&times;</div>').addClass("dtb-collection-closeable"), Li(w.insertAfter(p), l.fade);
         var k = ht(e.table().container()),
             P = w.css("position");
         if ((l.span === "container" || l.align === "dt-container") && (p = p.parent(), w.css("width", k.width())), P === "absolute") {
             var F = ht(p[0].offsetParent),
                 h = p.position(),
                 o = p.offset(),
                 f = F.offset(),
@@ -10858,15 +10871,15 @@
                     g = document.activeElement;
                 O.keyCode === 9 && (Z.index(g) === -1 ? (Z.first().focus(), O.preventDefault()) : O.shiftKey ? g === Z[0] && (Z.last().focus(), O.preventDefault()) : g === Z.last()[0] && (Z.first().focus(), O.preventDefault()))
             })
         }, 0)
     }
 });
 Jt.background = function(t, e, r, n) {
-    r === void 0 && (r = 400), n || (n = document.body), t ? Ri(ht("<div/>").addClass(e).css("display", "none").insertAfter(n), r) : Li(ht("div." + e), r, function() {
+    r === void 0 && (r = 400), n || (n = document.body), t ? Li(ht("<div/>").addClass(e).css("display", "none").insertAfter(n), r) : zi(ht("div." + e), r, function() {
         ht(this).removeClass(e).remove()
     })
 };
 Jt.instanceSelector = function(t, e) {
     if (t == null) return ht.map(e, function(a) {
         return a.inst
     });
@@ -10952,18 +10965,18 @@
         }, a = 0, l = t.length; a < l; a++) {
         var c = t[a];
         s(e, c)
     }
     return r
 };
 Jt.stripData = function(t, e) {
-    return typeof t != "string" || (t = Jt.stripHtmlScript(t), t = Jt.stripHtmlComments(t), (!e || e.stripHtml) && (t = st.util.stripHtml(t)), (!e || e.trim) && (t = t.trim()), (!e || e.stripNewlines) && (t = t.replace(/\n/g, " ")), (!e || e.decodeEntities) && (Oi ? t = Oi(t) : (ms.innerHTML = t, t = ms.value))), t
+    return typeof t != "string" || (t = Jt.stripHtmlScript(t), t = Jt.stripHtmlComments(t), (!e || e.stripHtml) && (t = st.util.stripHtml(t)), (!e || e.trim) && (t = t.trim()), (!e || e.stripNewlines) && (t = t.replace(/\n/g, " ")), (!e || e.decodeEntities) && (Ri ? t = Ri(t) : (gs.innerHTML = t, t = gs.value))), t
 };
 Jt.entityDecoder = function(t) {
-    Oi = t
+    Ri = t
 };
 Jt.stripHtmlComments = function(t) {
     var e;
     do e = t, t = t.replace(/(<!--.*?--!?>)|(<!--[\S\s]+?--!?>)|(<!--[\S\s]*?$)/g, ""); while (t !== e);
     return t
 };
 Jt.stripHtmlScript = function(t) {
@@ -11237,59 +11250,59 @@
     return this.each(function(t) {
         t.inst.remove(t.node)
     }), this
 });
 var Kr;
 st.Api.register("buttons.info()", function(t, e, r) {
     var n = this;
-    return t === !1 ? (this.off("destroy.btn-info"), Li(ht("#datatables_buttons_info"), 400, function() {
+    return t === !1 ? (this.off("destroy.btn-info"), zi(ht("#datatables_buttons_info"), 400, function() {
         ht(this).remove()
-    }), clearTimeout(Kr), Kr = null, this) : (Kr && clearTimeout(Kr), ht("#datatables_buttons_info").length && ht("#datatables_buttons_info").remove(), t = t ? "<h2>" + t + "</h2>" : "", Ri(ht('<div id="datatables_buttons_info" class="dt-button-info"/>').html(t).append(ht("<div/>")[typeof e == "string" ? "html" : "append"](e)).css("display", "none").appendTo("body")), r !== void 0 && r !== 0 && (Kr = setTimeout(function() {
+    }), clearTimeout(Kr), Kr = null, this) : (Kr && clearTimeout(Kr), ht("#datatables_buttons_info").length && ht("#datatables_buttons_info").remove(), t = t ? "<h2>" + t + "</h2>" : "", Li(ht('<div id="datatables_buttons_info" class="dt-button-info"/>').html(t).append(ht("<div/>")[typeof e == "string" ? "html" : "append"](e)).css("display", "none").appendTo("body")), r !== void 0 && r !== 0 && (Kr = setTimeout(function() {
         n.buttons.info(!1)
     }, r)), this.on("destroy.btn-info", function() {
         n.buttons.info(!1)
     }), this)
 });
 st.Api.register("buttons.exportData()", function(t) {
-    if (this.context.length) return Bl(new st.Api(this.context[0]), t)
+    if (this.context.length) return Nl(new st.Api(this.context[0]), t)
 });
 st.Api.register("buttons.exportInfo()", function(t) {
     return t || (t = {}), {
-        filename: Pl(t, this),
-        title: Fl(t, this),
-        messageTop: vs(this, t, t.message || t.messageTop, "top"),
-        messageBottom: vs(this, t, t.messageBottom, "bottom")
+        filename: Fl(t, this),
+        title: Bl(t, this),
+        messageTop: ms(this, t, t.message || t.messageTop, "top"),
+        messageBottom: ms(this, t, t.messageBottom, "bottom")
     }
 });
-var Pl = function(t, e) {
+var Fl = function(t, e) {
         var r = t.filename === "*" && t.title !== "*" && t.title !== void 0 && t.title !== null && t.title !== "" ? t.title : t.filename;
         if (typeof r == "function" && (r = r(t, e)), r == null) return null;
         r.indexOf("*") !== -1 && (r = r.replace(/\*/g, ht("head > title").text()).trim()), r = r.replace(/[^a-zA-Z0-9_\u00A1-\uFFFF\.,\-_ !\(\)]/g, "");
-        var n = zi(t.extension, t, e);
+        var n = ji(t.extension, t, e);
         return n || (n = ""), r + n
     },
-    zi = function(t, e, r) {
+    ji = function(t, e, r) {
         return t == null ? null : typeof t == "function" ? t(e, r) : t
     },
-    Fl = function(t, e) {
-        var r = zi(t.title, t, e);
+    Bl = function(t, e) {
+        var r = ji(t.title, t, e);
         return r === null ? null : r.indexOf("*") !== -1 ? r.replace(/\*/g, ht("head > title").text() || "Exported data") : r
     },
-    vs = function(t, e, r, n) {
-        var s = zi(r, e, t);
+    ms = function(t, e, r, n) {
+        var s = ji(r, e, t);
         if (s === null) return null;
         var a = ht("caption", t.table().container()).eq(0);
         if (s === "*") {
             var l = a.css("caption-side");
             return l !== n ? null : a.length ? a.text() : ""
         }
         return s
     },
-    ms = ht("<textarea/>")[0],
-    Bl = function(t, e) {
+    gs = ht("<textarea/>")[0],
+    Nl = function(t, e) {
         var r = ht.extend(!0, {}, {
                 rows: null,
                 columns: "",
                 modifier: {
                     search: "applied",
                     order: "applied"
                 },
@@ -11335,23 +11348,23 @@
                 order: a.order
             }), p = c.render(r.orthogonal).toArray(), b = c.nodes().toArray(), m = c.indexes().toArray(), y = t.columns(r.columns).count(), T = y > 0 ? p.length / y : 0, w = [], k = 0, P = 0, F = T; P < F; P++) {
             for (var h = [y], o = 0; o < y; o++) h[o] = r.format.body(p[k], m[k].row, m[k].column, b[k]), k++;
             w[P] = h
         }
         var f = {
             header: n,
-            headerStructure: gs(r.format.header, t.table().header.structure(r.columns)),
+            headerStructure: ys(r.format.header, t.table().header.structure(r.columns)),
             footer: s,
-            footerStructure: gs(r.format.footer, t.table().footer.structure(r.columns)),
+            footerStructure: ys(r.format.footer, t.table().footer.structure(r.columns)),
             body: w
         };
         return r.customizeData && r.customizeData(f), f
     };
 
-function gs(t, e) {
+function ys(t, e) {
     for (var r = 0; r < e.length; r++)
         for (var n = 0; n < e[r].length; n++) {
             var s = e[r][n];
             s && (s.title = t(s.title, n, s.cell))
         }
     return e
 }
@@ -11360,44 +11373,44 @@
 ht(document).on("init.dt plugin-init.dt", function(t, e) {
     if (t.namespace === "dt") {
         var r = e.oInit.buttons || st.defaults.buttons;
         r && !e._buttons && new Jt(e, r).container()
     }
 });
 
-function ws(t, e) {
+function xs(t, e) {
     var r = new st.Api(t),
         n = e || r.init().buttons || st.defaults.buttons;
     return new Jt(r, n).container()
 }
 st.ext.feature.push({
-    fnInit: ws,
+    fnInit: xs,
     cFeature: "B"
 });
-st.feature && st.feature.register("buttons", ws);
-var Cs = ne(ie(), 1);
-var ae = Cs.default,
-    Ts, ks;
+st.feature && st.feature.register("buttons", xs);
+var Ts = ne(ie(), 1);
+var ae = Ts.default,
+    ks, Ss;
 
-function ji() {
-    return Ts || window.JSZip
+function Mi() {
+    return ks || window.JSZip
 }
 
-function Mi() {
-    return ks || window.pdfMake
+function Vi() {
+    return Ss || window.pdfMake
 }
 st.Buttons.pdfMake = function(t) {
-    if (!t) return Mi();
-    ks = t
+    if (!t) return Vi();
+    Ss = t
 };
 st.Buttons.jszip = function(t) {
-    if (!t) return ji();
-    Ts = t
+    if (!t) return Mi();
+    ks = t
 };
-var On = function(t) {
+var Rn = function(t) {
     "use strict";
     if (!(typeof t > "u" || typeof navigator < "u" && /MSIE [1-9]\./.test(navigator.userAgent))) {
         var e = t.document,
             r = function() {
                 return t.URL || t.webkitURL || t
             },
             n = e.createElementNS("http://www.w3.org/1999/xhtml", "a"),
@@ -11475,26 +11488,26 @@
                 return new k(h, o || h.name || "download", f)
             };
         return typeof navigator < "u" && navigator.msSaveOrOpenBlob ? function(h, o, f) {
             return o = o || h.name || "download", f || (h = w(h)), navigator.msSaveOrOpenBlob(h, o)
         } : (P.abort = function() {}, P.readyState = P.INIT = 0, P.WRITING = 1, P.DONE = 2, P.error = P.onwritestart = P.onprogress = P.onwrite = P.onabort = P.onerror = P.onwriteend = null, F)
     }
 }(typeof self < "u" && self || typeof window < "u" && window || (void 0).content);
-st.fileSave = On;
-var xs = function(t) {
+st.fileSave = Rn;
+var _s = function(t) {
         var e = "Sheet1";
         return t.sheetName && (e = t.sheetName.replace(/[\[\]\*\/\\\?\:]/g, "")), e
     },
-    Ss = function(t) {
+    Ds = function(t) {
         return t.newline ? t.newline : navigator.userAgent.match(/Windows/) ? `\r
 ` : `
 `
     },
-    Ds = function(t, e) {
-        var r = Ss(e),
+    As = function(t, e) {
+        var r = Ds(e),
             n = t.buttons.exportData(e.exportOptions),
             s = e.fieldBoundary,
             a = e.fieldSeparator,
             l = new RegExp(s, "g"),
             c = e.escapeChar !== void 0 ? e.escapeChar : "\\",
             p = function(k) {
                 for (var P = "", F = 0, h = k.length; F < h; F++) F > 0 && (P += a), P += s ? s + ("" + k[F]).replace(l, c + s) + s : k[F];
@@ -11514,35 +11527,35 @@
         }).join(r) + r);
         for (var T = 0, w = n.body.length; T < w; T++) y.push(p(n.body[T]));
         return {
             str: b + y.join(r) + r + m,
             rows: y.length
         }
     },
-    As = function() {
+    Is = function() {
         var t = navigator.userAgent.indexOf("Safari") !== -1 && navigator.userAgent.indexOf("Chrome") === -1 && navigator.userAgent.indexOf("Opera") === -1;
         if (!t) return !1;
         var e = navigator.userAgent.match(/AppleWebKit\/(\d+\.\d+)/);
         return !!(e && e.length > 1 && e[1] * 1 < 603.1)
     };
 
 function Qr(t) {
     for (var e = 65, r = 90, n = r - e + 1, s = ""; t >= 0;) s = String.fromCharCode(t % n + e) + s, t = Math.floor(t / n) - 1;
     return s
 }
 try {
-    Rn = new XMLSerializer
+    Ln = new XMLSerializer
 } catch {}
-var Rn, Yr;
+var Ln, Yr;
 
-function Is(t, e) {
-    Yr === void 0 && (Yr = Rn.serializeToString(new window.DOMParser().parseFromString(Ps["xl/worksheets/sheet1.xml"], "text/xml")).indexOf("xmlns:r") === -1), ae.each(e, function(r, n) {
+function Ps(t, e) {
+    Yr === void 0 && (Yr = Ln.serializeToString(new window.DOMParser().parseFromString(Fs["xl/worksheets/sheet1.xml"], "text/xml")).indexOf("xmlns:r") === -1), ae.each(e, function(r, n) {
         if (ae.isPlainObject(n)) {
             var s = t.folder(r);
-            Is(s, n)
+            Ps(s, n)
         } else {
             if (Yr) {
                 var a = n.childNodes[0],
                     l, c, p = [];
                 for (l = a.attributes.length - 1; l >= 0; l--) {
                     var b = a.attributes[l].nodeName,
                         m = a.attributes[l].nodeValue;
@@ -11552,50 +11565,50 @@
                     }), a.removeAttribute(b))
                 }
                 for (l = 0, c = p.length; l < c; l++) {
                     var y = n.createAttribute(p[l].name.replace(":", "_dt_b_namespace_token_"));
                     y.value = p[l].value, a.setAttributeNode(y)
                 }
             }
-            var T = Rn.serializeToString(n);
+            var T = Ln.serializeToString(n);
             Yr && (T.indexOf("<?xml") === -1 && (T = '<?xml version="1.0" encoding="UTF-8" standalone="yes"?>' + T), T = T.replace(/_dt_b_namespace_token_/g, ":"), T = T.replace(/xmlns:NS[\d]+="" NS[\d]+:/g, "")), T = T.replace(/<([^<>]*?) xmlns=""([^<>]*?)>/g, "<$1 $2>"), t.file(r, T)
         }
     })
 }
 
 function Ce(t, e, r) {
     var n = t.createElement(e);
     return r && (r.attr && ae(n).attr(r.attr), r.children && ae.each(r.children, function(s, a) {
         n.appendChild(a)
     }), r.text !== null && r.text !== void 0 && n.appendChild(t.createTextNode(r.text))), n
 }
 
-function El(t, e) {
+function Ol(t, e) {
     var r = t.header[e].length,
         n, s, a;
     t.footer && t.footer[e] && t.footer[e].length > r && (r = t.footer[e].length);
     for (var l = 0, c = t.body.length; l < c; l++) {
         var p = t.body[l][e];
         if (a = p != null ? p.toString() : "", a.indexOf(`
 `) !== -1 ? (s = a.split(`
 `), s.sort(function(b, m) {
                 return m.length - b.length
             }), n = s[0].length) : n = a.length, n > r && (r = n), r > 40) return 54
     }
     return r *= 1.35, r > 6 ? r : 6
 }
-var Ps = {
+var Fs = {
         "_rels/.rels": '<?xml version="1.0" encoding="UTF-8" standalone="yes"?><Relationships xmlns="http://schemas.openxmlformats.org/package/2006/relationships"><Relationship Id="rId1" Type="http://schemas.openxmlformats.org/officeDocument/2006/relationships/officeDocument" Target="xl/workbook.xml"/></Relationships>',
         "xl/_rels/workbook.xml.rels": '<?xml version="1.0" encoding="UTF-8" standalone="yes"?><Relationships xmlns="http://schemas.openxmlformats.org/package/2006/relationships"><Relationship Id="rId1" Type="http://schemas.openxmlformats.org/officeDocument/2006/relationships/worksheet" Target="worksheets/sheet1.xml"/><Relationship Id="rId2" Type="http://schemas.openxmlformats.org/officeDocument/2006/relationships/styles" Target="styles.xml"/></Relationships>',
         "[Content_Types].xml": '<?xml version="1.0" encoding="UTF-8" standalone="yes"?><Types xmlns="http://schemas.openxmlformats.org/package/2006/content-types"><Default Extension="xml" ContentType="application/xml" /><Default Extension="rels" ContentType="application/vnd.openxmlformats-package.relationships+xml" /><Default Extension="jpeg" ContentType="image/jpeg" /><Override PartName="/xl/workbook.xml" ContentType="application/vnd.openxmlformats-officedocument.spreadsheetml.sheet.main+xml" /><Override PartName="/xl/worksheets/sheet1.xml" ContentType="application/vnd.openxmlformats-officedocument.spreadsheetml.worksheet+xml" /><Override PartName="/xl/styles.xml" ContentType="application/vnd.openxmlformats-officedocument.spreadsheetml.styles+xml" /></Types>',
         "xl/workbook.xml": '<?xml version="1.0" encoding="UTF-8" standalone="yes"?><workbook xmlns="http://schemas.openxmlformats.org/spreadsheetml/2006/main" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships"><fileVersion appName="xl" lastEdited="5" lowestEdited="5" rupBuild="24816"/><workbookPr showInkAnnotation="0" autoCompressPictures="0"/><bookViews><workbookView xWindow="0" yWindow="0" windowWidth="25600" windowHeight="19020" tabRatio="500"/></bookViews><sheets><sheet name="Sheet1" sheetId="1" r:id="rId1"/></sheets><definedNames/></workbook>',
         "xl/worksheets/sheet1.xml": '<?xml version="1.0" encoding="UTF-8" standalone="yes"?><worksheet xmlns="http://schemas.openxmlformats.org/spreadsheetml/2006/main" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" mc:Ignorable="x14ac" xmlns:x14ac="http://schemas.microsoft.com/office/spreadsheetml/2009/9/ac"><sheetData/><mergeCells count="0"/></worksheet>',
         "xl/styles.xml": '<?xml version="1.0" encoding="UTF-8"?><styleSheet xmlns="http://schemas.openxmlformats.org/spreadsheetml/2006/main" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" mc:Ignorable="x14ac" xmlns:x14ac="http://schemas.microsoft.com/office/spreadsheetml/2009/9/ac"><numFmts count="6"><numFmt numFmtId="164" formatCode="[$$-409]#,##0.00;-[$$-409]#,##0.00"/><numFmt numFmtId="165" formatCode="&quot;\xA3&quot;#,##0.00"/><numFmt numFmtId="166" formatCode="[$\u20AC-2] #,##0.00"/><numFmt numFmtId="167" formatCode="0.0%"/><numFmt numFmtId="168" formatCode="#,##0;(#,##0)"/><numFmt numFmtId="169" formatCode="#,##0.00;(#,##0.00)"/></numFmts><fonts count="5" x14ac:knownFonts="1"><font><sz val="11" /><name val="Calibri" /></font><font><sz val="11" /><name val="Calibri" /><color rgb="FFFFFFFF" /></font><font><sz val="11" /><name val="Calibri" /><b /></font><font><sz val="11" /><name val="Calibri" /><i /></font><font><sz val="11" /><name val="Calibri" /><u /></font></fonts><fills count="6"><fill><patternFill patternType="none" /></fill><fill><patternFill patternType="none" /></fill><fill><patternFill patternType="solid"><fgColor rgb="FFD9D9D9" /><bgColor indexed="64" /></patternFill></fill><fill><patternFill patternType="solid"><fgColor rgb="FFD99795" /><bgColor indexed="64" /></patternFill></fill><fill><patternFill patternType="solid"><fgColor rgb="ffc6efce" /><bgColor indexed="64" /></patternFill></fill><fill><patternFill patternType="solid"><fgColor rgb="ffc6cfef" /><bgColor indexed="64" /></patternFill></fill></fills><borders count="2"><border><left /><right /><top /><bottom /><diagonal /></border><border diagonalUp="false" diagonalDown="false"><left style="thin"><color auto="1" /></left><right style="thin"><color auto="1" /></right><top style="thin"><color auto="1" /></top><bottom style="thin"><color auto="1" /></bottom><diagonal /></border></borders><cellStyleXfs count="1"><xf numFmtId="0" fontId="0" fillId="0" borderId="0" /></cellStyleXfs><cellXfs count="68"><xf numFmtId="0" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="1" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="2" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="3" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="4" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="0" fillId="2" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="1" fillId="2" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="2" fillId="2" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="3" fillId="2" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="4" fillId="2" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="0" fillId="3" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="1" fillId="3" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="2" fillId="3" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="3" fillId="3" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="4" fillId="3" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="0" fillId="4" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="1" fillId="4" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="2" fillId="4" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="3" fillId="4" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="4" fillId="4" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="0" fillId="5" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="1" fillId="5" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="2" fillId="5" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="3" fillId="5" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="4" fillId="5" borderId="0" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="0" fillId="0" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="1" fillId="0" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="2" fillId="0" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="3" fillId="0" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="4" fillId="0" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="0" fillId="2" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="1" fillId="2" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="2" fillId="2" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="3" fillId="2" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="4" fillId="2" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="0" fillId="3" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="1" fillId="3" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="2" fillId="3" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="3" fillId="3" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="4" fillId="3" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="0" fillId="4" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="1" fillId="4" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="2" fillId="4" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="3" fillId="4" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="4" fillId="4" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="0" fillId="5" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="1" fillId="5" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="2" fillId="5" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="3" fillId="5" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="4" fillId="5" borderId="1" applyFont="1" applyFill="1" applyBorder="1"/><xf numFmtId="0" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyAlignment="1"><alignment horizontal="left"/></xf><xf numFmtId="0" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyAlignment="1"><alignment horizontal="center"/></xf><xf numFmtId="0" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyAlignment="1"><alignment horizontal="right"/></xf><xf numFmtId="0" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyAlignment="1"><alignment horizontal="fill"/></xf><xf numFmtId="0" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyAlignment="1"><alignment textRotation="90"/></xf><xf numFmtId="0" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyAlignment="1"><alignment wrapText="1"/></xf><xf numFmtId="9"   fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyNumberFormat="1"/><xf numFmtId="164" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyNumberFormat="1"/><xf numFmtId="165" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyNumberFormat="1"/><xf numFmtId="166" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyNumberFormat="1"/><xf numFmtId="167" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyNumberFormat="1"/><xf numFmtId="168" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyNumberFormat="1"/><xf numFmtId="169" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyNumberFormat="1"/><xf numFmtId="3" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyNumberFormat="1"/><xf numFmtId="4" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyNumberFormat="1"/><xf numFmtId="1" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyNumberFormat="1"/><xf numFmtId="2" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyNumberFormat="1"/><xf numFmtId="14" fontId="0" fillId="0" borderId="0" applyFont="1" applyFill="1" applyBorder="1" xfId="0" applyNumberFormat="1"/></cellXfs><cellStyles count="1"><cellStyle name="Normal" xfId="0" builtinId="0" /></cellStyles><dxfs count="0" /><tableStyles count="0" defaultTableStyle="TableStyleMedium9" defaultPivotStyle="PivotStyleMedium4" /></styleSheet>'
     },
-    _s = [{
+    Cs = [{
         match: /^\-?\d+\.\d%$/,
         style: 60,
         fmt: function(t) {
             return t / 100
         }
     }, {
         match: /^\-?\d+\.?\d*%$/,
@@ -11639,31 +11652,31 @@
     }, {
         match: /^[\d]{4}\-[01][\d]\-[0123][\d]$/,
         style: 67,
         fmt: function(t) {
             return Math.round(25569 + Date.parse(t) / (86400 * 1e3))
         }
     }],
-    En = function(t, e, r, n, s) {
+    On = function(t, e, r, n, s) {
         var a = ae("mergeCells", t);
         a[0].appendChild(Ce(t, "mergeCell", {
             attr: {
                 ref: Qr(r) + e + ":" + Qr(r + s - 1) + (e + n - 1)
             }
         })), a.attr("count", parseFloat(a.attr("count")) + 1)
     };
 st.ext.buttons.copyHtml5 = {
     className: "buttons-copy buttons-html5",
     text: function(t) {
         return t.i18n("buttons.copy", "Copy")
     },
     action: function(t, e, r, n, s) {
-        var a = Ds(e, n),
+        var a = As(e, n),
             l = e.buttons.exportInfo(n),
-            c = Ss(n),
+            c = Ds(n),
             p = a.str,
             b = ae("<div/>").css({
                 height: 1,
                 width: 1,
                 overflow: "hidden",
                 position: "fixed",
                 top: 0,
@@ -11712,18 +11725,18 @@
     available: function() {
         return window.FileReader !== void 0 && window.Blob
     },
     text: function(t) {
         return t.i18n("buttons.csv", "CSV")
     },
     action: function(t, e, r, n, s) {
-        var a = Ds(e, n).str,
+        var a = As(e, n).str,
             l = e.buttons.exportInfo(n),
             c = n.charset;
-        n.customize && (a = n.customize(a, n, e)), c !== !1 ? (c || (c = document.characterSet || document.charset), c && (c = ";charset=" + c)) : c = "", n.bom && (a = "\uFEFF" + a), On(new Blob([a], {
+        n.customize && (a = n.customize(a, n, e)), c !== !1 ? (c || (c = document.characterSet || document.charset), c && (c = ";charset=" + c)) : c = "", n.bom && (a = "\uFEFF" + a), Rn(new Blob([a], {
             type: "text/csv" + c
         }), l.filename, !0), s()
     },
     async: 100,
     filename: "*",
     extension: ".csv",
     exportOptions: {},
@@ -11733,23 +11746,23 @@
     charset: null,
     header: !0,
     footer: !0
 };
 st.ext.buttons.excelHtml5 = {
     className: "buttons-excel buttons-html5",
     available: function() {
-        return window.FileReader !== void 0 && ji() !== void 0 && !As() && Rn
+        return window.FileReader !== void 0 && Mi() !== void 0 && !Is() && Ln
     },
     text: function(t) {
         return t.i18n("buttons.excel", "Excel")
     },
     action: function(t, e, r, n, s) {
         var a = 0,
             l, c, p = function(g) {
-                var _ = Ps[g];
+                var _ = Fs[g];
                 return ae.parseXML(_)
             },
             b = p("xl/worksheets/sheet1.xml"),
             m = b.getElementsByTagName("sheetData")[0],
             y = {
                 _rels: {
                     ".rels": p("_rels/.rels")
@@ -11777,16 +11790,16 @@
                     var N = Qr(_) + "" + w,
                         R = null;
                     if (g[_] === null || g[_] === void 0 || g[_] === "")
                         if (n.createEmptyCells === !0) g[_] = "";
                         else continue;
                     var L = g[_];
                     g[_] = typeof g[_].trim == "function" ? g[_].trim() : g[_];
-                    for (var X = 0, j = _s.length; X < j; X++) {
-                        var G = _s[X];
+                    for (var X = 0, j = Cs.length; X < j; X++) {
+                        var G = Cs[X];
                         if (g[_].match && !g[_].match(/^0\d+/) && g[_].match(G.match)) {
                             var at = g[_].replace(/[^\d\.\-]/g, "");
                             G.fmt && (at = G.fmt(at)), R = Ce(b, "c", {
                                 attr: {
                                     r: N,
                                     s: G.style
                                 },
@@ -11832,58 +11845,58 @@
                 m.appendChild(k), a++
             },
             F = function(g) {
                 g.forEach(function(_) {
                     P(_.map(function(S) {
                         return S ? S.title : ""
                     }), a), ae("row:last c", b).attr("s", "2"), _.forEach(function(S, N) {
-                        S && (S.colSpan > 1 || S.rowSpan > 1) && En(b, a, N, S.rowSpan, S.colSpan)
+                        S && (S.colSpan > 1 || S.rowSpan > 1) && On(b, a, N, S.rowSpan, S.colSpan)
                     })
                 })
             };
         n.customizeData && n.customizeData(T);
         var h = e.buttons.exportInfo(n);
-        h.title && (P([h.title], a), En(b, a, 0, 1, T.header.length), ae("row:last c", b).attr("s", "51")), h.messageTop && (P([h.messageTop], a), En(b, a, 0, 1, T.header.length)), n.header && F(T.headerStructure), l = a;
+        h.title && (P([h.title], a), On(b, a, 0, 1, T.header.length), ae("row:last c", b).attr("s", "51")), h.messageTop && (P([h.messageTop], a), On(b, a, 0, 1, T.header.length)), n.header && F(T.headerStructure), l = a;
         for (var o = 0, f = T.body.length; o < f; o++) P(T.body[o], a);
-        c = a, n.footer && T.footer && F(T.footerStructure), h.messageBottom && (P([h.messageBottom], a), En(b, a, 0, 1, T.header.length));
+        c = a, n.footer && T.footer && F(T.footerStructure), h.messageBottom && (P([h.messageBottom], a), On(b, a, 0, 1, T.header.length));
         var C = Ce(b, "cols");
         ae("worksheet", b).prepend(C);
         for (var B = 0, u = T.header.length; B < u; B++) C.appendChild(Ce(b, "col", {
             attr: {
                 min: B + 1,
                 max: B + 1,
-                width: El(T, B),
+                width: Ol(T, B),
                 customWidth: 1
             }
         }));
         var z = y.xl["workbook.xml"];
-        ae("sheets sheet", z).attr("name", xs(n)), n.autoFilter && (ae("mergeCells", b).before(Ce(b, "autoFilter", {
+        ae("sheets sheet", z).attr("name", _s(n)), n.autoFilter && (ae("mergeCells", b).before(Ce(b, "autoFilter", {
             attr: {
                 ref: "A" + l + ":" + Qr(T.header.length - 1) + c
             }
         })), ae("definedNames", z).append(Ce(z, "definedName", {
             attr: {
                 name: "_xlnm._FilterDatabase",
                 localSheetId: "0",
                 hidden: 1
             },
-            text: "'" + xs(n).replace(/'/g, "''") + "'!$A$" + l + ":" + Qr(T.header.length - 1) + c
+            text: "'" + _s(n).replace(/'/g, "''") + "'!$A$" + l + ":" + Qr(T.header.length - 1) + c
         }))), n.customize && n.customize(y, n, e), ae("mergeCells", b).children().length === 0 && ae("mergeCells", b).remove();
-        var q = ji(),
+        var q = Mi(),
             et = new q,
             O = {
                 compression: "DEFLATE",
                 type: "blob",
                 mimeType: "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet"
             };
-        Is(et, y);
+        Ps(et, y);
         var Z = h.filename;
         Z > 175 && (Z = Z.substr(0, 175)), n.customizeZip && n.customizeZip(et, T, Z), et.generateAsync ? et.generateAsync(O).then(function(g) {
-            On(g, Z), s()
-        }) : (On(et.generate(O), Z), s())
+            Rn(g, Z), s()
+        }) : (Rn(et.generate(O), Z), s())
     },
     async: 100,
     filename: "*",
     extension: ".xlsx",
     exportOptions: {},
     header: !0,
     footer: !0,
@@ -11893,15 +11906,15 @@
     createEmptyCells: !1,
     autoFilter: !1,
     sheetName: ""
 };
 st.ext.buttons.pdfHtml5 = {
     className: "buttons-pdf buttons-html5",
     available: function() {
-        return window.FileReader !== void 0 && Mi()
+        return window.FileReader !== void 0 && Vi()
     },
     text: function(t) {
         return t.i18n("buttons.pdf", "PDF")
     },
     action: function(t, e, r, n, s) {
         var a = e.buttons.exportData(n.exportOptions),
             l = e.buttons.exportInfo(n),
@@ -11994,16 +12007,16 @@
             style: "message",
             margin: [0, 0, 0, 12]
         }), l.title && m.content.unshift({
             text: l.title,
             style: "title",
             margin: [0, 0, 0, 12]
         }), n.customize && n.customize(m, n, e);
-        var y = Mi().createPdf(m);
-        n.download === "open" && !As() ? y.open() : y.download(l.filename), s()
+        var y = Vi().createPdf(m);
+        n.download === "open" && !Is() ? y.open() : y.download(l.filename), s()
     },
     async: 100,
     title: "*",
     filename: "*",
     extension: ".pdf",
     exportOptions: {},
     orientation: "portrait",
@@ -12011,22 +12024,22 @@
     header: !0,
     footer: !0,
     messageTop: "*",
     messageBottom: "*",
     customize: null,
     download: "download"
 };
-var Fs = ne(ie(), 1);
-var Nr = Fs.default,
+var Bs = ne(ie(), 1);
+var Nr = Bs.default,
     Br = document.createElement("a"),
-    Ol = function(t) {
+    Rl = function(t) {
         var e = Nr(t).clone()[0];
-        return e.nodeName.toLowerCase() === "link" && (e.href = Bs(e.href)), e.outerHTML
+        return e.nodeName.toLowerCase() === "link" && (e.href = Ns(e.href)), e.outerHTML
     },
-    Bs = function(t) {
+    Ns = function(t) {
         Br.href = t;
         var e = Br.host;
         return e.indexOf("/") === -1 && Br.pathname.indexOf("/") !== 0 && (e += "/"), Br.protocol + "//" + e + Br.pathname + Br.search
     };
 st.ext.buttons.print = {
     className: "buttons-print",
     text: function(t) {
@@ -12072,23 +12085,23 @@
         if (!k) {
             e.buttons.info(e.i18n("buttons.printErrorTitle", "Unable to open print view"), e.i18n("buttons.printErrorMsg", "Please allow popups in your browser for this site to be able to view the print view."), 5e3);
             return
         }
         k.document.close();
         var P = "<title>" + l.title + "</title>";
         Nr("style, link").each(function() {
-            P += Ol(this)
+            P += Rl(this)
         });
         try {
             k.document.head.innerHTML = P
         } catch {
             Nr(k.document.head).html(P)
         }
         k.document.body.innerHTML = "<h1>" + l.title + "</h1><div>" + (l.messageTop || "") + "</div>" + b + "<div>" + (l.messageBottom || "") + "</div>", Nr(k.document.body).addClass("dt-print-view"), Nr("img", k.document.body).each(function(h, o) {
-            o.setAttribute("src", Bs(o.getAttribute("src")))
+            o.setAttribute("src", Ns(o.getAttribute("src")))
         }), n.customize && n.customize(k, n, e);
         var F = function() {
             n.autoPrint && (k.print(), k.close())
         };
         k.setTimeout(F, 1e3), s()
     },
     async: 100,
@@ -12097,17 +12110,17 @@
     messageBottom: "*",
     exportOptions: {},
     header: !0,
     footer: !0,
     autoPrint: !0,
     customize: null
 };
-var Rl = ne(ie(), 1);
-var Ns = ne(ie(), 1);
-var ir = Ns.default;
+var Ll = ne(ie(), 1);
+var Es = ne(ie(), 1);
+var ir = Es.default;
 (function() {
     "use strict";
     var t, e;
 
     function r(l) {
         t = l, e = t.fn.dataTable
     }
@@ -12288,29 +12301,29 @@
             m = new n(p, b);
         return m
     }
     ir(document).on("plugin-init.dt", function(l, c) {
         l.namespace === "dt" && (c.oInit.fixedColumns || st.defaults.fixedColumns) && (c._fixedColumns || a(c, null))
     })
 })();
-var jl = ne(ie(), 1);
-var Es = ne(ie(), 1);
-var jt = Es.default,
-    Ll = 0,
+var Ml = ne(ie(), 1);
+var Os = ne(ie(), 1);
+var jt = Os.default,
     zl = 0,
+    jl = 0,
     vr = function(t, e) {
         if (!st.versionCheck || !st.versionCheck("1.10.8")) throw "KeyTable requires DataTables 1.10.8 or newer";
         this.c = jt.extend(!0, {}, st.defaults.keyTable, vr.defaults, e), this.s = {
             dt: new st.Api(t),
             dtDrawing: !1,
             enable: !0,
             focusDraw: !1,
             waitingForDraw: !1,
             lastFocus: null,
-            namespace: ".keyTable-" + Ll++,
+            namespace: ".keyTable-" + zl++,
             tabInput: null
         }, this.dom = {};
         var r = this.s.dt.settings()[0],
             n = r.keytable;
         if (n) return n;
         r.keytable = this, this._constructor()
     };
@@ -12443,15 +12456,15 @@
     },
     _editor: function(t, e, r) {
         if (this.s.lastFocus && !(e && e.type === "draw")) {
             var n = this,
                 s = this.s.dt,
                 a = this.c.editor,
                 l = this.s.lastFocus.cell,
-                c = this.s.namespace + "e" + zl++;
+                c = this.s.namespace + "e" + jl++;
             if (!jt("div.DTE", l.node()).length && !(t !== null && (t >= 0 && t <= 9 || t === 11 || t === 12 || t >= 14 && t <= 31 || t >= 112 && t <= 123 || t >= 127 && t <= 159))) {
                 e && (e.stopPropagation(), t === 13 && e.preventDefault());
                 var p = function() {
                     var b = n._inlineOptions(l.index());
                     a.one("open" + c, function() {
                         a.off("cancelOpen" + c), r || jt("div.DTE_Field_InputControl input, div.DTE_Field_InputControl textarea").select(), s.keys.enable(r ? "tab-only" : "navigation-only"), s.on("key-blur.editor", function(m, y, T) {
                             a.s.editOpts.onBlur !== "submit" && a.displayed() && T.node() === l.node() && a.submit()
@@ -12764,17 +12777,17 @@
             s = st.defaults.keys;
         if (n || s) {
             var a = jt.extend({}, s, n);
             n !== !1 && new vr(e, a)
         }
     }
 });
-var Ml = ne(ie(), 1);
-var Os = ne(ie(), 1);
-var Ee = Os.default,
+var Vl = ne(ie(), 1);
+var Rs = ne(ie(), 1);
+var Ee = Rs.default,
     mr = function(t, e) {
         if (!st.versionCheck || !st.versionCheck("1.11")) throw "RowGroup requires DataTables 1.11 or newer";
         this.c = Ee.extend(!0, {}, st.defaults.rowGroup, mr.defaults, e), this.s = {
             dt: new st.Api(t)
         }, this.dom = {};
         var r = this.s.dt.settings()[0],
             n = r.rowGroup;
@@ -12897,17 +12910,17 @@
             s = st.defaults.rowGroup;
         if (n || s) {
             var a = Ee.extend({}, s, n);
             n !== !1 && new mr(e, a)
         }
     }
 });
-var Vl = ne(ie(), 1);
-var Rs = ne(ie(), 1);
-var ar = Rs.default;
+var Hl = ne(ie(), 1);
+var Ls = ne(ie(), 1);
+var ar = Ls.default;
 (function() {
     "use strict";
     var t, e;
 
     function r() {
         return window.moment
     }
@@ -14805,17 +14818,17 @@
     ar(document).on("preInit.dt.dtsp", function(h, o) {
         h.namespace === "dt" && (o.oInit.searchBuilder || st.defaults.searchBuilder) && (o._searchBuilder || F(o))
     }), st.ext.feature.push({
         cFeature: "Q",
         fnInit: F
     }), st.feature && st.feature.register("searchBuilder", F)
 })();
-var Hl = ne(ie(), 1);
-var Ls = ne(ie(), 1);
-var qe = Ls.default;
+var Wl = ne(ie(), 1);
+var zs = ne(ie(), 1);
+var Ge = zs.default;
 (function() {
     "use strict";
     var t, e;
 
     function r(g) {
         t = g, e = g.fn.dataTable
     }
@@ -16256,18 +16269,18 @@
                         }
                     }
                     this.s.dt.draw(!1)
                 }
                 this.s.updating = !1
             }, _
         }(B);
-    r(qe), C(qe), p(qe), T(qe), F(qe);
-    var q = qe.fn.dataTable;
+    r(Ge), C(Ge), p(Ge), T(Ge), F(Ge);
+    var q = Ge.fn.dataTable;
     q.SearchPanes = B, st.SearchPanes = B, q.SearchPanesST = z, st.SearchPanesST = z, q.SearchPane = n, st.SearchPane = n, q.SearchPaneViewTotal = b, st.SearchPaneViewTotal = b, q.SearchPaneCascade = w, st.SearchPaneCascade = w, q.SearchPaneCascadeViewTotal = h, st.SearchPaneCascadeViewTotal = h;
-    var et = qe.fn.dataTable.Api.register;
+    var et = Ge.fn.dataTable.Api.register;
     et("searchPanes()", function() {
         return this
     }), et("searchPanes.clearSelections()", function() {
         return this.iterator("table", function(g) {
             g._searchPanes && g._searchPanes.clearSelections()
         })
     }), et("searchPanes.rebuildPane()", function(g, _) {
@@ -16292,27 +16305,27 @@
             N._panes ? (this.popover(N._panes.getNode(), {
                 align: "container",
                 span: "container"
             }), N._panes.rebuild(void 0, !0)) : (this.processing(!0), setTimeout(function() {
                 O(_, S, N), R.popover(N._panes.getNode(), {
                     align: "container",
                     span: "container"
-                }), N._panes.rebuild(void 0, !0), qe("table.dataTable", N._panes.getNode()).DataTable().columns.adjust(), L.processing(!1)
+                }), N._panes.rebuild(void 0, !0), Ge("table.dataTable", N._panes.getNode()).DataTable().columns.adjust(), L.processing(!1)
             }, 10))
         },
         init: function(g, _, S) {
             g.button(_).text(S.text || g.i18n("searchPanes.collapse", "SearchPanes", 0)), (g.init().stateSave || S.delayInit === !1) && O(g, _, S)
         },
         config: {},
         text: "",
         delayInit: !0
     };
 
     function O(g, _, S) {
-        var N = qe.extend({
+        var N = Ge.extend({
                 filterChanged: function(L) {
                     g.button(_).text(g.i18n("searchPanes.collapse", g.context[0].oLanguage.searchPanes !== void 0 ? g.context[0].oLanguage.searchPanes.collapse : g.context[0]._searchPanes.c.i18n.collapse, L))
                 }
             }, S.config),
             R = N && (N.cascadePanes || N.viewTotal) ? new st.SearchPanesST(g, N) : new st.SearchPanes(g, N);
         g.button(_).text(S.text || g.i18n("searchPanes.collapse", R.c.i18n.collapse, 0)), S._panes = R
     }
@@ -16321,26 +16334,29 @@
         _ === void 0 && (_ = null), S === void 0 && (S = !1);
         var N = new q.Api(g),
             R = _ || N.init().searchPanes || q.defaults.searchPanes,
             L = R && (R.cascadePanes || R.viewTotal) ? new z(N, R, S) : new B(N, R, S),
             X = L.getNode();
         return X
     }
-    qe(document).on("preInit.dt.dtsp", function(g, _) {
+    Ge(document).on("preInit.dt.dtsp", function(g, _) {
         g.namespace === "dt" && (_.oInit.searchPanes || st.defaults.searchPanes) && (_._searchPanes || Z(_, null, !0))
     }), st.ext.feature.push({
         cFeature: "P",
         fnInit: Z
     }), st.feature && st.feature.register("searchPanes", Z)
 })();
-var ql = ne(ie(), 1);
-var Hs = ne(ie(), 1);
-var Rt = Hs.default;
+var Gl = ne(ie(), 1);
+var Ws = ne(ie(), 1);
+var Rt = Ws.default;
 st.select = {};
-st.select.version = "2.0.1";
+st.select.classes = {
+    checkbox: "dt-select-checkbox"
+};
+st.select.version = "2.0.2";
 st.select.init = function(t) {
     var e = t.settings()[0];
     if (!st.versionCheck("2")) throw "Warning: Select requires DataTables 2 or newer";
     if (!e._select) {
         var r = t.state.loaded(),
             n = function(F, h, o) {
                 if (!(o === null || o.select === void 0)) {
@@ -16381,21 +16397,21 @@
             y = !0,
             T = "td, th",
             w = "selected",
             k = !0,
             P = !1;
         e._select = {
             infoEls: []
-        }, l === !0 ? (p = "os", P = !0) : typeof l == "string" ? (p = l, P = !0) : Rt.isPlainObject(l) && (l.blurable !== void 0 && (b = l.blurable), l.toggleable !== void 0 && (m = l.toggleable), l.info !== void 0 && (y = l.info), l.items !== void 0 && (c = l.items), l.style !== void 0 ? (p = l.style, P = !0) : (p = "os", P = !0), l.selector !== void 0 && (T = l.selector), l.className !== void 0 && (w = l.className), l.headerCheckbox !== void 0 && (k = l.headerCheckbox)), t.select.selector(T), t.select.items(c), t.select.style(p), t.select.blurable(b), t.select.toggleable(m), t.select.info(y), e._select.className = w, !P && Rt(t.table().node()).hasClass("selectable") && t.select.style("os"), k && (Ms(t), t.on("init", function() {
-            Ms(t)
+        }, l === !0 ? (p = "os", P = !0) : typeof l == "string" ? (p = l, P = !0) : Rt.isPlainObject(l) && (l.blurable !== void 0 && (b = l.blurable), l.toggleable !== void 0 && (m = l.toggleable), l.info !== void 0 && (y = l.info), l.items !== void 0 && (c = l.items), l.style !== void 0 ? (p = l.style, P = !0) : (p = "os", P = !0), l.selector !== void 0 && (T = l.selector), l.className !== void 0 && (w = l.className), l.headerCheckbox !== void 0 && (k = l.headerCheckbox)), t.select.selector(T), t.select.items(c), t.select.style(p), t.select.blurable(b), t.select.toggleable(m), t.select.info(y), e._select.className = w, !P && Rt(t.table().node()).hasClass("selectable") && t.select.style("os"), k && (Vs(t), t.on("init", function() {
+            Vs(t)
         }))
     }
 };
 
-function zs(t, e, r) {
+function js(t, e, r) {
     var n, s, a, l = function(p, b) {
             if (p > b) {
                 var m = b;
                 b = p, p = m
             }
             var y = !1;
             return t.columns(":visible").indexes().filter(function(T) {
@@ -16418,21 +16434,26 @@
     !t.cells({
         selected: !0
     }).any() && !r ? (s = l(0, e.column), a = c(0, e.row)) : (s = l(r.column, e.column), a = c(r.row, e.row)), n = t.cells(a, s).flatten(), t.cells(e, {
         selected: !0
     }).any() ? t.cells(n).deselect() : t.cells(n).select()
 }
 
-function Ui(t) {
+function Jr(t) {
+    var e = st.select.classes.checkbox;
+    return t ? e.replace(/ /g, ".") : e
+}
+
+function qi(t) {
     var e = t.settings()[0],
         r = e._select.selector;
-    Rt(t.table().container()).off("mousedown.dtSelect", r).off("mouseup.dtSelect", r).off("click.dtSelect", r), Rt("body").off("click.dtSelect" + qi(t.table().node()))
+    Rt(t.table().container()).off("mousedown.dtSelect", r).off("mouseup.dtSelect", r).off("click.dtSelect", r), Rt("body").off("click.dtSelect" + Gi(t.table().node()))
 }
 
-function Ws(t) {
+function Us(t) {
     var e = Rt(t.table().container()),
         r = t.settings()[0],
         n = r._select.selector,
         s;
     e.on("mousedown.dtSelect", n, function(a) {
         (a.shiftKey || a.metaKey || a.ctrlKey) && e.css("-moz-user-select", "none").one("selectstart.dtSelect", n, function() {
             return !1
@@ -16448,35 +16469,35 @@
         }
         var b = t.settings()[0],
             m = t.table().container();
         if (Rt(a.target).closest("div.dt-container")[0] == m) {
             var y = t.cell(Rt(a.target).closest("td, th"));
             if (y.any()) {
                 var T = Rt.Event("user-select.dt");
-                if (Ge(t, T, [l, y, a]), !T.isDefaultPrevented()) {
+                if (Xe(t, T, [l, y, a]), !T.isDefaultPrevented()) {
                     var w = y.index();
-                    l === "row" ? (c = w.row, Vi(a, t, b, "row", c)) : l === "column" ? (c = y.index().column, Vi(a, t, b, "column", c)) : l === "cell" && (c = y.index(), Vi(a, t, b, "cell", c)), b._select_lastCell = w
+                    l === "row" ? (c = w.row, Hi(a, t, b, "row", c)) : l === "column" ? (c = y.index().column, Hi(a, t, b, "column", c)) : l === "cell" && (c = y.index(), Hi(a, t, b, "cell", c)), b._select_lastCell = w
                 }
             }
         }
-    }), Rt("body").on("click.dtSelect" + qi(t.table().node()), function(a) {
+    }), Rt("body").on("click.dtSelect" + Gi(t.table().node()), function(a) {
         if (r._select.blurable) {
             if (Rt(a.target).parents().filter(t.table().container()).length || Rt(a.target).parents("html").length === 0 || Rt(a.target).parents("div.DTE").length) return;
             var l = Rt.Event("select-blur.dt");
-            if (Ge(t, l, [a.target, a]), l.isDefaultPrevented()) return;
-            Jr(r, !0)
+            if (Xe(t, l, [a.target, a]), l.isDefaultPrevented()) return;
+            tn(r, !0)
         }
     })
 }
 
-function Ge(t, e, r, n) {
+function Xe(t, e, r, n) {
     n && !t.flatten().length || (typeof e == "string" && (e = e + ".dt"), r.unshift(t), Rt(t.table().node()).trigger(e, r))
 }
 
-function js(t, e) {
+function Ms(t, e) {
     if (!(t.select.style() === "api" || t.select.info() === !1)) {
         var r = t.rows({
                 selected: !0
             }).flatten().length,
             n = t.columns({
                 selected: !0
             }).flatten().length,
@@ -16494,20 +16515,20 @@
             c = Rt('<span class="select-info"/>');
         a(c, "row", r), a(c, "column", n), a(c, "cell", s);
         var p = l.children("span.select-info");
         p.length && p.remove(), c.text() !== "" && l.append(c)
     }
 }
 
-function Ms(t) {
+function Vs(t) {
     t.columns(".dt-select").every(function() {
         var e = this.header();
         if (!Rt("input", e).length) {
             var r = Rt("<input>").attr({
-                class: "dt-select-checkbox",
+                class: Jr(!0),
                 type: "checkbox",
                 "aria-label": t.i18n("select.aria.headerCheckbox") || "Select all rows"
             }).appendTo(e).on("change", function() {
                 this.checked ? t.rows({
                     search: "applied"
                 }).select() : t.rows({
                     selected: !0
@@ -16530,19 +16551,19 @@
                     c && c <= l && c === p ? r.prop("checked", !0).prop("indeterminate", !1) : c === 0 && l === 0 ? r.prop("checked", !1).prop("indeterminate", !1) : r.prop("checked", !1).prop("indeterminate", !0)
                 }
             })
         }
     })
 }
 
-function Wl(t) {
+function Ul(t) {
     var e = new st.Api(t);
     t._select_init = !0, t.aoRowCreatedCallback.push(function(r, n, s) {
         var a, l, c = t.aoData[s];
-        for (c._select_selected && Rt(r).addClass(t._select.className).find("input.dt-select-checkbox").prop("checked", !0), a = 0, l = t.aoColumns.length; a < l; a++)(t.aoColumns[a]._select_selected || c._selected_cells && c._selected_cells[a]) && Rt(c.anCells[a]).addClass(t._select.className)
+        for (c._select_selected && Rt(r).addClass(t._select.className).find("input." + Jr(!0)).prop("checked", !0), a = 0, l = t.aoColumns.length; a < l; a++)(t.aoColumns[a]._select_selected || c._selected_cells && c._selected_cells[a]) && Rt(c.anCells[a]).addClass(t._select.className)
     }), e.on("preXhr.dt.dtSelect", function(r, n) {
         if (n === e.settings()[0]) {
             var s = e.rows({
                     selected: !0
                 }).ids(!0).filter(function(l) {
                     return l !== void 0
                 }),
@@ -16560,27 +16581,27 @@
             e.one("draw.dt.dtSelect", function() {
                 e.rows(s).select(), a.any() && a.each(function(l) {
                     e.cells(l.row, l.column).select()
                 })
             })
         }
     }), e.on("info.dt", function(r, n, s) {
-        n._select.infoEls.includes(s) || n._select.infoEls.push(s), js(e, s)
+        n._select.infoEls.includes(s) || n._select.infoEls.push(s), Ms(e, s)
     }), e.on("select.dtSelect.dt deselect.dtSelect.dt", function() {
         t._select.infoEls.forEach(function(r) {
-            js(e, r)
+            Ms(e, r)
         }), e.state.save()
     }), e.on("destroy.dtSelect", function() {
         Rt(e.rows({
             selected: !0
-        }).nodes()).removeClass(e.settings()[0]._select.className), Ui(e), e.off(".dtSelect"), Rt("body").off(".dtSelect" + qi(e.table().node()))
+        }).nodes()).removeClass(e.settings()[0]._select.className), qi(e), e.off(".dtSelect"), Rt("body").off(".dtSelect" + Gi(e.table().node()))
     })
 }
 
-function Vs(t, e, r, n) {
+function Hs(t, e, r, n) {
     var s = t[e + "s"]({
             search: "applied"
         }).indexes(),
         a = s.indexOf(n),
         l = s.indexOf(r);
     if (!t[e + "s"]({
             selected: !0
@@ -16593,46 +16614,46 @@
         s.splice(l + 1, s.length), s.splice(0, a)
     }
     t[e](r, {
         selected: !0
     }).any() ? (s.splice(s.indexOf(r), 1), t[e + "s"](s).deselect()) : t[e + "s"](s).select()
 }
 
-function Jr(t, e) {
+function tn(t, e) {
     if (e || t._select.style === "single") {
         var r = new st.Api(t);
         r.rows({
             selected: !0
         }).deselect(), r.columns({
             selected: !0
         }).deselect(), r.cells({
             selected: !0
         }).deselect()
     }
 }
 
-function Vi(t, e, r, n, s) {
+function Hi(t, e, r, n, s) {
     var a = e.select.style(),
         l = e.select.toggleable(),
         c = e[n](s, {
             selected: !0
         }).any();
     if (!(c && !l))
         if (a === "os")
             if (t.ctrlKey || t.metaKey) e[n](s).select(!c);
-            else if (t.shiftKey) n === "cell" ? zs(e, s, r._select_lastCell || null) : Vs(e, n, s, r._select_lastCell ? r._select_lastCell[n] : null);
+            else if (t.shiftKey) n === "cell" ? js(e, s, r._select_lastCell || null) : Hs(e, n, s, r._select_lastCell ? r._select_lastCell[n] : null);
     else {
         var p = e[n + "s"]({
             selected: !0
         });
         c && p.flatten().length === 1 ? e[n](s).deselect() : (p.deselect(), e[n](s).select())
-    } else a == "multi+shift" && t.shiftKey ? n === "cell" ? zs(e, s, r._select_lastCell || null) : Vs(e, n, s, r._select_lastCell ? r._select_lastCell[n] : null) : e[n](s).select(!c)
+    } else a == "multi+shift" && t.shiftKey ? n === "cell" ? js(e, s, r._select_lastCell || null) : Hs(e, n, s, r._select_lastCell ? r._select_lastCell[n] : null) : e[n](s).select(!c)
 }
 
-function qi(t) {
+function Gi(t) {
     return t.id.replace(/[^a-zA-Z0-9\-\_]/g, "-")
 }
 Rt.each([{
     type: "row",
     prop: "aoData"
 }, {
     type: "column",
@@ -16673,77 +16694,77 @@
 ze("select.info()", function(t) {
     return t === void 0 ? this.context[0]._select.info : this.iterator("table", function(e) {
         e._select.info = t
     })
 });
 ze("select.items()", function(t) {
     return t === void 0 ? this.context[0]._select.items : this.iterator("table", function(e) {
-        e._select.items = t, Ge(new st.Api(e), "selectItems", [t])
+        e._select.items = t, Xe(new st.Api(e), "selectItems", [t])
     })
 });
 ze("select.style()", function(t) {
     return t === void 0 ? this.context[0]._select.style : this.iterator("table", function(e) {
-        e._select || st.select.init(new st.Api(e)), e._select_init || Wl(e), e._select.style = t;
+        e._select || st.select.init(new st.Api(e)), e._select_init || Ul(e), e._select.style = t;
         var r = new st.Api(e);
-        Ui(r), t !== "api" && Ws(r), Ge(new st.Api(e), "selectStyle", [t])
+        qi(r), t !== "api" && Us(r), Xe(new st.Api(e), "selectStyle", [t])
     })
 });
 ze("select.selector()", function(t) {
     return t === void 0 ? this.context[0]._select.selector : this.iterator("table", function(e) {
-        Ui(new st.Api(e)), e._select.selector = t, e._select.style !== "api" && Ws(new st.Api(e))
+        qi(new st.Api(e)), e._select.selector = t, e._select.style !== "api" && Us(new st.Api(e))
     })
 });
 ze("select.last()", function(t) {
     let e = this.context[0];
     return t ? (e._select_lastCell = t, this) : e._select_lastCell
 });
 Or("rows().select()", "row().select()", function(t) {
     var e = this;
     return t === !1 ? this.deselect() : (this.iterator("row", function(r, n) {
-        Jr(r);
+        tn(r);
         var s = r.aoData[n],
             a = r.aoColumns;
         Rt(s.nTr).addClass(r._select.className), s._select_selected = !0;
         for (var l = 0; l < a.length; l++) {
             var c = a[l];
             if (c.sType === null && e.columns().types(), c.sType === "select-checkbox") {
                 var p = s.anCells;
-                p && p[l] && Rt("input.dt-select-checkbox", p[l]).prop("checked", !0), s._aSortData !== null && (s._aSortData[l] = null)
+                p && p[l] && Rt("input." + Jr(!0), p[l]).prop("checked", !0), s._aSortData !== null && (s._aSortData[l] = null)
             }
         }
     }), this.iterator("table", function(r, n) {
-        Ge(e, "select", ["row", e[n]], !0)
+        Xe(e, "select", ["row", e[n]], !0)
     }), this)
 });
 ze("row().selected()", function() {
     var t = this.context[0];
     return !!(t && this.length && t.aoData[this[0]] && t.aoData[this[0]]._select_selected)
 });
 Or("columns().select()", "column().select()", function(t) {
     var e = this;
     return t === !1 ? this.deselect() : (this.iterator("column", function(r, n) {
-        Jr(r), r.aoColumns[n]._select_selected = !0;
+        tn(r), r.aoColumns[n]._select_selected = !0;
         var s = new st.Api(r).column(n);
         Rt(s.header()).addClass(r._select.className), Rt(s.footer()).addClass(r._select.className), s.nodes().to$().addClass(r._select.className)
     }), this.iterator("table", function(r, n) {
-        Ge(e, "select", ["column", e[n]], !0)
+        Xe(e, "select", ["column", e[n]], !0)
     }), this)
 });
 ze("column().selected()", function() {
     var t = this.context[0];
     return !!(t && this.length && t.aoColumns[this[0]] && t.aoColumns[this[0]]._select_selected)
 });
 Or("cells().select()", "cell().select()", function(t) {
     var e = this;
     return t === !1 ? this.deselect() : (this.iterator("cell", function(r, n, s) {
-        Jr(r);
+        tn(r);
         var a = r.aoData[n];
         a._selected_cells === void 0 && (a._selected_cells = []), a._selected_cells[s] = !0, a.anCells && Rt(a.anCells[s]).addClass(r._select.className)
     }), this.iterator("table", function(r, n) {
-        Ge(e, "select", ["cell", e.cells(e[n]).indexes().toArray()], !0)
+        Xe(e, "select", ["cell", e.cells(e[n]).indexes().toArray()], !0)
     }), this)
 });
 ze("cell().selected()", function() {
     var t = this.context[0];
     if (t && this.length) {
         var e = t.aoData[this[0][0].row];
         if (e && e._selected_cells && e._selected_cells[this[0][0].column]) return !0
@@ -16756,88 +16777,88 @@
         var n = e.aoData[r],
             s = e.aoColumns;
         Rt(n.nTr).removeClass(e._select.className), n._select_selected = !1, e._select_lastCell = null;
         for (var a = 0; a < s.length; a++) {
             var l = s[a];
             if (l.sType === null && t.columns().types(), l.sType === "select-checkbox") {
                 var c = n.anCells;
-                c && c[a] && Rt("input.dt-select-checkbox", n.anCells[a]).prop("checked", !1), n._aSortData !== null && (n._aSortData[a] = null)
+                c && c[a] && Rt("input." + Jr(!0), n.anCells[a]).prop("checked", !1), n._aSortData !== null && (n._aSortData[a] = null)
             }
         }
     }), this.iterator("table", function(e, r) {
-        Ge(t, "deselect", ["row", t[r]], !0)
+        Xe(t, "deselect", ["row", t[r]], !0)
     }), this
 });
 Or("columns().deselect()", "column().deselect()", function() {
     var t = this;
     return this.iterator("column", function(e, r) {
         e.aoColumns[r]._select_selected = !1;
         var n = new st.Api(e),
             s = n.column(r);
         Rt(s.header()).removeClass(e._select.className), Rt(s.footer()).removeClass(e._select.className), n.cells(null, r).indexes().each(function(a) {
             var l = e.aoData[a.row],
                 c = l._selected_cells;
             l.anCells && (!c || !c[a.column]) && Rt(l.anCells[a.column]).removeClass(e._select.className)
         })
     }), this.iterator("table", function(e, r) {
-        Ge(t, "deselect", ["column", t[r]], !0)
+        Xe(t, "deselect", ["column", t[r]], !0)
     }), this
 });
 Or("cells().deselect()", "cell().deselect()", function() {
     var t = this;
     return this.iterator("cell", function(e, r, n) {
         var s = e.aoData[r];
         s._selected_cells !== void 0 && (s._selected_cells[n] = !1), s.anCells && !e.aoColumns[n]._select_selected && Rt(s.anCells[n]).removeClass(e._select.className)
     }), this.iterator("table", function(e, r) {
-        Ge(t, "deselect", ["cell", t[r]], !0)
+        Xe(t, "deselect", ["cell", t[r]], !0)
     }), this
 });
 
 function Er(t, e) {
     return function(r) {
         return r.i18n("buttons." + t, e)
     }
 }
 
-function Hi(t) {
+function Wi(t) {
     var e = t._eventNamespace;
     return "draw.dt.DT" + e + " select.dt.DT" + e + " deselect.dt.DT" + e
 }
 
-function Ul(t, e) {
+function ql(t, e) {
     return !!(e.limitTo.indexOf("rows") !== -1 && t.rows({
         selected: !0
     }).any() || e.limitTo.indexOf("columns") !== -1 && t.columns({
         selected: !0
     }).any() || e.limitTo.indexOf("cells") !== -1 && t.cells({
         selected: !0
     }).any())
 }
-var Wi = 0;
+var Ui = 0;
 Rt.extend(st.ext.buttons, {
     selected: {
         text: Er("selected", "Selected"),
         className: "buttons-selected",
         limitTo: ["rows", "columns", "cells"],
         init: function(t, e, r) {
             var n = this;
-            r._eventNamespace = ".select" + Wi++, t.on(Hi(r), function() {
-                n.enable(Ul(t, r))
+            r._eventNamespace = ".select" + Ui++, t.on(Wi(r), function() {
+                n.enable(ql(t, r))
             }), this.disable()
         },
         destroy: function(t, e, r) {
             t.off(r._eventNamespace)
         }
     },
     selectedSingle: {
         text: Er("selectedSingle", "Selected single"),
         className: "buttons-selected-single",
         init: function(t, e, r) {
             var n = this;
-            r._eventNamespace = ".select" + Wi++, t.on(Hi(r), function() {
+            r._eventNamespace = ".select" + Ui++, t.on(Wi(r), function() {
                 var s = t.rows({
                     selected: !0
                 }).flatten().length + t.columns({
                     selected: !0
                 }).flatten().length + t.cells({
                     selected: !0
                 }).flatten().length;
@@ -16857,19 +16878,19 @@
             a ? (typeof a == "function" && (a = a.call(e, t, e, r, n)), this[s + "s"](a).select()) : this[s + "s"]().select()
         }
     },
     selectNone: {
         text: Er("selectNone", "Deselect all"),
         className: "buttons-select-none",
         action: function() {
-            Jr(this.settings()[0], !0)
+            tn(this.settings()[0], !0)
         },
         init: function(t, e, r) {
             var n = this;
-            r._eventNamespace = ".select" + Wi++, t.on(Hi(r), function() {
+            r._eventNamespace = ".select" + Ui++, t.on(Wi(r), function() {
                 var s = t.rows({
                     selected: !0
                 }).flatten().length + t.columns({
                     selected: !0
                 }).flatten().length + t.cells({
                     selected: !0
                 }).flatten().length;
@@ -16934,15 +16955,15 @@
         n = e ? st.util.get(e) : null;
     return function(s, a, l, c) {
         var p = c.settings.aoData[c.row],
             b = p._select_selected,
             m = c.settings.oLanguage.select.aria.rowCheckbox;
         return a === "display" ? Rt("<input>").attr({
             "aria-label": m,
-            class: "dt-select-checkbox",
+            class: Jr(),
             name: n ? n(l) : null,
             type: "checkbox",
             value: r ? r(l) : null,
             checked: b
         })[0] : a === "type" ? "select-checkbox" : a === "filter" ? "" : b ? "X" : ""
     }
 };
@@ -16953,18 +16974,20 @@
         return t._select.items === "row" ? Rt(r).parent().hasClass(t._select.className) : t._select.items === "cell" ? Rt(r).hasClass(t._select.className) : !1
     })
 };
 Rt.fn.DataTable.select = st.select;
 Rt(document).on("preInit.dt.dtSelect", function(t, e) {
     t.namespace === "dt" && st.select.init(new st.Api(e))
 });
-Ke.Buttons.jszip(Us.default);
-var export_jQuery = Gl.default;
+qe.Buttons.jszip(qs.default);
+var Iu = qe;
+var export_jQuery = Xl.default;
 export {
-    Ke as DataTable, export_jQuery as jQuery
+    qe as DataTable, Iu as
+    default, export_jQuery as jQuery
 };
 /*! Bundled license information:
 
 jszip/dist/jszip.min.js:
   (*!
   
   JSZip v3.10.1 - A JavaScript class for generating and reading zip files
@@ -16986,15 +17009,15 @@
    * Released under the MIT license
    * https://jquery.org/license
    *
    * Date: 2023-08-28T13:37Z
    *)
 
 datatables.net/js/dataTables.mjs:
-  (*! DataTables 2.0.5
+  (*! DataTables 2.0.7
    * © SpryMedia Ltd - datatables.net/license
    *)
 
 datatables.net-dt/js/dataTables.dataTables.mjs:
   (*! DataTables styling integration
    * © SpryMedia Ltd - datatables.net/license
    *)
@@ -17071,15 +17094,15 @@
 
 datatables.net-searchpanes-dt/js/searchPanes.dataTables.mjs:
   (*! Bootstrap integration for DataTables' SearchPanes
    * © SpryMedia Ltd - datatables.net/license
    *)
 
 datatables.net-select/js/dataTables.select.mjs:
-  (*! Select for DataTables 2.0.1
+  (*! Select for DataTables 2.0.2
    * © SpryMedia Ltd - datatables.net/license/mit
    *)
 
 datatables.net-select-dt/js/select.dataTables.mjs:
   (*! DataTables styling wrapper for Select
    * © SpryMedia Ltd - datatables.net/license
    *)
```

### Comparing `itables-2.0.1/itables/dt_for_itables/package-lock.json` & `itables-2.1.0rc1/packages/dt_for_itables/package-lock.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8943705234159779%*

 * *Differences: {"'packages'": "{'': {'version': '2.0.7', 'dependencies': {'datatables.net-dt': '^2.0.7', "*

 * *               "'datatables.net-select-dt': '^2.0.2'}}, 'node_modules/@esbuild/aix-ppc64': "*

 * *               "{'version': '0.21.4', 'resolved': "*

 * *               "'https://registry.npmjs.org/@esbuild/aix-ppc64/-/aix-ppc64-0.21.4.tgz', "*

 * *               "'integrity': "*

 * *               "'sha512-Zrm+B33R4LWPLjDEVnEqt2+SLTATlru1q/xYKVn8oVTbiRBGmK2VIMoIYGJDGyftnGaC788IuzGFAlb7IQ0Y8A=='}, "*

 * *               "'node_modules/@esbui […]*

```diff
@@ -2,411 +2,411 @@
     "lockfileVersion": 3,
     "name": "dt_for_itables",
     "packages": {
         "": {
             "dependencies": {
                 "datatables.net-buttons": "^3.0.1",
                 "datatables.net-buttons-dt": "^3.0.1",
-                "datatables.net-dt": "^2.0.5",
+                "datatables.net-dt": "^2.0.7",
                 "datatables.net-fixedcolumns-dt": "^5.0.0",
                 "datatables.net-keytable-dt": "^2.12.0",
                 "datatables.net-rowgroup-dt": "^1.5.0",
                 "datatables.net-searchbuilder-dt": "^1.7.0",
                 "datatables.net-searchpanes-dt": "^2.3.0",
-                "datatables.net-select-dt": "^2.0.0",
+                "datatables.net-select-dt": "^2.0.2",
                 "jquery": "^3.7.1",
                 "jszip": "^3.10.1"
             },
             "devDependencies": {
                 "esbuild": "*"
             },
             "license": "MIT",
             "name": "dt_for_itables",
-            "version": "2.0.5"
+            "version": "2.0.7"
         },
         "node_modules/@esbuild/aix-ppc64": {
             "cpu": [
                 "ppc64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-D+EBOJHXdNZcLJRBkhENNG8Wji2kgc9AZ9KiPr1JuZjsNtyHzrsfLRrY0tk2H2aoFu6RANO1y1iPPUCDYWkb5g==",
+            "integrity": "sha512-Zrm+B33R4LWPLjDEVnEqt2+SLTATlru1q/xYKVn8oVTbiRBGmK2VIMoIYGJDGyftnGaC788IuzGFAlb7IQ0Y8A==",
             "optional": true,
             "os": [
                 "aix"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/aix-ppc64/-/aix-ppc64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/aix-ppc64/-/aix-ppc64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/android-arm": {
             "cpu": [
                 "arm"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-t98Ra6pw2VaDhqNWO2Oph2LXbz/EJcnLmKLGBJwEwXX/JAN83Fym1rU8l0JUWK6HkIbWONCSSatf4sf2NBRx/w==",
+            "integrity": "sha512-E7H/yTd8kGQfY4z9t3nRPk/hrhaCajfA3YSQSBrst8B+3uTcgsi8N+ZWYCaeIDsiVs6m65JPCaQN/DxBRclF3A==",
             "optional": true,
             "os": [
                 "android"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/android-arm/-/android-arm-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/android-arm/-/android-arm-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/android-arm64": {
             "cpu": [
                 "arm64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-mRzjLacRtl/tWU0SvD8lUEwb61yP9cqQo6noDZP/O8VkwafSYwZ4yWy24kan8jE/IMERpYncRt2dw438LP3Xmg==",
+            "integrity": "sha512-fYFnz+ObClJ3dNiITySBUx+oNalYUT18/AryMxfovLkYWbutXsct3Wz2ZWAcGGppp+RVVX5FiXeLYGi97umisA==",
             "optional": true,
             "os": [
                 "android"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/android-arm64/-/android-arm64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/android-arm64/-/android-arm64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/android-x64": {
             "cpu": [
                 "x64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-btzExgV+/lMGDDa194CcUQm53ncxzeBrWJcncOBxuC6ndBkKxnHdFJn86mCIgTELsooUmwUm9FkhSp5HYu00Rg==",
+            "integrity": "sha512-mDqmlge3hFbEPbCWxp4fM6hqq7aZfLEHZAKGP9viq9wMUBVQx202aDIfc3l+d2cKhUJM741VrCXEzRFhPDKH3Q==",
             "optional": true,
             "os": [
                 "android"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/android-x64/-/android-x64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/android-x64/-/android-x64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/darwin-arm64": {
             "cpu": [
                 "arm64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-4J6IRT+10J3aJH3l1yzEg9y3wkTDgDk7TSDFX+wKFiWjqWp/iCfLIYzGyasx9l0SAFPT1HwSCR+0w/h1ES/MjA==",
+            "integrity": "sha512-72eaIrDZDSiWqpmCzVaBD58c8ea8cw/U0fq/PPOTqE3c53D0xVMRt2ooIABZ6/wj99Y+h4ksT/+I+srCDLU9TA==",
             "optional": true,
             "os": [
                 "darwin"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/darwin-arm64/-/darwin-arm64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/darwin-arm64/-/darwin-arm64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/darwin-x64": {
             "cpu": [
                 "x64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-tBcXp9KNphnNH0dfhv8KYkZhjc+H3XBkF5DKtswJblV7KlT9EI2+jeA8DgBjp908WEuYll6pF+UStUCfEpdysA==",
+            "integrity": "sha512-uBsuwRMehGmw1JC7Vecu/upOjTsMhgahmDkWhGLWxIgUn2x/Y4tIwUZngsmVb6XyPSTXJYS4YiASKPcm9Zitag==",
             "optional": true,
             "os": [
                 "darwin"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/darwin-x64/-/darwin-x64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/darwin-x64/-/darwin-x64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/freebsd-arm64": {
             "cpu": [
                 "arm64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-d3qI41G4SuLiCGCFGUrKsSeTXyWG6yem1KcGZVS+3FYlYhtNoNgYrWcvkOoaqMhwXSMrZRl69ArHsGJ9mYdbbw==",
+            "integrity": "sha512-8JfuSC6YMSAEIZIWNL3GtdUT5NhUA/CMUCpZdDRolUXNAXEE/Vbpe6qlGLpfThtY5NwXq8Hi4nJy4YfPh+TwAg==",
             "optional": true,
             "os": [
                 "freebsd"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/freebsd-arm64/-/freebsd-arm64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/freebsd-arm64/-/freebsd-arm64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/freebsd-x64": {
             "cpu": [
                 "x64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-d+DipyvHRuqEeM5zDivKV1KuXn9WeRX6vqSqIDgwIfPQtwMP4jaDsQsDncjTDDsExT4lR/91OLjRo8bmC1e+Cw==",
+            "integrity": "sha512-8d9y9eQhxv4ef7JmXny7591P/PYsDFc4+STaxC1GBv0tMyCdyWfXu2jBuqRsyhY8uL2HU8uPyscgE2KxCY9imQ==",
             "optional": true,
             "os": [
                 "freebsd"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/freebsd-x64/-/freebsd-x64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/freebsd-x64/-/freebsd-x64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/linux-arm": {
             "cpu": [
                 "arm"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-VhLPeR8HTMPccbuWWcEUD1Az68TqaTYyj6nfE4QByZIQEQVWBB8vup8PpR7y1QHL3CpcF6xd5WVBU/+SBEvGTg==",
+            "integrity": "sha512-2rqFFefpYmpMs+FWjkzSgXg5vViocqpq5a1PSRgT0AvSgxoXmGF17qfGAzKedg6wAwyM7UltrKVo9kxaJLMF/g==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/linux-arm/-/linux-arm-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/linux-arm/-/linux-arm-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/linux-arm64": {
             "cpu": [
                 "arm64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-9pb6rBjGvTFNira2FLIWqDk/uaf42sSyLE8j1rnUpuzsODBq7FvpwHYZxQ/It/8b+QOS1RYfqgGFNLRI+qlq2A==",
+            "integrity": "sha512-/GLD2orjNU50v9PcxNpYZi+y8dJ7e7/LhQukN3S4jNDXCKkyyiyAz9zDw3siZ7Eh1tRcnCHAo/WcqKMzmi4eMQ==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/linux-arm64/-/linux-arm64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/linux-arm64/-/linux-arm64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/linux-ia32": {
             "cpu": [
                 "ia32"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-o10utieEkNPFDZFQm9CoP7Tvb33UutoJqg3qKf1PWVeeJhJw0Q347PxMvBgVVFgouYLGIhFYG0UGdBumROyiig==",
+            "integrity": "sha512-pNftBl7m/tFG3t2m/tSjuYeWIffzwAZT9m08+9DPLizxVOsUl8DdFzn9HvJrTQwe3wvJnwTdl92AonY36w/25g==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/linux-ia32/-/linux-ia32-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/linux-ia32/-/linux-ia32-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/linux-loong64": {
             "cpu": [
                 "loong64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-PR7sp6R/UC4CFVomVINKJ80pMFlfDfMQMYynX7t1tNTeivQ6XdX5r2XovMmha/VjR1YN/HgHWsVcTRIMkymrgQ==",
+            "integrity": "sha512-cSD2gzCK5LuVX+hszzXQzlWya6c7hilO71L9h4KHwqI4qeqZ57bAtkgcC2YioXjsbfAv4lPn3qe3b00Zt+jIfQ==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/linux-loong64/-/linux-loong64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/linux-loong64/-/linux-loong64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/linux-mips64el": {
             "cpu": [
                 "mips64el"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-4BlTqeutE/KnOiTG5Y6Sb/Hw6hsBOZapOVF6njAESHInhlQAghVVZL1ZpIctBOoTFbQyGW+LsVYZ8lSSB3wkjA==",
+            "integrity": "sha512-qtzAd3BJh7UdbiXCrg6npWLYU0YpufsV9XlufKhMhYMJGJCdfX/G6+PNd0+v877X1JG5VmjBLUiFB0o8EUSicA==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/linux-mips64el/-/linux-mips64el-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/linux-mips64el/-/linux-mips64el-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/linux-ppc64": {
             "cpu": [
                 "ppc64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-rD3KsaDprDcfajSKdn25ooz5J5/fWBylaaXkuotBDGnMnDP1Uv5DLAN/45qfnf3JDYyJv/ytGHQaziHUdyzaAg==",
+            "integrity": "sha512-yB8AYzOTaL0D5+2a4xEy7OVvbcypvDR05MsB/VVPVA7nL4hc5w5Dyd/ddnayStDgJE59fAgNEOdLhBxjfx5+dg==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/linux-ppc64/-/linux-ppc64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/linux-ppc64/-/linux-ppc64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/linux-riscv64": {
             "cpu": [
                 "riscv64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-snwmBKacKmwTMmhLlz/3aH1Q9T8v45bKYGE3j26TsaOVtjIag4wLfWSiZykXzXuE1kbCE+zJRmwp+ZbIHinnVg==",
+            "integrity": "sha512-Y5AgOuVzPjQdgU59ramLoqSSiXddu7F3F+LI5hYy/d1UHN7K5oLzYBDZe23QmQJ9PIVUXwOdKJ/jZahPdxzm9w==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/linux-riscv64/-/linux-riscv64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/linux-riscv64/-/linux-riscv64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/linux-s390x": {
             "cpu": [
                 "s390x"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-wcWISOobRWNm3cezm5HOZcYz1sKoHLd8VL1dl309DiixxVFoFe/o8HnwuIwn6sXre88Nwj+VwZUvJf4AFxkyrQ==",
+            "integrity": "sha512-Iqc/l/FFwtt8FoTK9riYv9zQNms7B8u+vAI/rxKuN10HgQIXaPzKZc479lZ0x6+vKVQbu55GdpYpeNWzjOhgbA==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/linux-s390x/-/linux-s390x-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/linux-s390x/-/linux-s390x-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/linux-x64": {
             "cpu": [
                 "x64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-1MdwI6OOTsfQfek8sLwgyjOXAu+wKhLEoaOLTjbijk6E2WONYpH9ZU2mNtR+lZ2B4uwr+usqGuVfFT9tMtGvGw==",
+            "integrity": "sha512-Td9jv782UMAFsuLZINfUpoF5mZIbAj+jv1YVtE58rFtfvoKRiKSkRGQfHTgKamLVT/fO7203bHa3wU122V/Bdg==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/linux-x64/-/linux-x64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/linux-x64/-/linux-x64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/netbsd-x64": {
             "cpu": [
                 "x64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-K8/DhBxcVQkzYc43yJXDSyjlFeHQJBiowJ0uVL6Tor3jGQfSGHNNJcWxNbOI8v5k82prYqzPuwkzHt3J1T1iZQ==",
+            "integrity": "sha512-Awn38oSXxsPMQxaV0Ipb7W/gxZtk5Tx3+W+rAPdZkyEhQ6968r9NvtkjhnhbEgWXYbgV+JEONJ6PcdBS+nlcpA==",
             "optional": true,
             "os": [
                 "netbsd"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/netbsd-x64/-/netbsd-x64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/netbsd-x64/-/netbsd-x64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/openbsd-x64": {
             "cpu": [
                 "x64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-eMpKlV0SThJmmJgiVyN9jTPJ2VBPquf6Kt/nAoo6DgHAoN57K15ZghiHaMvqjCye/uU4X5u3YSMgVBI1h3vKrQ==",
+            "integrity": "sha512-IsUmQeCY0aU374R82fxIPu6vkOybWIMc3hVGZ3ChRwL9hA1TwY+tS0lgFWV5+F1+1ssuvvXt3HFqe8roCip8Hg==",
             "optional": true,
             "os": [
                 "openbsd"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/openbsd-x64/-/openbsd-x64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/openbsd-x64/-/openbsd-x64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/sunos-x64": {
             "cpu": [
                 "x64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-2UyFtRC6cXLyejf/YEld4Hajo7UHILetzE1vsRcGL3earZEW77JxrFjH4Ez2qaTiEfMgAXxfAZCm1fvM/G/o8w==",
+            "integrity": "sha512-hsKhgZ4teLUaDA6FG/QIu2q0rI6I36tZVfM4DBZv3BG0mkMIdEnMbhc4xwLvLJSS22uWmaVkFkqWgIS0gPIm+A==",
             "optional": true,
             "os": [
                 "sunos"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/sunos-x64/-/sunos-x64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/sunos-x64/-/sunos-x64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/win32-arm64": {
             "cpu": [
                 "arm64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-GRibxoawM9ZCnDxnP3usoUDO9vUkpAxIIZ6GQI+IlVmr5kP3zUq+l17xELTHMWTWzjxa2guPNyrpq1GWmPvcGQ==",
+            "integrity": "sha512-UUfMgMoXPoA/bvGUNfUBFLCh0gt9dxZYIx9W4rfJr7+hKe5jxxHmfOK8YSH4qsHLLN4Ck8JZ+v7Q5fIm1huErg==",
             "optional": true,
             "os": [
                 "win32"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/win32-arm64/-/win32-arm64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/win32-arm64/-/win32-arm64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/win32-ia32": {
             "cpu": [
                 "ia32"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-HfLOfn9YWmkSKRQqovpnITazdtquEW8/SoHW7pWpuEeguaZI4QnCRW6b+oZTztdBnZOS2hqJ6im/D5cPzBTTlQ==",
+            "integrity": "sha512-yIxbspZb5kGCAHWm8dexALQ9en1IYDfErzjSEq1KzXFniHv019VT3mNtTK7t8qdy4TwT6QYHI9sEZabONHg+aw==",
             "optional": true,
             "os": [
                 "win32"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/win32-ia32/-/win32-ia32-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/win32-ia32/-/win32-ia32-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/@esbuild/win32-x64": {
             "cpu": [
                 "x64"
             ],
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
-            "integrity": "sha512-N49X4lJX27+l9jbLKSqZ6bKNjzQvHaT8IIFUy+YIqmXQdjYCToGWwOItDrfby14c78aDd5NHQl29xingXfCdLQ==",
+            "integrity": "sha512-sywLRD3UK/qRJt0oBwdpYLBibk7KiRfbswmWRDabuncQYSlf8aLEEUor/oP6KRz8KEG+HoiVLBhPRD5JWjS8Sg==",
             "optional": true,
             "os": [
                 "win32"
             ],
-            "resolved": "https://registry.npmjs.org/@esbuild/win32-x64/-/win32-x64-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/@esbuild/win32-x64/-/win32-x64-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/core-util-is": {
             "integrity": "sha512-ZQBvi1DcpJ4GDqanjucZ2Hj3wEO5pZDS89BWbkcrvdxksJorwUDDZamX9ldFkp9aw2lmBDLgkObEA4DWNJ9FYQ==",
             "resolved": "https://registry.npmjs.org/core-util-is/-/core-util-is-1.0.3.tgz",
             "version": "1.0.3"
         },
         "node_modules/datatables.net": {
             "dependencies": {
                 "jquery": ">=1.7"
             },
-            "integrity": "sha512-Eu7z0ErFyr44hopfLQ7kyIWRdfqH2zFG93aHcnGKGrt/ICWXUsLrjUwghuN5b1pktnKzXCFYsl6Ad9WypiSNeA==",
-            "resolved": "https://registry.npmjs.org/datatables.net/-/datatables.net-2.0.5.tgz",
-            "version": "2.0.5"
+            "integrity": "sha512-cyW+HZwkMzb4bLrao/SS9/i64ZHiw5nYhXl+OwuOPgddG+R9O11iOEke8wYsdiyOQmjv2mE6xkEmRMZwHZc8zw==",
+            "resolved": "https://registry.npmjs.org/datatables.net/-/datatables.net-2.0.7.tgz",
+            "version": "2.0.7"
         },
         "node_modules/datatables.net-buttons": {
             "dependencies": {
                 "datatables.net": "^2",
                 "jquery": ">=1.7"
             },
             "integrity": "sha512-J+vk4hLtTivnl+RxzpKPE7CG4ggdgHPQcHnpqViy9w6ia18Uh69dQktX6NJ87QrqNPCTMUyHDzUzsRFURG4/Fw==",
@@ -421,20 +421,20 @@
             },
             "integrity": "sha512-TIzu5D81zNwcXUO6flVqDb8zKpGlhl1D2CLA8vfktMsBtFVa6xJ92rB/0np9yuFpWjkxtM3ivYLGiyWmbCF9Ow==",
             "resolved": "https://registry.npmjs.org/datatables.net-buttons-dt/-/datatables.net-buttons-dt-3.0.2.tgz",
             "version": "3.0.2"
         },
         "node_modules/datatables.net-dt": {
             "dependencies": {
-                "datatables.net": "2.0.5",
+                "datatables.net": "2.0.7",
                 "jquery": ">=1.7"
             },
-            "integrity": "sha512-YVlBgz2rg5iWCp1wvtgknfgeoyuf+7YL5cR7avP0B10E6af+sIcCzcoMiP0g6wvnoyCVhlyah8alw2wNuRrBeA==",
-            "resolved": "https://registry.npmjs.org/datatables.net-dt/-/datatables.net-dt-2.0.5.tgz",
-            "version": "2.0.5"
+            "integrity": "sha512-geClTADRyr/3B4S4eXLspidnkTzwvyLlUivYLQBlmq6M3+AAz1MI7kYXDEuOLC12Q8cvaABXFPI0oQ7Z4VZp4A==",
+            "resolved": "https://registry.npmjs.org/datatables.net-dt/-/datatables.net-dt-2.0.7.tgz",
+            "version": "2.0.7"
         },
         "node_modules/datatables.net-fixedcolumns": {
             "dependencies": {
                 "datatables.net": ">=2.0.0",
                 "jquery": ">=1.7"
             },
             "integrity": "sha512-7dTJrVDkZCicx9g//N3ufuEjvwrZpcmpjbkwrtC5LiQFCnuL/hMOiOb4CBcvTg5OiTU7VmtbBuQkeAJGs3QM5g==",
@@ -528,65 +528,65 @@
             "version": "2.3.0"
         },
         "node_modules/datatables.net-select": {
             "dependencies": {
                 "datatables.net": "^2",
                 "jquery": ">=1.7"
             },
-            "integrity": "sha512-ZrVseEmu+9cNd0PtuKpqRagwwp1K9P/JNaG6kdveCm5RzDYOqdulSB6owuIoIZwI59g9H4/d3paNl2q/wrYHZg==",
-            "resolved": "https://registry.npmjs.org/datatables.net-select/-/datatables.net-select-2.0.1.tgz",
-            "version": "2.0.1"
+            "integrity": "sha512-1dFrVfzfudFezcbFM0AE4Nj7U1JeDlffAXwaEu/Ff6O2sBYL0XrSJsz5AIkkDgJmeKeeqDH8rrc3OanFblIWKg==",
+            "resolved": "https://registry.npmjs.org/datatables.net-select/-/datatables.net-select-2.0.2.tgz",
+            "version": "2.0.2"
         },
         "node_modules/datatables.net-select-dt": {
             "dependencies": {
                 "datatables.net-dt": "^2",
-                "datatables.net-select": "2.0.1",
+                "datatables.net-select": "2.0.2",
                 "jquery": ">=1.7"
             },
-            "integrity": "sha512-QShROPJIC/Gfq+Xi7U/11yTyVSTRxf2+UYTq6B8mdLrGazJTkKT4YGOtRLLsjQchL21EisIN79TEW+v870dj9Q==",
-            "resolved": "https://registry.npmjs.org/datatables.net-select-dt/-/datatables.net-select-dt-2.0.1.tgz",
-            "version": "2.0.1"
+            "integrity": "sha512-rMqsfl6nQcmMdwU3NNNrIdkjDOGkBuKS9BZ3jin20RRfw7089ghU0M6iqhvdHPY6yvUZ9iQ0RBdaurGXRIshNA==",
+            "resolved": "https://registry.npmjs.org/datatables.net-select-dt/-/datatables.net-select-dt-2.0.2.tgz",
+            "version": "2.0.2"
         },
         "node_modules/esbuild": {
             "bin": {
                 "esbuild": "bin/esbuild"
             },
             "dev": true,
             "engines": {
                 "node": ">=12"
             },
             "hasInstallScript": true,
-            "integrity": "sha512-WdOOppmUNU+IbZ0PaDiTst80zjnrOkyJNHoKupIcVyU8Lvla3Ugx94VzkQ32Ijqd7UhHJy75gNWDMUekcrSJ6g==",
+            "integrity": "sha512-sFMcNNrj+Q0ZDolrp5pDhH0nRPN9hLIM3fRPwgbLYJeSHHgnXSnbV3xYgSVuOeLWH9c73VwmEverVzupIv5xuA==",
             "optionalDependencies": {
-                "@esbuild/aix-ppc64": "0.20.2",
-                "@esbuild/android-arm": "0.20.2",
-                "@esbuild/android-arm64": "0.20.2",
-                "@esbuild/android-x64": "0.20.2",
-                "@esbuild/darwin-arm64": "0.20.2",
-                "@esbuild/darwin-x64": "0.20.2",
-                "@esbuild/freebsd-arm64": "0.20.2",
-                "@esbuild/freebsd-x64": "0.20.2",
-                "@esbuild/linux-arm": "0.20.2",
-                "@esbuild/linux-arm64": "0.20.2",
-                "@esbuild/linux-ia32": "0.20.2",
-                "@esbuild/linux-loong64": "0.20.2",
-                "@esbuild/linux-mips64el": "0.20.2",
-                "@esbuild/linux-ppc64": "0.20.2",
-                "@esbuild/linux-riscv64": "0.20.2",
-                "@esbuild/linux-s390x": "0.20.2",
-                "@esbuild/linux-x64": "0.20.2",
-                "@esbuild/netbsd-x64": "0.20.2",
-                "@esbuild/openbsd-x64": "0.20.2",
-                "@esbuild/sunos-x64": "0.20.2",
-                "@esbuild/win32-arm64": "0.20.2",
-                "@esbuild/win32-ia32": "0.20.2",
-                "@esbuild/win32-x64": "0.20.2"
+                "@esbuild/aix-ppc64": "0.21.4",
+                "@esbuild/android-arm": "0.21.4",
+                "@esbuild/android-arm64": "0.21.4",
+                "@esbuild/android-x64": "0.21.4",
+                "@esbuild/darwin-arm64": "0.21.4",
+                "@esbuild/darwin-x64": "0.21.4",
+                "@esbuild/freebsd-arm64": "0.21.4",
+                "@esbuild/freebsd-x64": "0.21.4",
+                "@esbuild/linux-arm": "0.21.4",
+                "@esbuild/linux-arm64": "0.21.4",
+                "@esbuild/linux-ia32": "0.21.4",
+                "@esbuild/linux-loong64": "0.21.4",
+                "@esbuild/linux-mips64el": "0.21.4",
+                "@esbuild/linux-ppc64": "0.21.4",
+                "@esbuild/linux-riscv64": "0.21.4",
+                "@esbuild/linux-s390x": "0.21.4",
+                "@esbuild/linux-x64": "0.21.4",
+                "@esbuild/netbsd-x64": "0.21.4",
+                "@esbuild/openbsd-x64": "0.21.4",
+                "@esbuild/sunos-x64": "0.21.4",
+                "@esbuild/win32-arm64": "0.21.4",
+                "@esbuild/win32-ia32": "0.21.4",
+                "@esbuild/win32-x64": "0.21.4"
             },
-            "resolved": "https://registry.npmjs.org/esbuild/-/esbuild-0.20.2.tgz",
-            "version": "0.20.2"
+            "resolved": "https://registry.npmjs.org/esbuild/-/esbuild-0.21.4.tgz",
+            "version": "0.21.4"
         },
         "node_modules/immediate": {
             "integrity": "sha512-XXOFtyqDjNDAQxVfYxuF7g9Il/IbWmmlQg2MYKOH8ExIT1qg6xc4zyS3HaEEATgs1btfzxq15ciUiY7gjSXRGQ==",
             "resolved": "https://registry.npmjs.org/immediate/-/immediate-3.0.6.tgz",
             "version": "3.0.6"
         },
         "node_modules/inherits": {
@@ -668,9 +668,9 @@
         "node_modules/util-deprecate": {
             "integrity": "sha512-EPD5q1uXyFxJpCrLnCc1nHnq3gOa6DZBocAIiI2TaSCA7VCJ1UJDMagCzIkXNsUYfD1daK//LTEQ8xiIbrHtcw==",
             "resolved": "https://registry.npmjs.org/util-deprecate/-/util-deprecate-1.0.2.tgz",
             "version": "1.0.2"
         }
     },
     "requires": true,
-    "version": "2.0.5"
+    "version": "2.0.7"
 }
```

### Comparing `itables-2.0.1/itables/dt_for_itables/package.json` & `itables-2.1.0rc1/packages/dt_for_itables/package.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7948232323232324%*

 * *Differences: {"'dependencies'": "{'datatables.net-dt': '^2.0.7', 'datatables.net-select-dt': '^2.0.2'}",*

 * * "'main'": "'src/index.js'",*

 * * "'scripts'": "{'build': 'npm run build:js && npm run install:js', 'build:js': 'esbuild "*

 * *              "src/index.js --format=esm --bundle --outfile=dt_bundle.js --minify', 'install:js': "*

 * *              "'cp dt_bundle.js dt_bundle.css  ../../src/itables/html'}",*

 * * "'typings'": "'src/index.d.js'",*

 * * "'version'": "'2.0.7'"}*

```diff
@@ -1,32 +1,35 @@
 {
     "author": "Marc Wouts",
     "dependencies": {
         "datatables.net-buttons": "^3.0.1",
         "datatables.net-buttons-dt": "^3.0.1",
-        "datatables.net-dt": "^2.0.5",
+        "datatables.net-dt": "^2.0.7",
         "datatables.net-fixedcolumns-dt": "^5.0.0",
         "datatables.net-keytable-dt": "^2.12.0",
         "datatables.net-rowgroup-dt": "^1.5.0",
         "datatables.net-searchbuilder-dt": "^1.7.0",
         "datatables.net-searchpanes-dt": "^2.3.0",
-        "datatables.net-select-dt": "^2.0.0",
+        "datatables.net-select-dt": "^2.0.2",
         "jquery": "^3.7.1",
         "jszip": "^3.10.1"
     },
     "description": "DataTables bundle for itables",
     "devDependencies": {
         "esbuild": "*"
     },
     "homepage": "https://mwouts.github.io/itables",
     "license": "MIT",
-    "main": "src.js",
+    "main": "src/index.js",
     "name": "dt_for_itables",
     "repository": {
         "type": "git",
         "url": "https://github.com/mwouts/itables.git"
     },
     "scripts": {
-        "build": "esbuild src.js --format=esm --bundle --outfile=dt_bundle.js --minify"
+        "build": "npm run build:js && npm run install:js",
+        "build:js": "esbuild src/index.js --format=esm --bundle --outfile=dt_bundle.js --minify",
+        "install:js": "cp dt_bundle.js dt_bundle.css  ../../src/itables/html"
     },
-    "version": "2.0.5"
+    "typings": "src/index.d.js",
+    "version": "2.0.7"
 }
```

### Comparing `itables-2.0.1/itables/dt_for_itables/src.js` & `itables-2.1.0rc1/packages/dt_for_itables/src/index.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -27,8 +27,10 @@
 
 import 'datatables.net-select-dt';
 import 'datatables.net-select-dt/css/select.dataTables.min.css';
 
 export {
     DataTable,
     jQuery
-};
+};
+
+export default DataTable;
```

### Comparing `itables-2.0.1/itables/html/datatables_template.html` & `itables-2.1.0rc1/src/itables/html/datatables_template.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <table id="table_id"><thead><tr><th>A</th></tr></thead></table>
-<link href="https://www.unpkg.com/dt_for_itables@2.0.5/dt_bundle.css" rel="stylesheet">
+<link href="https://www.unpkg.com/dt_for_itables@2.0.7/dt_bundle.css" rel="stylesheet">
 <script type="module">
-    import {DataTable, jQuery as $} from 'https://www.unpkg.com/dt_for_itables@2.0.5/dt_bundle.js';
+    import {DataTable, jQuery as $} from 'https://www.unpkg.com/dt_for_itables@2.0.7/dt_bundle.js';
 
     document.querySelectorAll("#table_id:not(.dataTable)").forEach(table => {
         // Define the table data
         const data = [];
 
         // Define the dt_args
         let dt_args = {};
```

### Comparing `itables-2.0.1/itables/logo/loading.svg` & `itables-2.1.0rc1/src/itables/logo/loading.svg`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/itables/logo/logo.svg` & `itables-2.1.0rc1/src/itables/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/itables/logo/text.svg` & `itables-2.1.0rc1/src/itables/logo/text.svg`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/itables/logo/wide.svg` & `itables-2.1.0rc1/src/itables/logo/wide.svg`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/itables/logo/with_text.svg` & `itables-2.1.0rc1/src/itables/logo/with_text.svg`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/itables/samples/countries.csv` & `itables-2.1.0rc1/src/itables/samples/countries.csv`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/itables/samples/indicators.csv` & `itables-2.1.0rc1/src/itables/samples/indicators.csv`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/itables/samples/population.csv` & `itables-2.1.0rc1/src/itables/samples/population.csv`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/tests/conftest.py` & `itables-2.1.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/tests/test_changelog.py` & `itables-2.1.0rc1/tests/test_changelog.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/tests/test_connected_notebook_is_small.py` & `itables-2.1.0rc1/tests/test_connected_notebook_is_small.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/tests/test_datatables_format.py` & `itables-2.1.0rc1/tests/test_datatables_format.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/tests/test_documentation_notebooks_run.py` & `itables-2.1.0rc1/tests/test_documentation_notebooks_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 from pathlib import Path
 
 import jupytext
 import pytest
 
+import itables.options as opt
 from itables import init_notebook_mode
 from itables.javascript import pd_style
 
 try:
     import polars as pl
 except ImportError:
     pl = None
@@ -27,13 +28,19 @@
 )
 def test_run_documentation_notebooks(notebook):
     if "polars" in notebook.stem and pl is None:
         pytest.skip("Polars is not available")
     if "pandas_style" in notebook.stem and pd_style is None:
         pytest.skip("Pandas Style is not available")
 
+    org_options = dir(opt)
+
     nb = jupytext.read(notebook)
     py_notebook = jupytext.writes(nb, "py:percent")
     exec(py_notebook, {})
 
+    new_options = set(dir(opt)).difference(org_options)
+    for name in new_options:
+        delattr(opt, name)
+
     # Revert back to the non initialized mode
     init_notebook_mode(all_interactive=False, connected=True)
```

### Comparing `itables-2.0.1/tests/test_downsample.py` & `itables-2.1.0rc1/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/tests/test_javascript.py` & `itables-2.1.0rc1/tests/test_javascript.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 @pytest.mark.parametrize("url", [UNPKG_DT_BUNDLE_URL, UNPKG_DT_BUNDLE_CSS])
 def test_unpkg_links(url):
     response = requests.get(url)
     assert response.ok, url
 
 
 def test_unpkg_urls_are_up_to_date():
-    with open(Path(__file__).parent / "../itables/dt_for_itables/package.json") as fp:
+    with open(Path(__file__).parent / "../packages/dt_for_itables/package.json") as fp:
         dt_for_itables = json.load(fp)
     bundle_version = dt_for_itables["version"]
     assert (
         UNPKG_DT_BUNDLE_URL
         == f"https://www.unpkg.com/dt_for_itables@{bundle_version}/dt_bundle.js"
     )
     assert (
```

### Comparing `itables-2.0.1/tests/test_json_dumps.py` & `itables-2.1.0rc1/tests/test_json_dumps.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/tests/test_notebook.ipynb` & `itables-2.1.0rc1/tests/test_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/tests/test_pandas_style.py` & `itables-2.1.0rc1/tests/test_pandas_style.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/tests/test_polars.py` & `itables-2.1.0rc1/tests/test_polars.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/tests/test_sample_dfs.py` & `itables-2.1.0rc1/tests/test_sample_dfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,24 +72,24 @@
 
 
 def test_show_test_dfs(df, connected, use_to_html, lengthMenu, monkeypatch):
     show(
         df,
         connected=connected,
         use_to_html=use_to_html,
-        **kwargs_remove_none(lengthMenu=lengthMenu)
+        **kwargs_remove_none(lengthMenu=lengthMenu),
     )
 
 
 def test_to_html_datatable(df, connected, use_to_html, lengthMenu, monkeypatch):
     html = to_html_datatable(
         df,
         connected=connected,
         use_to_html=use_to_html,
-        **kwargs_remove_none(lengthMenu=lengthMenu)
+        **kwargs_remove_none(lengthMenu=lengthMenu),
     )
     if use_to_html:
         assert "quarto" not in html
     else:
         assert 'data-quarto-disable-processing="true"' in html
```

### Comparing `itables-2.0.1/tests/test_sample_python_apps.py` & `itables-2.1.0rc1/tests/test_sample_python_apps.py`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/tests/test_update_samples.py` & `itables-2.1.0rc1/tests/test_update_samples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 import world_bank_data as wb
 
-SAMPLE_DIR = Path(__file__).parent / ".." / "itables" / "samples"
+SAMPLE_DIR = Path(__file__).parent / ".." / "src" / "itables" / "samples"
 
 
 def create_csv_file_if_missing(df, csv_file):
     if not csv_file.exists():
         with open(str(csv_file), "w") as fp:  # pragma: no cover
             fp.write(df.to_csv())
```

### Comparing `itables-2.0.1/LICENSE` & `itables-2.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `itables-2.0.1/README.md` & `itables-2.1.0rc1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![ITables Logo](itables/logo/wide.svg)
+![ITables logo](https://raw.githubusercontent.com/mwouts/itables/3f8e8bd75af7ad38a500518fcb4fbbc370ea6c4c/itables/logo/wide.svg)
 
 ![CI](https://github.com/mwouts/itables/actions/workflows/continuous-integration.yml/badge.svg?branch=main)
 [![codecov.io](https://codecov.io/github/mwouts/itables/coverage.svg?branch=main)](https://codecov.io/github/mwouts/itables?branch=main)
 [![Pypi](https://img.shields.io/pypi/v/itables.svg)](https://pypi.python.org/pypi/itables)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/itables.svg)](https://anaconda.org/conda-forge/itables)
 [![pyversions](https://img.shields.io/pypi/pyversions/itables.svg)](https://pypi.python.org/pypi/itables)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `itables-2.0.1/pyproject.toml` & `itables-2.1.0rc1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -46,15 +46,15 @@
   # Shiny test app
   "shiny",
   # Test urls
   "requests",
 ]
 
 [tool.hatch.version]
-path = "itables/version.py"
+path = "src/itables/version.py"
 
 [project.urls]
 Homepage = "https://mwouts.github.io/itables/"
 Documentation = "https://mwouts.github.io/itables"
 Repository = "https://github.com/mwouts/itables.git"
 Issues = "https://github.com/mwouts/itables/issues"
 Changelog = "https://github.com/mwouts/itables/blob/main/docs/changelog.md"
@@ -72,19 +72,23 @@
     "except ImportError",
   ]
 
 [tool.hatch.build.hooks.jupyter-builder]
 enable-by-default = true
 dependencies = ["hatch-jupyter-builder"]
 build-function = "hatch_jupyter_builder.npm_builder"
-ensured-targets = ["itables/dt_for_itables/dt_bundle.js", "itables/dt_for_itables/dt_bundle.css"]
+ensured-targets = [
+    "src/itables/html/dt_bundle.js",
+    "src/itables/html/dt_bundle.css",
+    "src/itables/itables_for_streamlit/asset-manifest.json"
+    ]
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
-path = "itables/dt_for_itables"
+path = "packages"
 build_cmd = "build"
 npm = ["npm"]
 
 [tool.hatch.build.targets.sdist]
-artifacts = ["itables/dt_for_itables/dt_bundle.js", "itables/dt_for_itables/dt_bundle.css"]
+artifacts = ["src/itables/html/dt_bundle.js", "src/itables/html/dt_bundle.css"]
 
 [tool.hatch.build.targets.wheel]
-artifacts = ["itables/dt_for_itables/dt_bundle.js", "itables/dt_for_itables/dt_bundle.css"]
+artifacts = ["src/itables/html/dt_bundle.js", "src/itables/html/dt_bundle.css"]
```

### Comparing `itables-2.0.1/PKG-INFO` & `itables-2.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: itables
-Version: 2.0.1
+Version: 2.1.0rc1
 Summary: Pandas and Polar DataFrames as interactive DataTables
 Project-URL: Homepage, https://mwouts.github.io/itables/
 Project-URL: Documentation, https://mwouts.github.io/itables
 Project-URL: Repository, https://github.com/mwouts/itables.git
 Project-URL: Issues, https://github.com/mwouts/itables/issues
 Project-URL: Changelog, https://github.com/mwouts/itables/blob/main/docs/changelog.md
 Author-email: Marc Wouts <marc.wouts@gmail.com>
@@ -74,15 +74,15 @@
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytz; extra == 'test'
 Requires-Dist: requests; extra == 'test'
 Requires-Dist: shiny; extra == 'test'
 Requires-Dist: world-bank-data; extra == 'test'
 Description-Content-Type: text/markdown
 
-![ITables Logo](itables/logo/wide.svg)
+![ITables logo](https://raw.githubusercontent.com/mwouts/itables/3f8e8bd75af7ad38a500518fcb4fbbc370ea6c4c/itables/logo/wide.svg)
 
 ![CI](https://github.com/mwouts/itables/actions/workflows/continuous-integration.yml/badge.svg?branch=main)
 [![codecov.io](https://codecov.io/github/mwouts/itables/coverage.svg?branch=main)](https://codecov.io/github/mwouts/itables?branch=main)
 [![Pypi](https://img.shields.io/pypi/v/itables.svg)](https://pypi.python.org/pypi/itables)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/itables.svg)](https://anaconda.org/conda-forge/itables)
 [![pyversions](https://img.shields.io/pypi/pyversions/itables.svg)](https://pypi.python.org/pypi/itables)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

