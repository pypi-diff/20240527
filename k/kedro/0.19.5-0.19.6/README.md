# Comparing `tmp/kedro-0.19.5.tar.gz` & `tmp/kedro-0.19.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-0.19.5.tar", last modified: Mon Apr 22 14:50:00 2024, max compression
+gzip compressed data, was "kedro-0.19.6.tar", last modified: Mon May 27 16:32:36 2024, max compression
```

## Comparing `kedro-0.19.5.tar` & `kedro-0.19.6.tar`

### file list

```diff
@@ -1,156 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.446335 kedro-0.19.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 14:49:52.000000 kedro-0.19.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-22 14:49:52.000000 kedro-0.19.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-04-22 14:50:00.446335 kedro-0.19.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-22 14:49:52.000000 kedro-0.19.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.426335 kedro-0.19.5/kedro/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.426335 kedro-0.19.5/kedro/config/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/config/abstract_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19977 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/config/omegaconf_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.426335 kedro-0.19.5/kedro/framework/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.430335 kedro-0.19.5/kedro/framework/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/cli/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     8286 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.430335 kedro-0.19.5/kedro/framework/cli/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/cli/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/cli/hooks/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/cli/hooks/markers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/cli/hooks/specs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/cli/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)    35330 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/cli/micropkg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/cli/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/cli/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/cli/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    37263 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/cli/starters.py
--rw-r--r--   0 runner    (1001) docker     (127)    16788 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.430335 kedro-0.19.5/kedro/framework/context/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11093 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/context/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.430335 kedro-0.19.5/kedro/framework/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/hooks/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/hooks/markers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/hooks/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.434335 kedro-0.19.5/kedro/framework/project/
--rw-r--r--   0 runner    (1001) docker     (127)    15688 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/project/default_logging.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.434335 kedro-0.19.5/kedro/framework/session/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/session/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/session/shelvestore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/session/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/framework/startup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.434335 kedro-0.19.5/kedro/io/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/io/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    27679 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/io/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    28395 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/io/data_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/io/lambda_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/io/memory_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/io/shared_memory_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.434335 kedro-0.19.5/kedro/ipython/
--rw-r--r--   0 runner    (1001) docker     (127)    14517 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/ipython/logo-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/ipython/logo-64x64.png
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/ipython/logo-svg.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.434335 kedro-0.19.5/kedro/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/pipeline/_transcoding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12464 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/pipeline/modular_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    25777 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/pipeline/node.py
--rw-r--r--   0 runner    (1001) docker     (127)    32689 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.438335 kedro-0.19.5/kedro/runner/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/runner/parallel_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    20053 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/runner/sequential_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/runner/thread_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.422335 kedro-0.19.5/kedro/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.438335 kedro-0.19.5/kedro/templates/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/pipeline/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.438335 kedro-0.19.5/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.438335 kedro-0.19.5/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/parameters_{{ cookiecutter.pipeline_name }}.yml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.438335 kedro-0.19.5/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/test_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.438335 kedro-0.19.5/kedro/templates/project/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.438335 kedro-0.19.5/kedro/templates/project/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/hooks/post_gen_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/hooks/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/prompts.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.438335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.438335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.438335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.438335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/credentials.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/logging.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.422335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.438335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/01_raw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.442335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/02_intermediate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.442335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/03_primary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.442335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.442335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.442335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.442335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.442335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.422335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.442335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.442335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.422335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.442335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.442335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.442335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.442335 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-22 14:49:52.000000 kedro-0.19.5/kedro/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.442335 kedro-0.19.5/kedro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-04-22 14:50:00.000000 kedro-0.19.5/kedro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-22 14:50:00.000000 kedro-0.19.5/kedro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 14:50:00.000000 kedro-0.19.5/kedro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 14:50:00.000000 kedro-0.19.5/kedro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 14:49:55.000000 kedro-0.19.5/kedro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-22 14:50:00.000000 kedro-0.19.5/kedro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 14:50:00.000000 kedro-0.19.5/kedro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-22 14:49:52.000000 kedro-0.19.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 14:50:00.446335 kedro-0.19.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:50:00.442335 kedro-0.19.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-22 14:49:52.000000 kedro-0.19.5/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-22 14:49:52.000000 kedro-0.19.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.421738 kedro-0.19.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 16:32:25.000000 kedro-0.19.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-27 16:32:25.000000 kedro-0.19.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13277 2024-05-27 16:32:36.421738 kedro-0.19.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-05-27 16:32:25.000000 kedro-0.19.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.401739 kedro-0.19.6/kedro/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.405739 kedro-0.19.6/kedro/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/config/abstract_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19977 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/config/omegaconf_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.405739 kedro-0.19.6/kedro/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.405739 kedro-0.19.6/kedro/framework/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/cli/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8286 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.405739 kedro-0.19.6/kedro/framework/cli/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/cli/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/cli/hooks/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/cli/hooks/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/cli/hooks/specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/cli/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35895 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/cli/micropkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/cli/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/cli/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/cli/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37263 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/cli/starters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16788 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.405739 kedro-0.19.6/kedro/framework/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11092 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.409739 kedro-0.19.6/kedro/framework/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/hooks/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/hooks/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/hooks/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.409739 kedro-0.19.6/kedro/framework/project/
+-rw-r--r--   0 runner    (1001) docker     (127)    17798 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/project/default_logging.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/project/rich_logging.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.409739 kedro-0.19.6/kedro/framework/session/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/session/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/session/shelvestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/session/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/framework/startup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.409739 kedro-0.19.6/kedro/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/io/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27679 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/io/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29669 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/io/data_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/io/lambda_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/io/memory_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/io/shared_memory_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.409739 kedro-0.19.6/kedro/ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)    14884 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/ipython/logo-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/ipython/logo-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/ipython/logo-svg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.409739 kedro-0.19.6/kedro/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/pipeline/modular_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25776 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/pipeline/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33137 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/pipeline/transcoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.413739 kedro-0.19.6/kedro/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/runner/parallel_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20053 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/runner/sequential_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/runner/thread_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.401739 kedro-0.19.6/kedro/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.413739 kedro-0.19.6/kedro/templates/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/pipeline/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.413739 kedro-0.19.6/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.413739 kedro-0.19.6/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/parameters_{{ cookiecutter.pipeline_name }}.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.413739 kedro-0.19.6/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.413739 kedro-0.19.6/kedro/templates/project/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.413739 kedro-0.19.6/kedro/templates/project/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/hooks/post_gen_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/hooks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/prompts.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.413739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.413739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.413739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.413739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/credentials.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/logging.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.401739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.413739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/01_raw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.413739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/02_intermediate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.417739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/03_primary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.417739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.417739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.417739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.417739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.417739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.401739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.417739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.417739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.401739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.417739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.417739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.417739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.417739 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-27 16:32:25.000000 kedro-0.19.6/kedro/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.417739 kedro-0.19.6/kedro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13277 2024-05-27 16:32:36.000000 kedro-0.19.6/kedro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-27 16:32:36.000000 kedro-0.19.6/kedro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:32:36.000000 kedro-0.19.6/kedro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-27 16:32:36.000000 kedro-0.19.6/kedro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:32:31.000000 kedro-0.19.6/kedro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-27 16:32:36.000000 kedro-0.19.6/kedro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 16:32:36.000000 kedro-0.19.6/kedro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-27 16:32:25.000000 kedro-0.19.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:32:36.421738 kedro-0.19.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:32:36.417739 kedro-0.19.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-27 16:32:25.000000 kedro-0.19.6/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-27 16:32:25.000000 kedro-0.19.6/tests/test_utils.py
```

### Comparing `kedro-0.19.5/LICENSE.md` & `kedro-0.19.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/PKG-INFO` & `kedro-0.19.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro
-Version: 0.19.5
+Version: 0.19.6
 Summary: Kedro helps you build production-ready data and analytics pipelines
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://kedro.org
 Project-URL: Source, https://github.com/kedro-org/kedro
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro/issues
@@ -26,15 +26,15 @@
 Requires-Dist: fsspec>=2021.4
 Requires-Dist: gitpython>=3.0
 Requires-Dist: importlib-metadata<8.0,>=3.6; python_version >= "3.8"
 Requires-Dist: importlib_resources<7.0,>=1.3
 Requires-Dist: more_itertools>=8.14.0
 Requires-Dist: omegaconf>=2.1.1
 Requires-Dist: parse>=1.19.0
-Requires-Dist: pluggy<1.4.0,>=1.0
+Requires-Dist: pluggy>=1.0
 Requires-Dist: pre-commit-hooks
 Requires-Dist: PyYAML<7.0,>=4.2
 Requires-Dist: rich<14.0,>=12.0
 Requires-Dist: rope<2.0,>=0.21
 Requires-Dist: toml>=0.10.0
 Requires-Dist: graphlib_backport>=1.0.0; python_version < "3.9"
 Provides-Extra: test
@@ -47,21 +47,21 @@
 Requires-Dist: jupyterlab_server>=2.11.1; extra == "test"
 Requires-Dist: jupyterlab<5,>=3; extra == "test"
 Requires-Dist: jupyter~=1.0; extra == "test"
 Requires-Dist: kedro-datasets; python_version >= "3.9" and extra == "test"
 Requires-Dist: kedro-datasets<2.0.0; python_version < "3.9" and extra == "test"
 Requires-Dist: mypy~=1.0; extra == "test"
 Requires-Dist: pandas~=2.0; extra == "test"
-Requires-Dist: pluggy<1.4,>=1.0; extra == "test"
+Requires-Dist: pluggy>=1.0; extra == "test"
 Requires-Dist: pre-commit<4.0,>=2.9.2; extra == "test"
 Requires-Dist: pytest-cov~=3.0; extra == "test"
 Requires-Dist: pytest-mock<4.0,>=1.7.1; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=2.2.1; extra == "test"
 Requires-Dist: pytest<9.0,>=7.2; extra == "test"
-Requires-Dist: s3fs<2024.4,>=2021.4; extra == "test"
+Requires-Dist: s3fs<2024.6,>=2021.4; extra == "test"
 Requires-Dist: trufflehog~=2.1; extra == "test"
 Requires-Dist: pandas-stubs; extra == "test"
 Requires-Dist: types-PyYAML; extra == "test"
 Requires-Dist: types-cachetools; extra == "test"
 Requires-Dist: types-toml; extra == "test"
 Provides-Extra: docs
 Requires-Dist: kedro-sphinx-theme==2024.4.0; extra == "docs"
@@ -71,15 +71,15 @@
 Requires-Dist: ipylab>=1.0.0; extra == "jupyter"
 Requires-Dist: notebook>=7.0.0; extra == "jupyter"
 Provides-Extra: all
 Requires-Dist: kedro[docs,jupyter,test]; extra == "all"
 
 ![Kedro Logo Banner - Light](https://raw.githubusercontent.com/kedro-org/kedro/main/.github/demo-dark.png#gh-dark-mode-only)
 ![Kedro Logo Banner - Dark](https://raw.githubusercontent.com/kedro-org/kedro/main/.github/demo-light.png#gh-light-mode-only)
-[![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://pypi.org/project/kedro/)
+[![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg)](https://pypi.org/project/kedro/)
 [![PyPI version](https://badge.fury.io/py/kedro.svg)](https://pypi.org/project/kedro/)
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/kedro.svg)](https://anaconda.org/conda-forge/kedro)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/kedro-org/kedro/blob/main/LICENSE.md)
 [![Slack Organisation](https://img.shields.io/badge/slack-chat-blueviolet.svg?label=Kedro%20Slack&logo=slack)](https://slack.kedro.org)
 [![Slack Archive](https://img.shields.io/badge/slack-archive-blueviolet.svg?label=Kedro%20Slack%20)](https://linen-slack.kedro.org/)
 ![GitHub Actions Workflow Status - Main](https://img.shields.io/github/actions/workflow/status/kedro-org/kedro/all-checks.yml?label=main)
 ![GitHub Actions Workflow Status - Develop](https://img.shields.io/github/actions/workflow/status/kedro-org/kedro/all-checks.yml?branch=develop&label=develop)
```

### Comparing `kedro-0.19.5/README.md` & `kedro-0.19.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![Kedro Logo Banner - Light](https://raw.githubusercontent.com/kedro-org/kedro/main/.github/demo-dark.png#gh-dark-mode-only)
 ![Kedro Logo Banner - Dark](https://raw.githubusercontent.com/kedro-org/kedro/main/.github/demo-light.png#gh-light-mode-only)
-[![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://pypi.org/project/kedro/)
+[![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg)](https://pypi.org/project/kedro/)
 [![PyPI version](https://badge.fury.io/py/kedro.svg)](https://pypi.org/project/kedro/)
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/kedro.svg)](https://anaconda.org/conda-forge/kedro)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/kedro-org/kedro/blob/main/LICENSE.md)
 [![Slack Organisation](https://img.shields.io/badge/slack-chat-blueviolet.svg?label=Kedro%20Slack&logo=slack)](https://slack.kedro.org)
 [![Slack Archive](https://img.shields.io/badge/slack-archive-blueviolet.svg?label=Kedro%20Slack%20)](https://linen-slack.kedro.org/)
 ![GitHub Actions Workflow Status - Main](https://img.shields.io/github/actions/workflow/status/kedro-org/kedro/all-checks.yml?label=main)
 ![GitHub Actions Workflow Status - Develop](https://img.shields.io/github/actions/workflow/status/kedro-org/kedro/all-checks.yml?branch=develop&label=develop)
```

### Comparing `kedro-0.19.5/kedro/__init__.py` & `kedro-0.19.6/kedro/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 data pipelines by providing uniform project templates, data abstraction,
 configuration and pipeline assembly.
 """
 
 import sys
 import warnings
 
-__version__ = "0.19.5"
+__version__ = "0.19.6"
 
 
 class KedroDeprecationWarning(DeprecationWarning):
     """Custom class for warnings about deprecated Kedro features."""
 
 
 class KedroPythonVersionWarning(UserWarning):
```

### Comparing `kedro-0.19.5/kedro/config/abstract_config.py` & `kedro-0.19.6/kedro/config/abstract_config.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/config/omegaconf_config.py` & `kedro-0.19.6/kedro/config/omegaconf_config.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/framework/cli/catalog.py` & `kedro-0.19.6/kedro/framework/cli/catalog.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,18 +83,20 @@
         used_ds = catalog_ds - unused_ds
 
         # resolve any factory datasets in the pipeline
         factory_ds_by_type = defaultdict(list)
         for ds_name in default_ds:
             matched_pattern = data_catalog._match_pattern(
                 data_catalog._dataset_patterns, ds_name
-            )
+            ) or data_catalog._match_pattern(data_catalog._default_pattern, ds_name)
             if matched_pattern:
                 ds_config_copy = copy.deepcopy(
-                    data_catalog._dataset_patterns[matched_pattern]
+                    data_catalog._dataset_patterns.get(matched_pattern)
+                    or data_catalog._default_pattern.get(matched_pattern)
+                    or {}
                 )
 
                 ds_config = data_catalog._resolve_config(
                     ds_name, matched_pattern, ds_config_copy
                 )
                 factory_ds_by_type[ds_config["type"]].append(ds_name)
 
@@ -211,15 +213,18 @@
 @env_option
 @click.pass_obj
 def rank_catalog_factories(metadata: ProjectMetadata, env: str) -> None:
     """List all dataset factories in the catalog, ranked by priority by which they are matched."""
     session = _create_session(metadata.package_name, env=env)
     context = session.load_context()
 
-    catalog_factories = context.catalog._dataset_patterns
+    catalog_factories = {
+        **context.catalog._dataset_patterns,
+        **context.catalog._default_pattern,
+    }
     if catalog_factories:
         click.echo(yaml.dump(list(catalog_factories.keys())))
     else:
         click.echo("There are no dataset factories in the catalog.")
 
 
 @catalog.command("resolve")
@@ -255,18 +260,20 @@
     for ds_name in datasets:
         is_param = ds_name.startswith("params:") or ds_name == "parameters"
         if ds_name in explicit_datasets or is_param:
             continue
 
         matched_pattern = data_catalog._match_pattern(
             data_catalog._dataset_patterns, ds_name
-        )
+        ) or data_catalog._match_pattern(data_catalog._default_pattern, ds_name)
         if matched_pattern:
             ds_config_copy = copy.deepcopy(
-                data_catalog._dataset_patterns[matched_pattern]
+                data_catalog._dataset_patterns.get(matched_pattern)
+                or data_catalog._default_pattern.get(matched_pattern)
+                or {}
             )
 
             ds_config = data_catalog._resolve_config(
                 ds_name, matched_pattern, ds_config_copy
             )
             explicit_datasets[ds_name] = ds_config
```

### Comparing `kedro-0.19.5/kedro/framework/cli/cli.py` & `kedro-0.19.6/kedro/framework/cli/cli.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/framework/cli/hooks/manager.py` & `kedro-0.19.6/kedro/framework/cli/hooks/manager.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/framework/cli/hooks/specs.py` & `kedro-0.19.6/kedro/framework/cli/hooks/specs.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/framework/cli/jupyter.py` & `kedro-0.19.6/kedro/framework/cli/jupyter.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/framework/cli/micropkg.py` & `kedro-0.19.6/kedro/framework/cli/micropkg.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,16 @@
 @click.group(name="Kedro")
 def micropkg_cli() -> None:  # pragma: no cover
     pass
 
 
 @micropkg_cli.group()
 def micropkg() -> None:
-    """Commands for working with micro-packages."""
+    """(DEPRECATED) Commands for working with micro-packages. DeprecationWarning: micro-packaging is deprecated
+    and will not be available from Kedro 0.20.0."""
 
 
 @command_with_verbosity(micropkg, "pull")
 @click.argument("package_path", nargs=1, required=False)
 @click.option(
     "--all",
     "-a",
@@ -163,15 +164,21 @@
     env: str,
     alias: str,
     destination: str,
     fs_args: str,
     all_flag: str,
     **kwargs: Any,
 ) -> None:
-    """Pull and unpack a modular pipeline and other micro-packages in your project."""
+    """(DEPRECATED) Pull and unpack a modular pipeline and other micro-packages in your project."""
+    deprecation_message = (
+        "DeprecationWarning: Command 'kedro micropkg pull' is deprecated and "
+        "will not be available from Kedro 0.20.0."
+    )
+    click.secho(deprecation_message, fg="red")
+
     if not package_path and not all_flag:
         click.secho(
             "Please specify a package path or add '--all' to pull all micro-packages in the "
             "'pyproject.toml' package manifest section."
         )
         sys.exit(1)
 
@@ -337,15 +344,21 @@
     module_path: str,
     env: str,
     alias: str,
     destination: str,
     all_flag: str,
     **kwargs: Any,
 ) -> None:
-    """Package up a modular pipeline or micro-package as a Python source distribution."""
+    """(DEPRECATED) Package up a modular pipeline or micro-package as a Python source distribution."""
+    deprecation_message = (
+        "DeprecationWarning: Command 'kedro micropkg package' is deprecated and "
+        "will not be available from Kedro 0.20.0."
+    )
+    click.secho(deprecation_message, fg="red")
+
     if not module_path and not all_flag:
         click.secho(
             "Please specify a micro-package name or add '--all' to package all micro-packages in "
             "the 'pyproject.toml' package manifest section."
         )
         sys.exit(1)
```

### Comparing `kedro-0.19.5/kedro/framework/cli/pipeline.py` & `kedro-0.19.6/kedro/framework/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/framework/cli/project.py` & `kedro-0.19.6/kedro/framework/cli/project.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/framework/cli/registry.py` & `kedro-0.19.6/kedro/framework/cli/registry.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/framework/cli/starters.py` & `kedro-0.19.6/kedro/framework/cli/starters.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/framework/cli/utils.py` & `kedro-0.19.6/kedro/framework/cli/utils.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/framework/context/context.py` & `kedro-0.19.6/kedro/framework/context/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from attrs import define, field
 from omegaconf import OmegaConf
 from pluggy import PluginManager
 
 from kedro.config import AbstractConfigLoader, MissingConfigException
 from kedro.framework.project import settings
 from kedro.io import DataCatalog
-from kedro.pipeline._transcoding import _transcode_split
+from kedro.pipeline.transcoding import _transcode_split
 
 
 def _is_relative_path(path_string: str) -> bool:
     """Checks whether a path string is a relative path.
 
     Example:
     ::
```

### Comparing `kedro-0.19.5/kedro/framework/hooks/manager.py` & `kedro-0.19.6/kedro/framework/hooks/manager.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/framework/hooks/specs.py` & `kedro-0.19.6/kedro/framework/hooks/specs.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/framework/project/__init__.py` & `kedro-0.19.6/kedro/framework/project/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -212,21 +212,49 @@
     __repr__ = _load_data_wrapper(repr)
     __str__ = _load_data_wrapper(str)
 
 
 class _ProjectLogging(UserDict):
     def __init__(self) -> None:
         """Initialise project logging. The path to logging configuration is given in
-        environment variable KEDRO_LOGGING_CONFIG (defaults to default_logging.yml)."""
-        path = os.environ.get(
-            "KEDRO_LOGGING_CONFIG", Path(__file__).parent / "default_logging.yml"
-        )
+        environment variable KEDRO_LOGGING_CONFIG (defaults to conf/logging.yml)."""
+
+        # Check if a user path is set in the environment variable
+        user_logging_path = os.environ.get("KEDRO_LOGGING_CONFIG")
+
+        # Check if the default logging configuration exists
+        default_logging_path = Path("conf/logging.yml")
+        if not default_logging_path.exists():
+            default_logging_path = Path(
+                os.environ.get(
+                    "KEDRO_LOGGING_CONFIG",
+                    Path(__file__).parent / "rich_logging.yml"
+                    if importlib.util.find_spec("rich")
+                    else Path(__file__).parent / "default_logging.yml",
+                )
+            )
+
+        # Use the user path if available, otherwise, use the default path
+        if user_logging_path and Path(user_logging_path).exists():
+            path = Path(user_logging_path)
+        else:
+            path = default_logging_path
+
+        # Load and apply the logging configuration
         logging_config = Path(path).read_text(encoding="utf-8")
         self.configure(yaml.safe_load(logging_config))
 
+        # Log info about the logging configuration
+        if not user_logging_path and default_logging_path == Path("conf/logging.yml"):
+            logger = logging.getLogger(__name__)
+            logger.info(
+                f"Using `{path}` as logging configuration. "
+                f"You can change this by setting the KEDRO_LOGGING_CONFIG environment variable accordingly."
+            )
+
     def configure(self, logging_config: dict[str, Any]) -> None:
         """Configure project logging using ``logging_config`` (e.g. from project
         logging.yml). We store this in the UserDict data so that it can be reconfigured
         in _bootstrap_subprocess.
         """
         logging.config.dictConfig(logging_config)
         self.data = logging_config
@@ -315,42 +343,58 @@
             f"'find_pipelines'."
         )
         return None
 
     return obj
 
 
-def find_pipelines() -> dict[str, Pipeline]:  # noqa: PLR0912
+def find_pipelines(raise_errors: bool = False) -> dict[str, Pipeline]:  # noqa: PLR0912
     """Automatically find modular pipelines having a ``create_pipeline``
     function. By default, projects created using Kedro 0.18.3 and higher
     call this function to autoregister pipelines upon creation/addition.
 
     Projects that require more fine-grained control can still define the
     pipeline registry without calling this function. Alternatively, they
     can modify the mapping generated by the ``find_pipelines`` function.
 
     For more information on the pipeline registry and autodiscovery, see
     https://kedro.readthedocs.io/en/stable/nodes_and_pipelines/pipeline_registry.html
 
+    Args:
+        raise_errors: If ``True``, raise an error upon failed discovery.
+
     Returns:
         A generated mapping from pipeline names to ``Pipeline`` objects.
 
+    Raises:
+        ImportError: When a module does not expose a ``create_pipeline``
+            function, the ``create_pipeline`` function does not return a
+            ``Pipeline`` object, or if the module import fails up front.
+            If ``raise_errors`` is ``False``, see Warns section instead.
+
     Warns:
         UserWarning: When a module does not expose a ``create_pipeline``
             function, the ``create_pipeline`` function does not return a
             ``Pipeline`` object, or if the module import fails up front.
+            If ``raise_errors`` is ``True``, see Raises section instead.
     """
     pipeline_obj = None
 
     # Handle the simplified project structure found in several starters.
     pipeline_module_name = f"{PACKAGE_NAME}.pipeline"
     try:
         pipeline_module = importlib.import_module(pipeline_module_name)
     except Exception as exc:
         if str(exc) != f"No module named '{pipeline_module_name}'":
+            if raise_errors:
+                raise ImportError(
+                    f"An error occurred while importing the "
+                    f"'{pipeline_module_name}' module."
+                ) from exc
+
             warnings.warn(
                 IMPORT_ERROR_MESSAGE.format(
                     module=pipeline_module_name, tb_exc=traceback.format_exc()
                 )
             )
     else:
         pipeline_obj = _create_pipeline(pipeline_module)
@@ -374,15 +418,21 @@
         # Prevent imports of hidden directories/files
         if pipeline_name.startswith("."):
             continue
 
         pipeline_module_name = f"{PACKAGE_NAME}.pipelines.{pipeline_name}"
         try:
             pipeline_module = importlib.import_module(pipeline_module_name)
-        except:  # noqa: E722
+        except Exception as exc:
+            if raise_errors:
+                raise ImportError(
+                    f"An error occurred while importing the "
+                    f"'{pipeline_module_name}' module."
+                ) from exc
+
             warnings.warn(
                 IMPORT_ERROR_MESSAGE.format(
                     module=pipeline_module_name, tb_exc=traceback.format_exc()
                 )
             )
             continue
```

### Comparing `kedro-0.19.5/kedro/framework/session/session.py` & `kedro-0.19.6/kedro/framework/session/session.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/framework/session/shelvestore.py` & `kedro-0.19.6/kedro/framework/session/shelvestore.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/framework/session/store.py` & `kedro-0.19.6/kedro/framework/session/store.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/framework/startup.py` & `kedro-0.19.6/kedro/framework/startup.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/io/__init__.py` & `kedro-0.19.6/kedro/io/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/io/cached_dataset.py` & `kedro-0.19.6/kedro/io/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/io/core.py` & `kedro-0.19.6/kedro/io/core.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/io/data_catalog.py` & `kedro-0.19.6/kedro/io/data_catalog.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,14 +140,15 @@
     def __init__(  # noqa: PLR0913
         self,
         datasets: dict[str, AbstractDataset] | None = None,
         feed_dict: dict[str, Any] | None = None,
         dataset_patterns: Patterns | None = None,
         load_versions: dict[str, str] | None = None,
         save_version: str | None = None,
+        default_pattern: Patterns | None = None,
     ) -> None:
         """``DataCatalog`` stores instances of ``AbstractDataset``
         implementations to provide ``load`` and ``save`` capabilities from
         anywhere in the program. To use a ``DataCatalog``, you need to
         instantiate it with a dictionary of data sets. Then it will act as a
         single point of reference for your calls, relaying load and save
         functions to the underlying data sets.
@@ -168,14 +169,16 @@
             load_versions: A mapping between data set names and versions
                 to load. Has no effect on data sets without enabled versioning.
             save_version: Version string to be used for ``save`` operations
                 by all data sets with enabled versioning. It must: a) be a
                 case-insensitive string that conforms with operating system
                 filename limitations, b) always return the latest version when
                 sorted in lexicographical order.
+            default_pattern: A dictionary of the default catch-all pattern that overrides the default
+                pattern provided through the runners.
 
         Example:
         ::
 
             >>> from kedro_datasets.pandas import CSVDataset
             >>>
             >>> cars = CSVDataset(filepath="cars.csv",
@@ -186,14 +189,15 @@
         self._datasets = dict(datasets or {})
         self.datasets = _FrozenDatasets(self._datasets)
         # Keep a record of all patterns in the catalog.
         # {dataset pattern name : dataset pattern body}
         self._dataset_patterns = dataset_patterns or {}
         self._load_versions = load_versions or {}
         self._save_version = save_version
+        self._default_pattern = default_pattern or {}
 
         if feed_dict:
             self.add_feed_dict(feed_dict)
 
     @property
     def _logger(self) -> logging.Logger:
         return logging.getLogger(__name__)
@@ -277,28 +281,35 @@
         """
         datasets = {}
         dataset_patterns = {}
         catalog = copy.deepcopy(catalog) or {}
         credentials = copy.deepcopy(credentials) or {}
         save_version = save_version or generate_timestamp()
         load_versions = copy.deepcopy(load_versions) or {}
+        user_default = {}
 
         for ds_name, ds_config in catalog.items():
             ds_config = _resolve_credentials(  # noqa: PLW2901
                 ds_config, credentials
             )
             if cls._is_pattern(ds_name):
                 # Add each factory to the dataset_patterns dict.
                 dataset_patterns[ds_name] = ds_config
 
             else:
                 datasets[ds_name] = AbstractDataset.from_config(
                     ds_name, ds_config, load_versions.get(ds_name), save_version
                 )
         sorted_patterns = cls._sort_patterns(dataset_patterns)
+        if sorted_patterns:
+            # If the last pattern is a catch-all pattern, pop it and set it as the default
+            if cls._specificity(list(sorted_patterns.keys())[-1]) == 0:
+                last_pattern = sorted_patterns.popitem()
+                user_default = {last_pattern[0]: last_pattern[1]}
+
         missing_keys = [
             key
             for key in load_versions.keys()
             if not (key in catalog or cls._match_pattern(sorted_patterns, key))
         ]
         if missing_keys:
             raise DatasetNotFoundError(
@@ -307,14 +318,15 @@
             )
 
         return cls(
             datasets=datasets,
             dataset_patterns=sorted_patterns,
             load_versions=load_versions,
             save_version=save_version,
+            default_pattern=user_default,
         )
 
     @staticmethod
     def _is_pattern(pattern: str) -> bool:
         """Check if a given string is a pattern. Assume that any name with '{' is a pattern."""
         return "{" in pattern
 
@@ -342,14 +354,21 @@
             dataset_patterns,
             key=lambda pattern: (
                 -(cls._specificity(pattern)),
                 -pattern.count("{"),
                 pattern,
             ),
         )
+        catch_all = [
+            pattern for pattern in sorted_keys if cls._specificity(pattern) == 0
+        ]
+        if len(catch_all) > 1:
+            raise DatasetError(
+                f"Multiple catch-all patterns found in the catalog: {', '.join(catch_all)}. Only one catch-all pattern is allowed, remove the extras."
+            )
         return {key: dataset_patterns[key] for key in sorted_keys}
 
     @staticmethod
     def _specificity(pattern: str) -> int:
         """Helper function to check the length of exactly matched characters not inside brackets.
 
         Example:
@@ -365,31 +384,37 @@
 
     def _get_dataset(
         self,
         dataset_name: str,
         version: Version | None = None,
         suggest: bool = True,
     ) -> AbstractDataset:
-        matched_pattern = self._match_pattern(self._dataset_patterns, dataset_name)
+        matched_pattern = self._match_pattern(
+            self._dataset_patterns, dataset_name
+        ) or self._match_pattern(self._default_pattern, dataset_name)
         if dataset_name not in self._datasets and matched_pattern:
             # If the dataset is a patterned dataset, materialise it and add it to
             # the catalog
-            config_copy = copy.deepcopy(self._dataset_patterns[matched_pattern])
+            config_copy = copy.deepcopy(
+                self._dataset_patterns.get(matched_pattern)
+                or self._default_pattern.get(matched_pattern)
+                or {}
+            )
             dataset_config = self._resolve_config(
                 dataset_name, matched_pattern, config_copy
             )
             dataset = AbstractDataset.from_config(
                 dataset_name,
                 dataset_config,
                 self._load_versions.get(dataset_name),
                 self._save_version,
             )
             if (
                 self._specificity(matched_pattern) == 0
-                and matched_pattern != "{default}"
+                and matched_pattern in self._default_pattern
             ):
                 self._logger.warning(
                     "Config from the dataset factory pattern '%s' in the catalog will be used to "
                     "override the default dataset creation for '%s'",
                     matched_pattern,
                     dataset_name,
                 )
@@ -717,27 +742,28 @@
         self, extra_dataset_patterns: Patterns | None = None
     ) -> DataCatalog:
         """Returns a shallow copy of the current object.
 
         Returns:
             Copy of the current object.
         """
-        if extra_dataset_patterns:
+        if not self._default_pattern and extra_dataset_patterns:
             unsorted_dataset_patterns = {
                 **self._dataset_patterns,
                 **extra_dataset_patterns,
             }
             dataset_patterns = self._sort_patterns(unsorted_dataset_patterns)
         else:
             dataset_patterns = self._dataset_patterns
         return DataCatalog(
             datasets=self._datasets,
             dataset_patterns=dataset_patterns,
             load_versions=self._load_versions,
             save_version=self._save_version,
+            default_pattern=self._default_pattern,
         )
 
     def __eq__(self, other) -> bool:  # type: ignore[no-untyped-def]
         return (self._datasets, self._dataset_patterns) == (
             other._datasets,
             other._dataset_patterns,
         )
```

### Comparing `kedro-0.19.5/kedro/io/lambda_dataset.py` & `kedro-0.19.6/kedro/io/lambda_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/io/memory_dataset.py` & `kedro-0.19.6/kedro/io/memory_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/io/shared_memory_dataset.py` & `kedro-0.19.6/kedro/io/shared_memory_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/ipython/__init__.py` & `kedro-0.19.6/kedro/ipython/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """
 This script creates an IPython extension to load Kedro-related variables in
 local scope.
 """
 
 from __future__ import annotations
 
+import importlib
 import inspect
 import logging
 import os
 import sys
 import typing
 import warnings
 from pathlib import Path
 from types import MappingProxyType
 from typing import Any, Callable, OrderedDict
 
 from IPython.core.getipython import get_ipython
 from IPython.core.magic import needs_local_scope, register_line_magic
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
-from rich.console import Console
-from rich.syntax import Syntax
+
+try:
+    import rich.console as rich_console
+    import rich.syntax as rich_syntax
+except ImportError:  # pragma: no cover
+    pass
 
 from kedro.framework.cli import load_entry_points
 from kedro.framework.cli.project import CONF_SOURCE_HELP, PARAMS_ARG_HELP
 from kedro.framework.cli.utils import ENV_HELP, _split_params
 from kedro.framework.project import (
     LOGGING,  # noqa: F401
     _ProjectPipelines,
@@ -35,14 +40,16 @@
 from kedro.pipeline.node import Node
 from kedro.utils import _find_kedro_project, _is_databricks
 
 logger = logging.getLogger(__name__)
 
 FunctionParameters = MappingProxyType
 
+RICH_INSTALLED = True if importlib.util.find_spec("rich") is not None else False
+
 
 def load_ipython_extension(ipython: Any) -> None:
     """
     Main entry point when %load_ext kedro.ipython is executed, either manually or
     automatically through `kedro ipython` or `kedro jupyter lab/notebook`.
     IPython will look for this function specifically.
     See https://ipython.readthedocs.io/en/stable/config/extensions/index.html
@@ -277,16 +284,22 @@
         app.commands.execute("notebook:replace-selection", {"text": text})
     else:
         get_ipython().set_next_input(text)  # type: ignore[no-untyped-call]
 
 
 def _print_cells(cells: list[str]) -> None:
     for cell in cells:
-        Console().print("")
-        Console().print(Syntax(cell, "python", theme="monokai", line_numbers=False))
+        if RICH_INSTALLED is True:
+            rich_console.Console().print("")
+            rich_console.Console().print(
+                rich_syntax.Syntax(cell, "python", theme="monokai", line_numbers=False)
+            )
+        else:
+            print("")  # noqa: T201
+            print(cell)  # noqa: T201
 
 
 def _load_node(node_name: str, pipelines: _ProjectPipelines) -> list[str]:
     """Prepare the code to load dataset from catalog, import statements and function body.
 
     Args:
         node_name (str): The name of the node.
```

### Comparing `kedro-0.19.5/kedro/ipython/logo-svg.svg` & `kedro-0.19.6/kedro/ipython/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/logging.py` & `kedro-0.19.6/kedro/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-"""
-This module contains a logging handler class which produces coloured logs and tracebacks.
-"""
-
 import logging
 import sys
 from pathlib import Path
 from typing import Any
 
 import click
 import rich.logging
```

### Comparing `kedro-0.19.5/kedro/pipeline/_transcoding.py` & `kedro-0.19.6/kedro/pipeline/transcoding.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/pipeline/modular_pipeline.py` & `kedro-0.19.6/kedro/pipeline/modular_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import copy
 import difflib
 from typing import AbstractSet, Iterable
 
 from kedro.pipeline.node import Node
 from kedro.pipeline.pipeline import Pipeline
 
-from ._transcoding import TRANSCODING_SEPARATOR, _strip_transcoding, _transcode_split
+from .transcoding import TRANSCODING_SEPARATOR, _strip_transcoding, _transcode_split
 
 
 class ModularPipelineError(Exception):
     """Raised when a modular pipeline is not adapted and integrated
     appropriately using the helper.
     """
 
@@ -95,16 +95,18 @@
 
     Args:
         names: A dataset name or collection of dataset names.
             When str or set[str] is provided, the listed names will stay
             the same as they are named in the provided pipeline.
             When dict[str, str] is provided, current names will be
             mapped to new names in the resultant pipeline.
+
     Returns:
         A dictionary that maps the old dataset names to the provided ones.
+
     Examples:
         >>> _get_dataset_names_mapping("dataset_name")
         {"dataset_name": "dataset_name"}  # a str name will stay the same
         >>> _get_dataset_names_mapping(set(["ds_1", "ds_2"]))
         {"ds_1": "ds_1", "ds_2": "ds_2"}  # a set[str] of names will stay the same
         >>> _get_dataset_names_mapping({"ds_1": "new_ds_1_name"})
         {"ds_1": "new_ds_1_name"}  # a dict[str, str] of names will map key to value
@@ -134,16 +136,18 @@
 
     Args:
         names: A parameter name or collection of parameter names.
             When str or set[str] is provided, the listed names will stay
             the same as they are named in the provided pipeline.
             When dict[str, str] is provided, current names will be
             mapped to new names in the resultant pipeline.
+
     Returns:
         A dictionary that maps the old parameter names to the provided ones.
+
     Examples:
         >>> _get_param_names_mapping("param_name")
         {"params:param_name": "params:param_name"}  # a str name will stay the same
         >>> _get_param_names_mapping(set(["param_1", "param_2"]))
         # a set[str] of names will stay the same
         {"params:param_1": "params:param_1", "params:param_2": "params:param_2"}
         >>> _get_param_names_mapping({"param_1": "new_name_for_param_1"})
@@ -219,15 +223,14 @@
         pipe = Pipeline([pipe], tags=tags)
     else:
         pipe = Pipeline(pipe, tags=tags)
 
     if not any([inputs, outputs, parameters, namespace]):
         return pipe
 
-    # noqa: protected-access
     inputs = _get_dataset_names_mapping(inputs)
     outputs = _get_dataset_names_mapping(outputs)
     parameters = _get_param_names_mapping(parameters)
 
     _validate_datasets_exist(inputs.keys(), outputs.keys(), parameters.keys(), pipe)
     _validate_inputs_outputs(inputs.keys(), outputs.keys(), pipe)
```

### Comparing `kedro-0.19.5/kedro/pipeline/node.py` & `kedro-0.19.6/kedro/pipeline/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import re
 from collections import Counter
 from typing import Any, Callable, Iterable
 from warnings import warn
 
 from more_itertools import spy, unzip
 
-from ._transcoding import _strip_transcoding
+from .transcoding import _strip_transcoding
 
 
 class Node:
     """``Node`` is an auxiliary class facilitating the operations required to
     run user-provided functions as part of Kedro pipelines.
     """
```

### Comparing `kedro-0.19.5/kedro/pipeline/pipeline.py` & `kedro-0.19.6/kedro/pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,31 @@
 from typing import Any, Iterable
 
 from graphlib import CycleError, TopologicalSorter
 
 import kedro
 from kedro.pipeline.node import Node, _to_list
 
-from ._transcoding import (
-    TRANSCODING_SEPARATOR,  # noqa: F401 for 0.19.x backward compatibility
-    _strip_transcoding,
-)
+from .transcoding import _strip_transcoding
+
+
+def __getattr__(name: str) -> Any:
+    if name == "TRANSCODING_SEPARATOR":
+        import warnings
+
+        from kedro.pipeline.transcoding import TRANSCODING_SEPARATOR
+
+        warnings.warn(
+            f"{repr(name)} has been moved to 'kedro.pipeline.transcoding', "
+            f"and the alias will be removed in Kedro 0.20.0",
+            kedro.KedroDeprecationWarning,
+            stacklevel=2,
+        )
+        return TRANSCODING_SEPARATOR
+    raise AttributeError(f"module {repr(__name__)} has no attribute {repr(name)}")
 
 
 class OutputNotUniqueError(Exception):
     """Raised when two or more nodes that are part of the same pipeline
     produce outputs with the same name.
     """
```

### Comparing `kedro-0.19.5/kedro/runner/parallel_runner.py` & `kedro-0.19.6/kedro/runner/parallel_runner.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/runner/runner.py` & `kedro-0.19.6/kedro/runner/runner.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/runner/sequential_runner.py` & `kedro-0.19.6/kedro/runner/sequential_runner.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/runner/thread_runner.py` & `kedro-0.19.6/kedro/runner/thread_runner.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/templates/project/hooks/post_gen_project.py` & `kedro-0.19.6/kedro/templates/project/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/templates/project/hooks/utils.py` & `kedro-0.19.6/kedro/templates/project/hooks/utils.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/templates/project/prompts.yml` & `kedro-0.19.6/kedro/templates/project/prompts.yml`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/.gitignore` & `kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/README.md` & `kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/README.md`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/README.md` & `kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/README.md`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/logging.yml` & `kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/logging.yml`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py` & `kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/pyproject.toml` & `kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py` & `kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py` & `kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/test_run.py` & `kedro-0.19.6/kedro/templates/project/{{ cookiecutter.repo_name }}/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro/utils.py` & `kedro-0.19.6/kedro/utils.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/kedro.egg-info/PKG-INFO` & `kedro-0.19.6/kedro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro
-Version: 0.19.5
+Version: 0.19.6
 Summary: Kedro helps you build production-ready data and analytics pipelines
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://kedro.org
 Project-URL: Source, https://github.com/kedro-org/kedro
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro/issues
@@ -26,15 +26,15 @@
 Requires-Dist: fsspec>=2021.4
 Requires-Dist: gitpython>=3.0
 Requires-Dist: importlib-metadata<8.0,>=3.6; python_version >= "3.8"
 Requires-Dist: importlib_resources<7.0,>=1.3
 Requires-Dist: more_itertools>=8.14.0
 Requires-Dist: omegaconf>=2.1.1
 Requires-Dist: parse>=1.19.0
-Requires-Dist: pluggy<1.4.0,>=1.0
+Requires-Dist: pluggy>=1.0
 Requires-Dist: pre-commit-hooks
 Requires-Dist: PyYAML<7.0,>=4.2
 Requires-Dist: rich<14.0,>=12.0
 Requires-Dist: rope<2.0,>=0.21
 Requires-Dist: toml>=0.10.0
 Requires-Dist: graphlib_backport>=1.0.0; python_version < "3.9"
 Provides-Extra: test
@@ -47,21 +47,21 @@
 Requires-Dist: jupyterlab_server>=2.11.1; extra == "test"
 Requires-Dist: jupyterlab<5,>=3; extra == "test"
 Requires-Dist: jupyter~=1.0; extra == "test"
 Requires-Dist: kedro-datasets; python_version >= "3.9" and extra == "test"
 Requires-Dist: kedro-datasets<2.0.0; python_version < "3.9" and extra == "test"
 Requires-Dist: mypy~=1.0; extra == "test"
 Requires-Dist: pandas~=2.0; extra == "test"
-Requires-Dist: pluggy<1.4,>=1.0; extra == "test"
+Requires-Dist: pluggy>=1.0; extra == "test"
 Requires-Dist: pre-commit<4.0,>=2.9.2; extra == "test"
 Requires-Dist: pytest-cov~=3.0; extra == "test"
 Requires-Dist: pytest-mock<4.0,>=1.7.1; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=2.2.1; extra == "test"
 Requires-Dist: pytest<9.0,>=7.2; extra == "test"
-Requires-Dist: s3fs<2024.4,>=2021.4; extra == "test"
+Requires-Dist: s3fs<2024.6,>=2021.4; extra == "test"
 Requires-Dist: trufflehog~=2.1; extra == "test"
 Requires-Dist: pandas-stubs; extra == "test"
 Requires-Dist: types-PyYAML; extra == "test"
 Requires-Dist: types-cachetools; extra == "test"
 Requires-Dist: types-toml; extra == "test"
 Provides-Extra: docs
 Requires-Dist: kedro-sphinx-theme==2024.4.0; extra == "docs"
@@ -71,15 +71,15 @@
 Requires-Dist: ipylab>=1.0.0; extra == "jupyter"
 Requires-Dist: notebook>=7.0.0; extra == "jupyter"
 Provides-Extra: all
 Requires-Dist: kedro[docs,jupyter,test]; extra == "all"
 
 ![Kedro Logo Banner - Light](https://raw.githubusercontent.com/kedro-org/kedro/main/.github/demo-dark.png#gh-dark-mode-only)
 ![Kedro Logo Banner - Dark](https://raw.githubusercontent.com/kedro-org/kedro/main/.github/demo-light.png#gh-light-mode-only)
-[![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://pypi.org/project/kedro/)
+[![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg)](https://pypi.org/project/kedro/)
 [![PyPI version](https://badge.fury.io/py/kedro.svg)](https://pypi.org/project/kedro/)
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/kedro.svg)](https://anaconda.org/conda-forge/kedro)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/kedro-org/kedro/blob/main/LICENSE.md)
 [![Slack Organisation](https://img.shields.io/badge/slack-chat-blueviolet.svg?label=Kedro%20Slack&logo=slack)](https://slack.kedro.org)
 [![Slack Archive](https://img.shields.io/badge/slack-archive-blueviolet.svg?label=Kedro%20Slack%20)](https://linen-slack.kedro.org/)
 ![GitHub Actions Workflow Status - Main](https://img.shields.io/github/actions/workflow/status/kedro-org/kedro/all-checks.yml?label=main)
 ![GitHub Actions Workflow Status - Develop](https://img.shields.io/github/actions/workflow/status/kedro-org/kedro/all-checks.yml?branch=develop&label=develop)
```

### Comparing `kedro-0.19.5/kedro.egg-info/SOURCES.txt` & `kedro-0.19.6/kedro.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 kedro/framework/context/context.py
 kedro/framework/hooks/__init__.py
 kedro/framework/hooks/manager.py
 kedro/framework/hooks/markers.py
 kedro/framework/hooks/specs.py
 kedro/framework/project/__init__.py
 kedro/framework/project/default_logging.yml
+kedro/framework/project/rich_logging.yml
 kedro/framework/session/__init__.py
 kedro/framework/session/session.py
 kedro/framework/session/shelvestore.py
 kedro/framework/session/store.py
 kedro/io/__init__.py
 kedro/io/cached_dataset.py
 kedro/io/core.py
@@ -53,18 +54,18 @@
 kedro/io/memory_dataset.py
 kedro/io/shared_memory_dataset.py
 kedro/ipython/__init__.py
 kedro/ipython/logo-32x32.png
 kedro/ipython/logo-64x64.png
 kedro/ipython/logo-svg.svg
 kedro/pipeline/__init__.py
-kedro/pipeline/_transcoding.py
 kedro/pipeline/modular_pipeline.py
 kedro/pipeline/node.py
 kedro/pipeline/pipeline.py
+kedro/pipeline/transcoding.py
 kedro/runner/__init__.py
 kedro/runner/parallel_runner.py
 kedro/runner/runner.py
 kedro/runner/sequential_runner.py
 kedro/runner/thread_runner.py
 kedro/templates/pipeline/cookiecutter.json
 kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/__init__.py
```

### Comparing `kedro-0.19.5/kedro.egg-info/requires.txt` & `kedro-0.19.6/kedro.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 dynaconf<4.0,>=3.1.2
 fsspec>=2021.4
 gitpython>=3.0
 importlib_resources<7.0,>=1.3
 more_itertools>=8.14.0
 omegaconf>=2.1.1
 parse>=1.19.0
-pluggy<1.4.0,>=1.0
+pluggy>=1.0
 pre-commit-hooks
 PyYAML<7.0,>=4.2
 rich<14.0,>=12.0
 rope<2.0,>=0.21
 toml>=0.10.0
 
 [:python_version < "3.9"]
@@ -41,21 +41,21 @@
 import-linter==2.0
 ipylab>=1.0.0
 jupyterlab_server>=2.11.1
 jupyterlab<5,>=3
 jupyter~=1.0
 mypy~=1.0
 pandas~=2.0
-pluggy<1.4,>=1.0
+pluggy>=1.0
 pre-commit<4.0,>=2.9.2
 pytest-cov~=3.0
 pytest-mock<4.0,>=1.7.1
 pytest-xdist[psutil]~=2.2.1
 pytest<9.0,>=7.2
-s3fs<2024.4,>=2021.4
+s3fs<2024.6,>=2021.4
 trufflehog~=2.1
 pandas-stubs
 types-PyYAML
 types-cachetools
 types-toml
 
 [test:python_version < "3.8"]
```

### Comparing `kedro-0.19.5/pyproject.toml` & `kedro-0.19.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "fsspec>=2021.4",
     "gitpython>=3.0",
     "importlib-metadata>=3.6,<8.0; python_version >= '3.8'",
     "importlib_resources>=1.3,<7.0",  # The `files()` API was introduced in `importlib_resources` 1.3 and Python 3.9.
     "more_itertools>=8.14.0",
     "omegaconf>=2.1.1",
     "parse>=1.19.0",
-    "pluggy>=1.0, <1.4.0",
+    "pluggy>=1.0",
     "pre-commit-hooks",
     "PyYAML>=4.2,<7.0",
     "rich>=12.0,<14.0",
     "rope>=0.21,<2.0",  # subject to LGPLv3 license
     "toml>=0.10.0",
     "graphlib_backport>=1.0.0; python_version < '3.9'",
 ]
@@ -61,21 +61,21 @@
     "jupyterlab_server>=2.11.1",
     "jupyterlab>=3,<5",
     "jupyter~=1.0",
     "kedro-datasets; python_version >= '3.9'",
     "kedro-datasets<2.0.0; python_version < '3.9'",
     "mypy~=1.0",
     "pandas~=2.0",
-    "pluggy>=1.0, <1.4", # pluggy 1.4 hide imports inside function and causing mocking issue
+    "pluggy>=1.0",
     "pre-commit>=2.9.2, <4.0",  # The hook `mypy` requires pre-commit version 2.9.2.
     "pytest-cov~=3.0",
     "pytest-mock>=1.7.1, <4.0",
     "pytest-xdist[psutil]~=2.2.1",
     "pytest>=7.2,<9.0",
-    "s3fs>=2021.4, <2024.4",  # Upper bound set arbitrarily, to be reassessed in early 2024
+    "s3fs>=2021.4, <2024.6",  # Upper bound set arbitrarily, to be reassessed in early 2024
     "trufflehog~=2.1",
     # mypy related dependencies
     "pandas-stubs",
     "types-PyYAML",
     "types-cachetools",
     "types-toml"
 ]
```

### Comparing `kedro-0.19.5/tests/test_import.py` & `kedro-0.19.6/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `kedro-0.19.5/tests/test_utils.py` & `kedro-0.19.6/tests/test_utils.py`

 * *Files identical despite different names*

