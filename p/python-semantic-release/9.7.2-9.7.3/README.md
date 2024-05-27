# Comparing `tmp/python_semantic_release-9.7.2.tar.gz` & `tmp/python_semantic_release-9.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_semantic_release-9.7.2.tar", last modified: Mon May 13 03:23:03 2024, max compression
+gzip compressed data, was "python_semantic_release-9.7.3.tar", last modified: Wed May 15 11:46:37 2024, max compression
```

## Comparing `python_semantic_release-9.7.2.tar` & `python_semantic_release-9.7.3.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.582741 python_semantic_release-9.7.2/
--rw-r--r--   0 root         (0) root         (0)      230 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1083 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      225 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5348 2024-05-13 03:23:03.582741 python_semantic_release-9.7.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2673 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.554741 python_semantic_release-9.7.2/docs/
--rw-r--r--   0 root         (0) root         (0)     6984 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)     9656 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/algorithm.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.554741 python_semantic_release-9.7.2/docs/automatic-releases/
--rw-r--r--   0 root         (0) root         (0)     1284 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/automatic-releases/cronjobs.rst
--rw-r--r--   0 root         (0) root         (0)     4046 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/automatic-releases/github-actions.rst
--rw-r--r--   0 root         (0) root         (0)      738 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/automatic-releases/index.rst
--rw-r--r--   0 root         (0) root         (0)     2268 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/automatic-releases/travis.rst
--rw-r--r--   0 root         (0) root         (0)    17609 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/changelog_templates.rst
--rw-r--r--   0 root         (0) root         (0)    16256 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/commands.rst
--rw-r--r--   0 root         (0) root         (0)    15380 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/commit-parsing.rst
--rw-r--r--   0 root         (0) root         (0)     2288 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)    33028 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/configuration.rst
--rw-r--r--   0 root         (0) root         (0)       33 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/contributing.rst
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/contributors.rst
--rw-r--r--   0 root         (0) root         (0)     3644 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/github-action.rst
--rw-r--r--   0 root         (0) root         (0)     6814 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     6735 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)    21218 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/migrating_from_v7.rst
--rw-r--r--   0 root         (0) root         (0)     8869 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/multibranch_releases.rst
--rw-r--r--   0 root         (0) root         (0)     2403 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/strict_mode.rst
--rw-r--r--   0 root         (0) root         (0)     1452 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/docs/troubleshooting.rst
--rw-r--r--   0 root         (0) root         (0)     9264 2024-05-13 03:22:52.000000 python_semantic_release-9.7.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.578741 python_semantic_release-9.7.2/python_semantic_release.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5348 2024-05-13 03:23:03.000000 python_semantic_release-9.7.2/python_semantic_release.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5600 2024-05-13 03:23:03.000000 python_semantic_release-9.7.2/python_semantic_release.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 03:23:03.000000 python_semantic_release-9.7.2/python_semantic_release.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2024-05-13 03:23:03.000000 python_semantic_release-9.7.2/python_semantic_release.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      634 2024-05-13 03:23:03.000000 python_semantic_release-9.7.2/python_semantic_release.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-13 03:23:03.000000 python_semantic_release-9.7.2/python_semantic_release.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.558741 python_semantic_release-9.7.2/semantic_release/
--rw-r--r--   0 root         (0) root         (0)      870 2024-05-13 03:22:52.000000 python_semantic_release-9.7.2/semantic_release/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.558741 python_semantic_release-9.7.2/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)      262 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1051 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/changelog/context.py
--rw-r--r--   0 root         (0) root         (0)     6675 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/changelog/release_history.py
--rw-r--r--   0 root         (0) root         (0)     4640 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/changelog/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.558741 python_semantic_release-9.7.2/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)      419 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.562741 python_semantic_release-9.7.2/semantic_release/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4197 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/commands/changelog.py
--rw-r--r--   0 root         (0) root         (0)     3443 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/commands/cli_context.py
--rw-r--r--   0 root         (0) root         (0)     1699 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/commands/generate_config.py
--rw-r--r--   0 root         (0) root         (0)     2900 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     1958 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    26160 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)     1439 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/common.py
--rw-r--r--   0 root         (0) root         (0)    21769 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/config.py
--rw-r--r--   0 root         (0) root         (0)       39 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/const.py
--rw-r--r--   0 root         (0) root         (0)     2110 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     3071 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/cli/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.562741 python_semantic_release-9.7.2/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)      615 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3004 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/commit_parser/_base.py
--rw-r--r--   0 root         (0) root         (0)     4579 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/commit_parser/angular.py
--rw-r--r--   0 root         (0) root         (0)     3452 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/commit_parser/emoji.py
--rw-r--r--   0 root         (0) root         (0)     5879 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/commit_parser/scipy.py
--rw-r--r--   0 root         (0) root         (0)     3353 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/commit_parser/tag.py
--rw-r--r--   0 root         (0) root         (0)     1505 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/commit_parser/token.py
--rw-r--r--   0 root         (0) root         (0)      730 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/commit_parser/util.py
--rw-r--r--   0 root         (0) root         (0)      831 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.546742 python_semantic_release-9.7.2/semantic_release/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.562741 python_semantic_release-9.7.2/semantic_release/data/templates/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/data/templates/CHANGELOG.md.j2
--rw-r--r--   0 root         (0) root         (0)      465 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/data/templates/release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)     1020 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/enums.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/errors.py
--rw-r--r--   0 root         (0) root         (0)     5581 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.566742 python_semantic_release-9.7.2/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)      494 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2607 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/_base.py
--rw-r--r--   0 root         (0) root         (0)     9216 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/bitbucket.py
--rw-r--r--   0 root         (0) root         (0)    11152 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/gitea.py
--rw-r--r--   0 root         (0) root         (0)    18287 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/github.py
--rw-r--r--   0 root         (0) root         (0)     6249 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/gitlab.py
--rw-r--r--   0 root         (0) root         (0)     6055 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/remote_hvcs_base.py
--rw-r--r--   0 root         (0) root         (0)      663 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/token_auth.py
--rw-r--r--   0 root         (0) root         (0)     2886 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/hvcs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.566742 python_semantic_release-9.7.2/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)      270 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16854 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/version/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7357 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/version/declaration.py
--rw-r--r--   0 root         (0) root         (0)     3050 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/version/translator.py
--rw-r--r--   0 root         (0) root         (0)    14175 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/semantic_release/version/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 03:23:03.582741 python_semantic_release-9.7.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.566742 python_semantic_release-9.7.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.570742 python_semantic_release-9.7.2/tests/command_line/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/command_line/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2983 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/command_line/conftest.py
--rw-r--r--   0 root         (0) root         (0)    11360 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/command_line/test_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1759 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/command_line/test_generate_config.py
--rw-r--r--   0 root         (0) root         (0)     6566 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/command_line/test_help.py
--rw-r--r--   0 root         (0) root         (0)     5255 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/command_line/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1425 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/command_line/test_publish.py
--rw-r--r--   0 root         (0) root         (0)    35485 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/command_line/test_version.py
--rw-r--r--   0 root         (0) root         (0)     2880 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     7826 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.570742 python_semantic_release-9.7.2/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      197 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1178 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/commit_parsers.py
--rw-r--r--   0 root         (0) root         (0)    12976 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/example_project.py
--rw-r--r--   0 root         (0) root         (0)    13342 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/git_repo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.570742 python_semantic_release-9.7.2/tests/fixtures/repos/
--rw-r--r--   0 root         (0) root         (0)      142 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.570742 python_semantic_release-9.7.2/tests/fixtures/repos/git_flow/
--rw-r--r--   0 root         (0) root         (0)      140 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/git_flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21042 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py
--rw-r--r--   0 root         (0) root         (0)    21711 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.570742 python_semantic_release-9.7.2/tests/fixtures/repos/github_flow/
--rw-r--r--   0 root         (0) root         (0)       71 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/github_flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15712 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/github_flow/repo_w_release_channels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.570742 python_semantic_release-9.7.2/tests/fixtures/repos/trunk_based_dev/
--rw-r--r--   0 root         (0) root         (0)      199 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/trunk_based_dev/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10463 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py
--rw-r--r--   0 root         (0) root         (0)    13604 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py
--rw-r--r--   0 root         (0) root         (0)    10698 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py
--rw-r--r--   0 root         (0) root         (0)    14083 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/fixtures/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.574741 python_semantic_release-9.7.2/tests/scenario/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)   127286 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/scenario/test_next_version.py
--rw-r--r--   0 root         (0) root         (0)    12845 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/scenario/test_release_history.py
--rw-r--r--   0 root         (0) root         (0)     5074 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/scenario/test_template_render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.574741 python_semantic_release-9.7.2/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.574741 python_semantic_release-9.7.2/tests/unit/semantic_release/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.574741 python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10042 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/test_changelog_context.py
--rw-r--r--   0 root         (0) root         (0)     6358 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/test_default_changelog.py
--rw-r--r--   0 root         (0) root         (0)     3560 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/test_release_notes.py
--rw-r--r--   0 root         (0) root         (0)     2116 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/test_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.574741 python_semantic_release-9.7.2/tests/unit/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8907 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_config.py
--rw-r--r--   0 root         (0) root         (0)     2129 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     6361 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     4344 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_util.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.578741 python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6374 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_angular.py
--rw-r--r--   0 root         (0) root         (0)     2567 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_emoji.py
--rw-r--r--   0 root         (0) root         (0)      778 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_parsed_commit.py
--rw-r--r--   0 root         (0) root         (0)     4457 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_scipy.py
--rw-r--r--   0 root         (0) root         (0)     2203 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      836 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.578741 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1761 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test__base.py
--rw-r--r--   0 root         (0) root         (0)    10290 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_bitbucket.py
--rw-r--r--   0 root         (0) root         (0)    27795 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_gitea.py
--rw-r--r--   0 root         (0) root         (0)    36478 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_github.py
--rw-r--r--   0 root         (0) root         (0)    15576 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)      966 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_token_auth.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_util.py
--rw-r--r--   0 root         (0) root         (0)     4507 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/test_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 03:23:03.578741 python_semantic_release-9.7.2/tests/unit/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9605 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/version/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     3874 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/version/test_declaration.py
--rw-r--r--   0 root         (0) root         (0)     2951 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/version/test_translator.py
--rw-r--r--   0 root         (0) root         (0)     9714 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/unit/semantic_release/version/test_version.py
--rw-r--r--   0 root         (0) root         (0)     6271 2024-05-13 03:21:37.000000 python_semantic_release-9.7.2/tests/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.044705 python_semantic_release-9.7.3/
+-rw-r--r--   0 root         (0) root         (0)      230 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      225 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5348 2024-05-15 11:46:37.044705 python_semantic_release-9.7.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2673 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.016705 python_semantic_release-9.7.3/docs/
+-rw-r--r--   0 root         (0) root         (0)     6984 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)     9656 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/algorithm.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.016705 python_semantic_release-9.7.3/docs/automatic-releases/
+-rw-r--r--   0 root         (0) root         (0)     1284 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/automatic-releases/cronjobs.rst
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/automatic-releases/github-actions.rst
+-rw-r--r--   0 root         (0) root         (0)      738 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/automatic-releases/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/automatic-releases/travis.rst
+-rw-r--r--   0 root         (0) root         (0)    17609 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/changelog_templates.rst
+-rw-r--r--   0 root         (0) root         (0)    16256 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/commands.rst
+-rw-r--r--   0 root         (0) root         (0)    15380 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/commit-parsing.rst
+-rw-r--r--   0 root         (0) root         (0)     2288 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)    33028 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/configuration.rst
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/contributors.rst
+-rw-r--r--   0 root         (0) root         (0)     3644 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/github-action.rst
+-rw-r--r--   0 root         (0) root         (0)     6814 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     6735 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)    21218 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/migrating_from_v7.rst
+-rw-r--r--   0 root         (0) root         (0)     8869 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/multibranch_releases.rst
+-rw-r--r--   0 root         (0) root         (0)     2403 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/strict_mode.rst
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/docs/troubleshooting.rst
+-rw-r--r--   0 root         (0) root         (0)     9264 2024-05-15 11:46:25.000000 python_semantic_release-9.7.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.040705 python_semantic_release-9.7.3/python_semantic_release.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5348 2024-05-15 11:46:36.000000 python_semantic_release-9.7.3/python_semantic_release.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5600 2024-05-15 11:46:37.000000 python_semantic_release-9.7.3/python_semantic_release.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 11:46:36.000000 python_semantic_release-9.7.3/python_semantic_release.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2024-05-15 11:46:36.000000 python_semantic_release-9.7.3/python_semantic_release.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      634 2024-05-15 11:46:36.000000 python_semantic_release-9.7.3/python_semantic_release.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-15 11:46:36.000000 python_semantic_release-9.7.3/python_semantic_release.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.020705 python_semantic_release-9.7.3/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)      870 2024-05-15 11:46:25.000000 python_semantic_release-9.7.3/semantic_release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.020705 python_semantic_release-9.7.3/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)      262 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1051 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/changelog/context.py
+-rw-r--r--   0 root         (0) root         (0)     6675 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/changelog/release_history.py
+-rw-r--r--   0 root         (0) root         (0)     4640 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/changelog/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.020705 python_semantic_release-9.7.3/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)      419 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.020705 python_semantic_release-9.7.3/semantic_release/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/cli/commands/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     3443 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/cli/commands/cli_context.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/cli/commands/generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/cli/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/cli/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    26160 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    21769 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/cli/const.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/cli/github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/cli/masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/cli/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.024705 python_semantic_release-9.7.3/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)      615 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3004 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/commit_parser/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/commit_parser/angular.py
+-rw-r--r--   0 root         (0) root         (0)     3452 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/commit_parser/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     5879 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/commit_parser/scipy.py
+-rw-r--r--   0 root         (0) root         (0)     3353 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/commit_parser/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/commit_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)      730 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/commit_parser/util.py
+-rw-r--r--   0 root         (0) root         (0)      831 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.008705 python_semantic_release-9.7.3/semantic_release/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.024705 python_semantic_release-9.7.3/semantic_release/data/templates/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/data/templates/CHANGELOG.md.j2
+-rw-r--r--   0 root         (0) root         (0)      465 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/data/templates/release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/enums.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5581 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.028705 python_semantic_release-9.7.3/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/hvcs/_base.py
+-rw-r--r--   0 root         (0) root         (0)     9216 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/hvcs/bitbucket.py
+-rw-r--r--   0 root         (0) root         (0)    11152 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/hvcs/gitea.py
+-rw-r--r--   0 root         (0) root         (0)    18287 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/hvcs/github.py
+-rw-r--r--   0 root         (0) root         (0)     6249 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/hvcs/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)     6055 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/hvcs/remote_hvcs_base.py
+-rw-r--r--   0 root         (0) root         (0)      663 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/hvcs/token_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/hvcs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.028705 python_semantic_release-9.7.3/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16854 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/version/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7357 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/version/declaration.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/version/translator.py
+-rw-r--r--   0 root         (0) root         (0)    14175 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/semantic_release/version/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 11:46:37.044705 python_semantic_release-9.7.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.028705 python_semantic_release-9.7.3/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.028705 python_semantic_release-9.7.3/tests/command_line/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/command_line/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2983 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/command_line/conftest.py
+-rw-r--r--   0 root         (0) root         (0)    11360 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/command_line/test_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/command_line/test_generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     6566 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/command_line/test_help.py
+-rw-r--r--   0 root         (0) root         (0)     5255 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/command_line/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/command_line/test_publish.py
+-rw-r--r--   0 root         (0) root         (0)    35485 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/command_line/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     7826 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.032705 python_semantic_release-9.7.3/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      197 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/fixtures/commit_parsers.py
+-rw-r--r--   0 root         (0) root         (0)    12976 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/fixtures/example_project.py
+-rw-r--r--   0 root         (0) root         (0)    13342 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/fixtures/git_repo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.032705 python_semantic_release-9.7.3/tests/fixtures/repos/
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/fixtures/repos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.032705 python_semantic_release-9.7.3/tests/fixtures/repos/git_flow/
+-rw-r--r--   0 root         (0) root         (0)      140 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/fixtures/repos/git_flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21042 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py
+-rw-r--r--   0 root         (0) root         (0)    21711 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.032705 python_semantic_release-9.7.3/tests/fixtures/repos/github_flow/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/fixtures/repos/github_flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15712 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/fixtures/repos/github_flow/repo_w_release_channels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.032705 python_semantic_release-9.7.3/tests/fixtures/repos/trunk_based_dev/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/fixtures/repos/trunk_based_dev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10463 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py
+-rw-r--r--   0 root         (0) root         (0)    13604 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py
+-rw-r--r--   0 root         (0) root         (0)    10698 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py
+-rw-r--r--   0 root         (0) root         (0)    14083 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/fixtures/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.036705 python_semantic_release-9.7.3/tests/scenario/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   127286 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/scenario/test_next_version.py
+-rw-r--r--   0 root         (0) root         (0)    12845 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/scenario/test_release_history.py
+-rw-r--r--   0 root         (0) root         (0)     5074 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/scenario/test_template_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.036705 python_semantic_release-9.7.3/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.036705 python_semantic_release-9.7.3/tests/unit/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.036705 python_semantic_release-9.7.3/tests/unit/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10042 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/changelog/test_changelog_context.py
+-rw-r--r--   0 root         (0) root         (0)     6358 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/changelog/test_default_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     3560 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/changelog/test_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/changelog/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.036705 python_semantic_release-9.7.3/tests/unit/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8907 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/cli/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/cli/test_github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     6361 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/cli/test_masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4344 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/cli/test_util.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/cli/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.040705 python_semantic_release-9.7.3/tests/unit/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6374 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/commit_parser/test_angular.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/commit_parser/test_emoji.py
+-rw-r--r--   0 root         (0) root         (0)      778 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/commit_parser/test_parsed_commit.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/commit_parser/test_scipy.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/commit_parser/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      836 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/commit_parser/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.040705 python_semantic_release-9.7.3/tests/unit/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/hvcs/test__base.py
+-rw-r--r--   0 root         (0) root         (0)    10290 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/hvcs/test_bitbucket.py
+-rw-r--r--   0 root         (0) root         (0)    27795 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/hvcs/test_gitea.py
+-rw-r--r--   0 root         (0) root         (0)    36478 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/hvcs/test_github.py
+-rw-r--r--   0 root         (0) root         (0)    15576 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/hvcs/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      966 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/hvcs/test_token_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/hvcs/test_util.py
+-rw-r--r--   0 root         (0) root         (0)     4507 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/test_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 11:46:37.040705 python_semantic_release-9.7.3/tests/unit/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9605 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/version/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3874 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/version/test_declaration.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/version/test_translator.py
+-rw-r--r--   0 root         (0) root         (0)     9714 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/unit/semantic_release/version/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     6271 2024-05-15 11:45:11.000000 python_semantic_release-9.7.3/tests/util.py
```

### Comparing `python_semantic_release-9.7.2/LICENSE` & `python_semantic_release-9.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/PKG-INFO` & `python_semantic_release-9.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 9.7.2
+Version: 9.7.3
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: changelog, https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md
 Project-URL: documentation, https://python-semantic-release.readthedocs.io
 Project-URL: homepage, https://python-semantic-release.readthedocs.io
 Project-URL: issues, https://github.com/python-semantic-release/python-semantic-release/issues
```

### Comparing `python_semantic_release-9.7.2/README.rst` & `python_semantic_release-9.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/Makefile` & `python_semantic_release-9.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/algorithm.rst` & `python_semantic_release-9.7.3/docs/algorithm.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/automatic-releases/cronjobs.rst` & `python_semantic_release-9.7.3/docs/automatic-releases/cronjobs.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/automatic-releases/github-actions.rst` & `python_semantic_release-9.7.3/docs/automatic-releases/github-actions.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/automatic-releases/index.rst` & `python_semantic_release-9.7.3/docs/automatic-releases/index.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/automatic-releases/travis.rst` & `python_semantic_release-9.7.3/docs/automatic-releases/travis.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/changelog_templates.rst` & `python_semantic_release-9.7.3/docs/changelog_templates.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/commands.rst` & `python_semantic_release-9.7.3/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/commit-parsing.rst` & `python_semantic_release-9.7.3/docs/commit-parsing.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/conf.py` & `python_semantic_release-9.7.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/configuration.rst` & `python_semantic_release-9.7.3/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/github-action.rst` & `python_semantic_release-9.7.3/docs/github-action.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/index.rst` & `python_semantic_release-9.7.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/make.bat` & `python_semantic_release-9.7.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/migrating_from_v7.rst` & `python_semantic_release-9.7.3/docs/migrating_from_v7.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/multibranch_releases.rst` & `python_semantic_release-9.7.3/docs/multibranch_releases.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/strict_mode.rst` & `python_semantic_release-9.7.3/docs/strict_mode.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/docs/troubleshooting.rst` & `python_semantic_release-9.7.3/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/pyproject.toml` & `python_semantic_release-9.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # and https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools ~= 69.0", "wheel ~= 0.42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-semantic-release"
-version = "9.7.2"
+version = "9.7.3"
 description = "Automatic Semantic Versioning for Python projects"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
```

### Comparing `python_semantic_release-9.7.2/python_semantic_release.egg-info/PKG-INFO` & `python_semantic_release-9.7.3/python_semantic_release.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 9.7.2
+Version: 9.7.3
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: changelog, https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md
 Project-URL: documentation, https://python-semantic-release.readthedocs.io
 Project-URL: homepage, https://python-semantic-release.readthedocs.io
 Project-URL: issues, https://github.com/python-semantic-release/python-semantic-release/issues
```

### Comparing `python_semantic_release-9.7.2/python_semantic_release.egg-info/SOURCES.txt` & `python_semantic_release-9.7.3/python_semantic_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/python_semantic_release.egg-info/requires.txt` & `python_semantic_release-9.7.3/python_semantic_release.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/__init__.py` & `python_semantic_release-9.7.3/semantic_release/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from semantic_release.version import (
     Version,
     VersionTranslator,
     next_version,
     tags_and_versions,
 )
 
-__version__ = "9.7.2"
+__version__ = "9.7.3"
 
 
 def setup_hook(argv: list[str]) -> None:
     """
     A hook to be used in setup.py to enable `python setup.py publish`.
 
     :param argv: sys.argv
```

### Comparing `python_semantic_release-9.7.2/semantic_release/changelog/context.py` & `python_semantic_release-9.7.3/semantic_release/changelog/context.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/changelog/release_history.py` & `python_semantic_release-9.7.3/semantic_release/changelog/release_history.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/changelog/template.py` & `python_semantic_release-9.7.3/semantic_release/changelog/template.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/cli/commands/changelog.py` & `python_semantic_release-9.7.3/semantic_release/cli/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/cli/commands/cli_context.py` & `python_semantic_release-9.7.3/semantic_release/cli/commands/cli_context.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/cli/commands/generate_config.py` & `python_semantic_release-9.7.3/semantic_release/cli/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/cli/commands/main.py` & `python_semantic_release-9.7.3/semantic_release/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/cli/commands/publish.py` & `python_semantic_release-9.7.3/semantic_release/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/cli/commands/version.py` & `python_semantic_release-9.7.3/semantic_release/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/cli/common.py` & `python_semantic_release-9.7.3/semantic_release/cli/common.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/cli/config.py` & `python_semantic_release-9.7.3/semantic_release/cli/config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/cli/github_actions_output.py` & `python_semantic_release-9.7.3/semantic_release/cli/github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/cli/masking_filter.py` & `python_semantic_release-9.7.3/semantic_release/cli/masking_filter.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/cli/util.py` & `python_semantic_release-9.7.3/semantic_release/cli/util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/commit_parser/__init__.py` & `python_semantic_release-9.7.3/semantic_release/commit_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/commit_parser/_base.py` & `python_semantic_release-9.7.3/semantic_release/commit_parser/_base.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/commit_parser/angular.py` & `python_semantic_release-9.7.3/semantic_release/commit_parser/angular.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/commit_parser/emoji.py` & `python_semantic_release-9.7.3/semantic_release/commit_parser/emoji.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/commit_parser/scipy.py` & `python_semantic_release-9.7.3/semantic_release/commit_parser/scipy.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/commit_parser/tag.py` & `python_semantic_release-9.7.3/semantic_release/commit_parser/tag.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/commit_parser/token.py` & `python_semantic_release-9.7.3/semantic_release/commit_parser/token.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/commit_parser/util.py` & `python_semantic_release-9.7.3/semantic_release/commit_parser/util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/const.py` & `python_semantic_release-9.7.3/semantic_release/const.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/data/templates/CHANGELOG.md.j2` & `python_semantic_release-9.7.3/semantic_release/data/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/enums.py` & `python_semantic_release-9.7.3/semantic_release/enums.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/errors.py` & `python_semantic_release-9.7.3/semantic_release/errors.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/helpers.py` & `python_semantic_release-9.7.3/semantic_release/helpers.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/hvcs/_base.py` & `python_semantic_release-9.7.3/semantic_release/hvcs/_base.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/hvcs/bitbucket.py` & `python_semantic_release-9.7.3/semantic_release/hvcs/bitbucket.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/hvcs/gitea.py` & `python_semantic_release-9.7.3/semantic_release/hvcs/gitea.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/hvcs/github.py` & `python_semantic_release-9.7.3/semantic_release/hvcs/github.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/hvcs/gitlab.py` & `python_semantic_release-9.7.3/semantic_release/hvcs/gitlab.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/hvcs/remote_hvcs_base.py` & `python_semantic_release-9.7.3/semantic_release/hvcs/remote_hvcs_base.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/hvcs/token_auth.py` & `python_semantic_release-9.7.3/semantic_release/hvcs/token_auth.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/hvcs/util.py` & `python_semantic_release-9.7.3/semantic_release/hvcs/util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/version/algorithm.py` & `python_semantic_release-9.7.3/semantic_release/version/algorithm.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/version/declaration.py` & `python_semantic_release-9.7.3/semantic_release/version/declaration.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/version/translator.py` & `python_semantic_release-9.7.3/semantic_release/version/translator.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/semantic_release/version/version.py` & `python_semantic_release-9.7.3/semantic_release/version/version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/command_line/conftest.py` & `python_semantic_release-9.7.3/tests/command_line/conftest.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/command_line/test_changelog.py` & `python_semantic_release-9.7.3/tests/command_line/test_changelog.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/command_line/test_generate_config.py` & `python_semantic_release-9.7.3/tests/command_line/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/command_line/test_help.py` & `python_semantic_release-9.7.3/tests/command_line/test_help.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/command_line/test_main.py` & `python_semantic_release-9.7.3/tests/command_line/test_main.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/command_line/test_publish.py` & `python_semantic_release-9.7.3/tests/command_line/test_publish.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/command_line/test_version.py` & `python_semantic_release-9.7.3/tests/command_line/test_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/conftest.py` & `python_semantic_release-9.7.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/const.py` & `python_semantic_release-9.7.3/tests/const.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/fixtures/commit_parsers.py` & `python_semantic_release-9.7.3/tests/fixtures/commit_parsers.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/fixtures/example_project.py` & `python_semantic_release-9.7.3/tests/fixtures/example_project.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/fixtures/git_repo.py` & `python_semantic_release-9.7.3/tests/fixtures/git_repo.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py` & `python_semantic_release-9.7.3/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py` & `python_semantic_release-9.7.3/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/fixtures/repos/github_flow/repo_w_release_channels.py` & `python_semantic_release-9.7.3/tests/fixtures/repos/github_flow/repo_w_release_channels.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py` & `python_semantic_release-9.7.3/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py` & `python_semantic_release-9.7.3/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py` & `python_semantic_release-9.7.3/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/fixtures/scipy.py` & `python_semantic_release-9.7.3/tests/fixtures/scipy.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/scenario/test_next_version.py` & `python_semantic_release-9.7.3/tests/scenario/test_next_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/scenario/test_release_history.py` & `python_semantic_release-9.7.3/tests/scenario/test_release_history.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/scenario/test_template_render.py` & `python_semantic_release-9.7.3/tests/scenario/test_template_render.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/test_changelog_context.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/changelog/test_changelog_context.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/test_default_changelog.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/changelog/test_default_changelog.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/test_release_notes.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/changelog/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/changelog/test_template.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/changelog/test_template.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_config.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_github_actions_output.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/cli/test_github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_masking_filter.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/cli/test_masking_filter.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_util.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/cli/test_util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/cli/test_version.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/cli/test_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_angular.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/commit_parser/test_angular.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_emoji.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/commit_parser/test_emoji.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_parsed_commit.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/commit_parser/test_parsed_commit.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_scipy.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/commit_parser/test_scipy.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_tag.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/commit_parser/test_tag.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/commit_parser/test_util.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/commit_parser/test_util.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test__base.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/hvcs/test__base.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_bitbucket.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/hvcs/test_bitbucket.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_gitea.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/hvcs/test_gitea.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_github.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/hvcs/test_github.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_gitlab.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/hvcs/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/hvcs/test_token_auth.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/hvcs/test_token_auth.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/test_helpers.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/version/test_algorithm.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/version/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/version/test_declaration.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/version/test_declaration.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/version/test_translator.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/version/test_translator.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/unit/semantic_release/version/test_version.py` & `python_semantic_release-9.7.3/tests/unit/semantic_release/version/test_version.py`

 * *Files identical despite different names*

### Comparing `python_semantic_release-9.7.2/tests/util.py` & `python_semantic_release-9.7.3/tests/util.py`

 * *Files identical despite different names*

