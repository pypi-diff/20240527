# Comparing `tmp/django-simple-deploy-0.6.1.tar.gz` & `tmp/django_simple_deploy-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-simple-deploy-0.6.1.tar", last modified: Wed Dec  6 16:32:18 2023, max compression
+gzip compressed data, was "django_simple_deploy-0.6.2.tar", last modified: Mon May 27 16:35:04 2024, max compression
```

## Comparing `django-simple-deploy-0.6.1.tar` & `django_simple_deploy-0.6.2.tar`

### file list

```diff
@@ -1,80 +1,89 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.473085 django-simple-deploy-0.6.1/
--rw-r--r--   0 eric       (501) staff       (20)     1484 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)      121 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)     2710 2023-12-06 16:32:18.473011 django-simple-deploy-0.6.1/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1367 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.472756 django-simple-deploy-0.6.1/django_simple_deploy.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)     2710 2023-12-06 16:32:18.000000 django-simple-deploy-0.6.1/django_simple_deploy.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     2477 2023-12-06 16:32:18.000000 django-simple-deploy-0.6.1/django_simple_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-12-06 16:32:18.000000 django-simple-deploy-0.6.1/django_simple_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       25 2023-12-06 16:32:18.000000 django-simple-deploy-0.6.1/django_simple_deploy.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       14 2023-12-06 16:32:18.000000 django-simple-deploy-0.6.1/django_simple_deploy.egg-info/top_level.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.466309 django-simple-deploy-0.6.1/docs/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.466746 django-simple-deploy-0.6.1/docs/contributing/
--rw-r--r--   0 eric       (501) staff       (20)    13922 2023-11-01 22:47:04.000000 django-simple-deploy-0.6.1/docs/contributing/development_environment.md
--rw-r--r--   0 eric       (501) staff       (20)     3471 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/contributing/index.md
--rw-r--r--   0 eric       (501) staff       (20)     3392 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/contributing/own_account.md
--rw-r--r--   0 eric       (501) staff       (20)     7296 2023-11-01 22:47:04.000000 django-simple-deploy-0.6.1/docs/contributing/test_run.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.467081 django-simple-deploy-0.6.1/docs/design_docs/
--rw-r--r--   0 eric       (501) staff       (20)     2727 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/design_docs/rationale.md
--rw-r--r--   0 eric       (501) staff       (20)     5146 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/design_docs/strengths_limitations.md
--rw-r--r--   0 eric       (501) staff       (20)     3589 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/design_docs/use_cases.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.467299 django-simple-deploy-0.6.1/docs/general_documentation/
--rw-r--r--   0 eric       (501) staff       (20)     7738 2023-12-04 20:37:01.000000 django-simple-deploy-0.6.1/docs/general_documentation/choosing_platform.md
--rw-r--r--   0 eric       (501) staff       (20)     9197 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/general_documentation/cli_reference.md
--rw-r--r--   0 eric       (501) staff       (20)     1543 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/index.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.467651 django-simple-deploy-0.6.1/docs/integration_tests/
--rw-r--r--   0 eric       (501) staff       (20)      969 2023-11-01 22:47:04.000000 django-simple-deploy-0.6.1/docs/integration_tests/index.md
--rw-r--r--   0 eric       (501) staff       (20)     2068 2023-11-01 22:47:04.000000 django-simple-deploy-0.6.1/docs/integration_tests/running_integration_tests.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.468630 django-simple-deploy-0.6.1/docs/maintaining/
--rw-r--r--   0 eric       (501) staff       (20)     4088 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/maintaining/adr.md
--rw-r--r--   0 eric       (501) staff       (20)     1049 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/maintaining/index.md
--rw-r--r--   0 eric       (501) staff       (20)     1831 2023-11-01 22:47:04.000000 django-simple-deploy-0.6.1/docs/maintaining/managing_releases.md
--rw-r--r--   0 eric       (501) staff       (20)     1518 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/maintaining/merging_prs.md
--rw-r--r--   0 eric       (501) staff       (20)     3418 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/maintaining/updating_docs.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.469177 django-simple-deploy-0.6.1/docs/quick_starts/
--rw-r--r--   0 eric       (501) staff       (20)      408 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/quick_starts/index.md
--rw-r--r--   0 eric       (501) staff       (20)     4059 2023-12-04 20:37:01.000000 django-simple-deploy-0.6.1/docs/quick_starts/quick_start_flyio.md
--rw-r--r--   0 eric       (501) staff       (20)     3835 2023-12-06 08:10:57.000000 django-simple-deploy-0.6.1/docs/quick_starts/quick_start_heroku.md
--rw-r--r--   0 eric       (501) staff       (20)     3620 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/quick_starts/quick_start_platformsh.md
--rw-r--r--   0 eric       (501) staff       (20)       17 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/requirements.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.469433 django-simple-deploy-0.6.1/docs/roadmap/
--rw-r--r--   0 eric       (501) staff       (20)      222 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/roadmap/index.md
--rw-r--r--   0 eric       (501) staff       (20)     6149 2023-12-06 08:10:57.000000 django-simple-deploy-0.6.1/docs/roadmap/reaching_one_point_o.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.469804 django-simple-deploy-0.6.1/docs/unit_tests/
--rw-r--r--   0 eric       (501) staff       (20)      369 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/unit_tests/index.md
--rw-r--r--   0 eric       (501) staff       (20)     6085 2023-06-16 23:26:17.000000 django-simple-deploy-0.6.1/docs/unit_tests/running_unit_tests.md
--rw-r--r--   0 eric       (501) staff       (20)    27366 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/docs/unit_tests/understanding_unit_tests.md
--rw-r--r--   0 eric       (501) staff       (20)      100 2023-05-09 23:04:33.000000 django-simple-deploy-0.6.1/pyproject.toml
--rw-r--r--   0 eric       (501) staff       (20)     1283 2023-12-06 16:32:18.473432 django-simple-deploy-0.6.1/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/setup.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.470047 django-simple-deploy-0.6.1/simple_deploy/
--rw-r--r--   0 eric       (501) staff       (20)        0 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/simple_deploy/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      157 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/simple_deploy/apps.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.464364 django-simple-deploy-0.6.1/simple_deploy/management/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.470569 django-simple-deploy-0.6.1/simple_deploy/management/commands/
--rw-r--r--   0 eric       (501) staff       (20)     3907 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/cli.py
--rw-r--r--   0 eric       (501) staff       (20)     3342 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/deploy_messages.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.470829 django-simple-deploy-0.6.1/simple_deploy/management/commands/fly_io/
--rw-r--r--   0 eric       (501) staff       (20)    30528 2023-12-06 16:30:46.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/fly_io/deploy.py
--rw-r--r--   0 eric       (501) staff       (20)     7966 2023-12-06 16:30:46.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/fly_io/deploy_messages.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.471445 django-simple-deploy-0.6.1/simple_deploy/management/commands/fly_io/templates/
--rw-r--r--   0 eric       (501) staff       (20)      507 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/fly_io/templates/dockerfile
--rw-r--r--   0 eric       (501) staff       (20)      555 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv
--rw-r--r--   0 eric       (501) staff       (20)      687 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/fly_io/templates/dockerfile_poetry
--rw-r--r--   0 eric       (501) staff       (20)      889 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/fly_io/templates/fly.toml
--rw-r--r--   0 eric       (501) staff       (20)     1433 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/fly_io/templates/settings.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.471700 django-simple-deploy-0.6.1/simple_deploy/management/commands/heroku/
--rw-r--r--   0 eric       (501) staff       (20)    23728 2023-12-06 08:10:57.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/heroku/deploy.py
--rw-r--r--   0 eric       (501) staff       (20)     3776 2023-12-06 08:10:57.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/heroku/deploy_messages.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.471950 django-simple-deploy-0.6.1/simple_deploy/management/commands/platform_sh/
--rw-r--r--   0 eric       (501) staff       (20)    18637 2023-12-06 16:30:46.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/platform_sh/deploy.py
--rw-r--r--   0 eric       (501) staff       (20)     7045 2023-12-06 16:30:46.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/platform_sh/deploy_messages.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-12-06 16:32:18.472567 django-simple-deploy-0.6.1/simple_deploy/management/commands/platform_sh/templates/
--rw-r--r--   0 eric       (501) staff       (20)     1977 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml
--rw-r--r--   0 eric       (501) staff       (20)     1934 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/platform_sh/templates/platform.app.yaml
--rw-r--r--   0 eric       (501) staff       (20)     2423 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml
--rw-r--r--   0 eric       (501) staff       (20)      249 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/platform_sh/templates/services.yaml
--rw-r--r--   0 eric       (501) staff       (20)     1071 2023-05-09 22:08:39.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/platform_sh/templates/settings.py
--rw-r--r--   0 eric       (501) staff       (20)    39328 2023-12-04 20:37:01.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/simple_deploy.py
--rw-r--r--   0 eric       (501) staff       (20)     1832 2023-11-06 16:50:02.000000 django-simple-deploy-0.6.1/simple_deploy/management/commands/utils.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.557356 django_simple_deploy-0.6.2/
+-rw-r--r--   0 eric       (501) staff       (20)     1484 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)      121 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)     2805 2024-05-27 16:35:04.557300 django_simple_deploy-0.6.2/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1367 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.557075 django_simple_deploy-0.6.2/django_simple_deploy.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)     2805 2024-05-27 16:35:04.000000 django_simple_deploy-0.6.2/django_simple_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     2804 2024-05-27 16:35:04.000000 django_simple_deploy-0.6.2/django_simple_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2024-05-27 16:35:04.000000 django_simple_deploy-0.6.2/django_simple_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)       42 2024-05-27 16:35:04.000000 django_simple_deploy-0.6.2/django_simple_deploy.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)       14 2024-05-27 16:35:04.000000 django_simple_deploy-0.6.2/django_simple_deploy.egg-info/top_level.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.542937 django_simple_deploy-0.6.2/docs/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.543895 django_simple_deploy-0.6.2/docs/contributing/
+-rw-r--r--   0 eric       (501) staff       (20)     2239 2024-05-26 21:53:10.000000 django_simple_deploy-0.6.2/docs/contributing/architecture_notes.md
+-rw-r--r--   0 eric       (501) staff       (20)      836 2024-05-23 00:41:20.000000 django_simple_deploy-0.6.2/docs/contributing/coding_guide.md
+-rw-r--r--   0 eric       (501) staff       (20)    13922 2023-11-01 22:47:04.000000 django_simple_deploy-0.6.2/docs/contributing/development_environment.md
+-rw-r--r--   0 eric       (501) staff       (20)     3471 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/contributing/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     3392 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/contributing/own_account.md
+-rw-r--r--   0 eric       (501) staff       (20)      464 2024-05-26 21:53:10.000000 django_simple_deploy-0.6.2/docs/contributing/parking_lot.md
+-rw-r--r--   0 eric       (501) staff       (20)     7296 2023-11-01 22:47:04.000000 django_simple_deploy-0.6.2/docs/contributing/test_run.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.544320 django_simple_deploy-0.6.2/docs/design_docs/
+-rw-r--r--   0 eric       (501) staff       (20)     2727 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/design_docs/rationale.md
+-rw-r--r--   0 eric       (501) staff       (20)     5146 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/design_docs/strengths_limitations.md
+-rw-r--r--   0 eric       (501) staff       (20)     3589 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/design_docs/use_cases.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.544605 django_simple_deploy-0.6.2/docs/general_documentation/
+-rw-r--r--   0 eric       (501) staff       (20)     7738 2023-12-04 20:37:01.000000 django_simple_deploy-0.6.2/docs/general_documentation/choosing_platform.md
+-rw-r--r--   0 eric       (501) staff       (20)     9197 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/general_documentation/cli_reference.md
+-rw-r--r--   0 eric       (501) staff       (20)     1543 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/index.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.545292 django_simple_deploy-0.6.2/docs/maintaining/
+-rw-r--r--   0 eric       (501) staff       (20)     4088 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/maintaining/adr.md
+-rw-r--r--   0 eric       (501) staff       (20)     1049 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/maintaining/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     1831 2023-11-01 22:47:04.000000 django_simple_deploy-0.6.2/docs/maintaining/managing_releases.md
+-rw-r--r--   0 eric       (501) staff       (20)     1518 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/maintaining/merging_prs.md
+-rw-r--r--   0 eric       (501) staff       (20)     3418 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/maintaining/updating_docs.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.545809 django_simple_deploy-0.6.2/docs/quick_starts/
+-rw-r--r--   0 eric       (501) staff       (20)      408 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/quick_starts/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     4059 2023-12-04 20:37:01.000000 django_simple_deploy-0.6.2/docs/quick_starts/quick_start_flyio.md
+-rw-r--r--   0 eric       (501) staff       (20)     3835 2023-12-06 08:10:57.000000 django_simple_deploy-0.6.2/docs/quick_starts/quick_start_heroku.md
+-rw-r--r--   0 eric       (501) staff       (20)     3527 2024-05-23 00:41:20.000000 django_simple_deploy-0.6.2/docs/quick_starts/quick_start_platformsh.md
+-rw-r--r--   0 eric       (501) staff       (20)       17 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/requirements.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.546075 django_simple_deploy-0.6.2/docs/roadmap/
+-rw-r--r--   0 eric       (501) staff       (20)      222 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/docs/roadmap/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     6149 2023-12-06 08:10:57.000000 django_simple_deploy-0.6.2/docs/roadmap/reaching_one_point_o.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.546584 django_simple_deploy-0.6.2/docs/testing/
+-rw-r--r--   0 eric       (501) staff       (20)     4740 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.2/docs/testing/e2e_tests.md
+-rw-r--r--   0 eric       (501) staff       (20)      665 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.2/docs/testing/index.md
+-rw-r--r--   0 eric       (501) staff       (20)     5142 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.2/docs/testing/integration_tests.md
+-rw-r--r--   0 eric       (501) staff       (20)     1251 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.2/docs/testing/unit_tests.md
+-rw-r--r--   0 eric       (501) staff       (20)      100 2023-05-09 23:04:33.000000 django_simple_deploy-0.6.2/pyproject.toml
+-rw-r--r--   0 eric       (501) staff       (20)     1355 2024-05-27 16:35:04.557992 django_simple_deploy-0.6.2/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.546804 django_simple_deploy-0.6.2/simple_deploy/
+-rw-r--r--   0 eric       (501) staff       (20)        0 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      157 2024-05-23 22:47:20.000000 django_simple_deploy-0.6.2/simple_deploy/apps.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.540474 django_simple_deploy-0.6.2/simple_deploy/management/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.547712 django_simple_deploy-0.6.2/simple_deploy/management/commands/
+-rw-r--r--   0 eric       (501) staff       (20)     3902 2024-04-22 20:08:42.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/cli.py
+-rw-r--r--   0 eric       (501) staff       (20)     3342 2024-05-23 22:47:20.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/deploy_messages.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.547972 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/
+-rw-r--r--   0 eric       (501) staff       (20)    29794 2024-05-25 19:59:51.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/deploy.py
+-rw-r--r--   0 eric       (501) staff       (20)     8089 2024-01-12 06:54:17.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/deploy_messages.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.549005 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/
+-rw-r--r--   0 eric       (501) staff       (20)      507 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/dockerfile
+-rw-r--r--   0 eric       (501) staff       (20)      555 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv
+-rw-r--r--   0 eric       (501) staff       (20)      687 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/dockerfile_poetry
+-rw-r--r--   0 eric       (501) staff       (20)      889 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/fly.toml
+-rw-r--r--   0 eric       (501) staff       (20)     1428 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/settings.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.553151 django_simple_deploy-0.6.2/simple_deploy/management/commands/heroku/
+-rw-r--r--   0 eric       (501) staff       (20)    19163 2024-05-27 15:48:02.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/heroku/deploy.py
+-rw-r--r--   0 eric       (501) staff       (20)     4650 2024-05-26 21:53:10.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/heroku/deploy_messages.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.553459 django_simple_deploy-0.6.2/simple_deploy/management/commands/heroku/templates/
+-rw-r--r--   0 eric       (501) staff       (20)     1284 2024-05-27 15:48:02.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/heroku/templates/settings.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.555521 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/
+-rw-r--r--   0 eric       (501) staff       (20)    17108 2024-05-25 19:59:51.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/deploy.py
+-rw-r--r--   0 eric       (501) staff       (20)     6698 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/deploy_messages.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.556470 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/
+-rw-r--r--   0 eric       (501) staff       (20)     1977 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml
+-rw-r--r--   0 eric       (501) staff       (20)     1934 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/platform.app.yaml
+-rw-r--r--   0 eric       (501) staff       (20)     2423 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml
+-rw-r--r--   0 eric       (501) staff       (20)      249 2023-05-09 22:08:39.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/services.yaml
+-rw-r--r--   0 eric       (501) staff       (20)     1072 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/settings.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.541072 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/tests/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.556618 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/tests/unit_tests/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-27 16:35:04.556773 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/
+-rw-r--r--   0 eric       (501) staff       (20)      640 2024-05-23 00:41:20.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/projects_info_output_csv.txt
+-rw-r--r--   0 eric       (501) staff       (20)      673 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/tests/unit_tests/test_plsh_utils.py
+-rw-r--r--   0 eric       (501) staff       (20)      788 2024-05-23 23:04:10.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/utils.py
+-rw-r--r--   0 eric       (501) staff       (20)    27315 2024-05-26 21:53:10.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/simple_deploy.py
+-rw-r--r--   0 eric       (501) staff       (20)    12349 2024-05-25 22:52:28.000000 django_simple_deploy-0.6.2/simple_deploy/management/commands/utils.py
```

### Comparing `django-simple-deploy-0.6.1/LICENSE` & `django_simple_deploy-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/PKG-INFO` & `django_simple_deploy-0.6.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: django-simple-deploy
-Version: 0.6.1
+Version: 0.6.2
 Summary: A management command that auto-configures a Django project for deployment.
 Author: Eric Matthes
 Author-email: ehmatthes@gmail.com
 License: BSD
 Project-URL: Documentation, https://django-simple-deploy.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/ehmatthes/django-simple-deploy
 Project-URL: Changelog, https://github.com/ehmatthes/django-simple-deploy/blob/main/CHANGELOG.md
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=3.0
+Requires-Dist: Django>=4.2
 Requires-Dist: toml>=0.10.2
+Requires-Dist: requests>=2.28.0
 
 # django-simple-deploy
 
 Initial Django deployments made easy.
 
 ## Documentation
```

### Comparing `django-simple-deploy-0.6.1/README.md` & `django_simple_deploy-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/django_simple_deploy.egg-info/PKG-INFO` & `django_simple_deploy-0.6.2/django_simple_deploy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: django-simple-deploy
-Version: 0.6.1
+Version: 0.6.2
 Summary: A management command that auto-configures a Django project for deployment.
 Author: Eric Matthes
 Author-email: ehmatthes@gmail.com
 License: BSD
 Project-URL: Documentation, https://django-simple-deploy.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/ehmatthes/django-simple-deploy
 Project-URL: Changelog, https://github.com/ehmatthes/django-simple-deploy/blob/main/CHANGELOG.md
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=3.0
+Requires-Dist: Django>=4.2
 Requires-Dist: toml>=0.10.2
+Requires-Dist: requests>=2.28.0
 
 # django-simple-deploy
 
 Initial Django deployments made easy.
 
 ## Documentation
```

### Comparing `django-simple-deploy-0.6.1/django_simple_deploy.egg-info/SOURCES.txt` & `django_simple_deploy-0.6.2/django_simple_deploy.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,39 +7,41 @@
 django_simple_deploy.egg-info/PKG-INFO
 django_simple_deploy.egg-info/SOURCES.txt
 django_simple_deploy.egg-info/dependency_links.txt
 django_simple_deploy.egg-info/requires.txt
 django_simple_deploy.egg-info/top_level.txt
 docs/index.md
 docs/requirements.txt
+docs/contributing/architecture_notes.md
+docs/contributing/coding_guide.md
 docs/contributing/development_environment.md
 docs/contributing/index.md
 docs/contributing/own_account.md
+docs/contributing/parking_lot.md
 docs/contributing/test_run.md
 docs/design_docs/rationale.md
 docs/design_docs/strengths_limitations.md
 docs/design_docs/use_cases.md
 docs/general_documentation/choosing_platform.md
 docs/general_documentation/cli_reference.md
-docs/integration_tests/index.md
-docs/integration_tests/running_integration_tests.md
 docs/maintaining/adr.md
 docs/maintaining/index.md
 docs/maintaining/managing_releases.md
 docs/maintaining/merging_prs.md
 docs/maintaining/updating_docs.md
 docs/quick_starts/index.md
 docs/quick_starts/quick_start_flyio.md
 docs/quick_starts/quick_start_heroku.md
 docs/quick_starts/quick_start_platformsh.md
 docs/roadmap/index.md
 docs/roadmap/reaching_one_point_o.md
-docs/unit_tests/index.md
-docs/unit_tests/running_unit_tests.md
-docs/unit_tests/understanding_unit_tests.md
+docs/testing/e2e_tests.md
+docs/testing/index.md
+docs/testing/integration_tests.md
+docs/testing/unit_tests.md
 simple_deploy/__init__.py
 simple_deploy/apps.py
 simple_deploy/management/commands/cli.py
 simple_deploy/management/commands/deploy_messages.py
 simple_deploy/management/commands/simple_deploy.py
 simple_deploy/management/commands/utils.py
 simple_deploy/management/commands/fly_io/deploy.py
@@ -47,14 +49,18 @@
 simple_deploy/management/commands/fly_io/templates/dockerfile
 simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv
 simple_deploy/management/commands/fly_io/templates/dockerfile_poetry
 simple_deploy/management/commands/fly_io/templates/fly.toml
 simple_deploy/management/commands/fly_io/templates/settings.py
 simple_deploy/management/commands/heroku/deploy.py
 simple_deploy/management/commands/heroku/deploy_messages.py
+simple_deploy/management/commands/heroku/templates/settings.py
 simple_deploy/management/commands/platform_sh/deploy.py
 simple_deploy/management/commands/platform_sh/deploy_messages.py
+simple_deploy/management/commands/platform_sh/utils.py
 simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml
 simple_deploy/management/commands/platform_sh/templates/platform.app.yaml
 simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml
 simple_deploy/management/commands/platform_sh/templates/services.yaml
-simple_deploy/management/commands/platform_sh/templates/settings.py
+simple_deploy/management/commands/platform_sh/templates/settings.py
+simple_deploy/management/commands/platform_sh/tests/unit_tests/test_plsh_utils.py
+simple_deploy/management/commands/platform_sh/tests/unit_tests/resources/projects_info_output_csv.txt
```

### Comparing `django-simple-deploy-0.6.1/docs/contributing/development_environment.md` & `django_simple_deploy-0.6.2/docs/contributing/development_environment.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/contributing/index.md` & `django_simple_deploy-0.6.2/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/contributing/own_account.md` & `django_simple_deploy-0.6.2/docs/contributing/own_account.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/contributing/test_run.md` & `django_simple_deploy-0.6.2/docs/contributing/test_run.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/design_docs/rationale.md` & `django_simple_deploy-0.6.2/docs/design_docs/rationale.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/design_docs/strengths_limitations.md` & `django_simple_deploy-0.6.2/docs/design_docs/strengths_limitations.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/design_docs/use_cases.md` & `django_simple_deploy-0.6.2/docs/design_docs/use_cases.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/general_documentation/choosing_platform.md` & `django_simple_deploy-0.6.2/docs/general_documentation/choosing_platform.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/general_documentation/cli_reference.md` & `django_simple_deploy-0.6.2/docs/general_documentation/cli_reference.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/index.md` & `django_simple_deploy-0.6.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/maintaining/adr.md` & `django_simple_deploy-0.6.2/docs/maintaining/adr.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/maintaining/index.md` & `django_simple_deploy-0.6.2/docs/maintaining/index.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/maintaining/managing_releases.md` & `django_simple_deploy-0.6.2/docs/maintaining/managing_releases.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/maintaining/merging_prs.md` & `django_simple_deploy-0.6.2/docs/maintaining/merging_prs.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/maintaining/updating_docs.md` & `django_simple_deploy-0.6.2/docs/maintaining/updating_docs.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/quick_starts/quick_start_flyio.md` & `django_simple_deploy-0.6.2/docs/quick_starts/quick_start_flyio.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/quick_starts/quick_start_heroku.md` & `django_simple_deploy-0.6.2/docs/quick_starts/quick_start_heroku.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/docs/quick_starts/quick_start_platformsh.md` & `django_simple_deploy-0.6.2/docs/quick_starts/quick_start_platformsh.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,24 +4,24 @@
     - footer
 ---
 
 # Quick Start: Deploying to Platform.sh
 
 ## Overview
 
-Support for Platform.sh is in a very preliminary phase. For example, it may not work when deploying from Windows. It should work if you're using `requirements.txt`, but may not work if you're using Poetry or Pipenv. `django-simple-deploy` should only be used on test projects at this point.
+Support for Platform.sh is in a preliminary phase. For example, it won't work if you already have a project deployed to Platform.sh, or if you have more than one org.
 
 Deployment to Platform.sh can be fully automated, but the configuration-only approach is recommended. This allows you to review the changes that are made to your project before committing them and making the initial push. The fully automated approach configures your project, commits these changes, and pushes the project to Platform.sh' servers.
 
 ## Prerequisites
 
 Deployment to Platform.sh requires three things:
 
 - You must be using Git to track your project.
-- You need to have a `requirements.txt` file at the root of your project.
+- You need to be tracking your dependencies with a `requirements.txt` file, or be using Poetry or Pipenv.
 - The [Platform.sh CLI](https://docs.platform.sh/development/cli.html) must be installed on your system.
 
 ## Configuration-only deployment
 
 First, install `django-simple-deploy`, and add `simple_deploy` to `INSTALLED_APPS` in *settings.py*:
 
 ```sh
@@ -71,10 +71,10 @@
 $ git add .
 $ git commit -m "Updated project."
 $ platform push
 ```
 
 ## Troubleshooting
 
-If deployment does not work, please feel free to open an [issue](https://github.com/ehmatthes/django-simple-deploy/issues). Please share the OS you're  using locally, and the specific error message or unexpected behavior you saw. If the project you're deploying is hosted in a public repository, please share that as well.
+If deployment doesn't work, please feel free to open an [issue](https://github.com/ehmatthes/django-simple-deploy/issues). Please share the OS you're  using locally, and the specific error message or unexpected behavior you saw. If the project you're deploying is hosted in a public repository, please share that as well.
 
 Please remember that `django-simple-deploy` is in a preliminary state. That said, I'd love to know the specific issues people are running into so we can reach a 1.0 state in a reasonable time frame.
```

### Comparing `django-simple-deploy-0.6.1/docs/roadmap/reaching_one_point_o.md` & `django_simple_deploy-0.6.2/docs/roadmap/reaching_one_point_o.md`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/setup.cfg` & `django_simple_deploy-0.6.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 [metadata]
 name = django-simple-deploy
-version = 0.6.1
+version = 0.6.2
 description = A management command that auto-configures a Django project for deployment.
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Documentation = https://django-simple-deploy.readthedocs.io/en/latest/
 	GitHub = https://github.com/ehmatthes/django-simple-deploy
 	Changelog = https://github.com/ehmatthes/django-simple-deploy/blob/main/CHANGELOG.md
 author = Eric Matthes
 author_email = ehmatthes@gmail.com
 license = BSD
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 3.0
-	Framework :: Django :: 3.1
-	Framework :: Django :: 3.2
+	Framework :: Django :: 4.2
+	Framework :: Django :: 5.0
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 
 [options]
 include_package_data = true
 packages = simple_deploy
 python_requires = >=3.8
 install_requires = 
-	Django >=  3.0
+	Django >=  4.2
 	toml >= 0.10.2
+	requests >= 2.28.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django-simple-deploy-0.6.1/simple_deploy/management/commands/cli.py` & `django_simple_deploy-0.6.2/simple_deploy/management/commands/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         [--no-logging]
         [--ignore-unclean-git]
 
         [--region REGION]
         [--deployed-project-name DEPLOYED_PROJECT_NAME]"""
 
 
+# fmt: off
 class SimpleDeployCLI:
     def __init__(self, parser):
         """Defines the CLI for django-simple-deploy."""
 
         # Define groups of arguments. These groups help generate a clean
         #   output for `manage.py simple_deploy --help`
         help_group = parser.add_argument_group("Get help")
@@ -96,11 +97,11 @@
 
         # If we're doing local unit testing, we need to avoid some network
         #   calls.
         parser.add_argument(
             "--unit-testing", action="store_true", help=argparse.SUPPRESS
         )
 
-        # Used for integration testing, to avoid confirmations.
+        # Used for e2e testing, to avoid confirmations.
         parser.add_argument(
-            "--integration-testing", action="store_true", help=argparse.SUPPRESS
+            "--e2e-testing", action="store_true", help=argparse.SUPPRESS
         )
```

### Comparing `django-simple-deploy-0.6.1/simple_deploy/management/commands/deploy_messages.py` & `django_simple_deploy-0.6.2/simple_deploy/management/commands/deploy_messages.py`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/simple_deploy/management/commands/fly_io/deploy.py` & `django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/deploy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,805 +1,790 @@
-"""Manages all Fly.io-specific aspects of the deployment process."""
+"""Manages all Fly.io-specific aspects of the deployment process.
 
-# Note: Internal references to Fly.io will almost always be flyio.
-#   Public references, such as the --platform argument, will be fly_io.
+Notes:
+- Internal references to Fly.io will almost always be flyio. Public references, such as
+  the --platform argument, will be fly_io.
+- self.deployed_project_name and self.app_name are identical. The first is used in the
+  simple_deploy CLI, but Fly refers to "apps" in their docs. This redundancy makes it
+  easier to code Fly CLI commands.
+"""
 
-import sys, os, re, subprocess, json
+import sys, os, re, json
 from pathlib import Path
 
-from django.conf import settings
-from django.core.management.base import CommandError
-from django.core.management.utils import get_random_secret_key
-from django.utils.crypto import get_random_string
 from django.utils.safestring import mark_safe
 
 import requests
 
 from simple_deploy.management.commands import deploy_messages as d_msgs
 from simple_deploy.management.commands.fly_io import deploy_messages as flyio_msgs
 
-from simple_deploy.management.commands.utils import write_file_from_template, SimpleDeployCommandError
+from simple_deploy.management.commands.utils import SimpleDeployCommandError
+from simple_deploy.management.commands import utils as sd_utils
 
 
 class PlatformDeployer:
-    """Perform the initial deployment of a simple project.
-    Configure as much as possible automatically.
+    """Perform the initial deployment to Fly.io
+
+    If --automate-all is used, carry out an actual deployment.
+    If not, do all configuration work so the user only has to commit changes, and call
+    `fly deploy`.
     """
 
     def __init__(self, command):
         """Establishes connection to existing simple_deploy command object."""
         self.sd = command
         self.stdout = self.sd.stdout
+        self.messages = flyio_msgs
 
+    # --- Public methods ---
 
     def deploy(self, *args, **options):
-        self.sd.write_output("Configuring project for deployment to Fly.io...")
+        """Coordinate the overall configuration and deployment."""
+        self.sd.write_output("\nConfiguring project for deployment to Fly.io...")
+
+        self._confirm_preliminary()
+
+        self._validate_platform()
+
+        if self.sd.automate_all:
+            self._prep_automate_all()
 
         self._set_on_flyio()
         self._set_debug()
-
         self._add_dockerfile()
         self._add_dockerignore()
-        self._add_flytoml_file()
+        self._add_flytoml()
         self._modify_settings()
         self._add_requirements()
-
         self._conclude_automate_all()
-
         self._show_success_message()
 
+    # --- Helper methods for deploy() ---
 
-    def _set_on_flyio(self):
-        """Set a secret, ON_FLYIO. This is used in settings.py to apply
-        deployment-specific settings.
-        Returns:
-        - None
-        """
-        msg = "Setting ON_FLYIO secret..."
-        self.sd.write_output(msg)
+    def _confirm_preliminary(self):
+        """Confirm acknwledgement of preliminary (pre-1.0) state of project."""
+        self.sd.write_output(self.messages.confirm_preliminary)
 
-        # Skip when unit testing.
+        # Unit test check is here, so message is logged.
         if self.sd.unit_testing:
-            msg = "  Skipping for unit testing."
-            self.sd.write_output(msg)
-            return
-
-        # First check if secret has already been set.
-        #   Don't log output of `fly secrets list`!
-        cmd = f"fly secrets list -a {self.deployed_project_name}"
-        output_obj = self.sd.execute_subp_run(cmd)
-        output_str = output_obj.stdout.decode()
-        self.sd.log_info(cmd)
-
-        if 'ON_FLYIO' in output_str:
-            msg = "  Found ON_FLYIO in existing secrets."
-            self.sd.write_output(msg)
             return
 
-        cmd = f"fly secrets set -a {self.deployed_project_name} ON_FLYIO=1"
-        output_obj = self.sd.execute_subp_run(cmd)
-        output_str = output_obj.stdout.decode()
-        self.sd.log_info(cmd)
-        self.sd.write_output(output_str)
+        if self.sd.get_confirmation():
+            self.sd.write_output("  Continuing with Fly.io deployment...")
+        else:
+            # Quit and invite the user to try another platform. We are happily exiting
+            # the script; there's no need to raise an error.
+            self.sd.write_output(self.messages.cancel_flyio)
+            sys.exit()
 
-        msg = "  Set ON_FLYIO secret."
-        self.sd.write_output(msg)
+    def _validate_platform(self):
+        """Make sure the local environment and project supports deployment to Fly.io.
 
+        Make sure CLI is installed, and user is authenticated. Make sure necessary
+        resources have been created and identified, and that we have the user's
+        permission to use those resources.
 
-    def _set_debug(self):
-        """Set a secret, DEBUG=FALSE. This is used in settings.py to apply
-        deployment-specific settings.
         Returns:
-        - None
-        """
-        msg = "Setting DEBUG secret..."
-        self.sd.write_output(msg)
+            None
 
-        # Skip when unit testing.
+        Raises:
+            SimpleDeployCommandError: If we find any reason deployment won't work.
+        """
         if self.sd.unit_testing:
-            msg = "  Skipping for unit testing."
-            self.sd.write_output(msg)
+            # Unit tests don't use the platform's CLI. Use the deployed project name
+            # that was passed to the simple_deploy CLI.
+            self.deployed_project_name = self.sd.deployed_project_name
             return
 
-        # First check if secret has already been set.
-        #   Don't log output of `fly secrets list`!
-        cmd = f"fly secrets list -a {self.deployed_project_name}"
-        output_obj = self.sd.execute_subp_run(cmd)
-        output_str = output_obj.stdout.decode()
-        self.sd.log_info(cmd)
+        self._validate_cli()
 
-        if 'DEBUG' in output_str:
-            msg = "  Found DEBUG in existing secrets."
-            self.sd.write_output(msg)
-            return
+        # Make sure a Fly.io app has been created, or create one if  using
+        # --automate-all. Get the name of that app, which will be the  same as
+        # self.app_name.
+        self.deployed_project_name = self._get_deployed_project_name()
 
-        cmd = f"fly secrets set -a {self.deployed_project_name} DEBUG=FALSE"
-        output_obj = self.sd.execute_subp_run(cmd)
-        output_str = output_obj.stdout.decode()
-        self.sd.log_info(cmd)
-        self.sd.write_output(output_str)
+        # Create the db now, before any additional configuration.
+        self._create_db()
 
-        msg = "  Set DEBUG=FALSE secret."
+    def _prep_automate_all(self):
+        """Take any further actions needed if using automate_all."""
+        # All necessary resources have been created earlier, during validation.
+        pass
+
+    def _set_on_flyio(self):
+        """Set a secret, ON_FLYIO. This is used in settings.py to apply
+        deployment-specific settings.
+        """
+        msg = "\nSetting ON_FLYIO secret..."
         self.sd.write_output(msg)
+        self._set_secret("ON_FLYIO", "ON_FLYIO=1")
 
+    def _set_debug(self):
+        """Set a secret, DEBUG=FALSE. This is used in settings.py to apply
+        deployment-specific settings.
+        """
+        msg = "Setting DEBUG secret..."
+        self.sd.write_output(msg)
+        self._set_secret("DEBUG", "DEBUG=FALSE")
 
     def _add_dockerfile(self):
         """Add a minimal dockerfile.
 
-        Different dependency management systems need different Dockerfiles.
-        We could send an argument to the template to dynamically generate the
-          appropriate dockerfile, but that makes the template *much* harder to
-          read and reason about. It's much nicer to keep that logic in here, and
-          have a couple clean templates that read almost as easily as the final
-          dockerfiles that are generated for each dependency management system.
-
-        Returns:
-        - path to Dockerfile that was gnerated.
-        - None, if an existing Dockerfile was found.
+        Different dependency management systems need different Dockerfiles. We could
+        send an argument to the template to dynamically generate the appropriate
+        dockerfile, but that makes the template *much* harder to read and reason about.
+        It's much nicer to keep that logic in here, and have a couple clean templates
+        that read almost as easily as the final dockerfiles that are generated for each
+        dependency management system.
         """
 
-        # File should be in project root, if present.
+        # Existing dockerfile should be in project root, if present.
         self.sd.write_output(f"\n  Looking in {self.sd.git_path} for Dockerfile...")
-        dockerfile_present = 'Dockerfile' in os.listdir(self.sd.git_path)
 
-        if dockerfile_present:
+        path = self.sd.project_root / "Dockerfile"
+        if path.exists():
             self.sd.write_output("    Found existing Dockerfile.")
-        else:
-            # Generate file from template.
-            self.sd.write_output("    No Dockerfile found. Generating file...")
+            return
 
-            context = {
-                'django_project_name': self.sd.project_name,
-                }
+        # No Dockerfile exists. Generate new file from template.
+        self.sd.write_output("    No Dockerfile found. Generating file...")
 
-            path = self.sd.project_root / 'Dockerfile'
-            if self.sd.pkg_manager == "poetry":
-                dockerfile_template = "dockerfile_poetry"
-            elif self.sd.pkg_manager == "pipenv":
-                dockerfile_template = 'dockerfile_pipenv'
-            else:
-                dockerfile_template = 'dockerfile'
-            write_file_from_template(path, dockerfile_template, context)
+        context = {
+            "django_project_name": self.sd.local_project_name,
+        }
 
-            msg = f"\n    Generated Dockerfile: {path}"
-            self.sd.write_output(msg)
-            return path
+        if self.sd.pkg_manager == "poetry":
+            dockerfile_template = "dockerfile_poetry"
+        elif self.sd.pkg_manager == "pipenv":
+            dockerfile_template = "dockerfile_pipenv"
+        else:
+            dockerfile_template = "dockerfile"
+        sd_utils.write_file_from_template(path, dockerfile_template, context)
 
+        msg = f"\n    Generated Dockerfile: {path}"
+        self.sd.write_output(msg)
 
     def _add_dockerignore(self):
         """Add a dockerignore file, based on user's local project environmnet.
         Ignore virtual environment dir, system-specific cruft, and IDE cruft.
 
         If an existing dockerignore is found, make note of that but don't overwrite.
-
-        Returns:
-        - True if added dockerignore.
-        - False if dockerignore found unnecessary, or if an existing dockerfile
-          was found.
         """
-
         # Check for existing dockerignore file; we're only looking in project root.
         #   If we find one, don't make any changes.
-        path = Path('.dockerignore')
+        path = Path(".dockerignore")
         if path.exists():
             msg = "  Found existing .dockerignore file. Not overwriting this file."
             self.sd.write_output(msg)
-            return
-
-        # Build dockerignore string.
-        dockerignore_str = ""
-
-        # Ignore git repository.
-        dockerignore_str += ".git/\n"
-
-        # Ignore venv dir if a venv is active.
-        if self.sd.unit_testing:
-            venv_dir = 'b_env'
         else:
-            venv_dir = os.environ.get("VIRTUAL_ENV")
-            
-        if venv_dir:
-            venv_path = Path(venv_dir)
-            dockerignore_str += f"\n{venv_path.name}/\n"
-
-
-        # Add python cruft.
-        dockerignore_str += "\n__pycache__/\n*.pyc\n"
-
-        # Ignore any SQLite databases.
-        dockerignore_str += "\n*.sqlite3\n"
-
-        # If on macOS, add .DS_Store.
-        if self.sd.on_macos:
-            dockerignore_str += "\n.DS_Store\n"
-
-        # Write file.
-        path.write_text(dockerignore_str, encoding='utf-8')
-        msg = "  Wrote .dockerignore file."
-        self.sd.write_output(msg)
-
+            dockerignore_str = self._build_dockerignore()
+            path.write_text(dockerignore_str, encoding="utf-8")
+            msg = "  Wrote .dockerignore file."
+            self.sd.write_output(msg)
 
-    def _add_flytoml_file(self):
+    def _add_flytoml(self):
         """Add a minimal fly.toml file."""
         # File should be in project root, if present.
         self.sd.write_output(f"\n  Looking in {self.sd.git_path} for fly.toml file...")
-        flytoml_present = 'fly.toml' in os.listdir(self.sd.git_path)
 
-        if flytoml_present:
+        path = self.sd.project_root / "fly.toml"
+        if path.exists():
             self.sd.write_output("    Found existing fly.toml file.")
         else:
             # Generate file from template.
             context = {
-                'deployed_project_name': self.deployed_project_name,
-                'using_pipenv': (self.sd.pkg_manager == "pipenv"),
-                }
-            path = self.sd.project_root / 'fly.toml'
-            write_file_from_template(path, 'fly.toml', context)
+                "deployed_project_name": self.deployed_project_name,
+                "using_pipenv": (self.sd.pkg_manager == "pipenv"),
+            }
+            sd_utils.write_file_from_template(path, "fly.toml", context)
 
             msg = f"\n    Generated fly.toml: {path}"
             self.sd.write_output(msg)
-            return path
-
 
     def _modify_settings(self):
-        """Add settings specific to Fly.io."""
-        #   Check if a fly.io section is present. If not, add settings. If already present,
-        #   do nothing.
-        self.sd.write_output("\n  Checking if settings block for Fly.io present in settings.py...")
-
-        with open(self.sd.settings_path) as f:
-            settings_string = f.read()
+        """Add settings specific to Fly.io, if not already present."""
+        self.sd.write_output("\n  Checking for Fly.io-specific settings...")
 
+        settings_string = self.sd.settings_path.read_text()
         if 'if os.environ.get("ON_FLYIO"):' in settings_string:
             self.sd.write_output("\n    Found Fly.io settings block in settings.py.")
             return
 
-        # Add Fly.io settings block.
-        self.sd.write_output("    No Fly.io settings found in settings.py; adding settings...")
+        # No Fly-specific settings found; add Fly.io settings block.
+        self.sd.write_output("    No Fly.io settings found; adding settings...")
 
         safe_settings_string = mark_safe(settings_string)
         context = {
-            'current_settings': safe_settings_string,
-            'deployed_project_name': self.deployed_project_name,
+            "current_settings": safe_settings_string,
+            "deployed_project_name": self.deployed_project_name,
         }
-        path = Path(self.sd.settings_path)
-        write_file_from_template(path, 'settings.py', context)
+        sd_utils.write_file_from_template(self.sd.settings_path, "settings.py", context)
 
-        msg = f"    Modified settings.py file: {path}"
+        msg = f"    Modified settings.py file: {self.sd.settings_path}"
         self.sd.write_output(msg)
 
-
     def _add_requirements(self):
-        """Add requirements for serving on Fly.io."""
+        """Add requirements for deploying to Fly.io."""
         requirements = ["gunicorn", "psycopg2-binary", "dj-database-url", "whitenoise"]
         self.sd.add_packages(requirements)
 
-
     def _conclude_automate_all(self):
         """Finish automating the push to Fly.io.
+
         - Commit all changes.
         - Call `fly deploy`.
         - Call `fly apps open`, and grab URL.
         """
         # Making this check here lets deploy() be cleaner.
         if not self.sd.automate_all:
             return
 
         self.sd.commit_changes()
 
         # Push project.
-        # Use execute_command() to stream output of this long-running command.
         self.sd.write_output("  Deploying to Fly.io...")
         cmd = "fly deploy"
-        self.sd.log_info(cmd)
-        self.sd.execute_command(cmd)
+        self.sd.run_slow_command(cmd)
 
         # Open project.
         self.sd.write_output("  Opening deployed app in a new browser tab...")
         cmd = f"fly apps open -a {self.app_name}"
-        output = self.sd.execute_subp_run(cmd)
-        self.sd.log_info(cmd)
+        output = self.sd.run_quick_command(cmd)
         self.sd.write_output(output)
 
-        # Get url of deployed project.
-        url_re = r'(opening )(http.*?)( \.\.\.)'
+        # Get URL of deployed project.
+        url_re = r"(opening )(http.*?)( \.\.\.)"
         output_str = output.stdout.decode()
         m = re.search(url_re, output_str)
         if m:
             self.deployed_url = m.group(2).strip()
 
-
     def _show_success_message(self):
-        """After a successful run, show a message about what to do next."""
-
-        # DEV:
-        # - Mention that this script should not need to be run again, unless
-        #   creating a new deployment.
-        #   - Describe ongoing approach of commit, push, migrate. Lots to consider
-        #     when doing this on production app with users, make sure you learn.
+        """After a successful run, show a message about what to do next.
 
+        Describe ongoing approach of commit, push, migrate.
+        """
         if self.sd.automate_all:
-            msg = flyio_msgs.success_msg_automate_all(self.deployed_url)
-            self.sd.write_output(msg)
+            msg = self.messages.success_msg_automate_all(self.deployed_url)
         else:
-            msg = flyio_msgs.success_msg(log_output=self.sd.log_output)
+            msg = self.messages.success_msg(log_output=self.sd.log_output)
+        self.sd.write_output(msg)
+
+    def _set_secret(self, needle, secret):
+        """Set a secret on Fly, if it's not already set."""
+        if self.sd.unit_testing:
+            msg = "  Skipping for unit testing."
             self.sd.write_output(msg)
+            return
 
+        # First check if secret has already been set.
+        #   Don't log output of `fly secrets list`!
+        cmd = f"fly secrets list -a {self.deployed_project_name} --json"
+        output_obj = self.sd.run_quick_command(cmd)
+        secrets_json = json.loads(output_obj.stdout.decode())
 
-    # --- Methods called from simple_deploy.py ---
+        secrets_keys = [secret["Name"] for secret in secrets_json]
 
-    def confirm_preliminary(self):
-        """Deployment to Fly.io is in a preliminary state, and we need to be
-        explicit about that.
-        """
-        # Skip this confirmation when unit testing.
-        if self.sd.unit_testing:
+        if needle in secrets_keys:
+            msg = f"  Found {needle} in existing secrets."
+            self.sd.write_output(msg)
             return
 
-        self.sd.write_output(flyio_msgs.confirm_preliminary)
-        confirmed = self.sd.get_confirmation()
+        cmd = f"fly secrets set -a {self.deployed_project_name} {secret}"
+        output_obj = self.sd.run_quick_command(cmd)
+        output_str = output_obj.stdout.decode()
+        self.sd.write_output(output_str)
 
-        if confirmed:
-            self.sd.write_output("  Continuing with Fly.io deployment...")
-        else:
-            # Quit and invite the user to try another platform.
-            # We are happily exiting the script; there's no need to raise a
-            #   CommandError.
-            self.sd.write_output(flyio_msgs.cancel_flyio)
-            sys.exit()
+        msg = f"  Set secret: {secret}"
+        self.sd.write_output(msg)
+
+    def _build_dockerignore(self):
+        """Build the contents of the dockerignore file."""
 
+        # Start with git repository.
+        dockerignore_str = ".git/\n"
 
-    def validate_platform(self):
-        """Make sure the local environment and project supports deployment to
-        Fly.io.
-        
-        The returncode for a successful command is 0, so anything truthy means
-          a command errored out.
-        """
-
-        # When running unit tests, will not be logged into CLI.
-        if not self.sd.unit_testing:
-            self._validate_cli()
-            
-            self.deployed_project_name = self._get_deployed_project_name()
-
-            # If using automate_all, we need to create the app before creating
-            #   the db. But if there's already an app with no deployment, we can 
-            #   use that one (maybe created from a previous automate_all run).
-            # DEV: Update _get_deployed_project_name() to not throw error if
-            #   using automate_all. _create_flyio_app() can exit if not using
-            #   automate_all(). If self.deployed_project_name is set, just return
-            #   because we'll use that project. If it's not set, call create.
-            if not self.deployed_project_name and self.sd.automate_all:
-                self.deployed_project_name = self._create_flyio_app()
-
-            # Create the db now, before any additional configuration. Get region
-            #   so we know where to create the db.
-            self.region = self._get_region()
-            self._create_db()
+        # Ignore venv dir if a venv is active.
+        if self.sd.unit_testing:
+            # Unit tests build a venv dir, but use the direct path to the venv. They
+            # don't run in an active venv.
+            venv_dir = "b_env"
         else:
-            self.deployed_project_name = self.sd.deployed_project_name
+            venv_dir = os.environ.get("VIRTUAL_ENV")
 
+        if venv_dir:
+            venv_path = Path(venv_dir)
+            dockerignore_str += f"\n{venv_path.name}/\n"
 
-    def prep_automate_all(self):
-        """Take any further actions needed if using automate_all."""
-        # All creation has been taken care of earlier, during validation.
-        pass
+        # Ignore Python stuff, SQLite db.
+        dockerignore_str += "\n__pycache__/\n*.pyc\n\n*.sqlite3\n"
+
+        # If on macOS, ignore .DS_Store.
+        if self.sd.on_macos:
+            dockerignore_str += "\n.DS_Store\n"
 
+        return dockerignore_str
 
-    # --- Helper methods for methods called from simple_deploy.py ---
+    # --- Helper methods for _validate_platform() ---
 
     def _validate_cli(self):
-        """Make sure the Fly.io CLI is installed, and user is logged in."""
-        cmd = 'fly version'
-        self.sd.log_info(cmd)
-        
-        # This generates a FileNotFoundError on Ubuntu.
+        """Make sure the Fly.io CLI is installed, and user is authenticated."""
+        cmd = "fly version"
+
+        # This generates a FileNotFoundError on Ubuntu if the CLI is not installed.
         try:
-            output_obj = self.sd.execute_subp_run(cmd)
+            output_obj = self.sd.run_quick_command(cmd)
         except FileNotFoundError:
-            raise SimpleDeployCommandError(self.sd, flyio_msgs.cli_not_installed)
-        
+            raise SimpleDeployCommandError(self.sd, self.messages.cli_not_installed)
+
         self.sd.log_info(output_obj)
+
+        # DEV: Note which OS this block runs on; I believe it's macOS.
         if output_obj.returncode:
-            raise SimpleDeployCommandError(self.sd, flyio_msgs.cli_not_installed)
-            
-        # Check that user is logged in.
+            raise SimpleDeployCommandError(self.sd, self.messages.cli_not_installed)
+
+        # Check that user is authenticated.
         cmd = "fly auth whoami --json"
-        self.sd.log_info(cmd)
-        output_obj = self.sd.execute_subp_run(cmd)
-        if "Error: No access token available. Please login with 'flyctl auth login'" in output_obj.stderr.decode():
-            raise SimpleDeployCommandError(self.sd, flyio_msgs.cli_logged_out)
-        
+        output_obj = self.sd.run_quick_command(cmd)
+
+        error_msg = "Error: No access token available."
+        if error_msg in output_obj.stderr.decode():
+            raise SimpleDeployCommandError(self.sd, self.messages.cli_logged_out)
+
         # Show current authenticated fly user.
         whoami_json = json.loads(output_obj.stdout.decode())
         user_email = whoami_json["email"]
         msg = f"  Logged in to Fly.io CLI as: {user_email}"
         self.sd.write_output(msg)
-        
 
     def _get_deployed_project_name(self):
         """Get the Fly.io project name.
+
         Parse the output of `fly apps list`, and look for apps that have not
-          been deployed yet.
+        been deployed yet. Note there's some ambiguity between the use of
+        "project name" and "app name". This comes from usage in both Django
+        and target platforms. Also note that database apps can't be easily
+        distinguished from other apps.
+
+        During automated runs, creates a new Fly app if there isn't one we can use.
+
+        User interactions:
+        - If one app found, prompts user to confirm correct app.
+        - If multiple apps found, prompts user to select correct one.
 
-        Also, sets self.app_name, so the name can be used here as well.
+        Sets:
+            str: self.app_name
 
         Returns:
-        - String representing deployed project name.
-        - Empty string if no deployed project name found, but using automate_all.
-        - Raises CommandError if deployed project name can't be found.
-        """
-        if self.sd.automate_all:
-            # Simply return an empty string to indicate no suitable app was found,
-            #   and we'll create one later.
-            return ""
+            str: The deployed project name (self.app_name). Empty string if
+            using --automate-all.
 
+        Raises:
+            SimpleDeployCommandError: If deployed project name can't be found.
+        """
         msg = "\nLooking for Fly.io app to deploy against..."
         self.sd.write_output(msg)
 
-        # Get apps info.
+        # Get info about user's apps on Fly.io.
         cmd = "fly apps list --json"
-        output_obj = self.sd.execute_subp_run(cmd)
-        output_str = output_obj.stdout.decode()
-        self.sd.log_info(cmd)
+
+        # Run command, and get json output.
+        # CLI has been validated; should not have to deal with stderr.
+        output_str = self.sd.run_quick_command(cmd).stdout.decode()
         self.sd.log_info(output_str)
         output_json = json.loads(output_str)
 
-        # Only consider projects that have not been deployed yet.
+        project_names = self._get_undeployed_projects(output_json)
+        self._select_project_name(project_names)
+
+        # Display and return deployed app name.
+        msg = f"  Using Fly.io app: {self.app_name}"
+        self.sd.write_output(msg)
+        return self.app_name
+
+    def _get_undeployed_projects(self, output_json):
+        """Identify fly apps that have not yet been deployed to."""
         candidate_apps = [
-            app_dict
-            for app_dict in output_json
-            if not app_dict["Deployed"]
+            app_dict for app_dict in output_json if not app_dict["Deployed"]
+        ]
+
+        # Remove all apps with 'builder' in name.
+        project_names = [
+            apps_dict["Name"]
+            for apps_dict in candidate_apps
+            if "builder" not in apps_dict["Name"]
         ]
 
-        # Get all names that might be the app we want to deploy to.
-        project_names = [apps_dict["Name"] for apps_dict in candidate_apps]
-        project_names = [name for name in project_names if 'builder' not in name]
-
-        # We need to respond according to how many possible names were found.
-        if len(project_names) == 0:
-            # If no app name found, raise error.
-            raise SimpleDeployCommandError(self.sd, flyio_msgs.no_project_name)
+        return project_names
+
+    def _select_project_name(self, project_names):
+        """Select the correct project to deploy to."""
+
+        if not project_names:
+            # No app name found.
+            if self.sd.automate_all:
+                self.app_name = self._create_flyio_app()
+            else:
+                raise SimpleDeployCommandError(self.sd, self.messages.no_project_name)
         elif len(project_names) == 1:
-            # If only one project name, confirm that it's the correct project.
+            # Only one app name found. Confirm we can deploy to this app.
             project_name = project_names[0]
-            msg = f"\n*** Found one app on Fly.io: {project_name} ***"
+            msg = f"\n*** Found one undeployed app on Fly.io: {project_name} ***"
             self.sd.write_output(msg)
-            msg = "Is this the app you want to deploy to?"
-            if self.sd.get_confirmation(msg):
+
+            prompt = "Is this the app you want to deploy to?"
+            if self.sd.get_confirmation(prompt):
                 self.app_name = project_name
+            elif self.sd.automate_all:
+                self.app_name = self._create_flyio_app()
             else:
-                raise SimpleDeployCommandError(self.sd, flyio_msgs.no_project_name)
+                raise SimpleDeployCommandError(self.sd, self.messages.no_project_name)
         else:
-            # `apps list` does not show much specific inforamtion for undeployed apps.
-            #   ie, no creation date, so can't identify most recently created app.
+            # More than one undeployed app found. `apps list` doesn't show
+            # much specific information for undeployed apps. For exmaple we
+            # don't know the creation date, so we can't identify the most
+            # recently created app.
+
+            # Rather than a bunch of conditional logic about automate-all runs, just add
+            # "Create a new app" for automated runs. If that's chosen, create a new app.
+            if self.sd.automate_all:
+                project_names.append("Create a new app")
+
             # Show all undeployed apps, ask user to make selection.
-            while True:
-                msg = "\n*** Found multiple undeployed apps on Fly.io. ***"
-                for index, name in enumerate(project_names):
-                    msg += f"\n  {index}: {name}"
-                msg += "\n\nYou can cancel this configuration work by entering q."
-                msg += "\nWhich app would you like to use? "
-                self.sd.log_info(msg)
-                selection = input(msg)
-                self.sd.log_info(selection)
-
-                if selection.lower() in ['q', 'quit']:
-                    raise SimpleDeployCommandError(self.sd, flyio_msgs.no_project_name)
-
-                selected_name = project_names[int(selection)]
-
-                # Confirm selection, because we do *not* want to deploy against
-                #   the wrong app.
-                msg = f"You have selected {selected_name}. Is that correct?"
-                confirmed = self.sd.get_confirmation(msg)
-                if confirmed:
-                    self.app_name = selected_name
-                    break
-
-        # Return deployed app name, or raise CommandError.
-        if self.app_name:
-            msg = f"  Using Fly.io app: {self.app_name}"
-            self.sd.write_output(msg)
-            return self.app_name
-        else:
-            # Can't continue without a Fly.io app to configure against.
-            raise SimpleDeployCommandError(self.sd, flyio_msgs.no_project_name)
+            prompt = "\n*** Found multiple undeployed apps on Fly.io. ***"
+            for index, name in enumerate(project_names):
+                prompt += f"\n  {index}: {name}"
+            prompt += "\nWhich app would you like to use? "
+
+            valid_choices = [i for i in range(len(project_names))]
+
+            # Confirm selection, because we do *not* want to deploy
+            # against the wrong app.
+            confirmed = False
+            while not confirmed:
+                selection = sd_utils.get_numbered_choice(
+                    self.sd, prompt, valid_choices, self.messages.no_project_name
+                )
+                selected_name = project_names[selection]
+
+                confirm_prompt = f"You have selected {selected_name}."
+                confirm_prompt += " Is that correct?"
+                confirmed = self.sd.get_confirmation(confirm_prompt)
+
+            # Create a new app for automated runs, if needed.
+            if selected_name == "Create a new app":
+                self.app_name = self._create_flyio_app()
+            else:
+                self.app_name = selected_name
 
     def _create_flyio_app(self):
         """Create a new Fly.io app.
-        Assumes caller already checked for automate_all, and that a suitable
-          app is not already available.
+
+        Assumes caller already checked for automate_all, and that a suitable app to
+        deploy to is not already available.
+
+        Sets:
+            str: self.app_name
+
         Returns:
-        - String representing new app name.
-        - Raises CommandError if an app can't be created.
+            str: self.app_name
+
+        Raises:
+            SimpleDeployCommandError: if an app can't be created.
         """
         msg = "  Creating a new app on Fly.io..."
         self.sd.write_output(msg)
 
-        cmd = "fly apps create --generate-name"
-        output_obj = self.sd.execute_subp_run(cmd)
+        cmd = "fly apps create --generate-name --json"
+        output_obj = self.sd.run_quick_command(cmd)
         output_str = output_obj.stdout.decode()
-        self.sd.log_info(cmd)
         self.sd.write_output(output_str)
 
         # Get app name.
-        app_name_re = r'(New app created: )(\w+\-\w+\-\d+)'
-        self.app_name = ''
-        m = re.search(app_name_re, output_str)
-        if m:
-            self.app_name = m.group(2).strip()
-
-        if self.app_name:
+        app_dict = json.loads(output_str)
+        try:
+            self.app_name = app_dict["Name"]
+        except KeyError:
+            raise SimpleDeployCommandError(self.sd, self.messages.create_app_failed)
+        else:
             msg = f"  Created new app: {self.app_name}"
             self.sd.write_output(msg)
             return self.app_name
-        else:
-            # Can't continue without a Fly.io app to deploy to.
-            raise SimpleDeployCommandError(self.sd, flyio_msgs.create_app_failed)
 
+    def _create_db(self):
+        """Create a remote database.
+
+        An appropriate db should not already exist. We tell people to create
+        an app, and then we take care of everything else. We create a db with
+        the name app_name-db.
+
+        We'll look for a db with that name, for example in case someone has already run
+        simple_deploy, but only gotten partway through the deployment process. If one
+        exists, we'll ask if we should use it. Otherwise, we'll just create a new db for
+        the app.
+
+        Sets:
+            str: self.db_name
+
+        Returns:
+            None
+
+        Raises:
+            SimpleDeployCommandError: If can't create a new db, or don't get
+            permission to use existing db with matching name.
+        """
+        msg = "Looking for a Postgres database..."
+        self.sd.write_output(msg)
+
+        self.db_name = self.app_name + "-db"
+        if self._check_db_exists():
+            return self._manage_existing_db()
+
+        # No usable db found. Get region before creating the db.
+        self.region = self._get_region()
+
+        # Create a new db.
+        msg = f"  Creating a new Postgres database..."
+        self.sd.write_output(msg)
+
+        cmd = f"fly postgres create --name {self.db_name} --region {self.region}"
+        cmd += " --initial-cluster-size 1 --vm-size shared-cpu-1x --volume-size 1"
+        self._confirm_create_db(db_cmd=cmd)
+
+        # Create database. Log command, but don't log output because it should contain
+        # db credentials. May want to scrub and then log output.
+        self.sd.log_info(cmd)
+        self.sd.run_slow_command(cmd, skip_logging=True)
+
+        msg = "  Created Postgres database."
+        self.sd.write_output(msg)
+
+        self._attach_db()
 
     def _get_region(self):
-        """Get the region that the Fly.io app is configured for. We'll need this
-        to create a postgres database.
+        """Get the region nearest to the user.
 
         Notes:
         - V1 `fly apps create` automatically configured a region for the app.
-        - In V2, an app doesn't seem to have a region until it's deployed.
+        - In V2, an app doesn't have a region; it's really a container for machines,
+          which do have regions.
         - We need a region to create a db.
         - `fly postgres create` only prompts for a region, there's no -q or -y.
         - `fly postgres create` does highlight nearest region.
         - `fly platform regions` lists available regions, but doesn't identify nearest.
-        - So, for now:
+        - Possible approach:
           - Default to sea just so deployments work for now. They'll be slow for people
             far from sea.
           - Full fix: Parse `fly platform regions`, present list, ask user to select
             nearest region.
 
         Current approach:
         - This forum post: https://community.fly.io/t/feature-requests-region-latency-tests/968/6
         - Leads to this tool: https://liveview-counter.fly.dev/
         - It identifies the region with lowest latency, ie "Connected to iad".
         - Solution: request this page, parse for that phrase, select region.
         - Return 'sea' if this doesn't work.
 
         Returns:
-        - String representing region.
+            str: Region with lowest latency for user.
         """
 
         msg = "Looking for Fly.io region..."
         self.sd.write_output(msg)
 
         # Get region output.
         url = "https://liveview-counter.fly.dev/"
         r = requests.get(url)
 
-        re_region = r'Connected to ([a-z]{3})'
+        re_region = r"Connected to ([a-z]{3})"
         m = re.search(re_region, r.text)
         if m:
             region = m.group(1)
 
             msg = f"  Found lowest latency region: {region}"
             self.sd.write_output(msg)
         else:
-            region = 'sea'
+            region = "sea"
 
             msg = f"  Couldn't find lowest latency region, using 'sea'."
             self.sd.write_output(msg)
 
         return region
 
-
-    def _create_db(self):
-        """Create a db to deploy to.
-
-        An appropriate db should not already exist. We tell people to create
-          an app, and then we take care of everything else. We create a db with
-          the name app_name-db.
-        We will look for a db with that name. If one exists, we'll ask if we
-          should use it.
-        Otherwise, we'll just create a new db for the app.
-
-        Returns: 
-        - None.
-        - Raises CommandError if...
-        """
-        msg = "Looking for a Postgres database..."
-        self.sd.write_output(msg)
-
-        db_exists = self._check_if_db_exists()
-
-        if db_exists:
-            # A database with the name app_name-db exists.
-            # - Is it attached to this app?
-            # - Can we use it?
-            attached = self._check_db_attached()
-
-            db_name = self.app_name + "-db"
-            if attached:
-                # Database is attached to this app; get permission to use it.
-                msg = flyio_msgs.use_attached_db(db_name, self.db_users)
-                self.sd.write_output(msg)
-
-                msg = f"Okay to use {db_name} and proceed?"
-                use_db = self.sd.get_confirmation(msg)
-
-                if use_db:
-                    # We're going to use this db, and it's already been
-                    #   attached. We don't need to do anything further.
-                    return
-                else:
-                    # Permission to use this db denied.
-                    # Can't simply create a new db, because the name we'd use
-                    #   is already taken.
-                    raise SimpleDeployCommandError(self.sd, flyio_msgs.cancel_no_db)
-            else:
-                # Existing db is not attached; get permission to attach this db.
-                msg = flyio_msgs.use_unattached_db(db_name, self.db_users)
-                self.sd.write_output(msg)
-
-                msg = f"Okay to use {db_name} and proceed?"
-                use_db = self.sd.get_confirmation(msg)
-
-                # Attach db if confirmed.
-                if use_db:
-                    self._attach_db(db_name)
-                    self.db_name = db_name
-                    # We're all done.
-                    return
-                else:
-                    # Permission to use this db denied.
-                    # Can't simply create a new db, because the name we'd use
-                    #   is already taken.
-                    raise SimpleDeployCommandError(self.sd, flyio_msgs.cancel_no_db)
-
-        # No usable db found, create a new db.
-        msg = f"  Create a new Postgres database..."
-        self.sd.write_output(msg)
-
-        self.db_name = f"{self.deployed_project_name}-db"
-        cmd = f"fly postgres create --name {self.db_name} --region {self.region}"
-        cmd += " --initial-cluster-size 1 --vm-size shared-cpu-1x --volume-size 1"
-        self.sd.log_info(cmd)
-
-        # If not using automate_all, make sure it's okay to create a resource
-        #   on user's account.
-        if not self.sd.automate_all:
-            self._confirm_create_db(db_cmd=cmd)
-
-        # Create database.
-        # Use execute_command(), to stream output of long-running process.
-        # Also, we're not logging this because I believe it contains
-        #   db credentials. May want to scrub and then log output.
-        self.sd.execute_command(cmd, skip_logging=True)
-
-        msg = "  Created Postgres database."
-        self.sd.write_output(msg)
-
-        self._attach_db(self.db_name)
-
-    def _attach_db(self, db_name):
-        """Attach the database to the app."""
-        # Run `attach` command (and confirm DATABASE_URL is set?)
-        msg = "  Attaching database to Fly.io app..."
-        self.sd.write_output(msg)
-        cmd = f"fly postgres attach --app {self.deployed_project_name} {db_name}"
-        self.sd.log_info(cmd)
-
-        output_obj = self.sd.execute_subp_run(cmd)
-        output_str = output_obj.stdout.decode()
-        self.sd.write_output(output_str)
-
-        msg = "  Attached database to app."
-        self.sd.write_output(msg)
-
-    def _check_if_db_exists(self):
+    def _check_db_exists(self):
         """Check if a postgres db already exists that should be used with this app.
+
         Returns:
-        - True if db found.
-        - False if not found.
+            bool: True if appropriate db found; False if not found.
         """
 
         # First, see if any Postgres clusters exist.
         cmd = "fly postgres list --json"
-        output_obj = self.sd.execute_subp_run(cmd)
+        output_obj = self.sd.run_quick_command(cmd)
         output_str = output_obj.stdout.decode()
-        self.sd.log_info(cmd)
         self.sd.log_info(output_str)
 
         if "No postgres clusters found" in output_str:
             return False
 
         # There are some Postgres dbs. Get their names.
-        pg_names = [
-            pg_dict["Name"]
-            for pg_dict in json.loads(output_str)
-        ]
+        pg_names = [pg_dict["Name"] for pg_dict in json.loads(output_str)]
 
         # See if any of these names match this app.
-        usable_pg_name = self.app_name + "-db"
-        if usable_pg_name in pg_names:
-            msg = f"  Postgres db found: {usable_pg_name}"
+        if self.db_name in pg_names:
+            msg = f"  Postgres db found: {self.db_name}"
             self.sd.write_output(msg)
             return True
         else:
             msg = "  No matching Postgres database found."
             self.sd.write_output(msg)
             return False
 
+    def _manage_existing_db(self):
+        """Figure out what to do with an existing db whose name matches app.
+
+        Returns:
+            None: If we can use and configure existing db.
+
+        Raises:
+            SimpleDeployCommandError: If we can't use existing db, or fail to configure
+            it correctly.
+        """
+        if self._check_db_attached():
+            return self._confirm_use_attached_db()
+        else:
+            return self._confirm_use_unattached_db()
+
     def _check_db_attached(self):
         """Check if the db that was found is attached to this app.
 
         Database is considered attached to this app it has a user with the same
-          name as the app, using underscores instead of hyphens.
-        This is the default behavior if you create a new app, then a new db,
-          then attach the db to that app.
+        name as the app, using underscores instead of hyphens. This is the default
+        behavior if you create a new app, then a new db, then attach the db to that app.
+
+        Sets:
+            list: self.db_users, which can be used in messages to the user.
 
         Returns:
-        - True if db attached to this app.
-        - False if db not attached to this app.
-        - Raises SimpleDeployCommandError if we can't find a reason to use the db.
+            bool: True if attached to this app, False if not attached.
 
-        Also, defines self.db_users, which can be used in subsequent messages.
+        Raises:
+            SimpleDeployCommandError: If this db has users in addtion to the default db
+            users and a user corresponding to this app, we raise an error.
         """
         # Get users of this db.
-        #   `fly postgres users list` does not accept `--json` flag. :/
-        db_name = self.app_name + "-db"
-        cmd = f"fly postgres users list -a {db_name}"
-        output_obj = self.sd.execute_subp_run(cmd)
+        cmd = f"fly postgres users list -a {self.db_name} --json"
+        output_obj = self.sd.run_quick_command(cmd)
         output_str = output_obj.stdout.decode()
-        self.sd.log_info(cmd)
         self.sd.log_info(output_str)
 
-        # Break output into lines, get rid of header line.
-        lines = output_str.split("\n")[1:]
-        # Get rid of blank lines.
-        lines = [line for line in lines if line]
-        # Pull user from each line.
-        self.db_users = []
-        for line in lines:
-            # user is everything before first tab.
-            tab_index = line.find("\t")
-            user = line[:tab_index].strip()
-            self.db_users.append(user)
-
+        pg_users_json = json.loads(output_str)
+        self.db_users = [user_dict["Username"] for user_dict in pg_users_json]
         self.sd.log_info(f"DB users: {self.db_users}")
 
-        default_users = {'flypgadmin', 'postgres', 'repmgr'}
-        app_user = self.app_name.replace('-', '_')
+        default_users = {"flypgadmin", "postgres", "repmgr"}
+        app_user = self.app_name.replace("-", "_")
         if set(self.db_users) == default_users:
-            # This db only has default users set when a fresh db is made.
+            # This db only has the default users set when a fresh db is made.
             #   Assume it's unattached.
             return False
         elif (app_user in self.db_users) and (len(self.db_users) == 4):
-            # The current remote app has been attached to this db.
-            #   Will still need confirmation we can use this db.
+            # This db appears to have been attached to the remote app. Will still need
+            # confirmation we can use this db.
             return True
         else:
-            # This db has more than the default users, and not just the
-            #   current app. Let's not touch it.
-            # If anyone hits this situation and we should proceed, we'll
-            #   revisit this block.
+            # This db has more than the default users, and not just the current app.
+            # Let's not touch it. If anyone hits this situation and we should proceed,
+            # we'll revisit this block.
             # Note: This path has only been tested once, by manually adding
-            #   "dummy-user" to the list of db users."
-            msg = flyio_msgs.cant_use_db(db_name, self.db_users)
+            # "dummy-user" to the list of db users."
+            msg = self.messages.cant_use_db(self.db_name, self.db_users)
             raise SimpleDeployCommandError(self.sd, msg)
 
-    def _confirm_create_db(self, db_cmd):
-        """We really need to confirm that the user wants a db created on their behalf.
-        Show the command that will be run on the user's behalf.
+    def _confirm_use_attached_db(self):
+        """Confirm it's okay to use db that's already attached to this app.
+
         Returns:
-        - True if confirmed.
-        - Raises CommandError if not confirmed.
+            None: If confirmation granted.
+
+        Raises:
+            SimpleDeployCommandError: If confirmation denied.
         """
-        if self.sd.unit_testing:
+        msg = self.messages.use_attached_db(self.db_name, self.db_users)
+        self.sd.write_output(msg)
+
+        msg = f"Okay to use {self.db_name} and proceed?"
+        if not self.sd.get_confirmation(msg):
+            # Permission to use this db denied. Can't simply create a new db,
+            # because the name we'd use is already taken.
+            raise SimpleDeployCommandError(self.sd, self.messages.cancel_no_db)
+
+    def _confirm_use_unattached_db(self):
+        """Confirm it's okay to use db whose name matches this app, but hasn't
+        been attached to this app.
+
+        If confirmation given, calls _attach_db().
+
+        Sets:
+            str: self.db_name
+
+        Returns:
+            None: If confirmation given.
+
+        Raises:
+            SimpleDeployCommandError: If confirmation denied.
+        """
+        msg = self.messages.use_unattached_db(self.db_name, self.db_users)
+        self.sd.write_output(msg)
+
+        msg = f"Okay to use {self.db_name} and proceed?"
+        if self.sd.get_confirmation(msg):
+            self._attach_db(self.db_name)
             return
+        else:
+            # Permission to use this db denied.
+            # Can't simply create a new db, because the name we'd use is
+            # already taken.
+            raise SimpleDeployCommandError(self.sd, self.messages.cancel_no_db)
 
-        self.stdout.write(flyio_msgs.confirm_create_db(db_cmd))
-        confirmed = self.sd.get_confirmation()
+    def _confirm_create_db(self, db_cmd):
+        """Confirm the user wants a database created on their behalf.
 
-        if confirmed:
+        Returns:
+            None
+
+        Raises:
+            SimpleDeployCommandError: If not confirmed.
+        """
+        # Ignore this check during testing, and when using --automate-all.
+        if self.sd.unit_testing or self.sd.automate_all:
+            return
+
+        # Show the command that will be run on the user's behalf.
+        self.stdout.write(self.messages.confirm_create_db(db_cmd))
+        if self.sd.get_confirmation():
             self.stdout.write("  Creating database...")
         else:
             # Quit and invite the user to create a database manually.
-            raise SimpleDeployCommandError(self.sd, flyio_msgs.cancel_no_db)
+            raise SimpleDeployCommandError(self.sd, self.messages.cancel_no_db)
+
+    def _attach_db(self):
+        """Attach the database to the app."""
+        msg = "  Attaching database to Fly.io app..."
+        self.sd.write_output(msg)
+        cmd = f"fly postgres attach --app {self.deployed_project_name} {self.db_name}"
+
+        output_obj = self.sd.run_quick_command(cmd)
+        output_str = output_obj.stdout.decode()
+
+        # Show full output, then scrub for logging.
+        self.sd.write_output(output_str, skip_logging=True)
+
+        output_scrubbed = [
+            l for l in output_str.splitlines() if "DATABASE_URL" not in l
+        ]
+        output_scrubbed = "\n".join(output_scrubbed)
+        self.sd.log_info(output_scrubbed)
+
+        msg = "  Attached database to app."
+        self.sd.write_output(msg)
```

### Comparing `django-simple-deploy-0.6.1/simple_deploy/management/commands/fly_io/deploy_messages.py` & `django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/deploy_messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,117 +83,129 @@
   manually, and configure it to work with this app.
 If you think there's a database that simple_deploy should be able to use,
   please open an issue: https://github.com/ehmatthes/django-simple-deploy/issues
 """
 
 
 # --- Dynamic strings ---
-# These need to be generated in functions, to display information that's 
+# These need to be generated in functions, to display information that's
 #   determined as the script runs.
 
+
 def region_not_found(app_name):
     """Could not find a region to deploy to."""
 
-    msg = dedent(f"""
+    msg = dedent(
+        f"""
         --- A Fly.io region was not found. ---
 
         We need to know what region the app is going to be deployed to.
         We could not find a region in the output of:
 
         $ fly regions list -a {app_name}
-    """)
+    """
+    )
 
     return msg
 
 
 def confirm_use_org_name(org_name):
     """Confirm use of this org name to create a new project."""
 
-    msg = dedent(f"""
+    msg = dedent(
+        f"""
         --- The Fly.io CLI requires an organization name when creating a new project. ---
         When using --automate-all, a project will be created on your behalf. The following
         organization name was found: {org_name}
 
         This organization will be used to create a new project. If this is not okay,
         enter n to cancel this operation.
-    """)
+    """
+    )
 
     return msg
 
 
 def confirm_create_db(db_cmd):
     """Confirm it's okay to create a Postgres database on the user's account."""
 
-    msg = dedent(f"""
+    msg = dedent(
+        f"""
         A Postgres database is required to continue with deployment. If you confirm this,
         the following command will be run, to create a new database on your account:
         $ {db_cmd}
-    """)
+    """
+    )
 
     return msg
 
 
 def use_attached_db(db_name, users):
-    """Found the db attached, with only default users and app_name-db user.
-    """
-    msg = dedent(f"""
+    """Found the db attached, with only default users and app_name-db user."""
+    msg = dedent(
+        f"""
         *** Found a database whose name matches the app name: {db_name} ***
         This is the naming convention used by simple_deploy, so this is
           probably a database that was created for you by a previous
           simple_deploy run.
         This database has the following users:
           {users}
         Three of these are the default users, and the fourth is the name of the 
           app (with underscores). This database appears to have been configured
           to work with this app.
-    """)
+    """
+    )
 
     return msg
 
 
 def use_unattached_db(db_name, users):
-    """Found the db unattached, with only default users.
-    """
-    msg = dedent(f"""
+    """Found the db unattached, with only default users."""
+    msg = dedent(
+        f"""
         *** Found a database whose name matches the app name: {db_name} ***
         This is the naming convention used by simple_deploy, so this is
           probably a database that was created for you by a previous
           simple_deploy run.
         This database has the following users:
           {users}
         These are the default users for a Fly.io Postgres database. This database
           does not appear to have been used yet.
-    """)
+    """
+    )
 
     return msg
 
 
 def cant_use_db(db_name, users):
     """Can't use the db that was found, because it has multiple users."""
-    msg = dedent(f"""
+    msg = dedent(
+        f"""
         Found a database whose name matches the app name: {db_name}
         This database has the following users:
           {users}
         This is more than the default set of users that a freshly-created db
           will have. It also has a user that doesn't match the name of the app.
         This situation is unexpected; if you think this situation should be handled, 
           please open an issue: https://github.com/ehmatthes/django-simple-deploy/issues
-    """)
+    """
+    )
 
     return msg
 
 
-def success_msg(log_output=''):
+def success_msg(log_output=""):
     """Success message, for configuration-only run.
 
     Note: This is immensely helpful; I use it just about every time I do a
       manual test run.
     """
 
-    msg = dedent(f"""
+    msg = dedent(
+        f"""
         --- Your project is now configured for deployment on Fly.io ---
 
         To deploy your project, you will need to:
         - Commit the changes made in the configuration process.
             $ git status
             $ git add .
             $ git commit -am "Configured project for deployment."
@@ -201,35 +213,39 @@
             $ fly deploy
         - Open your project:
             $ fly open    
         - As you develop your project further:
             - Make local changes
             - Commit your local changes
             - Run `fly deploy` again to push your changes.
-    """)
+    """
+    )
 
     if log_output:
-        msg += dedent(f"""
+        msg += dedent(
+            f"""
         - You can find a full record of this configuration in the simple_deploy_logs directory.
-        """)
+        """
+        )
 
     return msg
 
 
 def success_msg_automate_all(deployed_url):
     """Success message, when using --automate-all."""
 
-    msg = dedent(f"""
+    msg = dedent(
+        f"""
 
         --- Your project should now be deployed on Fly.io ---
 
         It should have opened up in a new browser tab. If you see a
           "server not available" message, wait a minute or two and
           refresh the tab. It sometimes takes a few minutes for the
           server to be ready.
         - You can also visit your project at {deployed_url}
 
         If you make further changes and want to push them to Fly.io,
         commit your changes and then run `fly deploy`.
-    """)
+    """
+    )
     return msg
-
```

### Comparing `django-simple-deploy-0.6.1/simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv` & `django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/dockerfile_pipenv`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/simple_deploy/management/commands/fly_io/templates/dockerfile_poetry` & `django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/dockerfile_poetry`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/simple_deploy/management/commands/fly_io/templates/fly.toml` & `django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/fly.toml`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/simple_deploy/management/commands/fly_io/templates/settings.py` & `django_simple_deploy-0.6.2/simple_deploy/management/commands/fly_io/templates/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-{{ current_settings }}
+{{current_settings}}
 
 
 # --- Settings for Fly.io. ---
 import os
 
 if os.environ.get("ON_FLYIO_SETUP") or os.environ.get("ON_FLYIO"):
     # Static file configuration needs to take effect during the build process,
     #   and when deployed.
     # from https://whitenoise.evans.io/en/stable/#quickstart-for-django-apps
-    STATIC_ROOT = os.path.join(BASE_DIR, 'staticfiles')
-    STATIC_URL = '/static/'
-    STATICFILES_DIRS = (os.path.join(BASE_DIR, 'static'),)
+    STATIC_ROOT = os.path.join(BASE_DIR, "staticfiles")
+    STATIC_URL = "/static/"
+    STATICFILES_DIRS = (os.path.join(BASE_DIR, "static"),)
     i = MIDDLEWARE.index("django.middleware.security.SecurityMiddleware")
-    MIDDLEWARE.insert(i + 1,"whitenoise.middleware.WhiteNoiseMiddleware")
+    MIDDLEWARE.insert(i + 1, "whitenoise.middleware.WhiteNoiseMiddleware")
 
 if os.environ.get("ON_FLYIO"):
     # These settings need to be in place during deployment, but not during
     #   the setup process.
     # The `dj_database_url.parse()` call causes the build to fail; other settings
     #   here may not.
     import dj_database_url
-    
+
     # Use secret, if set, to update DEBUG value.
     if os.environ.get("DEBUG") == "FALSE":
         DEBUG = False
     elif os.environ.get("DEBUG") == "TRUE":
         DEBUG = True
 
     # Set a Fly.io-specific allowed host.
-    ALLOWED_HOSTS.append('{{ deployed_project_name }}.fly.dev')
+    ALLOWED_HOSTS.append("{{ deployed_project_name }}.fly.dev")
 
     # Use the Fly.io Postgres database.
     db_url = os.environ.get("DATABASE_URL")
-    DATABASES['default'] = dj_database_url.parse(db_url)
+    DATABASES["default"] = dj_database_url.parse(db_url)
 
     # Prevent CSRF "Origin checking failed" issue.
-    CSRF_TRUSTED_ORIGINS = ['https://{{ deployed_project_name }}.fly.dev']
+    CSRF_TRUSTED_ORIGINS = ["https://{{ deployed_project_name }}.fly.dev"]
```

### Comparing `django-simple-deploy-0.6.1/simple_deploy/management/commands/heroku/deploy.py` & `django_simple_deploy-0.6.2/simple_deploy/management/commands/simple_deploy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,573 +1,731 @@
-"""Manages all Heroku-specific aspects of the deployment process."""
+"""Manage deployement to a variety of platforms.
 
-import sys, os, re, json, subprocess
+Configuration-only mode: 
+    $ python manage.py simple_deploy --platform <platform-name>
+    Configures project for deployment to the specified platform.
+
+Automated mode:
+    $ python manage.py simple_deploy --platform <platform-name> --automate-all
+    Configures project for deployment, *and* issues platform's CLI commands to create
+    any resources needed for deployment. Also commits changes, and pushes project.
+
+Overview:
+    This is the command that's called to manage the configuration. In the automated
+    mode, it also makes the actual deployment. The entire process is coordinated in 
+    handle():
+    - Parse the CLI options that were passed.
+    - Start logging, unless suppressed.
+    - Validate the set of arguments that were passed.
+    - Inspect the user's system.
+    - Inspect the project.
+    - Add django-simple-deploy to project requirements.
+    - Call the platform's `deploy()` method.
+
+See the project documentation for more about this process:
+    https://django-simple-deploy.readthedocs.io/en/latest/
+"""
+
+import sys, os, platform, re, subprocess, logging, shlex
+from datetime import datetime
+from pathlib import Path
+from importlib import import_module
 
+from django.core.management.base import BaseCommand
 from django.conf import settings
-from django.core.management.base import CommandError
-from django.core.management.utils import get_random_secret_key
-from django.utils.crypto import get_random_string
 
-from simple_deploy.management.commands import deploy_messages as d_msgs
-from simple_deploy.management.commands.heroku import deploy_messages as dh_msgs
+import toml
 
-from simple_deploy.management.commands.utils import SimpleDeployCommandError
+from . import deploy_messages as d_msgs
+from . import utils as sd_utils
+from . import cli
 
 
-class PlatformDeployer:
-    """Perform the initial deployment of a simple project.
-    Configure as much as possible automatically.
+class Command(BaseCommand):
+    """Configure a project for deployment to a specific platform.
+
+    If using --automate-all, carry out the actual deployment as well.
     """
 
-    def __init__(self, command):
-        """Establishes connection to existing simple_deploy command object."""
-        self.sd = command
-        self.stdout = self.sd.stdout
-
-
-    def deploy(self, *args, **options):
-        self.sd.write_output("Configuring project for deployment to Heroku...")
-
-        self._get_heroku_app_info()
-        self._set_heroku_env_var()
-        self._get_heroku_settings()
-        self._generate_procfile()
-        self._add_gunicorn()
-        self._check_allowed_hosts()
-        self._configure_db()
-        self._configure_static_files()
-        self._configure_debug()
-        self._configure_secret_key()
-        self._conclude_automate_all()
-        self._summarize_deployment()
-        self._show_success_message()
-
-
-    # --- Methods used in this class ---
-
-    def _get_heroku_app_info(self):
-        """Get info about the Heroku app we're pushing to."""
-        # We assume the user has already run 'heroku create', or --automate-all
-        #   has run it. If it hasn't been run, we'll quit and tell them to do so.
-
-        # We'll also look for a Postgres db. If we don't find one, we'll create one.
-
-        # DEV: The testing approach here should be improved. We should be able
-        #   to easily test for a failed apps:info call. Also, probably want
-        #   to mock the output of apps:info rather than directly setting
-        #   heroku_app_name.
-        if self.sd.unit_testing:
-            self.heroku_app_name = 'sample-name-11894'
-        else:
-            self.sd.write_output("  Inspecting Heroku app...")
-            cmd = 'heroku apps:info --json'
-            output_obj = self.sd.execute_subp_run(cmd)
-            self.sd.log_info(cmd)
-            self.sd.write_output(output_obj)
-
-            output_str = output_obj.stdout.decode()
-
-            # If output_str is emtpy, there is no heroku app.
-            if not output_str:
-                raise SimpleDeployCommandError(self.sd, dh_msgs.no_heroku_app_detected)
-
-            # Parse output for app_name.
-            apps_list = json.loads(output_str)
-
-            # Find app name.
-            app_dict = apps_list["app"]
-            self.heroku_app_name = app_dict["name"]
-            self.sd.write_output(f"    Found Heroku app: {self.heroku_app_name}")
-
-            # Look for a Postgres database.
-            addons_list = apps_list["addons"]
-            db_exists = False
-            for addon_dict in addons_list:
-                # Look for a plan name indicating a postgres db.
-                try:
-                    plan_name = addon_dict["plan"]["name"]
-                except KeyError:
-                    pass
-                else:
-                    if "heroku-postgresql" in plan_name:
-                        db_exists = True
-                        break
-
-            if db_exists:
-                msg = f"  Found a {plan_name} database."
-                self.sd.write_output(msg)
-                return
-
-            # DEV: This should be moved to a separate method.
-            #   New method should be called from here and prep_automate_all().
-            msg = f"  Could not find an existing database. Creating one now..."
-            self.sd.write_output(msg)
-            cmd = 'heroku addons:create heroku-postgresql:mini'
-            output_obj = self.sd.execute_subp_run(cmd)
-            self.sd.log_info(cmd)
-            self.sd.write_output(output_obj)
-
-
-    def _set_heroku_env_var(self):
-        """Set a config var to indicate when we're in the Heroku environment.
-        This is mostly used to modify settings for the deployed project.
+    # Show a summary of simple_deploy in the help text.
+    help = "Configures your project for deployment to the specified platform."
+
+    def __init__(self):
+        """Customize help output."""
+
+        # Keep default BaseCommand args out of help text.
+        self.suppressed_base_arguments.update(
+            [
+                "--version",
+                "-v",
+                "--settings",
+                "--pythonpath",
+                "--traceback",
+                "--no-color",
+                "--force-color",
+            ]
+        )
+        # Ensure that --skip-checks is not included in help output.
+        self.requires_system_checks = []
+
+        super().__init__()
+
+    def create_parser(self, prog_name, subcommand, **kwargs):
+        """Customize the ArgumentParser object that will be created."""
+        epilog = "For more help, see the full documentation at: "
+        epilog += "https://django-simple-deploy.readthedocs.io"
+        parser = super().create_parser(
+            prog_name,
+            subcommand,
+            usage=cli.get_usage(),
+            epilog=epilog,
+            add_help=False,
+            **kwargs,
+        )
+
+        return parser
+
+    def add_arguments(self, parser):
+        """Define CLI options."""
+        sd_cli = cli.SimpleDeployCLI(parser)
+
+    def handle(self, *args, **options):
+        """Manage the overall configuration process.
+
+        Parse options, start logging, validate the simple_deploy command used, inspect
+        the user's system, inspect the project.
+        Verify that the user should be able to deploy to this platform.
+        Add django-simple-deploy to project requirements.
+        Call the platform-specific deploy() method.
+        """
+        self.write_output("Configuring project for deployment...", skip_logging=True)
+
+        # CLI options need to be parsed before logging starts, in case --no-logging
+        # has been passed.
+        self._parse_cli_options(options)
+
+        if self.log_output:
+            self._start_logging()
+            self._log_cli_args(options)
+
+        self._validate_command()
+        self._inspect_system()
+        self._inspect_project()
+        self._add_simple_deploy_req()
+
+        self._create_deployer()
+        self._confirm_automate_all()
+        self.platform_deployer.deploy()
+
+    # --- Methods used here, and also by platform-specific modules ---
+
+    def write_output(self, output, write_to_console=True, skip_logging=False):
+        """Write output to the appropriate places.
+
+        Typically, this is used for writing output to the console as the configuration
+        and deployment work is carried out.  Output may be a string, or an instance of
+        subprocess.CompletedProcess.
+
+        Output that's passed to this method typically needs to be logged as well, unless
+        skip_logging has been passed. This is useful, for example, when writing
+        sensitive information to the console.
+
+        Returns:
+            None
         """
+        output_str = sd_utils.get_string_from_output(output)
 
-        # Skip this entirely when unit testing.
-        if self.sd.unit_testing:
-            return
+        if write_to_console:
+            self.stdout.write(output_str)
 
-        self.sd.write_output("  Setting Heroku environment variable...")
-        cmd = 'heroku config:set ON_HEROKU=1'
-        output = self.sd.execute_subp_run(cmd)
-        self.sd.log_info(cmd)
-        self.sd.write_output(output)
-        self.sd.write_output("    Set ON_HEROKU=1.")
-        self.sd.write_output("    This is used to define Heroku-specific settings.")
-
-
-    def _get_heroku_settings(self):
-        """Get any heroku-specific settings that are already in place.
-        """
-        # If any heroku settings have already been written, we don't want to
-        #  add them again. This assumes a section at the end, starting with a
-        #  check for 'ON_HEROKU' in os.environ.
-
-        with open(self.sd.settings_path) as f:
-            settings_lines = f.readlines()
-
-        self.found_heroku_settings = False
-        self.current_heroku_settings_lines = []
-        for line in settings_lines:
-            if "if 'ON_HEROKU' in os.environ:" in line:
-                self.found_heroku_settings = True
-            if self.found_heroku_settings:
-                self.current_heroku_settings_lines.append(line)
-
-        self.sd.log_info("\nExisting Heroku settings found:")
-        self.sd.log_info('\n'.join(self.current_heroku_settings_lines))
-
-
-    def _generate_procfile(self):
-        """Create Procfile, if none present."""
-
-        #   Procfile should be in project root, if present.
-        self.sd.write_output(f"\n  Looking in {self.sd.git_path} for Procfile...")
-        procfile_present = 'Procfile' in os.listdir(self.sd.git_path)
+        if not skip_logging:
+            self.log_info(output_str)
+
+    def log_info(self, output):
+        """Log output, which may be a string or CompletedProcess instance."""
+        if self.log_output:
+            output_str = sd_utils.get_string_from_output(output)
+            sd_utils.log_output_string(output_str)
+
+    def run_quick_command(self, cmd, check=False, skip_logging=False):
+        """Run a command that should finish quickly.
+
+        Commands that should finish quickly can be run more simply than commands that
+        will take a long time. For quick commands, we can capture output and then deal
+        with it however we like, and the user won't notice that we first captured
+        the output.
+
+        The `check` parameter is included because some callers will need to handle
+        exceptions. For example, see prep_automate_all() in deploy_platformsh.py. Most
+        callers will only check stderr, or maybe the returncode; they won't need to
+        involve exception handling.
 
-        if procfile_present:
-            self.sd.write_output("    Found existing Procfile.")
-        else:
-            self.sd.write_output("    No Procfile found. Generating Procfile...")
-            if self.sd.nested_project:
-                proc_command = f"web: gunicorn {self.sd.project_name}.{self.sd.project_name}.wsgi --log-file -"
-            else:
-                proc_command = f"web: gunicorn {self.sd.project_name}.wsgi --log-file -"
+        Returns:
+            CompletedProcess
+
+        Raises:
+            CalledProcessError: If check=True is passed, will raise CPError instead of
+            returning a CompletedProcess instance with an error code set.
+        """
+        if not skip_logging:
+            self.log_info(f"\n{cmd}")
 
-            with open(f"{self.sd.git_path}/Procfile", 'w') as f:
-                f.write(proc_command)
+        if self.on_windows:
+            output = subprocess.run(cmd, shell=True, capture_output=True)
+        else:
+            cmd_parts = shlex.split(cmd)
+            output = subprocess.run(cmd_parts, capture_output=True, check=check)
 
-            self.sd.write_output("    Generated Procfile with following process:")
-            self.sd.write_output(f"      {proc_command}")
+        return output
 
+    def run_slow_command(self, cmd, skip_logging=False):
+        """Run a command that may take some time.
 
-    def _add_gunicorn(self):
-        """Add gunicorn to project requirements."""
-        self.sd.add_package("gunicorn")
+        For commands that may take a while, we need to stream output to the user, rather
+        than just capturing it. Otherwise, the command will appear to hang.
+        """
+
+        # DEV: This only captures stderr right now.
+        # The first call I used this for was `git push heroku`. That call writes to
+        # stderr; I believe streaming to stdout and stderr requires multithreading. The
+        # current approach seems to be working for all calls that use it.
+        #
+        # Adding a parameter stdout=subprocess.PIPE and adding a separate identical loop
+        # over p.stdout misses stderr. Maybe combine the loops with zip()? SO posts on
+        # this topic date back to Python2/3 days.
+        if not skip_logging:
+            self.log_info(f"\n{cmd}")
+
+        cmd_parts = cmd.split()
+        with subprocess.Popen(
+            cmd_parts,
+            stderr=subprocess.PIPE,
+            bufsize=1,
+            universal_newlines=True,
+            shell=self.use_shell,
+        ) as p:
+            for line in p.stderr:
+                self.write_output(line, skip_logging=skip_logging)
+
+        if p.returncode != 0:
+            raise subprocess.CalledProcessError(p.returncode, p.args)
+
+    def get_confirmation(
+        self, msg="Are you sure you want to do this?", skip_logging=False
+    ):
+        """Get confirmation for an action.
+
+        Assumes an appropriate message has already been displayed about what is to be
+        done. Shows a yes|no prompt. You can pass a different message for the prompt; it
+        should be phrased to elicit a yes/no response.
 
+        Returns:
+            bool: True if confirmation granted, False if not granted.
+        """
+        prompt = f"\n{msg} (yes|no) "
+        confirmed = ""
 
-    def _check_allowed_hosts(self):
-        """Make sure project can be served from heroku."""
-        # This method is specific to Heroku.
+        # If doing e2e testing, always return True.
+        if self.e2e_testing:
+            self.write_output(prompt, skip_logging=skip_logging)
+            msg = "  Confirmed for e2e testing..."
+            self.write_output(msg, skip_logging=skip_logging)
+            return True
+
+        if self.unit_testing:
+            self.write_output(prompt, skip_logging=skip_logging)
+            msg = "  Confirmed for unit testing..."
+            self.write_output(msg, skip_logging=skip_logging)
+            return True
+
+        while True:
+            self.write_output(prompt, skip_logging=skip_logging)
+            confirmed = input()
+
+            # Log user's response before processing it.
+            self.write_output(
+                confirmed, skip_logging=skip_logging, write_to_console=False
+            )
+
+            if confirmed.lower() in ("y", "yes"):
+                return True
+            elif confirmed.lower() in ("n", "no"):
+                return False
+            else:
+                self.write_output(
+                    "  Please answer yes or no.", skip_logging=skip_logging
+                )
 
-        self.sd.write_output("\n  Making sure project can be served from Heroku...")
-        heroku_host = f"{self.heroku_app_name}.herokuapp.com"
+    def check_settings(self, platform, start_line, msg_found, msg_cant_overwrite):
+        """Check if a platform-specific settings block already exists.
 
-        if heroku_host in settings.ALLOWED_HOSTS:
-            self.sd.write_output(f"    Found {heroku_host} in ALLOWED_HOSTS.")
-        elif 'herokuapp.com' in settings.ALLOWED_HOSTS:
-            # This is a generic entry that allows serving from any heroku URL.
-            self.sd.write_output("    Found 'herokuapp.com' in ALLOWED_HOSTS.")
-        else:
-            # DEV: This is not currently working; Heroku is adding a hash after the heroku_host.
-            #   See: https://github.com/ehmatthes/django-simple-deploy/issues/242
-            # new_setting = f"ALLOWED_HOSTS.append('{heroku_host}')"
-            new_setting = "ALLOWED_HOSTS.append('*')"
-            msg_added = f"    Added {heroku_host} to ALLOWED_HOSTS for the deployed project."
-            msg_already_set = f"    Found {heroku_host} in ALLOWED_HOSTS for the deployed project."
-            self._add_heroku_setting(new_setting, msg_added, msg_already_set)
+        If so, ask if we can overwrite that block. This is much simpler than trying to
+        keep track of individual settings.
 
+        Returns:
+            None
 
-    def _configure_db(self):
-        """Add required db-related packages, and modify settings for Heroku db.
+        Raises:
+            SimpleDeployCommandError: If we can't overwrite existing platform-specific
+            settings block.
         """
-        self.sd.write_output("\n  Configuring project for Heroku database...")
-        self._add_db_packages()
-        self._add_db_settings()
+        settings_text = self.settings_path.read_text()
 
+        re_platform_settings = f"(.*)({start_line})(.*)"
+        m = re.match(re_platform_settings, settings_text, re.DOTALL)
+        
+        if not m:
+            self.log_info(f"No {platform.title()}-specific settings block found.")
+            return
 
-    def _add_db_packages(self):
-        """Add packages required for the Heroku db."""
-        self.sd.write_output("    Adding db-related packages...")
+        # A platform-specific settings block exists. Get permission to overwrite it.
+        if not self.get_confirmation(msg_found):
+            raise sd_utils.SimpleDeployCommandError(self, msg_cant_overwrite)
 
-        # psycopg2 2.9 causes "database connection isn't set to UTC" issue.
-        #   See: https://github.com/ehmatthes/heroku-buildpack-python/issues/31
-        self.sd.add_package("psycopg2")
-        self.sd.add_package("dj-database-url")
+        # Platform-specific settings exist, but we can remove them and start fresh.
+        self.settings_path.write_text(m.group(1))
 
+        msg = f"  Removed existing {platform.title()}-specific settings block."
+        self.write_output(msg)
 
-    def _add_db_settings(self):
-        """Add settings for Heroku db."""
-        self.sd.write_output("   Checking Heroku db settings...")
 
-        # Import dj-database-url.
-        new_setting = "import dj_database_url"
-        msg_added = "    Added import statement for dj-database-url."
-        msg_already_set = "    Found import statement for dj-database-url."
-        self._add_heroku_setting(new_setting, msg_added, msg_already_set)
+    def add_packages(self, package_list):
+        """Add a set of packages to the project's requirements.
 
-        # Configure db.
-        new_setting = "DATABASES = {'default': dj_database_url.config(default='postgres://localhost')}"
-        msg_added = "    Added setting to configure Postgres on Heroku."
-        msg_already_set = "    Found setting to configure Postgres on Heroku."
-        self._add_heroku_setting(new_setting, msg_added, msg_already_set)
+        This is a simple wrapper for add_package(), to make it easier to add multiple
+        requirements at once. If you need to specify a version for a particular package,
+        use add_package().
 
+        Returns:
+            None
+        """
+        for package in package_list:
+            self.add_package(package)
 
-    def _configure_static_files(self):
-        """Configure static files for Heroku deployment."""
+    def add_package(self, package_name, version=""):
+        """Add a package to the project's requirements, if not already present.
 
-        self.sd.write_output("\n  Configuring static files for Heroku deployment...")
+        Handles calls with version information with pip formatting:
+            add_package("psycopg2", version="<2.9")
+        The utility methods handle this version information correctly for the dependency
+        management system in use.
 
-        # Add whitenoise to requirements.
-        self.sd.write_output("    Adding staticfiles-related packages...")
-        self.sd.add_package("whitenoise")
+        Returns:
+            None
+        """
+        self.write_output(f"\nLooking for {package_name}...")
 
-        # Modify settings, and add a directory for static files.
-        self._add_static_file_settings()
-        self._add_static_file_directory()
+        if package_name in self.requirements:
+            self.write_output(f"  Found {package_name} in requirements file.")
+            return
 
+        if self.pkg_manager == "pipenv":
+            sd_utils.add_pipenv_pkg(self.pipfile_path, package_name, version)
+        elif self.pkg_manager == "poetry":
+            self._check_poetry_deploy_group()
+            sd_utils.add_poetry_pkg(self.pyprojecttoml_path, package_name, version)
+        else:
+            sd_utils.add_req_txt_pkg(self.req_txt_path, package_name, version)
 
-    def _add_static_file_settings(self):
-        """Add all settings needed to manage static files."""
-        self.sd.write_output("    Configuring static files settings...")
+        self.write_output(f"  Added {package_name} to requirements file.")
 
-        new_setting = "STATIC_ROOT = os.path.join(BASE_DIR, 'staticfiles')"
-        msg_added = "    Added STATIC_ROOT setting for Heroku."
-        msg_already_set = "    Found STATIC_ROOT setting for Heroku."
-        self._add_heroku_setting(new_setting, msg_added, msg_already_set)
+    def commit_changes(self):
+        """Commit changes that have been made to the project.
 
-        new_setting = "STATIC_URL = '/static/'"
-        msg_added = "    Added STATIC_URL setting for Heroku."
-        msg_already_set = "    Found STATIC_URL setting for Heroku."
-        self._add_heroku_setting(new_setting, msg_added, msg_already_set)
+        This should only be called when automate_all is being used.
+        """
+        if not self.automate_all:
+            return
 
-        new_setting = "STATICFILES_DIRS = (os.path.join(BASE_DIR, 'static'),)"
-        msg_added = "    Added STATICFILES_DIRS setting for Heroku."
-        msg_already_set = "    Found STATICFILES_DIRS setting for Heroku."
-        self._add_heroku_setting(new_setting, msg_added, msg_already_set)
+        self.write_output("  Committing changes...")
 
-        new_setting = 'i = MIDDLEWARE.index("django.middleware.security.SecurityMiddleware")'
-        new_setting += '\n    MIDDLEWARE.insert(i + 1, "whitenoise.middleware.WhiteNoiseMiddleware")'
-        msg_added = "    Added Whitenoise to middleware."
-        msg_already_set = "    Found Whitenoise in middleware."
-        self._add_heroku_setting(new_setting, msg_added, msg_already_set)
+        cmd = "git add ."
+        output = self.run_quick_command(cmd)
+        self.write_output(output)
+
+        cmd = 'git commit -m "Configured project for deployment."'
+        output = self.run_quick_command(cmd)
+        self.write_output(output)
+
+    # --- Internal methods; used only in this class ---
+
+    def _parse_cli_options(self, options):
+        """Parse CLI options from simple_deploy command."""
+
+        # Platform-agnostic arguments.
+        self.automate_all = options["automate_all"]
+        self.platform = options["platform"]
+        self.log_output = not (options["no_logging"])
+        self.ignore_unclean_git = options["ignore_unclean_git"]
+
+        # Platform.sh arguments.
+        self.deployed_project_name = options["deployed_project_name"]
+        self.region = options["region"]
+
+        # Developer arguments.
+        self.unit_testing = options["unit_testing"]
+        self.e2e_testing = options["e2e_testing"]
+
+    def _start_logging(self):
+        """Set up for logging.
+
+        Create a log directory if needed; create a new log file for every run of
+        simple_deploy. Since simple_deploy should be called once, it's helpful to have
+        separate files for each run. It should only be run more than once when users
+        are fixing errors that are called out by simple_deploy, or if a remote resource
+        hangs.
 
+        Log path is added to .gitignore when the project is inspected.
+        See _inspect_project().
 
-    def _add_static_file_directory(self):
-        """Create a folder for static files, if it doesn't already exist.
+        Returns:
+            None
         """
-        self.sd.write_output("    Checking for static files directory...")
+        created_log_dir = self._create_log_dir()
+
+        # Instantiate a logger. Append a timestamp so each new run generates a unique
+        # log filename.
+        timestamp = datetime.now().strftime("%Y-%m-%d-%H%M%S")
+        log_filename = f"simple_deploy_{timestamp}.log"
+        verbose_log_path = self.log_dir_path / log_filename
+        verbose_logger = logging.basicConfig(
+            level=logging.INFO,
+            filename=verbose_log_path,
+            format="%(asctime)s %(levelname)s: %(message)s",
+        )
+
+        self.write_output("Logging run of `manage.py simple_deploy`...")
+        self.write_output(f"Created {verbose_log_path}.")
+
+    def _log_cli_args(self, options):
+        """Log the args used for this call."""
+        self.log_info(f"\nCLI args:")
+        for option, value in options.items():
+            self.log_info(f"  {option}: {value}")
 
-        # Make sure there's a static files directory.
-        static_files_dir = f"{self.sd.project_root}/static"
-        if os.path.exists(static_files_dir):
-            if os.listdir(static_files_dir):
-                self.sd.write_output("    Found non-empty static files directory.")
-                return
+
+    def _create_log_dir(self):
+        """Create a directory to hold log files, if not already present.
+
+        Returns:
+            bool: True if created directory, False if already one present.
+        """
+        self.log_dir_path = settings.BASE_DIR / "simple_deploy_logs"
+        if not self.log_dir_path.exists():
+            self.log_dir_path.mkdir()
+            return True
         else:
-            os.makedirs(static_files_dir)
-            self.sd.write_output("    Created empty static files directory.")
+            return False
 
-        # Add a placeholder file to the empty static files directory.
-        placeholder_file = f"{static_files_dir}/placeholder.txt"
-        with open(placeholder_file, 'w') as f:
-            f.write("This is a placeholder file to make sure this folder is pushed to Heroku.")
-        self.sd.write_output("    Added placeholder file to static files directory.")
-
-
-    def _configure_debug(self):
-        """Use an env var to manage DEBUG setting, and set to False."""
-
-        # Config variables are strings, which always causes confusion for people
-        #   when setting boolean env vars. A good habit is to use something other than
-        #   True or False, so it's clear we're not trying to use Python's default
-        #   boolean values.
-        # Here we use 'TRUE' and 'FALSE'. Then a simple test:
-        #    os.environ.get('DEBUG') == 'TRUE'
-        # returns the bool value True for 'TRUE', and False for 'FALSE'.
-        # Taken from: https://stackoverflow.com/a/56828137/748891
-
-        # When unit testing, don't set the heroku config var, but do make
-        #   the change to settings.
-        if not self.sd.unit_testing:
-            self.sd.write_output("  Setting DEBUG env var...")
-            cmd = 'heroku config:set DEBUG=FALSE'
-            output = self.sd.execute_subp_run(cmd)
-            self.sd.log_info(cmd)
-            self.sd.write_output(output)
-            self.sd.write_output("    Set DEBUG config variable to FALSE.")
-
-        # Modify settings to use the DEBUG config variable.
-        new_setting = "DEBUG = os.getenv('DEBUG') == 'TRUE'"
-        msg_added = "    Added DEBUG setting for Heroku."
-        msg_already_set = "    Found DEBUG setting for Heroku."
-        self._add_heroku_setting(new_setting, msg_added, msg_already_set)
-
-
-    def _configure_secret_key(self):
-        """Use an env var to manage the secret key."""
-        # Generate a new key.
-        if self.sd.on_windows:
-            # Non-alphanumeric keys have been problematic on Windows.
-            new_secret_key = get_random_string(length=50,
-                    allowed_chars='abcdefghijklmnopqrstuvwxyz0123456789')
+    def _validate_command(self):
+        """Verify simple_deploy has been called with a valid set of arguments.
+
+        Returns:
+            None
+
+        Raises:
+            SimpleDeployCommandError: If requested platform is supported.
+        """
+        if not self.platform:
+            raise sd_utils.SimpleDeployCommandError(self, d_msgs.requires_platform_flag)
+        elif self.platform in ["fly_io", "platform_sh", "heroku"]:
+            self.write_output(f"\nDeployment target: {self.platform}")
         else:
-            new_secret_key = get_random_secret_key()
+            error_msg = d_msgs.invalid_platform_msg(self.platform)
+            raise sd_utils.SimpleDeployCommandError(self, error_msg)
 
-        # Set the new key as an env var on Heroku.
-        #   Skip when unit testing.
-        if not self.sd.unit_testing:
-            self.sd.write_output("  Setting new secret key for Heroku...")
-            cmd = f"heroku config:set SECRET_KEY={new_secret_key}"
-            output = self.sd.execute_subp_run(cmd)
-            self.sd.write_output(output)
-            self.sd.write_output("    Set SECRET_KEY config variable.")
-
-        # Modify settings to use the env var's value as the secret key.
-        new_setting = "SECRET_KEY = os.getenv('SECRET_KEY')"
-        msg_added = "    Added SECRET_KEY setting for Heroku."
-        msg_already_set = "    Found SECRET_KEY setting for Heroku."
-        self._add_heroku_setting(new_setting, msg_added, msg_already_set)
-
-
-    def _conclude_automate_all(self):
-        """Finish automating the push to Heroku."""
-        # Making this check here lets deploy() be cleaner.
-        if not self.sd.automate_all:
-            return
+    def _inspect_system(self):
+        """Inspect the user's local system for relevant information.
 
-        self.sd.commit_changes()
+        Uses self.on_windows and self.on_macos because those are clean checks to run.
+        May want to refactor to self.user_system at some point. Don't ever use
+        self.platform, because "platform" refers to the host we're deploying to.
+
+        Linux is not mentioned because so far, if it works on macOS it works on Linux.
+        """
+        self.use_shell = False
+        self.on_windows, self.on_macos = False, False
+        if platform.system() == "Windows":
+            self.on_windows = True
+            self.use_shell = True
+            self.log_info("Local platform identified: Windows")
+        elif platform.system() == "Darwin":
+            self.on_macos = True
+            self.log_info("Local platform identified: macOS")
+
+    def _inspect_project(self):
+        """Inspect the local project.
+
+        Find out everything we need to know about the project before making any remote
+        calls.
+            Determine project name.
+            Find paths: .git/, settings, project root.
+            Determine if it's a nested project or not.
+            Get the dependency management approach: requirements.txt, Pipenv, Poetry
+            Get current requirements.
+
+        Anything that might cause us to exit before making the first remote call should
+        be inspected here.
+
+        Sets:
+            self.local_project_name, self.project_root, self.settings_path,
+            self.pkg_manager, self.requirements
 
-        self.sd.write_output("  Pushing to heroku...")
+        Returns:
+            None
+        """
+        self.local_project_name = settings.ROOT_URLCONF.replace(".urls", "")
+        self.log_info(f"Local project name: {self.local_project_name}")
 
-        # Get the current branch name. Get the first line of status output,
-        #   and keep everything after "On branch ".
-        cmd = 'git status'
-        git_status = self.sd.execute_subp_run(cmd)
-        self.sd.log_info(cmd)
-        self.sd.write_output(git_status)
-        status_str = git_status.stdout.decode()
-        self.current_branch = status_str.split('\n')[0][10:]
-
-        # Push current local branch to Heroku main branch.
-        # This process usually takes a minute or two, which is longer than we
-        #   want users to wait for console output. So rather than capturing
-        #   output with subprocess.run(), we use Popen and stream while logging.
-        # DEV: Note that the output of `git push heroku` goes to stderr, not stdout.
-        self.sd.write_output(f"    Pushing branch {self.current_branch}...")
-        if self.current_branch in ('main', 'master'):
-            cmd = f"git push heroku {self.current_branch}"
-        else:
-            cmd = f"git push heroku {self.current_branch}:main"
-        self.sd.execute_command(cmd)
-        self.sd.log_info(cmd)
-
-        # Run initial set of migrations.
-        self.sd.write_output("  Migrating deployed app...")
-        if self.sd.nested_project:
-            cmd = f"heroku run python {self.sd.project_name}/manage.py migrate"
-        else:
-            cmd = 'heroku run python manage.py migrate'
-        output = self.sd.execute_subp_run(cmd)
-        self.sd.log_info(cmd)
-
-        self.sd.write_output(output)
-
-        # Open Heroku app, so it simply appears in user's browser.
-        self.sd.write_output("  Opening deployed app in a new browser tab...")
-        cmd = 'heroku open'
-        output = self.sd.execute_subp_run(cmd)
-        self.sd.log_info(cmd)
-        self.sd.write_output(output)
-
-
-    def _summarize_deployment(self):
-        """Manage all tasks related to generating and showing the friendly
-        summary of the deployment.
-
-        This does not take the place of the platform's official documentation.
-          Instead, it gives the user a friendly entry into the platform's
-          official documentation. It also gives them a brief summary of some
-          followup steps they can take, for example making a second push, or
-          changing the URL of the deployed app.
-        """
-        self._generate_summary()
-
-
-    def _show_success_message(self):
-        """After a successful run, show a message about what to do next."""
-
-        # DEV:
-        # - Say something about DEBUG setting.
-        #   - Should also consider setting DEBUG = False in the Heroku-specific
-        #     settings.
-        # - Mention that this script should not need to be run again, unless
-        #   creating a new deployment.
-        #   - Describe ongoing approach of commit, push, migrate. Lots to consider
-        #     when doing this on production app with users, make sure you learn.
-
-        if self.sd.automate_all:
-            # Show how to make future deployments.
-            msg = dh_msgs.success_msg_automate_all(self.heroku_app_name,
-                    self.current_branch)
-        else:
-            # Show steps to finish the deployment process.
-            msg = dh_msgs.success_msg(self.sd.pkg_manager, self.heroku_app_name)
+        self.project_root = settings.BASE_DIR
+        self.log_info(f"Project root: {self.project_root}")
 
-        self.sd.write_output(msg)
+        # Find .git location, and make sure there's a clean status.
+        self._find_git_dir()
+        self._check_git_status()
 
+        # Now that we know where .git is, we can ignore simple_deploy logs.
+        if self.log_output:
+            self._ignore_sd_logs()
 
-    # --- Utility methods ---
+        self.settings_path = self.project_root / self.local_project_name / "settings.py"
 
-    def _check_current_heroku_settings(self, heroku_setting):
-        """Check if a setting has already been defined in the heroku-specific
-        settings section.
-        """
-        return any(heroku_setting in line for line in self.current_heroku_settings_lines)
+        # Find out which package manager is being used: req_txt, poetry, or pipenv
+        self.pkg_manager = self._get_dep_man_approach()
+        msg = f"Dependency management system: {self.pkg_manager}"
+        self.write_output(msg)
+
+        self.requirements = self._get_current_requirements()
+
+    def _find_git_dir(self):
+        """Find .git/ location.
 
+        Should be in BASE_DIR or BASE_DIR.parent. If it's in BASE_DIR.parent, this is a
+        project with a nested directory structure. A nested project has the structure
+        set up by:
+           `django-admin startproject project_name`
+        A non-nested project has manage.py at the root level, started by:
+           `django-admin startproject .`
+        This matters for knowing where manage.py is, and knowing where the .git/ dir is
+        likely to be.
 
-    def _add_heroku_setting(self, new_setting, msg_added='',
-            msg_already_set=''):
-        """Add a new setting to the heroku-specific settings, if not already
-        present.
+        Sets:
+            self.git_path, self.nested_project
+
+        Returns:
+            None
+
+        Raises:
+            SimpleDeployCommandError: If .git/ dir not found.
         """
-        already_set = self._check_current_heroku_settings(new_setting)
-        if not already_set:
-            with open(self.sd.settings_path, 'a') as f:
-                self._prep_heroku_setting(f)
-                f.write(f"\n    {new_setting}")
-                self.sd.write_output(msg_added)
+        if (self.project_root / ".git").exists():
+            self.git_path = self.project_root
+            self.write_output(f"Found .git dir at {self.git_path}.")
+            self.nested_project = False
+        elif (self.project_root.parent / ".git").exists():
+            self.git_path = self.project_root.parent
+            self.write_output(f"Found .git dir at {self.git_path}.")
+            self.nested_project = True
         else:
-            self.sd.write_output(msg_already_set)
+            error_msg = "Could not find a .git/ directory."
+            error_msg += (
+                f"\n  Looked in {self.project_root} and in {self.project_root.parent}."
+            )
+            raise sd_utils.SimpleDeployCommandError(self, error_msg)
+
+    def _check_git_status(self):
+        """Make sure all non-simple_deploy changes have already been committed.
+
+        All configuration-specific work should be contained in a single commit. This
+        allows users to easily revert back to the version of the project that worked
+        locally, if the overall deployment effort fails, or if they don't like what
+        simple_deploy does for any reason.
+
+        Don't just look for a clean git status. Some uncommitted changes related to
+        simple_deploy's work is acceptable, for example if they are doing a couple
+        runs to get things right.
+
+        Users can override this check with the --ignore-unclean-git flag.
 
+        Returns:
+            None: If status is such that simple_deploy can continue.
 
-    def _prep_heroku_setting(self, f_settings):
-        """Add a block for Heroku-specific settings, if it doesn't already
-        exist.
+        Raises:
+            SimpleDeployCommandError: If any reason found not to continue.
         """
-        if not self.found_heroku_settings:
-            # DEV: Should check if `import os` already exists in settings file.
-            f_settings.write("\nimport os")
-            f_settings.write("\nif 'ON_HEROKU' in os.environ:")
+        if self.ignore_unclean_git:
+            msg = "Ignoring git status."
+            self.write_output(msg)
+            return
 
-            # Won't need to add these lines anymore.
-            self.found_heroku_settings = True
+        cmd = "git status --porcelain"
+        output_obj = self.run_quick_command(cmd)
+        status_output = output_obj.stdout.decode()
+        self.log_info(f"{status_output}")
+
+        cmd = "git diff --unified=0"
+        output_obj = self.run_quick_command(cmd)
+        diff_output = output_obj.stdout.decode()
+        self.log_info(f"{diff_output}\n")
+
+        proceed = sd_utils.check_status_output(status_output, diff_output)
+
+        if proceed:
+            msg = "No uncommitted changes, other than simple_deploy work."
+            self.write_output(msg)
+        else:
+            self._raise_unclean_error()
 
-    def _generate_summary(self):
-        """Generate the friendly summary, which is html for now."""
-        # Generate the summary file.
-        path = self.sd.log_dir_path / 'deployment_summary.html'
+    def _raise_unclean_error(self):
+        """Raise unclean git status error."""
+        error_msg = d_msgs.unclean_git_status
+        if self.automate_all:
+            error_msg += d_msgs.unclean_git_automate_all
 
-        summary_str = "<h2>Understanding your deployment</h2>"
-        path.write_text(summary_str, encoding='utf-8')
+        raise sd_utils.SimpleDeployCommandError(self, error_msg)
 
-        msg = f"\n  Generated friendly summary: {path}"
-        self.sd.write_output(msg)
+    def _ignore_sd_logs(self):
+        """Add log dir to .gitignore.
 
+        Adds a .gitignore file if one is not found.
+        """
+        ignore_msg = "simple_deploy_logs/\n"
 
-    # --- Methods called from simple_deploy.py ---
+        gitignore_path = self.git_path / ".gitignore"
+        if not gitignore_path.exists():
+            # Make the .gitignore file, and add log directory.
+            gitignore_path.write_text(ignore_msg, encoding="utf-8")
+            self.write_output("No .gitignore file found; created .gitignore.")
+            self.write_output("Added simple_deploy_logs/ to .gitignore.")
+        else:
+            # Append log directory to .gitignore if it's not already there.
+            contents = gitignore_path.read_text()
+            if "simple_deploy_logs/" not in contents:
+                contents += f"\n{ignore_msg}"
+                gitignore_path.write_text(contents)
+                self.write_output("Added simple_deploy_logs/ to .gitignore")
+
+    def _get_dep_man_approach(self):
+        """Identify which dependency management approach the project uses.
+
+        Looks for most specific tests first: Pipenv, Poetry, then requirements.txt. For
+        example, if a project uses Poetry and has a requirements.txt file, we'll
+        prioritize Poetry.
 
-    def prep_automate_all(self):
-        """Do intial work for automating entire process.
-        - Create a heroku app to deploy to.
-        - Create a Heroku Postgres database.
+        Sets:
+            self.pkg_manager
 
         Returns:
-        - None if successful.
+            str: "req_txt" | "poetry" | "pipenv"
+
+        Raises:
+            SimpleDeployCommandError: If a pkg manager can't be identified.
         """
+        if (self.git_path / "Pipfile").exists():
+            return "pipenv"
+        elif self._check_using_poetry():
+            return "poetry"
+        elif (self.git_path / "requirements.txt").exists():
+            return "req_txt"
+
+        # Exit if we haven't found any requirements.
+        error_msg = f"Couldn't find any specified requirements in {self.git_path}."
+        raise sd_utils.SimpleDeployCommandError(self, error_msg)
+
+    def _check_using_poetry(self):
+        """Check if the project appears to be using poetry.
 
-        self.sd.write_output("  Running `heroku create`...")
-        cmd = 'heroku create'
-        output = self.sd.execute_subp_run(cmd)
-        self.sd.log_info(cmd)
-        self.sd.write_output(output)
+        Check for a pyproject.toml file with a [tool.poetry] section.
 
-        self.sd.write_output("  Creating Postgres database...")
-        cmd = 'heroku addons:create heroku-postgresql-mini'
-        output = self.sd.execute_subp_run(cmd)
-        self.sd.log_info(cmd)
-        self.sd.write_output(output)
+        Returns:
+            bool: True if found, False if not found.
+        """
+        path = self.git_path / "pyproject.toml"
+        if not path.exists():
+            return False
 
+        pptoml_data = toml.load(path)
+        return "poetry" in pptoml_data.get("tool", {})
 
-    def validate_platform(self):
-        """Make sure the local environment and project supports deployment to
-        Heroku.
+    def _get_current_requirements(self):
+        """Get current project requirements.
 
-        The returncode for a successful command is 0, so anything truthy means
-          a command errored out.
+        We need to know which requirements are already specified, so we can add any that
+        are needed on the remote platform. We don't need to deal with version numbers
+        for most packages.
+
+        Sets:
+            self.req_txt_path
+
+        Returns:
+            List[str]: List of strings, each representing a requirement.
         """
-        # Make sure Heroku CLI is installed, if we're not unit testing.
-        if not self.sd.unit_testing:
-            cmd = 'heroku --version'
-            self.sd.log_info(cmd)
-            
-            # This generates a FileNotFoundError on Linux (Ubuntu) if CLI not installed.
-            try:
-            	output_obj = self.sd.execute_subp_run(cmd)
-            except FileNotFoundError:
-                raise SimpleDeployCommandError(self.sd, dh_msgs.cli_not_installed)
-            
-            self.sd.log_info(output_obj)
-            if output_obj.returncode:
-                raise SimpleDeployCommandError(self.sd, dh_msgs.cli_not_installed)
+        msg = "Checking current project requirements..."
+        self.write_output(msg)
+
+        if self.pkg_manager == "req_txt":
+            self.req_txt_path = self.git_path / "requirements.txt"
+            requirements = sd_utils.parse_req_txt(self.req_txt_path)
+        elif self.pkg_manager == "pipenv":
+            self.pipfile_path = self.git_path / "Pipfile"
+            requirements = sd_utils.parse_pipfile(self.pipfile_path)
+        elif self.pkg_manager == "poetry":
+            self.pyprojecttoml_path = self.git_path / "pyproject.toml"
+            requirements = sd_utils.parse_pyproject_toml(self.pyprojecttoml_path)
+
+        # Report findings.
+        msg = "  Found existing dependencies:"
+        self.write_output(msg)
+        for requirement in requirements:
+            msg = f"    {requirement}"
+            self.write_output(msg)
+
+        return requirements
+
+    def _add_simple_deploy_req(self):
+        """Add django-simple-deploy to the project's requirements.
+
+        Since simple_deploy is in INCLUDED_APPS, it needs to be in the project's
+        requirements. If it's missing, platforms will reject the push.
+        """
+        msg = "\nLooking for django-simple-deploy in requirements..."
+        self.write_output(msg)
+        self.add_package("django-simple-deploy")
+
+    def _check_poetry_deploy_group(self):
+        """Make sure a deploy group exists in pyproject.toml."""
+        pptoml_data = toml.load(self.pyprojecttoml_path)
+        try:
+            deploy_group = pptoml_data["tool"]["poetry"]["group"]["deploy"]
+        except KeyError:
+            sd_utils.create_poetry_deploy_group(self.pyprojecttoml_path)
+            msg = "    Added optional deploy group to pyproject.toml."
+            self.write_output(msg)
+
+    def _create_deployer(self):
+        """Instantiate the PlatformDeployer object."""
+        deployer_module = import_module(
+            f".{self.platform}.deploy", package="simple_deploy.management.commands"
+        )
+        self.platform_deployer = deployer_module.PlatformDeployer(self)
+
+    def _confirm_automate_all(self):
+        """Confirm the user understands what --automate-all does.
 
-        # Respond appropriately if the local project uses Poetry.
-        if self.sd.pkg_manager == "poetry":
-            self.handle_poetry()
+        If confirmation not granted, exit with a message, but no error.
 
+        This must be called after the platform-specific deployer object is instantiated,
+        because we need a platform-specific confirmation message.
+        """
+        # Placing this check here keeps the handle() method cleaner.
+        if not self.automate_all:
+            return
 
-    def handle_poetry(self):
-        """Respond appropriately if the local project uses Poetry.
+        self.write_output(self.platform_deployer.messages.confirm_automate_all)
+        confirmed = self.get_confirmation()
 
-        If the project uses Poetry, generate a requirements.txt file, and 
-          override the initial value of self.sd.pkg_manager.
-        
-        Heroku does not work directly with Poetry, so we need to generate
-          a requirements.txt file for the user, which we can then add requirements
-          to. We should inform the user about this, as they may be used to 
-          just working with Poetry's requirements specification files.
-
-        This should probably be addressed in the success message as well,
-          and in the summary file. They will need to update the requirements.txt
-          file whenever they install additional packages.
-
-        Returns:
-        - None
-        """
-        msg = "  Generating a requirements.txt file, because Heroku does not support Poetry directly..."
-        self.sd.write_output(msg)
-
-        cmd = "poetry export -f requirements.txt --output requirements.txt --without-hashes"
-        output = self.sd.execute_subp_run(cmd)
-        self.sd.log_info(cmd)
-        self.sd.write_output(output)
-
-        msg = "    Wrote requirements.txt file."
-        self.sd.write_output(msg)
-
-        # From this point forward, we'll treat this user the same as anyone
-        #   who's using a bare requirements.txt file.
-        self.sd.pkg_manager = "req_txt"
-        self.sd.req_txt_path = self.sd.git_path / "requirements.txt"
-        self.sd.log_info("    Package manager set to req_txt.")
-        self.sd.log_info(f"    req_txt path: {self.sd.req_txt_path}")
-    
+        if confirmed:
+            self.write_output("Automating all steps...")
+        else:
+            # Quit with a message, but don't raise an error.
+            self.write_output(d_msgs.cancel_automate_all)
+            sys.exit()
```

### Comparing `django-simple-deploy-0.6.1/simple_deploy/management/commands/heroku/deploy_messages.py` & `django_simple_deploy-0.6.2/simple_deploy/management/commands/heroku/deploy_messages.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,39 +19,65 @@
 - Open your deployed project in a new browser tab.
 """
 
 no_heroku_app_detected = """No Heroku app name has been detected.
 
 - The simple_deploy command assumes you have already run 'heroku create'
   to start the deployment process.
-- Please run 'heroku create', and then run
-  'python manage.py simple_deploy' again.
+- Please run 'heroku create', and then run 'python manage.py simple_deploy' again.
 - If you haven't already done so, you will need to install the Heroku CLI:
   https://devcenter.heroku.com/articles/heroku-cli
 """
 
 cli_not_installed = """
 In order to deploy to Heroku, you need to install the Heroku CLI.
   See here: https://devcenter.heroku.com/articles/heroku-cli
 After installing the CLI, you can run simple_deploy again.
 """
 
+cli_not_authenticated = """
+In order to deploy to Heroku, you must be authenticated through the Heroku CLI.
+Please run `heroku login`, and then run simple_deploy again.
+"""
+
+heroku_settings_found = """
+There is already a Heroku-specific settings block in settings.py. Is it okay to
+overwrite this block, and everything that follows in settings.py?
+"""
+
+cant_overwrite_settings = """
+In order to configure the project for deployment, we need to write a Heroku-specific
+settings block. Please remove the current Heroku-specific settings, and then run
+simple_deploy again.
+"""
+
+procfile_found = """
+A Procfile already exists. Is it okay to overwrite this file?
+"""
+
+cant_overwrite_procfile = """
+In order to configure the project for deployment, we need to write a Procfile. Please
+remove the current Procfile, and then run simple_deploy again.
+"""
+
 
 # --- Dynamic strings ---
-# These need to be generated in functions, to display information that's 
+# These need to be generated in functions, to display information that's
 #   determined as the script runs.
 
+
 def success_msg(pkg_manager, heroku_app_name):
     """Success message, when not using --automate-all flag."""
 
     # You can't use backslashes in f-strings, so this is the cleanest way I
     #   can add a pipenv line when needed.
-    newline = '\n'
+    newline = "\n"
 
-    msg = dedent(f"""
+    msg = dedent(
+        f"""
 
         --- Your project is now configured for deployment on Heroku. ---
         
         To deploy your project, you will need to:
         - Commit the changes made in the configuration process.
         - Push the changes to Heroku.
         - Migrate the database on Heroku.
@@ -61,28 +87,30 @@
         $ git commit -am "Configured for Heroku deployment."
         $ git push heroku main
         $ heroku run python manage.py migrate
         
         After this, you can see your project by running 'heroku open'.
         Or, you can visit https://{heroku_app_name}.herokuapp.com.
 
-    """)
+    """
+    )
     return msg
 
 
 def success_msg_automate_all(heroku_app_name, current_branch):
     """Success message, when using --automate-all."""
 
     # Set correct command for pushing to heroku.
-    if current_branch in ('main', 'master'):
+    if current_branch in ("main", "master"):
         push_command = f"$ git push heroku {current_branch}"
     else:
         push_command = f"$ git push heroku {current_branch}:main"
 
-    msg = dedent(f"""
+    msg = dedent(
+        f"""
 
         --- Your project should now be deployed on Heroku. ---
 
         It should have opened up in a new browser tab.
         - If you see the message "There's nothing here, yet"
           try waiting a moment and then refreshing your browser.
         - Sometimes when the process is automated there's a little lag
@@ -95,9 +123,10 @@
 
         Also, if you haven't already done so you should review the
         documentation for Python deployments on Heroku at:
         - https://devcenter.heroku.com/categories/python-support
         - This documentation will help you understand how to maintain
           your deployment.
 
-    """)
-    return msg
+    """
+    )
+    return msg
```

### Comparing `django-simple-deploy-0.6.1/simple_deploy/management/commands/platform_sh/deploy.py` & `django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/deploy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,465 +1,433 @@
 """Manages all platform.sh-specific aspects of the deployment process."""
 
 # Note: All public-facing references to platform.sh will include a dot, dash, or
 #  underscore, ie platform_sh.
 #  Internally, we won't use a space, ie platformsh or plsh.
 
-import sys, os, re, subprocess, time
+import sys, os, subprocess, time
 from pathlib import Path
 
 from django.conf import settings
 from django.core.management.utils import get_random_secret_key
 from django.utils.crypto import get_random_string
 from django.utils.safestring import mark_safe
 
 from simple_deploy.management.commands import deploy_messages as d_msgs
 from simple_deploy.management.commands.platform_sh import deploy_messages as plsh_msgs
 
-from simple_deploy.management.commands.utils import write_file_from_template, SimpleDeployCommandError
+from simple_deploy.management.commands.utils import SimpleDeployCommandError
+from simple_deploy.management.commands import utils as sd_utils
+from simple_deploy.management.commands.platform_sh import utils as plsh_utils
 
 
 class PlatformDeployer:
-    """Perform the initial deployment of a simple project.
-    Configure as much as possible automatically.
+    """Perform the initial deployment to Platform.sh.
+
+    If --automate-all is used, carry out an actual deployment.
+    If not, do all configuration work so the user only has to commit changes, and call
+    `platform push`.
     """
 
     def __init__(self, command):
         """Establishes connection to existing simple_deploy command object."""
         self.sd = command
         self.stdout = self.sd.stdout
+        self.messages = plsh_msgs
 
+    # --- Public methods ---
 
     def deploy(self, *args, **options):
-        self.sd.write_output("Configuring project for deployment to Platform.sh...")
+        """Coordinate the overall configuration and deployment."""
 
-        self._add_platformsh_settings()
+        self.sd.write_output("\nConfiguring project for deployment to Platform.sh...")
 
-        # DEV: Group this with later yaml generation methods.
-        self._generate_platform_app_yaml()
+        self._confirm_preliminary()
 
-        self._add_requirements()
+        if self.sd.automate_all:
+            self._confirm_automate_all()
+
+        self._validate_platform()
 
-        # DEV: These could be refactored.
+        if self.sd.automate_all:
+            self._prep_automate_all()
+
+        self._add_platformsh_settings()
+        self._add_requirements()
+        self._generate_platform_app_yaml()
         self._make_platform_dir()
         self._generate_services_yaml()
-
         self._conclude_automate_all()
-
         self._show_success_message()
 
+    # --- Helper methods for deploy() ---
 
-    # --- Methods used in this class ---
+    def _confirm_preliminary(self):
+        """Confirm acknwledgement of preliminary (pre-1.0) state of project."""
+        self.sd.write_output(self.messages.confirm_preliminary)
 
-    def _add_platformsh_settings(self):
-        """Add platformsh-specific settings."""
-        # The only project-specific setting is the ALLOWED_HOSTS; that makes
-        #   modifying settings *much* easier than for other platforms.
-        #   Just check if the settings are present, and if not, dump them in.
+        # Unit test check is here, so message is logged.
+        if self.sd.unit_testing:
+            return
 
-        # DEV: Modify this to make a more specific ALLOWED_HOSTS entry.
-        #   For now, at proof of concept stage, it's just '*'.
+        if self.sd.get_confirmation():
+            self.sd.write_output("  Continuing with platform.sh deployment...")
+        else:
+            # Quit and invite the user to try another platform. We are happily exiting
+            # the script; there's no need to raise an error.
+            self.sd.write_output(self.messages.cancel_plsh)
+            sys.exit()
 
-        self.sd.write_output("\n  Checking if platform.sh-specific settings present in settings.py...")
+    def _validate_platform(self):
+        """Make sure the local environment and project supports deployment to
+        Platform.sh.
 
-        with open(self.sd.settings_path) as f:
-            settings_string = f.read()
+        Make sure CLI is installed, and user is authenticated. Make sure necessary
+        resources have been created and identified, and that we have the user's
+        permission to use those resources.
 
-        if 'if os.environ.get("PLATFORM_APPLICATION_NAME"):' in settings_string:
-            self.sd.write_output("\n    Found platform.sh settings block in settings.py.")
+        Returns:
+            None
+
+        Raises:
+            SimpleDeployCommandError: If we find any reason deployment won't work.
+        """
+        if self.sd.unit_testing:
+            # Unit tests don't use the CLI. Use the deployed project name that was
+            # passed to the simple_deploy CLI.
+            self.deployed_project_name = self.sd.deployed_project_name
+            self.sd.log_info(f"Deployed project name: {self.deployed_project_name}")
             return
 
-        # Add platformsh settings block.
-        self.sd.write_output("    No platform.sh settings found in settings.py; adding settings...")
+        self._validate_cli()
 
-        safe_settings_string = mark_safe(settings_string)
-        context = {'current_settings': safe_settings_string}
-        path = Path(self.sd.settings_path)
-        write_file_from_template(path, 'settings.py', context)
+        self.deployed_project_name = self._get_platformsh_project_name()
+        self.sd.log_info(f"Deployed project name: {self.deployed_project_name}")
 
-        msg = f"    Modified settings.py file: {path}"
-        self.sd.write_output(msg)
+        self.org_name = self._get_org_name()
+        self.sd.log_info(f"\nOrg name: {self.org_name}")
+
+    def _add_platformsh_settings(self):
+        """Add platformsh-specific settings.
 
+        The only project-specific setting is ALLOWED_HOSTS. That makes modifying
+        settings *much* easier than for other platforms. Just check if the settings are
+        present, and if not, dump them in.
 
-    def _get_platformsh_settings(self):
-        """Get any platformsh-specific settings that are already in place.
+        DEV: Modify this to make a more specific ALLOWED_HOSTS entry instead of "*".
         """
-        # If any platformsh settings have already been written, we don't want to
-        #  add them again. This assumes a section at the end, starting with a
-        #  check for `if config.is_valid_platform():`
-
-        with open(self.sd.settings_path) as f:
-            settings_lines = f.readlines()
-
-        self.found_platformsh_settings = False
-        self.current_platformsh_settings_lines = []
-        for line in settings_lines:
-            if 'if os.environ.get("PLATFORM_APPLICATION_NAME"):' in line:
-                self.found_platformsh_settings = True
-            if self.found_platformsh_settings:
-                self.current_platformsh_settings_lines.append(line)
+        self.sd.write_output(
+            "\n  Checking if Platform.sh-specific settings present in settings.py..."
+        )
+
+        # PLATFORM_APPLICATION_NAME is an env var that's reliably set in the Platform.sh
+        # environment.
+        # See: https://docs.platform.sh/development/variables/use-variables.html#use-provided-variables
+        settings_string = self.sd.settings_path.read_text()
+        if 'if os.environ.get("PLATFORM_APPLICATION_NAME"):' in settings_string:
+            self.sd.write_output(
+                "\n    Found platform.sh settings block in settings.py."
+            )
+            return
 
+        # Add platformsh settings block.
+        self.sd.write_output(
+            "    No platform.sh settings found in settings.py; adding settings..."
+        )
+
+        safe_settings_string = mark_safe(settings_string)
+        context = {"current_settings": safe_settings_string}
+        sd_utils.write_file_from_template(self.sd.settings_path, "settings.py", context)
+
+        msg = f"    Modified settings.py file: {self.sd.settings_path}"
+        self.sd.write_output(msg)
 
     def _generate_platform_app_yaml(self):
         """Create .platform.app.yaml file, if not present."""
 
-        # File should be in project root, if present.
-        self.sd.write_output(f"\n  Looking in {self.sd.git_path} for .platform.app.yaml file...")
-        p_app_yaml_present = '.platform.app.yaml' in os.listdir(self.sd.git_path)
+        path = self.sd.project_root / ".platform.app.yaml"
+        self.sd.write_output(f"\n  Looking for {path.as_posix()}...")
 
-        if p_app_yaml_present:
+        if path.exists():
             self.sd.write_output("    Found existing .platform.app.yaml file.")
         else:
             # Generate file from template.
-            self.sd.write_output("    No .platform.app.yaml file found. Generating file...")
+            self.sd.write_output(
+                "    No .platform.app.yaml file found. Generating file..."
+            )
 
             context = {
-                'project_name': self.sd.project_name, 
-                'deployed_project_name': self.deployed_project_name
-                }
-            path = self.sd.project_root / '.platform.app.yaml'
-            if self.sd.pkg_manager == 'poetry':
-                template_path = 'poetry.platform.app.yaml'
+                "project_name": self.sd.local_project_name,
+                "deployed_project_name": self.deployed_project_name,
+            }
+
+            if self.sd.pkg_manager == "poetry":
+                template_path = "poetry.platform.app.yaml"
             elif self.sd.pkg_manager == "pipenv":
-                template_path = 'pipenv.platform.app.yaml'
+                template_path = "pipenv.platform.app.yaml"
             else:
-                template_path = 'platform.app.yaml'
-            write_file_from_template(path, template_path, context)
+                template_path = "platform.app.yaml"
+            sd_utils.write_file_from_template(path, template_path, context)
 
-            msg = f"\n    Generated .platform.app.yaml file: {path}"
+            msg = f"\n    Generated {path.as_posix()}"
             self.sd.write_output(msg)
             return path
 
-
     def _add_requirements(self):
-        """Add requirements for serving on Platform.sh."""
+        """Add requirements for Platform.sh."""
         requirements = ["platformshconfig", "gunicorn", "psycopg2"]
         self.sd.add_packages(requirements)
 
-
-    def _check_allowed_hosts(self):
-        """Make sure project can be served from platformsh."""
-        # This method is specific to platformsh.
-
-        self.sd.write_output("\n  Making sure project can be served from platform.sh...")
-
-        # DEV: Configure an ALLOWED_HOSTS entry that's specific to this deployment.
-        # Use '*' for now, to focus on more specific aspects of platformsh deployment.
-        platformsh_host = '*'
-
-        if platformsh_host in settings.ALLOWED_HOSTS:
-            self.sd.write_output(f"    Found {platformsh_host} in ALLOWED_HOSTS.")
-        else:
-            new_setting = f"ALLOWED_HOSTS.append('{platformsh_host}')"
-            msg_added = f"    Added {platformsh_host} to ALLOWED_HOSTS for the deployed project."
-            msg_already_set = f"    Found {platformsh_host} in ALLOWED_HOSTS for the deployed project."
-            self._add_platformsh_setting(new_setting, msg_added, msg_already_set)
-
-
     def _make_platform_dir(self):
         """Add a .platform directory, if it doesn't already exist."""
 
-        # Directory should be in project root, if present.
-        self.sd.write_output(f"\n  Looking in {self.sd.git_path} for .platform/ directory...")
+        self.platform_dir_path = self.sd.project_root / ".platform"
+        self.sd.write_output(f"\n  Looking for {self.platform_dir_path.as_posix()}...")
 
-        self.platform_dir_path = self.sd.git_path / '.platform'
         if self.platform_dir_path.exists():
-            self.sd.write_output("    Found existing .platform/ directory.")
+            self.sd.write_output(f"    Found {self.platform_dir_path.as_posix()}")
         else:
             self.platform_dir_path.mkdir()
-            self.sd.write_output(f"    Made .platform directory: {self.platform_dir_path}")
-
+            self.sd.write_output(f"    Generated {self.platform_dir_path.as_posix()}")
 
     def _generate_services_yaml(self):
         """Generate the .platform/services.yaml file, if not present."""
-        
-        # File should be in self.platform_dir_path, if present.
-        self.sd.write_output(f"\n  Looking in {self.platform_dir_path} for services.yaml file...")
-        services_yaml_present = 'services.yaml' in os.listdir(self.platform_dir_path)
 
-        if services_yaml_present:
+        path = self.platform_dir_path / "services.yaml"
+        self.sd.write_output(f"\n  Looking for {path.as_posix()}...")
+
+        if path.exists():
             self.sd.write_output("    Found existing services.yaml file.")
         else:
-            # Generate file from template.
             self.sd.write_output("    No services.yaml file found. Generating file...")
-            path = self.platform_dir_path / 'services.yaml'
-            write_file_from_template(path, 'services.yaml')
+            sd_utils.write_file_from_template(path, "services.yaml")
 
-            msg = f"\n    Generated services.yaml file: {path}"
+            msg = f"\n    Generated {path.as_posix()}"
             self.sd.write_output(msg)
             return path
 
-
     def _conclude_automate_all(self):
         """Finish automating the push to Platform.sh.
+
         - Commit all changes.
         - Call `platform push`.
         - Open project.
         """
         # Making this check here lets deploy() be cleaner.
         if not self.sd.automate_all:
             return
 
         self.sd.commit_changes()
 
         # Push project.
-        # Use execute_command(), to stream the output as it runs.
         self.sd.write_output("  Pushing to Platform.sh...")
 
-        # Pause to make sure project that was created can be used.
+        # Pause to make sure project that was just created can be used.
         self.sd.write_output("    Pausing 10s to make sure project is ready to use...")
         time.sleep(10)
 
+        # Use run_slow_command(), to stream output as it runs.
         cmd = "platform push --yes"
-        self.sd.log_info(cmd)
-        self.sd.execute_command(cmd)
+        self.sd.run_slow_command(cmd)
 
         # Open project.
         self.sd.write_output("  Opening deployed app in a new browser tab...")
         cmd = "platform url --yes"
-        output = self.sd.execute_subp_run(cmd)
-        self.sd.log_info(cmd)
+        output = self.sd.run_quick_command(cmd)
         self.sd.write_output(output)
 
         # Get url of deployed project.
         #   This can be done with an re, but there's one line of output with
         #   a url, so finding that line is simpler.
-        self.deployed_url = ''
-        for line in output.stdout.decode().split('\n'):
-            if 'https' in line:
+        # DEV: Move this to a utility, and write a test against standard Platform.sh
+        # output.
+        self.deployed_url = ""
+        for line in output.stdout.decode().split("\n"):
+            if "https" in line:
                 self.deployed_url = line.strip()
 
-
     def _show_success_message(self):
         """After a successful run, show a message about what to do next."""
 
         # DEV:
-        # - Mention that this script should not need to be run again, unless
-        #   creating a new deployment.
-        #   - Describe ongoing approach of commit, push, migrate. Lots to consider
-        #     when doing this on production app with users, make sure you learn.
+        # - Mention that this script should not need to be run again unless creating
+        #   a new deployment.
+        # - Describe ongoing approach of commit, push, migrate. Lots to consider
+        #   when doing this on production app with users, make sure you learn.
 
         if self.sd.automate_all:
-            msg = plsh_msgs.success_msg_automate_all(self.deployed_url)
+            msg = self.messages.success_msg_automate_all(self.deployed_url)
             self.sd.write_output(msg)
         else:
-            msg = plsh_msgs.success_msg(self.sd.log_output)
+            msg = self.messages.success_msg(self.sd.log_output)
             self.sd.write_output(msg)
 
+    # --- Other helper methods ---
 
-    # --- Methods called from simple_deploy.py ---
+    def _prep_automate_all(self):
+        """Intial work for automating entire process.
 
-    def confirm_preliminary(self):
-        """Deployment to platform.sh is in a preliminary state, and we need to be
-        explicit about that.
-        """
-        # Skip this confirmation when unit testing.
-        if self.sd.unit_testing:
-            return
-
-        self.sd.write_output(plsh_msgs.confirm_preliminary)
-        confirmed = self.sd.get_confirmation()
-
-        if confirmed:
-            self.sd.write_output("  Continuing with platform.sh deployment...")
-        else:
-            # Quit and invite the user to try another platform.
-            # We are happily exiting the script; there's no need to raise a
-            #   CommandError.
-            self.sd.write_output(plsh_msgs.cancel_plsh)
-            sys.exit()
-
-
-    def validate_platform(self):
-        """Make sure the local environment and project supports deployment to
-        Platform.sh.
-        
-        The returncode for a successful command is 0, so anything truthy means
-          a command errored out.
-        """
-
-        # When running unit tests, will not be logged into CLI.
-        if not self.sd.unit_testing:
-            self._validate_cli()
-            
-            self.deployed_project_name = self._get_platformsh_project_name()
-            self.org_name = self._get_org_name()
-
-            # Log org name here, because it doesn't apply to unit testing.
-            self.sd.log_info(f"\nOrg name: {self.org_name}")
-        else:
-            self.deployed_project_name = self.sd.deployed_project_name
-
-        self.sd.log_info(f"Deployed project name: {self.deployed_project_name}")
-
-
-    def prep_automate_all(self):
-        """Do intial work for automating entire process.
-        We know from validate_project() that user is logged into CLI.
-        
         Returns:
-        - None if creation was successful.
-        - Should raise CommandError if create command fails.
+            None: If creation of new project was successful.
+
+        Raises:
+            SimpleDeployCommandError: If create command fails.
 
         Note: create command outputs project id to stdout if known, all other
           output goes to stderr.
         """
 
         self.sd.write_output("  Running `platform create`...")
         self.sd.write_output("    (Please be patient, this can take a few minutes.")
-        cmd = f'platform create --title { self.deployed_project_name } --org {self.org_name} --region {self.sd.region} --yes'
-        self.sd.log_info(cmd)
+        cmd = f"platform create --title { self.deployed_project_name } --org {self.org_name} --region {self.sd.region} --yes"
 
         try:
             # Note: if user can't create a project the returncode will be 6, not 1.
             #   This may affect whether a CompletedProcess is returned, or an Exception
             # is raised.
-            self.sd.execute_command(cmd)
+            # Also, create command outputs project id to stdout if known, all other
+            # output goes to stderr.
+            self.sd.run_slow_command(cmd)
         except subprocess.CalledProcessError as e:
-            error_msg = plsh_msgs.unknown_create_error(e)
+            error_msg = self.messages.unknown_create_error(e)
             raise SimpleDeployCommandError(self.sd, error_msg)
 
-
     # --- Helper methods for methods called from simple_deploy.py ---
 
     def _validate_cli(self):
         """Make sure the Platform.sh CLI is installed, and user is authenticated."""
-        cmd = 'platform --version'
-        self.sd.log_info(cmd)
+        cmd = "platform --version"
 
+        # This generates a FileNotFoundError on Ubuntu if the CLI is not installed.
         try:
-            output_obj = self.sd.execute_subp_run(cmd)
+            output_obj = self.sd.run_quick_command(cmd)
         except FileNotFoundError:
-            raise SimpleDeployCommandError(self.sd, plsh_msgs.cli_not_installed)
-        else:
-            # Log the version output.
-            self.sd.log_info(output_obj)
-            
+            raise SimpleDeployCommandError(self.sd, self.messages.cli_not_installed)
+
+        self.sd.log_info(output_obj)
+
         # Check that the user is authenticated.
         cmd = "platform auth:info --no-interaction"
-        self.sd.log_info(cmd)
-        output_obj = self.sd.execute_subp_run(cmd)
-        output_str = output_obj.stdout.decode()
-        output_err = output_obj.stderr.decode()
-        
-        if "Authentication is required." in output_err:
-            raise SimpleDeployCommandError(self.sd, plsh_msgs.cli_logged_out)
+        output_obj = self.sd.run_quick_command(cmd)
 
+        if "Authentication is required." in output_obj.stderr.decode():
+            raise SimpleDeployCommandError(self.sd, self.messages.cli_logged_out)
 
     def _get_platformsh_project_name(self):
         """Get the deployed project name.
-        This is the name that was given in the `platform create` command.
+
+        If using automate_all, we'll set this. Otherwise, we're looking for the name
+        that was given in the `platform create` command.
         - Try to get this from `project:info`.
         - If can't get project name:
           - Exit with warning, and inform user of --deployed-project-name
             flag to override this error.
+
+        Retuns:
+            str: The deployed project name.
+        Raises:
+            SimpleDeployCommandError: If deployed project name can't be found.
         """
         # If we're creating the project, we'll just use the startproject name.
         if self.sd.automate_all:
-            return self.sd.project_name
+            return self.sd.local_project_name
 
         # Use the provided name if --deployed-project-name specified.
         if self.sd.deployed_project_name:
             return self.sd.deployed_project_name
 
         # Use --yes flag to avoid interactive prompt hanging in background
         #   if the user is not currently logged in to the CLI.
-        cmd = "platform project:info --yes"
-        output_obj = self.sd.execute_subp_run(cmd)
+        cmd = "platform project:info --yes --format csv"
+        output_obj = self.sd.run_quick_command(cmd)
         output_str = output_obj.stdout.decode()
 
+        # Log cmd, but don't log the output of `project:info`. It contains identifying
+        # information about the user and project, including client_ssh_key.
         self.sd.log_info(cmd)
-        # Don't log the output of `project:info`. It contains identifying information
-        #   about the user and project, including client_ssh_key.
 
         # If there's no stdout, the user is probably logged out, hasn't called
         #   create, or doesn't have the CLI installed.
         # Also, I've seen both ProjectNotFoundException and RootNotFoundException
         #   raised when no project has been created.
         if not output_str:
             output_str = output_obj.stderr.decode()
-            if 'LoginRequiredException' in output_str:
-                raise SimpleDeployCommandError(self.sd, plsh_msgs.login_required)
-            elif 'ProjectNotFoundException' in output_str:
-                raise SimpleDeployCommandError(self.sd, plsh_msgs.no_project_name)
-            elif 'RootNotFoundException' in output_str:
-                raise SimpleDeployCommandError(self.sd, plsh_msgs.no_project_name)
+            if "LoginRequiredException" in output_str:
+                raise SimpleDeployCommandError(self.sd, self.messages.login_required)
+            elif "ProjectNotFoundException" in output_str:
+                raise SimpleDeployCommandError(self.sd, self.messages.no_project_name)
+            elif "RootNotFoundException" in output_str:
+                raise SimpleDeployCommandError(self.sd, self.messages.no_project_name)
             else:
-                error_msg = plsh_msgs.unknown_error
-                error_msg += plsh_msgs.cli_not_installed
+                error_msg = self.messages.unknown_error
+                error_msg += self.messages.cli_not_installed
                 raise SimpleDeployCommandError(self.sd, error_msg)
 
         # Pull deployed project name from output.
-        deployed_project_name_re = r'(\| title\s+?\|\s*?)(.*?)(\s*?\|)'
-        match = re.search(deployed_project_name_re, output_str)
-        if match:
-            return match.group(2).strip()
-        
-        # Couldn't find a project name. Warn user, and let them know
-        #   about override flag.
-        raise SimpleDeployCommandError(self.sd, plsh_msgs.no_project_name)
+        lines = output_str.splitlines()
+        title_line = [line for line in lines if "title," in line][0]
+        # Assume first project is one to use.
+        project_name = title_line.split(",")[1].strip()
+        project_name = plsh_utils.get_project_name(output_str)
+        if project_name:
+            return project_name
 
+        # Couldn't find a project name. Warn user, and tell them about override flag.
+        raise SimpleDeployCommandError(self.sd, self.messages.no_project_name)
 
     def _get_org_name(self):
-        """Get the organization name associated with the user's Platform.sh
-        account. This is needed for creating a project using automate_all.
+        """Get the organization name associated with the user's Platform.sh account.
 
+        This is needed for creating a project using automate_all.
         Confirm that it's okay to use this org.
 
         Returns:
-        - None if not using automate-all.
-        - String containing org name if found, and confirmed.
-        - Raises CommandError if org name found, but not confirmed.
-        - Raises CommandError with msg if CLI login required.
-        - Raises CommandError with msg if org name not found.
+            str: org name
+            None: if not using automate-all
+        Raises:
+            SimpleDeployCommandError:
+            - if org name found, but not confirmed.
+            - if org name not found
         """
         if not self.sd.automate_all:
             return
 
-        # Use --yes to suppress hanging at login prompt.
-        cmd = "platform organization:list --yes"
-        output_obj = self.sd.execute_subp_run(cmd)
+        cmd = "platform organization:list --yes --format csv"
+        output_obj = self.sd.run_quick_command(cmd)
         output_str = output_obj.stdout.decode()
-        self.sd.log_info(cmd)
         self.sd.log_info(output_str)
 
         if not output_str:
             output_str = output_obj.stderr.decode()
-            if 'LoginRequiredException' in output_str:
-                raise SimpleDeployCommandError(self.sd, plsh_msgs.login_required)
+            if "LoginRequiredException" in output_str:
+                raise SimpleDeployCommandError(self.sd, self.messages.login_required)
             else:
-                error_msg = plsh_msgs.unknown_error
-                error_msg += plsh_msgs.cli_not_installed
+                error_msg = self.messages.unknown_error
+                error_msg += self.messages.cli_not_installed
                 raise SimpleDeployCommandError(self.sd, error_msg)
 
-        # Pull org name from output. Start by removing line containing lables.
-        output_str_lines = [line for line in output_str.split("\n") if "Owner email" not in line]
-        modified_output_str = '\n'.join(output_str_lines)
-        org_name_re = r'(\|\s*)([a-zA-Z_]*)(.*)'
-        match = re.search(org_name_re, modified_output_str)
-        if match:
-            org_name = match.group(2).strip()
-            if self._confirm_use_org_name(org_name):
-                return org_name
-        else:
-            # Got stdout, but can't find org id. Unknown error.
-            raise SimpleDeployCommandError(self.sd, plsh_msgs.org_not_found)
+        org_name = plsh_utils.get_org_name(output_str)
+        if not org_name:
+            raise SimpleDeployCommandError(self.sd, self.messages.org_not_found)
 
+        if self._confirm_use_org_name(org_name):
+            return org_name
 
     def _confirm_use_org_name(self, org_name):
         """Confirm that it's okay to use the org name that was found.
+
         Returns:
-        - True if confirmed.
-        - sys.exit() if not confirmed.
+            True: if confirmed
+            SimpleDeployCommandError: if not confirmed
         """
 
-        self.stdout.write(plsh_msgs.confirm_use_org_name(org_name))
+        self.stdout.write(self.messages.confirm_use_org_name(org_name))
         confirmed = self.sd.get_confirmation(skip_logging=True)
 
         if confirmed:
             self.stdout.write("  Okay, continuing with deployment.")
             return True
         else:
             # Exit, with a message that configuration is still an option.
-            msg = plsh_msgs.cancel_plsh
-            msg += plsh_msgs.may_configure
+            msg = self.messages.cancel_plsh
+            msg += self.messages.may_configure
             raise SimpleDeployCommandError(self.sd, msg)
```

### Comparing `django-simple-deploy-0.6.1/simple_deploy/management/commands/platform_sh/deploy_messages.py` & `django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/deploy_messages.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,18 @@
 
 from textwrap import dedent
 
 from django.conf import settings
 
 
 confirm_preliminary = """
-***** Deployments to platform.sh are experimental at this point ***
+***** Deployment to platform.sh is under active development at this point ***
 
-- Support for deploying to platform.sh is in an exploratory phase at this point.
-- You should only be using this project to deploy to platform.sh at this point if
-  you are interested in helping to develop or test the simple_deploy project.
-- You should look at the deploy_platformsh.py script before running this command,
-  so you know what kinds of changes will be made to your project.
-- You should understand the platform.sh console, and be comfortable deleting resources
-  that are created during this deployment.
-- You may want to cancel this run and deploy to a different platform.
+- If you already have a project deployed on Platform.sh, configuration will fail.
+- If you have more than one org on Platform.sh, configuration will fail.
 """
 
 confirm_automate_all = """
 The --automate-all flag means simple_deploy will:
 - Run `platform create` for you, to create an empty Platform.sh project.
   - This will create a project in the us-3.platform.sh region. If you wish
     to use a different region, cancel this operation and use the --region flag.
@@ -88,40 +82,44 @@
 
 You will have to create the Platform.sh project yourself, but simple_deploy
 will do all of the necessary configuration for deployment.
 """
 
 
 # --- Dynamic strings ---
-# These need to be generated in functions, to display information that's 
+# These need to be generated in functions, to display information that's
 #   determined as the script runs.
 
+
 def confirm_use_org_name(org_name):
     """Confirm use of this org name to create a new project."""
 
-    msg = dedent(f"""
+    msg = dedent(
+        f"""
         --- The Platform.sh CLI requires an organization name when creating a new project. ---
         When using --automate-all, a project will be created on your behalf. The following
         organization name was found: {org_name}
 
         This organization will be used to create a new project. If this is not okay,
         enter n to cancel this operation.
-    """)
+    """
+    )
 
     return msg
 
 
 def unknown_create_error(e):
-    """Process a non-specific error when running `platform create` 
+    """Process a non-specific error when running `platform create`
     while using automate_all. This is most likely an issue with the user
     not having permission to create a new project, for example because they
     are on a trial plan and have already created too many projects.
     """
 
-    msg = dedent(f"""
+    msg = dedent(
+        f"""
         --- An error has occurred when trying to create a new Platform.sh project. ---
 
         While running `platform create`, an error has occurred. You should check
         the Platform.sh console to see if a project was partially created.
 
         The error messages that Platform.sh provides, both through the CLI and
         the console, are not always specific enough to be helpful. For example, 
@@ -132,23 +130,25 @@
 
         The following output may help diagnose the error:
         ***** output of `platform create` *****
 
         {e.stderr.decode()}
 
         ***** end output *****
-    """)
+    """
+    )
 
     return msg
 
 
-def success_msg(log_output=''):
+def success_msg(log_output=""):
     """Success message, for configuration-only run."""
 
-    msg = dedent(f"""
+    msg = dedent(
+        f"""
         --- Your project is now configured for deployment on Platform.sh. ---
 
         To deploy your project, you will need to:
         - Commit the changes made in the configuration process.
             $ git status
             $ git add .
             $ git commit -am "Configured project for deployment."
@@ -156,28 +156,32 @@
             $ platform push
         - Open your project:
             $ platform url    
         - As you develop your project further:
             - Make local changes
             - Commit your local changes
             - Run `platform push`
-    """)
+    """
+    )
 
     if log_output:
-        msg += dedent(f"""
+        msg += dedent(
+            f"""
         - You can find a full record of this configuration in the simple_deploy_logs directory.
-        """)
+        """
+        )
 
     return msg
 
 
 def success_msg_automate_all(deployed_url):
     """Success message, when using --automate-all."""
 
-    msg = dedent(f"""
+    msg = dedent(
+        f"""
 
         --- Your project should now be deployed on Platform.sh. ---
 
         It should have opened up in a new browser tab.
         - You can also visit your project at {deployed_url}
 
         If you make further changes and want to push them to Platform.sh,
@@ -185,9 +189,10 @@
 
         Also, if you haven't already done so you should review the
         documentation for Python deployments on Platform.sh at:
         - https://docs.platform.sh/languages/python.html
         - This documentation will help you understand how to maintain
           your deployment.
 
-    """)
+    """
+    )
     return msg
```

### Comparing `django-simple-deploy-0.6.1/simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml` & `django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/pipenv.platform.app.yaml`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/simple_deploy/management/commands/platform_sh/templates/platform.app.yaml` & `django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/platform.app.yaml`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml` & `django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/poetry.platform.app.yaml`

 * *Files identical despite different names*

### Comparing `django-simple-deploy-0.6.1/simple_deploy/management/commands/platform_sh/templates/settings.py` & `django_simple_deploy-0.6.2/simple_deploy/management/commands/platform_sh/templates/settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-{{ current_settings }}
+{{current_settings}}
 
 # Platform.sh settings.
 import os
+
 if os.environ.get("PLATFORM_APPLICATION_NAME"):
     # Import some Platform.sh settings from the environment.
     from platformshconfig import Config
 
     config = Config()
 
-    ALLOWED_HOSTS.append('*')
+    ALLOWED_HOSTS.append("*")
     DEBUG = False
 
-    STATIC_URL = '/static/'
+    STATIC_URL = "/static/"
 
     if config.appDir:
-        STATIC_ROOT = os.path.join(config.appDir, 'static')
+        STATIC_ROOT = os.path.join(config.appDir, "static")
     if config.projectEntropy:
         SECRET_KEY = config.projectEntropy
 
     if not config.in_build():
-        db_settings = config.credentials('database')
+        db_settings = config.credentials("database")
         DATABASES = {
-            'default': {
-                'ENGINE': 'django.db.backends.postgresql',
-                'NAME': db_settings['path'],
-                'USER': db_settings['username'],
-                'PASSWORD': db_settings['password'],
-                'HOST': db_settings['host'],
-                'PORT': db_settings['port'],
+            "default": {
+                "ENGINE": "django.db.backends.postgresql",
+                "NAME": db_settings["path"],
+                "USER": db_settings["username"],
+                "PASSWORD": db_settings["password"],
+                "HOST": db_settings["host"],
+                "PORT": db_settings["port"],
+            },
+            "sqlite": {
+                "ENGINE": "django.db.backends.sqlite3",
+                "NAME": os.path.join(BASE_DIR, "db.sqlite3"),
             },
-            'sqlite': {
-                'ENGINE': 'django.db.backends.sqlite3',
-                'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
-            }
-        }
+        }
```

