# Comparing `tmp/dpdispatcher-0.6.4.tar.gz` & `tmp/dpdispatcher-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpdispatcher-0.6.4.tar", last modified: Sun Jan 21 20:29:49 2024, max compression
+gzip compressed data, was "dpdispatcher-0.6.5.tar", last modified: Mon May 27 14:48:53 2024, max compression
```

## Comparing `dpdispatcher-0.6.4.tar` & `dpdispatcher-0.6.5.tar`

### file list

```diff
@@ -1,304 +1,333 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.233169 dpdispatcher-0.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.193168 dpdispatcher-0.6.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.193168 dpdispatcher-0.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/.github/workflows/ci-docker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/.github/workflows/machines.yml
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/.github/workflows/mirror_gitee.yml
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/.github/workflows/publish_conda.yml
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/.github/workflows/pyright.yml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/.github/workflows/test-bohrium.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-01-21 20:29:49.229169 dpdispatcher-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.193168 dpdispatcher-0.6.4/ci/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/ci/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/ci/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.193168 dpdispatcher-0.6.4/ci/pbs/
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/ci/pbs/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/ci/pbs/start-pbs.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      665 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/ci/pbs.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.193168 dpdispatcher-0.6.4/ci/slurm/
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/ci/slurm/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/ci/slurm/register_cluster.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      662 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/ci/slurm/start-slurm.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      423 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/ci/slurm.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.197168 dpdispatcher-0.6.4/ci/ssh/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/ci/ssh/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      302 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/ci/ssh/start-ssh.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      411 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/ci/ssh.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      586 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/ci/ssh_rsync.sh
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.197168 dpdispatcher-0.6.4/conda/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/conda/conda_build_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.197168 dpdispatcher-0.6.4/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/batch.md
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/context.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/credits.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/dpdispatcher_on_yarn.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.201168 dpdispatcher-0.6.4/doc/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/examples/expanse.md
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/examples/g16.md
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/examples/shell.md
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/examples/template.md
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/install.md
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/machine.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/doc/task.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.201168 dpdispatcher-0.6.4/dpdispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-21 20:29:49.000000 dpdispatcher-0.6.4/dpdispatcher/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/arginfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/base_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.205168 dpdispatcher-0.6.4/dpdispatcher/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/contexts/dp_cloud_server_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/contexts/hdfs_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/contexts/lazy_local_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    14052 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/contexts/local_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/contexts/openapi_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    38612 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/contexts/ssh_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/dlog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.205168 dpdispatcher-0.6.4/dpdispatcher/dpcloudserver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/dpcloudserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/dpcloudserver/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/dpdisp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.205168 dpdispatcher-0.6.4/dpdispatcher/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/entrypoints/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/entrypoints/submission.py
--rw-r--r--   0 runner    (1001) docker     (127)    16140 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.205168 dpdispatcher-0.6.4/dpdispatcher/machines/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/machines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/machines/distributed_shell.py
--rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/machines/dp_cloud_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/machines/fugaku.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/machines/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/machines/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10331 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/machines/pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/machines/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)    15611 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/machines/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)    48447 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/submission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.205168 dpdispatcher-0.6.4/dpdispatcher/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.209168 dpdispatcher-0.6.4/dpdispatcher/utils/dpcloudserver/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/utils/dpcloudserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/utils/dpcloudserver/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/utils/dpcloudserver/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/utils/dpcloudserver/retcode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/utils/dpcloudserver/zip_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/utils/hdfs_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/utils/job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/utils/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/dpdispatcher/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.229169 dpdispatcher-0.6.4/dpdispatcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-01-21 20:29:49.000000 dpdispatcher-0.6.4/dpdispatcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-01-21 20:29:49.000000 dpdispatcher-0.6.4/dpdispatcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 20:29:49.000000 dpdispatcher-0.6.4/dpdispatcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-21 20:29:49.000000 dpdispatcher-0.6.4/dpdispatcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-21 20:29:49.000000 dpdispatcher-0.6.4/dpdispatcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-21 20:29:49.000000 dpdispatcher-0.6.4/dpdispatcher.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.185168 dpdispatcher-0.6.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.209168 dpdispatcher-0.6.4/examples/machine/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/examples/machine/expanse.json
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/examples/machine/lazy_local.json
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/examples/machine/mandu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.209168 dpdispatcher-0.6.4/examples/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/examples/resources/expanse_cpu.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/examples/resources/mandu.json
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/examples/resources/template.slurm
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/examples/resources/tiger.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.209168 dpdispatcher-0.6.4/examples/task/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/examples/task/deepmd-kit.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/examples/task/g16.json
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.209168 dpdispatcher-0.6.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/scripts/script_gen_dargs_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/scripts/script_gen_dargs_json.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-21 20:29:49.233169 dpdispatcher-0.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.217168 dpdispatcher-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/batch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/context.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1843 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/debug_test_class_submission_init.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3228 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/devel_test_ali_ehpc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2669 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/devel_test_dp_cloud_server.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1752 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/devel_test_lazy_ali_ehpc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1398 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/devel_test_lsf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2357 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/devel_test_shell.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2673 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/devel_test_slurm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2629 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/devel_test_ssh_ali_ehpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/graph.pb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.217168 dpdispatcher-0.6.4/tests/jsons/
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/job.json
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/machine.json
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/machine_ali_ehpc.json
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/machine_center.json
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/machine_diffenert.json
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/machine_dp_cloud_server.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      707 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/machine_fugaku.json
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/machine_if_cuda_multi_devices.json
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/machine_lazy_local_lsf.json
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/machine_lazy_local_slurm.json
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/machine_lazylocal_shell.json
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/machine_local_fugaku.json
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/machine_local_shell.json
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/machine_lsf.json
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/machine_openapi.json
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/machine_slurm.json
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/machine_yarn.json
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/resources.json
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/submission.json
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/jsons/task.json
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/sample_class.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1074 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/script_gen_json.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/slurm_test.env
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_argcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_class_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_class_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_class_machine_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_class_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_class_submission.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_class_submission_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_class_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.185168 dpdispatcher-0.6.4/tests/test_context_dir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.217168 dpdispatcher-0.6.4/tests/test_context_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.221168 dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.221168 dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-1/some_dir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-1/some_dir/some_file
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.221168 dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.221168 dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.221168 dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-4/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.221168 dpdispatcher-0.6.4/tests/test_context_dir/0_md/dir with space/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_context_dir/0_md/dir with space/file with space
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_context_dir/0_md/graph.pb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.221168 dpdispatcher-0.6.4/tests/test_context_dir/0_md/some_dir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_context_dir/0_md/some_dir/some_file
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_group_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_hdfs_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.185168 dpdispatcher-0.6.4/tests/test_hdfs_dir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.221168 dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.221168 dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.221168 dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.221168 dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.221168 dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/bct-4/input.lammps
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/graph.pb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.185168 dpdispatcher-0.6.4/tests/test_if_cuda_multi_devices/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.221168 dpdispatcher-0.6.4/tests/test_if_cuda_multi_devices/test_dir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_if_cuda_multi_devices/test_dir/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_import_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_lazy_local_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    11278 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_local_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.185168 dpdispatcher-0.6.4/tests/test_lsf_dir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.221168 dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.221168 dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.225169 dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.225169 dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.225169 dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/bct-4/input.lammps
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/graph.pb
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/submission.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     6378 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_lsf_script_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.189168 dpdispatcher-0.6.4/tests/test_pbs_dir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.225169 dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.225169 dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.225169 dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.225169 dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.225169 dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/bct-4/input.lammps
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/graph.pb
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_run_submission.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_run_submission_bohrium.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_run_submission_ratio_unfinished.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1913 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_shell_cuda_multi_devices.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4895 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_shell_trival.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.189168 dpdispatcher-0.6.4/tests/test_shell_trival_dir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.225169 dpdispatcher-0.6.4/tests/test_shell_trival_dir/fail_dir/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_shell_trival_dir/fail_dir/mock_fail_task.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.225169 dpdispatcher-0.6.4/tests/test_shell_trival_dir/parent_dir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.225169 dpdispatcher-0.6.4/tests/test_shell_trival_dir/parent_dir/dir with space/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_shell_trival_dir/parent_dir/dir with space/example.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.225169 dpdispatcher-0.6.4/tests/test_shell_trival_dir/parent_dir/dir1/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_shell_trival_dir/parent_dir/dir1/example.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.225169 dpdispatcher-0.6.4/tests/test_shell_trival_dir/parent_dir/dir2/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_shell_trival_dir/parent_dir/dir2/example.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.225169 dpdispatcher-0.6.4/tests/test_shell_trival_dir/parent_dir/dir3/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_shell_trival_dir/parent_dir/dir3/example.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.225169 dpdispatcher-0.6.4/tests/test_shell_trival_dir/parent_dir/dir4/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_shell_trival_dir/parent_dir/dir4/example.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_shell_trival_dir/parent_dir/graph.pb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.225169 dpdispatcher-0.6.4/tests/test_shell_trival_dir/recover_dir/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_shell_trival_dir/recover_dir/mock_recover_task.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.189168 dpdispatcher-0.6.4/tests/test_slurm_dir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.229169 dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.229169 dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.229169 dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.229169 dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.229169 dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/bct-4/input.lammps
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/d3c842c5b9476e48f7145b370cd330372b9293e1.json
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/graph.pb
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/submission.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     4722 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_slurm_script_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_ssh_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:49.229169 dpdispatcher-0.6.4/tests/test_work_path/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 20:29:40.000000 dpdispatcher-0.6.4/tests/test_work_path/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.196355 dpdispatcher-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.156355 dpdispatcher-0.6.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.156355 dpdispatcher-0.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/.github/workflows/ci-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/.github/workflows/machines.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/.github/workflows/mirror_gitee.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/.github/workflows/publish_conda.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/.github/workflows/pyright.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/.github/workflows/test-bohrium.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12817 2024-05-27 14:48:53.196355 dpdispatcher-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.156355 dpdispatcher-0.6.5/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/ci/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/ci/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.156355 dpdispatcher-0.6.5/ci/pbs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/ci/pbs/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/ci/pbs/start-pbs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      695 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/ci/pbs.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.156355 dpdispatcher-0.6.5/ci/slurm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/ci/slurm/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/ci/slurm/register_cluster.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      662 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/ci/slurm/start-slurm.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      467 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/ci/slurm.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.156355 dpdispatcher-0.6.5/ci/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/ci/ssh/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      302 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/ci/ssh/start-ssh.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/ci/ssh.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      630 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/ci/ssh_rsync.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.156355 dpdispatcher-0.6.5/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/conda/conda_build_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.160355 dpdispatcher-0.6.5/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/batch.md
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/context.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/dpdispatcher_on_yarn.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.160355 dpdispatcher-0.6.5/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/examples/expanse.md
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/examples/g16.md
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/examples/shell.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/examples/template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/machine.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/pep723.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/run.md
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/doc/task.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.164355 dpdispatcher-0.6.5/dpdispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 14:48:53.000000 dpdispatcher-0.6.5/dpdispatcher/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/arginfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/base_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.164355 dpdispatcher-0.6.5/dpdispatcher/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/contexts/dp_cloud_server_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/contexts/hdfs_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/contexts/lazy_local_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14065 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/contexts/local_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/contexts/openapi_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38578 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/contexts/ssh_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/dlog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.164355 dpdispatcher-0.6.5/dpdispatcher/dpcloudserver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/dpcloudserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/dpcloudserver/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/dpdisp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.164355 dpdispatcher-0.6.5/dpdispatcher/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/entrypoints/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/entrypoints/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/entrypoints/submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16138 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.168355 dpdispatcher-0.6.5/dpdispatcher/machines/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/machines/JH_UniScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/machines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/machines/distributed_shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/machines/dp_cloud_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/machines/fugaku.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7932 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/machines/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/machines/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/machines/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/machines/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15592 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/machines/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48361 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/submission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.168355 dpdispatcher-0.6.5/dpdispatcher/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.168355 dpdispatcher-0.6.5/dpdispatcher/utils/dpcloudserver/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/utils/dpcloudserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/utils/dpcloudserver/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/utils/dpcloudserver/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/utils/dpcloudserver/retcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/utils/dpcloudserver/zip_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/utils/hdfs_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/utils/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/utils/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/dpdispatcher/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.192355 dpdispatcher-0.6.5/dpdispatcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12817 2024-05-27 14:48:53.000000 dpdispatcher-0.6.5/dpdispatcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-27 14:48:53.000000 dpdispatcher-0.6.5/dpdispatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:48:53.000000 dpdispatcher-0.6.5/dpdispatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-27 14:48:53.000000 dpdispatcher-0.6.5/dpdispatcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-27 14:48:53.000000 dpdispatcher-0.6.5/dpdispatcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 14:48:53.000000 dpdispatcher-0.6.5/dpdispatcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.168355 dpdispatcher-0.6.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/examples/dpdisp_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.168355 dpdispatcher-0.6.5/examples/machine/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/examples/machine/expanse.json
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/examples/machine/lazy_local.json
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/examples/machine/mandu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.172355 dpdispatcher-0.6.5/examples/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/examples/resources/expanse_cpu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/examples/resources/mandu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/examples/resources/template.slurm
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/examples/resources/tiger.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.172355 dpdispatcher-0.6.5/examples/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/examples/task/deepmd-kit.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/examples/task/g16.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.172355 dpdispatcher-0.6.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/scripts/script_gen_dargs_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/scripts/script_gen_dargs_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:48:53.196355 dpdispatcher-0.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.176355 dpdispatcher-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1843 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/debug_test_class_submission_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/devel_test_JH_UniScheduler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3228 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/devel_test_ali_ehpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2669 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/devel_test_dp_cloud_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1752 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/devel_test_lazy_ali_ehpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1398 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/devel_test_lsf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2357 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/devel_test_shell.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2673 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/devel_test_slurm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2629 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/devel_test_ssh_ali_ehpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/graph.pb
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.180355 dpdispatcher-0.6.5/tests/jsons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/job.json
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine.json
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_JH_UniScheduler.json
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_ali_ehpc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_center.json
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_diffenert.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_dp_cloud_server.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      707 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_fugaku.json
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_if_cuda_multi_devices.json
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_lazy_local_jh_unischeduler.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_lazy_local_lsf.json
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_lazy_local_slurm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_lazylocal_shell.json
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_local_fugaku.json
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_local_shell.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_lsf.json
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_openapi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_slurm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/machine_yarn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/resources.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/submission.json
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/jsons/task.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/sample_class.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1074 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/script_gen_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/slurm_test.env
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_JH_UniScheduler_script_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_argcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_class_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_class_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_class_machine_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_class_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_class_submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_class_submission_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_class_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.148355 dpdispatcher-0.6.5/tests/test_context_dir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.180355 dpdispatcher-0.6.5/tests/test_context_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.180355 dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.180355 dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-1/some_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-1/some_dir/some_file
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.184355 dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.184355 dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.184355 dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-4/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.184355 dpdispatcher-0.6.5/tests/test_context_dir/0_md/dir with space/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_context_dir/0_md/dir with space/file with space
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_context_dir/0_md/graph.pb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.184355 dpdispatcher-0.6.5/tests/test_context_dir/0_md/some_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_context_dir/0_md/some_dir/some_file
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_group_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_hdfs_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.148355 dpdispatcher-0.6.5/tests/test_hdfs_dir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.184355 dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.184355 dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.184355 dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.184355 dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.184355 dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/graph.pb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.148355 dpdispatcher-0.6.5/tests/test_if_cuda_multi_devices/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.184355 dpdispatcher-0.6.5/tests/test_if_cuda_multi_devices/test_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_if_cuda_multi_devices/test_dir/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_import_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.148355 dpdispatcher-0.6.5/tests/test_jh_unischeduler/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.184355 dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.184355 dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.184355 dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.184355 dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.188355 dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/graph.pb
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_lazy_local_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11278 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_local_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.148355 dpdispatcher-0.6.5/tests/test_lsf_dir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.188355 dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.188355 dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.188355 dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.188355 dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.188355 dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/graph.pb
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/submission.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6378 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_lsf_script_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.152355 dpdispatcher-0.6.5/tests/test_pbs_dir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.188355 dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.188355 dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.188355 dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.188355 dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.188355 dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/graph.pb
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_run_submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_run_submission_bohrium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_run_submission_ratio_unfinished.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1913 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_shell_cuda_multi_devices.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4895 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_shell_trival.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.152355 dpdispatcher-0.6.5/tests/test_shell_trival_dir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.188355 dpdispatcher-0.6.5/tests/test_shell_trival_dir/fail_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_shell_trival_dir/fail_dir/mock_fail_task.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.188355 dpdispatcher-0.6.5/tests/test_shell_trival_dir/parent_dir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.188355 dpdispatcher-0.6.5/tests/test_shell_trival_dir/parent_dir/dir with space/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_shell_trival_dir/parent_dir/dir with space/example.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.188355 dpdispatcher-0.6.5/tests/test_shell_trival_dir/parent_dir/dir1/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_shell_trival_dir/parent_dir/dir1/example.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.192355 dpdispatcher-0.6.5/tests/test_shell_trival_dir/parent_dir/dir2/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_shell_trival_dir/parent_dir/dir2/example.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.192355 dpdispatcher-0.6.5/tests/test_shell_trival_dir/parent_dir/dir3/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_shell_trival_dir/parent_dir/dir3/example.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.192355 dpdispatcher-0.6.5/tests/test_shell_trival_dir/parent_dir/dir4/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_shell_trival_dir/parent_dir/dir4/example.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_shell_trival_dir/parent_dir/graph.pb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.192355 dpdispatcher-0.6.5/tests/test_shell_trival_dir/recover_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_shell_trival_dir/recover_dir/mock_recover_task.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.152355 dpdispatcher-0.6.5/tests/test_slurm_dir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.192355 dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.192355 dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.192355 dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.192355 dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.192355 dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/d3c842c5b9476e48f7145b370cd330372b9293e1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/graph.pb
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/submission.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4722 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_slurm_script_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_ssh_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:53.192355 dpdispatcher-0.6.5/tests/test_work_path/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:48:48.000000 dpdispatcher-0.6.5/tests/test_work_path/.gitkeep
```

### Comparing `dpdispatcher-0.6.4/.github/workflows/ci-docker.yml` & `dpdispatcher-0.6.5/.github/workflows/ci-docker.yml`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     if: github.repository == 'deepmodeling/dpdispatcher'
     runs-on: ubuntu-latest
     steps:
     - name: Check out the repo
       uses: actions/checkout@v4
 
     - name: Log in to Docker Hub
-      uses: docker/login-action@343f7c4344506bcbf9b4de18042ae17996df046d
+      uses: docker/login-action@v3
       with:
         username: ${{ secrets.DOCKER_USERNAME }}
         password: ${{ secrets.DOCKER_PASSWORD }}
 
     - name: Set up QEMU
       uses: docker/setup-qemu-action@v3
```

### Comparing `dpdispatcher-0.6.4/.github/workflows/release.yml` & `dpdispatcher-0.6.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/.github/workflows/test-bohrium.yml` & `dpdispatcher-0.6.5/.github/workflows/test-bohrium.yml`

 * *Files 4% similar despite different names*

```diff
@@ -16,24 +16,27 @@
       with:
         ref: "${{ github.event.pull_request.merge_commit_sha }}"
     - name: Set up Python 3.12
       uses: actions/setup-python@v5
       with:
         python-version: '3.12'
         cache: 'pip'
-    - run: pip install .[bohrium] coverage
+    - run: pip install uv
+    - run: uv pip install --system .[bohrium] coverage
     - name: Test
       run: coverage run --source=./dpdispatcher -m unittest -v tests/test_run_submission_bohrium.py && coverage report
       env:
         DPDISPATCHER_TEST: bohrium
         BOHRIUM_EMAIL: ${{ secrets.BOHRIUM_EMAIL }}
         BOHRIUM_PASSWORD: ${{ secrets.BOHRIUM_PASSWORD }}
         BOHRIUM_PROJECT_ID: ${{ secrets.BOHRIUM_PROJECT_ID }}
         BOHRIUM_ACCESS_KEY: ${{ secrets.BOHRIUM_ACCESS_KEY }}
-    - uses: codecov/codecov-action@v3
+    - uses: codecov/codecov-action@v4
+      env:
+        CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
   remove_label:
     permissions:
       contents: read
       pull-requests: write
     # so one can re-trigger the workflow without manually removing the label
     runs-on: ubuntu-latest
     if: github.repository_owner == 'deepmodeling' && github.event.label.name == 'Test Bohrium'
```

### Comparing `dpdispatcher-0.6.4/.pre-commit-config.yaml` & `dpdispatcher-0.6.5/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.6.0
     hooks:
-    -   id: trailing-whitespace
+      - id: trailing-whitespace
         exclude: "^tests/"
-    -   id: end-of-file-fixer
+      - id: end-of-file-fixer
         exclude: "^tests/"
-    -   id: check-yaml
+      - id: check-yaml
         exclude: "^conda/"
-    -   id: check-json
-    -   id: check-added-large-files
-    -   id: check-merge-conflict
-    -   id: check-symlinks
-    -   id: check-toml
-# Python
--   repo: https://github.com/astral-sh/ruff-pre-commit
+      - id: check-json
+      - id: check-added-large-files
+      - id: check-merge-conflict
+      - id: check-symlinks
+      - id: check-toml
+  # Python
+  - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: v0.1.13
+    rev: v0.4.4
     hooks:
-    - id: ruff
-      args: ["--fix"]
-    - id: ruff-format
-# numpydoc
--   repo: https://github.com/Carreau/velin
+      - id: ruff
+        args: ["--fix"]
+      - id: ruff-format
+  # numpydoc
+  - repo: https://github.com/Carreau/velin
     rev: 0.0.12
     hooks:
-    - id: velin
-      args: ["--write"]
-# Python inside docs
--   repo: https://github.com/asottile/blacken-docs
+      - id: velin
+        args: ["--write"]
+  # Python inside docs
+  - repo: https://github.com/asottile/blacken-docs
     rev: 1.16.0
     hooks:
-    -   id: blacken-docs
+      - id: blacken-docs
+  # markdown, yaml
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: v4.0.0-alpha.8
+    hooks:
+      - id: prettier
+        types_or: [markdown, yaml]
+        # workflow files cannot be modified by pre-commit.ci
+        exclude: ^(\.github/workflows|conda)
```

### Comparing `dpdispatcher-0.6.4/CONTRIBUTING.md` & `dpdispatcher-0.6.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/LICENSE` & `dpdispatcher-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/PKG-INFO` & `dpdispatcher-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpdispatcher
-Version: 0.6.4
+Version: 0.6.5
 Summary: Generate HPC scheduler systems jobs input scripts, submit these scripts to HPC systems, and poke until they finish
 Author: DeepModeling
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -168,15 +168,15 @@
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
         
 Project-URL: Homepage, https://github.com/deepmodeling/dpdispatcher
 Project-URL: documentation, https://docs.deepmodeling.com/projects/dpdispatcher
 Project-URL: repository, https://github.com/deepmodeling/dpdispatcher
-Keywords: dispatcher,hpc,slurm,lsf,pbs,ssh
+Keywords: dispatcher,hpc,slurm,lsf,pbs,ssh,jh_unischeduler
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
@@ -187,14 +187,15 @@
 License-File: LICENSE
 Requires-Dist: paramiko
 Requires-Dist: dargs>=0.4.1
 Requires-Dist: requests
 Requires-Dist: tqdm>=4.9.0
 Requires-Dist: typing_extensions; python_version < "3.7"
 Requires-Dist: pyyaml
+Requires-Dist: tomli>=1.1.0; python_version < "3.11"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=1.0.0rc1; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: deepmodeling_sphinx>=0.1.1; extra == "docs"
 Requires-Dist: dargs>=0.3.1; extra == "docs"
@@ -246,8 +247,8 @@
 ## Contributing
 
 DPDispatcher is maintained by Deep Modeling's developers and welcomes other people.
 See [Contributing Guide](CONTRIBUTING.md) to become a contributor! 🤓
 
 ## References
 
-DPDispatcher is derivated from the [DP-GEN](https://github.com/deepmodeling/dpgen) package. To mention DPDispatcher in a scholarly publication, please read Section 3.3 in the [DP-GEN paper](https://doi.org/10.1016/j.cpc.2020.107206).
+DPDispatcher is derived from the [DP-GEN](https://github.com/deepmodeling/dpgen) package. To mention DPDispatcher in a scholarly publication, please read Section 3.3 in the [DP-GEN paper](https://doi.org/10.1016/j.cpc.2020.107206).
```

### Comparing `dpdispatcher-0.6.4/README.md` & `dpdispatcher-0.6.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 ## Contributing
 
 DPDispatcher is maintained by Deep Modeling's developers and welcomes other people.
 See [Contributing Guide](CONTRIBUTING.md) to become a contributor! 🤓
 
 ## References
 
-DPDispatcher is derivated from the [DP-GEN](https://github.com/deepmodeling/dpgen) package. To mention DPDispatcher in a scholarly publication, please read Section 3.3 in the [DP-GEN paper](https://doi.org/10.1016/j.cpc.2020.107206).
+DPDispatcher is derived from the [DP-GEN](https://github.com/deepmodeling/dpgen) package. To mention DPDispatcher in a scholarly publication, please read Section 3.3 in the [DP-GEN paper](https://doi.org/10.1016/j.cpc.2020.107206).
```

### Comparing `dpdispatcher-0.6.4/ci/LICENSE` & `dpdispatcher-0.6.5/ci/LICENSE`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/ci/pbs/docker-compose.yml` & `dpdispatcher-0.6.5/ci/pbs/docker-compose.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 version: "2"
 
 services:
-
   master:
     image: daskdev/dask-jobqueue:pbs
     build: .
     container_name: pbs_master
     hostname: pbs_master
     environment:
       - CI_SHARED_SPACE=/shared_space
```

### Comparing `dpdispatcher-0.6.4/ci/slurm/docker-compose.yml` & `dpdispatcher-0.6.5/ci/slurm/docker-compose.yml`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     image: daskdev/dask-jobqueue:slurm
     build: .
     command: ["slurmctld"]
     container_name: slurmctld
     hostname: slurmctld
     environment:
       CI_SHARED_SPACE: /data
-      DPDISPATCHER_TEST : slurm
+      DPDISPATCHER_TEST: slurm
     volumes:
       - etc_munge:/etc/munge
       - etc_slurm:/etc/slurm
       - slurm_jobdir:/data
       - var_log_slurm:/var/log/slurm
       - ../..:/dpdispatcher
     expose:
```

### Comparing `dpdispatcher-0.6.4/ci/slurm/start-slurm.sh` & `dpdispatcher-0.6.5/ci/slurm/start-slurm.sh`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/ci/ssh/docker-compose.yml` & `dpdispatcher-0.6.5/ci/ssh/docker-compose.yml`

 * *Files 23% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   test:
     image: python:3.10
     tty: true
     build: .
     container_name: test
     hostname: test
     environment:
-      DPDISPATCHER_TEST : ssh
+      DPDISPATCHER_TEST: ssh
     volumes:
       - ssh_config:/root/.ssh
       - ../..:/dpdispatcher
     depends_on:
       - server
 
 volumes:
```

### Comparing `dpdispatcher-0.6.4/ci/ssh_rsync.sh` & `dpdispatcher-0.6.5/ci/ssh_rsync.sh`

 * *Files 26% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 ./start-ssh.sh
 cd -
 
 # install rsync
 docker exec server /bin/bash -c "apt-get -y update && apt-get -y install rsync"
 docker exec test /bin/bash -c "apt-get -y update && apt-get -y install rsync"
 
-docker exec test /bin/bash -c "cd /dpdispatcher && pip install .[test] coverage && coverage run --source=./dpdispatcher -m unittest -v && coverage report"
-docker exec --env-file <(env | grep GITHUB) test /bin/bash -c "cd /dpdispatcher && curl -Os https://uploader.codecov.io/latest/linux/codecov && chmod +x codecov && ./codecov"
+docker exec test /bin/bash -c "cd /dpdispatcher && pip install uv && uv pip install --system .[test] coverage && coverage run --source=./dpdispatcher -m unittest -v && coverage report"
+docker exec --env-file <(env | grep -e GITHUB -e CODECOV) test /bin/bash -c "cd /dpdispatcher && curl -Os https://uploader.codecov.io/latest/linux/codecov && chmod +x codecov && ./codecov"
```

### Comparing `dpdispatcher-0.6.4/conda/meta.yaml` & `dpdispatcher-0.6.5/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/doc/.gitignore` & `dpdispatcher-0.6.5/doc/.gitignore`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/doc/Makefile` & `dpdispatcher-0.6.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/doc/batch.md` & `dpdispatcher-0.6.5/doc/batch.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,85 +1,91 @@
-# Supported batch job systems
-
-Batch job system is a system to process batch jobs.
-One needs to set {dargs:argument}`batch_type <machine/batch_type>` to one of the following values:
-
-## Bash
-
-{dargs:argument}`batch_type <resources/batch_type>`: `Shell`
-
-When {dargs:argument}`batch_type <resources/batch_type>` is set to `Shell`, dpdispatcher will generate a bash script to process jobs.
-No extra packages are required for `Shell`.
-
-Due to lack of scheduling system, `Shell` runs all jobs at the same time.
-To avoid running multiple jobs at the same time, one could set {dargs:argument}`group_size <resources/group_size>` to `0` (means infinity) to generate only one job with multiple tasks.
-
-## Slurm
-
-{dargs:argument}`batch_type <resources/batch_type>`: `Slurm`, `SlurmJobArray`
-
-[Slurm](https://slurm.schedmd.com/) is a job scheduling system used by lots of HPCs.
-One needs to make sure slurm has been setup in the remote server and the related environment is activated.
-
-When `SlurmJobArray` is used, dpdispatcher submits Slurm jobs with [job arrays](https://slurm.schedmd.com/job_array.html).
-In this way, several dpdispatcher {class}`task <dpdispatcher.submission.Task>`s map to a Slurm job and a dpdispatcher {class}`job <dpdispatcher.submission.Job>` maps to a Slurm job array.
-Millions of Slurm jobs can be submitted quickly and Slurm can execute all Slurm jobs at the same time.
-One can use {dargs:argument}`group_size <resources/group_size>` and {dargs:argument}`slurm_job_size <resources[SlurmJobArray]/kwargs/slurm_job_size>` to control how many Slurm jobs are contained in a Slurm job array.
-
-## OpenPBS or PBSPro
-
-{dargs:argument}`batch_type <resources/batch_type>`: `PBS`
-
-[OpenPBS](https://www.openpbs.org/) is an open-source job scheduling of the Linux Foundation and [PBS Profession](https://www.altair.com/pbs-professional/) is its commercial solution.
-One needs to make sure OpenPBS has been setup in the remote server and the related environment is activated.
-
-Note that do not use `PBS` for Torque.
-
-## TORQUE
-
-{dargs:argument}`batch_type <resources/batch_type>`: `Torque`
-
-The [Terascale Open-source Resource and QUEue Manager (TORQUE)](https://adaptivecomputing.com/cherry-services/torque-resource-manager/) is a distributed resource manager based on standard OpenPBS.
-However, not all OpenPBS flags are still supported in TORQUE.
-One needs to make sure TORQUE has been setup in the remote server and the related environment is activated.
-
-## LSF
-
-{dargs:argument}`batch_type <resources/batch_type>`: `LSF`
-
-[IBM Spectrum LSF Suites](https://www.ibm.com/products/hpc-workload-management) is a comprehensive workload management solution used by HPCs.
-One needs to make sure LSF has been setup in the remote server and the related environment is activated.
-
-## Bohrium
-
-{dargs:argument}`batch_type <resources/batch_type>`: `Bohrium`
-
-Bohrium is the cloud platform for scientific computing.
-Read Bohrium documentation for details.
-
-## DistributedShell
-
-{dargs:argument}`batch_type <resources/batch_type>`: `DistributedShell`
-
-`DistributedShell` is used to submit yarn jobs.
-Read [Support DPDispatcher on Yarn](dpdispatcher_on_yarn.md) for details.
-
-## Fugaku
-
-{dargs:argument}`batch_type <resources/batch_type>`: `Fugaku`
-
-[Fujitsu cloud service](https://doc.cloud.global.fujitsu.com/lib/common/jp/hpc-user-manual/) is a job scheduling system used by Fujitsu's HPCs such as Fugaku, ITO and K computer. It should be noted that although the same job scheduling system is used, there are some differences in the details, Fagaku class cannot be directly used for other HPCs.
-
-Read Fujitsu cloud service documentation for details.
-
-
-## OpenAPI
-
-{dargs:argument}`batcy_type <resources/batch_type>`: `OpenAPI`
-OpenAPI is a new way to submit jobs to Bohrium. It using [AccessKey](https://bohrium.dp.tech/personal/setting) instead of username and password. Read Bohrium documentation for details.
-
-
-## SGE
-
-{dargs:argument}`batch_type <resources/batch_type>`: `SGE`
-
-The [Sun Grid Engine (SGE) scheduler](https://gridscheduler.sourceforge.net) is a batch-queueing system distributed resource management. The commands and flags of SGE share a lot similarity with PBS except when checking job status. Use this argument if one is submitting job to SGE based batch system.
+# Supported batch job systems
+
+Batch job system is a system to process batch jobs.
+One needs to set {dargs:argument}`batch_type <machine/batch_type>` to one of the following values:
+
+## Bash
+
+{dargs:argument}`batch_type <resources/batch_type>`: `Shell`
+
+When {dargs:argument}`batch_type <resources/batch_type>` is set to `Shell`, dpdispatcher will generate a bash script to process jobs.
+No extra packages are required for `Shell`.
+
+Due to lack of scheduling system, `Shell` runs all jobs at the same time.
+To avoid running multiple jobs at the same time, one could set {dargs:argument}`group_size <resources/group_size>` to `0` (means infinity) to generate only one job with multiple tasks.
+
+## Slurm
+
+{dargs:argument}`batch_type <resources/batch_type>`: `Slurm`, `SlurmJobArray`
+
+[Slurm](https://slurm.schedmd.com/) is a job scheduling system used by lots of HPCs.
+One needs to make sure slurm has been set up in the remote server and the related environment is activated.
+
+When `SlurmJobArray` is used, dpdispatcher submits Slurm jobs with [job arrays](https://slurm.schedmd.com/job_array.html).
+In this way, several dpdispatcher {class}`task <dpdispatcher.submission.Task>`s map to a Slurm job and a dpdispatcher {class}`job <dpdispatcher.submission.Job>` maps to a Slurm job array.
+Millions of Slurm jobs can be submitted quickly and Slurm can execute all Slurm jobs at the same time.
+One can use {dargs:argument}`group_size <resources/group_size>` and {dargs:argument}`slurm_job_size <resources[SlurmJobArray]/kwargs/slurm_job_size>` to control how many Slurm jobs are contained in a Slurm job array.
+
+## OpenPBS or PBSPro
+
+{dargs:argument}`batch_type <resources/batch_type>`: `PBS`
+
+[OpenPBS](https://www.openpbs.org/) is an open-source job scheduling of the Linux Foundation and [PBS Profession](https://www.altair.com/pbs-professional/) is its commercial solution.
+One needs to make sure OpenPBS has been set up in the remote server and the related environment is activated.
+
+Note that do not use `PBS` for Torque.
+
+## TORQUE
+
+{dargs:argument}`batch_type <resources/batch_type>`: `Torque`
+
+The [Terascale Open-source Resource and QUEue Manager (TORQUE)](https://adaptivecomputing.com/cherry-services/torque-resource-manager/) is a distributed resource manager based on standard OpenPBS.
+However, not all OpenPBS flags are still supported in TORQUE.
+One needs to make sure TORQUE has been set up in the remote server and the related environment is activated.
+
+## LSF
+
+{dargs:argument}`batch_type <resources/batch_type>`: `LSF`
+
+[IBM Spectrum LSF Suites](https://www.ibm.com/products/hpc-workload-management) is a comprehensive workload management solution used by HPCs.
+One needs to make sure LSF has been set up in the remote server and the related environment is activated.
+
+## JH UniScheduler
+
+{dargs:argument}`batch_type <resources/batch_type>`: `JH_UniScheduler`
+
+[JH UniScheduler](http://www.jhinno.com/m/custom_case_05.html) was developed by JHINNO company and uses "jsub" to submit tasks.
+Its overall architecture is similar to that of IBM's LSF. However, there are still some differences between them. One needs to
+make sure JH UniScheduler has been set up in the remote server and the related environment is activated.
+
+## Bohrium
+
+{dargs:argument}`batch_type <resources/batch_type>`: `Bohrium`
+
+Bohrium is the cloud platform for scientific computing.
+Read Bohrium documentation for details.
+
+## DistributedShell
+
+{dargs:argument}`batch_type <resources/batch_type>`: `DistributedShell`
+
+`DistributedShell` is used to submit yarn jobs.
+Read [Support DPDispatcher on Yarn](dpdispatcher_on_yarn.md) for details.
+
+## Fugaku
+
+{dargs:argument}`batch_type <resources/batch_type>`: `Fugaku`
+
+[Fujitsu cloud service](https://doc.cloud.global.fujitsu.com/lib/common/jp/hpc-user-manual/) is a job scheduling system used by Fujitsu's HPCs such as Fugaku, ITO and K computer. It should be noted that although the same job scheduling system is used, there are some differences in the details, Fagaku class cannot be directly used for other HPCs.
+
+Read Fujitsu cloud service documentation for details.
+
+## OpenAPI
+
+{dargs:argument}`batcy_type <resources/batch_type>`: `OpenAPI`
+OpenAPI is a new way to submit jobs to Bohrium. It is using [AccessKey](https://bohrium.dp.tech/personal/setting) instead of username and password. Read Bohrium documentation for details.
+
+## SGE
+
+{dargs:argument}`batch_type <resources/batch_type>`: `SGE`
+
+The [Sun Grid Engine (SGE) scheduler](https://gridscheduler.sourceforge.net) is a batch-queueing system distributed resource management. The commands and flags of SGE share a lot of similarity with PBS except when checking job status. Use this argument if one is submitting job to an SGE-based batch system.
```

### Comparing `dpdispatcher-0.6.4/doc/conf.py` & `dpdispatcher-0.6.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/doc/dpdispatcher_on_yarn.md` & `dpdispatcher-0.6.5/doc/dpdispatcher_on_yarn.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 # Support DPDispatcher on Yarn
+
 ## Background
+
 Currently, DPGen(or other DP softwares) supports for HPC systems like Slurm, PBS, LSF and cloud machines. In order to run DPGen jobs on ByteDance internal platform, we need to extend it to support yarn resources. Hadoop Ecosystem is a very commonly used platform to process the big data, and in the process of developing the new interface, we found it can be implemented by only using hadoop opensource components. So for the convenience of the masses, we decided to contribute the codes to opensource community.
 
 ## Design
+
 We use DistributedShell and HDFS to implement it. The control flow shows as follows:
 ![image](https://github.com/shazj99/dpdispatcher/blob/yarn/doc/dpgen_yarn.jpg?raw=true)
+
 - Use DistributedShell to submit yarn jobs. It contains generating shell script and submitting it to yarn queues.
 - Use HDFS to save input files and output results. For performance reasons, we choose to pack forward files to a tar.gz file and upload it to HDFS directory. Accordingly, the task will download the tar file before running and upload result tar file to HDFS after it has done.
 
 ## Implement
+
 We only need to add two Class which are HDFSContext and DistributedShell:
 
 ```
 class HDFSContext(BaseContext) :
     def upload(self, job_dirs, local_up_files):
     """ upload forward files and forward command files to HDFS root dir
 
@@ -102,14 +107,15 @@
     script: string
         script command string
     """
         pass
 ```
 
 The following is an example of generated shell script. It will be executed in a yarn container:
+
 ```
 #!/bin/bash
 
 ## set envionment variables
 source /opt/intel/oneapi/setvars.sh
 
 ## download the tar file from hdfs which contains forward files
@@ -142,14 +148,15 @@
 ## upload result files to hdfs
 tar czf uuid_download.tar.gz sys-0001-0015
 hadoop fs -put -f uuid_download.tar.gz /root/uuid/sys-0001-0015
 
 ## mark the job has finished
 hadoop fs -touchz /root/uuid/uuid_tag_finished
 ```
+
 An example of machine.json is as follows, whose batch_type is `DistributedShell`，and context_type is `HDFSContext`:
 
 ```
   "fp": [
     {
       "command": "mpirun -n 32 vasp_std",
       "machine": {
```

### Comparing `dpdispatcher-0.6.4/doc/examples/expanse.md` & `dpdispatcher-0.6.5/doc/examples/expanse.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/doc/examples/shell.md` & `dpdispatcher-0.6.5/doc/examples/shell.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/doc/examples/template.md` & `dpdispatcher-0.6.5/doc/examples/template.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/doc/getting-started.md` & `dpdispatcher-0.6.5/doc/getting-started.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Getting Started
 
 DPDispatcher provides the following classes:
 
 - {class}`Task <dpdispatcher.submission.Task>` class, which represents a command to be run on batch job system, as well as the essential files need by the command.
 - {class}`Submission <dpdispatcher.submission.Submission>` class, which represents a collection of jobs defined by the HPC system.
-And there may be common files to be uploaded by them.
-DPDispatcher will create and submit these jobs when a `submission` instance execute {meth}`run_submission <dpdispatcher.submission.Submission.run_submission>` method.
-This method will poke until the jobs finish and return.
+  And there may be common files to be uploaded by them.
+  DPDispatcher will create and submit these jobs when a `submission` instance execute {meth}`run_submission <dpdispatcher.submission.Submission.run_submission>` method.
+  This method will poke until the jobs finish and return.
 - {class}`Job <dpdispatcher.submission.Job>` class, a class used by {class}`Submission <dpdispatcher.submission.Submission>` class, which represents a job on the HPC system.
-{class}`Submission <dpdispatcher.submission.Submission>` will generate `job`s' submitting scripts used by HPC systems automatically with the {class}`Task <dpdispatcher.submission.Task>` and {class}`Resources <dpdispatcher.submission.Resources>`
-- {class}`Resources <dpdispatcher.submission.Resources>` class, which represents the computing resources for each job  within a `submission`.
+  {class}`Submission <dpdispatcher.submission.Submission>` will generate `job`s' submitting scripts used by HPC systems automatically with the {class}`Task <dpdispatcher.submission.Task>` and {class}`Resources <dpdispatcher.submission.Resources>`
+- {class}`Resources <dpdispatcher.submission.Resources>` class, which represents the computing resources for each job within a `submission`.
 
 You can use DPDispatcher in a Python script to submit five tasks:
 
 ```python
 from dpdispatcher import Machine, Resources, Task, Submission
 
 machine = Machine.load_from_json("machine.json")
@@ -61,58 +61,58 @@
     backward_common_files=[],
 )
 
 submission.run_submission()
 ```
 
 where `machine.json` is
+
 ```json
 {
-    "batch_type": "Slurm",
-    "context_type": "SSHContext",
-    "local_root" : "/home/user123/workplace/22_new_project/",
-    "remote_root": "/home/user123/dpdispatcher_work_dir/",
-    "remote_profile":{
-        "hostname": "39.106.xx.xxx",
-        "username": "user123",
-        "port": 22,
-        "timeout": 10
-    }
+  "batch_type": "Slurm",
+  "context_type": "SSHContext",
+  "local_root": "/home/user123/workplace/22_new_project/",
+  "remote_root": "/home/user123/dpdispatcher_work_dir/",
+  "remote_profile": {
+    "hostname": "39.106.xx.xxx",
+    "username": "user123",
+    "port": 22,
+    "timeout": 10
+  }
 }
 ```
 
 `resources.json` is
+
 ```json
 {
-    "number_node": 1,
-    "cpu_per_node": 4,
-    "gpu_per_node": 1,
-    "queue_name": "GPUV100",
-    "group_size": 5
+  "number_node": 1,
+  "cpu_per_node": 4,
+  "gpu_per_node": 1,
+  "queue_name": "GPUV100",
+  "group_size": 5
 }
 ```
 
 and `task.json` is
+
 ```json
 {
-    "command": "lmp -i input.lammps",
-    "task_work_path": "bct-0/",
-    "forward_files": [
-        "conf.lmp",
-        "input.lammps"
-    ],
-    "backward_files": [
-        "log.lammps"
-    ],
-    "outlog": "log",
-    "errlog": "err",
+  "command": "lmp -i input.lammps",
+  "task_work_path": "bct-0/",
+  "forward_files": ["conf.lmp", "input.lammps"],
+  "backward_files": ["log.lammps"],
+  "outlog": "log",
+  "errlog": "err"
 }
 ```
+
 You may also submit mutiple GPU jobs:
 complex resources example
+
 ```python3
 resources = Resources(
     number_node=1,
     cpu_per_node=4,
     gpu_per_node=2,
     queue_name="GPU_2080Ti",
     group_size=4,
```

### Comparing `dpdispatcher-0.6.4/doc/index.rst` & `dpdispatcher-0.6.5/doc/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
    sphinx-quickstart on Sat Nov 21 18:36:24 2020.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 DPDispatcher's documentation
 ======================================
 
-DPDispatcher is a Python package used to generate HPC (High Performance Computing) scheduler systems (Slurm/PBS/LSF/dpcloudserver) jobs input scripts and submit these scripts to HPC systems and poke until they finish.
+DPDispatcher is a Python package used to generate HPC (High Performance Computing) scheduler systems (Slurm/PBS/LSF/JH_SCheduler/dpcloudserver) jobs input scripts and submit these scripts to HPC systems and poke until they finish.
 
 DPDispatcher will monitor (poke) until these jobs finish and download the results files (if these jobs is running on remote systems connected by SSH).
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
@@ -18,14 +18,15 @@
    install
    getting-started
    context
    batch
    machine
    resources
    task
+   run
    cli
    api/api
 
 .. toctree::
    :caption: Examples
    :glob:
```

### Comparing `dpdispatcher-0.6.4/doc/make.bat` & `dpdispatcher-0.6.5/doc/make.bat`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/dpdispatcher/__init__.py` & `dpdispatcher-0.6.5/dpdispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/dpdispatcher/base_context.py` & `dpdispatcher-0.6.5/dpdispatcher/base_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/dpdispatcher/contexts/dp_cloud_server_context.py` & `dpdispatcher-0.6.5/dpdispatcher/contexts/dp_cloud_server_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/dpdispatcher/contexts/hdfs_context.py` & `dpdispatcher-0.6.5/dpdispatcher/contexts/hdfs_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
         # download all hdfs files to tmp dir
         gz_dir = os.path.join(self.local_root, "tmp")
         if os.path.exists(gz_dir):
             shutil.rmtree(gz_dir, ignore_errors=True)
         os.mkdir(os.path.join(self.local_root, "tmp"))
         rfile_tgz = f"{self.remote_root}/{submission.submission_hash}_*_download.tar.gz"
-        lfile_tgz = "%s/tmp/" % (self.local_root)
+        lfile_tgz = f"{self.local_root}/tmp/"
         HDFS.copy_to_local(rfile_tgz, lfile_tgz)
 
         tgz_file_list = glob(os.path.join(self.local_root, "tmp/*_download.tar.gz"))
         for tgz in tgz_file_list:
             with tarfile.open(tgz, "r:gz") as tar:
                 tar.extractall(path=gz_dir)
 
@@ -160,15 +160,15 @@
                 if not os.path.exists(rfile):
                     if check_exists:
                         if mark_failure:
                             with open(
                                 os.path.join(
                                     self.local_root,
                                     task.task_work_path,
-                                    "tag_failure_download_%s" % jj,
+                                    f"tag_failure_download_{jj}",
                                 ),
                                 "w",
                             ) as fp:
                                 pass
                         else:
                             raise FileNotFoundError(
                                 "do not find download file " + rfile
@@ -194,17 +194,15 @@
             rfile = os.path.join(remote_job, jj)
             lfile = os.path.join(local_job, jj)
 
             if not os.path.exists(rfile):
                 if check_exists:
                     if mark_failure:
                         with open(
-                            os.path.join(
-                                self.local_root, "tag_failure_download_%s" % jj
-                            ),
+                            os.path.join(self.local_root, f"tag_failure_download_{jj}"),
                             "w",
                         ) as fp:
                             pass
                     else:
                         raise FileNotFoundError("do not find download file " + rfile)
                 else:
                     raise FileNotFoundError("do not find download file " + rfile)
```

### Comparing `dpdispatcher-0.6.4/dpdispatcher/contexts/lazy_local_context.py` & `dpdispatcher-0.6.5/dpdispatcher/contexts/lazy_local_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/dpdispatcher/contexts/local_context.py` & `dpdispatcher-0.6.5/dpdispatcher/contexts/local_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                 abs_flist_l = glob(os.path.join(local_job, kk))
                 if not abs_flist_r and not abs_flist_l:
                     if check_exists:
                         if mark_failure:
                             tag_file_path = os.path.join(
                                 self.local_root,
                                 ii.task_work_path,
-                                "tag_failure_download_%s" % kk,
+                                f"tag_failure_download_{kk}",
                             )
                             with open(tag_file_path, "w") as fp:
                                 pass
                         else:
                             pass
                     else:
                         raise FileNotFoundError(
@@ -177,15 +177,15 @@
                 if not os.path.realpath(rfile) == os.path.realpath(lfile):
                     if (not os.path.exists(rfile)) and (not os.path.exists(lfile)):
                         if check_exists:
                             if mark_failure:
                                 tag_file_path = os.path.join(
                                     self.local_root,
                                     ii.task_work_path,
-                                    "tag_failure_download_%s" % jj,
+                                    f"tag_failure_download_{jj}",
                                 )
                                 with open(tag_file_path, "w") as fp:
                                     pass
                             else:
                                 pass
                         else:
                             raise FileNotFoundError(
@@ -223,15 +223,15 @@
         for kk in submission.backward_common_files:
             abs_flist_r = glob(os.path.join(remote_job, kk))
             abs_flist_l = glob(os.path.join(local_job, kk))
             if not abs_flist_r and not abs_flist_l:
                 if check_exists:
                     if mark_failure:
                         tag_file_path = os.path.join(
-                            self.local_root, "tag_failure_download_%s" % kk
+                            self.local_root, f"tag_failure_download_{kk}"
                         )
                         with open(tag_file_path, "w") as fp:
                             pass
                     else:
                         pass
                 else:
                     raise FileNotFoundError(
@@ -248,15 +248,15 @@
             lfile = os.path.join(local_job, jj)
             if not os.path.realpath(rfile) == os.path.realpath(lfile):
                 if (not os.path.exists(rfile)) and (not os.path.exists(lfile)):
                     if check_exists:
                         if mark_failure:
                             with open(
                                 os.path.join(
-                                    self.local_root, "tag_failure_download_%s" % jj
+                                    self.local_root, f"tag_failure_download_{jj}"
                                 ),
                                 "w",
                             ) as fp:
                                 pass
                         else:
                             pass
                     else:
@@ -294,16 +294,16 @@
         )
         o, e = proc.communicate()
         stdout = SPRetObj(o)
         stderr = SPRetObj(e)
         code = proc.returncode
         if code != 0:
             raise RuntimeError(
-                "Get error code %d in locally calling %s with job: %s ",
-                (code, cmd, self.submission.submission_hash),
+                f"Get error code {code} in locally calling {cmd} with job: {self.submission.submission_hash}"
+                f"\nStandard error: {stderr}"
             )
         return None, stdout, stderr
 
     def block_call(self, cmd):
         proc = sp.Popen(
             cmd, cwd=self.remote_root, shell=True, stdout=sp.PIPE, stderr=sp.PIPE
         )
```

### Comparing `dpdispatcher-0.6.4/dpdispatcher/contexts/openapi_context.py` & `dpdispatcher-0.6.5/dpdispatcher/contexts/openapi_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/dpdispatcher/contexts/ssh_context.py` & `dpdispatcher-0.6.5/dpdispatcher/contexts/ssh_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,15 +296,15 @@
         try:
             return self.ssh.exec_command(cmd)
         except (paramiko.ssh_exception.SSHException, socket.timeout, EOFError) as e:
             # SSH session not active
             # retry for up to 3 times
             # ensure alive
             self.ensure_alive()
-            raise RetrySignal("SSH session not active in calling %s" % cmd) from e
+            raise RetrySignal(f"SSH session not active in calling {cmd}") from e
 
     @property
     def sftp(self):
         """Returns sftp. Open a new one if not existing."""
         if self._sftp is None:
             assert self.ssh is not None
             self.ensure_alive()
@@ -624,16 +624,15 @@
             sha256_file = os.path.join(
                 self.remote_root, ".tmp.sha256." + str(uuid.uuid4())
             )
             self.write_file(sha256_file, "\n".join(sha256_list))
             # check sha256
             # `:` means pass: https://stackoverflow.com/a/2421592/9567349
             _, stdout, _ = self.block_checkcall(
-                "sha256sum -c %s --quiet >.sha256sum_stdout 2>/dev/null || :"
-                % shlex.quote(sha256_file)
+                f"sha256sum -c {shlex.quote(sha256_file)} --quiet >.sha256sum_stdout 2>/dev/null || :"
             )
             self.sftp.remove(sha256_file)
             # regenerate file list
             file_list = []
 
             for ii in self.read_file(".sha256sum_stdout").split("\n"):
                 if ii:
@@ -704,15 +703,15 @@
                         if self.check_file_exists(file_name):
                             file_list.append(file_name)
                         elif mark_failure:
                             with open(
                                 os.path.join(
                                     self.local_root,
                                     ii.task_work_path,
-                                    "tag_failure_download_%s" % jj,
+                                    f"tag_failure_download_{jj}",
                                 ),
                                 "w",
                             ) as fp:
                                 pass
                         else:
                             pass
                 else:
@@ -754,17 +753,17 @@
             If not None, the stderr will be checked against the whitelist. If the stderr
             contains any of the strings in the whitelist, the command will be considered
             successful.
         """
         assert self.remote_root is not None
         self.ssh_session.ensure_alive()
         if asynchronously:
-            cmd = "nohup %s >/dev/null &" % cmd
+            cmd = f"nohup {cmd} >/dev/null &"
         stdin, stdout, stderr = self.ssh_session.exec_command(
-            ("cd %s ;" % shlex.quote(self.remote_root)) + cmd
+            (f"cd {shlex.quote(self.remote_root)} ;") + cmd
         )
         exit_status = stdout.channel.recv_exit_status()
         if exit_status != 0:
             raise RuntimeError(
                 "Get error code %d in calling %s through ssh with job: %s . message: %s"
                 % (
                     exit_status,
@@ -775,15 +774,15 @@
             )
         return stdin, stdout, stderr
 
     def block_call(self, cmd):
         assert self.remote_root is not None
         self.ssh_session.ensure_alive()
         stdin, stdout, stderr = self.ssh_session.exec_command(
-            ("cd %s ;" % shlex.quote(self.remote_root)) + cmd
+            (f"cd {shlex.quote(self.remote_root)} ;") + cmd
         )
         exit_status = stdout.channel.recv_exit_status()
         return exit_status, stdin, stdout, stderr
 
     def clean(self):
         self.ssh_session.ensure_alive()
         self._rmtree(self.remote_root)
@@ -842,20 +841,20 @@
     def _rmtree(self, remotepath, verbose=False):
         """Remove the remote path."""
         # The original implementation method removes files one by one using sftp.
         # If the latency of the remote server is high, it is very slow.
         # Thus, it's better to use system's `rm` to remove a directory, which may
         # save a lot of time.
         if verbose:
-            dlog.info("removing %s" % remotepath)
+            dlog.info(f"removing {remotepath}")
         # In some supercomputers, it's very slow to remove large numbers of files
         # (e.g. directory containing trajectory) due to bad I/O performance.
         # So an asynchronously option is provided.
         self.block_checkcall(
-            "rm -rf %s" % shlex.quote(remotepath),
+            f"rm -rf {shlex.quote(remotepath)}",
             asynchronously=self.clean_asynchronously,
         )
 
     def _put_files(
         self,
         files,
         dereference=True,
@@ -917,15 +916,15 @@
         try:
             self.ssh_session.put(from_f, to_f)
         except FileNotFoundError:
             raise FileNotFoundError(
                 f"from {from_f} to {self.ssh_session.username} @ {self.ssh_session.hostname} : {to_f} Error!"
             )
         # remote extract
-        self.block_checkcall("tar xf %s" % of)
+        self.block_checkcall(f"tar xf {of}")
         # clean up
         os.remove(from_f)
         self.sftp.remove(to_f)
 
     def _get_files(self, files, tar_compress=True):
         assert self.remote_root is not None
         # avoid compressing duplicated files
```

### Comparing `dpdispatcher-0.6.4/dpdispatcher/dlog.py` & `dpdispatcher-0.6.5/dpdispatcher/dlog.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,29 +2,33 @@
 import os
 import sys
 import warnings
 
 dlog = logging.getLogger("dpdispatcher")
 dlog.propagate = False
 dlog.setLevel(logging.INFO)
+cwd_logfile_path = os.path.join(os.getcwd(), "dpdispatcher.log")
+dlogf = logging.FileHandler(cwd_logfile_path, delay=True)
 try:
-    dlogf = logging.FileHandler(
-        os.getcwd() + os.sep + "dpdispatcher" + ".log", delay=True
-    )
+    dlog.addHandler(dlogf)
+    dlog.info(f"LOG INIT:dpdispatcher log direct to {cwd_logfile_path}")
 except PermissionError:
+    dlog.removeHandler(dlogf)
     warnings.warn(
-        "dpdispatcher.log meet permission error. redirect the log to ~/dpdispatcher.log"
+        f"dump logfile dpdispatcher.log to {cwd_logfile_path} meet permission error. redirect the log to ~/dpdispatcher.log"
     )
     dlogf = logging.FileHandler(
         os.path.join(os.path.expanduser("~"), "dpdispatcher.log"), delay=True
     )
+    dlog.addHandler(dlogf)
+    dlog.info("LOG INIT:dpdispatcher log init at ~/dpdispatcher.log")
 
 dlogf_formatter = logging.Formatter("%(asctime)s - %(levelname)s : %(message)s")
 dlogf.setFormatter(dlogf_formatter)
-dlog.addHandler(dlogf)
+# dlog.addHandler(dlogf)
 
 dlog_stdout = logging.StreamHandler(sys.stdout)
 dlog_stdout.setFormatter(dlogf_formatter)
 dlog.addHandler(dlog_stdout)
 
 __all__ = [
     "dlog",
```

### Comparing `dpdispatcher-0.6.4/dpdispatcher/dpdisp.py` & `dpdispatcher-0.6.5/dpdispatcher/dpdisp.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 import argparse
 from typing import List, Optional
 
 from dpdispatcher.entrypoints.gui import start_dpgui
+from dpdispatcher.entrypoints.run import run
 from dpdispatcher.entrypoints.submission import handle_submission
 
 
 def main_parser() -> argparse.ArgumentParser:
     """Dpdispatcher commandline options argument parser.
 
     Notes
@@ -77,14 +78,26 @@
         "--bind_all",
         action="store_true",
         help=(
             "Serve on all public interfaces. This will expose your DP-GUI instance "
             "to the network on both IPv4 and IPv6 (where available)."
         ),
     )
+    ##########################################
+    # run
+    parser_run = subparsers.add_parser(
+        "run",
+        help="Run a Python script.",
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
+    parser_run.add_argument(
+        "filename",
+        type=str,
+        help="Python script to run. PEP 723 metadata should be contained in this file.",
+    )
     return parser
 
 
 def parse_args(args: Optional[List[str]] = None):
     """Dpdispatcher commandline options argument parsing.
 
     Parameters
@@ -113,14 +126,16 @@
             reset_fail_count=args.reset_fail_count,
         )
     elif args.command == "gui":
         start_dpgui(
             port=args.port,
             bind_all=args.bind_all,
         )
+    elif args.command == "run":
+        run(filename=args.filename)
     elif args.command is None:
         pass
     else:
         raise RuntimeError(f"unknown command {args.command}")
 
 
 if __name__ == "__main__":
```

### Comparing `dpdispatcher-0.6.4/dpdispatcher/entrypoints/gui.py` & `dpdispatcher-0.6.5/dpdispatcher/entrypoints/gui.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/dpdispatcher/entrypoints/submission.py` & `dpdispatcher-0.6.5/dpdispatcher/entrypoints/submission.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/dpdispatcher/machine.py` & `dpdispatcher-0.6.5/dpdispatcher/machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,15 @@
         module_load_part = ""
         module_list = job.resources.module_list
         for ii in module_list:
             module_load_part += f"module load {ii}\n"
 
         source_list = job.resources.source_list
         for ii in source_list:
-            line = "{ source %s; } \n" % ii
+            line = f"{{ source {ii}; }} \n"
             source_files_part += line
 
         export_envs_part = ""
         envs = job.resources.envs
         for k, v in envs.items():
             if isinstance(v, list):
                 for each_value in v:
@@ -462,15 +462,15 @@
         If not implemented, pass and let the user manually kill it.
 
         Parameters
         ----------
         job : Job
             job
         """
-        dlog.warning("Job %s should be manually killed" % job.job_id)
+        dlog.warning(f"Job {job.job_id} should be manually killed")
 
     def get_exit_code(self, job):
         """Get exit code of the job.
 
         Parameters
         ----------
         job : Job
```

### Comparing `dpdispatcher-0.6.4/dpdispatcher/machines/distributed_shell.py` & `dpdispatcher-0.6.5/dpdispatcher/machines/distributed_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         module_load_part = ""
         module_list = job.resources.module_list
         for ii in module_list:
             module_load_part += f"module load {ii}\n"
 
         source_list = job.resources.source_list
         for ii in source_list:
-            line = "{ source %s; } \n" % ii
+            line = f"{{ source {ii}; }} \n"
             source_files_part += line
 
         export_envs_part = ""
         envs = job.resources.envs
         for k, v in envs.items():
             if isinstance(v, list):
                 for each_value in v:
@@ -92,15 +92,15 @@
             submission_hash=self.context.submission.submission_hash,
         )
         return script_env
 
     def gen_script_end(self, job):
         all_task_dirs = ""
         for task in job.job_task_list:
-            all_task_dirs += "%s " % task.task_work_path
+            all_task_dirs += f"{task.task_work_path} "
         job_tag_finished = job.job_hash + "_job_tag_finished"
         flag_if_job_task_fail = job.job_hash + "_flag_if_job_task_fail"
 
         append_script = job.resources.append_script
         append_script_part = "\n".join(append_script)
 
         script_end = script_end_template.format(
@@ -169,18 +169,16 @@
                 resources.kwargs.get("img_name", ""),
                 resources.kwargs.get("mem_limit", 1) * 1024,
                 resources.cpu_per_node,
                 script_file_name,
             )
         )
 
-        cmd = "{{ nohup {} 1>{} 2>{} & }} && echo $!".format(
-            submit_command,
-            output_name,
-            output_name,
+        cmd = (
+            f"{{ nohup {submit_command} 1>{output_name} 2>{output_name} & }} && echo $!"
         )
         ret, stdout, stderr = run_cmd_with_all_output(cmd)
 
         if ret != 0:
             err_str = stderr.decode("utf-8")
             raise RuntimeError(
                 "Command squeue fails to execute, error message:%s\nreturn code %d\n"
```

### Comparing `dpdispatcher-0.6.4/dpdispatcher/machines/dp_cloud_server.py` & `dpdispatcher-0.6.5/dpdispatcher/machines/dp_cloud_server.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/dpdispatcher/machines/fugaku.py` & `dpdispatcher-0.6.5/dpdispatcher/machines/fugaku.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     def gen_script(self, job):
         fugaku_script = super().gen_script(job)
         return fugaku_script
 
     def gen_script_header(self, job):
         resources = job.resources
         fugaku_script_header_dict = {}
-        fugaku_script_header_dict[
-            "fugaku_node_number_line"
-        ] = f'#PJM -L "node={resources.number_node}" '
-        fugaku_script_header_dict[
-            "fugaku_ntasks_per_node_line"
-        ] = f'#PJM --mpi "max-proc-per-node={resources.cpu_per_node}"'
-        fugaku_script_header_dict[
-            "queue_name_line"
-        ] = f'#PJM -L "rscgrp={resources.queue_name}"'
+        fugaku_script_header_dict["fugaku_node_number_line"] = (
+            f'#PJM -L "node={resources.number_node}" '
+        )
+        fugaku_script_header_dict["fugaku_ntasks_per_node_line"] = (
+            f'#PJM --mpi "max-proc-per-node={resources.cpu_per_node}"'
+        )
+        fugaku_script_header_dict["queue_name_line"] = (
+            f'#PJM -L "rscgrp={resources.queue_name}"'
+        )
         if (
             resources["strategy"].get("customized_script_header_template_file")
             is not None
         ):
             fugaku_script_header = customized_script_header_template(
                 resources["strategy"]["customized_script_header_template_file"],
                 resources,
```

### Comparing `dpdispatcher-0.6.4/dpdispatcher/machines/lsf.py` & `dpdispatcher-0.6.5/dpdispatcher/machines/lsf.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,15 @@
     def gen_script(self, job):
         lsf_script = super().gen_script(job)
         return lsf_script
 
     def gen_script_header(self, job):
         resources = job.resources
         script_header_dict = {
-            "lsf_nodes_line": "#BSUB -n {number_cores}".format(
-                number_cores=resources.number_node * resources.cpu_per_node
-            ),
+            "lsf_nodes_line": f"#BSUB -n {resources.number_node * resources.cpu_per_node}",
             "lsf_ptile_line": f"#BSUB -R 'span[ptile={resources.cpu_per_node}]'",
             "lsf_partition_line": f"#BSUB -q {resources.queue_name}",
         }
         gpu_usage_flag = resources.kwargs.get("gpu_usage", False)
         gpu_new_syntax_flag = resources.kwargs.get("gpu_new_syntax", False)
         gpu_exclusive_flag = resources.kwargs.get("gpu_exclusive", True)
         custom_gpu_line = resources.kwargs.get("custom_gpu_line", None)
@@ -119,15 +117,15 @@
             job_id = job.job_id
         except AttributeError:
             return JobStatus.terminated
         if job_id == "":
             return JobStatus.unsubmitted
         ret, stdin, stdout, stderr = self.context.block_call("bjobs " + job_id)
         err_str = stderr.read().decode("utf-8")
-        if ("Job <%s> is not found" % job_id) in err_str:
+        if (f"Job <{job_id}> is not found") in err_str:
             if self.check_finish_tag(job):
                 return JobStatus.finished
             else:
                 return JobStatus.terminated
         elif ret != 0:
             # just retry when any unknown error raised.
             raise RetrySignal(
```

### Comparing `dpdispatcher-0.6.4/dpdispatcher/machines/openapi.py` & `dpdispatcher-0.6.5/dpdispatcher/machines/openapi.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/dpdispatcher/machines/pbs.py` & `dpdispatcher-0.6.5/dpdispatcher/machines/pbs.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
     def gen_script(self, job):
         pbs_script = super().gen_script(job)
         return pbs_script
 
     def gen_script_header(self, job):
         resources = job.resources
         pbs_script_header_dict = {}
-        pbs_script_header_dict[
-            "select_node_line"
-        ] = f"#PBS -l select={resources.number_node}:ncpus={resources.cpu_per_node}"
+        pbs_script_header_dict["select_node_line"] = (
+            f"#PBS -l select={resources.number_node}:ncpus={resources.cpu_per_node}"
+        )
         if resources.gpu_per_node != 0:
-            pbs_script_header_dict[
-                "select_node_line"
-            ] += f":ngpus={resources.gpu_per_node}"
+            pbs_script_header_dict["select_node_line"] += (
+                f":ngpus={resources.gpu_per_node}"
+            )
         pbs_script_header_dict["queue_name_line"] = f"#PBS -q {resources.queue_name}"
         if (
             resources["strategy"].get("customized_script_header_template_file")
             is not None
         ):
             pbs_script_header = customized_script_header_template(
                 resources["strategy"]["customized_script_header_template_file"],
@@ -152,20 +152,20 @@
         else:
             return JobStatus.unknown
 
     def gen_script_header(self, job):
         # ref: https://support.adaptivecomputing.com/wp-content/uploads/2021/02/torque/torque.htm#topics/torque/2-jobs/requestingRes.htm
         resources = job.resources
         pbs_script_header_dict = {}
-        pbs_script_header_dict[
-            "select_node_line"
-        ] = f"#PBS -l nodes={resources.number_node}:ppn={resources.cpu_per_node}"
+        pbs_script_header_dict["select_node_line"] = (
+            f"#PBS -l nodes={resources.number_node}:ppn={resources.cpu_per_node}"
+        )
         if resources.gpu_per_node != 0:
-            pbs_script_header_dict["select_node_line"] += ":gpus={gpu_per_node}".format(
-                gpu_per_node=resources.gpu_per_node
+            pbs_script_header_dict["select_node_line"] += (
+                f":gpus={resources.gpu_per_node}"
             )
         pbs_script_header_dict["queue_name_line"] = f"#PBS -q {resources.queue_name}"
         if (
             resources["strategy"].get("customized_script_header_template_file")
             is not None
         ):
             pbs_script_header = customized_script_header_template(
@@ -208,17 +208,17 @@
             context=context,
         )
 
     def gen_script_header(self, job):
         resources = job.resources
         sge_script_header_dict = {}
         # resources.number_node is not used
-        sge_script_header_dict[
-            "select_node_line"
-        ] = f"#$ -pe mpi {resources.cpu_per_node} "
+        sge_script_header_dict["select_node_line"] = (
+            f"#$ -pe mpi {resources.cpu_per_node} "
+        )
         # resources.queue_name is not necessary
         sge_script_header = sge_script_header_template.format(**sge_script_header_dict)
         return sge_script_header
 
     def do_submit(self, job):
         script_file_name = job.script_file_name
         script_str = self.gen_script(job)
```

### Comparing `dpdispatcher-0.6.4/dpdispatcher/machines/shell.py` & `dpdispatcher-0.6.5/dpdispatcher/machines/shell.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,20 +35,15 @@
         job_id_name = job.job_hash + "_job_id"
         output_name = job.job_hash + ".out"
         self.context.write_file(fname=script_file_name, write_str=script_str)
         script_run_str = self.gen_script_command(job)
         script_run_file_name = f"{job.script_file_name}.run"
         self.context.write_file(fname=script_run_file_name, write_str=script_run_str)
         ret, stdin, stdout, stderr = self.context.block_call(
-            "cd {} && {{ nohup bash {} 1>>{} 2>>{} & }} && echo $!".format(
-                shlex.quote(self.context.remote_root),
-                script_file_name,
-                output_name,
-                output_name,
-            )
+            f"cd {shlex.quote(self.context.remote_root)} && {{ nohup bash {script_file_name} 1>>{output_name} 2>>{output_name} & }} && echo $!"
         )
         if ret != 0:
             err_str = stderr.read().decode("utf-8")
             raise RuntimeError(
                 "status command squeue fails to execute\nerror message:%s\nreturn code %d\n"
                 % (err_str, ret)
             )
```

### Comparing `dpdispatcher-0.6.4/dpdispatcher/machines/slurm.py` & `dpdispatcher-0.6.5/dpdispatcher/machines/slurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,31 +35,31 @@
     def gen_script(self, job):
         slurm_script = super().gen_script(job)
         return slurm_script
 
     def gen_script_header(self, job):
         resources = job.resources
         script_header_dict = {}
-        script_header_dict["slurm_nodes_line"] = "#SBATCH --nodes {number_node}".format(
-            number_node=resources.number_node
+        script_header_dict["slurm_nodes_line"] = (
+            f"#SBATCH --nodes {resources.number_node}"
+        )
+        script_header_dict["slurm_ntasks_per_node_line"] = (
+            f"#SBATCH --ntasks-per-node {resources.cpu_per_node}"
         )
-        script_header_dict[
-            "slurm_ntasks_per_node_line"
-        ] = f"#SBATCH --ntasks-per-node {resources.cpu_per_node}"
         custom_gpu_line = resources.kwargs.get("custom_gpu_line", None)
         if not custom_gpu_line:
-            script_header_dict[
-                "slurm_number_gpu_line"
-            ] = f"#SBATCH --gres=gpu:{resources.gpu_per_node}"
+            script_header_dict["slurm_number_gpu_line"] = (
+                f"#SBATCH --gres=gpu:{resources.gpu_per_node}"
+            )
         else:
             script_header_dict["slurm_number_gpu_line"] = custom_gpu_line
         if resources.queue_name != "":
-            script_header_dict[
-                "slurm_partition_line"
-            ] = f"#SBATCH --partition {resources.queue_name}"
+            script_header_dict["slurm_partition_line"] = (
+                f"#SBATCH --partition {resources.queue_name}"
+            )
         else:
             script_header_dict["slurm_partition_line"] = ""
         if (
             resources["strategy"].get("customized_script_header_template_file")
             is not None
         ):
             slurm_script_header = customized_script_header_template(
@@ -250,15 +250,15 @@
             for ii, task in enumerate(job.job_task_list):
                 task_tag_finished = (
                     pathlib.PurePath(task.task_work_path)
                     / (task.task_hash + "_task_tag_finished")
                 ).as_posix()
                 if not self.context.check_file_exists(task_tag_finished):
                     job_array.add(ii // slurm_job_size)
-            return super().gen_script_header(job) + "\n#SBATCH --array=%s" % (
+            return super().gen_script_header(job) + "\n#SBATCH --array={}".format(
                 ",".join(map(str, job_array))
             )
         return super().gen_script_header(job) + "\n#SBATCH --array=0-%d" % (
             math.ceil(len(job.job_task_list) / slurm_job_size) - 1
         )
 
     def gen_script_command(self, job):
```

### Comparing `dpdispatcher-0.6.4/dpdispatcher/submission.py` & `dpdispatcher-0.6.5/dpdispatcher/submission.py`

 * *Files 0% similar despite different names*

```diff
@@ -859,17 +859,15 @@
                 )
                 if last_error_message is not None:
                     err_msg += f"\nPossible remote error message: {last_error_message}"
                 raise RuntimeError(err_msg)
             self.submit_job()
             if self.job_state != JobStatus.unsubmitted:
                 dlog.info(
-                    "job:{job_hash} re-submit after terminated; new job_id is {job_id}".format(
-                        job_hash=self.job_hash, job_id=self.job_id
-                    )
+                    f"job:{self.job_hash} re-submit after terminated; new job_id is {self.job_id}"
                 )
                 time.sleep(0.2)
                 self.get_job_state()
                 dlog.info(
                     f"job:{self.job_hash} job_id:{self.job_id} after re-submitting; the state now is {repr(self.job_state)}"
                 )
                 self.handle_unexpected_job_state()
```

### Comparing `dpdispatcher-0.6.4/dpdispatcher/utils/dpcloudserver/client.py` & `dpdispatcher-0.6.5/dpdispatcher/utils/dpcloudserver/client.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/dpdispatcher/utils/dpcloudserver/config.py` & `dpdispatcher-0.6.5/dpdispatcher/utils/dpcloudserver/config.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/dpdispatcher/utils/dpcloudserver/retcode.py` & `dpdispatcher-0.6.5/dpdispatcher/utils/dpcloudserver/retcode.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/dpdispatcher/utils/dpcloudserver/zip_file.py` & `dpdispatcher-0.6.5/dpdispatcher/utils/dpcloudserver/zip_file.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/dpdispatcher/utils/hdfs_cli.py` & `dpdispatcher-0.6.5/dpdispatcher/utils/hdfs_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,18 +84,16 @@
         cmd = f"hadoop fs -copyFromLocal -f {local_path} {to_uri}"
         try:
             ret, out, err = run_cmd_with_all_output(cmd)
             if ret == 0:
                 return True, out
             else:
                 raise RuntimeError(
-                    "Cannot copy local[{}] to remote[{}] with cmd[{}]; "
-                    "ret[{}] output[{}] stderr[{}]".format(
-                        local_path, to_uri, cmd, ret, out, err
-                    )
+                    f"Cannot copy local[{local_path}] to remote[{to_uri}] with cmd[{cmd}]; "
+                    f"ret[{ret}] output[{out}] stderr[{err}]"
                 )
         except Exception as e:
             raise RuntimeError(
                 f"Cannot copy local[{local_path}] to remote[{to_uri}] with cmd[{cmd}]"
             ) from e
 
     @staticmethod
@@ -109,18 +107,16 @@
 
         try:
             ret, out, err = run_cmd_with_all_output(cmd)
             if ret == 0:
                 return True
             else:
                 raise RuntimeError(
-                    "Cannot copy remote[{}] to local[{}] with cmd[{}]; "
-                    "ret[{}] output[{}] stderr[{}]".format(
-                        from_uri, local_path, cmd, ret, out, err
-                    )
+                    f"Cannot copy remote[{from_uri}] to local[{local_path}] with cmd[{cmd}]; "
+                    f"ret[{ret}] output[{out}] stderr[{err}]"
                 )
         except Exception as e:
             raise RuntimeError(
                 f"Cannot copy remote[{from_uri}] to local[{local_path}] with cmd[{cmd}]"
             ) from e
 
     @staticmethod
```

### Comparing `dpdispatcher-0.6.4/dpdispatcher/utils/record.py` & `dpdispatcher-0.6.5/dpdispatcher/utils/record.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/dpdispatcher/utils/utils.py` & `dpdispatcher-0.6.5/dpdispatcher/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/dpdispatcher.egg-info/PKG-INFO` & `dpdispatcher-0.6.5/dpdispatcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpdispatcher
-Version: 0.6.4
+Version: 0.6.5
 Summary: Generate HPC scheduler systems jobs input scripts, submit these scripts to HPC systems, and poke until they finish
 Author: DeepModeling
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -168,15 +168,15 @@
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
         
 Project-URL: Homepage, https://github.com/deepmodeling/dpdispatcher
 Project-URL: documentation, https://docs.deepmodeling.com/projects/dpdispatcher
 Project-URL: repository, https://github.com/deepmodeling/dpdispatcher
-Keywords: dispatcher,hpc,slurm,lsf,pbs,ssh
+Keywords: dispatcher,hpc,slurm,lsf,pbs,ssh,jh_unischeduler
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
@@ -187,14 +187,15 @@
 License-File: LICENSE
 Requires-Dist: paramiko
 Requires-Dist: dargs>=0.4.1
 Requires-Dist: requests
 Requires-Dist: tqdm>=4.9.0
 Requires-Dist: typing_extensions; python_version < "3.7"
 Requires-Dist: pyyaml
+Requires-Dist: tomli>=1.1.0; python_version < "3.11"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=1.0.0rc1; extra == "docs"
 Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: deepmodeling_sphinx>=0.1.1; extra == "docs"
 Requires-Dist: dargs>=0.3.1; extra == "docs"
@@ -246,8 +247,8 @@
 ## Contributing
 
 DPDispatcher is maintained by Deep Modeling's developers and welcomes other people.
 See [Contributing Guide](CONTRIBUTING.md) to become a contributor! 🤓
 
 ## References
 
-DPDispatcher is derivated from the [DP-GEN](https://github.com/deepmodeling/dpgen) package. To mention DPDispatcher in a scholarly publication, please read Section 3.3 in the [DP-GEN paper](https://doi.org/10.1016/j.cpc.2020.107206).
+DPDispatcher is derived from the [DP-GEN](https://github.com/deepmodeling/dpgen) package. To mention DPDispatcher in a scholarly publication, please read Section 3.3 in the [DP-GEN paper](https://doi.org/10.1016/j.cpc.2020.107206).
```

### Comparing `dpdispatcher-0.6.4/dpdispatcher.egg-info/SOURCES.txt` & `dpdispatcher-0.6.5/dpdispatcher.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.git_archival.txt
+.gitattributes
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 CONTRIBUTING.md
 Dockerfile
 LICENSE
 README.md
@@ -40,29 +42,32 @@
 doc/credits.rst
 doc/dpdispatcher_on_yarn.md
 doc/getting-started.md
 doc/index.rst
 doc/install.md
 doc/machine.rst
 doc/make.bat
+doc/pep723.rst
 doc/requirements.txt
 doc/resources.rst
+doc/run.md
 doc/task.rst
 doc/examples/expanse.md
 doc/examples/g16.md
 doc/examples/shell.md
 doc/examples/template.md
 dpdispatcher/__init__.py
 dpdispatcher/__main__.py
 dpdispatcher/_version.py
 dpdispatcher/arginfo.py
 dpdispatcher/base_context.py
 dpdispatcher/dlog.py
 dpdispatcher/dpdisp.py
 dpdispatcher/machine.py
+dpdispatcher/run.py
 dpdispatcher/submission.py
 dpdispatcher.egg-info/PKG-INFO
 dpdispatcher.egg-info/SOURCES.txt
 dpdispatcher.egg-info/dependency_links.txt
 dpdispatcher.egg-info/entry_points.txt
 dpdispatcher.egg-info/requires.txt
 dpdispatcher.egg-info/top_level.txt
@@ -73,15 +78,17 @@
 dpdispatcher/contexts/local_context.py
 dpdispatcher/contexts/openapi_context.py
 dpdispatcher/contexts/ssh_context.py
 dpdispatcher/dpcloudserver/__init__.py
 dpdispatcher/dpcloudserver/client.py
 dpdispatcher/entrypoints/__init__.py
 dpdispatcher/entrypoints/gui.py
+dpdispatcher/entrypoints/run.py
 dpdispatcher/entrypoints/submission.py
+dpdispatcher/machines/JH_UniScheduler.py
 dpdispatcher/machines/__init__.py
 dpdispatcher/machines/distributed_shell.py
 dpdispatcher/machines/dp_cloud_server.py
 dpdispatcher/machines/fugaku.py
 dpdispatcher/machines/lsf.py
 dpdispatcher/machines/openapi.py
 dpdispatcher/machines/pbs.py
@@ -93,14 +100,15 @@
 dpdispatcher/utils/record.py
 dpdispatcher/utils/utils.py
 dpdispatcher/utils/dpcloudserver/__init__.py
 dpdispatcher/utils/dpcloudserver/client.py
 dpdispatcher/utils/dpcloudserver/config.py
 dpdispatcher/utils/dpcloudserver/retcode.py
 dpdispatcher/utils/dpcloudserver/zip_file.py
+examples/dpdisp_run.py
 examples/machine/expanse.json
 examples/machine/lazy_local.json
 examples/machine/mandu.json
 examples/resources/expanse_cpu.json
 examples/resources/mandu.json
 examples/resources/template.slurm
 examples/resources/tiger.json
@@ -109,25 +117,28 @@
 scripts/script_gen_dargs_docs.py
 scripts/script_gen_dargs_json.py
 tests/.gitignore
 tests/__init__.py
 tests/batch.json
 tests/context.py
 tests/debug_test_class_submission_init.py
+tests/devel_test_JH_UniScheduler.py
 tests/devel_test_ali_ehpc.py
 tests/devel_test_dp_cloud_server.py
 tests/devel_test_lazy_ali_ehpc.py
 tests/devel_test_lsf.py
 tests/devel_test_shell.py
 tests/devel_test_slurm.py
 tests/devel_test_ssh_ali_ehpc.py
 tests/graph.pb
+tests/hello_world.py
 tests/sample_class.py
 tests/script_gen_json.py
 tests/slurm_test.env
+tests/test_JH_UniScheduler_script_generation.py
 tests/test_argcheck.py
 tests/test_class_job.py
 tests/test_class_machine.py
 tests/test_class_machine_dispatch.py
 tests/test_class_resources.py
 tests/test_class_submission.py
 tests/test_class_submission_init.py
@@ -138,29 +149,32 @@
 tests/test_gui.py
 tests/test_hdfs_context.py
 tests/test_import_classes.py
 tests/test_lazy_local_context.py
 tests/test_local_context.py
 tests/test_lsf_script_generation.py
 tests/test_retry.py
+tests/test_run.py
 tests/test_run_submission.py
 tests/test_run_submission_bohrium.py
 tests/test_run_submission_ratio_unfinished.py
 tests/test_shell_cuda_multi_devices.py
 tests/test_shell_trival.py
 tests/test_slurm_script_generation.py
 tests/test_ssh_context.py
 tests/jsons/job.json
 tests/jsons/machine.json
+tests/jsons/machine_JH_UniScheduler.json
 tests/jsons/machine_ali_ehpc.json
 tests/jsons/machine_center.json
 tests/jsons/machine_diffenert.json
 tests/jsons/machine_dp_cloud_server.json
 tests/jsons/machine_fugaku.json
 tests/jsons/machine_if_cuda_multi_devices.json
+tests/jsons/machine_lazy_local_jh_unischeduler.json
 tests/jsons/machine_lazy_local_lsf.json
 tests/jsons/machine_lazy_local_slurm.json
 tests/jsons/machine_lazylocal_shell.json
 tests/jsons/machine_local_fugaku.json
 tests/jsons/machine_local_shell.json
 tests/jsons/machine_lsf.json
 tests/jsons/machine_openapi.json
@@ -187,14 +201,23 @@
 tests/test_hdfs_dir/0_md/bct-2/conf.lmp
 tests/test_hdfs_dir/0_md/bct-2/input.lammps
 tests/test_hdfs_dir/0_md/bct-3/conf.lmp
 tests/test_hdfs_dir/0_md/bct-3/input.lammps
 tests/test_hdfs_dir/0_md/bct-4/conf.lmp
 tests/test_hdfs_dir/0_md/bct-4/input.lammps
 tests/test_if_cuda_multi_devices/test_dir/test.txt
+tests/test_jh_unischeduler/0_md/graph.pb
+tests/test_jh_unischeduler/0_md/bct-1/conf.lmp
+tests/test_jh_unischeduler/0_md/bct-1/input.lammps
+tests/test_jh_unischeduler/0_md/bct-2/conf.lmp
+tests/test_jh_unischeduler/0_md/bct-2/input.lammps
+tests/test_jh_unischeduler/0_md/bct-3/conf.lmp
+tests/test_jh_unischeduler/0_md/bct-3/input.lammps
+tests/test_jh_unischeduler/0_md/bct-4/conf.lmp
+tests/test_jh_unischeduler/0_md/bct-4/input.lammps
 tests/test_lsf_dir/0_md/graph.pb
 tests/test_lsf_dir/0_md/submission.json
 tests/test_lsf_dir/0_md/bct-1/conf.lmp
 tests/test_lsf_dir/0_md/bct-1/input.lammps
 tests/test_lsf_dir/0_md/bct-2/conf.lmp
 tests/test_lsf_dir/0_md/bct-2/input.lammps
 tests/test_lsf_dir/0_md/bct-3/conf.lmp
```

### Comparing `dpdispatcher-0.6.4/examples/resources/expanse_cpu.json` & `dpdispatcher-0.6.5/examples/resources/expanse_cpu.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/pyproject.toml` & `dpdispatcher-0.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=61", "setuptools_scm[toml]>=6.2"]
+requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dpdispatcher"
 dynamic = ["version"]
 description = "Generate HPC scheduler systems jobs input scripts, submit these scripts to HPC systems, and poke until they finish"
 authors = [
@@ -24,18 +24,19 @@
 dependencies = [
     'paramiko',
     'dargs>=0.4.1',
     'requests',
     'tqdm>=4.9.0',
     'typing_extensions; python_version < "3.7"',
     'pyyaml',
+    'tomli >= 1.1.0; python_version < "3.11"',
 ]
 requires-python = ">=3.7"
 readme = "README.md"
-keywords = ["dispatcher", "hpc", "slurm", "lsf", "pbs", "ssh"]
+keywords = ["dispatcher", "hpc", "slurm", "lsf", "pbs", "ssh", "jh_unischeduler"]
 
 [project.urls]
 Homepage = "https://github.com/deepmodeling/dpdispatcher"
 documentation = "https://docs.deepmodeling.com/projects/dpdispatcher"
 repository = "https://github.com/deepmodeling/dpdispatcher"
 
 [project.scripts]
```

### Comparing `dpdispatcher-0.6.4/scripts/script_gen_dargs_docs.py` & `dpdispatcher-0.6.5/scripts/script_gen_dargs_docs.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/context.py` & `dpdispatcher-0.6.5/tests/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 from dpdispatcher.contexts.hdfs_context import HDFSContext  # noqa: F401
 from dpdispatcher.contexts.lazy_local_context import LazyLocalContext  # noqa: F401
 from dpdispatcher.contexts.local_context import LocalContext  # noqa: F401
 from dpdispatcher.contexts.ssh_context import SSHContext, SSHSession  # noqa: F401
 
 # test backward compatibility with dflow
 from dpdispatcher.dpcloudserver.client import RequestInfoException as _  # noqa: F401
+from dpdispatcher.entrypoints.run import run  # noqa: F401
 from dpdispatcher.entrypoints.submission import handle_submission  # noqa: F401
 from dpdispatcher.machine import Machine  # noqa: F401
 from dpdispatcher.machines.distributed_shell import DistributedShell  # noqa: F401
 from dpdispatcher.machines.dp_cloud_server import Lebesgue  # noqa: F401
+from dpdispatcher.machines.JH_UniScheduler import JH_UniScheduler  # noqa: F401
 from dpdispatcher.machines.lsf import LSF  # noqa: F401
 from dpdispatcher.machines.pbs import PBS  # noqa: F401
 from dpdispatcher.machines.shell import Shell  # noqa: F401
 from dpdispatcher.machines.slurm import Slurm  # noqa: F401
 from dpdispatcher.submission import Job, Resources, Submission, Task  # noqa: F401
 from dpdispatcher.utils.hdfs_cli import HDFS  # noqa: F401
 from dpdispatcher.utils.job_status import JobStatus  # noqa: F401
```

### Comparing `dpdispatcher-0.6.4/tests/debug_test_class_submission_init.py` & `dpdispatcher-0.6.5/tests/debug_test_class_submission_init.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/devel_test_ali_ehpc.py` & `dpdispatcher-0.6.5/tests/devel_test_ali_ehpc.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/devel_test_dp_cloud_server.py` & `dpdispatcher-0.6.5/tests/devel_test_dp_cloud_server.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/devel_test_lazy_ali_ehpc.py` & `dpdispatcher-0.6.5/tests/devel_test_lazy_ali_ehpc.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/devel_test_lsf.py` & `dpdispatcher-0.6.5/tests/devel_test_lsf.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/devel_test_shell.py` & `dpdispatcher-0.6.5/tests/devel_test_shell.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/devel_test_slurm.py` & `dpdispatcher-0.6.5/tests/devel_test_slurm.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/devel_test_ssh_ali_ehpc.py` & `dpdispatcher-0.6.5/tests/devel_test_ssh_ali_ehpc.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/jsons/job.json` & `dpdispatcher-0.6.5/tests/jsons/job.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/jsons/machine_center.json` & `dpdispatcher-0.6.5/tests/jsons/machine_center.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/jsons/machine_diffenert.json` & `dpdispatcher-0.6.5/tests/jsons/machine_diffenert.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/jsons/machine_dp_cloud_server.json` & `dpdispatcher-0.6.5/tests/jsons/machine_dp_cloud_server.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/jsons/machine_fugaku.json` & `dpdispatcher-0.6.5/tests/jsons/machine_fugaku.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/jsons/machine_lazy_local_lsf.json` & `dpdispatcher-0.6.5/tests/jsons/machine_lazy_local_lsf.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/jsons/machine_lazy_local_slurm.json` & `dpdispatcher-0.6.5/tests/jsons/machine_lazy_local_slurm.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/jsons/machine_lsf.json` & `dpdispatcher-0.6.5/tests/jsons/machine_lsf.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/jsons/machine_slurm.json` & `dpdispatcher-0.6.5/tests/jsons/machine_slurm.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/jsons/machine_yarn.json` & `dpdispatcher-0.6.5/tests/jsons/machine_yarn.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/jsons/submission.json` & `dpdispatcher-0.6.5/tests/jsons/submission.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/sample_class.py` & `dpdispatcher-0.6.5/tests/sample_class.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/script_gen_json.py` & `dpdispatcher-0.6.5/tests/script_gen_json.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_argcheck.py` & `dpdispatcher-0.6.5/tests/test_argcheck.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_class_job.py` & `dpdispatcher-0.6.5/tests/test_class_job.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_class_machine.py` & `dpdispatcher-0.6.5/tests/test_class_machine.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_class_machine_dispatch.py` & `dpdispatcher-0.6.5/tests/test_class_machine_dispatch.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 import unittest
 from socket import gaierror
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
 from dargs.dargs import ArgumentValueError
 
-from .context import (
+from .context import (  # noqa: F401
     LSF,
     PBS,
     BaseContext,
     DistributedShell,
+    JH_UniScheduler,
     LazyLocalContext,
     Lebesgue,
     LocalContext,
     Machine,
     Shell,
     Slurm,
-    setUpModule,  # noqa: F401
+    setUpModule,
 )
 
 
 class TestMachineDispatch(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
 
@@ -150,14 +151,23 @@
             "batch_type": "Slurm",
             "context_type": "LazyLocalContext",
             "local_root": "./",
         }
         machine = Machine.load_from_dict(machine_dict=machine_dict)
         self.assertIsInstance(machine, Slurm)
 
+    def test_jh_unischeduler(self):
+        machine_dict = {
+            "batch_type": "JH_UniScheduler",
+            "context_type": "LazyLocalContext",
+            "local_root": "./",
+        }
+        machine = Machine.load_from_dict(machine_dict=machine_dict)
+        self.assertIsInstance(machine, JH_UniScheduler)
+
     def test_shell(self):
         machine_dict = {
             "batch_type": "Shell",
             "context_type": "LazyLocalContext",
             "local_root": "./",
         }
         machine = Machine.load_from_dict(machine_dict=machine_dict)
```

### Comparing `dpdispatcher-0.6.4/tests/test_class_resources.py` & `dpdispatcher-0.6.5/tests/test_class_resources.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_class_submission.py` & `dpdispatcher-0.6.5/tests/test_class_submission.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_class_submission_init.py` & `dpdispatcher-0.6.5/tests/test_class_submission_init.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_class_task.py` & `dpdispatcher-0.6.5/tests/test_class_task.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_context_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.6.5/tests/test_context_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_examples.py` & `dpdispatcher-0.6.5/tests/test_examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module ensures input in the examples directory
 could pass the argument checking.
 """
+
 import json
 import unittest
 from pathlib import Path
 from typing import Sequence, Tuple
 
 from dargs import Argument
```

### Comparing `dpdispatcher-0.6.4/tests/test_group_size.py` & `dpdispatcher-0.6.5/tests/test_group_size.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_hdfs_context.py` & `dpdispatcher-0.6.5/tests/test_hdfs_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_hdfs_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.6.5/tests/test_hdfs_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_import_classes.py` & `dpdispatcher-0.6.5/tests/test_import_classes.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_lazy_local_context.py` & `dpdispatcher-0.6.5/tests/test_lazy_local_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_local_context.py` & `dpdispatcher-0.6.5/tests/test_local_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.6.5/tests/test_jh_unischeduler/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_lsf_dir/0_md/submission.json` & `dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/submission.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_lsf_script_generation.py` & `dpdispatcher-0.6.5/tests/test_lsf_script_generation.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_pbs_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.6.5/tests/test_lsf_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_retry.py` & `dpdispatcher-0.6.5/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_run_submission.py` & `dpdispatcher-0.6.5/tests/test_run_submission.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_run_submission_bohrium.py` & `dpdispatcher-0.6.5/tests/test_run_submission_bohrium.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_run_submission_ratio_unfinished.py` & `dpdispatcher-0.6.5/tests/test_run_submission_ratio_unfinished.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_shell_cuda_multi_devices.py` & `dpdispatcher-0.6.5/tests/test_shell_cuda_multi_devices.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_shell_trival.py` & `dpdispatcher-0.6.5/tests/test_shell_trival.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.6.5/tests/test_pbs_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/d3c842c5b9476e48f7145b370cd330372b9293e1.json` & `dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/d3c842c5b9476e48f7145b370cd330372b9293e1.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_slurm_dir/0_md/submission.json` & `dpdispatcher-0.6.5/tests/test_slurm_dir/0_md/submission.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_slurm_script_generation.py` & `dpdispatcher-0.6.5/tests/test_slurm_script_generation.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.6.4/tests/test_ssh_context.py` & `dpdispatcher-0.6.5/tests/test_ssh_context.py`

 * *Files identical despite different names*

