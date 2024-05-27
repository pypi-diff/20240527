# Comparing `tmp/bootwrap-1.0.0.tar.gz` & `tmp/bootwrap-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootwrap-1.0.0.tar", last modified: Fri Jul 16 11:02:07 2021, max compression
+gzip compressed data, was "bootwrap-1.0.1.tar", last modified: Mon May 27 19:59:16 2024, max compression
```

## Comparing `bootwrap-1.0.0.tar` & `bootwrap-1.0.1.tar`

### file list

```diff
@@ -1,98 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 11:02:07.757753 bootwrap-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 11:02:07.749752 bootwrap-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 11:02:07.753753 bootwrap-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2021-07-16 11:02:00.000000 bootwrap-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      608 2021-07-16 11:02:00.000000 bootwrap-1.0.0/.github/workflows/pre-release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      534 2021-07-16 11:02:00.000000 bootwrap-1.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      452 2021-07-16 11:02:00.000000 bootwrap-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     6546 2021-07-16 11:02:00.000000 bootwrap-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-07-16 11:02:00.000000 bootwrap-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4653 2021-07-16 11:02:07.757753 bootwrap-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4037 2021-07-16 11:02:00.000000 bootwrap-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 11:02:07.749752 bootwrap-1.0.0/bootwrap/
--rw-r--r--   0 runner    (1001) docker     (121)      286 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 11:02:07.753753 bootwrap-1.0.0/bootwrap/components/
--rw-r--r--   0 runner    (1001) docker     (121)      852 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4399 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/anchor.py
--rw-r--r--   0 runner    (1001) docker     (121)      864 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/badge.py
--rw-r--r--   0 runner    (1001) docker     (121)    17837 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5810 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/button.py
--rw-r--r--   0 runner    (1001) docker     (121)     8417 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/deck.py
--rw-r--r--   0 runner    (1001) docker     (121)     2264 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/dialog.py
--rw-r--r--   0 runner    (1001) docker     (121)    16954 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/form.py
--rw-r--r--   0 runner    (1001) docker     (121)     3313 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/icon.py
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/javascript.py
--rw-r--r--   0 runner    (1001) docker     (121)     1279 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/link.py
--rw-r--r--   0 runner    (1001) docker     (121)     9679 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5174 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/navigation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4263 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/panel.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/separator.py
--rw-r--r--   0 runner    (1001) docker     (121)    15898 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/table.py
--rw-r--r--   0 runner    (1001) docker     (121)     5382 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/text.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/components/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2490 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/menu.py
--rw-r--r--   0 runner    (1001) docker     (121)     3766 2021-07-16 11:02:00.000000 bootwrap-1.0.0/bootwrap/page.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 11:02:07.753753 bootwrap-1.0.0/bootwrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4653 2021-07-16 11:02:07.000000 bootwrap-1.0.0/bootwrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2646 2021-07-16 11:02:07.000000 bootwrap-1.0.0/bootwrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-16 11:02:07.000000 bootwrap-1.0.0/bootwrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-07-16 11:02:07.000000 bootwrap-1.0.0/bootwrap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 11:02:07.753753 bootwrap-1.0.0/demo/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-07-16 11:02:00.000000 bootwrap-1.0.0/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2021-07-16 11:02:00.000000 bootwrap-1.0.0/demo/demo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 11:02:07.757753 bootwrap-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8132 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/amazon-logo.png
--rw-r--r--   0 runner    (1001) docker     (121)   111496 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/base.html
--rw-r--r--   0 runner    (1001) docker     (121)    25995 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/bootwrap-equation.png
--rw-r--r--   0 runner    (1001) docker     (121)   294493 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/components.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 11:02:07.757753 bootwrap-1.0.0/docs/config/
--rw-r--r--   0 runner    (1001) docker     (121)      516 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/config/base.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16663 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/config/components.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3350 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/config/home.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2382 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/config/layout.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    17159 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/doc_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     6840 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/doc_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)    15406 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)    52572 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/flash.png
--rw-r--r--   0 runner    (1001) docker     (121)    16363 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/google-logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     9864 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     7424 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/layout.html
--rw-r--r--   0 runner    (1001) docker     (121)     4541 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/layout.png
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/linkedin-logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     6517 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     7278 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/menu.png
--rw-r--r--   0 runner    (1001) docker     (121)    32506 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/multi-pages-app.png
--rw-r--r--   0 runner    (1001) docker     (121)     8411 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/page.png
--rw-r--r--   0 runner    (1001) docker     (121)    17798 2021-07-16 11:02:00.000000 bootwrap-1.0.0/docs/single-page-app.png
--rwxr-xr-x   0 runner    (1001) docker     (121)     3318 2021-07-16 11:02:00.000000 bootwrap-1.0.0/helper.sh
--rw-r--r--   0 runner    (1001) docker     (121)      555 2021-07-16 11:02:00.000000 bootwrap-1.0.0/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2021-07-16 11:02:00.000000 bootwrap-1.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-07-16 11:02:00.000000 bootwrap-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-16 11:02:07.757753 bootwrap-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-07-16 11:02:00.000000 bootwrap-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 11:02:07.757753 bootwrap-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5966 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3765 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_anchor.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_badge.py
--rw-r--r--   0 runner    (1001) docker     (121)     4163 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7235 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (121)     5688 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_deck.py
--rw-r--r--   0 runner    (1001) docker     (121)     3012 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_dialog.py
--rw-r--r--   0 runner    (1001) docker     (121)    15703 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1327 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_icon.py
--rw-r--r--   0 runner    (1001) docker     (121)      515 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_javascript.py
--rw-r--r--   0 runner    (1001) docker     (121)      624 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_link.py
--rw-r--r--   0 runner    (1001) docker     (121)     6895 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2198 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (121)     3093 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_navigation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3881 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (121)     2744 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_panel.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_separator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5572 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     2539 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2021-07-16 11:02:00.000000 bootwrap-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.653569 bootwrap-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.621569 bootwrap-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.629569 bootwrap-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-27 19:59:11.000000 bootwrap-1.0.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-27 19:59:11.000000 bootwrap-1.0.1/.github/workflows/pre-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-27 19:59:11.000000 bootwrap-1.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-27 19:59:11.000000 bootwrap-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-27 19:59:11.000000 bootwrap-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-27 19:59:11.000000 bootwrap-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-27 19:59:16.653569 bootwrap-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-05-27 19:59:11.000000 bootwrap-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.629569 bootwrap-1.0.1/bootwrap/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.637569 bootwrap-1.0.1/bootwrap/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17817 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/deck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14694 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/separator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/components/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/generic.css
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/generic.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-27 19:59:11.000000 bootwrap-1.0.1/bootwrap/page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.653569 bootwrap-1.0.1/bootwrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-27 19:59:16.000000 bootwrap-1.0.1/bootwrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-27 19:59:16.000000 bootwrap-1.0.1/bootwrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:59:16.000000 bootwrap-1.0.1/bootwrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 19:59:16.000000 bootwrap-1.0.1/bootwrap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.641569 bootwrap-1.0.1/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48411 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/aapl-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59453 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/account-screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)   115095 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/activity-screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/amzn-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   284519 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/background.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    39185 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/bank.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/cash.png
+-rw-r--r--   0 runner    (1001) docker     (127)   458319 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/collage.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/demo.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/demo_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/demo_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/demo_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/demo_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)   117258 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/discovery-screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    16363 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/googl-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36084 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/hard-work.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/lnkd-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38559 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/login-screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45146 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/nvda-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31403 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/party.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    75442 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/piggybank-title.png
+-rw-r--r--   0 runner    (1001) docker     (127)   108158 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/portfolio-screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/stock.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-27 19:59:11.000000 bootwrap-1.0.1/demo/tsla-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.645569 bootwrap-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/amazon-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   112499 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28291 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/bootwrap-equation.png
+-rw-r--r--   0 runner    (1001) docker     (127)   297611 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/components.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.649569 bootwrap-1.0.1/docs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/config/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/config/components.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/config/home.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/config/layout.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17454 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/doc_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/doc_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    52572 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/flash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16363 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/google-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10647 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/layout.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/linkedin-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/menu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32506 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/multi-pages-app.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/page.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17798 2024-05-27 19:59:11.000000 bootwrap-1.0.1/docs/single-page-app.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2886 2024-05-27 19:59:11.000000 bootwrap-1.0.1/helper.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-27 19:59:11.000000 bootwrap-1.0.1/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-27 19:59:11.000000 bootwrap-1.0.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-27 19:59:11.000000 bootwrap-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:59:16.653569 bootwrap-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 19:59:11.000000 bootwrap-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:59:16.653569 bootwrap-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_anchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_deck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15690 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_separator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-27 19:59:11.000000 bootwrap-1.0.1/tests/test_utils.py
```

### Comparing `bootwrap-1.0.0/.github/workflows/ci.yml` & `bootwrap-1.0.1/.github/workflows/ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -41,11 +41,13 @@
     - name: Generate coverage report
       run: |
         pip install pytest
         pip install pytest-cov
         pytest --cov=bootwrap --cov-report=xml
 
     - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v1
+      uses: codecov/codecov-action@v4
       with:
         fail_ci_if_error: true
         verbose: true
+      env:
+        CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `bootwrap-1.0.0/.github/workflows/pre-release.yml` & `bootwrap-1.0.1/.github/workflows/pre-release.yml`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/.github/workflows/release.yml` & `bootwrap-1.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/CONTRIBUTING.md` & `bootwrap-1.0.1/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -81,27 +81,26 @@
 ~$ ./helper.sh
 
     ____              __ _       __                
    / __ )____  ____  / /| |     / /________ _____  
   / __  / __ \/ __ \/ __/ | /| / / ___/ __ '/ __ \ 
  / /_/ / /_/ / /_/ / /_ | |/ |/ / /  / /_/ / /_/ / 
 /_____/\____/\____/\__/ |__/|__/_/   \__,_/ .___/  
-                                         /_/       
+Python + Bootstrap                       /_/       
 
 System Commands:
    init initializers environment;
    test ... runs tests;
       -m <MARK> runs tests for mark;
       -c generates code coverage summary;
       -r generates code coverage report;
    preview runs web-server with documentation preview;
    docs generates documentation (HTML-pages);
    demo runs web-server with showcase project;
    build generates distribution archives;
-   stage deploys Bootwrap to Test Python Package Index;
 ```
 
 ### Init
 
 `init` command performs initialization of Bootwrap project from scratch. Usually, it should be called just once  (straight after cloning repository).  First, it creates a virtual environment and installs necessary dependencies defined in the `requirements.txt` file. If you introduce a new dependency (to `requirements.txt` file) run the `init` command again.
 
 ### Test
@@ -166,27 +165,7 @@
 ### Build
 
 Run the `build` command to package the Bootwrap project for PIP installation. This command should be most used by the repository administrator. However, it would be also useful for testing the Bootwrap package installation on the local machine.  
 
 ```bash
 ~$ ./helper.sh build
 ```
-
-### Stage
-
-Use the `stage` command to deploy prebuilt Bootwrap packages to the [Test Python Package Index](https://test.pypi.org/).
-
-```bash
-~$ ./helper.sh stage
-```
-
-**This command must be used by the repository administrator.**
-
-### Deploy
-
-Use the `deploy` command to deploy prebuilt Bootwrap packages to the [Python Package Index](https://pypi.org/).
-
-```bash
-~$ ./helper.sh deploy
-```
-
-**This command must be used by the repository administrator.**
```

### Comparing `bootwrap-1.0.0/LICENSE` & `bootwrap-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/PKG-INFO` & `bootwrap-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: bootwrap
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package for rapid development of web-based user interfaces.
 Home-page: https://github.com/mmgalushka/bootwrap
 Author: Mykola Galushka
 Author-email: mm.galushka@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/mmgalushka/bootwrap/issues
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,71 +22,81 @@
 [![Code Coverage Percentage](https://codecov.io/gh/mmgalushka/bootwrap/branch/main/graphs/badge.svg)](https://codecov.io/gh/mmgalushka/bootwrap)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/763657a471ff424c85a5b894ddb750d0)](https://www.codacy.com/gh/mmgalushka/bootwrap/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mmgalushka/bootwrap&amp;utm_campaign=Badge_Grade)
 [![Project License](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/mmgalushka/bootwrap/blob/main/LICENSE)
 [![Project Documentation](https://img.shields.io/badge/docs-up--to--date-success)](https://mmgalushka.github.io/bootwrap/)
 
 **Bootwrap** is a Python library for rapid developing of web-based user interfaces (WebUI). It helps creating WebUI using Python code only and can be used in conjunction with different web-development frameworks such as [Flask](https://palletsprojects.com/p/flask/). Under the hood, this library wraps one of the most popular front-end toolkit [Bootstrap](https://getbootstrap.com/).
 
-This library would be useful for developers and data scientists who wish to build interactive web-application without crafting HTML, CSS and Javascript.
-
 As a showcase of what this library is capable of please check the documentation. The entire [documentation](https://mmgalushka.github.io/bootwrap/) web interface is created using the **Bootwrap**.
 
 ## Installing
 
 Install and update using [pip](https://pip.pypa.io/en/stable/quickstart/):
 
 ```bash
 ~$ pip install bootwrap
 ```
 
-## A Simple Example
+Bootwrap package has no external dependencies!
+
+## Why & where you might use Bootwrap?
+
+The vast majority of web applications consist of frontend and backend. If you are a small team or even a solo developer you need to divide resources and time to focus on both parts. This often results in switching between different platforms such as Python and [React](https://reactjs.org/), [AngularJs](https://angular.io/), Flask templates (HTML, CSS, JS), etc. But what if your main focus is the backend and you also don't want to compromise on the quality of your WebUI. In this case, the Bootwrap library is for you! It will help you develop WebUI without leaving the Python ecosystem and not waste your time on HTML, CSS, and Javascript. To understand its capability just clone the project and run the [demo application](demo/demo.md) ":pig: PiggyBank".
+
+![Screenshots Collage](demo/collage.png)
+
+For more information also read the Bootwrap [documentation](https://mmgalushka.github.io/bootwrap/).
 
-The following code will care three pages application with the top-level menu bar for navigations.  
+## Hello World Application
+
+The following code will create three pages application with a top-level menu bar for navigations. Since this application is based on [Flask](https://palletsprojects.com/p/flask/) make sure that you installed it as well.
 
 ```Python
 from flask import Flask, Markup
 from bootwrap import Page, Menu, Image, Anchor, Button, Text
 
-# Both 'logo.png' and 'favicon.ico' are stored in 'docs' folder
 app = Flask(__name__, static_folder='docs', static_url_path='')
 
+LOGO = 'https://github.com/mmgalushka/bootwrap/blob/main/docs/logo.png?raw=true'
+FAVICON = 'https://raw.githubusercontent.com/mmgalushka/bootwrap/main/docs/favicon.ico'
+
 class MyMenu(Menu):
     def __init__(self):
         super().__init__(
-            logo=Image('logo.png', width=32, alt='Logo'),
+            logo=Image(LOGO, width=32, alt='Logo'),
             brand=Text('Bootwrap').as_strong().as_light().ml(2),
             anchors=[
                 Anchor('Home').link('/'),
                 Anchor('About').link('/about')
             ], 
             actions=[
                 Button('Sign In').as_outline().as_light().link('/signin')
             ]
         )
 
 class MyPage(Page):
     def __init__(self, container):
         super().__init__(
-            favicon = 'favicon.ico',
+            favicon = FAVICON,
             title='Hello World Application',
             menu=MyMenu(),
             container=container
         )
 
 @app.route('/')
 def home():
-    return Markup(MyPage(container=[Text('Home').as_heading(1)]))
+    return Markup(MyPage(container=Text('Home').as_heading(1)))
 
 @app.route('/about')
 def about():
-    return Markup(MyPage(container=[Text('About').as_heading(1)]))
+    return Markup(MyPage(container=Text('About').as_heading(1)))
 
 @app.route('/signin')
 def signin():
-    return Markup(MyPage(container=[Text('Sign In').as_heading(1)]))
+    return Markup(MyPage(container=Text('Sign In').as_heading(1)))
 
 if __name__ == '__main__':
     app.run(debug=True)
 ```
 
 Use the following command to launch the application.
 
@@ -104,12 +112,10 @@
 ## Contributing
 
 For information on how to set up a development environment and how to make a contribution to Bootwrap, see the [contributing guidelines](CONTRIBUTING.md).
 
 ## Links
 
 - Documentation: [https://mmgalushka.github.io/bootwrap/](https://mmgalushka.github.io/bootwrap/)
-- PyPI Releases: [https://test.pypi.org/project/bootwrap/](https://test.pypi.org/project/bootwrap/)
+- PyPI Releases: [https://pypi.org/project/bootwrap/](https://pypi.org/project/bootwrap/)
 - Source Code: [https://github.com/mmgalushka/bootwrap](https://github.com/mmgalushka/bootwrap/)
 - Issue Tracker: [https://github.com/mmgalushka/bootwrap/issues](https://github.com/mmgalushka/bootwrap/)
-
-
```

### Comparing `bootwrap-1.0.0/README.md` & `bootwrap-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -6,71 +6,81 @@
 [![Code Coverage Percentage](https://codecov.io/gh/mmgalushka/bootwrap/branch/main/graphs/badge.svg)](https://codecov.io/gh/mmgalushka/bootwrap)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/763657a471ff424c85a5b894ddb750d0)](https://www.codacy.com/gh/mmgalushka/bootwrap/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mmgalushka/bootwrap&amp;utm_campaign=Badge_Grade)
 [![Project License](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/mmgalushka/bootwrap/blob/main/LICENSE)
 [![Project Documentation](https://img.shields.io/badge/docs-up--to--date-success)](https://mmgalushka.github.io/bootwrap/)
 
 **Bootwrap** is a Python library for rapid developing of web-based user interfaces (WebUI). It helps creating WebUI using Python code only and can be used in conjunction with different web-development frameworks such as [Flask](https://palletsprojects.com/p/flask/). Under the hood, this library wraps one of the most popular front-end toolkit [Bootstrap](https://getbootstrap.com/).
 
-This library would be useful for developers and data scientists who wish to build interactive web-application without crafting HTML, CSS and Javascript.
-
 As a showcase of what this library is capable of please check the documentation. The entire [documentation](https://mmgalushka.github.io/bootwrap/) web interface is created using the **Bootwrap**.
 
 ## Installing
 
 Install and update using [pip](https://pip.pypa.io/en/stable/quickstart/):
 
 ```bash
 ~$ pip install bootwrap
 ```
 
-## A Simple Example
+Bootwrap package has no external dependencies!
+
+## Why & where you might use Bootwrap?
+
+The vast majority of web applications consist of frontend and backend. If you are a small team or even a solo developer you need to divide resources and time to focus on both parts. This often results in switching between different platforms such as Python and [React](https://reactjs.org/), [AngularJs](https://angular.io/), Flask templates (HTML, CSS, JS), etc. But what if your main focus is the backend and you also don't want to compromise on the quality of your WebUI. In this case, the Bootwrap library is for you! It will help you develop WebUI without leaving the Python ecosystem and not waste your time on HTML, CSS, and Javascript. To understand its capability just clone the project and run the [demo application](demo/demo.md) ":pig: PiggyBank".
+
+![Screenshots Collage](demo/collage.png)
 
-The following code will care three pages application with the top-level menu bar for navigations.  
+For more information also read the Bootwrap [documentation](https://mmgalushka.github.io/bootwrap/).
+
+## Hello World Application
+
+The following code will create three pages application with a top-level menu bar for navigations. Since this application is based on [Flask](https://palletsprojects.com/p/flask/) make sure that you installed it as well.
 
 ```Python
 from flask import Flask, Markup
 from bootwrap import Page, Menu, Image, Anchor, Button, Text
 
-# Both 'logo.png' and 'favicon.ico' are stored in 'docs' folder
 app = Flask(__name__, static_folder='docs', static_url_path='')
 
+LOGO = 'https://github.com/mmgalushka/bootwrap/blob/main/docs/logo.png?raw=true'
+FAVICON = 'https://raw.githubusercontent.com/mmgalushka/bootwrap/main/docs/favicon.ico'
+
 class MyMenu(Menu):
     def __init__(self):
         super().__init__(
-            logo=Image('logo.png', width=32, alt='Logo'),
+            logo=Image(LOGO, width=32, alt='Logo'),
             brand=Text('Bootwrap').as_strong().as_light().ml(2),
             anchors=[
                 Anchor('Home').link('/'),
                 Anchor('About').link('/about')
             ], 
             actions=[
                 Button('Sign In').as_outline().as_light().link('/signin')
             ]
         )
 
 class MyPage(Page):
     def __init__(self, container):
         super().__init__(
-            favicon = 'favicon.ico',
+            favicon = FAVICON,
             title='Hello World Application',
             menu=MyMenu(),
             container=container
         )
 
 @app.route('/')
 def home():
-    return Markup(MyPage(container=[Text('Home').as_heading(1)]))
+    return Markup(MyPage(container=Text('Home').as_heading(1)))
 
 @app.route('/about')
 def about():
-    return Markup(MyPage(container=[Text('About').as_heading(1)]))
+    return Markup(MyPage(container=Text('About').as_heading(1)))
 
 @app.route('/signin')
 def signin():
-    return Markup(MyPage(container=[Text('Sign In').as_heading(1)]))
+    return Markup(MyPage(container=Text('Sign In').as_heading(1)))
 
 if __name__ == '__main__':
     app.run(debug=True)
 ```
 
 Use the following command to launch the application.
 
@@ -86,10 +96,10 @@
 ## Contributing
 
 For information on how to set up a development environment and how to make a contribution to Bootwrap, see the [contributing guidelines](CONTRIBUTING.md).
 
 ## Links
 
 - Documentation: [https://mmgalushka.github.io/bootwrap/](https://mmgalushka.github.io/bootwrap/)
-- PyPI Releases: [https://test.pypi.org/project/bootwrap/](https://test.pypi.org/project/bootwrap/)
+- PyPI Releases: [https://pypi.org/project/bootwrap/](https://pypi.org/project/bootwrap/)
 - Source Code: [https://github.com/mmgalushka/bootwrap](https://github.com/mmgalushka/bootwrap/)
 - Issue Tracker: [https://github.com/mmgalushka/bootwrap/issues](https://github.com/mmgalushka/bootwrap/)
```

### Comparing `bootwrap-1.0.0/bootwrap/components/__init__.py` & `bootwrap-1.0.1/bootwrap/components/__init__.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/bootwrap/components/anchor.py` & `bootwrap-1.0.1/bootwrap/components/anchor.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,17 +25,14 @@
     conjunction with other components, for example, in creating a navigation
     menu.
 
     Args:
         inner (str|WebComponent): The object wrapped by the anchor.
 
     Example:
-        Anchor('Google Search').link('https://www.google.com/')
-
-    Demo:
         from bootwrap import Anchor
         output = Anchor('Google Search').link('https://www.google.com/')
     """
 
     def __init__(self, inner=None):
         super().__init__()
         self._inner = inner
```

### Comparing `bootwrap-1.0.0/bootwrap/components/badge.py` & `bootwrap-1.0.1/bootwrap/components/badge.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,18 @@
 class Badge(WebComponent, ClassMixin, AppearanceMixin):
     """A web component for a badge.
 
     Args:
         label (str): The badge label (text showing inside a badge).
 
     Example:
-        Badge('Some Badge')
-
-    Demo:
         from bootwrap import Badge
         output = Badge('Some Badge')
     """
+
     def __init__(self, label):
         super().__init__()
         self.__label = label
 
     def __str__(self):
         classes = 'badge'
         if self._category:
```

### Comparing `bootwrap-1.0.0/bootwrap/components/base.py` & `bootwrap-1.0.1/bootwrap/components/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -655,16 +655,16 @@
     """The breakpoint constants.
 
     Breakpoints are defined by Bootstrap and mostly based on minimum
     viewport widths and allow us to scale up elements as the viewport
     changes.
 
     See <a href="https://getbootstrap.com/docs/4.0/layout/overview/#responsive-breakpoints">
-    Bootstrap documentation</a> for more information.
-    """
+    for more information.
+    """  # NOQA
     XS = 'xs'
     SM = 'sm'
     MD = 'md'
     LG = 'lg'
     XL = 'xl'
```

### Comparing `bootwrap-1.0.0/bootwrap/components/button.py` & `bootwrap-1.0.1/bootwrap/components/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,14 @@
     Without applying a stylized method `Button` will be appearing very
     similar to the `Anchor`.
 
     Args:
         name (str): The button name.
 
     Example:
-        Button('Google Search').link('https://www.google.com/')
-
-    Demo:
         from bootwrap import Button
         output = Button('Google Search').link('https://www.google.com/')
     """
 
     def __init__(self, name):
         super().__init__()
         self.__name = name
@@ -148,15 +145,14 @@
                 </button>
             '''
         elif self._action == Action.SUBMIT:
             return f'''
                 <button {attr('id', self.identifier)}
                     {attr('class', self.classes)}
                     type="submit"
-                    onclick="return false;"
                     {attr('disabled', self._disabled)}>
                     {self.__name}
                 </button>
             '''
         else:
             return f'''
                 <button {attr('id', self.identifier)}
```

### Comparing `bootwrap-1.0.0/bootwrap/components/deck.py` & `bootwrap-1.0.1/bootwrap/components/list.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,256 +5,202 @@
 from .base import WebComponent, ClassMixin
 from .anchor import Anchor
 from .button import Button
 from .text import Text
 from .utils import attr, inject
 
 
-class Deck(WebComponent, ClassMixin):
-    """A web component for a deck of cards.
+class List(WebComponent, ClassMixin):
+    """A web component for a list of items.
 
     Args:
-        *cards (list): The `list` of `Deck.Card` elements.
+        *items (list): The `list` of `List.Item` elements.
 
     Example:
-        from bootwrap import Button, Deck, Image
+        from bootwrap import Button, List, Image
 
         actions = [
-            Button("Buy"),
+            Button("Buy").as_success(),
             Button("Sell"),
             Button("Transfer")
         ]
 
-        Deck(
-            Deck.Card(
+        output = List(
+            List.Item(
                 "Google (NASDAQ: GOOGL)",
                 description= "Price for a single Google share",
-                figure=Image("google-logo.png", width=128).mt(3),
+                figure=Image("google-logo.png", width=32, height=32),
                 marker="12:04:58 12/01/2021"
-            ).add_menu(*actions).pack_actions().link(
-                "https://www.google.com"),
-            Deck.Card(
-                "LinkedIn (NASDAQ: LNKD)",
-                description= "Price for a single LinkedIn share",
-                figure=Image("linkedin-logo.png", width=128).mt(3),
-                marker="12:04:58 12/01/2021"
-            ).add_menu(*actions).pack_actions().link(
-                "https://www.linkedin.com"),
-            Deck.Card(
-                "Amazon (NASDAQ: AMZN)",
-                description= "Price for a single Amazon share",
-                figure=Image("amazon-logo.png", width=128).mt(3),
-                marker="12:04:58 12/01/2021"
-            ).add_menu(*actions).pack_actions().link(
-                "https://www.amazon.com")
-        )
-
-    Demo:
-        from bootwrap import Button, Deck, Image
-        actions = [
-            Button("Buy"),
-            Button("Sell"),
-            Button("Transfer")
-        ]
-        output = Deck(
-            Deck.Card(
-                "Google (NASDAQ: GOOGL)",
-                description= "Price for a single Google share",
-                figure=Image("google-logo.png", width=128).mt(3),
-                marker="12:04:58 12/01/2021"
-            ).add_menu(*actions).pack_actions().link(
+            ).add_menu(*actions).pack_actions().as_selected().link(
                 "https://www.google.com"),
-            Deck.Card(
+            List.Item(
                 "LinkedIn (NASDAQ: LNKD)",
                 description= "Price for a single LinkedIn share",
-                figure=Image("linkedin-logo.png", width=128).mt(3),
+                figure=Image("linkedin-logo.png", width=32, height=32),
                 marker="12:04:58 12/01/2021"
             ).add_menu(*actions).pack_actions().link(
                 "https://www.linkedin.com"),
-            Deck.Card(
+            List.Item(
                 "Amazon (NASDAQ: AMZN)",
                 description= "Price for a single Amazon share",
-                figure=Image("amazon-logo.png", width=128).mt(3),
+                figure=Image("amazon-logo.png", width=32, height=32),
                 marker="12:04:58 12/01/2021"
             ).add_menu(*actions).pack_actions().link(
                 "https://www.amazon.com")
         )
     """
 
-    def __init__(self, *cards):
+    def __init__(self, *items):
         super().__init__()
 
-        for card in cards:
-            if not isinstance(card, Deck.Card):
+        for item in items:
+            if not isinstance(item, List.Item):
                 raise TypeError(
-                    f'A deck must contain the {Deck.Card.__class__} only '
-                    f'but got {type(card)};'
+                    f'A list must contain the {List.Item.__class__} only '
+                    f'but got {type(item)};'
                 )
-        self._cards = cards
+        self._items = items
 
-    class Card(Anchor):
-        """A deck card.
+    class Item(Anchor):
+        """A list item.
 
         Args:
-            title (str|WebComponent): The card title.
-            description (str|WebComponent): The card description.
-            marker (str|WebComponent): The card marker.
-            figure (str|WebComponent): The card figure.
+            title (str|WebComponent): The item title.
+            description (str|WebComponent): The item description.
+            marker (str|WebComponent): The item marker.
+            figure (str|WebComponent): The item figure.
 
         Example:
-            from bootwrap import Button, Deck, Image
+            from bootwrap import Button, List, Image
 
             actions = [
                 Button("Buy"),
                 Button("Sell"),
                 Button("Transfer")
             ]
 
-            Deck.Card(
+            output = List.Item(
                 "Google (NASDAQ: GOOGL)",
                 description= "Price for a single Google share",
-                figure=Image("google-logo.png", width=128).mt(3),
-                marker="12:04:58 12/01/2021"
-            ).add_menu(*actions).link(
-                "https://www.google.com")
-
-        Demo:
-            from bootwrap import Button, Deck, Image
-
-            actions = [
-                Button("Buy"),
-                Button("Sell"),
-                Button("Transfer")
-            ]
-
-            output = Deck.Card(
-                "Google (NASDAQ: GOOGL)",
-                description= "Price for a single Google share",
-                figure=Image("google-logo.png", width=128).mt(3),
+                figure=Image("google-logo.png", width=32, height=32),
                 marker="12:04:58 12/01/2021"
             ).add_menu(*actions).link(
                 "https://www.google.com")
         """
 
         def __init__(self, title, description=None, marker=None, figure=None):
             super().__init__()
             self._title = title
             self._description = description
             self._marker = marker
             self._figure = figure
+            self._selected = False
             self._pack_actions = False
 
-        def pack_actions(self):
-            """Makes item actions packed under a drop-down menu.
+        def as_selected(self):
+            """Makes a list item selected.
 
             Returns:
                 self
 
-        Example:
-            from bootwrap import Button, Deck, Image
+            Example:
+                from bootwrap import Button, List, Image
 
-            actions = [
-                Button("Buy"),
-                Button("Sell"),
-                Button("Transfer")
-            ]
+                actions = [
+                    Button("Buy"),
+                    Button("Sell"),
+                    Button("Transfer")
+                ]
+
+                output = List.Item(
+                    "Google (NASDAQ: GOOGL)",
+                    description= "Price for a single Google share",
+                    figure=Image("google-logo.png", width=32, height=32),
+                    marker="12:04:58 12/01/2021"
+                ).add_menu(*actions).as_selected().link(
+                    "https://www.google.com")
+            """
+            self._selected = True
+            return self
 
-            Deck.Card(
-                "Google (NASDAQ: GOOGL)",
-                description= "Price for a single Google share",
-                figure=Image("google-logo.png", width=128).mt(3),
-                marker="12:04:58 12/01/2021"
-            ).add_menu(*actions).pack_actions().link(
-                "https://www.google.com")
+        def pack_actions(self):
+            """Makes item actions packed under a drop-down menu.
 
-        Demo:
-            from bootwrap import Button, Deck, Image
+            Returns:
+                self
 
-            actions = [
-                Button("Buy"),
-                Button("Sell"),
-                Button("Transfer")
-            ]
+            Example:
+                from bootwrap import Button, List, Image
 
-            output = Deck.Card(
-                "Google (NASDAQ: GOOGL)",
-                description= "Price for a single Google share",
-                figure=Image("google-logo.png", width=128).mt(3),
-                marker="12:04:58 12/01/2021"
-            ).add_menu(*actions).pack_actions().link(
-                "https://www.google.com")
+                actions = [
+                    Button("Buy"),
+                    Button("Sell"),
+                    Button("Transfer")
+                ]
+
+                output = List.Item(
+                    "Google (NASDAQ: GOOGL)",
+                    description= "Price for a single Google share",
+                    figure=Image("google-logo.png", width=32, height=32),
+                    marker="12:04:58 12/01/2021"
+                ).add_menu(*actions).pack_actions().link(
+                    "https://www.google.com")
             """
             self._pack_actions = True
             return self
 
         def __str__(self):
             wc_title = self._title
-            if isinstance(wc_title, str):
-                wc_title = Text(wc_title).as_heading(5).\
-                    add_classes('card-title')
-            else:
-                wc_title.add_classes('card-title')
+            if wc_title:
+                if isinstance(wc_title, str):
+                    wc_title = Text(wc_title).as_heading(5)
 
             wc_marker = self._marker
             if wc_marker:
                 if isinstance(wc_marker, str):
-                    wc_marker = Text(wc_marker).as_small().as_muted()
-                wc_marker = f'''
-                    <div class="text-right mb-2">
-                        {inject(wc_marker)}
-                    </div>
-                '''
+                    wc_marker = Text(wc_marker).as_small()
 
             wc_actions = None
             if self._menu:
                 if self._pack_actions:
-                    wc_actions = f'''
-                        <div class="card-footer text-right">
-                            {inject(Button("...").add_menu(*self._menu))}
-                        </div>
-                    '''
+                    wc_actions = Button('...').add_menu(*self._menu)
                 else:
                     for action in self._menu:
                         action.ml(1)
-                    wc_actions = f'''
-                        <div class="card-footer text-right">
-                            {inject(*self._menu)}
-                        </div>
-                    '''
+                    wc_actions = inject(*self._menu)
+                wc_actions = f'''
+                    <div class="d-flex align-items-start">
+                        {inject(wc_actions)}
+                    </div>
+                '''
 
             self._inner = f'''
-                <div class="row justify-content-center">
+                <div class="d-flex w-100 justify-content-between">
                     {inject(self._figure)}
+                    <div class="ml-2 mr-2 w-100">
+                        <div class="d-flex w-100 justify-content-between">
+                            {inject(wc_title)}
+                            {inject(wc_marker)}
+                        </div>
+                        {inject(self._description)}
+                    </div>
+                    {inject(wc_actions)}
                 </div>
-                <div class="card-body">
-                    {inject(wc_marker)}
-                    {inject(wc_title)}
-                    {inject(self._description)}
-                </div>
-                {inject(wc_actions)}
             '''
 
-            self.add_classes('card')
+            self.add_classes(
+                'list-group-item list-group-item-action flex-column '
+                'align-items-start'
+            )
+            if self._selected:
+                self.add_classes('active')
 
             return super().__str__()
 
     def __str__(self):
-        style = '''
-            <style>
-                a.card {
-                    text-decoration: none;
-                }
-
-                a.card, a.card:visited, a.card:hover, a.card:active {
-                    color: inherit;
-                }
-            </style>
-        '''
-
-        self.add_classes('card-deck grid-container')
+        self.add_classes('list-group')
         return f'''
             <div {attr("id", self.identifier)}
                 {attr('class', self.classes)}>
-                {inject(*self._cards)}
+                {inject(*self._items)}
             </div>
-            {style}
         '''
```

### Comparing `bootwrap-1.0.0/bootwrap/components/dialog.py` & `bootwrap-1.0.1/bootwrap/components/dialog.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,35 +11,26 @@
 
     Args:
         title (str): The dialog title.
         content (str|WebComponent): The content inside a dialog window to show.
         *actions (list): The dialog actions.
 
     Example:
-        from bootwrap import Dialog, Button
-
-        dialog = Dialog(
-            'Greeting',
-            'Hello World!',
-            Button('Bye').dismiss()
-        )
-        button = Button('Say Hello').toggle(dialog)
-
-    Demo:
         from bootwrap import Panel, Dialog, Button
 
         dialog = Dialog(
             'Greeting',
             'Hello World!',
             Button('Bye').dismiss()
         )
         button = Button('Say Hello').toggle(dialog)
 
         output = Panel(dialog, button)
     """
+
     def __init__(self, title, content, *actions):
         super().__init__()
         self.__title = title
         self.__content = content
         self.__actions = actions
 
     def __str__(self):
```

### Comparing `bootwrap-1.0.0/bootwrap/components/form.py` & `bootwrap-1.0.1/bootwrap/components/form.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
         Form(
             # here should be an enumeration  of
             # input components and actions
             ...
         ).on_submit('go/to/this/url')
     """
+
     def __init__(self, *components):
         super().__init__()
         self.__components = components
         self.__href = None
 
     def on_submit(self, href):
         """Sets the submit URL, for the POST request.
@@ -64,14 +65,15 @@
 class Input(ABC, WebComponent, ClassMixin, AvailabilityMixin):
     """A base input.
 
     Args:
         label (str): The input label.
         name (str): The input name.
     """
+
     def __init__(self, label, name):
         super().__init__()
         self.__label = label
         self._name = name
         self.__label_on_top = False
 
     def label_on_top(self):
@@ -92,17 +94,17 @@
 
         if self.__label:
             label_classes = None
             receiver_classes = None
             if not self.__label_on_top:
                 self.add_classes('row')
                 label_classes = \
-                    'col-sm-2 col-form-label d-flex align-items-center'
+                    'col-sm-4 col-form-label d-flex align-items-center'
                 receiver_classes = \
-                    'col-sm-10 d-flex align-items-center'
+                    'col-sm-8 d-flex align-items-center'
             return f'''
                 <div {attr('class', self.classes)}>
                     <label {attr('class', label_classes)}
                         {attr('for', self.identifier)}>
                         {self.__label}
                     </label>
                     <div {attr('class', receiver_classes)}>
@@ -127,29 +129,21 @@
         label (str): The input label.
         name (str): The input name.
         checked (bool): The check box status.
 
     Example:
         from bootwrap import Form, CheckboxInput
 
-        Form(
-            CheckboxInput('One', 'opt1'),
-            CheckboxInput('Two', 'opt2', True),
-            CheckboxInput('Three', 'opt3').as_disabled()
-        )
-
-    Demo:
-        from bootwrap import Form, CheckboxInput
-
         output = Form(
             CheckboxInput('One', 'opt1'),
             CheckboxInput('Two', 'opt2', True),
             CheckboxInput('Three', 'opt3').as_disabled()
         )
     """
+
     def __init__(self, label, name, checked=False):
         super().__init__(label, name)
         self.__checked = checked
 
     def _receiver(self):
         return f'''
             <input {attr('id', self.identifier)}
@@ -167,14 +161,15 @@
 
     Args:
         label (str): The input label
         name (str): The input name.
         value (str): The input value.
         placeholder (str): The input placeholder.
     """
+
     def __init__(self, label, name, value, placeholder):
         super().__init__(label, name)
         self.__value = value
         self.__placeholder = placeholder
         self._type = None
         self._rows = 1
 
@@ -215,30 +210,22 @@
         name (str): The input name.
         value (str): The input value.
         placeholder (str): The input placeholder.
 
     Example:
         from bootwrap import Form, TextInput
 
-        Form(
-            TextInput('Text1', 'text'),
-            TextInput('Text2', 'text', placeholder='type here'),
-            TextInput('Text3', 'text', 'Hello World!'),
-            TextInput('Text4', 'text').as_disabled()
-        )
-    Demo:
-        from bootwrap import Form, TextInput
-
         output = Form(
             TextInput('Text1', 'text'),
             TextInput('Text2', 'text', placeholder='type here'),
             TextInput('Text3', 'text', 'Hello World!'),
             TextInput('Text4', 'text').as_disabled()
         )
     """
+
     def __init__(self, label, name, value=None, placeholder=None):
         super().__init__(label, name, value, placeholder)
         self._type = 'text'
 
     def with_multirows(self, n):
         """Sets the number of rows.
 
@@ -247,20 +234,14 @@
 
         Returns:
             obj (self): The instance of this class.
 
         Example:
             from bootwrap import Form, TextInput
 
-            Form(
-                TextInput('Text', 'text').with_multirows(3)
-            )
-        Demo:
-            from bootwrap import Form, TextInput
-
             output = Form(
                 TextInput('Text', 'text').with_multirows(3)
             )
         """
         self._rows = n
         return self
 
@@ -269,20 +250,14 @@
 
         Returns:
             obj (self): The instance of this class.
 
         Example:
             from bootwrap import Form, TextInput
 
-            Form(
-                TextInput('Email', 'email', 'my@email.com').for_email()
-            )
-        Demo:
-            from bootwrap import Form, TextInput
-
             output = Form(
                 TextInput('Email', 'email', 'my@email.com').for_email()
             )
         """
         self._type = 'email'
         return self
 
@@ -291,21 +266,14 @@
 
         Returns:
             obj (self): The instance of this class.
 
         Example:
             from bootwrap import Form, TextInput
 
-            Form(
-                TextInput('Password', 'password', '********').for_password()
-            )
-
-        Demo:
-            from bootwrap import Form, TextInput
-
             output = Form(
                 TextInput('Password', 'password', '********').for_password()
             )
         """
         self._type = 'password'
         return self
 
@@ -319,32 +287,24 @@
     Args:
         label (str): The input label
         name (str): The input name.
         value (obj): The input value.
         placeholder (str): The input placeholder.
 
     Example:
-        from bootwrap import Form, TextInput
-
-        Form(
-            NumericInput('Number1', 'number'),
-            NumericInput('Number2', 'number', placeholder='type here'),
-            NumericInput('Number3', 'number', 123),
-            NumericInput('Number4', 'number').as_disabled()
-        )
-    Demo:
         from bootwrap import Form, NumericInput
 
         output = Form(
             NumericInput('Number1', 'number'),
             NumericInput('Number2', 'number', placeholder='type here'),
             NumericInput('Number3', 'number', 123),
             NumericInput('Number4', 'number').as_disabled()
         )
     """
+
     def __init__(self, label, name, value=None, placeholder=None):
         super().__init__(label, name, value, placeholder)
         self._type = 'number'
 
 
 class SelectInput(Input):
     """A select input.
@@ -363,33 +323,20 @@
 
         options = [
             SelectInput.Option('One', 1),
             SelectInput.Option('Two', 2),
             SelectInput.Option('Three', 3, disabled=True)
         ]
 
-        Form(
-            SelectInput('Selector1', 'choice', 2, options)
-            SelectInput('Selector2', 'choice', 2, options).as_disabled()
-        )
-
-    Demo:
-        from bootwrap import Form, SelectInput
-
-        options = [
-            SelectInput.Option('One', 1),
-            SelectInput.Option('Two', 2),
-            SelectInput.Option('Three', 3, disabled=True)
-        ]
-
         output = Form(
             SelectInput('Selector1', 'choice', 2, options),
             SelectInput('Selector2', 'choice', 2, options).as_disabled()
         )
     """
+
     def __init__(self, label, name, value=None, options=None):
         super().__init__(label, name)
         self.__value = value
         self.__options = options
         self.__radio = False
 
     class Option(WebComponent):
@@ -397,14 +344,15 @@
 
         Args:
             name (str): The option name.
             value (str): The option value value.
             disabled (bool): `True` makes the option disabled (in other words
                 user will not be able to choose this option).
         """
+
         def __init__(self, name, value, disabled=False):
             super().__init__()
             self.__name = name
             self.__value = value
             self.__disabled = disabled
 
         @property
@@ -430,27 +378,14 @@
 
             options = [
                 SelectInput.Option('One', 1),
                 SelectInput.Option('Two', 2),
                 SelectInput.Option('Three', 3, disabled=True)
             ]
 
-            Form(
-                SelectInput('Selector', 'choice', 2, options).as_radio()
-            )
-
-        Demo:
-            from bootwrap import Form, SelectInput
-
-            options = [
-                SelectInput.Option('One', 1),
-                SelectInput.Option('Two', 2),
-                SelectInput.Option('Three', 3, disabled=True)
-            ]
-
             output = Form(
                 SelectInput('Selector', 'choice', 2, options).as_radio()
             )
         """
         self.__radio = True
         return self
 
@@ -508,14 +443,15 @@
     Example:
         from bootwrap import Form, SelectInput
 
         Form(
             HiddenInput('token', '123')
         )
     """
+
     def __init__(self, name, value=None):
         super().__init__(None, name)
         self.__value = value
 
     def _receiver(self):
         return f'''
             <input {attr('id', self.identifier)}
@@ -541,23 +477,16 @@
     Example:
         from bootwrap import Form, FileInput
 
         output = Form(
             FileInput('File', 'file'),
             FileInput('File', 'file').as_disabled()
         )
-
-    Demo:
-        from bootwrap import Form, FileInput
-
-        output = Form(
-            FileInput('File', 'file'),
-            FileInput('File', 'file').as_disabled()
-        )
     """
+
     def __init__(self, label, name):
         super().__init__(label, name)
 
     def _receiver(self):
         browse_button_class = 'btn btn-secondary'
         if self._disabled:
             browse_button_class += ' disabled'
```

### Comparing `bootwrap-1.0.0/bootwrap/components/icon.py` & `bootwrap-1.0.1/bootwrap/components/icon.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,41 +13,29 @@
 class Icon(WebComponent, ClassMixin, AppearanceMixin):
     """An icon.
 
     Args:
         name (str): The icon name.
 
     Example:
-        from bootwrap import Icon
-
-        Icon("fas fa-folder")
-        Icon("fas fa-folder").as_primary()
-        Icon("fas fa-folder").as_secondary()
-        Icon("fas fa-folder").as_success()
-        Icon("fas fa-folder").as_warning()
-        Icon("fas fa-folder").as_danger()
-        Icon("fas fa-folder").as_info()
-        Icon("fas fa-folder").as_light()
-        Icon("fas fa-folder").as_dark()
-
-    Demo:
         from bootwrap import Icon, Panel
 
         output = Panel(
             Icon("fas fa-folder"),
             Icon("fas fa-folder").as_primary(),
             Icon("fas fa-folder").as_secondary(),
             Icon("fas fa-folder").as_success(),
             Icon("fas fa-folder").as_warning(),
             Icon("fas fa-folder").as_danger(),
             Icon("fas fa-folder").as_info(),
             Icon("fas fa-folder").as_light(),
             Icon("fas fa-folder").as_dark()
         )
     """
+
     def __init__(self, name):
         super().__init__()
         self.__name = name
 
     def __str__(self):
         self.add_classes(self.__name)
 
@@ -61,41 +49,29 @@
         '''
 
 
 class Spinner(WebComponent, ClassMixin, AppearanceMixin):
     """A spinner icon.
 
     Example:
-        from bootwrap import Spinner
-
-        Spinner()
-        Spinner().as_primary()
-        Spinner().as_secondary()
-        Spinner().as_success()
-        Spinner().as_warning()
-        Spinner().as_danger()
-        Spinner().as_info()
-        Spinner().as_light()
-        Spinner().as_dark()
-
-    Demo:
         from bootwrap import Spinner, Panel
 
         output = Panel(
             Spinner(),
             Spinner().as_primary(),
             Spinner().as_secondary(),
             Spinner().as_success(),
             Spinner().as_warning(),
             Spinner().as_danger(),
             Spinner().as_info(),
             Spinner().as_light(),
             Spinner().as_dark()
         )
     """
+
     def __str__(self):
         self.add_classes('spinner')
 
         if self._category is not None:
             self.add_classes('text-%s' % self._category)
 
         return f'''
```

### Comparing `bootwrap-1.0.0/bootwrap/components/image.py` & `bootwrap-1.0.1/bootwrap/components/image.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,20 +17,17 @@
         width (int): The image width.
         height (int): The image height.
         alt (str): The alt text.
 
     Example:
         from bootwrap import Image
 
-        Image("logo.png", width=64, height=64, alt="Bootwarp Logo")
-    Demo:
-        from bootwrap import Image
-
         output = Image("logo.png")
     """
+
     def __init__(self, src, width=None, height=None, alt=None):
         super().__init__()
         self.__src = src
         self.__width = width
         self.__height = height
         self.__alt = alt
```

### Comparing `bootwrap-1.0.0/bootwrap/components/javascript.py` & `bootwrap-1.0.1/bootwrap/components/javascript.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/bootwrap/components/link.py` & `bootwrap-1.0.1/bootwrap/components/link.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/bootwrap/components/text.py` & `bootwrap-1.0.1/bootwrap/components/text.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,19 +17,14 @@
 
     Args:
         content (str): The textual content.
 
     Example:
         from bootwrap import Text
 
-        Text("Normal text")
-
-    Demo:
-        from bootwrap import Text
-
         output = Text("Normal text")
     """
 
     def __init__(self, content):
         super().__init__()
         self.__content = content
         self.__level = 0
@@ -43,19 +38,14 @@
 
         Returns:
             obj (self): The instance of this class.
 
         Example:
             from bootwrap import Text
 
-            Text("Muted text").as_muted()
-
-        Demo:
-            from bootwrap import Text
-
             output = Text("Muted text").as_muted()
         """
         self._category = 'muted'
         return self
 
     def as_heading(self, level):
         """Makes the text as heading.
@@ -63,24 +53,14 @@
         Args:
             level (int): The heading level;
 
         Returns:
             obj (self): The instance of this class.
 
         Example:
-            from bootwrap import Text
-
-            Text("Header text 1").as_heading(1)
-            Text("Header text 2").as_heading(2)
-            Text("Header text 3").as_heading(3)
-            Text("Header text 4").as_heading(4)
-            Text("Header text 5").as_heading(5)
-            Text("Header text 6").as_heading(6)
-
-        Demo:
             from bootwrap import Panel, Text
 
             output = Panel(
                 Text("Header text 1").as_heading(1),
                 Text("Header text 2").as_heading(2),
                 Text("Header text 3").as_heading(3),
                 Text("Header text 4").as_heading(4),
@@ -101,56 +81,40 @@
 
         Returns:
             obj (self): The instance of this class.
 
         Example:
             from bootwrap import Text
 
-            Text("Small text").as_small()
-
-        Demo:
-            from bootwrap import Text
-
             output = Text("Small text").as_small()
         """
         self.__small = True
         return self
 
     def as_strong(self):
         """Makes the text as strong.
 
         Returns:
             obj (self): The instance of this class.
 
         Example:
             from bootwrap import Text
 
-            Text("Strong text").as_strong()
-
-        Demo:
-            from bootwrap import Text
-
             output = Text("Strong text").as_strong()
         """
         self.__strong = True
         return self
 
     def as_paragraph(self):
         """Makes the text wrap in a paragraph.
 
         Returns:
             obj (self): The instance of this class.
 
         Example:
-            from bootwrap import Text
-
-            Text("Paragraph 1").as_paragraph()
-            Text("Paragraph 2").as_paragraph()
-            Text("Paragraph 3").as_paragraph()
-        Demo:
             from bootwrap import Panel, Text
 
             output = Panel(
                 Text("Paragraph 1").as_paragraph(),
                 Text("Paragraph 2").as_paragraph(),
                 Text("Paragraph 3").as_paragraph()
             )
@@ -161,18 +125,14 @@
     def as_code(self):
         """Makes the text wrap as a code snippet.
 
         Returns:
             obj (self): The instance of this class.
 
         Example:
-            from bootwrap import Text
-
-            Text("print('Hello world!')").as_code()
-        Demo:
             from bootwrap import Panel, Text
 
             output = Text("print('Hello world!')").as_code()
         """
         self.__code = True
         return self
```

### Comparing `bootwrap-1.0.0/bootwrap/components/utils.py` & `bootwrap-1.0.1/bootwrap/components/utils.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/bootwrap/menu.py` & `bootwrap-1.0.1/bootwrap/menu.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/bootwrap.egg-info/PKG-INFO` & `bootwrap-1.0.1/bootwrap.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: bootwrap
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package for rapid development of web-based user interfaces.
 Home-page: https://github.com/mmgalushka/bootwrap
 Author: Mykola Galushka
 Author-email: mm.galushka@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/mmgalushka/bootwrap/issues
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,71 +22,81 @@
 [![Code Coverage Percentage](https://codecov.io/gh/mmgalushka/bootwrap/branch/main/graphs/badge.svg)](https://codecov.io/gh/mmgalushka/bootwrap)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/763657a471ff424c85a5b894ddb750d0)](https://www.codacy.com/gh/mmgalushka/bootwrap/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mmgalushka/bootwrap&amp;utm_campaign=Badge_Grade)
 [![Project License](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/mmgalushka/bootwrap/blob/main/LICENSE)
 [![Project Documentation](https://img.shields.io/badge/docs-up--to--date-success)](https://mmgalushka.github.io/bootwrap/)
 
 **Bootwrap** is a Python library for rapid developing of web-based user interfaces (WebUI). It helps creating WebUI using Python code only and can be used in conjunction with different web-development frameworks such as [Flask](https://palletsprojects.com/p/flask/). Under the hood, this library wraps one of the most popular front-end toolkit [Bootstrap](https://getbootstrap.com/).
 
-This library would be useful for developers and data scientists who wish to build interactive web-application without crafting HTML, CSS and Javascript.
-
 As a showcase of what this library is capable of please check the documentation. The entire [documentation](https://mmgalushka.github.io/bootwrap/) web interface is created using the **Bootwrap**.
 
 ## Installing
 
 Install and update using [pip](https://pip.pypa.io/en/stable/quickstart/):
 
 ```bash
 ~$ pip install bootwrap
 ```
 
-## A Simple Example
+Bootwrap package has no external dependencies!
+
+## Why & where you might use Bootwrap?
+
+The vast majority of web applications consist of frontend and backend. If you are a small team or even a solo developer you need to divide resources and time to focus on both parts. This often results in switching between different platforms such as Python and [React](https://reactjs.org/), [AngularJs](https://angular.io/), Flask templates (HTML, CSS, JS), etc. But what if your main focus is the backend and you also don't want to compromise on the quality of your WebUI. In this case, the Bootwrap library is for you! It will help you develop WebUI without leaving the Python ecosystem and not waste your time on HTML, CSS, and Javascript. To understand its capability just clone the project and run the [demo application](demo/demo.md) ":pig: PiggyBank".
+
+![Screenshots Collage](demo/collage.png)
+
+For more information also read the Bootwrap [documentation](https://mmgalushka.github.io/bootwrap/).
 
-The following code will care three pages application with the top-level menu bar for navigations.  
+## Hello World Application
+
+The following code will create three pages application with a top-level menu bar for navigations. Since this application is based on [Flask](https://palletsprojects.com/p/flask/) make sure that you installed it as well.
 
 ```Python
 from flask import Flask, Markup
 from bootwrap import Page, Menu, Image, Anchor, Button, Text
 
-# Both 'logo.png' and 'favicon.ico' are stored in 'docs' folder
 app = Flask(__name__, static_folder='docs', static_url_path='')
 
+LOGO = 'https://github.com/mmgalushka/bootwrap/blob/main/docs/logo.png?raw=true'
+FAVICON = 'https://raw.githubusercontent.com/mmgalushka/bootwrap/main/docs/favicon.ico'
+
 class MyMenu(Menu):
     def __init__(self):
         super().__init__(
-            logo=Image('logo.png', width=32, alt='Logo'),
+            logo=Image(LOGO, width=32, alt='Logo'),
             brand=Text('Bootwrap').as_strong().as_light().ml(2),
             anchors=[
                 Anchor('Home').link('/'),
                 Anchor('About').link('/about')
             ], 
             actions=[
                 Button('Sign In').as_outline().as_light().link('/signin')
             ]
         )
 
 class MyPage(Page):
     def __init__(self, container):
         super().__init__(
-            favicon = 'favicon.ico',
+            favicon = FAVICON,
             title='Hello World Application',
             menu=MyMenu(),
             container=container
         )
 
 @app.route('/')
 def home():
-    return Markup(MyPage(container=[Text('Home').as_heading(1)]))
+    return Markup(MyPage(container=Text('Home').as_heading(1)))
 
 @app.route('/about')
 def about():
-    return Markup(MyPage(container=[Text('About').as_heading(1)]))
+    return Markup(MyPage(container=Text('About').as_heading(1)))
 
 @app.route('/signin')
 def signin():
-    return Markup(MyPage(container=[Text('Sign In').as_heading(1)]))
+    return Markup(MyPage(container=Text('Sign In').as_heading(1)))
 
 if __name__ == '__main__':
     app.run(debug=True)
 ```
 
 Use the following command to launch the application.
 
@@ -104,12 +112,10 @@
 ## Contributing
 
 For information on how to set up a development environment and how to make a contribution to Bootwrap, see the [contributing guidelines](CONTRIBUTING.md).
 
 ## Links
 
 - Documentation: [https://mmgalushka.github.io/bootwrap/](https://mmgalushka.github.io/bootwrap/)
-- PyPI Releases: [https://test.pypi.org/project/bootwrap/](https://test.pypi.org/project/bootwrap/)
+- PyPI Releases: [https://pypi.org/project/bootwrap/](https://pypi.org/project/bootwrap/)
 - Source Code: [https://github.com/mmgalushka/bootwrap](https://github.com/mmgalushka/bootwrap/)
 - Issue Tracker: [https://github.com/mmgalushka/bootwrap/issues](https://github.com/mmgalushka/bootwrap/)
-
-
```

### Comparing `bootwrap-1.0.0/bootwrap.egg-info/SOURCES.txt` & `bootwrap-1.0.1/bootwrap.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 README.md
 helper.sh
 main.py
 pytest.ini
 requirements.txt
 setup.py
 ./bootwrap/__init__.py
+./bootwrap/auth.py
 ./bootwrap/menu.py
 ./bootwrap/page.py
 ./bootwrap/components/__init__.py
 ./bootwrap/components/anchor.py
 ./bootwrap/components/badge.py
 ./bootwrap/components/base.py
 ./bootwrap/components/button.py
@@ -27,21 +28,27 @@
 ./bootwrap/components/panel.py
 ./bootwrap/components/separator.py
 ./bootwrap/components/table.py
 ./bootwrap/components/text.py
 ./bootwrap/components/utils.py
 ./demo/__init__.py
 ./demo/demo_app.py
+./demo/demo_components.py
+./demo/demo_stock.py
+./demo/demo_user.py
 ./docs/__init__.py
 ./docs/doc_app.py
 ./docs/doc_generator.py
 .github/workflows/ci.yml
 .github/workflows/pre-release.yml
 .github/workflows/release.yml
 bootwrap/__init__.py
+bootwrap/auth.py
+bootwrap/generic.css
+bootwrap/generic.js
 bootwrap/menu.py
 bootwrap/page.py
 bootwrap.egg-info/PKG-INFO
 bootwrap.egg-info/SOURCES.txt
 bootwrap.egg-info/dependency_links.txt
 bootwrap.egg-info/top_level.txt
 bootwrap/components/__init__.py
@@ -60,15 +67,40 @@
 bootwrap/components/navigation.py
 bootwrap/components/panel.py
 bootwrap/components/separator.py
 bootwrap/components/table.py
 bootwrap/components/text.py
 bootwrap/components/utils.py
 demo/__init__.py
+demo/aapl-logo.png
+demo/account-screenshot.png
+demo/activity-screenshot.png
+demo/amzn-logo.png
+demo/background.jpg
+demo/bank.png
+demo/cash.png
+demo/collage.png
+demo/demo.md
 demo/demo_app.py
+demo/demo_components.py
+demo/demo_stock.py
+demo/demo_user.py
+demo/discovery-screenshot.png
+demo/favicon.ico
+demo/googl-logo.png
+demo/hard-work.jpg
+demo/lnkd-logo.png
+demo/login-screenshot.png
+demo/logo.png
+demo/nvda-logo.png
+demo/party.jpg
+demo/piggybank-title.png
+demo/portfolio-screenshot.png
+demo/stock.png
+demo/tsla-logo.png
 docs/__init__.py
 docs/amazon-logo.png
 docs/base.html
 docs/bootwrap-equation.png
 docs/components.html
 docs/doc_app.py
 docs/doc_generator.py
@@ -87,14 +119,15 @@
 docs/config/base.yaml
 docs/config/components.yaml
 docs/config/home.yaml
 docs/config/layout.yaml
 tests/__init__.py
 tests/helper.py
 tests/test_anchor.py
+tests/test_auth.py
 tests/test_badge.py
 tests/test_base.py
 tests/test_button.py
 tests/test_deck.py
 tests/test_dialog.py
 tests/test_form.py
 tests/test_helper.py
```

### Comparing `bootwrap-1.0.0/docs/amazon-logo.png` & `bootwrap-1.0.1/demo/amzn-logo.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/docs/base.html` & `bootwrap-1.0.1/docs/base.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!DOCTYPE html>
 <html lang="en">
  <head>
   <meta charset="utf-8"/>
-  <meta container="width=device-width, initial-scale=1,
+  <meta content="width=device-width, initial-scale=1,
                         shrink-to-fit=no" name="viewport"/>
   <link href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" rel="stylesheet" type="text/css"/>
   <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.8.2/css/all.min.css" rel="stylesheet" type="text/css"/>
   <link href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.5.0/styles/default.min.css" rel="stylesheet" type="text/css"/>
   <link href="favicon.ico" rel="icon" type="image/x-icon"/>
   <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.0/jquery.min.js" type="application/javascript">
   </script>
@@ -17,111 +17,111 @@
   <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.5.0/highlight.min.js" type="application/javascript">
   </script>
   <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.5.0/languages/python.min.js" type="application/javascript">
   </script>
  </head>
  <body>
   <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
-   <img alt="Bootwrap Logo" id="bbc65eb7-892f-4f57-a1e0-437b6f73236c" src="logo.png" width="32"/>
-   <span class="text-light" id="2ee48f05-668a-4295-8aa1-00f82007a44c">
+   <img alt="Bootwrap Logo" id="a7ed3caf-2915-4fd7-812b-57b803002330" src="logo.png" width="32"/>
+   <span class="text-light" id="c33b455d-ac1e-4da6-83c9-59e2e21871fa">
     <strong>
      Bootwrap
     </strong>
    </span>
    <button aria-controls="menu" aria-expanded="false" aria-label="Toggle menu" class="navbar-toggler" data-target="#menu" data-toggle="collapse" type="button">
     <span class="navbar-toggler-icon">
     </span>
    </button>
    <div class="collapse navbar-collapse" id="menu">
     <ul class="navbar-nav mr-auto">
      <li class="nav-item">
-      <a class="ml-2 nav-link" href="index.html" id="05197dcb-4e73-4ba3-8287-c45347b618f2">
+      <a class="ml-2 nav-link" href="index.html" id="ed93c436-1df6-4a4e-a5eb-a087566e3687">
        Home
       </a>
      </li>
      <li class="nav-item">
-      <a class="ml-2 nav-link" href="layout.html" id="86e79a59-44aa-4845-9455-3ee9e1227ae9">
+      <a class="ml-2 nav-link" href="layout.html" id="c8544c01-13b0-4c72-b919-1e4ecfabb7a5">
        Layout
       </a>
      </li>
      <li class="nav-item">
-      <a class="ml-2 nav-link" href="base.html" id="63ef0348-4e70-4ebd-88c1-4fe6057929e6">
+      <a class="ml-2 nav-link" href="base.html" id="fb295d10-044a-46c5-8018-1a110a27912e">
        Base
       </a>
      </li>
      <li class="nav-item">
-      <a class="ml-2 nav-link" href="components.html" id="52565d3b-ded7-488d-a3fa-05718407fc4b">
+      <a class="ml-2 nav-link" href="components.html" id="d6bd9e6c-5bda-47de-8769-aee8941cf202">
        Components
       </a>
      </li>
     </ul>
-    <a class="ml-2 btn btn-outline-light" href="https://github.com/mmgalushka/bootwrap" id="42ba6035-a489-49f8-b8bf-c124b65c670c" role="button">
+    <a class="ml-2 btn btn-outline-light" href="https://github.com/mmgalushka/bootwrap" id="7bf5d17d-cd37-46ab-a7c6-b6cbe7db31a2" role="button">
      GitHub
     </a>
    </div>
   </nav>
-  <div class="container" style="margin-top: 90px;">
-   <ul class="nav nav-pills" id="f4d2db86-3424-4ce8-ad15-654798edcb75" role="tablist">
+  <div class="container-fluid">
+   <ul class="nav nav-pills" id="3388ff02-fd4c-456b-8854-334904eeb0ec" role="tablist">
     <li class="nav-item">
-     <a class="nav-link active" data-target="#5e6b8038-7ef2-4d66-9a04-03364ae02f63" data-toggle="tab" href="#5e6b8038-7ef2-4d66-9a04-03364ae02f63" id="2451f8e2-8f21-44b5-8f6c-a74eace71ed8" role="tab">
+     <a class="nav-link active" data-target="#636c6d6f-38fe-40aa-83ea-8bf0a268a145" data-toggle="tab" href="#636c6d6f-38fe-40aa-83ea-8bf0a268a145" id="53ca0a6e-f70e-4c9d-8d49-7672c385a0af" role="tab">
       WebComponent
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#cfc04d99-146e-4e09-8489-733ec6372458" data-toggle="tab" href="#cfc04d99-146e-4e09-8489-733ec6372458" id="d1035dfc-437d-4f6d-8f9c-dc78804f89f3" role="tab">
+     <a class="nav-link" data-target="#77d9fddf-decd-486e-bcf1-42f100a5a571" data-toggle="tab" href="#77d9fddf-decd-486e-bcf1-42f100a5a571" id="7eb630da-0f60-4877-8f6f-93d05bce4470" role="tab">
       ClassMixin
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#3d850a70-d19c-49e0-9ddd-eb2e3581970f" data-toggle="tab" href="#3d850a70-d19c-49e0-9ddd-eb2e3581970f" id="f98c364e-99d0-4ca6-8d49-d2948ecb2742" role="tab">
+     <a class="nav-link" data-target="#91cf097f-77f6-40c0-a713-03c716d79f4f" data-toggle="tab" href="#91cf097f-77f6-40c0-a713-03c716d79f4f" id="a1a9eae3-b8a8-4cb2-8fad-265769ab78a8" role="tab">
       ActionMixin
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#a743d34d-aadd-4be3-a44f-008d0b782587" data-toggle="tab" href="#a743d34d-aadd-4be3-a44f-008d0b782587" id="fd0efd8b-594e-4c76-bcfc-5cbd53ad9133" role="tab">
+     <a class="nav-link" data-target="#8bb80617-6b52-4ffa-82c9-25c8edb4a396" data-toggle="tab" href="#8bb80617-6b52-4ffa-82c9-25c8edb4a396" id="4200375b-c965-4962-9ccd-8bac0922f8ad" role="tab">
       AppearanceMixin
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#d7783dd1-0b16-4963-95e8-2f5ba94d6a16" data-toggle="tab" href="#d7783dd1-0b16-4963-95e8-2f5ba94d6a16" id="325f5ab9-0577-483d-b649-e8c10efb4fa0" role="tab">
+     <a class="nav-link" data-target="#43a7ec2a-2d5a-44a3-b992-0280967ce2cd" data-toggle="tab" href="#43a7ec2a-2d5a-44a3-b992-0280967ce2cd" id="80918368-6835-4d8f-a49f-1be9c454212f" role="tab">
       OutlineMixin
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#e3098ed6-7267-40d8-b65b-d8cba86578e7" data-toggle="tab" href="#e3098ed6-7267-40d8-b65b-d8cba86578e7" id="95b4d078-c42c-4cac-a6c7-b6e78b60bc19" role="tab">
+     <a class="nav-link" data-target="#2cdf283d-396b-4edc-b575-a87ffcef7d86" data-toggle="tab" href="#2cdf283d-396b-4edc-b575-a87ffcef7d86" id="f61e4c8d-3d1e-49cf-b02c-4200d5a56bb1" role="tab">
       AvailabilityMixin
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#9b467775-d72a-4dbb-ba10-68aac76c2131" data-toggle="tab" href="#9b467775-d72a-4dbb-ba10-68aac76c2131" id="7cd027e8-2e42-40a9-b43d-83f2eae72c06" role="tab">
+     <a class="nav-link" data-target="#4ab49bce-83d3-40d0-8250-b4b63097fe19" data-toggle="tab" href="#4ab49bce-83d3-40d0-8250-b4b63097fe19" id="33a9f572-5511-4bf6-8fac-9c717f1266c1" role="tab">
       Constants
      </a>
     </li>
    </ul>
    <div class="tab-content">
-    <div class="tab-pane fade active show" id="5e6b8038-7ef2-4d66-9a04-03364ae02f63">
-     <div class="mt-5" id="c6476f20-7bf7-4c6f-8918-c5d27ed88fa4">
-      <div class="d-flex justify-content-between" id="0fbdfec4-512d-4b72-9a5b-0ed98f73c864">
-       <h1 id="7114a496-4761-4e23-b4d1-bfed4be9fb5c">
+    <div class="tab-pane fade active show" id="636c6d6f-38fe-40aa-83ea-8bf0a268a145">
+     <div class="mt-5" id="ab38a43c-5134-45f9-8420-923a337fb47f">
+      <div class="d-flex justify-content-between" id="2701fca5-2955-4c4f-bf4f-4a44adff4473">
+       <h1 id="7e6c4fa4-9963-44cf-aec7-8f7605cccb68">
         Class
-        <span class="text-primary" id="ffe703a4-5eff-4869-8fd6-4dc0466f34dc">
+        <span class="text-primary" id="7e05c1d4-4d5e-4482-b6d0-ce9733715e67">
          WebComponent
         </span>
        </h1>
-       <div id="4bda89bf-4147-48c7-9df1-9331ba856379">
+       <div id="9c101a48-7225-478a-a11a-4fb39641ad26">
        </div>
       </div>
-      <span class="text-muted" id="8a12d67b-34a8-4877-8fc3-f486bff258f9">
+      <span class="text-muted" id="94c09d58-0ad5-4b56-8e1a-65fb4fbae119">
        A web component base class.
       </span>
-      <pre id="0260e1fd-fd47-4dac-a5f2-0787a1bcdaba"><code class="python">WebComponent()</code></pre>
-      <p id="eabe9d01-cbb5-4683-8f18-e30c86eab1ed">
+      <pre id="8b9d27b3-d138-48d6-aeea-7011183aeb9b"><code class="python">WebComponent()</code></pre>
+      <p id="4c5f93ed-d89d-47ea-898c-14fe175d7efc">
        This class must be inherited by all web components.
       </p>
-      <p id="bb38c559-4630-40ed-9857-5cd168ec1402">
+      <p id="dc291a77-fd6b-498f-b208-72b85cfdb24e">
        In many operations where one web component encapsulates another one has
     implemented a type check. If the received element is not
        <code>
         WebComponent
        </code>
        will be generated a
        <code>
@@ -130,57 +130,58 @@
        . To ensure correct handling of your
     custom component, do not forget to inherit the
        <code>
         WebComponent
        </code>
        class.
       </p>
-      <div class="ml-3" id="0968884d-d2db-4df9-91b8-16c81a16d245">
-       <h6 id="fbd13bd7-acc8-4e6f-99f2-210d17809e2a">
+      <div class="ml-3" id="cc97852d-7dda-4da8-aba7-55cf98c34549">
+       <h6 id="83c0cea6-e043-47f0-8a7c-f1640cbc8a48">
         <strong>
          Example
         </strong>
        </h6>
-       <pre id="d3ffdc83-5825-4f81-8a0b-0e8ea543c31d"><code class="python">from bootwrap import WebComponent
+       <pre id="3694f0aa-0bdd-4d72-ac3d-8a16003b5096"><code class="python">from bootwrap import WebComponent
 
 class CustomHeader(WebComponent):
     def __init__(self, title):
         self.__title = title
 
     sef __str__(self):
         return f'''
             &lt;h1 id="{self.identifier}"&gt;
                 {self.__title}
             &lt;/h1&gt;
-        '''</code></pre>
+        '''
+</code></pre>
       </div>
-      <div class="mt-5" id="1f2e8135-74ce-40a5-9731-9e23561036c7">
-       <h4 id="dc404e16-8244-4946-8e92-ead9fd835e52">
+      <div class="mt-5" id="50c383a4-281e-4928-825d-d96a66a6592f">
+       <h4 id="02d09e91-064a-4e7e-877e-f4ba6b5fa14c">
         Property
-        <span class="text-primary" id="d47bd64c-617f-43c8-95cd-f0bacaafff5c">
+        <span class="text-primary" id="e446fece-2444-46a0-9b76-7730389dc419">
          identifier
         </span>
        </h4>
-       <span class="text-muted" id="d163004a-3e20-46e4-8c04-037a07046872">
+       <span class="text-muted" id="2e4b7d26-7ba1-46fb-b88a-d141a8f046a5">
         A unique web component identifier.
        </span>
-       <p id="bd9e0864-4b2b-468f-8de8-42000749d676">
+       <p id="d841f85f-a594-4f55-b613-ec86f3077618">
         Every
         <code>
          WebComponent
         </code>
         has a unique identifier (ex. cfe040e6-df5f-4a3a-
         b96e-b0cefc31bbd9). This identifier is used for referencing between
         components inside a page. This property returns this identifier as
         <code>
          str
         </code>
         .
        </p>
-       <p id="bebd1c52-0c55-4ef1-b158-f10484af32a6">
+       <p id="58e62e68-de20-452d-b78f-f96b0bd20790">
         When you create a custom
         <code>
          WebComponent
         </code>
         it is advisable to set its
         tag attribute
         <code>
@@ -188,101 +189,103 @@
         </code>
         equals to
         <code>
          identifier
         </code>
         .
        </p>
-       <div class="ml-3" id="215362fb-b4d1-4ee0-a854-58ab6fc46df7">
-        <h6 id="fc97bd9d-49a3-4640-ae80-447e0567e3ef">
+       <div class="ml-3" id="7bb46561-b62f-4a4c-979d-d15817d11cef">
+        <h6 id="9d98517a-20db-4161-b6fc-e573446fd1b8">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="725b4f05-48a1-4f03-b212-ae4b6d121831"><code class="python">header = CustomHeader('Hello World")
+        <pre id="29d14189-6366-4dbf-9493-acf226dadb49"><code class="python">header = CustomHeader('Hello World")
 print(header.classes)
 
-# Result: cfe040e6-df5f-4a3a-b96e-b0cefc31bbd9</code></pre>
+# Result: cfe040e6-df5f-4a3a-b96e-b0cefc31bbd9
+</code></pre>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="cfc04d99-146e-4e09-8489-733ec6372458">
-     <div class="mt-5" id="b428fef3-8fc7-4b65-8475-8e4999b49e6f">
-      <div class="d-flex justify-content-between" id="968cb48b-b7f2-4534-b0a7-2e7e49af83f3">
-       <h1 id="16a595d7-dcd0-4036-b1bd-6f92b4445e14">
+    <div class="tab-pane fade" id="77d9fddf-decd-486e-bcf1-42f100a5a571">
+     <div class="mt-5" id="0304e4b0-a91f-4b64-9670-dccce90b32f9">
+      <div class="d-flex justify-content-between" id="e81cec18-1411-42b7-ae3d-45d4fc7fa5aa">
+       <h1 id="a37e20d1-1178-4cdd-8492-1911bda10821">
         Class
-        <span class="text-primary" id="0f2c8161-9fc5-4a7b-8dba-82f400b2c199">
+        <span class="text-primary" id="56ecac4d-bb1d-4402-b249-f9b52d836a3a">
          ClassMixin
         </span>
        </h1>
-       <div id="e2af7f42-9171-44b3-b0b2-9c45602868ce">
+       <div id="56e8bcbd-0018-4e00-b4bc-ef42d9049792">
        </div>
       </div>
-      <span class="text-muted" id="ec4e2506-26fb-4822-8ce3-66bca5996586">
+      <span class="text-muted" id="cb70642e-d90d-4772-bfb8-fff90fb27131">
        Mixin for a web component which class can be amended.
       </span>
-      <pre id="99b49298-f0df-4f98-a9c4-7484d115ca1d"><code class="python">ClassMixin()</code></pre>
-      <p id="3f7ec14f-d2b5-4bca-b224-d2242bcb3a56">
+      <pre id="c7d4694c-ad6c-4427-8db4-0769a30bd4fa"><code class="python">ClassMixin()</code></pre>
+      <p id="b2a3dd23-d969-4ad5-9bec-78d948dfa6d0">
        The vast majority of web components in Bootwrap inherit this class.
     It allows a user to adjust web components look and feel.
       </p>
-      <div class="mt-5" id="f7e34d77-81f7-4b2e-bae8-6e87fb8ab5c1">
-       <h4 id="bc1ac344-37d3-43a7-af4e-83aac36cabdc">
+      <div class="mt-5" id="bdfa8aba-56f1-41f5-b5c9-97ec2a12e964">
+       <h4 id="c7c61f6d-32ab-4ab6-92a7-e8b706a6e903">
         Property
-        <span class="text-primary" id="fee06b4e-5cbd-42b0-b54f-06dc0f4dac04">
+        <span class="text-primary" id="24291178-3778-4b46-b195-fa41934e7cc0">
          classes
         </span>
        </h4>
-       <span class="text-muted" id="3422375a-a006-4e45-91da-5e5d0bf40f5d">
+       <span class="text-muted" id="aaff917b-ff41-4957-85eb-ab7c717083d6">
         The web component classes.
        </span>
-       <div class="ml-3" id="67b64b76-c076-4958-a05e-5da3446982c3">
-        <h6 id="85309382-8a97-4c7b-b43c-b500474d3ff8">
+       <div class="ml-3" id="053cd65d-b04f-4609-bf83-be45e6437b7c">
+        <h6 id="0abbc725-2bb2-497d-b181-3a34836f39aa">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="6b5d75a3-3d29-4f83-bd39-84471823cb62"><code class="python">from bootwrap import Button
+        <pre id="0803d017-da3c-4c59-9d1a-da1f5ae53681"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ClassMixin.
 button = Button("Hello").add_classes("ml-1 mr-1")
 print(button.classes)
 
-# Result: ml-1 mr-1</code></pre>
+# Result: ml-1 mr-1
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="8ac77d57-0a4d-44cf-9676-04dac8760d7b">
-       <div class="d-flex justify-content-between" id="28d279bd-7283-487f-8373-1563c52e2eb0">
-        <h4 id="2591e643-5591-4d5e-963e-7056f9a97102">
+      <div class="mt-5" id="67082edd-0c18-4a0c-9a66-2f40541887ee">
+       <div class="d-flex justify-content-between" id="dfbbbca1-31a0-420a-a97d-3969cfd1b78c">
+        <h4 id="a40dd876-a0c5-464f-877f-cdd09d9a01b3">
          Method
-         <span class="text-primary" id="9eee01fb-c897-4553-a76a-9a636818d6ab">
+         <span class="text-primary" id="581a348b-6f01-4505-9c46-2fc965430893">
           add_classes
          </span>
         </h4>
-        <div id="3067d16e-f6a6-4ace-8d4f-3a2ac16604a9">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#f76a69ee-610e-4c2d-b163-96c88f5851ef" data-toggle="collapse" id="6c8b7755-7c51-4231-b18c-ace22cdf2bf8" onclick="return false;" type="button">
+        <div id="0fd93f58-0bb9-4465-9385-abe8f6897379">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#24b275a9-baf9-41cf-b9b4-0345f143428b" data-toggle="collapse" id="07ce2041-8255-45e4-a26e-c7e05b83893c" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#a4909c12-2bf4-4f46-bd0c-fe95fd2751b0" data-toggle="collapse" id="dd1bad44-fe33-4598-8704-1f5fa2ab40dd" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#659ff989-523a-44b7-b84e-d2b8c3161a15" data-toggle="collapse" id="d48a7b29-4c88-4898-9e5d-3e11bc87c5de" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="1e98d8af-7a07-4183-a841-e3c8194434a2">
+       <span class="text-muted" id="774f831b-8f80-4be1-bc60-5cdbff920655">
         Adds other classes.
        </span>
-       <pre id="8f133d97-dc58-4381-8762-5184d18ab385"><code class="python">add_classes(classes)</code></pre>
-       <div class="ml-3 collapse" id="f76a69ee-610e-4c2d-b163-96c88f5851ef">
-        <h6 id="0cd22760-1d9d-4af7-9978-94f419fb4d60">
+       <pre id="9e6e7fcc-756a-43ce-b857-5c7e84901d4c"><code class="python">add_classes(classes)</code></pre>
+       <div class="ml-3 collapse" id="24b275a9-baf9-41cf-b9b4-0345f143428b">
+        <h6 id="29cf75b8-df7e-46ce-94d5-aa7c01460d9d">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="8c64cf56-7da9-4a80-9724-d9465edb7d75">
+        <table class="table table-sm bg-light" id="98b15111-51cf-4cf0-87be-e479d2cd5bdc">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -308,21 +311,21 @@
             The classes to add. The specified classes must be
                 separated by white space.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="a4909c12-2bf4-4f46-bd0c-fe95fd2751b0">
-        <h6 id="26576c39-e587-4bc9-b8d4-d14e5c7b1545">
+       <div class="ml-3 collapse" id="659ff989-523a-44b7-b84e-d2b8c3161a15">
+        <h6 id="3aff5748-3d77-4eb6-b69a-da5eea06bba7">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="39a95cf0-4c4a-4157-bcdd-b16618a49951">
+        <table class="table table-sm bg-light" id="b20ab06f-fc62-4a25-b847-9b110d73998e">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -347,58 +350,59 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <p id="29cbbce5-c3d2-4ee1-a319-4b33517f6aa5">
+       <p id="c2beb978-ce16-4950-974f-2c302b5332cf">
         Note, the order of specified classes will be preserved during the
         component rendering.
        </p>
-       <div class="ml-3" id="378a9029-5140-4189-bcd8-f0a1883beba4">
-        <h6 id="8b3955aa-ef7d-4b7b-b45f-4071550ccfaa">
+       <div class="ml-3" id="6e4faf0e-8076-47b2-9ada-dee2c7ef1c39">
+        <h6 id="0e2ee076-c501-48a1-8594-674aca6cf17e">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="63b99bd1-802e-4307-8e5a-edee83e79e7e"><code class="python">from bootwrap import Button
+        <pre id="b9b48eef-9d39-4c45-a7c8-b3547f726082"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ClassMixin.
-button = Button("Hello").add_classes("ml-1 mr-1")</code></pre>
+button = Button("Hello").add_classes("ml-1 mr-1")
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="185879bc-e655-4334-815b-574de3f44f6b">
-       <div class="d-flex justify-content-between" id="b0c64f43-1e90-4273-ad1b-da2f97aa7e8e">
-        <h4 id="3df58ada-425e-44d5-9263-f4a3c3062bcb">
+      <div class="mt-5" id="0923ac6d-b121-4721-bac9-febcd4e6f735">
+       <div class="d-flex justify-content-between" id="d06c728f-1aa4-46e6-9504-d08821b7470d">
+        <h4 id="0956a9f3-0c18-4ff1-b815-b63b0a3d5baf">
          Method
-         <span class="text-primary" id="8a7473a8-7b7c-4400-8e53-1a189f833044">
+         <span class="text-primary" id="690f927f-a2d5-4055-9eff-5a17439e3954">
           m
          </span>
         </h4>
-        <div id="c9c1e583-1ea6-40e7-a131-aa415486435a">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#906f9011-aed4-4012-8427-e52856cf50e7" data-toggle="collapse" id="5d3eaec1-b8fe-4480-b28e-75e2776dfee3" onclick="return false;" type="button">
+        <div id="e8af54d3-f2e2-4523-9563-c956a0b542bd">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#fa8448d7-97be-435e-ae16-a7c3f1f27e77" data-toggle="collapse" id="43ffbe73-1217-4245-b377-381475321afc" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#f9eddeb7-7317-4571-8254-1f0e712645d8" data-toggle="collapse" id="e7e55da6-64ed-4289-a22d-e6f060106729" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#2d9161b2-501c-4920-8feb-f34bd4f7629a" data-toggle="collapse" id="b1b98bbc-8c5a-40be-a46d-2ab7c6a20017" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="9d398064-16fe-4eb9-b687-1833faf1c510">
+       <span class="text-muted" id="02ee1800-0d57-4135-8e38-a79ef45f8e15">
         Sets margin for all four sides to the specified size.
        </span>
-       <pre id="a9514630-b521-494a-9749-8a446c418560"><code class="python">m(size)</code></pre>
-       <div class="ml-3 collapse" id="906f9011-aed4-4012-8427-e52856cf50e7">
-        <h6 id="ba7bef43-934a-4636-ac66-dc9e978b7f7f">
+       <pre id="bf8a1f71-6986-4772-98e0-386d66355a09"><code class="python">m(size)</code></pre>
+       <div class="ml-3 collapse" id="fa8448d7-97be-435e-ae16-a7c3f1f27e77">
+        <h6 id="fd689e47-dfb0-4edb-95d4-dd8a8bf616ba">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="5d369eec-1957-49a6-9efe-aa04e33ea77c">
+        <table class="table table-sm bg-light" id="40e08038-2f98-47cb-a0e3-6366c2cd8cca">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -423,21 +427,21 @@
            <td>
             Size of the margin to set.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="f9eddeb7-7317-4571-8254-1f0e712645d8">
-        <h6 id="06e1cf7a-72d4-4fe8-82ac-ccd856c6df6e">
+       <div class="ml-3 collapse" id="2d9161b2-501c-4920-8feb-f34bd4f7629a">
+        <h6 id="a9199b45-c6ac-49c3-bf33-61d94e3dae3d">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="e21aa887-71fc-4306-8eb4-265a46a5f472">
+        <table class="table table-sm bg-light" id="5d4960d2-047e-4945-8b53-71558171b953">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -462,54 +466,55 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="180e754e-0de7-4309-91ff-be1ea4c12b61">
-        <h6 id="24b1ae55-4cc4-4230-bfdc-7c5dac443075">
+       <div class="ml-3" id="ea49bff7-6762-40d6-abcd-2fbe003a0720">
+        <h6 id="62d11f0c-b5e7-4acc-8bf8-87351829dee9">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="2559177b-218f-449d-92e0-29b7e8456645"><code class="python">from bootwrap import Button
+        <pre id="def2b28a-e781-4e9a-91b7-47ac422e3d81"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ClassMixin.
-button = Button("Hello").m(3)</code></pre>
+button = Button("Hello").m(3)
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="4490f16c-7b5d-496b-b341-a9c12911f3bd">
-       <div class="d-flex justify-content-between" id="1f19e1ce-9fb3-4467-ad24-7e0d55549614">
-        <h4 id="32fc6d65-c397-4170-944b-f50412786088">
+      <div class="mt-5" id="6f0baeb1-db7c-4887-8c2a-f3db74e53b70">
+       <div class="d-flex justify-content-between" id="814d4193-5d8c-4106-a4e4-1572e580a232">
+        <h4 id="9598cb96-8adf-49f8-b012-17e45cfb3b65">
          Method
-         <span class="text-primary" id="8e6ab89f-fa45-4e0f-a69b-431e3195b32f">
+         <span class="text-primary" id="bc952218-f080-40b9-b927-ab644ef8e505">
           mb
          </span>
         </h4>
-        <div id="ad9aeb09-1a07-40b1-ac0d-54e69d3004cd">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#a70a0a90-9a2b-49e8-9df7-442bb7d67081" data-toggle="collapse" id="a6a9a9ff-be40-4c99-87ee-c1b40045e1fe" onclick="return false;" type="button">
+        <div id="d33703e9-39e8-44ff-bb76-39ca536b24ee">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#fd865e77-9f67-4f22-8bb7-372449b7e720" data-toggle="collapse" id="877d832b-876b-464a-a04a-3dd16e32eb0f" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#f3c764a4-d175-44c4-9db2-6dbcc2c2371f" data-toggle="collapse" id="6d0cd45e-5281-48ce-9704-80450a530b0f" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#73f7fabc-733d-4f41-9d8d-46d3083c597e" data-toggle="collapse" id="422f79b6-d80e-49c3-94f2-2756ac2c84f0" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="50f508fb-ecaa-40f3-b084-34018d5b137a">
+       <span class="text-muted" id="8af2292e-06df-4aa4-94bd-dd2186e4b761">
         Sets margin for the bottom side the specified size.
        </span>
-       <pre id="e37d8c23-2fc4-4670-be23-b86369b374ef"><code class="python">mb(size)</code></pre>
-       <div class="ml-3 collapse" id="a70a0a90-9a2b-49e8-9df7-442bb7d67081">
-        <h6 id="7862b679-d01a-4b9e-ab9d-a6daeafa3f7c">
+       <pre id="b75bfa82-d5a4-4a6d-889c-e747142d54c4"><code class="python">mb(size)</code></pre>
+       <div class="ml-3 collapse" id="fd865e77-9f67-4f22-8bb7-372449b7e720">
+        <h6 id="740e010f-c388-4da5-a686-c94b24459d5d">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="1f7244e7-eda7-4a08-8dd8-37c19a8d8b87">
+        <table class="table table-sm bg-light" id="6e49e74f-1003-44db-9cdd-a133a1fba71b">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -534,21 +539,21 @@
            <td>
             Size of the margin to set.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="f3c764a4-d175-44c4-9db2-6dbcc2c2371f">
-        <h6 id="31fc4994-4ba7-4bd5-ad18-c3b2c527b1fc">
+       <div class="ml-3 collapse" id="73f7fabc-733d-4f41-9d8d-46d3083c597e">
+        <h6 id="1b2f8272-e295-4a31-838d-5132579fe5c5">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="f188a813-815c-43d5-879a-adfdb5d65ddf">
+        <table class="table table-sm bg-light" id="6a13f7bd-3784-4700-a303-cdcd51aa196e">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -573,54 +578,55 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="30e116e5-a910-42de-af51-6dba6cc32eba">
-        <h6 id="22046b6e-321a-463b-9f44-7efd84cef741">
+       <div class="ml-3" id="d38253d3-b698-4bb3-bc30-20ab8807f35d">
+        <h6 id="50cf2630-d637-4076-b169-8a74c598597f">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="6e6b9303-861b-4c82-90a7-e7986e67d766"><code class="python">from bootwrap import Button
+        <pre id="1af7038f-2587-419f-a295-a3bd901b2b3d"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ClassMixin.
-button = Button("Hello").mb(3)</code></pre>
+button = Button("Hello").mb(3)
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="cc0a138a-3718-4424-b204-d2321bfa8e31">
-       <div class="d-flex justify-content-between" id="ae742145-7e2d-4dc4-b57e-852f0480e13c">
-        <h4 id="05c17efd-928c-4b87-96ad-fc1b3c57e218">
+      <div class="mt-5" id="16050ca4-75a1-4fbe-8692-487c616b0de2">
+       <div class="d-flex justify-content-between" id="bbdaae93-2619-43ce-9c96-7eaa49dc172e">
+        <h4 id="881bc3ee-e923-4aec-b228-0a39edb26258">
          Method
-         <span class="text-primary" id="c75356f6-2dfb-4683-8ba1-095e0a7659b9">
+         <span class="text-primary" id="417b693f-2d5f-49fd-897a-2692ff38ca0b">
           ml
          </span>
         </h4>
-        <div id="7ddbf0c0-6f01-4de3-a6db-fdd94a811274">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#48313334-a1a0-4096-afa0-4b5c05ca5bf6" data-toggle="collapse" id="f71cfdef-7ed4-477e-8d5f-d149dac028b6" onclick="return false;" type="button">
+        <div id="4bbdfa55-595b-49bd-8e26-7908d5646954">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#2efa248b-31c6-4469-9ff2-40f54efe7570" data-toggle="collapse" id="529a8759-fb94-414d-ac01-772631274597" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#9a627d44-7864-43ce-8412-ceafcc4012e1" data-toggle="collapse" id="acdfc0c9-c70e-4c6f-8ace-c5f1266a9053" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#954ebade-06ac-410c-b568-e503d697555c" data-toggle="collapse" id="7aaff4c2-0c47-47ef-8e8e-3f182204ccd2" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="1be7548c-b245-446d-922f-658fdc4f5f05">
+       <span class="text-muted" id="0c24b65e-2fcf-425d-9e61-c7e756ed3066">
         Sets margin for the left side to the specified size.
        </span>
-       <pre id="2c7a2117-b03f-4acd-8fa9-41af616b10d5"><code class="python">ml(size)</code></pre>
-       <div class="ml-3 collapse" id="48313334-a1a0-4096-afa0-4b5c05ca5bf6">
-        <h6 id="9a2f110a-37b5-422b-95a4-dee58d319590">
+       <pre id="ddf39660-5ddd-474c-b077-a2f1d951ce60"><code class="python">ml(size)</code></pre>
+       <div class="ml-3 collapse" id="2efa248b-31c6-4469-9ff2-40f54efe7570">
+        <h6 id="106c6ea6-e221-4026-aecd-fc4e2c6d0da4">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="5c813024-b79c-47ed-acc6-16beb01f173c">
+        <table class="table table-sm bg-light" id="9cdd1d27-95b6-47d8-b302-e30ae7ca5072">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -645,21 +651,21 @@
            <td>
             Size of the margin to set.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="9a627d44-7864-43ce-8412-ceafcc4012e1">
-        <h6 id="7c3a3fcc-89f4-450f-8a16-6a511b3e5a15">
+       <div class="ml-3 collapse" id="954ebade-06ac-410c-b568-e503d697555c">
+        <h6 id="e4d44e18-238b-42f4-8ce4-11b09669ac94">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="0af09694-be6a-4c2d-a72a-375a992fbabb">
+        <table class="table table-sm bg-light" id="dea4d261-afbb-4342-8241-5d05d380ae0e">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -684,54 +690,55 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="f0e8c191-c6b1-4145-83dc-442bb99a69b4">
-        <h6 id="27849212-cf0a-49cc-8289-1d2cdaa64b2a">
+       <div class="ml-3" id="61dce341-d661-4bc2-a173-658c6889a1c2">
+        <h6 id="5175b3ec-dfee-4554-98f2-ce843bfa7726">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="2d9998c6-5ef4-42d5-8d37-9554c326a531"><code class="python">from bootwrap import Button
+        <pre id="a5defe14-9dd7-4553-8e78-45635f10d97f"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ClassMixin.
-button = Button("Hello").ml(3)</code></pre>
+button = Button("Hello").ml(3)
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="f5f72437-f5ef-48ee-94c9-d4c00975bb50">
-       <div class="d-flex justify-content-between" id="4cd637b8-78c6-4e22-bd78-3c3857480d26">
-        <h4 id="eefcf00b-fa6f-49ff-8674-0c2d51a88fee">
+      <div class="mt-5" id="0e614d24-64dc-4025-b9ec-cf2ac3827d37">
+       <div class="d-flex justify-content-between" id="bb372b70-7866-418b-a239-000255f25abf">
+        <h4 id="6d0a4ec0-018e-4b65-bbed-18d1c0532b75">
          Method
-         <span class="text-primary" id="6cfc1dc4-726d-47f8-a225-79d0b37dbf21">
+         <span class="text-primary" id="edf49a37-b440-4915-a499-1bd54ffb30cf">
           mr
          </span>
         </h4>
-        <div id="9212c3ef-2730-48ee-9c4d-015aaa73d93b">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#1b3a1e86-04d2-45b4-8549-debc22ca7e64" data-toggle="collapse" id="f4f34bfe-32f7-42c9-9a7d-6f7e62bd9de7" onclick="return false;" type="button">
+        <div id="dd233958-c40f-4511-9d1c-35694e7be4f4">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#4badfbd5-9942-4d29-8fd4-3715c61d6308" data-toggle="collapse" id="0f888167-9f6b-4f02-94ad-bf1ff5f2aa76" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#0ff953d3-0c0d-46c1-aa83-fb5df5aeff21" data-toggle="collapse" id="cb2a84d9-8501-4e26-b2c5-0620dfe45e19" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#b30558d9-4459-4fe1-b61c-fa117f690065" data-toggle="collapse" id="eafa88e9-c96b-4199-badb-de2fac08a7e0" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="2f684aab-3d58-41a7-b1b5-7913fa6b6279">
+       <span class="text-muted" id="d0df0324-039a-4966-b616-66b9f22ca3c5">
         Sets margin for the right side to the specified size.
        </span>
-       <pre id="e2290026-6d04-42d8-8e6b-5f9467f48b57"><code class="python">mr(size)</code></pre>
-       <div class="ml-3 collapse" id="1b3a1e86-04d2-45b4-8549-debc22ca7e64">
-        <h6 id="0f9d74bf-8dd1-4914-ba9f-229d43399e64">
+       <pre id="95f2ba2c-12ef-49cf-bdb4-c072fcb2b49d"><code class="python">mr(size)</code></pre>
+       <div class="ml-3 collapse" id="4badfbd5-9942-4d29-8fd4-3715c61d6308">
+        <h6 id="0878b836-5d7d-44fc-b5f2-dddca19d3247">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="198d494d-6fba-44df-9ba3-4f42191a2a6c">
+        <table class="table table-sm bg-light" id="bba1f268-338e-40ae-a7e7-3c4b5e1ae7fd">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -756,21 +763,21 @@
            <td>
             Size of the margin to set.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="0ff953d3-0c0d-46c1-aa83-fb5df5aeff21">
-        <h6 id="c9cadf8b-fe9e-4187-99c4-c7fcbdd14c61">
+       <div class="ml-3 collapse" id="b30558d9-4459-4fe1-b61c-fa117f690065">
+        <h6 id="c33bb946-b43f-44fe-b3d1-9a8ef86681ac">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="6778d1f2-9ae3-4153-bdbe-7c86f4381136">
+        <table class="table table-sm bg-light" id="98a24883-bc33-4316-ac44-8de69381d049">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -795,54 +802,55 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="c48c546a-b1a7-4c72-9edd-99017e192bae">
-        <h6 id="266eb0f2-208e-4241-8ef9-47772244be17">
+       <div class="ml-3" id="0c1ccad9-10e0-42af-a829-85d1575f5a1e">
+        <h6 id="f972011c-24d2-4510-bde8-ff1557d74742">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="3585b949-1f60-40b5-8c4b-67030561f89d"><code class="python">from bootwrap import Button
+        <pre id="c02732bf-5678-44e0-a3b0-0a02a3a537e2"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ClassMixin.
-button = Button("Hello").mr(3)</code></pre>
+button = Button("Hello").mr(3)
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="b7a88ab2-93aa-401a-b63d-9457c159e264">
-       <div class="d-flex justify-content-between" id="4c3fe6eb-cca5-4be5-890c-371d5d9fc0ca">
-        <h4 id="e1845294-b9f9-4ab7-8c3a-fd4d18560f1f">
+      <div class="mt-5" id="8f479a31-d3a4-40ca-b05a-0d1915f75716">
+       <div class="d-flex justify-content-between" id="c0cadbae-224d-420d-8e69-87cdac4c51d5">
+        <h4 id="cb2e5e91-42d6-4492-9f52-e638aed02a2b">
          Method
-         <span class="text-primary" id="b63f3d4f-868f-4e2c-995d-b37d79482b6f">
+         <span class="text-primary" id="048af173-f2c2-4c57-9b1c-9a15460b972a">
           mt
          </span>
         </h4>
-        <div id="3482cfbe-e3cc-4e1f-99e6-8cd401a87335">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#88e96553-f842-4e3b-b2f2-1c0097b82d0b" data-toggle="collapse" id="69823fe0-29ac-407e-8261-31b8df6f20cd" onclick="return false;" type="button">
+        <div id="d030579b-a61a-41ba-a6e0-f0b85c695cf4">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#a02bbf58-eaa7-4e5b-a890-292c9d371734" data-toggle="collapse" id="eb70da1e-870d-4445-a639-adf3965b1cf3" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#fce7480a-76dc-4b70-86de-cb90d95ffc60" data-toggle="collapse" id="0eaf6250-54d2-4b2f-b349-73826615976d" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#732c6672-641c-4724-9c49-39d94e91fc59" data-toggle="collapse" id="386269ee-61e0-4fd7-b42f-899fcf74d47b" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="e38b7ffe-3b07-4973-aa16-e845dc59b48d">
+       <span class="text-muted" id="c29e096e-fc34-46ec-8d7d-00f20ee2651e">
         Sets margin for the top side to the specified size.
        </span>
-       <pre id="fc86a9e3-0a77-4e35-adab-94415ec6ded2"><code class="python">mt(size)</code></pre>
-       <div class="ml-3 collapse" id="88e96553-f842-4e3b-b2f2-1c0097b82d0b">
-        <h6 id="beaa02f3-1828-4bb1-8c8b-e5406919bf9b">
+       <pre id="e02de7cc-d7fe-4877-98fb-cc63ae79208b"><code class="python">mt(size)</code></pre>
+       <div class="ml-3 collapse" id="a02bbf58-eaa7-4e5b-a890-292c9d371734">
+        <h6 id="79ca5888-e5a4-4485-b32f-d2b52932f317">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="a4e54ae9-d2fe-4cc6-a15e-a376d1870484">
+        <table class="table table-sm bg-light" id="1b6e721d-8adb-440b-9434-c8faddb28ca9">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -867,21 +875,21 @@
            <td>
             Size of the margin to set.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="fce7480a-76dc-4b70-86de-cb90d95ffc60">
-        <h6 id="2c23bfcf-c957-4163-8b8d-c42568db1acb">
+       <div class="ml-3 collapse" id="732c6672-641c-4724-9c49-39d94e91fc59">
+        <h6 id="5bb1e4a2-c242-4ab0-9e61-2bae73066c48">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="c18cfb7a-f44d-4e9d-a30a-f3b07fab24eb">
+        <table class="table table-sm bg-light" id="a6155e85-8eb9-4872-b860-7dab7dffc66a">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -906,54 +914,55 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="63da9237-e68f-49e8-b93e-ab812f7ce07d">
-        <h6 id="1f9e65b8-64d9-4d19-9252-679ba5a02b29">
+       <div class="ml-3" id="c53e4ea8-02fd-4f6d-9846-8c939600e7a3">
+        <h6 id="cdcae650-cf8c-4aeb-b985-d5a26cf96c98">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="74efec85-66de-411b-854f-880bc4aac27f"><code class="python">from bootwrap import Button
+        <pre id="6c32c392-65b2-4232-bb19-b784867498a2"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ClassMixin.
-button = Button("Hello").mt(3)</code></pre>
+button = Button("Hello").mt(3)
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="b4a2e1b7-56c9-4a3a-b3ca-c23de80c8142">
-       <div class="d-flex justify-content-between" id="d48a6535-d09a-4e06-a523-b01dc39bb003">
-        <h4 id="9db52395-df26-441b-9aa0-f131ee8b1247">
+      <div class="mt-5" id="fb16b443-d697-48fd-a480-6c4600ae04bc">
+       <div class="d-flex justify-content-between" id="3c422223-3c9d-45ed-9444-b85d727f5732">
+        <h4 id="227fa24a-3926-4bc4-8254-f8c527556729">
          Method
-         <span class="text-primary" id="9e2ac670-e7d4-47d0-84e7-33481ece759f">
+         <span class="text-primary" id="c60ad82e-2dbf-4a6a-923d-2cdc1680a297">
           mx
          </span>
         </h4>
-        <div id="9436da2b-086f-446a-8aa1-83f49b1702da">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#8d874d2a-ccc3-45b5-aedd-348ac9aa0f27" data-toggle="collapse" id="f2bbbfec-80b6-4b79-8340-8c60f53a6f50" onclick="return false;" type="button">
+        <div id="8d692c3d-61b8-4a01-a99a-2e686c650cf5">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#7083521f-97df-43d5-a225-3d9134266113" data-toggle="collapse" id="9d75ed1e-dcd1-4766-8b12-e88afd204226" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#1ef7342a-30c2-4139-8ad3-93bd7e5a6631" data-toggle="collapse" id="38ef7263-3ba5-4804-98b8-2a08dbce03bd" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#01b2adbe-b0e2-45f7-99e1-c3ed1271de20" data-toggle="collapse" id="e7b5952a-b9b4-4b3d-8a42-842f2f236169" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="f42b2e6f-e0eb-4189-924e-cda251f3d496">
+       <span class="text-muted" id="c93c02bb-3fef-462d-ad6f-4311e34fc126">
         Sets margin for left and right sides to the specified size.
        </span>
-       <pre id="faf15ebc-f368-4068-913b-a86c3cec2e26"><code class="python">mx(size)</code></pre>
-       <div class="ml-3 collapse" id="8d874d2a-ccc3-45b5-aedd-348ac9aa0f27">
-        <h6 id="f450cada-18ae-4241-ab88-ebd6e03417b7">
+       <pre id="d78a57b5-9960-4e4b-920e-cbec87508b0a"><code class="python">mx(size)</code></pre>
+       <div class="ml-3 collapse" id="7083521f-97df-43d5-a225-3d9134266113">
+        <h6 id="1335c46e-ba9a-436e-9f5a-95dc511b01a0">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="648de50b-c1b3-4805-8235-3a697169bf9d">
+        <table class="table table-sm bg-light" id="c3c29ed3-15b5-436c-b83e-e672d321d522">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -978,21 +987,21 @@
            <td>
             Size of the margin to set.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="1ef7342a-30c2-4139-8ad3-93bd7e5a6631">
-        <h6 id="87ae1b30-297c-4555-880c-003eb58dcc69">
+       <div class="ml-3 collapse" id="01b2adbe-b0e2-45f7-99e1-c3ed1271de20">
+        <h6 id="c7e79164-7520-4c30-aec1-2a6d851c0170">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="9718702a-fead-4543-b37d-8aeb19d73eb9">
+        <table class="table table-sm bg-light" id="5bf054c9-eef6-43dd-b168-0299b395d1d6">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1017,54 +1026,55 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="e45f3ee4-49eb-4b96-a57f-52062728d029">
-        <h6 id="659c98b4-e710-4ce6-9afc-0bcc41b76922">
+       <div class="ml-3" id="7399bfcf-d31b-43fb-a94f-f9c877644f36">
+        <h6 id="d99ac68a-6580-45b6-b007-93001c72f1ee">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="a66fc788-6db2-4692-8327-af64bfc6b3ff"><code class="python">from bootwrap import Button
+        <pre id="35974658-c2e2-4bac-a2a9-918e85cee3d8"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ClassMixin.
-button = Button("Hello").mx(3)</code></pre>
+button = Button("Hello").mx(3)
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="ecde43bd-195f-44fc-b780-1d06daef9e62">
-       <div class="d-flex justify-content-between" id="207ecf83-ae47-4075-9010-42ca7602184f">
-        <h4 id="c91eda25-f004-42a5-b023-f37ea9c7a86b">
+      <div class="mt-5" id="b2c5bd33-4fe1-4058-87bf-4f0925f481c3">
+       <div class="d-flex justify-content-between" id="6a73f2a9-f45f-497c-a9a8-9a3c16fe5b95">
+        <h4 id="3e61d24e-5b03-4f55-af00-aa11add15cee">
          Method
-         <span class="text-primary" id="25aef4c8-c9e2-4934-9fd9-b4eec0ac7398">
+         <span class="text-primary" id="d796f731-7e1e-4514-85ac-a092fa1dbd61">
           my
          </span>
         </h4>
-        <div id="20da1ce5-4d6e-44e1-857f-77aacf5a9766">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#6a315069-d080-48a7-afec-b0aa69eba44c" data-toggle="collapse" id="3ac6a0e2-42fd-4b34-806b-a50a378f6cc1" onclick="return false;" type="button">
+        <div id="22eb3189-b3ab-499f-bbf0-a123bfbb7bd2">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#dfa71a8e-9638-4a26-9df2-da5395701b89" data-toggle="collapse" id="af7950ff-e181-4097-aad0-ef6288b80ea8" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#9c2a79c6-fdbb-4f6a-8ef2-39133e2f4a1c" data-toggle="collapse" id="a9b0181b-4c76-45dc-baa9-d1724505aec3" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#13d39afb-f914-4fd3-808c-94ddef6a3a9c" data-toggle="collapse" id="ff223695-4a82-44b4-9b71-38683af1486f" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="fe945f1b-b0ba-42a2-a315-4ecd06e4cf2e">
+       <span class="text-muted" id="5638127e-e841-4a7a-a7a6-bccc3241f58e">
         Sets margin for top and bottom sides to the specified size.
        </span>
-       <pre id="02b9d086-a1db-4278-a118-d83b17d4d143"><code class="python">my(size)</code></pre>
-       <div class="ml-3 collapse" id="6a315069-d080-48a7-afec-b0aa69eba44c">
-        <h6 id="2b1abea9-143d-4c17-825b-0775851e1b47">
+       <pre id="fb64f43f-e1bd-4e0a-ad4b-a89b89ab321b"><code class="python">my(size)</code></pre>
+       <div class="ml-3 collapse" id="dfa71a8e-9638-4a26-9df2-da5395701b89">
+        <h6 id="4d9dbd3c-824c-4cac-86e3-3b11b57ab078">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="95b691d5-9c8f-4739-8e4b-587aabc3a5f3">
+        <table class="table table-sm bg-light" id="6c83d438-5fcb-4f0c-b89d-546fdb083dd7">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1089,21 +1099,21 @@
            <td>
             Size of the margin to set.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="9c2a79c6-fdbb-4f6a-8ef2-39133e2f4a1c">
-        <h6 id="7017265d-815b-4f32-9218-c694a4f45d0c">
+       <div class="ml-3 collapse" id="13d39afb-f914-4fd3-808c-94ddef6a3a9c">
+        <h6 id="0e4cfa9e-d352-4a41-84f8-056a6735219b">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="6bf31aa9-0f79-4586-a124-09c983e8c231">
+        <table class="table table-sm bg-light" id="f489242b-812a-459b-93c6-5524ab6c8037">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1128,54 +1138,55 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="636eb370-1af0-4f48-97c7-b018498307ea">
-        <h6 id="b36cb017-8ab3-4a21-92b9-f08f66a1ae5e">
+       <div class="ml-3" id="c8c17768-1dce-4901-827f-a7ef5709fab9">
+        <h6 id="e3cc19d0-3270-4cb7-8e20-544f729cbdf0">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="3b8e1ffc-6e6c-4c90-a260-fbe8d466af2e"><code class="python">from bootwrap import Button
+        <pre id="16f915d4-b382-46a4-afb8-305e5ac5fa9e"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ClassMixin.
-button = Button("Hello").my(3)</code></pre>
+button = Button("Hello").my(3)
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="7101050b-e151-4203-b030-c9664ef34c7b">
-       <div class="d-flex justify-content-between" id="f98cd368-58f5-4b43-b785-3a33dcedac73">
-        <h4 id="876609a8-84b4-477d-b3ed-0391ebc4180f">
+      <div class="mt-5" id="027cc2b3-d03b-46c7-9da0-937a2f995ec6">
+       <div class="d-flex justify-content-between" id="c79a8961-a509-44fb-8de3-6562892ec9a4">
+        <h4 id="123e141e-419d-45e3-9835-66a59671fa2b">
          Method
-         <span class="text-primary" id="9b56deb9-aba9-40da-ba11-69619ecdf6a0">
+         <span class="text-primary" id="60b8e0c4-d66d-4033-9884-e70cc83a274a">
           p
          </span>
         </h4>
-        <div id="cb503f95-232e-4c97-90a2-3850c781c8c8">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#68175a8d-5350-4f90-b284-b494d33be266" data-toggle="collapse" id="982be451-f4ec-43f9-9fd6-8a501d29f81a" onclick="return false;" type="button">
+        <div id="94fe0e37-4b5c-4192-aaa9-88a2b55addc8">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#aee25709-5c02-4bdd-bbb8-7b1b10ddc38f" data-toggle="collapse" id="8cf0278d-8af3-441a-acbb-dbb4943f87a8" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#77ce85b6-d609-4f99-9a92-61764891715c" data-toggle="collapse" id="a3209f52-f18b-48d0-b056-fef701df611d" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#47ebcc05-4e46-4afa-b9e6-3d5521328ce3" data-toggle="collapse" id="1b34e135-52de-4a5c-8ecc-a28a31c66bf1" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="0662f2c7-7236-4000-9335-1d5006c84bf8">
+       <span class="text-muted" id="525bbfa5-f3d5-48d6-a39f-2c0afdc79f51">
         Sets padding for all four sides to the specified size.
        </span>
-       <pre id="ff039d79-f231-4654-871c-9273620acb9c"><code class="python">p(size)</code></pre>
-       <div class="ml-3 collapse" id="68175a8d-5350-4f90-b284-b494d33be266">
-        <h6 id="2234f1e5-2b54-41b6-b679-05148c498034">
+       <pre id="2357ed5d-73c2-4b24-a98d-553c13b48cf6"><code class="python">p(size)</code></pre>
+       <div class="ml-3 collapse" id="aee25709-5c02-4bdd-bbb8-7b1b10ddc38f">
+        <h6 id="3c50f69a-e9d1-4366-8de6-90a768ce5d32">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="329b4d4b-d827-4ac0-bef9-010848fe2310">
+        <table class="table table-sm bg-light" id="d69852b5-5214-425a-b25f-f036546825de">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1200,21 +1211,21 @@
            <td>
             Size of the padding to set.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="77ce85b6-d609-4f99-9a92-61764891715c">
-        <h6 id="cc812b33-9cbd-4cf6-af58-7c1f65ffefc3">
+       <div class="ml-3 collapse" id="47ebcc05-4e46-4afa-b9e6-3d5521328ce3">
+        <h6 id="5f0b967a-e035-4969-b829-458f60ca3954">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="eeb1ad7c-a1d8-48ed-8518-aa1f3a11e822">
+        <table class="table table-sm bg-light" id="df34d188-e038-4a6a-ac0b-c6c643cd6d25">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1239,54 +1250,55 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="4a66a705-a394-4db5-9505-8ffc1f6382ac">
-        <h6 id="bbcb086e-fdc1-4645-8c79-41c385ea1d66">
+       <div class="ml-3" id="948bd5dd-213c-4db6-bd8b-17fefddf2c9d">
+        <h6 id="f2c39563-bddd-4470-911b-343e155d5f26">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="7fca9bfa-4c35-4011-9606-d151820ecec1"><code class="python">from bootwrap import Button
+        <pre id="e55d857b-c387-4341-97b8-1f51e18653de"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ClassMixin.
-button = Button("Hello").p(3)</code></pre>
+button = Button("Hello").p(3)
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="b604b749-de10-4cf5-9125-dd1bd77777dc">
-       <div class="d-flex justify-content-between" id="4b24de9e-0136-4e6a-ad4c-e5ad901f3387">
-        <h4 id="8af6c3b4-8a41-4a51-96c0-9b2e157d3561">
+      <div class="mt-5" id="1e791590-4e18-4181-b77d-fdf951317ce5">
+       <div class="d-flex justify-content-between" id="c0a58236-b6bb-4adc-9a41-e88ce1da8c0c">
+        <h4 id="c00d8cfa-4f49-4713-9c54-568c03bc655e">
          Method
-         <span class="text-primary" id="ecca20b0-83e2-4bb4-8156-f40707117f68">
+         <span class="text-primary" id="7c8041ea-0dcb-4f83-9408-17c6353b9af8">
           pb
          </span>
         </h4>
-        <div id="f5f4a8a8-98e0-46d8-ae7f-f8273ff2611f">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#5e39f636-9e42-4fec-90db-eeb909e2793d" data-toggle="collapse" id="f834fd25-a9a8-4f62-8e5e-fb7f9561b4a9" onclick="return false;" type="button">
+        <div id="430116db-22e2-4d61-85f3-b97906a220d4">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#1f41db3b-38ab-4fd5-b4ae-cc482d439cc4" data-toggle="collapse" id="a9113874-5824-4072-8484-2275bc2cbeae" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#493233cd-1298-4844-ad21-0f141cbbb0b2" data-toggle="collapse" id="d54fd295-e6f8-4cc3-9b7a-0110b13d4ff2" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#6aa2761a-f0d7-4e72-ae05-57a7df67e170" data-toggle="collapse" id="d43b0622-24c0-4f4f-8106-67c4d0ec79ea" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="95f29154-14d8-480e-aedd-819d48e571da">
+       <span class="text-muted" id="1b02eaa6-3028-40b5-9a77-6c1a52a014e5">
         Sets padding for the bottom side the specified size.
        </span>
-       <pre id="c7f71fdf-07d5-4ee2-92a3-9cc2874ef76f"><code class="python">pb(size)</code></pre>
-       <div class="ml-3 collapse" id="5e39f636-9e42-4fec-90db-eeb909e2793d">
-        <h6 id="f38d40fb-37b4-47e9-b20a-4cf6768494f9">
+       <pre id="82238e1d-9ea8-4319-a9b7-a8fec517c1ba"><code class="python">pb(size)</code></pre>
+       <div class="ml-3 collapse" id="1f41db3b-38ab-4fd5-b4ae-cc482d439cc4">
+        <h6 id="9dc010fe-ee1a-4a57-9adf-cf5c43ab7538">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="f32684c8-91d8-4860-bdbe-66322faa629f">
+        <table class="table table-sm bg-light" id="0b8a3cbb-cb0a-453e-8df8-476bc8dd2655">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1311,21 +1323,21 @@
            <td>
             Size of the padding to set.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="493233cd-1298-4844-ad21-0f141cbbb0b2">
-        <h6 id="bdfb6b62-525f-47f6-87b5-bb5898f5794e">
+       <div class="ml-3 collapse" id="6aa2761a-f0d7-4e72-ae05-57a7df67e170">
+        <h6 id="74c22aea-8393-46ee-9b0a-28a6993f020a">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="206ee8c3-3405-4f3a-bc86-1c14defa961b">
+        <table class="table table-sm bg-light" id="042b4cd6-e8a2-4c5d-8a12-2ba660f1d1e2">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1350,54 +1362,55 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="c1424000-071c-4767-9c38-efee2463f146">
-        <h6 id="91b65204-5e37-4da2-9c8d-7b3f718b611f">
+       <div class="ml-3" id="88de1306-7f44-43a2-8ede-135d31f93d1c">
+        <h6 id="f91d3087-4ec9-4cf3-bb8c-e13e60f665cc">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="d99d34ec-c2da-4b82-8fb8-dea6b739d756"><code class="python">from bootwrap import Button
+        <pre id="32e770b0-7874-4a9e-a27a-a82366f07770"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ClassMixin.
-button = Button("Hello").pb(3)</code></pre>
+button = Button("Hello").pb(3)
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="27f30839-e470-45d4-a87d-937bdf9bb99e">
-       <div class="d-flex justify-content-between" id="94b3a47f-1068-49b2-bd6a-c6a7a679a8e1">
-        <h4 id="58db2037-5019-4ce5-8e7f-638d1cb87945">
+      <div class="mt-5" id="0a22e742-e581-45b2-9709-cb1804043e60">
+       <div class="d-flex justify-content-between" id="ced103be-6f23-4815-a8b6-88aef8750181">
+        <h4 id="c98b6de7-e5ca-4c4d-824a-197eedb4a915">
          Method
-         <span class="text-primary" id="39b13dac-a702-4a2d-b0d7-4c7643253f2d">
+         <span class="text-primary" id="5a120967-d307-4ce3-90c5-9bfe72805b96">
           pl
          </span>
         </h4>
-        <div id="a6f2e13c-b5eb-44c8-9d8f-3ef1347a896a">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#e3fbbc6c-e089-4f67-905e-175c3e7ac4d9" data-toggle="collapse" id="c1a0b5da-556e-4c08-9218-e4b7739f60b9" onclick="return false;" type="button">
+        <div id="5a730e8c-f08b-461d-83bf-20163bbf536c">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#b4d416d6-9848-42a0-bb44-a551bd742416" data-toggle="collapse" id="3fb5236b-78fa-47ba-babd-0bf49ca863b4" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#4c2186b9-89a9-4b17-b9ec-4f82c99d1d2c" data-toggle="collapse" id="36fed11a-4c6e-4a9b-b801-081121ca2a16" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#b87805a9-59cc-49bc-a215-c7c04e191fe3" data-toggle="collapse" id="f8b03cb1-fb09-4bec-8fda-0e362674a61d" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="3232fbc7-99f3-45ee-9a5c-64237762faef">
+       <span class="text-muted" id="1897b613-a0e3-4bf3-9143-0834516385cd">
         Sets padding for the left side to the specified size.
        </span>
-       <pre id="e593e9e0-3d64-4839-b617-c9e1f3abad9e"><code class="python">pl(size)</code></pre>
-       <div class="ml-3 collapse" id="e3fbbc6c-e089-4f67-905e-175c3e7ac4d9">
-        <h6 id="694635e1-2a8b-4c49-9b8c-a52ab56c88ca">
+       <pre id="9c09810a-05f2-4494-9c08-228e161d602c"><code class="python">pl(size)</code></pre>
+       <div class="ml-3 collapse" id="b4d416d6-9848-42a0-bb44-a551bd742416">
+        <h6 id="fc88c623-ff9d-4bae-8095-77de1d1fbb6b">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="9434dc52-6560-4bc6-9fec-9efb082f608e">
+        <table class="table table-sm bg-light" id="a79b3974-8d51-4f62-9e10-6a57554fe3d2">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1422,21 +1435,21 @@
            <td>
             Size of the padding to set.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="4c2186b9-89a9-4b17-b9ec-4f82c99d1d2c">
-        <h6 id="845542ec-9a16-4b82-89cb-e19569123c05">
+       <div class="ml-3 collapse" id="b87805a9-59cc-49bc-a215-c7c04e191fe3">
+        <h6 id="99e105f1-1367-478b-af8d-e9b77b2f5700">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="5c1c02b8-067e-4c6d-bd7f-3fec52187b84">
+        <table class="table table-sm bg-light" id="ab38e78d-543c-4f64-9f64-0279d24b88e3">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1461,54 +1474,55 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="3b807f91-15ff-4df2-ac52-fd9882952fa0">
-        <h6 id="ea2cba5d-0345-4c72-ab85-b5893adc436a">
+       <div class="ml-3" id="429649e6-787a-4ae5-a595-a131db01e6ed">
+        <h6 id="05eac4f7-7754-4323-8f0a-b6ad893ea8dd">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="3e583526-c0fd-49c5-918c-ae7b831a31ca"><code class="python">from bootwrap import Button
+        <pre id="a352a35e-a830-48ab-8544-e4b971e81413"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ClassMixin.
-button = Button("Hello").pl(3)</code></pre>
+button = Button("Hello").pl(3)
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="b483a89f-935d-4b02-8b31-01f0d977a7a9">
-       <div class="d-flex justify-content-between" id="b2b878e9-09e9-429c-9696-fa3fdd188000">
-        <h4 id="7ccc7a2c-7869-4257-bd2c-e2e9a82ad955">
+      <div class="mt-5" id="24c4a1c9-44da-4931-a7c8-5ccb3167c419">
+       <div class="d-flex justify-content-between" id="9a913e4e-3a4e-4a35-9e4b-0cb770fc7cc6">
+        <h4 id="58249803-6eda-45a2-85d7-6514954c9c3b">
          Method
-         <span class="text-primary" id="ebcb94cf-556d-48d4-94f5-6b7cbddb5b88">
+         <span class="text-primary" id="a1fc885b-02b8-4190-aee1-288766dc19e2">
           pr
          </span>
         </h4>
-        <div id="3fc9d516-e83b-40b2-9b62-5b82443d602e">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#08d577b8-9b09-425e-ad2f-afff6e3265cb" data-toggle="collapse" id="e6c3c40b-4082-40ab-a5be-6359985bc13a" onclick="return false;" type="button">
+        <div id="14bff1db-5d64-4ae5-abec-e2a67dcc2067">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#17ad0375-07dd-446f-a2d3-949dcc1c810a" data-toggle="collapse" id="c26ec057-9ea5-4fd1-8d79-4c83e3639cde" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#6d6aa6b9-cf44-43dd-baaf-415cc300a686" data-toggle="collapse" id="f9ecfe38-39ae-4d6b-9f9d-8907760777cf" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#899fd56b-465c-46bb-b31e-18ed134bb270" data-toggle="collapse" id="fdc8754a-313b-4e67-af56-fa4102b210b3" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="b76cfa79-d3b6-4312-b5d9-0bd8d446d73d">
+       <span class="text-muted" id="8089b821-8538-4cc6-b7e5-860a36aadca9">
         Sets padding for the right side to the specified size.
        </span>
-       <pre id="9d9fb5db-e99e-4a36-907d-0d66a942cb6f"><code class="python">pr(size)</code></pre>
-       <div class="ml-3 collapse" id="08d577b8-9b09-425e-ad2f-afff6e3265cb">
-        <h6 id="128f5d66-1893-4fe8-a673-ebcd26432a5f">
+       <pre id="b1c4486a-b3a8-479a-bc0d-a10ec8ef268b"><code class="python">pr(size)</code></pre>
+       <div class="ml-3 collapse" id="17ad0375-07dd-446f-a2d3-949dcc1c810a">
+        <h6 id="c04eec89-8d4b-4370-9faf-f2c95dd3a8d0">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="7000dd6d-1121-45cd-ad38-d468f64db3ec">
+        <table class="table table-sm bg-light" id="c247dc9e-ced3-4e62-a426-5cb7fdc3e792">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1533,21 +1547,21 @@
            <td>
             Size of the padding to set.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="6d6aa6b9-cf44-43dd-baaf-415cc300a686">
-        <h6 id="504261eb-df1e-4f1c-a052-bb0183f95456">
+       <div class="ml-3 collapse" id="899fd56b-465c-46bb-b31e-18ed134bb270">
+        <h6 id="3c068f95-7b0f-42c6-9c93-136f754112a5">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="dc076d05-5fad-40e1-8a3e-b2686203ea89">
+        <table class="table table-sm bg-light" id="49222fb2-4369-45c9-a6f3-fc2b667e8dea">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1572,54 +1586,55 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="13b8b9aa-5221-4d9c-9d19-7d6e75a11013">
-        <h6 id="b3a4e664-0551-4741-b15b-255cba54b1af">
+       <div class="ml-3" id="07c90262-0bd8-4cda-9dde-945525936684">
+        <h6 id="84f7ea67-1206-43eb-b961-8493938a6fe7">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="8937f6c6-a6e7-4bb9-8c8b-8bc955578c75"><code class="python">from bootwrap import Button
+        <pre id="b6b354d5-dda9-4d9d-9bb3-6c7fb89c05b4"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ClassMixin.
-button = Button("Hello").pr(3)</code></pre>
+button = Button("Hello").pr(3)
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="88d482cb-e77a-4b6c-880c-c05e0413a27c">
-       <div class="d-flex justify-content-between" id="20d3438c-9c15-4af7-92e8-9b1384c8bfdc">
-        <h4 id="c5f7a2b5-d30a-4dd6-a8ef-43e1b031645a">
+      <div class="mt-5" id="d93b9bfd-9789-42d7-94fc-05716aa6aaa7">
+       <div class="d-flex justify-content-between" id="daba5f01-9b8b-42a6-b852-a5a316e3e995">
+        <h4 id="2cda9e00-7e58-4e55-80d5-950e8b47b4a9">
          Method
-         <span class="text-primary" id="d21c995e-d407-470e-bcf3-6be0cd578607">
+         <span class="text-primary" id="c4e4fea1-37fa-4174-9559-2249afc72ab5">
           pt
          </span>
         </h4>
-        <div id="7134cba8-fc5a-4776-9cbb-0b35f4b70f00">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#b6dfda03-b1f7-4770-9fdd-f7e04a67a4c9" data-toggle="collapse" id="de0a806a-5e5f-4d36-9553-62d4caed3ff2" onclick="return false;" type="button">
+        <div id="8d39d339-9b85-4760-814f-88b221b459c0">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#fb6189ac-6ad8-43fe-9970-2d6c7f1bc2c6" data-toggle="collapse" id="f3f7ba29-ded3-4015-897f-43ad6194b317" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#16548d7c-4c70-4290-a663-954564dc84b1" data-toggle="collapse" id="a3119c6c-1b53-4767-929b-0c9ee7e6ee42" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#fb707a34-8360-4420-ac97-9b98238ffff0" data-toggle="collapse" id="233f751a-17bb-4a34-92e6-b57d261f3983" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="8e2dfff8-c186-459e-998f-b5dc05917e46">
+       <span class="text-muted" id="284eb556-5064-446b-8998-f41eddfe42ee">
         Sets padding for the top side to the specified size.
        </span>
-       <pre id="b0f03f9d-c6b2-4208-9b94-e9be012c054b"><code class="python">pt(size)</code></pre>
-       <div class="ml-3 collapse" id="b6dfda03-b1f7-4770-9fdd-f7e04a67a4c9">
-        <h6 id="3c821dd6-550e-4bf8-89c6-3334ec654cd4">
+       <pre id="222f1f3d-8674-44f9-ba14-e60b328ada42"><code class="python">pt(size)</code></pre>
+       <div class="ml-3 collapse" id="fb6189ac-6ad8-43fe-9970-2d6c7f1bc2c6">
+        <h6 id="0011c73e-4122-4ffd-9877-7ef35aea34bc">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="1a77775e-1f32-4a4e-bce1-e21710aafe54">
+        <table class="table table-sm bg-light" id="5ea6811b-dd17-4a02-bc1f-42519297633b">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1644,21 +1659,21 @@
            <td>
             Size of the padding to set.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="16548d7c-4c70-4290-a663-954564dc84b1">
-        <h6 id="b8c8b8e7-8e61-4445-9c79-92477a8ecca7">
+       <div class="ml-3 collapse" id="fb707a34-8360-4420-ac97-9b98238ffff0">
+        <h6 id="5f60f2b2-1336-4bf3-ba7c-dbe0e67d89e7">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="e2e74876-6426-4577-98c0-04deb0e8044f">
+        <table class="table table-sm bg-light" id="9bd43ebe-3cc6-4d1b-a5bb-9671371ee939">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1683,54 +1698,55 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="a2ac3fec-3c46-47ce-a48b-f004d4175bc2">
-        <h6 id="eaf8daf1-1dbd-4a23-bebc-42ead8549f36">
+       <div class="ml-3" id="7704273d-04bf-4ed5-8cff-fc6ecd016c87">
+        <h6 id="ec3aa324-cbfe-4a76-9d18-f410fd75c8c1">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="50ed9533-67cc-49df-8d8f-f910ab498231"><code class="python">from bootwrap import Button
+        <pre id="49620a00-576e-4338-bc19-ff38a8a13ddd"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ClassMixin.
-button = Button("Hello").pt(3)</code></pre>
+button = Button("Hello").pt(3)
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="b2ac6474-ee2f-47f8-830f-287f0baf4a45">
-       <div class="d-flex justify-content-between" id="821e9d76-720d-4971-bef7-6c0a20f76de0">
-        <h4 id="5909adcc-f307-4485-9ca8-491db740ae58">
+      <div class="mt-5" id="6b97a93d-228a-423b-accb-f66ab9a775a9">
+       <div class="d-flex justify-content-between" id="2a115fd7-953b-4dc2-bd2c-ad360aa30a99">
+        <h4 id="db1f9f7a-7304-42bc-b009-5106745ed0b6">
          Method
-         <span class="text-primary" id="a635a4a9-a557-43c3-a988-2b26f12d0177">
+         <span class="text-primary" id="9c232d82-3105-42f0-9614-5bd49d37735e">
           px
          </span>
         </h4>
-        <div id="2677485b-080d-40a7-9049-ede10ba09131">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#f9ffd8fe-f60c-40aa-9daa-ea27f79ef35d" data-toggle="collapse" id="689b8916-1140-4865-8cac-bd760d422112" onclick="return false;" type="button">
+        <div id="e16582ce-c152-4041-9b8b-23381f6805c0">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#e37530be-730e-4265-af7c-e7acec2cb48e" data-toggle="collapse" id="848d1d01-f35e-488a-a973-c462f787ebbf" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#ab13ab84-2484-4481-bbc3-0a1650cd8634" data-toggle="collapse" id="d975960d-6459-49c1-8e4a-7c9b5a6caee7" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#a66770b7-d9d1-4666-83ee-393ed4faba5e" data-toggle="collapse" id="4f456824-d0b5-4b24-b0a5-d0868c6a7ae4" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="80fa48a4-9129-4982-aa05-5e0aeb28924c">
+       <span class="text-muted" id="7060f275-584f-457b-84e7-0f9f9b8cca3b">
         Sets padding for left and right sides to the specified size.
        </span>
-       <pre id="c53423b8-dae3-4f5f-a63d-d972cfb097c8"><code class="python">px(size)</code></pre>
-       <div class="ml-3 collapse" id="f9ffd8fe-f60c-40aa-9daa-ea27f79ef35d">
-        <h6 id="f487d3ee-916e-4310-baa3-2add0ca56be1">
+       <pre id="60b5bcb4-8486-4e21-9d4c-2164b9775865"><code class="python">px(size)</code></pre>
+       <div class="ml-3 collapse" id="e37530be-730e-4265-af7c-e7acec2cb48e">
+        <h6 id="b4dab141-aabe-4982-b5ec-54ee1fecc958">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="ee0e49b9-1ec5-4cf7-8bb1-c517fdf7bfdf">
+        <table class="table table-sm bg-light" id="cbac5c19-eb6d-4b9f-8529-d3330b7e24aa">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1755,21 +1771,21 @@
            <td>
             Size of the padding to set.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="ab13ab84-2484-4481-bbc3-0a1650cd8634">
-        <h6 id="685c9ca1-d636-48a3-b7e9-f0bd402676e0">
+       <div class="ml-3 collapse" id="a66770b7-d9d1-4666-83ee-393ed4faba5e">
+        <h6 id="935fec14-c431-4b8b-91ab-439290c7af8d">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="97befa9f-3c35-408c-bb51-3715e512eeae">
+        <table class="table table-sm bg-light" id="7936e377-c8eb-4224-a240-1a099bd1ea49">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1794,54 +1810,55 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="67a60b0a-aa60-400f-be1c-21487767902f">
-        <h6 id="a7e99c16-8fed-457e-a014-9c396a705ea9">
+       <div class="ml-3" id="6d72f72d-b8dd-48eb-adf1-29460d15761f">
+        <h6 id="de79f5c8-2c42-42c5-ba72-8d5594dfc763">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="2f54db50-af08-4024-8e98-b5cdd4b5789f"><code class="python">from bootwrap import Button
+        <pre id="e4ed72c2-1d9d-476f-a6d6-9f9cda161111"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ClassMixin.
-button = Button("Hello").px(3)</code></pre>
+button = Button("Hello").px(3)
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="3838f14c-5552-4c2c-a6f2-662ef6b51ec8">
-       <div class="d-flex justify-content-between" id="81178a85-9ac2-45d1-92e7-269787965c04">
-        <h4 id="f3c694de-1829-4d70-87a9-8c8063b84e9b">
+      <div class="mt-5" id="42f4adca-1699-4492-a472-1b6eb8d2a1fa">
+       <div class="d-flex justify-content-between" id="cf090904-7dbb-4726-9497-cd1156f74974">
+        <h4 id="d96778a9-6944-4e31-bce8-5726ac2cee87">
          Method
-         <span class="text-primary" id="66c02b5f-75d8-4912-8146-228c19180f90">
+         <span class="text-primary" id="89ee7f14-1a38-422a-9b01-3fa52b2c6333">
           py
          </span>
         </h4>
-        <div id="c7e31e83-ef10-42f2-84c8-d836f4ede3db">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#889d537a-3df5-43eb-88f4-5b19799f7557" data-toggle="collapse" id="2efdde20-80a1-4f0e-bff5-49793c564eff" onclick="return false;" type="button">
+        <div id="1c124503-dd0f-4e6c-a386-8546b391776d">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#bb4cdbfe-0232-41b4-b5e0-80e058e66313" data-toggle="collapse" id="af3c350c-c0fd-4c9f-8e1d-5d9306a5e580" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#ef4fc7af-7543-482f-a64a-0ca203846076" data-toggle="collapse" id="22c491ad-bd93-43d6-a324-75a1aa8e029e" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#058a63d0-291f-4822-9ce9-a00af6f7a570" data-toggle="collapse" id="48db3a68-7159-432f-80f1-f1910078e33a" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="6caf9588-a336-4141-ba2d-98d8045cfe87">
+       <span class="text-muted" id="08d7e612-142e-4783-8036-89468627a96c">
         Sets padding for top and bottom sides to the specified size.
        </span>
-       <pre id="6dc2a1e2-0748-4fa1-a653-8b69d64df234"><code class="python">py(size)</code></pre>
-       <div class="ml-3 collapse" id="889d537a-3df5-43eb-88f4-5b19799f7557">
-        <h6 id="794efcd2-9673-4739-ab5f-56fcd38642f6">
+       <pre id="15ac9c05-821d-49f3-a293-1fb171261793"><code class="python">py(size)</code></pre>
+       <div class="ml-3 collapse" id="bb4cdbfe-0232-41b4-b5e0-80e058e66313">
+        <h6 id="ee0c2af1-66ed-4750-a253-a4540273080e">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="13e0946b-ab63-409a-a381-e72e14de3d0d">
+        <table class="table table-sm bg-light" id="38fe95fb-58d5-4f6a-bd9b-9958a435f183">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1866,21 +1883,21 @@
            <td>
             Size of the padding to set.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="ef4fc7af-7543-482f-a64a-0ca203846076">
-        <h6 id="dcc4938e-3cc9-4fa5-a4e3-dc4190610a5c">
+       <div class="ml-3 collapse" id="058a63d0-291f-4822-9ce9-a00af6f7a570">
+        <h6 id="3c640231-b863-4df1-b4d1-335dc2c968c7">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="49f9ffa7-1e9c-41bd-90cd-683d193b0006">
+        <table class="table table-sm bg-light" id="f99d9787-0054-429b-9cc9-eda57e66415e">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -1905,72 +1922,73 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="78d3bec9-442b-4330-b482-c5a4b35c2980">
-        <h6 id="4ffc4400-16df-4056-bf70-c0cad2700ed7">
+       <div class="ml-3" id="3a7bbf70-0eda-4637-93b4-7734cd78be8c">
+        <h6 id="c93ab9d2-9a2c-439e-9385-7041ef81a28b">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="4019302f-99e9-4a14-b4a5-45867541befa"><code class="python">from bootwrap import Button
+        <pre id="334f3c74-21cb-4348-b58c-4e34cb3e5afb"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ClassMixin.
-button = Button("Hello").py(3)</code></pre>
+button = Button("Hello").py(3)
+</code></pre>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="3d850a70-d19c-49e0-9ddd-eb2e3581970f">
-     <div class="mt-5" id="6ad82697-8a50-4e1f-9186-2e9fbd7eef95">
-      <div class="d-flex justify-content-between" id="2cc8f0d5-c48f-4f9a-bc1e-332e7150f0af">
-       <h1 id="314bc2f1-7352-4bf5-87ac-5de8705a1d2c">
+    <div class="tab-pane fade" id="91cf097f-77f6-40c0-a713-03c716d79f4f">
+     <div class="mt-5" id="0a0cdb9a-c851-4dce-ac3f-9953bf7f2972">
+      <div class="d-flex justify-content-between" id="e1290acf-d71f-448a-b13a-4fbc15027dc1">
+       <h1 id="27f13e24-636f-47c7-a8b7-e0b2de7ff550">
         Class
-        <span class="text-primary" id="00fabd75-41b7-4454-9b98-888370a6cee6">
+        <span class="text-primary" id="687ab179-cd5d-43e8-942e-1b5ab9531ea4">
          ActionMixin
         </span>
        </h1>
-       <div id="5e88a5aa-31d5-4e61-87cc-40fe86c735cf">
+       <div id="3caafd69-52da-4622-ae94-b68d14b7d1c1">
        </div>
       </div>
-      <span class="text-muted" id="df5d7db6-4d80-45b9-854e-0cbcdd295a10">
+      <span class="text-muted" id="e65ebd7f-dafb-4f99-9145-793a4c39a7b2">
        Mixin for a web component which able to perform an action.
       </span>
-      <pre id="c084fb57-658a-4ca6-bce4-ec54cd94e839"><code class="python">ActionMixin()</code></pre>
-      <div class="mt-5" id="c2ccdcc7-6dd4-4a75-b78b-a5dbabdd5269">
-       <div class="d-flex justify-content-between" id="65cc14a0-0e33-4be5-9a60-6c65c252db73">
-        <h4 id="26d7047f-22c8-43fa-b638-c5c86f31164e">
+      <pre id="49619a63-9896-4ffd-bd5e-3f72cde88cd1"><code class="python">ActionMixin()</code></pre>
+      <div class="mt-5" id="c528d866-2c4c-4c06-8641-d82fec90c134">
+       <div class="d-flex justify-content-between" id="9265d690-302a-440f-95c8-d7ccac77ae89">
+        <h4 id="49eb7915-7ee7-4196-8917-3b809fe040c5">
          Method
-         <span class="text-primary" id="09e28634-0007-4d9d-ade1-89459334acbe">
+         <span class="text-primary" id="9f7c3e72-46ab-45fd-bf69-b66a40e5dc74">
           add_menu
          </span>
         </h4>
-        <div id="0747fb6d-7cce-43bc-b866-24657f3c3685">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#9cc3c2a8-0551-4c7e-b7d7-9dd9ccd5c0fc" data-toggle="collapse" id="6ba2e9df-1d1d-476f-b928-ad88ff9bf6fe" onclick="return false;" type="button">
+        <div id="ba38a0c5-62b2-40e9-91ef-4498b9f6c436">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#3cbf7bb7-f060-42c6-abd6-ac6efc114b9b" data-toggle="collapse" id="33eb37a5-4dd5-4688-bcd9-7007e7788653" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#5f1ca249-a12b-4164-966b-55da4064b0e3" data-toggle="collapse" id="a9888e3b-db00-4741-bb4b-83172dd15e12" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#770fd0a4-e15d-4cae-926e-43fe265fac40" data-toggle="collapse" id="573f8d0e-e444-4ef5-9516-60c4274c8997" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="3d36dca2-3875-4d48-b79e-91976fc45db3">
+       <span class="text-muted" id="c75d8cb5-7bba-4727-b48c-9ca5515035e5">
         Adds dropdown menu.
        </span>
-       <pre id="55b112c1-a7b1-45e5-91e0-4ba4586cac86"><code class="python">add_menu(*menu)</code></pre>
-       <div class="ml-3 collapse" id="9cc3c2a8-0551-4c7e-b7d7-9dd9ccd5c0fc">
-        <h6 id="a448cfdb-0e59-41b8-bb58-6fec913d2887">
+       <pre id="42520553-6b79-4ff0-bf87-35bfa050f849"><code class="python">add_menu(*menu)</code></pre>
+       <div class="ml-3 collapse" id="3cbf7bb7-f060-42c6-abd6-ac6efc114b9b">
+        <h6 id="788e84da-5b08-4e4a-9ea1-01e8c79088c7">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="8899d4f7-5627-4865-ac06-659e6d7432ac">
+        <table class="table table-sm bg-light" id="f0d1490f-2783-466b-ac06-7be282217ee9">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -2004,21 +2022,21 @@
             </code>
             class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="5f1ca249-a12b-4164-966b-55da4064b0e3">
-        <h6 id="876d9d08-4f72-4405-8e46-eb1ddb860885">
+       <div class="ml-3 collapse" id="770fd0a4-e15d-4cae-926e-43fe265fac40">
+        <h6 id="3cce767a-ba87-4a7b-b6b1-3a8c54eee94f">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="faeb983d-1ae5-4598-ac13-2821dabca42a">
+        <table class="table table-sm bg-light" id="0146ce6f-6bb5-4eba-8986-9c399305724b">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -2043,55 +2061,56 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="46487eb1-7d23-4b00-8717-3fb6fcd0772b">
-        <h6 id="bc3e8c0c-fea9-4034-a902-89b9cc8b1041">
+       <div class="ml-3" id="39812f2c-faeb-417e-bad2-fb851c323a52">
+        <h6 id="5bdea348-7232-4e1e-9d5b-f9b40c3f03e0">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="cab2ab6e-8e1f-4808-8688-2d5d2d442f6a"><code class="python">from bootwrap import Button
+        <pre id="c21c2311-66fc-4eba-bf4e-b76662d3d0b4"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ActionMixin.
 button = Button('Portfolio').add_menu(
     Button("Buy"),
     Button("Sell"),
     Button("Transfer")
-)</code></pre>
+)
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="8f7105a8-8e03-4064-bc77-67b2adb52343">
-       <div class="d-flex justify-content-between" id="4d0c8d48-6702-4713-8ede-9fc4fbba6850">
-        <h4 id="996cb6d4-a8e8-441f-95c9-4e11df0451f0">
+      <div class="mt-5" id="402611da-9c76-4858-8e9d-12292606b6e6">
+       <div class="d-flex justify-content-between" id="3a5b236e-0b3f-4695-a2f5-3be8e4d1086f">
+        <h4 id="d4cdacc4-1776-43f2-93cc-24dc5ab54ac1">
          Method
-         <span class="text-primary" id="aba9fdbd-2189-4dfa-bf86-80fa784f7595">
+         <span class="text-primary" id="fb24bdb7-05b5-4e0a-a270-00e7245e6680">
           dismiss
          </span>
         </h4>
-        <div id="d937287e-4adb-418c-b867-fcd9374490fa">
-         <button class="btn-sm btn btn-outline-primary" data-target="#642ad049-ef37-4dcc-8f81-2d699c3a8b25" data-toggle="collapse" id="f0ee30ff-6fd5-4849-b45b-e00cb4ce4413" onclick="return false;" type="button">
+        <div id="1194c59b-ed33-452e-8327-83dfa9a792d4">
+         <button class="btn-sm btn btn-outline-primary" data-target="#16bcab11-80c6-447e-a1e4-e811073b53d9" data-toggle="collapse" id="e758d479-4c9b-4a4f-ab82-f87f843d38c4" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="4e0340a3-12d7-4e39-9541-4b44ad29cbbd">
+       <span class="text-muted" id="95b4c1b5-9c37-4ed4-aa90-13aa683cf8aa">
         Performes a dismiss action.
        </span>
-       <pre id="1797b946-a8aa-421a-a791-aa40ac905f5d"><code class="python">dismiss()</code></pre>
-       <div class="ml-3 collapse" id="642ad049-ef37-4dcc-8f81-2d699c3a8b25">
-        <h6 id="959e2a33-bf83-41ae-86da-ece14a8bd539">
+       <pre id="e74561fe-0a51-49b2-9530-464ddc8a2cef"><code class="python">dismiss()</code></pre>
+       <div class="ml-3 collapse" id="16bcab11-80c6-447e-a1e4-e811073b53d9">
+        <h6 id="2cf833fd-8ae9-4a2d-8325-5f72e59ec987">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="882d6971-85ad-4c57-ad5c-d76063236220">
+        <table class="table table-sm bg-light" id="693f0988-e2af-44d3-a174-d9fe6b74d471">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -2116,57 +2135,58 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="352995eb-ad6f-4675-9339-5da0a774afea">
-        <h6 id="1f0613ff-45e2-419c-9cc3-4c4faa49de5e">
+       <div class="ml-3" id="d6998372-88b6-4442-9ff1-e41bd54e55ff">
+        <h6 id="a028e098-8a40-4281-859d-d3891325c336">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="defa09e3-b857-4fd1-af75-b523b0825adf"><code class="python">from bootwrap import Dialog, Button
+        <pre id="f1eac573-011a-4742-a265-6899e613edbf"><code class="python">from bootwrap import Dialog, Button
 
 # Note, that Button inherits ActionMixin.
 dialog = Dialog(
     ...,
     Button("Bye").dismiss()
-)</code></pre>
+)
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="14ff26c2-4a5f-46da-9792-2fd9db1465ab">
-       <div class="d-flex justify-content-between" id="5891acae-b905-41bd-a856-04e1dc177a7b">
-        <h4 id="dae05b87-d7a4-4551-abf2-d18b83f22d27">
+      <div class="mt-5" id="61fa2fa7-31af-4eb0-91a4-1cc1de5d692a">
+       <div class="d-flex justify-content-between" id="97abf760-42b1-4a7e-abc5-a8f34b9bcfa8">
+        <h4 id="386de36f-2eaa-4006-8803-ee630fd2f128">
          Method
-         <span class="text-primary" id="532ab04b-9167-4b5d-ae20-90b446a9fd5f">
+         <span class="text-primary" id="5921c756-8e13-4ea1-bea7-a560e31396dd">
           link
          </span>
         </h4>
-        <div id="74fbb0ae-61b2-4139-b8c0-74df6c171eb1">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#ce2e0879-ebc7-44c0-8380-3b08cfd28298" data-toggle="collapse" id="f606f733-355b-43ae-bdd8-666754d6efc2" onclick="return false;" type="button">
+        <div id="04d8d026-0813-4e6e-bb4d-1340797bead9">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#6e47cae7-685f-41c7-849d-93183e247f43" data-toggle="collapse" id="0d8d4321-4228-495f-9195-9d2e6e7fa17c" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#c940d701-210a-472c-8883-ca4cf5a45716" data-toggle="collapse" id="a078df82-efbc-43fd-a08a-8f5f64005c4f" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#2d568dc4-3ac4-4917-b0eb-daf4f52b2b0d" data-toggle="collapse" id="45d7a56b-2ae4-45b6-be9c-a3ac1d6530f5" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="58e045fa-a14b-4644-b76f-d9c3635a194c">
+       <span class="text-muted" id="53a05257-de3a-4102-9291-53001995e32d">
         Links to the web-resource.
        </span>
-       <pre id="c19347aa-31c1-4f06-b65b-4e054cd7a742"><code class="python">link(target)</code></pre>
-       <div class="ml-3 collapse" id="ce2e0879-ebc7-44c0-8380-3b08cfd28298">
-        <h6 id="c6983f6d-c2a2-4722-9e5d-3e7c74f35037">
+       <pre id="2b444f22-141c-462f-afb3-b67c213de946"><code class="python">link(target)</code></pre>
+       <div class="ml-3 collapse" id="6e47cae7-685f-41c7-849d-93183e247f43">
+        <h6 id="5d289ad0-5fc3-4908-b943-c08117983da2">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="24199729-0a0d-4ee3-bfc0-d5f25b19c66b">
+        <table class="table table-sm bg-light" id="1807bd13-dc2a-460e-bbb2-274a0d3d3489">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -2196,21 +2216,21 @@
             </code>
             .
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="c940d701-210a-472c-8883-ca4cf5a45716">
-        <h6 id="da655c38-d1ce-4324-ab37-31a31ae58fce">
+       <div class="ml-3 collapse" id="2d568dc4-3ac4-4917-b0eb-daf4f52b2b0d">
+        <h6 id="f880269d-415d-4b50-97d5-ce3bdb6b41e9">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="356cc728-54f1-4eb9-a67a-5c7d655b5ac3">
+        <table class="table table-sm bg-light" id="c56eaa19-4330-4443-8d6b-d0689d97bb35">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -2235,51 +2255,52 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="87527319-7110-4d77-9c07-f7d6f10b669f">
-        <h6 id="3809252b-f3ed-4785-b4b1-eb170b49f1cd">
+       <div class="ml-3" id="804e5b8b-e9bd-414a-a32a-46d1a82b5123">
+        <h6 id="6d0164c5-be3d-4d3b-be13-ed4c7b30b6e4">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="2860b2ef-f940-42d8-807d-e8876bd7b4a6"><code class="python">from bootwrap import Button
+        <pre id="e60f3816-1985-4b0b-b8f5-b25a74ee1fea"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits ActionMixin.
-button = Button("Search").link("https://www.google.com")</code></pre>
+button = Button("Search").link("https://www.google.com")
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="c28e7ea2-08a1-43f6-9df9-48c2cae5c21e">
-       <div class="d-flex justify-content-between" id="56cc279a-2455-4b72-b698-858e768f4d96">
-        <h4 id="3c780fc1-9ff5-448c-9885-9cfdd4a78544">
+      <div class="mt-5" id="065e4a7a-0fa8-4a43-a8d3-419e87cf8dff">
+       <div class="d-flex justify-content-between" id="6385390c-2310-4e83-8fd7-b25816659381">
+        <h4 id="097efffd-e1d8-48a9-bd40-b2e02d8e0dda">
          Method
-         <span class="text-primary" id="9fcfad5f-b3f6-4776-8245-760ba5e76ced">
+         <span class="text-primary" id="a508db2c-b814-49b6-a9c1-4926322ec379">
           submit
          </span>
         </h4>
-        <div id="75ab57d7-68d9-4601-8330-6cb551d2483c">
-         <button class="btn-sm btn btn-outline-primary" data-target="#0759ba1e-dcf0-4d96-99ce-4384238326ab" data-toggle="collapse" id="721e8dac-b11f-488d-8658-d0e5b236eacf" onclick="return false;" type="button">
+        <div id="27509427-aa6b-4c74-8f3f-6722691ec9ad">
+         <button class="btn-sm btn btn-outline-primary" data-target="#9a61494f-71b0-4ed2-94a1-b708d24ce152" data-toggle="collapse" id="3c2faff6-0ded-4da3-9cbd-b393e0c4dc0e" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="479ed82a-ba09-4f14-b80d-eccca14a0120">
+       <span class="text-muted" id="7d3f4ae4-4ee4-4e77-94f6-3dcb3535f94b">
         Performes a submit action.
        </span>
-       <pre id="3df3e90c-c884-420c-932a-5d5c17a061dd"><code class="python">submit()</code></pre>
-       <div class="ml-3 collapse" id="0759ba1e-dcf0-4d96-99ce-4384238326ab">
-        <h6 id="758027c4-35ee-40fe-a376-84925c52b92e">
+       <pre id="4d878385-5d76-4617-9c0f-7b06519c7359"><code class="python">submit()</code></pre>
+       <div class="ml-3 collapse" id="9a61494f-71b0-4ed2-94a1-b708d24ce152">
+        <h6 id="5f560847-7284-4b46-a768-2b07d6296cda">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="ecace5f0-b8fc-42f4-bcf2-eca37ee0a797">
+        <table class="table table-sm bg-light" id="ad3d09ad-64f6-4bdc-8cac-c6cc9d38a48d">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -2304,57 +2325,58 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="b72e99e9-62e7-41e2-ba0c-9dd55c7227d6">
-        <h6 id="2ea39d95-c5d7-4b7b-9dbb-166a84d990de">
+       <div class="ml-3" id="8c7f3e59-249e-4718-b3b9-bfa778ee6b90">
+        <h6 id="13e5ae7c-e575-4095-a227-a1aa7f664fa8">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="7b0d396c-8ca1-4351-944b-56f61a3201ab"><code class="python">from bootwrap import Form, Button
+        <pre id="5f542476-e763-446a-a1c2-ad3bfa81d150"><code class="python">from bootwrap import Form, Button
 
 # Note, that Button inherits ActionMixin.
 form = Form(
     ...,
     Button("Send").submit()
-)</code></pre>
+)
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="3e4e6209-ac75-4ac2-9356-508bc454cfb9">
-       <div class="d-flex justify-content-between" id="2ee1e875-54e7-43ac-affc-4fd6376a9260">
-        <h4 id="04421707-4115-4960-b2e3-5790b6f5e3bb">
+      <div class="mt-5" id="1e51485b-68e4-40d8-b17a-27aa44e4087b">
+       <div class="d-flex justify-content-between" id="108663f1-be33-4759-aa2e-075f75b3ae54">
+        <h4 id="0953b614-4ab0-44df-ac15-b850d92910d8">
          Method
-         <span class="text-primary" id="cec322a0-1297-4e91-9824-dced95301f97">
+         <span class="text-primary" id="3b94df81-1c4b-4526-84ca-79d75bd64578">
           toggle
          </span>
         </h4>
-        <div id="8151fd2c-f76d-4620-84da-67b9a7f4f790">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#3fa676ae-8376-4dd9-b2a0-1ae31f36daf5" data-toggle="collapse" id="9f0decb4-1ce6-418c-b059-2f8c06ed4591" onclick="return false;" type="button">
+        <div id="87f97a7f-8e59-4690-8dfd-c318506511f8">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#ff06c790-692e-4de0-83d3-6ddcaa67f288" data-toggle="collapse" id="b5f7397f-7547-4e67-bae2-ce2418e560ba" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#2353ae95-809a-4d0d-adc6-68993319ce84" data-toggle="collapse" id="eea6bcfa-23e9-4bf5-adae-4fd67dfe6914" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#2b5f2719-86da-4f37-a1a4-ba5d6af39725" data-toggle="collapse" id="14ce155c-253e-4591-a925-199e9546f0a0" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="4b7dc29d-f729-470c-a3a8-1aefe0418bfc">
+       <span class="text-muted" id="cd630db0-8bdc-4a95-8568-0068103773e6">
         Toggles an other web component.
        </span>
-       <pre id="899dd766-4896-4f7c-b519-02aa6e58dd17"><code class="python">toggle(target)</code></pre>
-       <div class="ml-3 collapse" id="3fa676ae-8376-4dd9-b2a0-1ae31f36daf5">
-        <h6 id="ea1275be-4199-450c-9065-3c9abae16eed">
+       <pre id="c50bcb8a-6475-4a6b-9c44-3ba49a3ff3c0"><code class="python">toggle(target)</code></pre>
+       <div class="ml-3 collapse" id="ff06c790-692e-4de0-83d3-6ddcaa67f288">
+        <h6 id="05158d34-13ed-470a-b7e4-e3d2d27ee473">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="35c5450e-b23f-4fea-bb76-78759c01a9f1">
+        <table class="table table-sm bg-light" id="4f4dc340-eab7-455c-98a5-bb08d2fb54a9">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -2379,21 +2401,21 @@
            <td>
             The web component to toggle.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="2353ae95-809a-4d0d-adc6-68993319ce84">
-        <h6 id="d0154d26-417f-4974-9720-770a6e619388">
+       <div class="ml-3 collapse" id="2b5f2719-86da-4f37-a1a4-ba5d6af39725">
+        <h6 id="e0c09957-a3d9-41eb-88eb-d7a102d911b7">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="2011f69b-8623-48ce-9c43-e1d120841d6a">
+        <table class="table table-sm bg-light" id="b22d1e89-c79b-45a8-bdda-ca9ba1dcb28c">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -2418,71 +2440,72 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="ad740611-16c8-4068-ba81-0db94dc10ff9">
-        <h6 id="6574b3c4-52c2-43e0-bdb1-0c7a43baf942">
+       <div class="ml-3" id="ec3859da-c9a8-4e8f-9cfa-f7f090a8c371">
+        <h6 id="0e4015a1-5196-4e0e-89e0-1ed16739bf9a">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="1a33f11f-b590-4bc3-9505-38bbd8df9c32"><code class="python">from bootwrap import Button, Dialog
+        <pre id="5d228f24-3aba-423f-962c-90c54e04c213"><code class="python">from bootwrap import Button, Dialog
 
 # Note, that Button inherits ActionMixin.
 dialog = Dialog(...)
-button = Button("Open").toggle(dialog)</code></pre>
+button = Button("Open").toggle(dialog)
+</code></pre>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="a743d34d-aadd-4be3-a44f-008d0b782587">
-     <div class="mt-5" id="643d71b4-14e8-486b-a80d-3dc8e6314751">
-      <div class="d-flex justify-content-between" id="4efdf582-1aae-4f1f-b53e-596d87a21ac7">
-       <h1 id="ee2e8d87-9984-46ff-afe5-81f081d98a10">
+    <div class="tab-pane fade" id="8bb80617-6b52-4ffa-82c9-25c8edb4a396">
+     <div class="mt-5" id="11b92557-e53d-49ce-9235-ea8fe34d135b">
+      <div class="d-flex justify-content-between" id="aaa2f95e-1f9c-4f4e-bfd5-f6fe72e0c469">
+       <h1 id="eddbc8ed-2fef-4585-b5e5-f08745186c0f">
         Class
-        <span class="text-primary" id="e14b8634-dcab-4eea-9f09-d8187bd60e2e">
+        <span class="text-primary" id="9aa85ea3-fd5a-4b89-9da3-15a72ce8ca74">
          AppearanceMixin
         </span>
        </h1>
-       <div id="f4b2ef0e-c281-4783-83b6-2b71bb0ff543">
+       <div id="431b545b-6b55-4ce0-823e-dc821f145f52">
        </div>
       </div>
-      <span class="text-muted" id="c6b0461c-8819-46fc-9815-ec8a541e060b">
+      <span class="text-muted" id="08cfef28-0057-4845-b82d-aba02b6dbcf2">
        Mixin for a web component which appearance can be associated
     with predefined categories.
       </span>
-      <pre id="0b6d62a0-b350-440c-9dac-2238bca10818"><code class="python">AppearanceMixin()</code></pre>
-      <div class="mt-5" id="17345ab2-e033-46cc-99da-c4250cf8af2c">
-       <div class="d-flex justify-content-between" id="79bb4118-84e1-4074-84d6-2119b0a101b3">
-        <h4 id="877634a9-9aba-42e7-bb63-8ddf7bf6d71a">
+      <pre id="58a1a846-2bf9-482d-9b09-6e52205d6637"><code class="python">AppearanceMixin()</code></pre>
+      <div class="mt-5" id="a9431970-0813-4e2d-9afd-05394619749a">
+       <div class="d-flex justify-content-between" id="98fa51d1-c15f-41b6-9f27-1e48f4376e2c">
+        <h4 id="5c75c0c3-dc8b-40b2-80ae-268be8b9d006">
          Method
-         <span class="text-primary" id="0d3be1e5-b6fa-43ff-8d84-2c110696613d">
+         <span class="text-primary" id="e1978e22-327e-42d5-aadd-aaff116d8c72">
           as_danger
          </span>
         </h4>
-        <div id="e02e926d-b8be-4a6f-846c-207d167ef08c">
-         <button class="btn-sm btn btn-outline-primary" data-target="#b79ea768-3e18-49de-9b17-2ff3e2e83a5c" data-toggle="collapse" id="6c07b8d8-b1af-4d97-ab32-51d93d45caeb" onclick="return false;" type="button">
+        <div id="8ef61e89-52bb-4619-b05f-14debb2bb7ae">
+         <button class="btn-sm btn btn-outline-primary" data-target="#965ff628-1ec6-4ad5-a797-17557ab3c94e" data-toggle="collapse" id="2d5b2ea2-0c95-4715-9712-9d1cdd81ebb2" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="289f988b-9e6f-42f4-ac6c-681c29668813">
+       <span class="text-muted" id="e3425172-d190-4368-9143-c61fbf8862a3">
         Makes the 'danger' look to a web components.
        </span>
-       <pre id="c97f2385-d24f-4fc4-8dfa-5b99ac542f67"><code class="python">as_danger()</code></pre>
-       <div class="ml-3 collapse" id="b79ea768-3e18-49de-9b17-2ff3e2e83a5c">
-        <h6 id="5d448e12-92c9-457a-9991-4368cbace92d">
+       <pre id="2c5b03d9-9927-468a-9d22-f84a436b1c53"><code class="python">as_danger()</code></pre>
+       <div class="ml-3 collapse" id="965ff628-1ec6-4ad5-a797-17557ab3c94e">
+        <h6 id="a11dc377-e92a-4c56-abd5-0cbcc66736de">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="3b4f33db-56bb-496a-925c-83787adf66e0">
+        <table class="table table-sm bg-light" id="966f6393-b157-4e26-91d3-eeaa37e81409">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -2507,51 +2530,52 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="fa5debfe-9a0d-49bc-ba5c-c295c0cb4011">
-        <h6 id="0ef10bad-91d2-4966-8c30-05992fe00a77">
+       <div class="ml-3" id="9f2d101f-8a40-474a-8f86-56e4e29f63c3">
+        <h6 id="1dc6ec99-9084-4bc4-a819-92f1b7bd77f4">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="8e357dab-3456-439d-9db1-ffcf8194eb9d"><code class="python">from bootwrap import Button
+        <pre id="e98e9072-bd10-42f5-8080-a156810eb05a"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits AppearanceMixin.
-button = ("Danger").as_danger()</code></pre>
+button = ("Danger").as_danger()
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="23d35b5b-cffd-48aa-9f3e-2c11f4c2f914">
-       <div class="d-flex justify-content-between" id="51030c01-89ae-4ae0-9944-c85f695f808e">
-        <h4 id="36b2c612-60ab-42b5-9b5c-7849048ffe65">
+      <div class="mt-5" id="ca57a67d-137c-442f-bdf7-da1470d91ab9">
+       <div class="d-flex justify-content-between" id="6e1867c0-19a3-4528-b1df-8d6e903ed82d">
+        <h4 id="68a31e13-e7b6-4cd4-8981-a601cfa3a009">
          Method
-         <span class="text-primary" id="330549ff-4d18-4448-afbe-ad403ef5aa34">
+         <span class="text-primary" id="6038b500-8d68-4726-aaa4-d29a17012b02">
           as_dark
          </span>
         </h4>
-        <div id="aeed0956-0a51-48c7-a2d5-1df2d2e4f6c2">
-         <button class="btn-sm btn btn-outline-primary" data-target="#5ca3ee15-3bf3-4e17-91e9-00358a21b3bc" data-toggle="collapse" id="6b261e5f-5c5d-4c4d-9d61-1643d89f6db2" onclick="return false;" type="button">
+        <div id="230d61b9-04b4-4bb6-9485-71fc234a35ec">
+         <button class="btn-sm btn btn-outline-primary" data-target="#bbfc6824-bf49-481f-bc53-a28a0ef4a25a" data-toggle="collapse" id="7facc32c-f775-46b2-9275-2e8bd00091e6" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="939c008a-147c-46c8-a5e2-6e224496004a">
+       <span class="text-muted" id="d1e9f701-9c6f-4ae1-a460-0bf238214fa9">
         Makes the 'dark' look to a web components.
        </span>
-       <pre id="de21a928-6484-4f80-9ca9-ed17c1f526f9"><code class="python">as_dark()</code></pre>
-       <div class="ml-3 collapse" id="5ca3ee15-3bf3-4e17-91e9-00358a21b3bc">
-        <h6 id="e00d9b1f-0161-4b6c-9dc6-1b8c049bf2bb">
+       <pre id="20fd3925-0a35-4d33-ab97-1f77f9da1016"><code class="python">as_dark()</code></pre>
+       <div class="ml-3 collapse" id="bbfc6824-bf49-481f-bc53-a28a0ef4a25a">
+        <h6 id="5ea8c42b-0149-420e-9c74-054cc7a9b733">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="d03b9183-13d8-4550-b1f8-12de3fc87d9c">
+        <table class="table table-sm bg-light" id="4a4547d3-3b6d-4844-907e-a3f0e60f0ae8">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -2576,51 +2600,52 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="3b964eb5-52a8-4db9-82ef-c1adcf219aa4">
-        <h6 id="064227df-6e16-4fbb-9c19-a0b065f883c8">
+       <div class="ml-3" id="dad2149d-88f5-4876-8afe-c8e7efa1461e">
+        <h6 id="f2a720b9-2676-4173-9178-c247419e636a">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="abd4993b-ec13-4483-8886-a9b538510200"><code class="python">from bootwrap import Button
+        <pre id="15f00f42-c6f6-4142-8ed8-6867e956f43a"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits AppearanceMixin.
-button = ("Dark").as_dark()</code></pre>
+button = ("Dark").as_dark()
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="1cf58472-010e-4847-997e-eb82bde44471">
-       <div class="d-flex justify-content-between" id="614a8049-acae-4d52-8d01-51ad187161b8">
-        <h4 id="ece1dddb-6c97-42c2-967f-59923c9fdd56">
+      <div class="mt-5" id="83492610-9ca4-4f92-a143-215fb5b2dd83">
+       <div class="d-flex justify-content-between" id="1f5c52e0-4bad-468b-8cb6-9b27006a98ba">
+        <h4 id="f3771d4c-cef5-44ba-b630-5309c8d81f55">
          Method
-         <span class="text-primary" id="badeb783-5c5b-4d2e-a29a-eecac3b70493">
+         <span class="text-primary" id="9a597105-024a-4e2c-8d47-2e0be59a3b9d">
           as_info
          </span>
         </h4>
-        <div id="27e52ee0-2389-402b-8e31-5f2d815a2f48">
-         <button class="btn-sm btn btn-outline-primary" data-target="#5c3bdc48-b285-4802-9d4f-38254f310957" data-toggle="collapse" id="e3b64ef9-8443-4a2a-9cb4-ad59d5b168d8" onclick="return false;" type="button">
+        <div id="9cef1ba1-c5cf-4365-9164-f89daa5266ec">
+         <button class="btn-sm btn btn-outline-primary" data-target="#43dba155-994f-43b3-b60e-e02641d96aa4" data-toggle="collapse" id="bf7b6381-61d2-44d3-a684-c5d269c8f877" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="0818c4c9-656e-47d8-b2f5-7c104ba25751">
+       <span class="text-muted" id="0d372e85-f6d8-480b-aa65-d66cc739fda2">
         Makes the 'info' look to a web components.
        </span>
-       <pre id="05f0484d-fb60-44b1-b5a9-d2e3f8c37de8"><code class="python">as_info()</code></pre>
-       <div class="ml-3 collapse" id="5c3bdc48-b285-4802-9d4f-38254f310957">
-        <h6 id="92850d9a-2b0e-4c45-9f21-c7e84322c341">
+       <pre id="f0559562-e1fb-4ba0-a9da-d4314815f5cd"><code class="python">as_info()</code></pre>
+       <div class="ml-3 collapse" id="43dba155-994f-43b3-b60e-e02641d96aa4">
+        <h6 id="a624e39b-b0ec-47a6-a986-0622ec3ccfb8">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="7650aca8-754e-421e-84dd-ae2e1b1cca2d">
+        <table class="table table-sm bg-light" id="9468d2d2-2766-42e2-a51c-d150fea30212">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -2645,51 +2670,52 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="ae93e225-c904-4f6d-ad23-8bdbbd61b788">
-        <h6 id="7c5b40ee-78ec-41e5-b123-3327049f0166">
+       <div class="ml-3" id="1fe72b3b-f5c6-4833-9e7a-842dd98db800">
+        <h6 id="26384190-e235-420f-a924-e0ec1fbbd9e2">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="17b5ba0e-47b6-43dc-b398-24cc6136feea"><code class="python">from bootwrap import Button
+        <pre id="4e1a15ae-ff44-475e-acce-54777d7e65bf"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits AppearanceMixin.
-button = ("Info").as_info()</code></pre>
+button = ("Info").as_info()
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="c805ff63-5ab3-491d-9177-54d13fd7c65e">
-       <div class="d-flex justify-content-between" id="16cd5063-9d59-47c2-80f1-d2c392f3b8c3">
-        <h4 id="8f949bc4-e5e9-4dc5-9bdf-e6d9f5528038">
+      <div class="mt-5" id="22691efc-d888-440e-97aa-2922fb2d57bc">
+       <div class="d-flex justify-content-between" id="a3ed3aa4-ec62-40f9-91bf-551ff9ad5d2d">
+        <h4 id="aa58ab26-4ef2-4f5b-8530-aa8ca3591784">
          Method
-         <span class="text-primary" id="2db3cfe7-6843-4eec-97c7-bac3d4a710a8">
+         <span class="text-primary" id="38f4dae5-ed6d-48af-b105-35e55d449d13">
           as_light
          </span>
         </h4>
-        <div id="fb4b2c34-5d95-4599-8eb8-dbb84a2c5b39">
-         <button class="btn-sm btn btn-outline-primary" data-target="#d886ac7a-e18e-4512-a3c6-cfa90da04717" data-toggle="collapse" id="e5472ee5-cc57-41ac-96ec-7b0680ba13d1" onclick="return false;" type="button">
+        <div id="280173cf-28a0-40ea-88ea-2ead6153d119">
+         <button class="btn-sm btn btn-outline-primary" data-target="#dcce5525-11f0-4c7b-b11c-0cd61c1b3681" data-toggle="collapse" id="060ec6cb-bc81-46b8-8fd0-81907c39e64c" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="22bfb675-130f-4d73-a6ad-d19d73f73226">
+       <span class="text-muted" id="5ce27fe7-3a0f-4ff7-b01c-119ec396e3c0">
         Makes the 'light' look to a web components.
        </span>
-       <pre id="c450c1bb-d433-443b-8ebd-361e4f0a47a0"><code class="python">as_light()</code></pre>
-       <div class="ml-3 collapse" id="d886ac7a-e18e-4512-a3c6-cfa90da04717">
-        <h6 id="56500e2a-0277-4be6-b437-2f5b4a5e062f">
+       <pre id="c586c520-977f-47c6-b3f2-d995ae29fe8e"><code class="python">as_light()</code></pre>
+       <div class="ml-3 collapse" id="dcce5525-11f0-4c7b-b11c-0cd61c1b3681">
+        <h6 id="69142022-efa6-4269-b0e3-eab1d694f3b5">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="83871cd3-b50a-43f6-86b7-6adc88666e6b">
+        <table class="table table-sm bg-light" id="9895c606-fb78-4f73-bb3f-e3a58546989d">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -2714,51 +2740,52 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="cef44a7e-6ed9-43c1-ae7b-0af7141a3f2c">
-        <h6 id="953ff968-e382-4888-abe8-78cdc52b3cfa">
+       <div class="ml-3" id="99bc4d05-2f6c-42e3-9973-4146a595683d">
+        <h6 id="5704969c-9f84-44d2-86ed-0b1d18a7a3d1">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="e50d1969-96cc-4a6c-a14b-d4a6e610784c"><code class="python">from bootwrap import Button
+        <pre id="306e3d48-4032-4798-83fd-48d1446886ae"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits AppearanceMixin.
-button = ("Light").as_light()</code></pre>
+button = ("Light").as_light()
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="adbfefc7-afce-42c1-9a03-74f1d1039423">
-       <div class="d-flex justify-content-between" id="d6a5433a-84c1-405e-b78c-25ec6d91dee5">
-        <h4 id="dd57a90b-e419-403a-8a63-8dcc44ae86ca">
+      <div class="mt-5" id="4ec7fad7-71ce-4a27-80cf-e51b46aaaf34">
+       <div class="d-flex justify-content-between" id="f6194309-ded2-4912-8674-9428a384a7bf">
+        <h4 id="386ac561-6680-4b90-91b7-7c7a664a03c3">
          Method
-         <span class="text-primary" id="b9f9c750-c197-4d2d-9bae-d1f4308f5490">
+         <span class="text-primary" id="7f08c656-43d3-497a-ae17-0f8668221b6e">
           as_primary
          </span>
         </h4>
-        <div id="88f48a5a-a664-482e-bbd2-36f3a96f9de6">
-         <button class="btn-sm btn btn-outline-primary" data-target="#63438d5f-1a00-4848-a06d-adc45faa5123" data-toggle="collapse" id="9e73e1e8-9530-4ff5-9a9e-1f16ed3fb020" onclick="return false;" type="button">
+        <div id="9190bb90-e1eb-407c-a63e-a3949cb8c64e">
+         <button class="btn-sm btn btn-outline-primary" data-target="#076dda46-fce3-4c6e-af02-3516d443fad8" data-toggle="collapse" id="ee743ce7-8ab3-4e51-b687-7904afd4298d" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="825fc6ef-69cf-49f1-ab0d-21884c654073">
+       <span class="text-muted" id="b36ae391-d730-42de-92bb-417c503acd56">
         Makes the 'primary' look to a web components.
        </span>
-       <pre id="85df1e59-eb6a-4b37-b812-1f2404703c80"><code class="python">as_primary()</code></pre>
-       <div class="ml-3 collapse" id="63438d5f-1a00-4848-a06d-adc45faa5123">
-        <h6 id="89ca5342-4a52-4d87-9abd-ebcd91260142">
+       <pre id="7dfeed25-a79c-45b7-a1a6-8a3df16eda7c"><code class="python">as_primary()</code></pre>
+       <div class="ml-3 collapse" id="076dda46-fce3-4c6e-af02-3516d443fad8">
+        <h6 id="fbf53692-aa60-41a5-b76f-c127d22c1a80">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="78056754-4f25-4df9-95a3-db5f500c80a5">
+        <table class="table table-sm bg-light" id="e2ad92d9-85a3-47d7-a704-0e2f5368cf72">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -2783,51 +2810,52 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="d0d3ac9b-7c37-4dde-9a48-f6f653f681f7">
-        <h6 id="433deee1-c5de-479e-bcf0-f694dcdbcb18">
+       <div class="ml-3" id="013e0dfe-1316-41ea-aa12-c52649b8b41a">
+        <h6 id="bec9f6c9-3983-4e6a-8f20-da2b3b9e8329">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="67a2ccff-9d8b-41f1-92d0-abe850628600"><code class="python">from bootwrap import Button
+        <pre id="c092cd46-41cd-4568-afcc-cdc5e9ba914e"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits AppearanceMixin.
-button = ("Primary").as_primary()</code></pre>
+button = ("Primary").as_primary()
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="2e6c6766-b49e-48b8-92e4-a7b44dfb2b7c">
-       <div class="d-flex justify-content-between" id="7181b2e1-176c-44e7-9034-93c62cc71037">
-        <h4 id="56928692-1691-418f-8e21-fc2c58e3f5a4">
+      <div class="mt-5" id="6aa8b141-0963-4463-b4d2-9190bd675207">
+       <div class="d-flex justify-content-between" id="196bd79c-0ccd-4ee9-8d39-abc544771ce3">
+        <h4 id="dc4e5e2b-0b5a-440b-b325-6598b7e4e7c5">
          Method
-         <span class="text-primary" id="c9156c0c-59f0-4a6c-a025-265363f98e77">
+         <span class="text-primary" id="10e62bfd-e038-4073-a94b-2aa54dae14f9">
           as_secondary
          </span>
         </h4>
-        <div id="ad07213f-f116-4617-9b7b-7fd2495b9e4f">
-         <button class="btn-sm btn btn-outline-primary" data-target="#86dc2e9e-4401-4783-9162-6af3dcac365e" data-toggle="collapse" id="443eebd1-41da-4e54-aacf-f8ed9c7f3fe1" onclick="return false;" type="button">
+        <div id="e5d23024-bdd1-4b32-8cb6-cf6c511be8f5">
+         <button class="btn-sm btn btn-outline-primary" data-target="#5200dd51-1b0b-43cc-a88f-2928d4b82caf" data-toggle="collapse" id="d3d3ff29-30b3-4756-aa06-a83a1fce7401" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="6d30cf1b-1024-4117-b111-66222e814ac1">
+       <span class="text-muted" id="c9f60c70-73b7-47bc-b33a-88134856a8ad">
         Makes the 'secondary' look to a web components.
        </span>
-       <pre id="b5699bf5-8fbc-46bf-9d17-7f4882c7b89a"><code class="python">as_secondary()</code></pre>
-       <div class="ml-3 collapse" id="86dc2e9e-4401-4783-9162-6af3dcac365e">
-        <h6 id="adc9e3ff-7080-4eb4-bcd9-28eb9cbff83b">
+       <pre id="c61c8108-c721-4212-b424-f940eaa4d86d"><code class="python">as_secondary()</code></pre>
+       <div class="ml-3 collapse" id="5200dd51-1b0b-43cc-a88f-2928d4b82caf">
+        <h6 id="4f190c1d-ab5b-4dd0-a199-8c18192639e4">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="0e4a0fcd-dcd2-4052-b698-2a133f5e3788">
+        <table class="table table-sm bg-light" id="0fe9e15b-0431-4a8f-970e-f004523a1730">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -2852,51 +2880,52 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="531db44b-be70-4615-a00f-7ca513742564">
-        <h6 id="0f0a6a7d-3a98-4491-8555-ddc8504c170c">
+       <div class="ml-3" id="2a199f31-76a7-49e6-bef0-293066f94865">
+        <h6 id="ae4161a3-31cf-492d-b59b-4123293bb935">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="2a1e5553-41c0-41a2-99df-e5964c3c8cc2"><code class="python">from bootwrap import Button
+        <pre id="9b8702ff-3cf4-42b1-8eea-289e5d11e7d4"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits AppearanceMixin.
-button = ("Secondary").as_secondary()</code></pre>
+button = ("Secondary").as_secondary()
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="74983ffc-a10e-48fc-85d7-25884acc3e93">
-       <div class="d-flex justify-content-between" id="427eea59-481e-483d-a2e7-55931e2393d9">
-        <h4 id="756350f3-cb9d-4544-b888-c43a54022102">
+      <div class="mt-5" id="2d715819-588e-48d8-b666-dbed5cc40cfe">
+       <div class="d-flex justify-content-between" id="30f619c2-d08c-43a5-ac48-f96b64a7dc87">
+        <h4 id="3d6af4d2-65ef-4b5e-bc5c-368a4e8e5114">
          Method
-         <span class="text-primary" id="502fa08f-43d2-4be3-800d-ff6330ef9b64">
+         <span class="text-primary" id="2784eb53-1542-451c-a040-71e1befae218">
           as_success
          </span>
         </h4>
-        <div id="eb0770d6-8032-4d6d-a9f0-da2a911aab6c">
-         <button class="btn-sm btn btn-outline-primary" data-target="#4f689330-237e-4458-ae77-5219256406d2" data-toggle="collapse" id="19ea09e4-8b19-4275-a8e3-90423c275b8e" onclick="return false;" type="button">
+        <div id="4121596c-4723-48f3-bcae-9d892e7d38dc">
+         <button class="btn-sm btn btn-outline-primary" data-target="#b2bc3c3d-ea6b-4027-9f1f-1144f63612b5" data-toggle="collapse" id="746a9341-8886-41e3-900a-55f12f4e93ed" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="6842c77d-1010-4ce3-9d2d-d88f4fe9134e">
+       <span class="text-muted" id="a79336e8-f76d-43f6-8d35-71069495a7b5">
         Makes the 'success' look to a web components.
        </span>
-       <pre id="aa28dd45-8d78-49bc-bd5e-98cce8abcb51"><code class="python">as_success()</code></pre>
-       <div class="ml-3 collapse" id="4f689330-237e-4458-ae77-5219256406d2">
-        <h6 id="23ffab48-81da-4f2a-a63e-754e2226c966">
+       <pre id="b8a1ff7f-40f8-43cd-bd42-c8b43b169f92"><code class="python">as_success()</code></pre>
+       <div class="ml-3 collapse" id="b2bc3c3d-ea6b-4027-9f1f-1144f63612b5">
+        <h6 id="ab7f493b-8a5d-461c-ad15-4f81448684c8">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="f07271ac-e8a1-4ad7-b0d1-0a3e92525a05">
+        <table class="table table-sm bg-light" id="7db3988c-0e20-4583-adae-24c5c10102ea">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -2921,51 +2950,52 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="6f7cbba5-8395-4604-a008-cd914d48a0e3">
-        <h6 id="8f6463f2-2d48-4218-9385-aad7a79e1748">
+       <div class="ml-3" id="276f6a44-e843-4743-9a1d-382d6a82a5a6">
+        <h6 id="5547fd6a-cdde-4b6d-bc7e-b852d38c0484">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="e03934fc-1369-4453-a093-0e7ad45108e2"><code class="python">from bootwrap import Button
+        <pre id="b67d7d73-f4d7-4fad-af9f-eab8542289f9"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits AppearanceMixin.
-button = ("Success").as_success()</code></pre>
+button = ("Success").as_success()
+</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="1774a277-1a05-4f6a-9ce5-5c21857ef219">
-       <div class="d-flex justify-content-between" id="0a27bef2-eaa3-4ec2-a86a-20cda5d1e1f5">
-        <h4 id="e200488f-733d-40de-ae5d-3139bd647fef">
+      <div class="mt-5" id="544842f9-8e22-48f0-9d4e-cee0c11ea352">
+       <div class="d-flex justify-content-between" id="3d235e89-af98-4df8-a9ad-0e6f2334731d">
+        <h4 id="352271fd-d5ed-438e-834a-79f6aa16b382">
          Method
-         <span class="text-primary" id="4b6a3949-1972-4a9c-a199-0942520780a7">
+         <span class="text-primary" id="03f37556-a451-4338-a2b1-4aa897952b9b">
           as_warning
          </span>
         </h4>
-        <div id="3ee416e6-1c9c-4281-9425-c9609c366031">
-         <button class="btn-sm btn btn-outline-primary" data-target="#58e2bd9f-fc71-4ec5-a443-fd460edddaf3" data-toggle="collapse" id="98871d96-80d4-4ae8-8a06-43ee0d0a134e" onclick="return false;" type="button">
+        <div id="b2afc3fb-509f-4cf2-bc37-2eb45c24519a">
+         <button class="btn-sm btn btn-outline-primary" data-target="#1a8f14c6-75b6-48b7-b2ec-a334941ddcfd" data-toggle="collapse" id="2b9a9401-9496-4f56-921c-b8996c2848fe" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="e471eee3-2e5e-4825-aea2-0b601d41fe0c">
+       <span class="text-muted" id="724ed52a-ac3c-4b3b-a25b-1da896498261">
         Makes the 'warning' look to a web components.
        </span>
-       <pre id="4ba542f0-994b-4d7b-8976-9d2f773bd04c"><code class="python">as_warning()</code></pre>
-       <div class="ml-3 collapse" id="58e2bd9f-fc71-4ec5-a443-fd460edddaf3">
-        <h6 id="74a02cd1-6aad-478d-9b2d-00987067723c">
+       <pre id="71e9a967-dcd4-42da-8f12-ea03e924209f"><code class="python">as_warning()</code></pre>
+       <div class="ml-3 collapse" id="1a8f14c6-75b6-48b7-b2ec-a334941ddcfd">
+        <h6 id="d3390d11-6476-40c0-aa35-b9af8a0ea41e">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="92e5325c-974f-450c-a8bc-0199bb59ad79">
+        <table class="table table-sm bg-light" id="59c3d283-102d-4bdb-9c69-384dfc4f1e09">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -2990,81 +3020,82 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="5246979e-deb2-4105-86f0-19a5520f4723">
-        <h6 id="904c314b-be81-41dc-b39c-e529f6252bbe">
+       <div class="ml-3" id="c98c5163-3b7a-483c-9a93-8016081f04e8">
+        <h6 id="e8354fe4-fed5-460d-be29-36a5277a3a57">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="2eba29d9-ad68-4fa8-b66c-ebc3a42952f6"><code class="python">from bootwrap import Button
+        <pre id="936ec580-3912-49aa-977d-47229ef5f83d"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits AppearanceMixin.
-button = ("Warning").as_warning()</code></pre>
+button = ("Warning").as_warning()
+</code></pre>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="d7783dd1-0b16-4963-95e8-2f5ba94d6a16">
-     <div class="mt-5" id="d9d2ab8f-4b02-4efc-84c8-c826f99f0157">
-      <div class="d-flex justify-content-between" id="2cbc321d-ef5c-4fb4-85ac-8ae384c05402">
-       <h1 id="549c0c86-e192-46ec-ae54-d53cc54cff0b">
+    <div class="tab-pane fade" id="43a7ec2a-2d5a-44a3-b992-0280967ce2cd">
+     <div class="mt-5" id="d265aee2-58b9-4fcb-adb4-cffba22c9a3b">
+      <div class="d-flex justify-content-between" id="470e4aef-e1ed-44eb-9597-c5591909f19f">
+       <h1 id="34de6e57-252d-456d-ad04-74dff146a84f">
         Class
-        <span class="text-primary" id="c3d70dac-30d1-4800-8f49-1dc84d38138a">
+        <span class="text-primary" id="4288ac97-7741-4899-99e2-9acd316e59df">
          OutlineMixin
         </span>
        </h1>
-       <div id="60db1800-b6cf-41ca-8331-089dd8dfda2d">
+       <div id="bcca7908-174c-474c-af89-d5eb76c523a1">
        </div>
       </div>
-      <span class="text-muted" id="bec30e90-1bfa-4c15-8c9e-6ae1cb9ca075">
+      <span class="text-muted" id="5a25b5ec-8efa-4d08-a9d3-29d2072817f1">
        Mixin for a web component that can be surrounded by a border.
       </span>
-      <pre id="001ef94d-b37b-4774-8c86-8fa279d3a313"><code class="python">OutlineMixin()</code></pre>
-      <p id="f3636b52-aa25-474d-bb19-8cd181639069">
+      <pre id="8301d2ff-d935-4bee-9b30-5e9b13ac884c"><code class="python">OutlineMixin()</code></pre>
+      <p id="553a737c-d673-4c09-a722-91d6dc7d3495">
        Usually
        <code>
         OutlineMixin
        </code>
        is used in conjunction with
        <code>
         AppearanceMixin
        </code>
        to
     specify the border appearance.
       </p>
-      <div class="mt-5" id="1b5cd59e-b5e5-4a03-beb9-c081532a0618">
-       <div class="d-flex justify-content-between" id="9933293c-b3cf-4624-8a1e-cc087984a930">
-        <h4 id="146d0f76-71ed-44c3-bad4-f0598c9f5f21">
+      <div class="mt-5" id="d0b660a8-11bc-408f-8a43-f5bd02907fe8">
+       <div class="d-flex justify-content-between" id="ee74ef08-fdc2-4926-96d0-7144848d3a0c">
+        <h4 id="cf6b811e-37c4-4d60-8755-0f796d31e4ac">
          Method
-         <span class="text-primary" id="87cddd72-4ce5-4fe3-9b01-a476c3370e5a">
+         <span class="text-primary" id="4715da91-150a-4577-94a4-1502f7247fa3">
           as_outline
          </span>
         </h4>
-        <div id="5b96cab5-ec9b-407e-b011-10d4bed2dd4b">
-         <button class="btn-sm btn btn-outline-primary" data-target="#b2b4f80f-c2ea-4dcc-b13d-150b0f50406f" data-toggle="collapse" id="ed3079dd-6cd9-4ab8-a39d-9413f49348ab" onclick="return false;" type="button">
+        <div id="0d5cb0bc-eb57-4c4f-977e-649a0ad20eb5">
+         <button class="btn-sm btn btn-outline-primary" data-target="#fcdad055-5646-4128-9c77-f2f7f8c7e3a4" data-toggle="collapse" id="62c127b1-7a17-4923-800f-a0b1c2bd93d5" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="ac7a8e9e-090e-44ff-ae3e-2dd36df02a4f">
+       <span class="text-muted" id="4be3fc24-7c0d-4792-83ee-e71be1234bdd">
         Makes the web component surrounded by a border.
        </span>
-       <pre id="7a3c7d5c-2a59-4e60-9757-56f33fa2706f"><code class="python">as_outline()</code></pre>
-       <div class="ml-3 collapse" id="b2b4f80f-c2ea-4dcc-b13d-150b0f50406f">
-        <h6 id="23c97942-3f08-41e9-9806-726afd782a16">
+       <pre id="fa67596c-de81-4fd6-9107-62a07d794608"><code class="python">as_outline()</code></pre>
+       <div class="ml-3 collapse" id="fcdad055-5646-4128-9c77-f2f7f8c7e3a4">
+        <h6 id="abb0e061-e7c6-45fe-8f81-deb306d2b437">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="44db34b9-9106-4939-ae32-38b67693212a">
+        <table class="table table-sm bg-light" id="8c519566-7ccf-443d-a137-34ffec637fc2">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -3089,73 +3120,74 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="e2b74278-d94d-4c21-85b5-28ade59d2aed">
-        <h6 id="33fe8f65-ca25-478e-86c2-8fabf4ab6558">
+       <div class="ml-3" id="47331edf-3d34-4e03-a701-ef6417c896df">
+        <h6 id="5bec8dbc-e23a-468a-a57f-eb94d782954d">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="067feb2f-9e5c-43b8-a9d9-534da0dff033"><code class="python">from bootwrap import Button
+        <pre id="b8f67a6f-5e2e-4e3d-ac2b-b4e7931ab5ce"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits AppearanceMixin.
-button = ("Primary").as_primary().as_outline()</code></pre>
+button = ("Primary").as_primary().as_outline()
+</code></pre>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="e3098ed6-7267-40d8-b65b-d8cba86578e7">
-     <div class="mt-5" id="ddc95f39-f1c1-451a-b28d-e613e4890b4f">
-      <div class="d-flex justify-content-between" id="a26e57fa-fa63-47e1-9b15-31958b4866f2">
-       <h1 id="404adf2f-aa98-472e-b8aa-72a11087c241">
+    <div class="tab-pane fade" id="2cdf283d-396b-4edc-b575-a87ffcef7d86">
+     <div class="mt-5" id="b2143754-f3df-4791-89a7-69ed453b3809">
+      <div class="d-flex justify-content-between" id="41d27945-73c2-467c-b73a-e75ac83c2507">
+       <h1 id="e73cfcfc-8617-4089-94e1-2168d3d9cf15">
         Class
-        <span class="text-primary" id="c755ffe8-6f23-4db9-b577-1fb62f7cce67">
+        <span class="text-primary" id="11ca59e1-cda5-4011-bbcc-0a42ea3fca08">
          AvailabilityMixin
         </span>
        </h1>
-       <div id="4631435a-c8e7-4b3e-b4fb-7ee1926bc177">
+       <div id="83b7b257-13c5-42ab-9866-50d61b39da3c">
        </div>
       </div>
-      <span class="text-muted" id="26306605-7604-4eb6-bbce-b9e20d6a6068">
+      <span class="text-muted" id="39467606-17a6-4acb-92fe-a2c5a9e1cf81">
        Mixin for a web component which can be enabled or disabled.
       </span>
-      <pre id="f97e1512-ffcb-4cea-bb71-8f2acbe15ff1"><code class="python">AvailabilityMixin()</code></pre>
-      <p id="568ce477-9695-4813-a2bc-2736ad5d8a18">
+      <pre id="7b32ae11-8b91-4330-b443-e14a06a6953c"><code class="python">AvailabilityMixin()</code></pre>
+      <p id="8c7b6ea3-9e99-48ba-b9b6-f009b36dca0b">
        By default, every web component is enabled. The web components inheriting
     this class can be forced to be disabled.
       </p>
-      <div class="mt-5" id="6b511b3a-43af-4c5a-bfe1-c9adb838cdce">
-       <div class="d-flex justify-content-between" id="94c8322b-4fd6-4691-b75f-6efd4fd06c40">
-        <h4 id="a6886323-69aa-45a3-83ce-f9fc71a6d3c5">
+      <div class="mt-5" id="d816b0d9-67de-4d2d-9599-585035212a46">
+       <div class="d-flex justify-content-between" id="86d3bb6a-e3b9-4518-bee7-3ee077148c49">
+        <h4 id="7e5a3c8a-6141-4a77-a080-b0347b7fb382">
          Method
-         <span class="text-primary" id="8861d305-20a5-46de-aaff-4f8cc9288493">
+         <span class="text-primary" id="8a56fb50-049e-4a36-8d6c-f5eb98decde1">
           as_disabled
          </span>
         </h4>
-        <div id="fb36114d-f5ca-4dea-8e0e-ee4849d5f899">
-         <button class="btn-sm btn btn-outline-primary" data-target="#dd473b03-dedb-4cb6-aa6b-a1f8d02c5101" data-toggle="collapse" id="ce920b94-5b22-49f9-aae2-ea2e5101026c" onclick="return false;" type="button">
+        <div id="8e82752e-0b24-4a90-bb6d-d37bfc427cc7">
+         <button class="btn-sm btn btn-outline-primary" data-target="#6566d826-8c76-45ab-b91c-7f9d3ce958c9" data-toggle="collapse" id="999174e6-7dae-4f47-b791-f71fd90d64b2" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="cf955a53-972e-44e4-9811-212918240ea9">
+       <span class="text-muted" id="9545e8d6-77e9-4c0f-8834-cd939efbeaf7">
         Disables a web component.
        </span>
-       <pre id="8acea71b-85d5-4c75-b6b1-8185590882b5"><code class="python">as_disabled()</code></pre>
-       <div class="ml-3 collapse" id="dd473b03-dedb-4cb6-aa6b-a1f8d02c5101">
-        <h6 id="2ba2e24b-c584-4202-ae40-fd038bf73b98">
+       <pre id="b81b5b45-bbec-4162-a83e-29375d79a25a"><code class="python">as_disabled()</code></pre>
+       <div class="ml-3 collapse" id="6566d826-8c76-45ab-b91c-7f9d3ce958c9">
+        <h6 id="6f40eb7f-ad0d-4578-a71e-ff0c97d0bc27">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="82d6f315-c79b-47d2-9f00-88e37ff9a611">
+        <table class="table table-sm bg-light" id="4c0c131a-c5ff-41e9-ae18-f0afca0c463b">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -3180,164 +3212,164 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="340d9721-e5d6-431b-a02e-87900205984a">
-        <h6 id="545b3682-c3c0-4df7-9a58-bc4fd26ce70b">
+       <div class="ml-3" id="96211a01-6692-487e-8179-e0e825520022">
+        <h6 id="78dcb993-4986-423b-8a7a-e63ad3587e4c">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="5e4fff21-0b02-43bb-8194-cf9bb8766423"><code class="python">from bootwrap import Button
+        <pre id="58207ca4-f776-433b-9bcc-c1490899e816"><code class="python">from bootwrap import Button
 
 # Note, that Button inherits AppearanceMixin.
-button = ("Primary").as_disabled()</code></pre>
+button = ("Primary").as_disabled()
+</code></pre>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="9b467775-d72a-4dbb-ba10-68aac76c2131">
-     <div id="d55e20ab-bdfa-481e-962f-bf7aa51bf931">
+    <div class="tab-pane fade" id="4ab49bce-83d3-40d0-8250-b4b63097fe19">
+     <div id="43dcfbcd-8831-4487-aeb7-b9371751dc86">
       <hr/>
-      <ul class="nav" id="979da39b-17c0-4128-b839-581afb00ca3a" role="tablist">
+      <ul class="nav" id="671c2c0a-2a05-4cd0-bdb5-2ccd485a21fe" role="tablist">
        <li class="nav-item">
-        <a class="nav-link active" data-target="#34f421bd-29f8-4189-aec8-4ab110cfb385" data-toggle="tab" href="#34f421bd-29f8-4189-aec8-4ab110cfb385" id="2fa97e1a-1797-499e-99bf-9fa33ad485bb" role="tab">
-         <span class="text-secondary" id="f6fc533b-f8d0-4e00-9b6e-4be51f389fff">
+        <a class="nav-link active" data-target="#5a27d164-f675-4e9a-b9b6-fd6b90340a12" data-toggle="tab" href="#5a27d164-f675-4e9a-b9b6-fd6b90340a12" id="1e0a847c-9160-4acc-955e-2f69e7279aa9" role="tab">
+         <span class="text-secondary" id="a0b42519-cb78-4ad8-9423-f2e71550f8cb">
           Breakpoint
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#3517f870-5cfe-4a07-862c-967897b96c60" data-toggle="tab" href="#3517f870-5cfe-4a07-862c-967897b96c60" id="c335057d-01da-463a-be17-7370e9896b93" role="tab">
-         <span class="text-secondary" id="d225bcad-73b3-450c-bad3-b6226a5bebf5">
+        <a class="nav-link" data-target="#1b1532c6-65c1-41c6-a4c3-3112034d1850" data-toggle="tab" href="#1b1532c6-65c1-41c6-a4c3-3112034d1850" id="dac6bbe0-9c71-45fc-905f-c467c1b10203" role="tab">
+         <span class="text-secondary" id="edfa23ea-9136-46d1-be85-eba0cdde075a">
           Action
          </span>
         </a>
        </li>
       </ul>
       <div class="tab-content">
-       <div class="tab-pane fade active show" id="34f421bd-29f8-4189-aec8-4ab110cfb385">
-        <div class="mt-5" id="a2412e7d-899a-4b22-b52a-24517b406f0e">
-         <div class="d-flex justify-content-between" id="03743e64-27f2-4b95-bcd6-e07280f3f946">
-          <h1 id="2a2483c2-1fc7-4013-8251-636a7c72d20b">
+       <div class="tab-pane fade active show" id="5a27d164-f675-4e9a-b9b6-fd6b90340a12">
+        <div class="mt-5" id="811f3946-d841-46a9-9f28-c49e436827ec">
+         <div class="d-flex justify-content-between" id="4b760fcc-fe37-4edc-bf1d-b04e82168e4d">
+          <h1 id="6ee685d5-dc94-4b9a-899e-342362c80128">
            Class
-           <span class="text-primary" id="acfe5402-cbda-4bdf-af81-8fe866336f91">
+           <span class="text-primary" id="b03e5cc5-e9ef-4b1e-ba9d-46d2812f824c">
             Breakpoint
            </span>
           </h1>
-          <div id="14c443fd-c499-4ad7-ae17-0e88573ab62a">
+          <div id="abc1341b-9645-4c93-bff3-3f1e877650bc">
           </div>
          </div>
-         <span class="text-muted" id="71433bb6-0299-410b-b6de-e16529e13151">
+         <span class="text-muted" id="73dd5c2a-4b57-4761-b10d-a9ee6161f131">
           The breakpoint constants.
          </span>
-         <p id="ebb230fb-03e6-4443-8c13-5269d3a07eaa">
+         <p id="46593039-3f88-4b07-bc6f-ca3388dee5db">
           Breakpoints are defined by Bootstrap and mostly based on minimum
     viewport widths and allow us to scale up elements as the viewport
     changes.
          </p>
-         <p id="6087ad38-4c50-4cdd-a87b-0b0fade39606">
+         <p id="a206fbde-f5f9-44dd-a62e-c1816fe7bb26">
           See
           <a href="https://getbootstrap.com/docs/4.0/layout/overview/#responsive-breakpoints">
-           Bootstrap documentation
+           for more information.
           </a>
-          for more information.
          </p>
-         <div id="c83d5552-1961-48eb-b41f-d83cc9d4b051">
+         <div id="09fd4306-9e7a-4309-ac94-c3ba3a9ff297">
           <div class="row">
            <div class="col-md">
-            <div class="p-1 m-1 border text-center" id="6554bb0b-23bc-4fc4-9cf6-a862c9cf9f58">
+            <div class="p-1 m-1 border text-center" id="42bcd2f6-3142-4bfd-9c11-358e5cd792dc">
              Breakpoint.
              <strong class="text-primary">
               LG
              </strong>
             </div>
            </div>
            <div class="col-md">
-            <div class="p-1 m-1 border text-center" id="0af0342b-c17f-47ec-b05f-0baceac9d8dd">
+            <div class="p-1 m-1 border text-center" id="78bbf7a3-13de-4395-a6dd-1bcf64d8b2e4">
              Breakpoint.
              <strong class="text-primary">
               MD
              </strong>
             </div>
            </div>
            <div class="col-md">
-            <div class="p-1 m-1 border text-center" id="77700f5a-b6f0-4a66-b2a3-6d07fc09b1c6">
+            <div class="p-1 m-1 border text-center" id="f7346137-4194-434e-9162-68db658310ea">
              Breakpoint.
              <strong class="text-primary">
               SM
              </strong>
             </div>
            </div>
            <div class="col-md">
-            <div class="p-1 m-1 border text-center" id="91d344af-6bd6-4402-9b78-7cad1b8072ee">
+            <div class="p-1 m-1 border text-center" id="fc664958-d99e-4bfa-8228-17f05dce1e2a">
              Breakpoint.
              <strong class="text-primary">
               XL
              </strong>
             </div>
            </div>
            <div class="col-md">
-            <div class="p-1 m-1 border text-center" id="c41c4ed6-a33d-49ce-83d7-a09354bb6e5d">
+            <div class="p-1 m-1 border text-center" id="a0192612-8ee0-4253-8e55-fd3ac344d993">
              Breakpoint.
              <strong class="text-primary">
               XS
              </strong>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="3517f870-5cfe-4a07-862c-967897b96c60">
-        <div class="mt-5" id="7598ca51-852a-4a1c-a3ef-446c4c736eb7">
-         <div class="d-flex justify-content-between" id="1591d659-d635-4183-bab6-1e42ca5437a9">
-          <h1 id="3c70843f-bd1e-4043-ac8d-1922b68ae99f">
+       <div class="tab-pane fade" id="1b1532c6-65c1-41c6-a4c3-3112034d1850">
+        <div class="mt-5" id="d121d06f-445d-4fba-b789-39c8286a37c9">
+         <div class="d-flex justify-content-between" id="7ec79e31-1ae9-4c46-a0d0-26796ee4545e">
+          <h1 id="5356e7c2-056a-4a08-b0ef-e710a334330e">
            Class
-           <span class="text-primary" id="ffa1a85d-3401-4c5a-845a-9fc29376494d">
+           <span class="text-primary" id="44a179c3-323d-4cdd-93dc-276fe7782831">
             Action
            </span>
           </h1>
-          <div id="7e03bb29-ac5e-49fd-80e0-cdaebb261019">
+          <div id="119513e6-47e7-4425-beab-008fe6a0de03">
           </div>
          </div>
-         <span class="text-muted" id="38a6cf35-5afc-4bbe-bdc4-2a24ecca73db">
+         <span class="text-muted" id="65309aca-0a06-4bf6-9ae9-30345fc6f0ed">
           The action constants.
          </span>
-         <div id="a1dcab7d-3eca-4451-b90f-7b0c394efb2b">
+         <div id="2f7d0e2a-2613-4aab-80ba-a5637ab7ed45">
           <div class="row">
            <div class="col-md">
-            <div class="p-1 m-1 border text-center" id="b5e9df99-6534-4d2f-a24c-bb7bd864d962">
+            <div class="p-1 m-1 border text-center" id="ac73981a-46cb-43bf-abf0-b40bc72915e2">
              Action.
              <strong class="text-primary">
               DISMISS
              </strong>
             </div>
            </div>
            <div class="col-md">
-            <div class="p-1 m-1 border text-center" id="e07fc2ab-203c-4af6-a8a5-a4c4103e198d">
+            <div class="p-1 m-1 border text-center" id="21efe207-a2fe-454a-b5f6-b50ad71226e0">
              Action.
              <strong class="text-primary">
               LINK
              </strong>
             </div>
            </div>
            <div class="col-md">
-            <div class="p-1 m-1 border text-center" id="e5ddcaa1-ea80-4d4c-a88b-4eba46b5c8a5">
+            <div class="p-1 m-1 border text-center" id="590c848c-21c1-4720-b751-4fca90f2b8a6">
              Action.
              <strong class="text-primary">
               SUBMIT
              </strong>
             </div>
            </div>
            <div class="col-md">
-            <div class="p-1 m-1 border text-center" id="745105d9-4490-4fa2-98dc-66f0a64c2ca7">
+            <div class="p-1 m-1 border text-center" id="95920e8c-1c7c-4f9b-b4c7-1c22ecf32350">
              Action.
              <strong class="text-primary">
               TOGGLE
              </strong>
             </div>
            </div>
           </div>
@@ -3349,8 +3381,11 @@
     </div>
    </div>
   </div>
  </body>
  <script>
   hljs.initHighlightingOnLoad();
  </script>
+ <style>
+  :root{--container-margin-top: 90px}html{  width: 100%;  height: 100%; }  body{  background-color: var(--body-background-color);  background-image: var(--body-background-image);  background-position: var(--body-background-position);  background-size: var(--body-background-size);  -webkit-background-size: var(--body-background-size);  -moz-background-size: var(--body-background-size);  -o-background-size: var(--body-background-size);  background-repeat: var(--body-background-repeat);  background-origin: var(--body-background-origin);  background-clip: var(--body-background-clip);  background-attachment: var(--body-background-attachment); }  .container-fluid{  margin-top: var(--container-margin-top); }  .auth{  width: 400px;  margin-top: 150px }  @media only screen and (max-width: 420px){  body{  background-image: none;  }   .auth{  width: 100%;  margin-top: 0px  } }  .grid-container {  display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); }  .card {  margin-top: 10px; }
+ </style>
 </html>
```

#### html2text {}

```diff
@@ -509,15 +509,15 @@
 ===============================================================================
     * _B_r_e_a_k_p_o_i_n_t
     * _A_c_t_i_o_n
 ************ CCllaassss BBrreeaakkppooiinntt ************
 The breakpoint constants.
 Breakpoints are defined by Bootstrap and mostly based on minimum viewport
 widths and allow us to scale up elements as the viewport changes.
-See _B_o_o_t_s_t_r_a_p_ _d_o_c_u_m_e_n_t_a_t_i_o_n_ for more information.
+See _f_o_r_ _m_o_r_e_ _i_n_f_o_r_m_a_t_i_o_n_.
 Breakpoint. LLGG
 Breakpoint. MMDD
 Breakpoint. SSMM
 Breakpoint. XXLL
 Breakpoint. XXSS
 ************ CCllaassss AAccttiioonn ************
 The action constants.
```

### Comparing `bootwrap-1.0.0/docs/components.html` & `bootwrap-1.0.1/docs/components.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!DOCTYPE html>
 <html lang="en">
  <head>
   <meta charset="utf-8"/>
-  <meta container="width=device-width, initial-scale=1,
+  <meta content="width=device-width, initial-scale=1,
                         shrink-to-fit=no" name="viewport"/>
   <link href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" rel="stylesheet" type="text/css"/>
   <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.8.2/css/all.min.css" rel="stylesheet" type="text/css"/>
   <link href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.5.0/styles/default.min.css" rel="stylesheet" type="text/css"/>
   <link href="favicon.ico" rel="icon" type="image/x-icon"/>
   <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.0/jquery.min.js" type="application/javascript">
   </script>
@@ -17,210 +17,210 @@
   <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.5.0/highlight.min.js" type="application/javascript">
   </script>
   <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.5.0/languages/python.min.js" type="application/javascript">
   </script>
  </head>
  <body>
   <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
-   <img alt="Bootwrap Logo" id="2cded683-d036-4eb8-bc76-265b2dad9c75" src="logo.png" width="32"/>
-   <span class="text-light" id="f4b974be-de5a-4e74-9a26-7c82841ab12e">
+   <img alt="Bootwrap Logo" id="10cc1b55-2061-4953-9105-2e45da609fd8" src="logo.png" width="32"/>
+   <span class="text-light" id="e099c105-f1a7-4db2-b39e-beb2b450890b">
     <strong>
      Bootwrap
     </strong>
    </span>
    <button aria-controls="menu" aria-expanded="false" aria-label="Toggle menu" class="navbar-toggler" data-target="#menu" data-toggle="collapse" type="button">
     <span class="navbar-toggler-icon">
     </span>
    </button>
    <div class="collapse navbar-collapse" id="menu">
     <ul class="navbar-nav mr-auto">
      <li class="nav-item">
-      <a class="ml-2 nav-link" href="index.html" id="5fe73361-f3f4-496c-b02f-d7c4b36fc35a">
+      <a class="ml-2 nav-link" href="index.html" id="b10e7e46-32e7-4fee-b619-904a14f2d409">
        Home
       </a>
      </li>
      <li class="nav-item">
-      <a class="ml-2 nav-link" href="layout.html" id="b25861e4-2f7e-4983-81ce-0272f029d7a5">
+      <a class="ml-2 nav-link" href="layout.html" id="c086a6c8-9ade-427f-b155-d92b43c64636">
        Layout
       </a>
      </li>
      <li class="nav-item">
-      <a class="ml-2 nav-link" href="base.html" id="bef45985-2f73-49b4-9999-fa6d5e05ad95">
+      <a class="ml-2 nav-link" href="base.html" id="5cd10e89-c6b3-4747-b43e-ff301aa9781b">
        Base
       </a>
      </li>
      <li class="nav-item">
-      <a class="ml-2 nav-link" href="components.html" id="ed497c99-55d4-40d2-ba1f-08f7c6e3a17b">
+      <a class="ml-2 nav-link" href="components.html" id="8b77e024-9cbe-4f65-b011-ec583b990efe">
        Components
       </a>
      </li>
     </ul>
-    <a class="ml-2 btn btn-outline-light" href="https://github.com/mmgalushka/bootwrap" id="259d907a-ee91-4419-b56d-461cd05ac7cf" role="button">
+    <a class="ml-2 btn btn-outline-light" href="https://github.com/mmgalushka/bootwrap" id="a6bded64-87a8-4755-8356-207ae963119c" role="button">
      GitHub
     </a>
    </div>
   </nav>
-  <div class="container" style="margin-top: 90px;">
-   <ul class="nav nav-pills" id="18eb987e-e782-4654-befe-ca43ae4727d9" role="tablist">
+  <div class="container-fluid">
+   <ul class="nav nav-pills" id="45c408e7-f56c-47f7-aa50-7d1cb364cceb" role="tablist">
     <li class="nav-item">
-     <a class="nav-link active" data-target="#61939bef-fbad-4176-9bb1-a4eb96030217" data-toggle="tab" href="#61939bef-fbad-4176-9bb1-a4eb96030217" id="d3cec24a-47ed-4b09-9d64-e96259caa7c0" role="tab">
+     <a class="nav-link active" data-target="#062c339e-3064-47f9-b1ce-39f7ab2967f3" data-toggle="tab" href="#062c339e-3064-47f9-b1ce-39f7ab2967f3" id="037bd5cb-4c88-4fd9-8712-c211ebba5c41" role="tab">
       Anchor
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#dbe831ae-15e3-460e-ab29-5cc4f0d82416" data-toggle="tab" href="#dbe831ae-15e3-460e-ab29-5cc4f0d82416" id="6762c87b-fa91-4d27-b465-55a5c736ab62" role="tab">
+     <a class="nav-link" data-target="#528aad1b-691d-4637-8b4a-58482729b51e" data-toggle="tab" href="#528aad1b-691d-4637-8b4a-58482729b51e" id="bbbf2a3d-1ad7-4885-95a0-7459f659ef03" role="tab">
       Badge
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#244d5aa9-7a2d-4332-8373-5b0987e7d08d" data-toggle="tab" href="#244d5aa9-7a2d-4332-8373-5b0987e7d08d" id="513741d1-d464-4f40-81d8-b43c840e565c" role="tab">
+     <a class="nav-link" data-target="#5be43bd9-e0c2-4145-816e-bd5f0c5aea59" data-toggle="tab" href="#5be43bd9-e0c2-4145-816e-bd5f0c5aea59" id="a0f2f7f0-6ddc-48f8-abf8-9e0c839e96e5" role="tab">
       Button
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#347e8840-54b9-4441-b8bd-9eeff202ea41" data-toggle="tab" href="#347e8840-54b9-4441-b8bd-9eeff202ea41" id="6b7566c6-7aea-4aa7-b5dd-8e32b8ff97a2" role="tab">
+     <a class="nav-link" data-target="#5f884099-12db-4603-8dd0-1dd887e53bc7" data-toggle="tab" href="#5f884099-12db-4603-8dd0-1dd887e53bc7" id="14fbbdc5-c310-4339-aa6d-66f08de67460" role="tab">
       Deck
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#f3fe07ea-df57-44b0-9175-c6ca9aa01de6" data-toggle="tab" href="#f3fe07ea-df57-44b0-9175-c6ca9aa01de6" id="e1bc3380-340f-44b1-99de-e1b60ea0e13c" role="tab">
+     <a class="nav-link" data-target="#3f8a4e63-08fe-44c1-9d8d-0b3f12c00fb7" data-toggle="tab" href="#3f8a4e63-08fe-44c1-9d8d-0b3f12c00fb7" id="046c16e3-cdf2-4178-ba99-3dbff0176995" role="tab">
       Dialog
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#f4a2e903-d7f8-4a64-93b9-85647e31031f" data-toggle="tab" href="#f4a2e903-d7f8-4a64-93b9-85647e31031f" id="dc69b2ac-2a0f-4dfe-ac28-0c4cc357fe3b" role="tab">
+     <a class="nav-link" data-target="#4809de16-7c3c-4c28-9093-69b35698e4ce" data-toggle="tab" href="#4809de16-7c3c-4c28-9093-69b35698e4ce" id="2470dac6-1f63-45a5-9276-36d7e2d40fd6" role="tab">
       Form
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#f0970b4c-6f15-48d3-9246-d8d245af3e57" data-toggle="tab" href="#f0970b4c-6f15-48d3-9246-d8d245af3e57" id="e6677fb4-0df8-4189-9174-444ca3e39498" role="tab">
+     <a class="nav-link" data-target="#4793739d-4728-4d95-a8e8-324923a67504" data-toggle="tab" href="#4793739d-4728-4d95-a8e8-324923a67504" id="7711c3fb-dab7-430e-ae49-9d7cf53a216c" role="tab">
       Icon
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#b352e040-ea7d-49e4-bb59-511ba97910dc" data-toggle="tab" href="#b352e040-ea7d-49e4-bb59-511ba97910dc" id="0a6f9f17-9f38-4b1f-b481-2f16c31770aa" role="tab">
+     <a class="nav-link" data-target="#5a85ba07-f6ac-42e5-a6e7-472caf5cd771" data-toggle="tab" href="#5a85ba07-f6ac-42e5-a6e7-472caf5cd771" id="1a8dc15b-ddf2-4eb4-a0ec-d5e8feb488cd" role="tab">
       Image
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#cd637315-f984-4528-a9e2-3a5a1c7d0f82" data-toggle="tab" href="#cd637315-f984-4528-a9e2-3a5a1c7d0f82" id="413efc8c-ad09-40df-a2e3-4ecae2c0c7dd" role="tab">
+     <a class="nav-link" data-target="#f70d9d6c-0f05-4f07-a4ca-2a50856faa9b" data-toggle="tab" href="#f70d9d6c-0f05-4f07-a4ca-2a50856faa9b" id="c70c67f3-bfe9-4163-ab55-79cf52c66182" role="tab">
       Javascript
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#b7b7831a-01df-4d41-b689-dc81d94581b5" data-toggle="tab" href="#b7b7831a-01df-4d41-b689-dc81d94581b5" id="2db73db7-3225-43dd-8a23-1a4d80710728" role="tab">
+     <a class="nav-link" data-target="#124666c1-23fd-47c4-bf7c-e3a88ef242d3" data-toggle="tab" href="#124666c1-23fd-47c4-bf7c-e3a88ef242d3" id="854ccd6e-a179-4870-a244-d70402cbdbb4" role="tab">
       Link
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#53f05ef7-9272-4e4e-b02d-ab119d10972f" data-toggle="tab" href="#53f05ef7-9272-4e4e-b02d-ab119d10972f" id="a5e5dad5-89b0-4d0b-aceb-f6c1706ab9a0" role="tab">
+     <a class="nav-link" data-target="#8e2eb34a-4f9e-4d8b-9754-6dd7a2eb2aea" data-toggle="tab" href="#8e2eb34a-4f9e-4d8b-9754-6dd7a2eb2aea" id="f25e9278-d4ef-4b38-aabe-66440108b8ac" role="tab">
       List
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#38b3263d-faca-45ad-922d-44f57f4e893b" data-toggle="tab" href="#38b3263d-faca-45ad-922d-44f57f4e893b" id="66845fd4-15de-4439-b0a8-16db2244ec06" role="tab">
+     <a class="nav-link" data-target="#2e0eddbe-00fc-4f38-ac91-e546f0ed51fe" data-toggle="tab" href="#2e0eddbe-00fc-4f38-ac91-e546f0ed51fe" id="25c867c2-88e2-4a51-878b-e0d2b223d9ea" role="tab">
       Navigation
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#bfe157cf-f2ed-4ea9-bcf1-4ef6d300462f" data-toggle="tab" href="#bfe157cf-f2ed-4ea9-bcf1-4ef6d300462f" id="2c507a23-0462-4da8-a53a-dae884bb7445" role="tab">
+     <a class="nav-link" data-target="#f7091e9c-ac2e-41c2-99ac-4022059d7445" data-toggle="tab" href="#f7091e9c-ac2e-41c2-99ac-4022059d7445" id="61188d84-dcba-4a9a-8504-7a2d9cb917e8" role="tab">
       Panel
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#6dc2e0f8-dd9b-4e2f-ad92-c8c98acc78d8" data-toggle="tab" href="#6dc2e0f8-dd9b-4e2f-ad92-c8c98acc78d8" id="8895eabd-1ee7-4ebf-8aa6-23378fec6e99" role="tab">
+     <a class="nav-link" data-target="#5dff1a6c-3836-464a-9083-5f34c8806812" data-toggle="tab" href="#5dff1a6c-3836-464a-9083-5f34c8806812" id="2eb5084a-c40b-4a84-a53d-4edb9b788a46" role="tab">
       Separator
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#3dfa68b6-c865-4f48-9383-91ffdadc3312" data-toggle="tab" href="#3dfa68b6-c865-4f48-9383-91ffdadc3312" id="f8fd8903-81cc-4c26-8e58-d699b5677ba6" role="tab">
+     <a class="nav-link" data-target="#b123cf21-44bd-42fe-97e2-17d6c9e47217" data-toggle="tab" href="#b123cf21-44bd-42fe-97e2-17d6c9e47217" id="08fde468-7a7e-4fdc-8297-1c14299ac6f1" role="tab">
       Table
      </a>
     </li>
     <li class="nav-item">
-     <a class="nav-link" data-target="#ea7d5a24-6909-4527-96c9-1333b9dd6d5b" data-toggle="tab" href="#ea7d5a24-6909-4527-96c9-1333b9dd6d5b" id="73b8d037-0c64-42e8-9740-24deed7223e0" role="tab">
+     <a class="nav-link" data-target="#d1653cdc-cb70-47ca-a06f-cfb4fde1e2b3" data-toggle="tab" href="#d1653cdc-cb70-47ca-a06f-cfb4fde1e2b3" id="e1bd3edb-ff10-4d3c-88c0-15de1c94fe09" role="tab">
       Text
      </a>
     </li>
    </ul>
    <div class="tab-content">
-    <div class="tab-pane fade active show" id="61939bef-fbad-4176-9bb1-a4eb96030217">
-     <div id="3bb2fd2b-aafb-4382-9b5b-77a096ac1cee">
+    <div class="tab-pane fade active show" id="062c339e-3064-47f9-b1ce-39f7ab2967f3">
+     <div id="c12ac5b2-5f87-4520-aeb6-f738f7e9f8d6">
       <hr/>
-      <ul class="nav" id="f415ee1f-7306-47c1-8b36-e83f0ffedfb4" role="tablist">
+      <ul class="nav" id="2f2a5d4e-4048-44e8-a7db-f2f7ee4548f9" role="tablist">
        <li class="nav-item">
-        <a class="nav-link active" data-target="#3b65705a-07ac-4c99-9f91-3b0a5b7a6c52" data-toggle="tab" href="#3b65705a-07ac-4c99-9f91-3b0a5b7a6c52" id="1986480d-b976-4542-9fc5-3166a8d381b5" role="tab">
-         <span class="text-secondary" id="7381c148-6046-4d74-8b05-6b374077ed0b">
+        <a class="nav-link active" data-target="#e353fea6-cb7c-401c-aeef-c6cfc3140f77" data-toggle="tab" href="#e353fea6-cb7c-401c-aeef-c6cfc3140f77" id="5f214bf6-9640-4e67-9be5-ebf3cd3fe639" role="tab">
+         <span class="text-secondary" id="8c510fc4-0c11-45ff-9c77-823d9dde9366">
           Anchor
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#d145ff15-f694-4634-8804-abadd0b39bef" data-toggle="tab" href="#d145ff15-f694-4634-8804-abadd0b39bef" id="ef9f5321-3c1b-45b0-80cc-33040525b478" role="tab">
-         <span class="text-secondary" id="cf505ec1-b3ad-4813-9651-8309e9d32133">
+        <a class="nav-link" data-target="#433909fd-d198-4f7b-bcef-9233a35470c3" data-toggle="tab" href="#433909fd-d198-4f7b-bcef-9233a35470c3" id="d26df2b1-5159-4568-9871-fc609f2acd73" role="tab">
+         <span class="text-secondary" id="2364346a-b14d-4e07-8f3b-b1905f4668c4">
           Appearance
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#ab1b886c-e498-4df0-a904-57f1f3158948" data-toggle="tab" href="#ab1b886c-e498-4df0-a904-57f1f3158948" id="ce6d35a1-ab9f-4b8b-b01d-07dbfbf48164" role="tab">
-         <span class="text-secondary" id="b309b447-b8ec-48e9-aba7-55ac0e477247">
+        <a class="nav-link" data-target="#4903d153-8507-469b-88fd-38e9747e7e15" data-toggle="tab" href="#4903d153-8507-469b-88fd-38e9747e7e15" id="8a9dce9c-4a12-4907-9619-e7f13fe882e5" role="tab">
+         <span class="text-secondary" id="92e34303-9a74-40bf-884a-7a9303956181">
           Link Resource
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#105f43b7-fb85-45c8-aebb-a50a6c2e0126" data-toggle="tab" href="#105f43b7-fb85-45c8-aebb-a50a6c2e0126" id="9087bb00-c566-493f-b06a-109f9a4d6112" role="tab">
-         <span class="text-secondary" id="e7c7c825-70b3-4de6-a463-9cee85a0d37f">
+        <a class="nav-link" data-target="#ca8d51d0-0c9c-4d73-9297-126011de6074" data-toggle="tab" href="#ca8d51d0-0c9c-4d73-9297-126011de6074" id="bdc77f8d-7848-4aaf-b40d-9ae0c4f80787" role="tab">
+         <span class="text-secondary" id="c6c0f001-beab-454f-afab-d4b61a6720f4">
           Open Dialog
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#c0152c9a-bb26-493e-912c-586c2dea445a" data-toggle="tab" href="#c0152c9a-bb26-493e-912c-586c2dea445a" id="da131f7f-0cc2-43e2-8461-5dbbf28c8af5" role="tab">
-         <span class="text-secondary" id="ee11b877-6a67-4230-9fa3-7e85120dd909">
+        <a class="nav-link" data-target="#7a81a75a-62b0-42bd-80ad-ff1a4281bef5" data-toggle="tab" href="#7a81a75a-62b0-42bd-80ad-ff1a4281bef5" id="c049a768-3f37-4716-aa8b-4edd547ada14" role="tab">
+         <span class="text-secondary" id="9efee550-46fc-4819-8ef3-42df4f22dd1d">
           Close Dialog
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#0c812bd2-06ab-4af6-b393-15e5c235ca84" data-toggle="tab" href="#0c812bd2-06ab-4af6-b393-15e5c235ca84" id="c9764ab8-f2e0-4db4-86fb-380dd308c280" role="tab">
-         <span class="text-secondary" id="5bcf2f13-8473-4d6a-adba-a776ebd6f2c2">
+        <a class="nav-link" data-target="#02f70fee-f643-4a6a-9e25-b26aeb334ca8" data-toggle="tab" href="#02f70fee-f643-4a6a-9e25-b26aeb334ca8" id="bc9594ed-16ab-4143-8de7-a6f505365adc" role="tab">
+         <span class="text-secondary" id="36854035-2b3f-4ee0-a534-d0da2d9fa0fe">
           Expand/Collapse Panel
          </span>
         </a>
        </li>
       </ul>
       <div class="tab-content">
-       <div class="tab-pane fade active show" id="3b65705a-07ac-4c99-9f91-3b0a5b7a6c52">
-        <div class="mt-5" id="3121c515-349e-486d-983f-192935c0b81e">
-         <div class="d-flex justify-content-between" id="76341b0f-57f8-4172-8a12-fc9d6e0d1d1d">
-          <h1 id="fe24697c-e77d-4241-bbb5-259dcaecc7e8">
+       <div class="tab-pane fade active show" id="e353fea6-cb7c-401c-aeef-c6cfc3140f77">
+        <div class="mt-5" id="ff532b23-aeca-4a4b-a5cf-8da587df3521">
+         <div class="d-flex justify-content-between" id="a476a815-c1f1-4ef4-b86a-23f6423fdc92">
+          <h1 id="a390dda0-ec98-4d77-a2c4-b4f8e7d06501">
            Class
-           <span class="text-primary" id="485f2e15-f022-4047-af49-7d023d942704">
+           <span class="text-primary" id="76a0138c-ff9c-4342-b3f4-5a5811748b4f">
             Anchor
            </span>
           </h1>
-          <div id="3e3a1339-b26a-4a7a-bdc9-f85054b931d4">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#689c8350-d812-4009-a02f-0ef3a349c35a" data-toggle="collapse" id="34751c7a-63e8-4a13-9c47-37cd25412b34" onclick="return false;" type="button">
+          <div id="cbe060d5-6d70-4ddb-8292-f91f942b9683">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#fb671360-8871-44f0-860a-fec10e4ac6e1" data-toggle="collapse" id="d8c01641-0ad1-4f83-a457-327971b38513" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="9a7aad2f-b03c-43f5-b4df-02d630547df9">
+         <span class="text-muted" id="755a04be-3263-475f-8b3d-11ce10cab26d">
           A web component for an anchor.
          </span>
-         <pre id="bf9461b8-cd6b-4407-885e-0cdc33851c05"><code class="python">Anchor(inner=None)</code></pre>
-         <div class="ml-3 collapse" id="689c8350-d812-4009-a02f-0ef3a349c35a">
-          <h6 id="0f4ad767-88c3-46cf-bdca-a6ceaa6867a4">
+         <pre id="3ad8b6cb-da03-446c-a224-f1f70abeeaad"><code class="python">Anchor(inner=None)</code></pre>
+         <div class="ml-3 collapse" id="fb671360-8871-44f0-860a-fec10e4ac6e1">
+          <h6 id="60acf5fd-edef-48ac-bb94-42e1bc2ade4e">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="3f2821f2-016c-47ea-b310-b12b5b979cc1">
+          <table class="table table-sm bg-light" id="aa3d92d2-3a56-46ec-8178-84303b33b686">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -245,15 +245,15 @@
              <td>
               The object wrapped by the anchor.
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <p id="16123638-a03b-4861-9881-ab0d9633305e">
+         <p id="e3937a25-0507-49b1-9d2e-3b259e3d1cd4">
           The
           <code>
            Anchor
           </code>
           component is used for creating a hyperlink to pages, files,
     email addresses, locations on the same page, or other web-resources
     defined by a URL address. The
@@ -264,51 +264,53 @@
           <code>
            Anchor
           </code>
           in
     conjunction with other components, for example, in creating a navigation
     menu.
          </p>
-         <div class="ml-3" id="25cc690b-e848-457b-b972-8aac21e6cca9">
-          <h6 id="78e98269-6a05-460d-889c-74bd78f57127">
+         <div class="ml-3" id="304518b9-7dd6-41d3-a8f9-ef8e22d9164b">
+          <h6 id="dffc6546-a813-48a4-8a3d-9f1afc755b25">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="7d750e96-e696-4336-bb1d-35cd6bb53f85"><code class="python">Anchor('Google Search').link('https://www.google.com/')</code></pre>
+          <pre id="673baa42-f219-46d7-9793-68941c7dcd67"><code class="python">from bootwrap import Anchor
+Anchor('Google Search').link('https://www.google.com/')
+</code></pre>
          </div>
-         <div class="ml-3" id="4d0b8695-0cc8-407a-9cf4-0ec4caca69ab">
-          <a href="https://www.google.com/" id="abd63873-15ec-4f80-957a-9e30f4bbb4c0">
+         <div class="ml-3" id="01a73a5c-997c-47ff-a185-ee6e0f7d228d">
+          <a href="https://www.google.com/" id="fe1d1c4b-741f-4784-9384-dc63ad7c6c90">
            Google Search
           </a>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="d145ff15-f694-4634-8804-abadd0b39bef">
-        <div class="mt-3" id="d63855b5-62ed-4072-b4d1-6af1cfb9d100">
-         <div id="fa9a07f2-77a0-4124-b8da-cd9ed5db8b1b">
+       <div class="tab-pane fade" id="433909fd-d198-4f7b-bcef-9233a35470c3">
+        <div class="mt-3" id="c4057299-17fc-463b-a2e6-4e2e69c7c54c">
+         <div id="2b8c3e71-3056-4c08-b338-fe0769aa0646">
           <div class="row">
            <div class="col-md">
-            <div id="eb9214e1-307c-42d6-865e-62987a7783ab">
-             <h1 id="c1b1dfa4-ae3f-4204-8fb2-2b475d2e4281">
+            <div id="faba9bed-e38f-43f9-b106-92239b79bce9">
+             <h1 id="b070b712-bda9-42aa-8bfd-db2d32f04d38">
               Appearance
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="b762be8e-9060-4c81-b19c-a80f467a73f3">
+            <div id="4e5631cf-b908-424c-93e4-48eb5c6103aa">
             </div>
            </div>
           </div>
          </div>
-         <div id="5fe2e9bf-5f7d-4fca-8984-016f7fcf7faf">
+         <div id="823a9f26-c772-4ee1-811c-b4f01370c60b">
           <div class="row">
            <div class="col-md">
-            <div id="c421e91f-731f-4f63-ae24-b84ceec31989">
-             <p id="665b2040-c18a-43a5-b53e-16ab2b39123c">
+            <div id="06fe5717-b654-466d-b7e7-ef8e24d1cb15">
+             <p id="6364dcfd-72b9-44e8-ae1e-7e2f2cb5cfa6">
               Change
               <code>
                Anchor
               </code>
               appearance using the following functions
               <code>
                as_primary()
@@ -342,146 +344,157 @@
                as_dark()
               </code>
               .
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="4c026b10-0941-49eb-8ee0-32ca75680dc2">
-             <pre id="6cc5b67c-6684-4a56-a1c1-e4798c70a83f"><code class="python">Anchor("Primary").as_primary()
-Anchor("Secondary").as_secondary()
-Anchor("Success").as_success()
-Anchor("Warning").as_warning()
-Anchor("Danger").as_danger()
-Anchor("Info").as_info()
-Anchor("Light").as_light()
-Anchor("Dark").as_dark()</code></pre>
-             <div id="facce678-de04-45b5-8ba6-002f78c2cbba">
-              <a class="mb-1 text-primary" href="#" id="cfbf0478-72ec-484e-b176-4f5be07353b6">
+            <div id="9c25f000-2140-4208-a74a-1a9452400760">
+             <pre id="88f0f90d-9733-4da8-bcb6-54b3ff65706d"><code class="python">from bootwrap import Panel, Anchor
+panel = Panel(
+  Anchor("Primary").link("#").as_primary(),
+  Anchor("Secondary").link("#").as_secondary(),
+  Anchor("Success").link("#").as_success(),
+  Anchor("Warning").link("#").as_warning(),
+  Anchor("Danger").link("#").as_danger(),
+  Anchor("Info").link("#").as_info(),
+  Anchor("Light").link("#").as_light(),
+  Anchor("Dark").link("#").as_dark()
+)
+for anchor in panel:
+  anchor.mb(1)
+panel</code></pre>
+             <div id="a5e42e48-89b9-4a2d-89ce-ce9ee9575268">
+              <a class="mb-1 text-primary" href="#" id="3dfbde10-00be-48de-beba-0f67d6fc2268">
                Primary
               </a>
-              <a class="mb-1 text-secondary" href="#" id="e3e9282a-f7cf-4409-b0fe-01f8308fb383">
+              <a class="mb-1 text-secondary" href="#" id="caff53d7-66b8-44e3-9eee-4c7a8a9fbcf9">
                Secondary
               </a>
-              <a class="mb-1 text-success" href="#" id="0231b790-e0d6-4eb8-9411-4b95b02e7d4f">
+              <a class="mb-1 text-success" href="#" id="82637482-75c9-4347-8c8f-9214b149aa41">
                Success
               </a>
-              <a class="mb-1 text-warning" href="#" id="1233b389-76eb-4231-9445-f89a6c5427fc">
+              <a class="mb-1 text-warning" href="#" id="b1129be8-9c82-4812-99ea-02d8fb590e40">
                Warning
               </a>
-              <a class="mb-1 text-danger" href="#" id="ab81b868-3120-4e8d-acf6-a51df2dc8db8">
+              <a class="mb-1 text-danger" href="#" id="9ab34d67-9b18-4200-846a-a8d28f681552">
                Danger
               </a>
-              <a class="mb-1 text-info" href="#" id="d89fd57d-fbf6-4bcd-a521-3a47ccf34cbf">
+              <a class="mb-1 text-info" href="#" id="39fc991b-45d0-45be-ba41-13a751f0f192">
                Info
               </a>
-              <a class="mb-1 text-light" href="#" id="b74f7433-609a-45cd-aedc-14b31edb52ce">
+              <a class="mb-1 text-light" href="#" id="40a1cdad-1046-42b4-9ceb-5269d631651c">
                Light
               </a>
-              <a class="mb-1 text-dark" href="#" id="a3bc9124-c3c9-480d-86b7-91de17800980">
+              <a class="mb-1 text-dark" href="#" id="081a33f0-ccf2-40cb-a842-976680373211">
                Dark
               </a>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="ab1b886c-e498-4df0-a904-57f1f3158948">
-        <div class="mt-3" id="6f236b38-e260-4aec-ae56-7ef36d35d8cf">
-         <div id="74f9a07c-5304-4bcb-bffe-6bfd2df73350">
+       <div class="tab-pane fade" id="4903d153-8507-469b-88fd-38e9747e7e15">
+        <div class="mt-3" id="e1181116-b646-40d8-aeea-56453e2b7b6c">
+         <div id="3d78b8da-9145-4432-ac84-787c0ab91106">
           <div class="row">
            <div class="col-md">
-            <div id="d28fa9ea-76f0-4895-b93c-35a6b7ed1e4b">
-             <h1 id="bb1744cf-2dba-48bd-bb3a-8cc97dbee4d0">
+            <div id="c4fce8d2-bdfa-4cee-b7ed-e82b179ac91e">
+             <h1 id="79e1345b-8a28-45ed-9faa-17cf77862a45">
               Link Resource
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="b1321bca-e4c2-4be7-a491-55f806a7a7cf">
+            <div id="c4c60814-4f43-46c2-9121-6c1886f4eefd">
             </div>
            </div>
           </div>
          </div>
-         <div id="d5f2514d-0a91-4694-90fd-d0ab5d8eda7d">
+         <div id="47f369c5-57aa-4bba-a21a-32318856dc76">
           <div class="row">
            <div class="col-md">
-            <div id="9f3d4ff8-68a6-4e56-9de1-f327b9ee3a53">
-             <p id="c291cbf2-c67c-459b-aa8f-303a280aa26c">
+            <div id="914906ff-d4c1-47db-a86d-8557252d11c8">
+             <p id="7449b4f2-06fc-49c0-aafe-e22603c74269">
               Associate
               <code>
                Anchor
               </code>
               with a hyperlink using the
               <code>
                link()
               </code>
               function.
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="e0221dbf-f6dd-47d3-af24-c3c7410c5f0d">
-             <pre id="6f0c32f8-fdf5-4bcd-872a-84e9b534d3d8"><code class="python">Anchor("Google Search").link("https://www.google.com/")</code></pre>
-             <div id="9c078626-670b-4250-bc36-a09304a63f63">
-              <a href="https://www.google.com/" id="52d88a63-7f5d-4517-8159-b593196982b0">
+            <div id="50a4de03-5c1d-4d97-ae96-69f86e03139a">
+             <pre id="b3b7f8a5-1856-412a-ac66-6b64760d8604"><code class="python">from bootwrap import Panel, Anchor
+Panel(
+    Anchor("Google Search").link("https://www.google.com/")
+)</code></pre>
+             <div id="b3b911c2-3331-4807-8d65-68d3f0f66021">
+              <a href="https://www.google.com/" id="3843e70f-b1c0-4e50-be32-f8cf1055ebba">
                Google Search
               </a>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="105f43b7-fb85-45c8-aebb-a50a6c2e0126">
-        <div class="mt-3" id="aa0c2720-503a-481d-a1a4-1d3ebb6900a1">
-         <div id="a2586fc8-304b-4a4f-9764-298ceaa137ce">
+       <div class="tab-pane fade" id="ca8d51d0-0c9c-4d73-9297-126011de6074">
+        <div class="mt-3" id="1c4aff83-be2b-45e4-87bb-514e69d0ce14">
+         <div id="cb01853f-e678-4bc3-adb2-53640d1e6c50">
           <div class="row">
            <div class="col-md">
-            <div id="1f8e8ccf-683d-4025-9f09-9d010e5246f4">
-             <h1 id="f3947b55-a598-420b-b2f1-70cf3a25d4dc">
+            <div id="2450dc10-d3f4-431f-a0b4-35dede680f46">
+             <h1 id="036c9a26-2435-4b1d-ac37-3998ea36bea6">
               Open Dialog
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="fa648cf1-5b4d-4456-a258-b4ddbba19a2f">
+            <div id="06e7cc85-fcb6-4996-8932-91af5fe06a3a">
             </div>
            </div>
           </div>
          </div>
-         <div id="2b923513-1130-4856-8191-09ff49467e39">
+         <div id="d31bfaf4-69ce-4be8-aca7-b53839db4c00">
           <div class="row">
            <div class="col-md">
-            <div id="72bce603-76cc-405e-9261-928889ee2cdb">
-             <p id="50c3544c-5613-4300-aebf-7d6f38ae0305">
+            <div id="79290846-6c8d-4f4b-907c-9028d4180c98">
+             <p id="74a530f4-b766-45d5-ac96-e9d75c009930">
               Use
               <code>
                Anchor
               </code>
               to open a dialog using the
               <code>
                toggle()
               </code>
               function.
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="ec698ae2-a400-4228-ac47-9b5245b57c09">
-             <pre id="6a0256b8-e8f0-4fce-8f9f-dd4d303c83f7"><code class="python">dialog = Dialog(
+            <div id="d9c82ff0-2c08-46a4-abbc-dab629f82bc8">
+             <pre id="9311525d-1c14-4504-b8d0-6530db4223df"><code class="python">from bootwrap import Panel, Dialog, Anchor
+dialog = Dialog(
   "Greeting",
   "Hello World!"
 )
-anchor = Anchor("Say Hello").toggle(dialog)</code></pre>
-             <div id="588edcf6-010b-4e63-be44-24fff3513ca8">
-              <div class="modal" id="5f17fe22-a1dc-4493-bd7d-8168160341d6">
+anchor = Anchor("Say Hello").toggle(dialog)
+Panel(dialog, anchor)</code></pre>
+             <div id="5f3e1e42-179e-45e4-a0e3-d2254e0720e5">
+              <div class="modal" id="aded6514-3876-4d71-ac20-4dc136ab3eca">
                <div class="modal-dialog" role="document">
                 <div class="modal-content">
                  <div class="modal-header">
                   <h5 class="modal-title text-None">
                    Greeting
                   </h5>
                   <button aria-label="Close" class="close" data-dismiss="modal" type="button">
@@ -492,68 +505,70 @@
                  </div>
                  <div class="modal-body">
                   Hello World!
                  </div>
                 </div>
                </div>
               </div>
-              <a data-toggle="modal" href="#5f17fe22-a1dc-4493-bd7d-8168160341d6" id="61998b3f-5037-4c40-9ce8-f26a71d3604b" role="modal">
+              <a data-toggle="modal" href="#aded6514-3876-4d71-ac20-4dc136ab3eca" id="431cd0a4-7626-416f-ab6e-d79df85f519d" role="modal">
                Say Hello
               </a>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="c0152c9a-bb26-493e-912c-586c2dea445a">
-        <div class="mt-3" id="aea978a0-bfde-463d-99af-74f43b193605">
-         <div id="9fda7571-7073-4ea5-9ace-1a0c683d4fe2">
+       <div class="tab-pane fade" id="7a81a75a-62b0-42bd-80ad-ff1a4281bef5">
+        <div class="mt-3" id="d57a63ef-efab-4e1e-a5df-377b5d060946">
+         <div id="c143bb18-b9e2-4b06-b943-6319e0414ca4">
           <div class="row">
            <div class="col-md">
-            <div id="7a0a9df4-5d3b-40d9-b940-0a87ee7efd8e">
-             <h1 id="b4474488-46f7-4085-a256-0101b12b5322">
+            <div id="1e6f8971-2c94-4be1-8565-741faffd3aae">
+             <h1 id="d967365c-34ad-4430-886d-037941405566">
               Close Dialog
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="4a5cebf4-c1e1-4de6-a330-5f1639264eac">
+            <div id="36f304c1-608d-4793-91f6-fa87951814b8">
             </div>
            </div>
           </div>
          </div>
-         <div id="f4384284-7b8e-4ff3-9a63-79065c862ef4">
+         <div id="45b5a9ec-5322-49a9-9c1b-6f87924a31d7">
           <div class="row">
            <div class="col-md">
-            <div id="2137c831-93fa-48c1-b8e5-812606c7d606">
-             <p id="cfbf5313-bde0-407c-b87c-688e528b935d">
+            <div id="7beb4ee8-b20b-4d51-8995-82a09749e7f5">
+             <p id="3025c343-64c7-4b02-9521-6cc3a6ac86cf">
               Use
               <code>
                Anchor
               </code>
               to close a dialog using the
               <code>
                dismiss()
               </code>
               function.
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="ea477c12-9d29-4351-890c-70b30fea1251">
-             <pre id="af101d27-6be6-45ab-9198-b79803e962a3"><code class="python">dialog = Dialog(
+            <div id="4614b44d-ce0c-4626-affd-ff716e8d9799">
+             <pre id="1882d889-a982-474f-9522-7ed13a484132"><code class="python">from bootwrap import Panel, Dialog, Anchor
+dialog = Dialog(
   "Greeting",
   "Hello World!",
   Anchor("Bye").dismiss()
 )
-anchor = Anchor("Say Hello").toggle(dialog)</code></pre>
-             <div id="a73f52fa-280e-4570-ba81-9c18a531a905">
-              <div class="modal" id="ec20c6a6-1c71-49d4-bca6-c5bc57c4bb17">
+anchor = Anchor("Say Hello").toggle(dialog)  
+Panel(dialog, anchor)</code></pre>
+             <div id="1e959628-4e0e-4c92-a38e-87aedbe831db">
+              <div class="modal" id="bdfc9d90-7b18-42fe-95ea-56ad64e86105">
                <div class="modal-dialog" role="document">
                 <div class="modal-content">
                  <div class="modal-header">
                   <h5 class="modal-title text-None">
                    Greeting
                   </h5>
                   <button aria-label="Close" class="close" data-dismiss="modal" type="button">
@@ -562,135 +577,139 @@
                    </span>
                   </button>
                  </div>
                  <div class="modal-body">
                   Hello World!
                  </div>
                  <div class="modal-footer">
-                  <a data-dismiss="modal" href="#" id="786af6fa-2599-43f6-85f5-b57df48dbed6">
+                  <a data-dismiss="modal" href="#" id="1be08b1f-d95d-4032-97f2-23a2f834173e">
                    Bye
                   </a>
                  </div>
                 </div>
                </div>
               </div>
-              <a data-toggle="modal" href="#ec20c6a6-1c71-49d4-bca6-c5bc57c4bb17" id="a5a76408-f8a5-4dd6-962a-31ef3521687e" role="modal">
+              <a data-toggle="modal" href="#bdfc9d90-7b18-42fe-95ea-56ad64e86105" id="10d0df86-1e45-4c80-9599-99619f9b744b" role="modal">
                Say Hello
               </a>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="0c812bd2-06ab-4af6-b393-15e5c235ca84">
-        <div class="mt-3" id="d405a98b-146b-4bce-af90-f6e026725921">
-         <div id="bec9844e-5712-415a-b0dc-1b0b132f87e3">
+       <div class="tab-pane fade" id="02f70fee-f643-4a6a-9e25-b26aeb334ca8">
+        <div class="mt-3" id="966b7182-ba9b-4cfc-8c96-cc901ca369ac">
+         <div id="b5d6077b-9e9d-4172-8b5a-7dc70ee337d7">
           <div class="row">
            <div class="col-md">
-            <div id="bf3525cd-807d-46e7-858d-8506ec2e09a8">
-             <h1 id="7284a57f-cdab-42ff-a554-ce3912ebc99c">
+            <div id="32fab3e1-92a3-4c9d-87fb-524ccd41265c">
+             <h1 id="d27186f9-b46b-493f-8a83-9fd4a84d32e9">
               Expand/Collapse Panel
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="86da8858-e9c3-4650-8760-adcd967716c9">
+            <div id="a91c6f55-5679-4920-9d5b-96064e448711">
             </div>
            </div>
           </div>
          </div>
-         <div id="e85b85fa-a6e9-4c2a-984c-aa0cdcb85aeb">
+         <div id="ec7b7331-52df-41f5-8626-bc93a59dc574">
           <div class="row">
            <div class="col-md">
-            <div id="b8d12f37-b605-4291-8647-b17cd88bc686">
-             <p id="532e7f32-e6b7-47ce-8533-eb7c5cf78480">
+            <div id="d7245863-53d3-4098-9615-9c56e61d8de9">
+             <p id="0b25970a-10e8-4e8e-b463-18f4b6034965">
               Use
               <code>
                Anchor
               </code>
               to expand/collapse a panel using the
               <code>
                toggle()
               </code>
               function.
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="a630ba1a-7aeb-44b2-8582-8cb5e9dab4eb">
-             <pre id="db3b1409-a64a-4e1a-9b71-f5a88440daf5"><code class="python">quote = Panel(
+            <div id="f64aa995-875b-4254-96da-4a7903c06aac">
+             <pre id="e4b5140b-fcbf-4893-8e54-dfbe139168e0"><code class="python">from bootwrap import Panel, Anchor
+quote = Panel(
   "Sometimes life is going to hit you in " +
   "the head with a brick. Don’t lose faith."
 ).as_collapse()
-Anchor("Steve Jobs Quote").toggle(quote)</code></pre>
-             <div id="42da9126-b064-4350-96f9-0c62ae8617f1">
-              <a data-target="#75a35060-0842-43b2-8a85-4196f6de2f11" data-toggle="collapse" href="#75a35060-0842-43b2-8a85-4196f6de2f11" id="e013735e-41fd-4491-ac38-887a6c26015c" role="collapse">
+Panel(
+  Anchor("Steve Jobs Quote").toggle(quote),
+  quote
+)</code></pre>
+             <div id="fd5aa206-d7be-4cd9-9e17-a09a49642e8c">
+              <a data-target="#b8004c32-2dc0-4cf4-8e7a-e3491956c01c" data-toggle="collapse" href="#b8004c32-2dc0-4cf4-8e7a-e3491956c01c" id="bfa650dd-76ef-409b-83d9-8b7370c08f10" role="collapse">
                Steve Jobs Quote
               </a>
-              <div class="collapse" id="75a35060-0842-43b2-8a85-4196f6de2f11">
+              <div class="collapse" id="b8004c32-2dc0-4cf4-8e7a-e3491956c01c">
                Sometimes life is going to hit you in the head with a brick. Don’t lose faith.
               </div>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="dbe831ae-15e3-460e-ab29-5cc4f0d82416">
-     <div id="5b801b6b-d200-4210-84d4-54f302b1fff6">
+    <div class="tab-pane fade" id="528aad1b-691d-4637-8b4a-58482729b51e">
+     <div id="a20b8e1a-4cc6-4144-9635-a4e628585436">
       <hr/>
-      <ul class="nav" id="0c4dcc4a-d7e4-48e0-aba3-e2d88a55d3ea" role="tablist">
+      <ul class="nav" id="ab44923c-ffb0-41f5-9064-517315773c28" role="tablist">
        <li class="nav-item">
-        <a class="nav-link active" data-target="#279c5a60-f591-44a6-beed-b5088ae720de" data-toggle="tab" href="#279c5a60-f591-44a6-beed-b5088ae720de" id="5bd65a0d-d9c5-4861-ab53-37fe1b09d45b" role="tab">
-         <span class="text-secondary" id="9faedcad-6838-4324-8b01-faf6a400e7a5">
+        <a class="nav-link active" data-target="#f5e8a6b5-4f69-48e5-91a2-24bed8298b22" data-toggle="tab" href="#f5e8a6b5-4f69-48e5-91a2-24bed8298b22" id="0ab7167c-ca7a-4890-8b03-7f382230cb3f" role="tab">
+         <span class="text-secondary" id="e59851ba-ba32-4d07-937f-0ade79c9cb3d">
           Badge
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#d2b0325b-2a50-480d-b591-99d7cf4a28f7" data-toggle="tab" href="#d2b0325b-2a50-480d-b591-99d7cf4a28f7" id="e990bbf9-507f-468f-9988-cf37846affa4" role="tab">
-         <span class="text-secondary" id="234a44fe-f644-4a2c-b6a1-afcbbc8fdfbe">
+        <a class="nav-link" data-target="#adad46db-c6bd-4a68-85a7-9ec9612deb45" data-toggle="tab" href="#adad46db-c6bd-4a68-85a7-9ec9612deb45" id="82c674d0-e97b-4c78-86d1-9f031de69799" role="tab">
+         <span class="text-secondary" id="2b7c9dbf-bed0-40fe-b980-c124e78eb7f7">
           Appearance
          </span>
         </a>
        </li>
       </ul>
       <div class="tab-content">
-       <div class="tab-pane fade active show" id="279c5a60-f591-44a6-beed-b5088ae720de">
-        <div class="mt-5" id="ca730eff-6e31-4e59-ab2c-6b8393193cc7">
-         <div class="d-flex justify-content-between" id="00c4ff06-6e08-491e-92c2-e7fab0a16741">
-          <h1 id="e12b6b3a-3a0b-4bbf-a3ed-7039e562e256">
+       <div class="tab-pane fade active show" id="f5e8a6b5-4f69-48e5-91a2-24bed8298b22">
+        <div class="mt-5" id="8f579c0c-38c8-4944-807c-3391f4282cb2">
+         <div class="d-flex justify-content-between" id="69604393-b45e-4173-a372-7f3adff94da0">
+          <h1 id="fdaeab91-644a-4793-b7c5-0b623dfd6268">
            Class
-           <span class="text-primary" id="40276c85-a9cd-4b21-aa87-36fd5320997b">
+           <span class="text-primary" id="57014c4a-80f4-4123-9c2a-80cc47fe49bf">
             Badge
            </span>
           </h1>
-          <div id="88ee7e81-b82d-456c-b45c-9197407570c1">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#a381dc84-273b-45e2-8ea7-dc1fd923ee2e" data-toggle="collapse" id="85861815-03c7-4b1a-9b01-ee74a2e66d04" onclick="return false;" type="button">
+          <div id="f4117d69-a64a-4eda-a61d-2b40618a18a0">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#a5c88a9d-9426-4008-8da6-b315d9a30119" data-toggle="collapse" id="5913709c-7c40-4090-a908-3ec36d7d9f72" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="f0dd4fcb-2be5-49b0-85ae-3cc70edc8be3">
+         <span class="text-muted" id="55ec37d4-9f81-401b-9f46-2932faf82a32">
           A web component for a badge.
          </span>
-         <pre id="1cff3fb1-ca54-4516-a565-2f406acc3009"><code class="python">Badge(label)</code></pre>
-         <div class="ml-3 collapse" id="a381dc84-273b-45e2-8ea7-dc1fd923ee2e">
-          <h6 id="62f78dd6-09d9-4501-8a4a-0913173052e8">
+         <pre id="81b50eb0-4658-447d-a4cb-2f36b1023c3f"><code class="python">Badge(label)</code></pre>
+         <div class="ml-3 collapse" id="a5c88a9d-9426-4008-8da6-b315d9a30119">
+          <h6 id="674ba8e2-a69f-4a68-a276-d2a48de6ef20">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="56674906-02f9-4039-972c-192f60e1f537">
+          <table class="table table-sm bg-light" id="8129c4d4-f692-44f5-b545-f0b93971427e">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -715,51 +734,53 @@
              <td>
               The badge label (text showing inside a badge).
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <div class="ml-3" id="b40049dd-2371-4f50-acc6-21e3a81a068b">
-          <h6 id="a41bc95e-8443-43c6-9129-9c7918f22929">
+         <div class="ml-3" id="645a582c-b3ba-4e17-856f-1f4e73871639">
+          <h6 id="1cbdc021-7de4-4014-b7e3-edec8eebe601">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="be05b1ca-69e5-4baa-bb56-06cc669bc51c"><code class="python">Badge('Some Badge')</code></pre>
+          <pre id="88d2ad2f-1ea5-4676-acf3-2861d736b0fb"><code class="python">from bootwrap import Badge
+Badge('Some Badge')
+</code></pre>
          </div>
-         <div class="ml-3" id="2262004c-9b4a-4c2e-8dfe-9bf091fae3b2">
-          <span class="badge" id="b02b77c4-e3f2-40ca-a860-ad3ad4e23829">
+         <div class="ml-3" id="221529da-ba11-4759-b7d9-45a883d2cbe5">
+          <span class="badge" id="ec535cf6-791d-4406-a1f9-839962bf1711">
            Some Badge
           </span>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="d2b0325b-2a50-480d-b591-99d7cf4a28f7">
-        <div class="mt-3" id="5aef4037-6609-4a2e-a82d-f37b3444fd1a">
-         <div id="bc4cab1d-def3-4d84-a874-45175e818898">
+       <div class="tab-pane fade" id="adad46db-c6bd-4a68-85a7-9ec9612deb45">
+        <div class="mt-3" id="e2dda6b6-19f6-4207-8229-155faa137001">
+         <div id="04153bb9-e730-4c3a-8655-46caad44822a">
           <div class="row">
            <div class="col-md">
-            <div id="b4b682c0-95e8-4e76-b4d7-b782ab2e2499">
-             <h1 id="7eb5498d-ca34-441c-b468-c6b85ae7cdc7">
+            <div id="9b08ad88-08f4-4cbc-b829-fbf81be775ce">
+             <h1 id="39c3b534-06c3-4dd8-a4f9-a258bccb9e81">
               Appearance
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="c2e13405-4781-4e92-86bb-b6facbc9cc06">
+            <div id="47f5df2e-c1df-4616-b545-0548240eb64e">
             </div>
            </div>
           </div>
          </div>
-         <div id="f7fa37ea-92e5-4609-9918-27c012331fb0">
+         <div id="60f43c88-4f5d-4d51-9b34-9674b9810a8b">
           <div class="row">
            <div class="col-md">
-            <div id="552b05ca-767c-49ac-8c28-10a2959ef09a">
-             <p id="3794828c-1ccb-4dac-bfb9-c5bb92146f7a">
+            <div id="8428c1e2-3003-48cc-9cda-767a572216a8">
+             <p id="b2d88540-2abe-4121-8100-c2badda4bc94">
               Change
               <code>
                Badge
               </code>
               appearance using the following functions
               <code>
                as_primary()
@@ -793,153 +814,159 @@
                as_dark()
               </code>
               .
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="0d695e45-160d-406e-ba06-0313dfe7eb1b">
-             <pre id="a4f8bcaf-9000-4f39-9dba-1c19bcaa11d6"><code class="python">Badge("Primary").as_primary()
-Badge("Secondary").as_secondary()
-Badge("Success").as_success()
-Badge("Warning").as_warning()
-Badge("Danger").as_danger()
-Badge("Info").as_info()
-Badge("Light").as_light()
-Badge("Dark").as_dark()</code></pre>
-             <div id="9c8cc119-be6b-45a9-8bfe-bcc0ca6da159">
-              <span class="badge badge-primary mb-1" id="1d2899c3-54dd-4cca-8ec3-291e9479eaab">
+            <div id="f453fa5f-9188-4661-b4c1-fc127d5d0e8e">
+             <pre id="c6667c6b-8b67-40b6-88d5-c58de70f5623"><code class="python">from bootwrap import Panel, Badge
+panel = Panel(
+  Badge("Primary").as_primary(),
+  Badge("Secondary").as_secondary(),
+  Badge("Success").as_success(),
+  Badge("Warning").as_warning(),
+  Badge("Danger").as_danger(),
+  Badge("Info").as_info(),
+  Badge("Light").as_light(),
+  Badge("Dark").as_dark()
+)
+for anchor in panel:
+  anchor.mb(1)
+panel</code></pre>
+             <div id="9d50d2ff-765e-4ad5-ad5d-1a65cb3dd0a5">
+              <span class="badge badge-primary mb-1" id="12e7017b-4e29-4e01-8d61-6fe8a6bad703">
                Primary
               </span>
-              <span class="badge badge-secondary mb-1" id="99289dd2-4326-48c1-96a8-2b2bf2a2a77c">
+              <span class="badge badge-secondary mb-1" id="858d83bd-699f-4ab6-b062-e37fb0e16b9d">
                Secondary
               </span>
-              <span class="badge badge-success mb-1" id="82f2c8b9-b1e0-49f7-ba44-b108e309b7ca">
+              <span class="badge badge-success mb-1" id="340e1c28-9ca7-4dcf-92fd-43dedf7d79cc">
                Success
               </span>
-              <span class="badge badge-warning mb-1" id="474d33b0-9f94-46ff-bb99-a7c24b8ab075">
+              <span class="badge badge-warning mb-1" id="96848803-1850-4927-87de-7ca708f3517b">
                Warning
               </span>
-              <span class="badge badge-danger mb-1" id="6551b0a6-e673-4422-8834-461b1fbf9262">
+              <span class="badge badge-danger mb-1" id="1ff3664f-4d67-473a-9fd6-a54f355cabf9">
                Danger
               </span>
-              <span class="badge badge-info mb-1" id="09adfc40-0c03-4836-8772-4144e4afae74">
+              <span class="badge badge-info mb-1" id="9923c4fd-3bc7-4f26-b326-312091235200">
                Info
               </span>
-              <span class="badge badge-light mb-1" id="1cb7b882-8d75-440b-990a-5fe6f3a9e531">
+              <span class="badge badge-light mb-1" id="527828d7-551d-475c-8d7e-13f7663c9443">
                Light
               </span>
-              <span class="badge badge-dark mb-1" id="a98b1212-ceac-4244-bf6d-fd4ac412f6c6">
+              <span class="badge badge-dark mb-1" id="148a9f66-0132-4f51-a0ad-7f29b8bb697d">
                Dark
               </span>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="244d5aa9-7a2d-4332-8373-5b0987e7d08d">
-     <div id="54412b82-1930-4b43-a45c-8cfa3e2b3d30">
+    <div class="tab-pane fade" id="5be43bd9-e0c2-4145-816e-bd5f0c5aea59">
+     <div id="b4300f14-6c97-456e-a0e6-180b4c90809f">
       <hr/>
-      <ul class="nav" id="c1b61583-142d-4030-847b-2854db6b0370" role="tablist">
+      <ul class="nav" id="fe03d047-acb0-4630-b68c-f823d185edcb" role="tablist">
        <li class="nav-item">
-        <a class="nav-link active" data-target="#762fe2a5-3e17-4051-aa4f-a9cfbe17d9c7" data-toggle="tab" href="#762fe2a5-3e17-4051-aa4f-a9cfbe17d9c7" id="400acf58-6999-4f96-a420-644d38778196" role="tab">
-         <span class="text-secondary" id="a525bbc7-6eab-4482-aed2-7f43da376614">
+        <a class="nav-link active" data-target="#aaf78920-d5f4-48b7-a6df-bcb7bf15a495" data-toggle="tab" href="#aaf78920-d5f4-48b7-a6df-bcb7bf15a495" id="78c898ba-d84f-4b82-b24c-6cd912ff25d2" role="tab">
+         <span class="text-secondary" id="71507013-e537-48b0-abd1-b1f63f0c7802">
           Button
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#213482a1-b0ef-45eb-abf1-7f54d862eb9d" data-toggle="tab" href="#213482a1-b0ef-45eb-abf1-7f54d862eb9d" id="a4b2307b-1685-4caa-9c2c-b013e0fd3225" role="tab">
-         <span class="text-secondary" id="58ae3a08-169e-462b-a894-34b5486ec3ef">
+        <a class="nav-link" data-target="#55bd2fe8-0a40-48f5-9fc3-002bc745765a" data-toggle="tab" href="#55bd2fe8-0a40-48f5-9fc3-002bc745765a" id="331e780c-8da0-439e-b931-17a26b7c9cc2" role="tab">
+         <span class="text-secondary" id="fdbb1ff1-4a6d-4193-bdbe-81a012b44ce8">
           Appearance
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#65913b4f-df08-4159-bbc7-2137408567ca" data-toggle="tab" href="#65913b4f-df08-4159-bbc7-2137408567ca" id="0fd8c95c-2686-4d33-bb99-b79bf40db5bc" role="tab">
-         <span class="text-secondary" id="2474c339-98f2-458a-b8d1-22711673f97d">
+        <a class="nav-link" data-target="#c74589e6-bbfe-40be-bc42-460378a0e6a9" data-toggle="tab" href="#c74589e6-bbfe-40be-bc42-460378a0e6a9" id="d74a878f-50f1-44b4-9538-353673061215" role="tab">
+         <span class="text-secondary" id="3fa84526-0fed-4196-b329-fb001a29cc47">
           Outline
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#82d51dac-3cf4-476a-b974-a59513539efa" data-toggle="tab" href="#82d51dac-3cf4-476a-b974-a59513539efa" id="fc8493e4-66f5-47ab-be0a-e79ec5cbc312" role="tab">
-         <span class="text-secondary" id="b03d65e3-9c54-40ce-bede-1bd14ec6c3d9">
+        <a class="nav-link" data-target="#5dcb506b-3590-4e2a-8369-3421c51dc045" data-toggle="tab" href="#5dcb506b-3590-4e2a-8369-3421c51dc045" id="945e0637-35ff-40fb-aa2c-92f904479a8a" role="tab">
+         <span class="text-secondary" id="b3af843e-bb57-4a1c-9316-4c153dd1a558">
           Disable
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#a16b72c5-9d3b-4443-88e7-ae35f54fa3a3" data-toggle="tab" href="#a16b72c5-9d3b-4443-88e7-ae35f54fa3a3" id="ff669bff-b377-43c7-9a80-a57f6ace50c4" role="tab">
-         <span class="text-secondary" id="409ec5c9-eafa-4ae1-ba84-743930fef8a1">
+        <a class="nav-link" data-target="#360cb23c-7ba4-4998-b0cb-ece4b54df72c" data-toggle="tab" href="#360cb23c-7ba4-4998-b0cb-ece4b54df72c" id="bf58971d-2184-40f7-a151-6ae6d170af99" role="tab">
+         <span class="text-secondary" id="445955e5-2bb8-4865-b22b-77365e1eebf2">
           Link Resource
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#a7aa8e9c-1379-4468-abec-c10958bfc587" data-toggle="tab" href="#a7aa8e9c-1379-4468-abec-c10958bfc587" id="4d046eed-f09e-477b-89f2-b27bef3398e9" role="tab">
-         <span class="text-secondary" id="ffbd520b-1a93-4897-a1d6-d2df7afa8ca6">
+        <a class="nav-link" data-target="#0f715e53-7ba3-41c5-a5d0-0c17fbf4252a" data-toggle="tab" href="#0f715e53-7ba3-41c5-a5d0-0c17fbf4252a" id="eb3bbfa9-b819-4479-bc5c-6bada0c81cf7" role="tab">
+         <span class="text-secondary" id="867ad7a3-2b49-45da-831e-039036742d8e">
           Open Dialog
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#dd4c1069-bc4f-4820-939e-a43ccf0829ae" data-toggle="tab" href="#dd4c1069-bc4f-4820-939e-a43ccf0829ae" id="d7245369-aa1d-4901-b1bf-d0a6d02e0414" role="tab">
-         <span class="text-secondary" id="2983ca75-3002-4ab5-bbaa-cd99105b4862">
+        <a class="nav-link" data-target="#9788024e-60c1-42bf-9792-a310e1f1c41f" data-toggle="tab" href="#9788024e-60c1-42bf-9792-a310e1f1c41f" id="188c864c-8674-49d0-b2e8-b43acf65f667" role="tab">
+         <span class="text-secondary" id="520dfb0f-c5dc-40b0-8a20-bc319d8ebda5">
           Close Dialog
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#bb3aa52f-0d51-4a21-ac5d-5e9c93289344" data-toggle="tab" href="#bb3aa52f-0d51-4a21-ac5d-5e9c93289344" id="e2d535f6-82ca-4923-9a78-23dc856c7592" role="tab">
-         <span class="text-secondary" id="67ae1b41-ff6c-4389-a045-7e01fd3ca98a">
+        <a class="nav-link" data-target="#8c3bc726-5007-4234-a21d-542129f845c5" data-toggle="tab" href="#8c3bc726-5007-4234-a21d-542129f845c5" id="10d8aa3d-a95e-4ff0-bcfb-324b31b431cb" role="tab">
+         <span class="text-secondary" id="5152afbf-9d62-4fd8-97ac-83f3ed21ac2b">
           Expand/Collapse Panel
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#a58710e1-9bcd-4b72-bbfd-c15ed85a27aa" data-toggle="tab" href="#a58710e1-9bcd-4b72-bbfd-c15ed85a27aa" id="85b1ee12-a6b3-4510-b15b-aa2824300b64" role="tab">
-         <span class="text-secondary" id="e8d09934-c9f6-460b-bb8e-70330eb6cc03">
+        <a class="nav-link" data-target="#5aa621b3-e462-454b-982e-f69687f7f8d8" data-toggle="tab" href="#5aa621b3-e462-454b-982e-f69687f7f8d8" id="78393606-9311-4529-b932-cf86d8b12919" role="tab">
+         <span class="text-secondary" id="5da64fb0-e9f7-4a16-bc28-f5e6de881f45">
           Submit Action
          </span>
         </a>
        </li>
       </ul>
       <div class="tab-content">
-       <div class="tab-pane fade active show" id="762fe2a5-3e17-4051-aa4f-a9cfbe17d9c7">
-        <div class="mt-5" id="b12d0004-1535-4f89-93fa-4975b147421c">
-         <div class="d-flex justify-content-between" id="ac98a7ab-1ac2-4d68-a546-e6bc5cdcf43f">
-          <h1 id="7b1b0952-497a-4906-848d-68ac215cb252">
+       <div class="tab-pane fade active show" id="aaf78920-d5f4-48b7-a6df-bcb7bf15a495">
+        <div class="mt-5" id="91ec8b05-7733-4e45-9eb9-156ce5bcdfa8">
+         <div class="d-flex justify-content-between" id="845f4170-c5f2-4d63-84c0-28ebfb799405">
+          <h1 id="3f92e115-1b1e-41f1-8afb-70f7d3fb3f98">
            Class
-           <span class="text-primary" id="82f66a40-509b-4b79-9f11-4867780cb961">
+           <span class="text-primary" id="d98d28f3-e7c2-406c-8ccf-e155b40223a7">
             Button
            </span>
           </h1>
-          <div id="3a2680e0-e5e0-4258-9808-fe4ffd564a61">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#913487cf-26ec-463e-a060-f2b5c7b4978c" data-toggle="collapse" id="e5000077-47e4-46ad-8042-55c5055556a1" onclick="return false;" type="button">
+          <div id="35611e2f-fdd7-4364-83fe-172100035f98">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#8785bca1-7659-42c0-862f-abe5d613add3" data-toggle="collapse" id="5328e7b4-1ebd-462b-9679-fe5faa8677a3" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="f1a77fbc-d374-4603-9899-7b59de79a95e">
+         <span class="text-muted" id="1c024b1c-c2e1-48c4-b6eb-fb4982496681">
           A web component for a button.
          </span>
-         <pre id="566f9e12-21af-45d1-a483-6ea024c34d90"><code class="python">Button(name)</code></pre>
-         <div class="ml-3 collapse" id="913487cf-26ec-463e-a060-f2b5c7b4978c">
-          <h6 id="79a8788f-6846-4568-8d4d-e72a7ad87212">
+         <pre id="e16545fb-e3a7-467a-aaca-7e9cf2e09c47"><code class="python">Button(name)</code></pre>
+         <div class="ml-3 collapse" id="8785bca1-7659-42c0-862f-abe5d613add3">
+          <h6 id="2589f658-7c36-48f8-8f65-0290d274814d">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="21081120-27b2-49de-af53-149da7ca3ea3">
+          <table class="table table-sm bg-light" id="179308dc-0504-4216-893d-4828d1eb1434">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -964,63 +991,65 @@
              <td>
               The button name.
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <p id="3709a88a-80a5-479c-bfe2-f96e418b5d39">
+         <p id="754825cd-b421-4e9a-a96e-1a9e7dee9e3f">
           Without applying a stylized method
           <code>
            Button
           </code>
           will be appearing very
     similar to the
           <code>
            Anchor
           </code>
           .
          </p>
-         <div class="ml-3" id="47ed62ff-1cb9-4d47-9588-2a78cb6eeb89">
-          <h6 id="1f74f1e6-39ca-4e16-97f7-7b5d0bef3d75">
+         <div class="ml-3" id="d35b207e-abd8-4f8f-a924-395663d65db0">
+          <h6 id="6d86a1ae-cb04-4dcf-8946-1e67de36a4f0">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="120c67e8-be07-41ca-b9c8-1dd296ea4e04"><code class="python">Button('Google Search').link('https://www.google.com/')</code></pre>
+          <pre id="3fac1fac-dea7-41bd-843a-b3fbe500c081"><code class="python">from bootwrap import Button
+Button('Google Search').link('https://www.google.com/')
+</code></pre>
          </div>
-         <div class="ml-3" id="e3b8183e-3dc4-4b03-be7d-e0b2319e1519">
-          <a class="btn" href="https://www.google.com/" id="902516c2-0161-46e9-9392-29bec187e3d2" role="button">
+         <div class="ml-3" id="ac66b20f-b834-4a04-8a7a-5b0346e2022b">
+          <a class="btn" href="https://www.google.com/" id="181d7ba8-98cf-4ad5-9582-0283951ff9db" role="button">
            Google Search
           </a>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="213482a1-b0ef-45eb-abf1-7f54d862eb9d">
-        <div class="mt-3" id="cf6ae29c-2e2b-497e-9ac5-da82f9c64572">
-         <div id="2e9320cc-3edd-4322-92e8-861393101212">
+       <div class="tab-pane fade" id="55bd2fe8-0a40-48f5-9fc3-002bc745765a">
+        <div class="mt-3" id="2db85e43-5082-42a8-bf9c-fdf6dd84c96e">
+         <div id="e22508a1-7888-4587-89a6-8bc0204bedea">
           <div class="row">
            <div class="col-md">
-            <div id="2461b8a8-f33b-4f13-a3ab-35a96e4fbb6a">
-             <h1 id="ac440905-7018-402e-85a6-9d225c4d7e53">
+            <div id="41af788f-8f7d-4150-83e3-3428cc62f290">
+             <h1 id="5f58c5b4-6146-4e64-b86b-de33287af715">
               Appearance
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="477f9570-9142-444b-ae06-ab1354d58b77">
+            <div id="d1b03283-9eb3-455c-aa04-947d0dc3288f">
             </div>
            </div>
           </div>
          </div>
-         <div id="524d9890-e1c1-44a4-be19-106dd737a9b4">
+         <div id="5a981e4d-a233-4f21-ad6a-422e8501891b">
           <div class="row">
            <div class="col-md">
-            <div id="31950c25-6858-4869-a1fb-7a2d17347f63">
-             <p id="87c07c07-29a5-4aa7-9ac9-c49f67265dfa">
+            <div id="59f4c4b1-9d3d-48ba-a6d8-513acef4eb31">
+             <p id="99fac71b-def9-4454-99d4-44551e5bac91">
               Change
               <code>
                Button
               </code>
               appearance using the following functions
               <code>
                as_primary()
@@ -1054,153 +1083,165 @@
                as_dark()
               </code>
               .
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="b75f6f8b-1c92-4753-9277-a868fc2904e4">
-             <pre id="ccf13007-4eeb-42a6-a014-3379ac6d907f"><code class="python">Button("Primary").as_primary()
-Button("Secondary").as_secondary()
-Button("Success").as_success()
-Button("Warning").as_warning()
-Button("Danger").as_danger()
-Button("Info").as_info()
-Button("Light").as_light()
-Button("Dark").as_dark()</code></pre>
-             <div id="37b9d088-a4f9-4053-a2f3-d730707ca40e">
-              <a class="mb-1 btn btn-primary" href="#" id="7ebfca89-42bd-47a7-a1c1-6f7e5d490b53" role="button">
+            <div id="868804ca-15d7-4d34-9bed-43a11387289a">
+             <pre id="66048ced-a309-4d67-b6e8-e1083de18847"><code class="python">from bootwrap import Panel, Button
+panel = Panel(
+  Button("Primary").link("#").as_primary(),
+  Button("Secondary").link("#").as_secondary(),
+  Button("Success").link("#").as_success(),
+  Button("Warning").link("#").as_warning(),
+  Button("Danger").link("#").as_danger(),
+  Button("Info").link("#").as_info(),
+  Button("Light").link("#").as_light(),
+  Button("Dark").link("#").as_dark()
+)
+for anchor in panel:
+  anchor.mb(1)
+panel</code></pre>
+             <div id="e8ba23da-ea57-44f6-aea2-c123ae111d95">
+              <a class="mb-1 btn btn-primary" href="#" id="5208d0be-66a6-4b11-a12f-d80a236f67ea" role="button">
                Primary
               </a>
-              <a class="mb-1 btn btn-secondary" href="#" id="4e5165b0-1980-4708-885a-9dabff2762b2" role="button">
+              <a class="mb-1 btn btn-secondary" href="#" id="75d76a93-8a24-4f8f-83bc-ba2f85e8bfa2" role="button">
                Secondary
               </a>
-              <a class="mb-1 btn btn-success" href="#" id="c4fab969-0456-495c-8b44-c8b8f170c331" role="button">
+              <a class="mb-1 btn btn-success" href="#" id="7c879827-96ec-474b-8ddd-7c7374f5d79e" role="button">
                Success
               </a>
-              <a class="mb-1 btn btn-warning" href="#" id="27133651-7c4d-4219-9302-0dc2e7c842b9" role="button">
+              <a class="mb-1 btn btn-warning" href="#" id="e2c89016-ffee-42da-b28a-c96ca9fdbfec" role="button">
                Warning
               </a>
-              <a class="mb-1 btn btn-danger" href="#" id="b6c8079b-a266-470a-9a5f-930396dc7dad" role="button">
+              <a class="mb-1 btn btn-danger" href="#" id="cf2b7adb-a39b-4bb3-8e9c-0db8b51824fc" role="button">
                Danger
               </a>
-              <a class="mb-1 btn btn-info" href="#" id="41047b57-acff-4e11-a334-9938815868ce" role="button">
+              <a class="mb-1 btn btn-info" href="#" id="a07f47e9-3254-4e5f-9594-592819c51c80" role="button">
                Info
               </a>
-              <a class="mb-1 btn btn-light" href="#" id="4ca426dd-bcde-4d84-ac48-90df55352ed4" role="button">
+              <a class="mb-1 btn btn-light" href="#" id="a895d751-48c8-4c64-9793-cf233be8f55c" role="button">
                Light
               </a>
-              <a class="mb-1 btn btn-dark" href="#" id="4e5cfa4b-1088-42ea-b1ae-eb30afc7be56" role="button">
+              <a class="mb-1 btn btn-dark" href="#" id="66398643-14d9-4e56-96d4-ef49053e50c1" role="button">
                Dark
               </a>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="65913b4f-df08-4159-bbc7-2137408567ca">
-        <div class="mt-3" id="81cfed33-8b79-4d81-8189-44ea4c10b096">
-         <div id="270dd6d9-2e33-47dd-82b8-a27aeacde810">
+       <div class="tab-pane fade" id="c74589e6-bbfe-40be-bc42-460378a0e6a9">
+        <div class="mt-3" id="a728752c-62af-4e2d-b144-43d3837c17a5">
+         <div id="59f07bc2-b322-46df-a5a0-38f6f74405de">
           <div class="row">
            <div class="col-md">
-            <div id="f955bc9f-ba0c-4b7d-9630-b5a9c3579463">
-             <h1 id="9cc602c8-014a-49e0-890f-c0d225958533">
+            <div id="eb3162c3-9692-42e9-96b9-f2d493f02cb8">
+             <h1 id="fc2f2116-91e7-49bc-9e7a-ef8f76f1525f">
               Outline
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="592560f9-dfb1-4ff7-a160-a26a33dc42ba">
+            <div id="d6e18cb2-073a-44b5-908c-59963987c283">
             </div>
            </div>
           </div>
          </div>
-         <div id="57287212-711a-4809-8c3a-88925af4b704">
+         <div id="97db861f-25ad-4d6a-bbe7-dd43c3ed31d0">
           <div class="row">
            <div class="col-md">
-            <div id="d2bacc64-2606-4072-8689-eea4d216e486">
-             <p id="21e0c7ef-e6f4-4d3a-9c09-8bc0002a4c0d">
+            <div id="5e8eebac-9f07-4af5-ab34-238af527e6f3">
+             <p id="215cb5d0-ea8f-4f39-b685-85ae22b972b8">
               Make
               <code>
                Button
               </code>
               without filling with surrounded by color border using the following function
               <code>
                as primary()
               </code>
               .
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="c76c8382-ba9b-43d4-b0ba-899498dceac8">
-             <pre id="8afc4b65-8af2-4e14-8667-106c070d136a"><code class="python">Button("Primary").as_primary().as_outline()
-Button("Secondary").as_secondary().as_outline()
-Button("Success").as_success().as_outline()
-Button("Warning").as_warning().as_outline()
-Button("Danger").as_danger().as_outline()
-Button("Info").as_info().as_outline()
-Button("Light").as_light().as_outline()
-Button("Dark").as_dark().as_outline()</code></pre>
-             <div id="b79ee502-f690-45c8-a13d-38efa08af389">
-              <a class="mb-1 btn btn-outline-primary" href="#" id="53af362d-3d76-414d-85c2-1c21f5eb727d" role="button">
+            <div id="e74f38ba-64c4-42fe-ae78-708d4f5512ce">
+             <pre id="49d4e02c-26be-48ea-a79d-e86127b9cdc9"><code class="python">from bootwrap import Panel, Button
+panel = Panel(
+  Button("Primary").link("#").as_primary().as_outline(),
+  Button("Secondary").link("#").as_secondary().as_outline(),
+  Button("Success").link("#").as_success().as_outline(),
+  Button("Warning").link("#").as_warning().as_outline(),
+  Button("Danger").link("#").as_danger().as_outline(),
+  Button("Info").link("#").as_info().as_outline(),
+  Button("Light").link("#").as_light().as_outline(),
+  Button("Dark").link("#").as_dark().as_outline()
+)
+for anchor in panel:
+  anchor.mb(1)
+panel</code></pre>
+             <div id="ad0be79c-99f5-47d1-9ae7-b2dd93be5f17">
+              <a class="mb-1 btn btn-outline-primary" href="#" id="1c48d9d8-7440-4412-8f3d-3bf7df880716" role="button">
                Primary
               </a>
-              <a class="mb-1 btn btn-outline-secondary" href="#" id="86dbfd31-ba21-4c76-b94a-481b3262139e" role="button">
+              <a class="mb-1 btn btn-outline-secondary" href="#" id="87f9b38e-f529-4e8f-bd8f-7e6f4af639f9" role="button">
                Secondary
               </a>
-              <a class="mb-1 btn btn-outline-success" href="#" id="2ab8abca-21a0-4321-9881-3c6efbee2e6f" role="button">
+              <a class="mb-1 btn btn-outline-success" href="#" id="4ef1dc5e-bab0-4f63-a6a1-8012c0c8a476" role="button">
                Success
               </a>
-              <a class="mb-1 btn btn-outline-warning" href="#" id="ab0a5601-52b3-46d3-a666-e37dcfdd49fe" role="button">
+              <a class="mb-1 btn btn-outline-warning" href="#" id="51bef0d3-40c7-423e-aefd-d57759150913" role="button">
                Warning
               </a>
-              <a class="mb-1 btn btn-outline-danger" href="#" id="93f7d0e6-de59-4410-802c-649a120f3f49" role="button">
+              <a class="mb-1 btn btn-outline-danger" href="#" id="3d08db5a-3823-44e5-8181-cf0148af5bb5" role="button">
                Danger
               </a>
-              <a class="mb-1 btn btn-outline-info" href="#" id="60ad0b08-27fb-49f9-a80f-41016880704a" role="button">
+              <a class="mb-1 btn btn-outline-info" href="#" id="6b970395-fc2e-4605-b42d-7395500a78aa" role="button">
                Info
               </a>
-              <a class="mb-1 btn btn-outline-light" href="#" id="7f2094a3-eb97-4939-a343-a8718bee3078" role="button">
+              <a class="mb-1 btn btn-outline-light" href="#" id="5ca836cd-2946-4f6e-ac45-41ae454b2bf8" role="button">
                Light
               </a>
-              <a class="mb-1 btn btn-outline-dark" href="#" id="2fab78d2-a5f4-4183-b2c3-1ffeee554418" role="button">
+              <a class="mb-1 btn btn-outline-dark" href="#" id="c50a9914-d89d-451e-8b17-7632e64272c6" role="button">
                Dark
               </a>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="82d51dac-3cf4-476a-b974-a59513539efa">
-        <div class="mt-3" id="32fdd127-1de2-40c4-a1b5-a99d67961f10">
-         <div id="c381d231-45dd-4a68-bb6d-94e69131695b">
+       <div class="tab-pane fade" id="5dcb506b-3590-4e2a-8369-3421c51dc045">
+        <div class="mt-3" id="547ed8c7-74fb-4d8c-afcb-bb1ff0110e42">
+         <div id="4f6f2437-f358-485d-8cae-f4d70598d1d6">
           <div class="row">
            <div class="col-md">
-            <div id="c004a374-791d-4108-9f54-1527db2c4011">
-             <h1 id="6accbaaa-6605-4b80-b06f-65f913e5c22d">
+            <div id="81f6cd61-2b19-410c-b17b-5f3fb6e71a56">
+             <h1 id="22efbc08-aa3f-4f75-8d42-85080db80061">
               Disable
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="d01de061-9a3f-4524-8713-266a12bac94d">
+            <div id="99be38cb-9eaf-415a-9415-5179b8ed589d">
             </div>
            </div>
           </div>
          </div>
-         <div id="a16a8533-35a3-4608-b359-0720d1d36e20">
+         <div id="ed20f36d-7124-49f7-b663-7a0f9286ecdc">
           <div class="row">
            <div class="col-md">
-            <div id="2e7051de-ad8a-4c48-a66d-a1adbea0409f">
-             <p id="c9f37722-79b7-4f14-b9c1-6e156737e36e">
+            <div id="050ab44c-fdef-4d24-92a4-f8c8b0dbc139">
+             <p id="3cd8c7cc-6447-446c-b1d1-e40b03800b80">
               But default the
               <code>
                Button
               </code>
               always enabled. Use the
               <code>
                as_disabled()
@@ -1214,122 +1255,130 @@
                Button
               </code>
               .
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="463d0fb3-dd9b-4f6e-9755-b125dc83b130">
-             <pre id="4daa3646-46ab-44ff-a447-e5a3a30e7601"><code class="python">Button("Enabled").as_primary()
-Button("Disabled").as_primary().as_disabled()</code></pre>
-             <div id="efb2b248-d672-4aed-a2dd-834f0cda168b">
-              <button class="btn btn-primary" id="29669ee0-655f-4d8e-8018-c58690a4250a" onclick="return false;">
+            <div id="68d9c2db-883e-400e-a4a7-e8d6b1758ffa">
+             <pre id="447446b9-cd6d-4f82-b213-0ae210bd65b5"><code class="python">from bootwrap import Panel, Button
+Panel(
+  Button("Enabled").as_primary(),
+  Button("Disabled").as_primary().as_disabled()
+)</code></pre>
+             <div id="0a373760-212f-4baa-b96a-cd0584deb522">
+              <button class="btn btn-primary" id="661119b5-571a-4890-810e-963a797e1fcd" onclick="return false;">
                Enabled
               </button>
-              <button class="btn btn-primary" disabled="" id="a9d3a0fc-df10-476e-aa95-a38ac3ccbf1b" onclick="return false;">
+              <button class="btn btn-primary" disabled="" id="fb41dc40-7a09-42c1-a116-70f9fbcc18a5" onclick="return false;">
                Disabled
               </button>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="a16b72c5-9d3b-4443-88e7-ae35f54fa3a3">
-        <div class="mt-3" id="c4ebdfe9-438e-4557-975b-dcbebc9c0686">
-         <div id="3ce913f0-8689-4121-bb49-4c6c2d09e026">
+       <div class="tab-pane fade" id="360cb23c-7ba4-4998-b0cb-ece4b54df72c">
+        <div class="mt-3" id="16ff236e-cf09-488b-94f3-3a1dcca767e2">
+         <div id="9c49558e-571d-4381-b6f0-a8e567534402">
           <div class="row">
            <div class="col-md">
-            <div id="a5016887-e69c-4f7f-b795-f56a5f2a8e8a">
-             <h1 id="debd41c9-6fdb-4b21-8342-9ded756e6fbe">
+            <div id="3df04e02-a423-4889-acf6-fd126edde1d7">
+             <h1 id="2160c0d8-8889-4b5e-9629-648848b8d320">
               Link Resource
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="a3be8cab-6d17-47ed-be3a-e6676d74d04d">
+            <div id="e01d471a-cfbf-4cba-ba0c-c816662794f0">
             </div>
            </div>
           </div>
          </div>
-         <div id="76ca83d1-30be-41b2-a7fb-e790350a1853">
+         <div id="8bf40b8e-355f-4d6a-9492-89dec1c4553d">
           <div class="row">
            <div class="col-md">
-            <div id="2905f208-82ff-4223-8de7-c5802361c58e">
-             <p id="c647402a-c842-45ef-816f-2c3cb983509b">
+            <div id="33ecd595-0a6f-49a9-8be7-3cabd25b7f79">
+             <p id="de56e6bf-a41e-4239-bdb2-f7070076a433">
               Associate
               <code>
                Button
               </code>
               with a hyperlink using the
               <code>
                link()
               </code>
               function.
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="7ecce2ef-0367-4fea-b004-9c18f947302b">
-             <pre id="a0594705-9eaf-42d2-bdac-4e6a89d182f1"><code class="python">Button("Google Search").as_primary().link("https://www.google.com/")</code></pre>
-             <div id="628edcdc-21e7-4100-a7ca-48ba40231777">
-              <a class="btn btn-primary" href="https://www.google.com/" id="6bab9a67-9aaf-4e2c-984e-825ed968b987" role="button">
+            <div id="ffc1a3c5-10f5-46cf-b924-edaa95e2bbba">
+             <pre id="550029d5-d190-48f2-acbb-1cab09470cf2"><code class="python">from bootwrap import Panel, Button
+Panel(
+    Button("Google Search").as_primary().link("https://www.google.com/")
+)</code></pre>
+             <div id="9836a231-2aa5-482c-aa09-ec04955d5197">
+              <a class="btn btn-primary" href="https://www.google.com/" id="5200407d-f57f-427b-8617-f37298a1b0ad" role="button">
                Google Search
               </a>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="a7aa8e9c-1379-4468-abec-c10958bfc587">
-        <div class="mt-3" id="0e3e0bfb-3940-4f3e-8f81-1e4681a2bd99">
-         <div id="7fdec717-894a-4ef1-b6a8-fa38c161de3d">
+       <div class="tab-pane fade" id="0f715e53-7ba3-41c5-a5d0-0c17fbf4252a">
+        <div class="mt-3" id="a453b480-c222-41f4-ba05-5195bd65ad61">
+         <div id="6d856cfb-3a59-4416-befc-ec6e8bc602b5">
           <div class="row">
            <div class="col-md">
-            <div id="db09130a-3905-42e6-b4a3-9ac2813dea23">
-             <h1 id="3cf54ecd-a9b6-477f-a936-04ec156378ce">
+            <div id="463f172f-778f-45d6-9856-611fa687bf84">
+             <h1 id="319fa3c2-9bdb-4d89-a6b0-8265c4ef0afe">
               Open Dialog
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="9ac0066e-72b5-4e9b-a0d8-efaeb4633055">
+            <div id="aba6b5af-92bf-4895-bcaa-6b0b775ffde5">
             </div>
            </div>
           </div>
          </div>
-         <div id="f9ffc7ab-06b5-4864-ac09-efed8c5004b7">
+         <div id="1827fc2b-d990-4b3c-91c2-cd7a2671af7b">
           <div class="row">
            <div class="col-md">
-            <div id="efd87fef-d1e1-424f-b551-6a6dde38733d">
-             <p id="511d28c0-48cd-4b33-ae3d-0b1111b9fdfa">
+            <div id="9bda6985-4748-40fb-9451-4b94e6a3ed19">
+             <p id="9146b3e3-f5de-4c3c-bb8c-6df3f72b801a">
               Use
               <code>
                Button
               </code>
               to open a dialog using the
               <code>
                toggle()
               </code>
               function.
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="54e42d07-4155-4c22-957e-c9de374a157e">
-             <pre id="79f3a3f2-20d6-4ea5-9353-86f0581275a2"><code class="python">dialog = Dialog(
+            <div id="4fad689f-0b6e-4e31-8eab-8d6741e2aa95">
+             <pre id="d73258f5-407d-43b8-acb3-a5d6d864c908"><code class="python">from bootwrap import Panel, Dialog, Button
+dialog = Dialog(
   "Greeting",
   "Hello World!"
 )
-button = Button("Say Hello").as_primary().toggle(dialog)</code></pre>
-             <div id="7c7bc64e-433e-4dc2-bacb-b3fbbf39ae08">
-              <div class="modal" id="ec0deb10-d66a-481a-906d-b9932d768226">
+button = Button("Say Hello").as_primary().toggle(dialog)
+Panel(dialog, button)</code></pre>
+             <div id="ab9796bf-b7e1-4c37-b945-3780f77c718a">
+              <div class="modal" id="14dfdd83-b77a-4e67-afcd-1a5cf91c9f77">
                <div class="modal-dialog" role="document">
                 <div class="modal-content">
                  <div class="modal-header">
                   <h5 class="modal-title text-None">
                    Greeting
                   </h5>
                   <button aria-label="Close" class="close" data-dismiss="modal" type="button">
@@ -1340,68 +1389,70 @@
                  </div>
                  <div class="modal-body">
                   Hello World!
                  </div>
                 </div>
                </div>
               </div>
-              <button class="btn btn-primary" data-target="#ec0deb10-d66a-481a-906d-b9932d768226" data-toggle="modal" id="25f2640e-8a18-4684-ad93-7da4e4858119" onclick="return false;" type="button">
+              <button class="btn btn-primary" data-target="#14dfdd83-b77a-4e67-afcd-1a5cf91c9f77" data-toggle="modal" id="732f5c37-e573-476f-a5cf-9fe28535a1b6" onclick="return false;" type="button">
                Say Hello
               </button>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="dd4c1069-bc4f-4820-939e-a43ccf0829ae">
-        <div class="mt-3" id="48595b8b-85a8-421f-a57d-a4cee17edb5b">
-         <div id="22482e6a-186d-4a40-8770-84102a129a9f">
+       <div class="tab-pane fade" id="9788024e-60c1-42bf-9792-a310e1f1c41f">
+        <div class="mt-3" id="579a02ac-7c0e-4586-8a4b-3274219aa9c7">
+         <div id="e0fdf8d4-5871-4454-9bdc-1521bf522189">
           <div class="row">
            <div class="col-md">
-            <div id="dbbb0d60-c118-4d44-a812-054c142a281a">
-             <h1 id="c7b2d59e-282c-4faf-a483-7396e2fe806f">
+            <div id="525f5716-4502-4dfe-99d2-d9e748a618ec">
+             <h1 id="4e45c00f-ad2c-4dc2-9b7c-463061d30a96">
               Close Dialog
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="bb71d2c4-3eaa-416d-ab0c-7a8e4ded5a24">
+            <div id="b8482355-0ebc-4fdc-9049-4c5f0dd6b274">
             </div>
            </div>
           </div>
          </div>
-         <div id="899b7edc-c463-44ef-9846-72d39bffc4fd">
+         <div id="7f444925-d6e5-4ef4-8a15-568392971c25">
           <div class="row">
            <div class="col-md">
-            <div id="9bc69e20-812f-4611-bc2c-d48116d95adb">
-             <p id="9f9b5b62-41e6-445b-b7c6-3ca49b88b29d">
+            <div id="dfbb6233-0e88-4b50-9a5a-f3c90d0fed5e">
+             <p id="732cf92f-dc70-4634-b659-83ec32f45cfb">
               Use
               <code>
                Button
               </code>
               to close a dialog using the
               <code>
                dismiss()
               </code>
               function.
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="68628346-6890-4f41-8ed0-2257cc2ea662">
-             <pre id="27bca140-f454-476f-a1b5-379687dbd776"><code class="python">dialog = Dialog(
+            <div id="67931189-7ae8-49dc-b4c4-cbabcdea61d5">
+             <pre id="6089c106-3de3-4a1d-b936-b5e31ab41cb3"><code class="python">from bootwrap import Panel, Dialog, Button
+dialog = Dialog(
   "Greeting",
   "Hello World!",
   Button("Bye").as_primary().dismiss()
 )
-button = Button("Say Hello").as_primary().toggle(dialog)</code></pre>
-             <div id="9da6f3b1-a480-4ab0-9ca3-3342d4a5945d">
-              <div class="modal" id="66cfe1c0-0aff-4ac1-ada7-7bc105728cf2">
+button = Button("Say Hello").as_primary().toggle(dialog)  
+Panel(dialog, button)</code></pre>
+             <div id="a015067b-84f4-48b4-b951-42aaf42f3e1c">
+              <div class="modal" id="a72808c7-4885-4bc9-ac04-e9b2ac3bb99f">
                <div class="modal-dialog" role="document">
                 <div class="modal-content">
                  <div class="modal-header">
                   <h5 class="modal-title text-None">
                    Greeting
                   </h5>
                   <button aria-label="Close" class="close" data-dismiss="modal" type="button">
@@ -1410,119 +1461,123 @@
                    </span>
                   </button>
                  </div>
                  <div class="modal-body">
                   Hello World!
                  </div>
                  <div class="modal-footer">
-                  <button class="btn btn-primary" data-dismiss="modal" id="c7b3e500-48a7-4ffa-9264-5bb7954c8a1e" onclick="return false;" type="button">
+                  <button class="btn btn-primary" data-dismiss="modal" id="7ee80bcd-e860-4fda-9f08-5748fa4c21ae" onclick="return false;" type="button">
                    Bye
                   </button>
                  </div>
                 </div>
                </div>
               </div>
-              <button class="btn btn-primary" data-target="#66cfe1c0-0aff-4ac1-ada7-7bc105728cf2" data-toggle="modal" id="6d078c5d-652f-4c88-a044-79a235e3e582" onclick="return false;" type="button">
+              <button class="btn btn-primary" data-target="#a72808c7-4885-4bc9-ac04-e9b2ac3bb99f" data-toggle="modal" id="a7cc191b-1503-4bff-b77d-d3da86b16664" onclick="return false;" type="button">
                Say Hello
               </button>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="bb3aa52f-0d51-4a21-ac5d-5e9c93289344">
-        <div class="mt-3" id="27c43927-871b-460e-ab20-6aa7ee05a749">
-         <div id="592cec16-51f5-4c5a-a7a2-3a530fb53dfc">
+       <div class="tab-pane fade" id="8c3bc726-5007-4234-a21d-542129f845c5">
+        <div class="mt-3" id="a2072373-a88a-4ce8-bd44-130da02ef95c">
+         <div id="c07f583e-2f0d-4db8-a861-93b86aef74dc">
           <div class="row">
            <div class="col-md">
-            <div id="fe54a5b1-c6ed-4870-962d-afe06bde5b61">
-             <h1 id="23e8d981-f128-400c-b410-e530b9d200d2">
+            <div id="8744a6cf-a2d9-4e29-bfbe-608425f42ddf">
+             <h1 id="d2c94698-6bba-478e-87c9-c30ee55e51c0">
               Expand/Collapse Panel
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="8492bfb2-b692-4fc1-be53-57d811620ad8">
+            <div id="2d2b1b5f-7a49-41c9-8adb-e42d5f39a776">
             </div>
            </div>
           </div>
          </div>
-         <div id="deb409f4-d3bc-4d68-8bc6-4eff31b630d4">
+         <div id="72162fd8-e04f-4829-8709-cb2e6829983b">
           <div class="row">
            <div class="col-md">
-            <div id="439458e7-72ca-436e-839b-e6903bc580f3">
-             <p id="8e536395-9722-4e6a-a8ae-880de3ef804d">
+            <div id="3678c644-7c64-4a57-a544-6c7a0a7fe6ad">
+             <p id="c0dace19-56d8-4ae6-b08a-aa1a0db1ae4e">
               Use
               <code>
                Button
               </code>
               to expand/collapse a panel using the
               <code>
                toggle()
               </code>
               function.
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="a4102547-2844-4a6f-b1e7-efea94805201">
-             <pre id="8fc35032-9102-433a-a12b-d7f72955f89a"><code class="python">quote = Panel(
+            <div id="091141d3-7559-47e8-ac00-95cada1e1486">
+             <pre id="25ef8f16-0aa6-4059-a5b2-e046ea00bfa4"><code class="python">from bootwrap import Panel, Button
+quote = Panel(
   "Sometimes life is going to hit you in " +
   "the head with a brick. Don’t lose faith."
 ).as_collapse()
-Button("Steve Jobs Quote").as_primary().toggle(quote)</code></pre>
-             <div id="80402087-de39-44bf-9aa6-4e8c499810f4">
-              <button class="btn btn-primary" data-target="#830e1e2e-97e3-4786-bc95-dc6281689fac" data-toggle="collapse" id="b778e38c-24fa-44cb-a294-38c17f97f144" onclick="return false;" type="button">
+Panel(
+  Button("Steve Jobs Quote").as_primary().toggle(quote),
+  quote
+)</code></pre>
+             <div id="5dd1d702-5361-40a2-867f-d761124a025b">
+              <button class="btn btn-primary" data-target="#87957e06-7bc4-475b-99a0-9dd0fe5efc1a" data-toggle="collapse" id="1bce6a87-1f9c-4792-bab2-c1c86f98b7c9" onclick="return false;" type="button">
                Steve Jobs Quote
               </button>
-              <div class="collapse" id="830e1e2e-97e3-4786-bc95-dc6281689fac">
+              <div class="collapse" id="87957e06-7bc4-475b-99a0-9dd0fe5efc1a">
                Sometimes life is going to hit you in the head with a brick. Don’t lose faith.
               </div>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="a58710e1-9bcd-4b72-bbfd-c15ed85a27aa">
-        <div class="mt-3" id="5e9e1897-0432-4069-8c9a-7337b7e8084c">
-         <div id="84200201-d4fd-4377-ad04-a6c7b24fd53b">
+       <div class="tab-pane fade" id="5aa621b3-e462-454b-982e-f69687f7f8d8">
+        <div class="mt-3" id="24cf95cc-2fac-4640-9ce2-a4b51669b40a">
+         <div id="7dbec3c5-152f-46f0-841d-4be70d5c6d23">
           <div class="row">
            <div class="col-md">
-            <div id="7776cdd7-ea46-47df-99f1-f4bbd0d42228">
-             <h1 id="b3499bc2-89d0-48c6-9e0a-a9437dde6121">
+            <div id="a6b8d3a5-0402-4aaf-a798-d5596f6fcf97">
+             <h1 id="f3f80704-a1be-4c1f-a22c-6a42a6b15c9a">
               Submit Action
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="c51ead69-f451-43e4-8d82-ca5ee8ffeb2e">
+            <div id="d9530a41-aec8-4867-87b3-97ede92f5701">
             </div>
            </div>
           </div>
          </div>
-         <div id="f07e39bc-137f-4c4b-883f-b8e8f75e2d6b">
+         <div id="3ee2f7d2-6f24-4f1c-9e6a-6640a5dfb035">
           <div class="row">
            <div class="col-md">
-            <div id="200f2a5e-10c2-449c-a5a4-446b55d82267">
-             <p id="a0a482c9-902f-48be-8790-ab240bb263b6">
+            <div id="968b373c-093b-46c2-b903-deae420d27a9">
+             <p id="5ce9558e-797d-458c-8734-fb76f5c0d1ef">
               Use
               <code>
                Button
               </code>
               to submit form content using the
               <code>
                submit()
               </code>
               function.
              </p>
-             <p id="02b3a286-5a29-4efb-91c3-2633992c0d66">
+             <p id="1ec370a9-74e3-4f18-8987-8c747a4f69ef">
               <strong>
                Note:
               </strong>
               to make a form submit do not forget to use the
               <code>
                Form
               </code>
@@ -1535,87 +1590,88 @@
                Form
               </code>
               documentation.
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="07486693-f1d2-4301-bfe8-82f5a73c3513">
-             <pre id="ae53d5a8-4eec-4193-8f46-37c123c120ca"><code class="python">Form(
+            <div id="49728573-1e77-4962-9fd4-87e4f2e5d15c">
+             <pre id="4f8cef05-45f4-4a47-82c0-9944d342321d"><code class="python">from bootwrap import Form, TextInput, Button
+Form(
   TextInput("Email", "email", "my@email.com").for_email(),
   Button("Send").as_primary().submit()
 )</code></pre>
-             <form enctype="multipart/form-data" id="3484e2ea-1236-4cd7-962f-b70dafcabe27" method="POST">
+             <form enctype="multipart/form-data" id="8c31ef8a-3125-4057-b647-6fb1a23cb42e" method="POST">
               <div class="form-group row">
-               <label class="col-sm-2 col-form-label d-flex align-items-center" for="2e31c84e-0684-4687-83e2-b6b51163c875">
+               <label class="col-sm-4 col-form-label d-flex align-items-center" for="af6e50a0-ef00-4098-987d-c17322eb3027">
                 Email
                </label>
-               <div class="col-sm-10 d-flex align-items-center">
-                <input class="form-control" id="2e31c84e-0684-4687-83e2-b6b51163c875" name="email" type="email" value="my@email.com"/>
+               <div class="col-sm-8 d-flex align-items-center">
+                <input class="form-control" id="af6e50a0-ef00-4098-987d-c17322eb3027" name="email" type="email" value="my@email.com"/>
                </div>
               </div>
-              <button class="btn btn-primary" id="8b9000a4-3aeb-4ef5-820b-b0b2e26829ac" onclick="return false;" type="submit">
+              <button class="btn btn-primary" id="22ff2bb8-7e11-40db-bf5b-948c048f42be" type="submit">
                Send
               </button>
              </form>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="347e8840-54b9-4441-b8bd-9eeff202ea41">
-     <div id="2aea867d-5d32-4501-8227-7d012426885b">
+    <div class="tab-pane fade" id="5f884099-12db-4603-8dd0-1dd887e53bc7">
+     <div id="55fea7be-2e05-43ab-910c-c335ef8a4232">
       <hr/>
-      <ul class="nav" id="40dc939f-c9a9-4059-bc66-bd6b4cad460c" role="tablist">
+      <ul class="nav" id="b2b8aa81-0e81-458a-ae2f-052821f64fae" role="tablist">
        <li class="nav-item">
-        <a class="nav-link active" data-target="#9726e3be-7ed9-4c3a-8efc-e04ff6b9d619" data-toggle="tab" href="#9726e3be-7ed9-4c3a-8efc-e04ff6b9d619" id="59e54784-9b1a-487f-9261-c40481119032" role="tab">
-         <span class="text-secondary" id="ae9bdb28-4bb4-417e-b195-49d3370f6e6d">
+        <a class="nav-link active" data-target="#4c8e66da-488a-4cdb-b73b-9af1581e8997" data-toggle="tab" href="#4c8e66da-488a-4cdb-b73b-9af1581e8997" id="91fa75a2-5f2c-42d8-a2f8-60be642ffb10" role="tab">
+         <span class="text-secondary" id="88b28629-7aa3-465f-9e55-4bed6464fe93">
           Deck
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#7ece1383-b4c6-46db-b063-16c0904744da" data-toggle="tab" href="#7ece1383-b4c6-46db-b063-16c0904744da" id="dc791a37-425f-4b82-898a-e7fa9a2e855f" role="tab">
-         <span class="text-secondary" id="0e6353e6-24bf-4141-92d4-39559e2b29a0">
+        <a class="nav-link" data-target="#48f43a7c-0866-40cd-a85f-5d17a84e42fa" data-toggle="tab" href="#48f43a7c-0866-40cd-a85f-5d17a84e42fa" id="f275ea2e-d3a6-4f19-9086-911741a18647" role="tab">
+         <span class="text-secondary" id="e04e083d-d194-4df1-9572-2f946bb14e46">
           Deck.Card
          </span>
         </a>
        </li>
       </ul>
       <div class="tab-content">
-       <div class="tab-pane fade active show" id="9726e3be-7ed9-4c3a-8efc-e04ff6b9d619">
-        <div class="mt-5" id="5bc46fbd-bed0-4763-b4d2-c2c3194a907e">
-         <div class="d-flex justify-content-between" id="7015e977-d940-45d2-b901-55387fcabddc">
-          <h1 id="e771fa24-a61d-48ad-9fc8-2e9914208e34">
+       <div class="tab-pane fade active show" id="4c8e66da-488a-4cdb-b73b-9af1581e8997">
+        <div class="mt-5" id="897df209-6d8a-4320-bc26-a0a4a7187513">
+         <div class="d-flex justify-content-between" id="b67a7427-a0d1-460b-be6a-5196489d8733">
+          <h1 id="081f5f53-6a40-46c5-849b-26f7d8cd71c7">
            Class
-           <span class="text-primary" id="ed11ca2f-6c8d-419c-b979-472799d14ffe">
+           <span class="text-primary" id="b6f57786-3443-4b50-beac-ba5d1bac6dab">
             Deck
            </span>
           </h1>
-          <div id="01d944a9-de37-4e5e-b013-5c2d95d370c8">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#107fd47c-ec10-40c5-95b7-af65e8a31095" data-toggle="collapse" id="4c998418-f9c8-413e-a0d4-a40a8325fe68" onclick="return false;" type="button">
+          <div id="e5e30006-0d2a-408b-a149-fb60a97aa202">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#f0ef6a79-803e-43a2-a29f-e663e512c7fb" data-toggle="collapse" id="b83b4922-6ce8-4492-8f0d-8ff043738336" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="e4a6cd31-a988-4810-a714-f8e2392605c4">
+         <span class="text-muted" id="3ad226af-f4f7-40d0-8bcf-8516febac4b3">
           A web component for a deck of cards.
          </span>
-         <pre id="2ab0f7fc-8090-4100-ac5d-77d0bb637ebf"><code class="python">Deck(*cards)</code></pre>
-         <div class="ml-3 collapse" id="107fd47c-ec10-40c5-95b7-af65e8a31095">
-          <h6 id="4be2333c-9c30-4162-a1eb-253d9579e7e0">
+         <pre id="1165435f-17c5-480c-8f5c-511ec445903a"><code class="python">Deck(*cards)</code></pre>
+         <div class="ml-3 collapse" id="f0ef6a79-803e-43a2-a29f-e663e512c7fb">
+          <h6 id="9fc6822c-189d-401c-8faa-31c3ec544e79">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="09ddab51-9911-4f4f-ae96-5904716b64f0">
+          <table class="table table-sm bg-light" id="559bc70c-fb3d-4fd7-a6af-465b6862126c">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -1648,21 +1704,21 @@
               </code>
               elements.
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <div class="ml-3" id="54338241-a42b-49df-af1c-c2e803179332">
-          <h6 id="91026691-3840-478c-bea2-6b05c13cc94e">
+         <div class="ml-3" id="c41f4cff-a1df-4b5a-ba7c-471fac6b5ee3">
+          <h6 id="2858c31f-1491-4171-8e22-da484ecf5e2c">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="746ea32f-0e02-43fb-8177-015eabf04ce1"><code class="python">from bootwrap import Button, Deck, Image
+          <pre id="041cdcc0-b038-40f4-aeb9-890051b86dfc"><code class="python">from bootwrap import Button, Deck, Image
 
 actions = [
     Button("Buy"),
     Button("Sell"),
     Button("Transfer")
 ]
 
@@ -1684,162 +1740,159 @@
     Deck.Card(
         "Amazon (NASDAQ: AMZN)",
         description= "Price for a single Amazon share",
         figure=Image("amazon-logo.png", width=128).mt(3),
         marker="12:04:58 12/01/2021"
     ).add_menu(*actions).pack_actions().link(
         "https://www.amazon.com")
-)</code></pre>
+)
+</code></pre>
          </div>
-         <div class="ml-3" id="fc96fbd2-2176-46e1-8b57-d5c5d4aae147">
-          <div class="card-deck grid-container" id="1336acb3-f12b-4e72-ae30-66d433f8e8fa">
-           <a class="card" href="https://www.google.com" id="7dd45d60-6fbb-4424-b009-07f5f1fc1581">
-            <div class="row justify-content-center">
-             <img class="mt-3" id="4c0c1a36-433c-450e-aa6f-de9ff6f08056" src="google-logo.png" width="128"/>
+         <div class="ml-3" id="b999fd64-f234-4244-b832-8d551538ad3f">
+          <div class="card-deck grid-container" id="eaacd0c3-d88e-4092-989c-bfe07e0fc301">
+           <div class="card" id="66a2f7b0-e3cb-43f6-9406-03341f9c9a33">
+            <div class="row justify-content-center" onclick="location.href='https://www.google.com';">
+             <img class="mt-3" id="a0d86873-e64b-483b-be05-ab776735ece5" src="google-logo.png" width="128"/>
             </div>
-            <div class="card-body">
+            <div class="card-body" onclick="location.href='https://www.google.com';">
              <div class="text-right mb-2">
-              <span class="text-muted" id="a67405b9-281c-46ea-bd5f-5b1dc51a14f9">
+              <span class="text-muted" id="f98c237e-82e5-4dc9-88bb-3147661cc8f7">
                <small>
                 12:04:58 12/01/2021
                </small>
               </span>
              </div>
-             <h5 class="card-title" id="3142f17b-cfed-4622-979f-6af732c1bfef">
+             <h5 class="card-title" id="953c4ab8-404c-4b39-b3bd-5d0a20525a11">
               Google (NASDAQ: GOOGL)
              </h5>
              Price for a single Google share
             </div>
             <div class="card-footer text-right">
              <div class="btn-group">
-              <i class="btn fas fa-ellipsis-v" data-toggle="dropdown" id="97a60353-5c6a-48ab-a207-7e7c360d494d" onclick="return false;" style="cursor: pointer">
+              <i class="btn fas fa-ellipsis-v" data-toggle="dropdown" id="570dea1c-2c0c-4097-af58-7a74fe78209d" onclick="return false;" style="cursor: pointer">
               </i>
               <div class="dropdown-menu dropdown-menu-right">
-               <button class="dropdown-item btn" id="61d517ca-150c-44f1-969f-e922de325a63" onclick="return false;">
+               <button class="dropdown-item btn" id="abacbff6-65bf-4ca7-abc4-97fe60e00a18" onclick="return false;">
                 Buy
                </button>
-               <button class="dropdown-item btn" id="240f4b03-5aa4-4f4b-91c4-35eb145427eb" onclick="return false;">
+               <button class="dropdown-item btn" id="fc0cc454-8c80-4128-98e8-d0746271002d" onclick="return false;">
                 Sell
                </button>
-               <button class="dropdown-item btn" id="75a897b2-790a-4ca4-badc-7c2f47a502c8" onclick="return false;">
+               <button class="dropdown-item btn" id="efacbca2-915f-4ac6-b016-272952e1a7e7" onclick="return false;">
                 Transfer
                </button>
               </div>
              </div>
             </div>
-           </a>
-           <a class="card" href="https://www.linkedin.com" id="dd65c304-d432-4545-908a-cca2c2b744a2">
-            <div class="row justify-content-center">
-             <img class="mt-3" id="81085ca3-944c-4dba-8aea-bc92305aa997" src="linkedin-logo.png" width="128"/>
+           </div>
+           <div class="card" id="a454c7a7-a66d-470b-bd07-d7c320c7c3dd">
+            <div class="row justify-content-center" onclick="location.href='https://www.linkedin.com';">
+             <img class="mt-3" id="7be3dbec-8377-4674-ab35-e8aac071d8d6" src="linkedin-logo.png" width="128"/>
             </div>
-            <div class="card-body">
+            <div class="card-body" onclick="location.href='https://www.linkedin.com';">
              <div class="text-right mb-2">
-              <span class="text-muted" id="017eb4aa-c500-4d01-a044-307d522ce3c6">
+              <span class="text-muted" id="13eacb6c-89fd-494d-9167-67b9760c3f40">
                <small>
                 12:04:58 12/01/2021
                </small>
               </span>
              </div>
-             <h5 class="card-title" id="a6b740e5-a417-4717-a3f6-5a26f79db601">
+             <h5 class="card-title" id="ade177de-d346-45a4-8028-8a35b131d178">
               LinkedIn (NASDAQ: LNKD)
              </h5>
              Price for a single LinkedIn share
             </div>
             <div class="card-footer text-right">
              <div class="btn-group">
-              <i class="btn fas fa-ellipsis-v" data-toggle="dropdown" id="13cd98af-2b05-4dc3-b9d3-53c73eaa05f8" onclick="return false;" style="cursor: pointer">
+              <i class="btn fas fa-ellipsis-v" data-toggle="dropdown" id="86a6dcc7-b944-4254-9855-8c557ed782be" onclick="return false;" style="cursor: pointer">
               </i>
               <div class="dropdown-menu dropdown-menu-right">
-               <button class="dropdown-item btn" id="61d517ca-150c-44f1-969f-e922de325a63" onclick="return false;">
+               <button class="dropdown-item btn" id="abacbff6-65bf-4ca7-abc4-97fe60e00a18" onclick="return false;">
                 Buy
                </button>
-               <button class="dropdown-item btn" id="240f4b03-5aa4-4f4b-91c4-35eb145427eb" onclick="return false;">
+               <button class="dropdown-item btn" id="fc0cc454-8c80-4128-98e8-d0746271002d" onclick="return false;">
                 Sell
                </button>
-               <button class="dropdown-item btn" id="75a897b2-790a-4ca4-badc-7c2f47a502c8" onclick="return false;">
+               <button class="dropdown-item btn" id="efacbca2-915f-4ac6-b016-272952e1a7e7" onclick="return false;">
                 Transfer
                </button>
               </div>
              </div>
             </div>
-           </a>
-           <a class="card" href="https://www.amazon.com" id="0c5035d0-74f6-4673-8d6a-6598b82e9553">
-            <div class="row justify-content-center">
-             <img class="mt-3" id="22fefecc-f4fb-4ed3-beef-cc5db6b29275" src="amazon-logo.png" width="128"/>
+           </div>
+           <div class="card" id="2c510f0b-66f5-4ed9-b894-ccddc6b1783f">
+            <div class="row justify-content-center" onclick="location.href='https://www.amazon.com';">
+             <img class="mt-3" id="d3d37c05-2fbb-49af-92d9-0069f8537db5" src="amazon-logo.png" width="128"/>
             </div>
-            <div class="card-body">
+            <div class="card-body" onclick="location.href='https://www.amazon.com';">
              <div class="text-right mb-2">
-              <span class="text-muted" id="09eee7d8-a2a2-4cbb-bb58-d8cab9e8ee3a">
+              <span class="text-muted" id="e905e38a-9d41-4b5e-9fe4-8ef7480714c7">
                <small>
                 12:04:58 12/01/2021
                </small>
               </span>
              </div>
-             <h5 class="card-title" id="bbf7c4d3-54f3-4ced-961a-61f5042c6f4e">
+             <h5 class="card-title" id="618fa2c5-c5fd-4c8b-b356-c8b11fbbbd1f">
               Amazon (NASDAQ: AMZN)
              </h5>
              Price for a single Amazon share
             </div>
             <div class="card-footer text-right">
              <div class="btn-group">
-              <i class="btn fas fa-ellipsis-v" data-toggle="dropdown" id="e0491465-f381-4984-8fb6-ede584feb570" onclick="return false;" style="cursor: pointer">
+              <i class="btn fas fa-ellipsis-v" data-toggle="dropdown" id="682f9027-4c4a-403b-8df8-f10f45bf62f0" onclick="return false;" style="cursor: pointer">
               </i>
               <div class="dropdown-menu dropdown-menu-right">
-               <button class="dropdown-item btn" id="61d517ca-150c-44f1-969f-e922de325a63" onclick="return false;">
+               <button class="dropdown-item btn" id="abacbff6-65bf-4ca7-abc4-97fe60e00a18" onclick="return false;">
                 Buy
                </button>
-               <button class="dropdown-item btn" id="240f4b03-5aa4-4f4b-91c4-35eb145427eb" onclick="return false;">
+               <button class="dropdown-item btn" id="fc0cc454-8c80-4128-98e8-d0746271002d" onclick="return false;">
                 Sell
                </button>
-               <button class="dropdown-item btn" id="75a897b2-790a-4ca4-badc-7c2f47a502c8" onclick="return false;">
+               <button class="dropdown-item btn" id="efacbca2-915f-4ac6-b016-272952e1a7e7" onclick="return false;">
                 Transfer
                </button>
               </div>
              </div>
             </div>
-           </a>
+           </div>
           </div>
           <style>
-           a.card {
-                    text-decoration: none;
-                }
-
-                a.card, a.card:visited, a.card:hover, a.card:active {
-                    color: inherit;
+           div.card {
+                    cursor:pointer
                 }
           </style>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="7ece1383-b4c6-46db-b063-16c0904744da">
-        <div class="mt-5" id="b691b384-44fd-4365-96bd-2ba385476fbe">
-         <div class="d-flex justify-content-between" id="6ab72deb-3d09-4a9c-9ae2-e1fd98ae4fa1">
-          <h1 id="4e84f2eb-f9e7-4589-98da-8187316bc6f4">
+       <div class="tab-pane fade" id="48f43a7c-0866-40cd-a85f-5d17a84e42fa">
+        <div class="mt-5" id="334e658f-b7de-42b0-bdc9-7e4eed2380fe">
+         <div class="d-flex justify-content-between" id="613036db-de3b-4a81-b809-92611752f3b6">
+          <h1 id="4afec6b5-da35-4b32-a8a8-17ca81c11830">
            Class
-           <span class="text-primary" id="ce82474a-975e-4408-bbe0-912a56a5eed8">
+           <span class="text-primary" id="89b1a940-319a-45d9-af99-ec7292213ed2">
             Deck.Card
            </span>
           </h1>
-          <div id="08e44917-0759-4f70-8fe0-05cb69789faa">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#642cafcb-0d78-4bba-8599-fd9e2738f252" data-toggle="collapse" id="d6310e68-9c52-432d-b513-3b2b20e342f4" onclick="return false;" type="button">
+          <div id="50acbfe2-79eb-40ec-93a0-c8af1bd26183">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#492f77b6-cb7c-4064-a703-26a2c91ce673" data-toggle="collapse" id="1beefe19-c035-48b3-8137-0d399fb0af25" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="4f0bada4-f04e-4d02-a9d2-f1bc5b2bafb7">
+         <span class="text-muted" id="c17fda88-660b-4ae7-bb59-a04688035ccd">
           A deck card.
          </span>
-         <pre id="b8d1b00c-3330-4c49-8772-311aec417b5a"><code class="python">Deck.Card(title, description=None, marker=None, figure=None)</code></pre>
-         <div class="ml-3 collapse" id="642cafcb-0d78-4bba-8599-fd9e2738f252">
-          <h6 id="d3c6886b-00d5-4276-bf6f-c1e79361fa4b">
+         <pre id="4f0c564e-6572-436c-94ae-6d5f19eedd00"><code class="python">Deck.Card(title, description=None, marker=None, figure=None)</code></pre>
+         <div class="ml-3 collapse" id="492f77b6-cb7c-4064-a703-26a2c91ce673">
+          <h6 id="9c59ad72-fb47-4ed7-aa7d-f471c50be4e6">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="701ee3ab-7dbe-403a-a354-65d273dbd3e9">
+          <table class="table table-sm bg-light" id="b3495891-9342-48d7-b655-5692ef357073">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -1909,200 +1962,202 @@
              <td>
               The card figure.
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <div class="ml-3" id="96bc13f7-3d02-41fb-9c06-7c7fde626c9b">
-          <h6 id="7da2b802-8e86-4968-bc69-405d8237652d">
+         <div class="ml-3" id="356ef985-0830-4cff-82a9-f0c9e716d11c">
+          <h6 id="51b9e9f8-799a-471b-b8cc-399a002bb5e5">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="c065a0ef-ed3a-47f5-8e15-76f77df718cd"><code class="python">from bootwrap import Button, Deck, Image
+          <pre id="192aa8d8-7af8-423b-b5c9-aa9c7777d0b3"><code class="python">from bootwrap import Button, Deck, Image
 
 actions = [
     Button("Buy"),
     Button("Sell"),
     Button("Transfer")
 ]
 
 Deck.Card(
     "Google (NASDAQ: GOOGL)",
     description= "Price for a single Google share",
     figure=Image("google-logo.png", width=128).mt(3),
     marker="12:04:58 12/01/2021"
 ).add_menu(*actions).link(
-    "https://www.google.com")</code></pre>
+    "https://www.google.com")
+</code></pre>
          </div>
-         <div class="ml-3" id="85a088b0-fe0b-47b2-83be-49f8d1590ee3">
-          <a class="card" href="https://www.google.com" id="212b3467-2387-4638-b0f8-0d4651417ee5">
-           <div class="row justify-content-center">
-            <img class="mt-3" id="d4e27c06-e071-4f59-80d7-07cce5348241" src="google-logo.png" width="128"/>
+         <div class="ml-3" id="5991183f-6da9-4d68-8e28-e1e8e889e138">
+          <div class="card" id="ef2c688d-1afc-4120-8327-9e54b68988d1">
+           <div class="row justify-content-center" onclick="location.href='https://www.google.com';">
+            <img class="mt-3" id="5c5385b6-e18a-43a3-aec4-a8c32a20c7b3" src="google-logo.png" width="128"/>
            </div>
-           <div class="card-body">
+           <div class="card-body" onclick="location.href='https://www.google.com';">
             <div class="text-right mb-2">
-             <span class="text-muted" id="3b7984e4-085a-41f9-b6fb-69b3d40df42c">
+             <span class="text-muted" id="91b7dc12-f335-4a47-b689-c49633363f09">
               <small>
                12:04:58 12/01/2021
               </small>
              </span>
             </div>
-            <h5 class="card-title" id="e5e13832-0721-4950-a193-6408fca1338b">
+            <h5 class="card-title" id="02f04c8e-2d90-4920-89a2-fe3b934e41cd">
              Google (NASDAQ: GOOGL)
             </h5>
             Price for a single Google share
            </div>
            <div class="card-footer text-right">
-            <button class="ml-1 btn" id="0250dde2-98c6-4668-9205-296c3447772b" onclick="return false;">
+            <button class="btn" id="24e13572-3911-49e4-a19c-587a1d69899b" onclick="return false;">
              Buy
             </button>
-            <button class="ml-1 btn" id="3128f86e-c21e-4262-9526-a79819d4eee3" onclick="return false;">
+            <button class="btn" id="aba7cb11-3a8a-46bc-b060-2c9624cdce04" onclick="return false;">
              Sell
             </button>
-            <button class="ml-1 btn" id="fe44465a-79f2-403d-8ef1-a4bc1f132137" onclick="return false;">
+            <button class="btn" id="47d87668-cfff-4db7-9786-1aec9ebda4fc" onclick="return false;">
              Transfer
             </button>
            </div>
-          </a>
+          </div>
          </div>
-         <div class="mt-5" id="ea573a01-8b47-4859-a066-3d907cb7f5f2">
-          <div class="d-flex justify-content-between" id="7f78dedf-2ac7-4249-bc28-f1b72d3e08cc">
-           <h4 id="d608990b-2a9b-4803-8516-dcd0ccf60b43">
+         <div class="mt-5" id="470fbd90-d9f7-4026-856a-be77802c88b8">
+          <div class="d-flex justify-content-between" id="fbf22d63-089f-45a9-ba07-9a50cdd84df5">
+           <h4 id="5b26ea8f-8597-463c-b67e-99198fcb33a8">
             Method
-            <span class="text-primary" id="cfb5ec99-1189-47c6-a927-5fe76bc97a1f">
+            <span class="text-primary" id="192a2da5-ef93-4426-8b07-9bc879e6a60e">
              pack_actions
             </span>
            </h4>
-           <div id="d0f15c3d-5806-4b91-b1fa-8395e862ccff">
+           <div id="9df926cd-0aaa-494d-8b08-c9ba243783d7">
            </div>
           </div>
-          <span class="text-muted" id="0b30f1cf-7217-4cc5-9b86-74a61d9e968c">
+          <span class="text-muted" id="0292fb14-7b5b-4733-9032-76c374cedb10">
            Makes item actions packed under a drop-down menu.
           </span>
-          <pre id="5ebdd6fe-edf8-4032-9d59-a40c0b2734cb"><code class="python">pack_actions()</code></pre>
-          <div class="ml-3" id="dd82772d-dc2d-4d7b-9696-fb67a28db245">
-           <h6 id="f3083ce6-cbfc-42db-b8a8-7ab97debc592">
+          <pre id="47b61121-37cd-4b9a-8ba8-95bd4dacdb21"><code class="python">pack_actions()</code></pre>
+          <div class="ml-3" id="d75aaffe-127f-460a-8de0-7e654adc0e60">
+           <h6 id="b66c6338-14fa-46f3-a83c-939399931421">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="b29e345c-98b9-40a9-b761-cc206c7a8d92"><code class="python">from bootwrap import Button, Deck, Image
+           <pre id="8585ec80-423c-49c8-9fbf-bff5842f0f52"><code class="python">from bootwrap import Button, Deck, Image
 
 actions = [
     Button("Buy"),
     Button("Sell"),
     Button("Transfer")
 ]
 
 Deck.Card(
     "Google (NASDAQ: GOOGL)",
     description= "Price for a single Google share",
     figure=Image("google-logo.png", width=128).mt(3),
     marker="12:04:58 12/01/2021"
 ).add_menu(*actions).pack_actions().link(
-    "https://www.google.com")</code></pre>
+    "https://www.google.com")
+</code></pre>
           </div>
-          <div class="ml-3" id="7ad71bc1-4f3a-45da-87b9-02bf6cb5452d">
-           <a class="card" href="https://www.google.com" id="9f431ce5-158a-41b7-a78e-8bcddf4f203f">
-            <div class="row justify-content-center">
-             <img class="mt-3" id="37756059-2abb-4152-9db2-056fa53e4ee0" src="google-logo.png" width="128"/>
+          <div class="ml-3" id="5dffcbba-0609-4f68-b9df-cea2b46de26f">
+           <div class="card" id="961e677a-7087-4172-b6c7-7b496289d14e">
+            <div class="row justify-content-center" onclick="location.href='https://www.google.com';">
+             <img class="mt-3" id="e73bb067-809b-4a86-9922-51703aa59327" src="google-logo.png" width="128"/>
             </div>
-            <div class="card-body">
+            <div class="card-body" onclick="location.href='https://www.google.com';">
              <div class="text-right mb-2">
-              <span class="text-muted" id="fa765eeb-910e-4ec2-8f31-bb612f3cf08c">
+              <span class="text-muted" id="14323928-acc2-449b-837b-92d542c2c370">
                <small>
                 12:04:58 12/01/2021
                </small>
               </span>
              </div>
-             <h5 class="card-title" id="7e5513a0-54bc-4a26-9e48-8df9b0d20025">
+             <h5 class="card-title" id="8c4c90b7-e195-45ba-9afa-553ee1e86942">
               Google (NASDAQ: GOOGL)
              </h5>
              Price for a single Google share
             </div>
             <div class="card-footer text-right">
              <div class="btn-group">
-              <i class="btn fas fa-ellipsis-v" data-toggle="dropdown" id="887ef197-5a38-4715-8431-8397848a673a" onclick="return false;" style="cursor: pointer">
+              <i class="btn fas fa-ellipsis-v" data-toggle="dropdown" id="a13c9ada-cdbe-463f-b222-109ea73fd713" onclick="return false;" style="cursor: pointer">
               </i>
               <div class="dropdown-menu dropdown-menu-right">
-               <button class="dropdown-item btn" id="aa51291c-e200-4a5f-a58f-e53ecac04d91" onclick="return false;">
+               <button class="dropdown-item btn" id="999c66b4-0698-40fb-ac7d-c5e4a0221edf" onclick="return false;">
                 Buy
                </button>
-               <button class="dropdown-item btn" id="95045bc6-d007-48c1-9ad9-511bfeaea67c" onclick="return false;">
+               <button class="dropdown-item btn" id="cf2a8860-cea1-4975-929a-e3c68dd4ddd4" onclick="return false;">
                 Sell
                </button>
-               <button class="dropdown-item btn" id="c65c9c5a-5cea-4505-94e1-eb4a4f21664c" onclick="return false;">
+               <button class="dropdown-item btn" id="92e85bb5-8987-435f-bdcd-0898c818c5a3" onclick="return false;">
                 Transfer
                </button>
               </div>
              </div>
             </div>
-           </a>
+           </div>
           </div>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="f3fe07ea-df57-44b0-9175-c6ca9aa01de6">
-     <div id="82f97aff-1ae9-4dbe-a254-3056d8052fe8">
+    <div class="tab-pane fade" id="3f8a4e63-08fe-44c1-9d8d-0b3f12c00fb7">
+     <div id="a009c452-719a-4bbe-b06f-73f4b5991be1">
       <hr/>
-      <ul class="nav" id="32d558a7-0a7f-4a94-9180-3b2bc024890a" role="tablist">
+      <ul class="nav" id="59e9f6d0-7988-49b3-9a64-4e200715eef4" role="tablist">
        <li class="nav-item">
-        <a class="nav-link active" data-target="#52a083a4-e0e3-4332-a64c-a54737e7449b" data-toggle="tab" href="#52a083a4-e0e3-4332-a64c-a54737e7449b" id="0883e6f6-cefb-4673-a1ba-17d6d9c7e484" role="tab">
-         <span class="text-secondary" id="4a4fe520-28f6-4d2a-ae2c-bbde43841259">
+        <a class="nav-link active" data-target="#f2182333-5dae-4c31-a6eb-89557515fa05" data-toggle="tab" href="#f2182333-5dae-4c31-a6eb-89557515fa05" id="19d0c930-39cc-4811-80fe-9d34ac2bcc31" role="tab">
+         <span class="text-secondary" id="8bafe360-3957-4704-a86f-0615a7b7a1f3">
           Dialog
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#13352493-a662-4add-b2b7-6c509d998a06" data-toggle="tab" href="#13352493-a662-4add-b2b7-6c509d998a06" id="e2a86d1f-3f47-4745-948a-254d9b0e14bc" role="tab">
-         <span class="text-secondary" id="905850ff-5c6a-4ca3-8a6e-1920c8820427">
+        <a class="nav-link" data-target="#0363063c-393c-45c0-8e9a-2bff9c92932f" data-toggle="tab" href="#0363063c-393c-45c0-8e9a-2bff9c92932f" id="f6bc6015-8da0-4684-a219-6f6a0134de52" role="tab">
+         <span class="text-secondary" id="70295b10-595a-4359-b1be-f5edb3708f40">
           Question Dialog
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#fe4e79ff-990c-43da-92e7-1117f47ae138" data-toggle="tab" href="#fe4e79ff-990c-43da-92e7-1117f47ae138" id="f0f071ed-de9a-4cb6-84ac-3d8d9356638c" role="tab">
-         <span class="text-secondary" id="0ba48b62-40ff-4eaf-b3df-99cd523b30da">
+        <a class="nav-link" data-target="#1f1488a0-4796-4b67-a6df-b078a7c6272a" data-toggle="tab" href="#1f1488a0-4796-4b67-a6df-b078a7c6272a" id="5c5d3a2d-1455-4f50-84f7-89f0c447ba0a" role="tab">
+         <span class="text-secondary" id="f4ca1410-524c-43a7-bdac-ba694d495e05">
           Complex Dialog
          </span>
         </a>
        </li>
       </ul>
       <div class="tab-content">
-       <div class="tab-pane fade active show" id="52a083a4-e0e3-4332-a64c-a54737e7449b">
-        <div class="mt-5" id="f76e9165-09c7-49fc-bd2d-87ff40e3e0e7">
-         <div class="d-flex justify-content-between" id="db35547f-88f8-4d22-9dea-03985bd768ce">
-          <h1 id="e05930ee-f321-4aed-8608-e11034207a8b">
+       <div class="tab-pane fade active show" id="f2182333-5dae-4c31-a6eb-89557515fa05">
+        <div class="mt-5" id="4da2e4af-6994-42bb-8571-bee45c354010">
+         <div class="d-flex justify-content-between" id="e276426a-9b53-4a8d-93aa-7745e8cc98c1">
+          <h1 id="c6775e40-d259-4dd3-b0eb-3e0a15b7a187">
            Class
-           <span class="text-primary" id="f5b3aaad-6655-4aa8-acdf-4c7f224097ff">
+           <span class="text-primary" id="941e13be-b76c-426c-b849-be5850b20003">
             Dialog
            </span>
           </h1>
-          <div id="bbea2d54-002b-4507-9b53-14896af8de07">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#6f2e765a-51de-4037-ac93-b9eff37c0f26" data-toggle="collapse" id="183dd2a8-a838-4cb2-96f2-eb2f82f405c5" onclick="return false;" type="button">
+          <div id="37138006-f6b7-4a61-876a-f0fbff71274f">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#f9f44e69-257d-485c-9458-324ffbfb83aa" data-toggle="collapse" id="e4a6a05b-6030-467b-aa99-0231460bba5b" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="d7be8b1f-16da-4e80-b63d-58422def5ad7">
+         <span class="text-muted" id="1a4a873b-3d79-4e9e-90e8-6637befd2baf">
           A dialog.
          </span>
-         <pre id="66869f66-81b9-421b-b9b8-08a259b49b63"><code class="python">Dialog(title, content, *actions)</code></pre>
-         <div class="ml-3 collapse" id="6f2e765a-51de-4037-ac93-b9eff37c0f26">
-          <h6 id="6099c37c-f5e5-4b66-b92c-61369942f769">
+         <pre id="e7da17b0-1eb7-44e5-bfb5-c55b8c9ac88b"><code class="python">Dialog(title, content, *actions)</code></pre>
+         <div class="ml-3 collapse" id="f9f44e69-257d-485c-9458-324ffbfb83aa">
+          <h6 id="d4325bf4-5418-4eb5-a4b0-1877d4c2efdd">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="7b3a06d5-783f-414c-918f-2b9de7d4e9e4">
+          <table class="table table-sm bg-light" id="be81ae08-eeb7-4f1d-b109-902be4ae2869">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -2157,32 +2212,35 @@
              <td>
               The dialog actions.
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <div class="ml-3" id="a8e9c8fb-a50a-4a10-a21b-c1d41277aa41">
-          <h6 id="05505fb6-af35-442b-a1e9-2a7d8bd9180c">
+         <div class="ml-3" id="41eb06aa-3261-4a7c-8246-062649526e9f">
+          <h6 id="639b699e-68dd-4b99-9fbb-5f19d7f73e10">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="0e636240-70ef-433a-8045-aabd44a39090"><code class="python">from bootwrap import Dialog, Button
+          <pre id="2d97b6c8-2811-4316-b3da-04ccb6366d2a"><code class="python">from bootwrap import Panel, Dialog, Button
 
 dialog = Dialog(
     'Greeting',
     'Hello World!',
     Button('Bye').dismiss()
 )
-button = Button('Say Hello').toggle(dialog)</code></pre>
+button = Button('Say Hello').toggle(dialog)
+
+Panel(dialog, button)
+</code></pre>
          </div>
-         <div class="ml-3" id="91c761ac-f79a-49a6-be1e-bc98cde7d244">
-          <div id="83d377f4-3766-4524-afc0-38537e204446">
-           <div class="modal" id="2f2efa4e-e9f6-425e-9f40-35ce521e4858">
+         <div class="ml-3" id="7a0ae7ad-aa43-442d-bce0-0cac48fc9bc4">
+          <div id="6e69158d-c079-4ee1-9119-12a8d323e347">
+           <div class="modal" id="393bb12b-8191-40bf-8067-96788d6f35c2">
             <div class="modal-dialog" role="document">
              <div class="modal-content">
               <div class="modal-header">
                <h5 class="modal-title text-None">
                 Greeting
                </h5>
                <button aria-label="Close" class="close" data-dismiss="modal" type="button">
@@ -2191,50 +2249,50 @@
                 </span>
                </button>
               </div>
               <div class="modal-body">
                Hello World!
               </div>
               <div class="modal-footer">
-               <button class="btn" data-dismiss="modal" id="f9437c89-2d78-4b41-837d-cc9f32058b16" onclick="return false;" type="button">
+               <button class="btn" data-dismiss="modal" id="326e2197-4f99-4cc8-94a0-34a7718899b2" onclick="return false;" type="button">
                 Bye
                </button>
               </div>
              </div>
             </div>
            </div>
-           <button class="btn" data-target="#2f2efa4e-e9f6-425e-9f40-35ce521e4858" data-toggle="modal" id="4ae7da9e-72ad-4921-b419-f972e0dfbf02" onclick="return false;" type="button">
+           <button class="btn" data-target="#393bb12b-8191-40bf-8067-96788d6f35c2" data-toggle="modal" id="a1fcf3be-7bce-4f23-9c36-90c8d5d55764" onclick="return false;" type="button">
             Say Hello
            </button>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="13352493-a662-4add-b2b7-6c509d998a06">
-        <div class="mt-3" id="a4b1d3ea-281c-4c75-964b-d4693b911aa6">
-         <div id="d83cf5e3-bde6-452f-8a31-c98671bdf609">
+       <div class="tab-pane fade" id="0363063c-393c-45c0-8e9a-2bff9c92932f">
+        <div class="mt-3" id="eb6417c9-9323-4d41-b6c5-3e2c94e95874">
+         <div id="1aa4503d-7b76-4b20-8b82-dd3b8f918605">
           <div class="row">
            <div class="col-md">
-            <div id="bc6777cc-28c2-4d6c-9547-0efb1966a7c0">
-             <h1 id="bdccc22a-bfc3-4085-846e-0b3616535fd5">
+            <div id="38a7e17b-17a1-47d7-8999-d8a8d682fb96">
+             <h1 id="400b745f-afbd-45a8-90a0-9cd721738835">
               Question Dialog
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="e9f151fc-8b6f-4019-9cbe-c1702ad975b6">
+            <div id="24d9fe64-8f2c-4dc9-b724-c55ba285a429">
             </div>
            </div>
           </div>
          </div>
-         <div id="57cef444-7a91-451b-81be-5da80026715d">
+         <div id="4f1048a3-52a9-4823-ae2f-07b037aebc07">
           <div class="row">
            <div class="col-md">
-            <div id="c6e183b9-35ab-4e2d-ab7f-f89d069ebce2">
-             <p id="4ce1d018-d598-416b-b7ee-4e7756b7c98b">
+            <div id="6c427d45-95b3-4456-b994-e261ad9481ea">
+             <p id="96ec0dea-21c4-4ee5-b56a-8869bc9e1fcf">
               An example of how
               <code>
                Dialog
               </code>
               can be used for confirming a specific action. Make sure that you provide a correct URL, which
               <strong>
                Confirm
@@ -2246,27 +2304,29 @@
               <code>
                local/file_system?file_id=1234567&amp;action=delete
               </code>
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="16ac58ca-d4c2-4fc2-94c9-2b299f523aaf">
-             <pre id="1ddaeafb-d1ee-4e56-a42d-46674da0de25"><code class="python">from bootwrap import Dialog, Button
+            <div id="cec61924-8ba1-44d6-8b35-ccfade28b52c">
+             <pre id="7fa413a7-353a-4ca2-b123-f1fefe7a2c79"><code class="python">from bootwrap import Panel, Dialog, Button
 
 dialog = Dialog(
   "Delete File",
-  "Are you sure?",
-  Button("Confirm").as_danger().link("url/to/act")
+  "Are you sure that you want to delete this file?",
+  Button("Confirm").as_danger().dismiss(),
   Button("Cancel").dismiss()
 ).as_danger()
 
-button = Button("Delete").as_danger().toggle(dialog)</code></pre>
-             <div id="943ab20a-1676-43fe-a513-9299a16cbc26">
-              <div class="modal" id="73be06dd-3f65-44f5-a6a0-f739affac506">
+button = Button("Delete").as_danger().toggle(dialog)   
+
+Panel(dialog, button)</code></pre>
+             <div id="259aa8db-ee49-474b-92eb-8ab226e1a4ea">
+              <div class="modal" id="4cabf234-e1c8-4414-af28-15ae83a4bbd8">
                <div class="modal-dialog" role="document">
                 <div class="modal-content">
                  <div class="modal-header">
                   <h5 class="modal-title text-danger">
                    Delete File
                   </h5>
                   <button aria-label="Close" class="close" data-dismiss="modal" type="button">
@@ -2275,56 +2335,56 @@
                    </span>
                   </button>
                  </div>
                  <div class="modal-body">
                   Are you sure that you want to delete this file?
                  </div>
                  <div class="modal-footer">
-                  <button class="btn btn-danger" data-dismiss="modal" id="adaee889-4ac1-4cf7-85ea-8f8760a04b56" onclick="return false;" type="button">
+                  <button class="btn btn-danger" data-dismiss="modal" id="9dc9fc32-c3cc-43c8-9a07-1988e3212d7f" onclick="return false;" type="button">
                    Confirm
                   </button>
-                  <button class="btn" data-dismiss="modal" id="ec866784-5e94-4e84-88bf-8d4951fc0375" onclick="return false;" type="button">
+                  <button class="btn" data-dismiss="modal" id="947e73d4-a99e-493b-96c6-b1429b07077c" onclick="return false;" type="button">
                    Cancel
                   </button>
                  </div>
                 </div>
                </div>
               </div>
-              <button class="btn btn-danger" data-target="#73be06dd-3f65-44f5-a6a0-f739affac506" data-toggle="modal" id="65f7cff2-1a4f-45ba-a19e-f83bd2f8d854" onclick="return false;" type="button">
+              <button class="btn btn-danger" data-target="#4cabf234-e1c8-4414-af28-15ae83a4bbd8" data-toggle="modal" id="46870afa-908a-492a-be2a-ed5b9459e42c" onclick="return false;" type="button">
                Delete
               </button>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="fe4e79ff-990c-43da-92e7-1117f47ae138">
-        <div class="mt-3" id="a7177dab-6254-48ef-9e68-24903e87638f">
-         <div id="1b80d01a-742d-4842-8465-d14080984ff6">
+       <div class="tab-pane fade" id="1f1488a0-4796-4b67-a6df-b078a7c6272a">
+        <div class="mt-3" id="34c879d3-0412-466b-b5d4-792317918c94">
+         <div id="6b3c562e-ee3d-439a-9b05-442affdde1f8">
           <div class="row">
            <div class="col-md">
-            <div id="4e419d74-7487-4291-ae44-bef609681ba6">
-             <h1 id="b2afe1a7-90ad-4169-8a5f-fdfea869e744">
+            <div id="63ef150c-9cbb-4f54-95db-7480e490f849">
+             <h1 id="cf34ebe8-6c59-4e64-a28e-9b14f0f1655b">
               Complex Dialog
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="2860e013-eabc-4000-8c19-98eb1c66390a">
+            <div id="61616afd-8733-4013-a507-cc7d0edb1b72">
             </div>
            </div>
           </div>
          </div>
-         <div id="3858145a-f2d6-48e0-9a96-bd32451bfa44">
+         <div id="e3555b1d-b6ea-4869-b8bd-43fe3772ff58">
           <div class="row">
            <div class="col-md">
-            <div id="dd9fa418-d848-4005-a012-7f2e42449582">
-             <p id="97e25333-1e4b-4e9d-b499-a367d058926a">
+            <div id="658386f9-cabb-461d-acf2-b17057644565">
+             <p id="ee718e70-3e10-4c2d-8348-ca19823640fb">
               An example of how
               <code>
                Dialog
               </code>
               can be used for buying shares. It contains a web
               <code>
                Form
@@ -2345,169 +2405,169 @@
                Cancel
               </strong>
               , the dialog will be closed, discarding the buying action.
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="2c13ad3b-bdca-42df-97a7-614521302d4e">
-             <pre id="5bdeeab3-f8aa-4f63-bb0c-cede1705f1f5"><code class="python">from bootwrap import Form, NumericInput, Dialog, Button
+            <div id="e95d9da3-1d09-4207-ae93-a3fa9bc5a630">
+             <pre id="3b2bef09-2ee0-495b-93f1-6eae6ad97e43"><code class="python">from bootwrap import Panel, Form, NumericInput, Dialog, Button
 
 dialog = Dialog(
     "Buy Company Shares",
     Form(
         NumericInput(
             "Amount($)",
             "amount",
-            placeholder=\
-              "enter an amount for buying shares"
+            placeholder="enter an amount for buying shares"
         ),
         Button("Cancel").add_classes("float-right").dismiss(),
-        Button("Buy").add_classes("float-right).mr(2).as_success().
-          submit()
-    ).on_submit("url/to/act")
+        Button("Buy").add_classes("float-right").mr(2).as_success().
+          dismiss()
+    )
 )
+button = Button("Buy Shares").as_primary().toggle(dialog)   
 
-button = Button("Buy Shares").as_primary().toggle(dialog)</code></pre>
-             <div id="96a0e43d-7b81-46ed-bb25-0430905c14bd">
-              <div class="modal" id="6624bc57-99b6-4c59-837a-08dc68893a36">
+Panel(dialog, button)</code></pre>
+             <div id="1a15e419-e8ea-41f4-912b-06ac9b194d1d">
+              <div class="modal" id="82ed9ea4-ff66-41a6-88d4-2094ac231c05">
                <div class="modal-dialog" role="document">
                 <div class="modal-content">
                  <div class="modal-header">
                   <h5 class="modal-title text-None">
                    Buy Company Shares
                   </h5>
                   <button aria-label="Close" class="close" data-dismiss="modal" type="button">
                    <span aria-hidden="true">
                     ×
                    </span>
                   </button>
                  </div>
                  <div class="modal-body">
-                  <form enctype="multipart/form-data" id="0c5fa134-56f7-4b22-b493-b5670e9a7e88" method="POST">
+                  <form enctype="multipart/form-data" id="0a85f58f-cb4a-4faa-b683-47ab6e53fdbb" method="POST">
                    <div class="form-group row">
-                    <label class="col-sm-2 col-form-label d-flex align-items-center" for="966b8777-adde-483a-9795-523536b6f0d8">
+                    <label class="col-sm-4 col-form-label d-flex align-items-center" for="f8d39d8c-ab49-4bf7-801f-c3069138229d">
                      Amount($)
                     </label>
-                    <div class="col-sm-10 d-flex align-items-center">
-                     <input class="form-control" id="966b8777-adde-483a-9795-523536b6f0d8" name="amount" placeholder="enter an amount for buying shares" type="number"/>
+                    <div class="col-sm-8 d-flex align-items-center">
+                     <input class="form-control" id="f8d39d8c-ab49-4bf7-801f-c3069138229d" name="amount" placeholder="enter an amount for buying shares" type="number"/>
                     </div>
                    </div>
-                   <button class="float-right btn" data-dismiss="modal" id="81aa6ca8-384c-406e-ae0d-9e8274c7259c" onclick="return false;" type="button">
+                   <button class="float-right btn" data-dismiss="modal" id="bb54254e-1793-41df-8140-3bd4b7c293be" onclick="return false;" type="button">
                     Cancel
                    </button>
-                   <button class="float-right mr-2 btn btn-success" data-dismiss="modal" id="3517eaa8-768e-492f-9ab6-30f190bc5d9a" onclick="return false;" type="button">
+                   <button class="float-right mr-2 btn btn-success" data-dismiss="modal" id="a6a8a355-b708-4de5-a7b6-20d1573a0272" onclick="return false;" type="button">
                     Buy
                    </button>
                   </form>
                  </div>
                 </div>
                </div>
               </div>
-              <button class="btn btn-primary" data-target="#6624bc57-99b6-4c59-837a-08dc68893a36" data-toggle="modal" id="93dd55ef-5189-44f6-bcff-899bc4715691" onclick="return false;" type="button">
+              <button class="btn btn-primary" data-target="#82ed9ea4-ff66-41a6-88d4-2094ac231c05" data-toggle="modal" id="40493fd2-9070-4105-b1f3-f912c4b0be0f" onclick="return false;" type="button">
                Buy Shares
               </button>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="f4a2e903-d7f8-4a64-93b9-85647e31031f">
-     <div id="184b9296-68c2-4ac6-a0b7-d141bf2acae5">
+    <div class="tab-pane fade" id="4809de16-7c3c-4c28-9093-69b35698e4ce">
+     <div id="a907193a-ae82-42af-bf08-3908d938a8b4">
       <hr/>
-      <ul class="nav" id="200d343e-627e-4528-9144-26bd4d83d502" role="tablist">
+      <ul class="nav" id="158c7f34-22ee-47f8-bdcb-10183713db04" role="tablist">
        <li class="nav-item">
-        <a class="nav-link active" data-target="#735fd4a4-eeda-41ad-a6ec-9cafce031e52" data-toggle="tab" href="#735fd4a4-eeda-41ad-a6ec-9cafce031e52" id="58a143b2-58c1-4e96-8527-7e1d6af7eefc" role="tab">
-         <span class="text-secondary" id="73c6d7b1-ed1d-4a7f-9955-b24077774e8b">
+        <a class="nav-link active" data-target="#6cb02366-a5af-475b-aabc-5775d98b4001" data-toggle="tab" href="#6cb02366-a5af-475b-aabc-5775d98b4001" id="ae298491-5c4e-439a-a43d-a6e8654116a1" role="tab">
+         <span class="text-secondary" id="376e5912-e914-4414-b8c8-ade838963017">
           Form
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#bc56bf67-6a65-42e1-8d77-ba133b724de6" data-toggle="tab" href="#bc56bf67-6a65-42e1-8d77-ba133b724de6" id="ab71edf4-7a5d-4a85-83dd-05c995d816a1" role="tab">
-         <span class="text-secondary" id="eec5214b-613a-46a0-8adf-d3255312f5a2">
+        <a class="nav-link" data-target="#ddf85724-9125-4252-b0f0-7cf37ce2c9d3" data-toggle="tab" href="#ddf85724-9125-4252-b0f0-7cf37ce2c9d3" id="68f04c0d-9e63-49d2-b272-e317c57b8767" role="tab">
+         <span class="text-secondary" id="c7ad846f-1724-4535-9961-ca639f3843d9">
           CheckboxInput
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#aaa2ca34-5859-4e67-ab61-a3354e49814c" data-toggle="tab" href="#aaa2ca34-5859-4e67-ab61-a3354e49814c" id="d81b172a-9453-45be-baa2-b6d758f20ac5" role="tab">
-         <span class="text-secondary" id="cb5ff79f-4612-4869-ad33-afb00baaa51f">
+        <a class="nav-link" data-target="#ef426526-dc25-4a29-b5b9-bc59e79d883b" data-toggle="tab" href="#ef426526-dc25-4a29-b5b9-bc59e79d883b" id="0de88761-6697-46ab-a932-6f177212d347" role="tab">
+         <span class="text-secondary" id="c5f46dec-272f-4d34-8bed-55a1eccce31b">
           TextInput
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#6a70564d-76b9-4f89-a2f6-20b801b6573b" data-toggle="tab" href="#6a70564d-76b9-4f89-a2f6-20b801b6573b" id="e6a3d4aa-7eac-44f6-8492-aaad509242b3" role="tab">
-         <span class="text-secondary" id="7ad3cc13-a378-4885-b7ef-dbe952a74e8a">
+        <a class="nav-link" data-target="#c0c5bab6-43ae-45b4-a0d9-e2e703e4aee5" data-toggle="tab" href="#c0c5bab6-43ae-45b4-a0d9-e2e703e4aee5" id="7a8d29ae-1ae0-4339-aeef-67b4be8d7f75" role="tab">
+         <span class="text-secondary" id="99f09b46-ce8e-4aeb-a8a6-15cd61d59aaa">
           NumericInput
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#e2790200-471a-46f6-a282-53f9a693e531" data-toggle="tab" href="#e2790200-471a-46f6-a282-53f9a693e531" id="00ab3152-f7b8-415a-9672-e1c43f33acc3" role="tab">
-         <span class="text-secondary" id="a2d23219-4fa2-434a-b972-543cbf6dad30">
+        <a class="nav-link" data-target="#fb4c3830-15e3-4f92-8f80-f7f24ce90fb5" data-toggle="tab" href="#fb4c3830-15e3-4f92-8f80-f7f24ce90fb5" id="d51d2cdd-53b4-41fb-8402-3d49367f8d66" role="tab">
+         <span class="text-secondary" id="efa3ff7a-0ba1-4b49-b9ea-1017a787dbbd">
           SelectInput
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#26fccd40-b42a-476f-9fe9-55c162893a03" data-toggle="tab" href="#26fccd40-b42a-476f-9fe9-55c162893a03" id="85ce15f8-77f1-4651-94bc-8a9f6e7ae58f" role="tab">
-         <span class="text-secondary" id="9aba99d8-da48-42c3-b978-f4286d3666f2">
+        <a class="nav-link" data-target="#92519a90-1163-4949-b82a-dec5f4658ec9" data-toggle="tab" href="#92519a90-1163-4949-b82a-dec5f4658ec9" id="650e7747-40d7-4684-83e4-eca9383a689e" role="tab">
+         <span class="text-secondary" id="72760876-c259-46a6-84df-5c03baa12c49">
           SelectInput.Option
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#c4bb12d8-b3c2-425b-b6a2-a69c7ca8604c" data-toggle="tab" href="#c4bb12d8-b3c2-425b-b6a2-a69c7ca8604c" id="c61d7b93-a231-4c43-a919-366e11705c91" role="tab">
-         <span class="text-secondary" id="f7e81f1e-8743-4ed9-aabb-b12cb03bd738">
+        <a class="nav-link" data-target="#2d325dac-243f-43fd-9b89-f4034d175837" data-toggle="tab" href="#2d325dac-243f-43fd-9b89-f4034d175837" id="8eb149ca-4ba1-45b6-9972-abf095eb1b82" role="tab">
+         <span class="text-secondary" id="4e2fe791-933d-4d39-967b-60a46a6f33ea">
           HiddenInput
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#223e9820-15a1-4fb4-8942-f7b4fea2009c" data-toggle="tab" href="#223e9820-15a1-4fb4-8942-f7b4fea2009c" id="f3aaf581-46b3-4151-b095-8e3fb9221ba9" role="tab">
-         <span class="text-secondary" id="97e2a68a-f079-47a9-bf4a-4c9d52801f51">
+        <a class="nav-link" data-target="#f8c73225-c95f-4444-a9e8-540c16a26bac" data-toggle="tab" href="#f8c73225-c95f-4444-a9e8-540c16a26bac" id="f3ac190c-7c56-4f21-ac57-ae49686a1075" role="tab">
+         <span class="text-secondary" id="168dd775-97f1-494b-a00a-233b0bc4c90e">
           FileInput
          </span>
         </a>
        </li>
       </ul>
       <div class="tab-content">
-       <div class="tab-pane fade active show" id="735fd4a4-eeda-41ad-a6ec-9cafce031e52">
-        <div class="mt-5" id="3d640fa7-b6ce-4dba-a42f-34768c9d8586">
-         <div class="d-flex justify-content-between" id="d2257da3-1138-4717-9071-cb7504cad58d">
-          <h1 id="7f06ac06-2187-4906-91d0-bb08e32aefb2">
+       <div class="tab-pane fade active show" id="6cb02366-a5af-475b-aabc-5775d98b4001">
+        <div class="mt-5" id="5159e305-7ca3-4e47-a36c-df8eff271104">
+         <div class="d-flex justify-content-between" id="b830ad36-4944-42d9-b4ce-3f6393fb8c67">
+          <h1 id="3179cc19-e9ae-4f1c-ac53-16fd94d91457">
            Class
-           <span class="text-primary" id="ff679d4c-4dfb-4337-a620-63afeb5998e1">
+           <span class="text-primary" id="1a1f3c68-a129-4ed3-b773-1767745d14fc">
             Form
            </span>
           </h1>
-          <div id="c3d5a18c-59c5-41e7-9787-e32c3fcd668b">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#c93f3378-90a0-4320-a819-23c05d47b37c" data-toggle="collapse" id="d41ac3be-0c66-4fd8-90a0-b856f90938e4" onclick="return false;" type="button">
+          <div id="35a5f9aa-19de-48d0-8127-e86a393e25f5">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#f9a8647b-ee4f-4e29-908d-87d8445ee12c" data-toggle="collapse" id="f7fb56e8-36c8-4130-9721-dd782e68ede6" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="4f2cb9f1-8c22-45f5-898a-d9f0e1edf3f9">
+         <span class="text-muted" id="972e6bc7-2e48-4204-aed9-658bdef73c5f">
           A web component for a form.
          </span>
-         <pre id="815fd8b4-6d35-4cfa-92ac-be4984e169a0"><code class="python">Form(*components)</code></pre>
-         <div class="ml-3 collapse" id="c93f3378-90a0-4320-a819-23c05d47b37c">
-          <h6 id="89c35a1a-a545-47c2-a4e1-ba2095035624">
+         <pre id="83f3da2d-0dcf-45b1-81c8-2ca14754f76f"><code class="python">Form(*components)</code></pre>
+         <div class="ml-3 collapse" id="f9a8647b-ee4f-4e29-908d-87d8445ee12c">
+          <h6 id="ec927ebc-fb68-4bcf-bb44-a54138f157e2">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="a5064704-e84f-4d93-a76b-76878b9bf44d">
+          <table class="table table-sm bg-light" id="c2b7386b-5eba-470b-b826-fcbf743158fc">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -2537,64 +2597,65 @@
               representing form
             elements for input and action.
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <p id="2a00b816-d76b-4fd4-ba39-30f39b3580ea">
+         <p id="5dc5a3cd-144e-41a5-8e8a-65f811a47470">
           Use the
           <code>
            on_submit(href)
           </code>
           function to specify URL where entered
     information should to be sent for processing.
          </p>
-         <div class="ml-3" id="bf68dd87-5906-42ef-9015-abb8b71d9bbd">
-          <h6 id="b38d0c43-aeef-4916-ab9a-be243bee04b8">
+         <div class="ml-3" id="cd0a58aa-18e7-4825-8ade-b329212c384c">
+          <h6 id="fbf9ed9f-3a52-4de1-acae-f0942384d588">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="8f125af4-c04e-4b29-9119-8c498e926301"><code class="python">from bootwrap import Form
+          <pre id="185d0d8c-33ef-4b1f-b0b2-effcceb74866"><code class="python">from bootwrap import Form
 
 Form(
     # here should be an enumeration  of
     # input components and actions
     ...
-).on_submit('go/to/this/url')</code></pre>
+).on_submit('go/to/this/url')
+</code></pre>
          </div>
-         <div class="mt-5" id="2c5cf956-88c9-4ff9-8159-03e7d70aefc5">
-          <div class="d-flex justify-content-between" id="bbaecada-b6a4-4627-a0e0-a281189dffd8">
-           <h4 id="b453cff7-ecbf-4efb-b491-1d41af17f2d9">
+         <div class="mt-5" id="c3bf2bdd-1f9d-4557-ad18-90457dc0369e">
+          <div class="d-flex justify-content-between" id="84bd1798-c89d-4a6e-895a-f1346884d759">
+           <h4 id="9c385713-c11a-40aa-bd37-7978262e5511">
             Method
-            <span class="text-primary" id="37f25306-a45e-46f3-a1ad-ea694df8bd69">
+            <span class="text-primary" id="dfffc558-ad46-4f7e-8042-098b5c347a72">
              on_submit
             </span>
            </h4>
-           <div id="a72c78f9-ad2b-40a5-83f4-c03c3561346f">
-            <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#0ff7b38c-467f-4401-9be9-4e68839ddba8" data-toggle="collapse" id="492f9891-db0b-48fc-b6e3-0e0479ac135a" onclick="return false;" type="button">
+           <div id="41b162da-8a63-4e59-813c-c2dd20f30573">
+            <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#e74abda1-e926-4b0e-97dd-2327d4b50c41" data-toggle="collapse" id="e006f7ec-45fc-479f-9c3a-f6caeb26cf6d" onclick="return false;" type="button">
              Argument
             </button>
-            <button class="btn-sm btn btn-outline-primary" data-target="#1d41a61a-3c3b-4351-973c-a5432e618c35" data-toggle="collapse" id="3232e488-9003-49bc-8ac3-b6c3426396ff" onclick="return false;" type="button">
+            <button class="btn-sm btn btn-outline-primary" data-target="#e9386834-72bd-460d-ade5-e9cfb0ee9e74" data-toggle="collapse" id="e75733d2-5cf0-467b-b971-5c4b6dd49803" onclick="return false;" type="button">
              Returns
             </button>
            </div>
           </div>
-          <span class="text-muted" id="a9fdf497-a559-4680-9815-653a83fb8fef">
+          <span class="text-muted" id="03d736c6-0e9e-4616-bcc2-7407b8e5a252">
            Sets the submit URL, for the POST request.
           </span>
-          <pre id="c1d41f66-1fb1-43c8-8a27-f3bf71cf4e28"><code class="python">on_submit(href)</code></pre>
-          <div class="ml-3 collapse" id="0ff7b38c-467f-4401-9be9-4e68839ddba8">
-           <h6 id="9bd19ebb-8749-464a-a88e-f9eb63ca8b91">
+          <pre id="2ed1a8a3-78ef-4c36-a6c0-857d0f7a4ab0"><code class="python">on_submit(href)</code></pre>
+          <div class="ml-3 collapse" id="e74abda1-e926-4b0e-97dd-2327d4b50c41">
+           <h6 id="43d33f04-511d-4f52-a299-06267e7be930">
             <strong>
              Arguments
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="0d944b01-33a9-4239-962b-c3071c33a0e8">
+           <table class="table table-sm bg-light" id="1e0fb7f5-9873-46fc-bce5-89a7aaae3d3d">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -2619,21 +2680,21 @@
               <td>
                The URL for submitting the form.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3 collapse" id="1d41a61a-3c3b-4351-973c-a5432e618c35">
-           <h6 id="3cc72dc4-be76-4eef-b418-ac9d3e13af42">
+          <div class="ml-3 collapse" id="e9386834-72bd-460d-ade5-e9cfb0ee9e74">
+           <h6 id="d28f79a1-4107-46ca-acd9-52dbf50fab89">
             <strong>
              Returns
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="20772702-056e-4caf-b944-e1b567eadad6">
+           <table class="table table-sm bg-light" id="c132a7b3-1f78-490e-9ff9-140ea7166332">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -2658,53 +2719,54 @@
               <td>
                The instance of this class.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3" id="77daff30-a865-447c-b562-15a4f015d304">
-           <h6 id="953ab04c-2bff-4c2d-b59e-a459a8a81984">
+          <div class="ml-3" id="311e0406-b0cc-4acc-b2ce-8e3e1924f2b0">
+           <h6 id="8cf405b0-f1eb-467e-b4f9-5a778a11af16">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="c42ccc10-38f8-427b-a185-ca8a1a5ab6b5"><code class="python">from bootwrap import Form
+           <pre id="14732345-4b7d-47be-be2f-2ccdefc4e104"><code class="python">from bootwrap import Form
 
-Form(...).on_submit('go/to/this/url')</code></pre>
+Form(...).on_submit('go/to/this/url')
+</code></pre>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="bc56bf67-6a65-42e1-8d77-ba133b724de6">
-        <div class="mt-5" id="3c6bd178-1d41-49ff-bf6b-31f09b9715f2">
-         <div class="d-flex justify-content-between" id="e4692d61-e7f6-40a2-9e52-de2c2cea567c">
-          <h1 id="0bf215cd-fb69-4e4f-baf5-1e828d234301">
+       <div class="tab-pane fade" id="ddf85724-9125-4252-b0f0-7cf37ce2c9d3">
+        <div class="mt-5" id="0fa0fdaf-2008-49c3-aa8b-f7000ef90fa7">
+         <div class="d-flex justify-content-between" id="6ef24d2e-a7d6-4f13-b2e6-db46ccd1d508">
+          <h1 id="078261e5-8e4c-42a8-8f03-d670ddb5af93">
            Class
-           <span class="text-primary" id="e2ddb84b-3912-470e-a5be-76521e79e58d">
+           <span class="text-primary" id="f1e17489-02a8-4817-926d-2377e9dde974">
             CheckboxInput
            </span>
           </h1>
-          <div id="c21f5e05-303d-4d45-8c31-9bd56a09f6b1">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#f0f61b7c-2c47-4dc0-ba6b-d51e1aefeb9a" data-toggle="collapse" id="6a0f2eaf-0c43-447a-b656-283b34597aa5" onclick="return false;" type="button">
+          <div id="636115ba-e980-42b9-8888-83c670248036">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#29094728-1fea-411c-a98a-d7f7a260cda5" data-toggle="collapse" id="38792f1c-ac93-48ec-a5a5-1e44f3fd4afc" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="eca719ab-77e7-4a66-9e6e-e74ae70f9fe2">
+         <span class="text-muted" id="3088b3cb-b2cd-49c2-baad-e49a4f090201">
           A checkbox input.
          </span>
-         <pre id="3f854140-d91d-4807-8cb2-574960a4d4a3"><code class="python">CheckboxInput(label, name, checked=False)</code></pre>
-         <div class="ml-3 collapse" id="f0f61b7c-2c47-4dc0-ba6b-d51e1aefeb9a">
-          <h6 id="04846326-d98d-4d20-a53f-f87e8d5808c3">
+         <pre id="84ca87db-c787-4c82-af71-f7933f9ff550"><code class="python">CheckboxInput(label, name, checked=False)</code></pre>
+         <div class="ml-3 collapse" id="29094728-1fea-411c-a98a-d7f7a260cda5">
+          <h6 id="11d171aa-5a4a-4394-8c25-af8499641972">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="e4f4d094-ea3a-459e-b61f-b6aee0aab7f3">
+          <table class="table table-sm bg-light" id="ad2750e8-6bf1-4c31-9e8e-a1ec61116ed0">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -2759,96 +2821,97 @@
              <td>
               The check box status.
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <p id="517e1328-cec1-47f1-ba4e-c5acb8ff00c7">
+         <p id="111eacfb-0121-41fd-861a-94652bfa2335">
           Use the
           <code>
            as_disabled()
           </code>
           function to prevent the user from changing
     status of the
           <code>
            CheckboxInput
           </code>
           component.
          </p>
-         <div class="ml-3" id="3a470b6c-7d6b-4e96-bcd7-c1b9abe73c8f">
-          <h6 id="8ad3a347-3a79-43f1-8513-133a22bc1817">
+         <div class="ml-3" id="dc381413-6a46-45af-9d9b-dd1afa660d46">
+          <h6 id="5352f5c3-fa96-405d-836d-dcd316b1630e">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="09240dd9-7d98-4fd1-b4ef-2830e927f7e2"><code class="python">from bootwrap import Form, CheckboxInput
+          <pre id="e7941fbb-8d91-42ad-93b0-b2e9252715e2"><code class="python">from bootwrap import Form, CheckboxInput
 
 Form(
     CheckboxInput('One', 'opt1'),
     CheckboxInput('Two', 'opt2', True),
     CheckboxInput('Three', 'opt3').as_disabled()
-)</code></pre>
+)
+</code></pre>
          </div>
-         <div class="ml-3" id="d03f5ab5-a57a-4df7-91e2-6aa50d3a60c2">
-          <form enctype="multipart/form-data" id="6484874a-ac37-48e8-b7f6-4a12676d27bf" method="POST">
+         <div class="ml-3" id="22ee5c06-12f8-41dc-83c0-e497d495ab5f">
+          <form enctype="multipart/form-data" id="70a922a3-cb93-4984-a611-10982a6f8a0f" method="POST">
            <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center" for="5cd786e8-c7ba-419f-86ec-4bb225e53fa0">
+            <label class="col-sm-4 col-form-label d-flex align-items-center" for="16af9274-a335-4aeb-bdf1-c0785e3049d4">
              One
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
-             <input autocomplete="off" class="form-check-input" id="5cd786e8-c7ba-419f-86ec-4bb225e53fa0" name="opt1" type="checkbox"/>
+            <div class="col-sm-8 d-flex align-items-center">
+             <input autocomplete="off" class="form-check-input" id="16af9274-a335-4aeb-bdf1-c0785e3049d4" name="opt1" type="checkbox"/>
             </div>
            </div>
            <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center" for="fbab006c-dcdc-43a9-9245-78d9213fa249">
+            <label class="col-sm-4 col-form-label d-flex align-items-center" for="cc6e05b4-11f9-4604-a3e8-489c55276242">
              Two
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
-             <input autocomplete="off" checked="" class="form-check-input" id="fbab006c-dcdc-43a9-9245-78d9213fa249" name="opt2" type="checkbox"/>
+            <div class="col-sm-8 d-flex align-items-center">
+             <input autocomplete="off" checked="" class="form-check-input" id="cc6e05b4-11f9-4604-a3e8-489c55276242" name="opt2" type="checkbox"/>
             </div>
            </div>
            <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center" for="6cf70546-ba44-4a24-8502-04b61336c1af">
+            <label class="col-sm-4 col-form-label d-flex align-items-center" for="f0025600-34e6-449e-9b88-9ef93df28268">
              Three
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
-             <input autocomplete="off" class="form-check-input" disabled="" id="6cf70546-ba44-4a24-8502-04b61336c1af" name="opt3" type="checkbox"/>
+            <div class="col-sm-8 d-flex align-items-center">
+             <input autocomplete="off" class="form-check-input" disabled="" id="f0025600-34e6-449e-9b88-9ef93df28268" name="opt3" type="checkbox"/>
             </div>
            </div>
           </form>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="aaa2ca34-5859-4e67-ab61-a3354e49814c">
-        <div class="mt-5" id="fb8550c8-655b-4a59-b7f0-7e43d4a3bfa4">
-         <div class="d-flex justify-content-between" id="082a2d41-078d-49f5-a93c-bfacd6eef7dd">
-          <h1 id="c593db99-68da-4e1f-b740-214b5ebebe7c">
+       <div class="tab-pane fade" id="ef426526-dc25-4a29-b5b9-bc59e79d883b">
+        <div class="mt-5" id="9e9d6371-1729-423e-82f4-703a47c4af15">
+         <div class="d-flex justify-content-between" id="e36f027e-b9d8-44a2-95e7-9ebc1168d528">
+          <h1 id="e823553e-d6cd-4eda-a407-84f857ff0e17">
            Class
-           <span class="text-primary" id="d0cd221a-aeff-42c3-a08b-698837fbdb2b">
+           <span class="text-primary" id="b4548232-ada8-420c-aa6d-2096917c0e6a">
             TextInput
            </span>
           </h1>
-          <div id="567c8a09-1207-4706-8d46-65e128b63f34">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#7cde5b98-5680-4f33-9dd7-09ee49f80b3b" data-toggle="collapse" id="a5743406-2762-454b-aafc-a7baa5cea6e1" onclick="return false;" type="button">
+          <div id="6877f702-392c-41c3-b3d3-dd733b02f373">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#57468a64-816b-4057-a215-8eb7aebf9a79" data-toggle="collapse" id="fc0268c5-858a-4c35-acb5-bd480bdbe6b5" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="a1e7c8c0-fd45-4ae8-bcee-05761a192500">
+         <span class="text-muted" id="d28ef899-e4cb-4a5c-947f-a61986515f97">
           A text input.
          </span>
-         <pre id="8a2b98d8-f7b2-4457-bc62-68cb421d5677"><code class="python">TextInput(label, name, value=None, placeholder=None)</code></pre>
-         <div class="ml-3 collapse" id="7cde5b98-5680-4f33-9dd7-09ee49f80b3b">
-          <h6 id="e9b62631-59ac-4ebf-87b1-f89a4dd9bb8f">
+         <pre id="ba4edb5b-5601-4bc2-a51a-0978b1d7e386"><code class="python">TextInput(label, name, value=None, placeholder=None)</code></pre>
+         <div class="ml-3 collapse" id="57468a64-816b-4057-a215-8eb7aebf9a79">
+          <h6 id="4a767bfb-4e1b-46fc-9e27-2b48719bde0f">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="33f08f38-2dec-4520-89d5-db4ced158ebe">
+          <table class="table table-sm bg-light" id="9674d2fc-88a6-4a82-b8a0-a18b724c9d02">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -2918,102 +2981,103 @@
              <td>
               The input placeholder.
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <p id="5ec459f8-6117-4d15-aeb3-8ff2de57f1e4">
+         <p id="17c855cf-e163-4f29-a86f-3f791d9e8bbd">
           Use the
           <code>
            as_disabled()
           </code>
           function to prevent the user from entering data
     to the
           <code>
            TextInput
           </code>
           component.
          </p>
-         <div class="ml-3" id="9c53187c-5838-47a4-99db-9cfe8f9d7639">
-          <h6 id="783af542-d400-4053-9c86-3ac6cf6607c9">
+         <div class="ml-3" id="21a4464f-6c97-4802-84bd-ee400b315a0c">
+          <h6 id="e1c1c705-52f2-4423-ae09-632d552ccba4">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="46ab94d2-f316-4e9c-b09a-0d2f862aac69"><code class="python">from bootwrap import Form, TextInput
+          <pre id="e59de20f-593e-4a89-8b11-733011fc7b5a"><code class="python">from bootwrap import Form, TextInput
 
 Form(
     TextInput('Text1', 'text'),
     TextInput('Text2', 'text', placeholder='type here'),
     TextInput('Text3', 'text', 'Hello World!'),
     TextInput('Text4', 'text').as_disabled()
-)</code></pre>
+)
+</code></pre>
          </div>
-         <div class="ml-3" id="0fb9bf0a-9619-433b-ba0f-93916957fb8e">
-          <form enctype="multipart/form-data" id="0d95a493-24aa-4cb9-8296-ee4818d38dd8" method="POST">
+         <div class="ml-3" id="6bab5f67-7440-4a0a-9cf2-79a34b2f96b9">
+          <form enctype="multipart/form-data" id="49219ec1-a320-4ce3-b5f6-0a79411596aa" method="POST">
            <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center" for="fc9b8a5d-8560-44ba-ae84-eb8ad65f7ccb">
+            <label class="col-sm-4 col-form-label d-flex align-items-center" for="d98c8891-a862-47e1-bb97-e9f3167fef9c">
              Text1
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
-             <input class="form-control" id="fc9b8a5d-8560-44ba-ae84-eb8ad65f7ccb" name="text" type="text"/>
+            <div class="col-sm-8 d-flex align-items-center">
+             <input class="form-control" id="d98c8891-a862-47e1-bb97-e9f3167fef9c" name="text" type="text"/>
             </div>
            </div>
            <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center" for="032edbb9-18cf-4448-972d-99bf8eec9983">
+            <label class="col-sm-4 col-form-label d-flex align-items-center" for="88b01d57-6095-4dc2-899d-2a14fd34b2d7">
              Text2
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
-             <input class="form-control" id="032edbb9-18cf-4448-972d-99bf8eec9983" name="text" placeholder="type here" type="text"/>
+            <div class="col-sm-8 d-flex align-items-center">
+             <input class="form-control" id="88b01d57-6095-4dc2-899d-2a14fd34b2d7" name="text" placeholder="type here" type="text"/>
             </div>
            </div>
            <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center" for="c197f5ef-ee53-41d0-ab04-a94238a095fe">
+            <label class="col-sm-4 col-form-label d-flex align-items-center" for="1b6d7cc7-607e-4abd-8f08-913be0bca645">
              Text3
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
-             <input class="form-control" id="c197f5ef-ee53-41d0-ab04-a94238a095fe" name="text" type="text" value="Hello World!"/>
+            <div class="col-sm-8 d-flex align-items-center">
+             <input class="form-control" id="1b6d7cc7-607e-4abd-8f08-913be0bca645" name="text" type="text" value="Hello World!"/>
             </div>
            </div>
            <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center" for="c11970cd-16bc-40da-97f5-09862a814a5f">
+            <label class="col-sm-4 col-form-label d-flex align-items-center" for="fe5a68ad-2d45-49f3-81b9-fbb70704005e">
              Text4
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
-             <input class="form-control" disabled="" id="c11970cd-16bc-40da-97f5-09862a814a5f" name="text" type="text"/>
+            <div class="col-sm-8 d-flex align-items-center">
+             <input class="form-control" disabled="" id="fe5a68ad-2d45-49f3-81b9-fbb70704005e" name="text" type="text"/>
             </div>
            </div>
           </form>
          </div>
-         <div class="mt-5" id="8e0a5ada-f2aa-4a0e-8c11-bae748cc4516">
-          <div class="d-flex justify-content-between" id="410a268d-8f03-4d67-b565-8910ba538cc4">
-           <h4 id="1b7476b4-8e00-4e35-abc2-61e962c5c10f">
+         <div class="mt-5" id="304fe442-8af9-4ff2-b0a4-c80a3eef7ca4">
+          <div class="d-flex justify-content-between" id="5fc836e6-d035-474b-813b-1b58d5a3644b">
+           <h4 id="8462b3a1-2d5b-43d9-a131-53c20f96bf8e">
             Method
-            <span class="text-primary" id="25fe5e1b-c778-4475-96cf-b088afa16af2">
+            <span class="text-primary" id="b5159411-1c76-4190-a6b4-f3c97b03df05">
              for_email
             </span>
            </h4>
-           <div id="f2686372-68d9-461a-870f-2cb99dc37612">
-            <button class="btn-sm btn btn-outline-primary" data-target="#a72ed475-6e49-47dd-85c4-1b08864c7a26" data-toggle="collapse" id="aaa31eec-f1cd-419a-a6f3-f19bd9fc26c3" onclick="return false;" type="button">
+           <div id="67f9598c-4ca0-46fd-b896-5a917a98a31d">
+            <button class="btn-sm btn btn-outline-primary" data-target="#2d0a92c6-9f6d-4b75-b5fe-c4cfaf3e799a" data-toggle="collapse" id="e922d8ec-3b46-4506-b9a4-67c7a74f00d5" onclick="return false;" type="button">
              Returns
             </button>
            </div>
           </div>
-          <span class="text-muted" id="76389304-97a3-41f2-a0d3-21cda17d4ed3">
+          <span class="text-muted" id="a8583529-7805-460e-8675-bd4ee1bfe761">
            Configuring input for entering email.
           </span>
-          <pre id="b37d8f9c-bd7c-4483-bd60-aa4153847fb2"><code class="python">for_email()</code></pre>
-          <div class="ml-3 collapse" id="a72ed475-6e49-47dd-85c4-1b08864c7a26">
-           <h6 id="fbfdf442-08b5-4487-9cfd-3eaf5acd2959">
+          <pre id="1b4a9eed-7851-4ea9-b3dc-fc568e869ada"><code class="python">for_email()</code></pre>
+          <div class="ml-3 collapse" id="2d0a92c6-9f6d-4b75-b5fe-c4cfaf3e799a">
+           <h6 id="82dd909b-6ff5-4847-a523-235c14186eee">
             <strong>
              Returns
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="8d28bb38-eb83-4154-b402-0612cc061865">
+           <table class="table table-sm bg-light" id="74aa46ef-ab88-41be-b1a8-2a762299d109">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -3038,64 +3102,65 @@
               <td>
                The instance of this class.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3" id="2dd72d3a-fc84-49ed-ba37-c52f6df86dab">
-           <h6 id="83a3d6aa-063f-4449-a3cb-40500c2e36d0">
+          <div class="ml-3" id="f30dd574-28de-41a6-9442-a85c027fdaf2">
+           <h6 id="bb0e573b-72b7-4d04-8a77-7e048e663b73">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="d336ba88-87ea-4133-8afb-a47fd87f1f88"><code class="python">from bootwrap import Form, TextInput
+           <pre id="ac3bf777-816c-4a64-882e-7b3bdb6dae48"><code class="python">from bootwrap import Form, TextInput
 
 Form(
     TextInput('Email', 'email', 'my@email.com').for_email()
-)</code></pre>
+)
+</code></pre>
           </div>
-          <div class="ml-3" id="e5704d95-70f8-491f-a642-798aa01caf96">
-           <form enctype="multipart/form-data" id="a5734409-faf8-4ded-b555-c129a09567eb" method="POST">
+          <div class="ml-3" id="4471dd79-9d44-4666-b657-24df0c9f80a2">
+           <form enctype="multipart/form-data" id="21fd4608-7fe1-4b91-8de9-2cf6d8b2df5b" method="POST">
             <div class="form-group row">
-             <label class="col-sm-2 col-form-label d-flex align-items-center" for="13081863-b2a7-407c-94df-e700656a4f5f">
+             <label class="col-sm-4 col-form-label d-flex align-items-center" for="86b71115-6d95-4999-9591-205fd28eb6e4">
               Email
              </label>
-             <div class="col-sm-10 d-flex align-items-center">
-              <input class="form-control" id="13081863-b2a7-407c-94df-e700656a4f5f" name="email" type="email" value="my@email.com"/>
+             <div class="col-sm-8 d-flex align-items-center">
+              <input class="form-control" id="86b71115-6d95-4999-9591-205fd28eb6e4" name="email" type="email" value="my@email.com"/>
              </div>
             </div>
            </form>
           </div>
          </div>
-         <div class="mt-5" id="69b39366-34a6-49d1-9447-949be5552ae7">
-          <div class="d-flex justify-content-between" id="54dff4c7-8f14-406b-aae1-4578db66adaa">
-           <h4 id="310fd0f7-5562-4f19-8aa1-233e0249ebce">
+         <div class="mt-5" id="4c4f37bd-76dc-44e2-a815-1c6c432bc86c">
+          <div class="d-flex justify-content-between" id="9ba01204-07f9-4880-850c-3f3bd9d2d977">
+           <h4 id="c17c8548-0a7c-4488-85ab-4b7a2b7c5c6e">
             Method
-            <span class="text-primary" id="6d01a8ff-cd02-46ed-a6ef-c45323c72567">
+            <span class="text-primary" id="968ceacb-2d47-4c95-9ab4-ae33051780c4">
              for_password
             </span>
            </h4>
-           <div id="2a062bc8-e257-4b16-8805-500caef705b9">
-            <button class="btn-sm btn btn-outline-primary" data-target="#6e3b4ad3-b1c4-4e13-99b3-a4e4a8442699" data-toggle="collapse" id="fa19bc51-1f40-44df-9774-0daee533f85e" onclick="return false;" type="button">
+           <div id="261ce58f-3406-4f9a-b004-dd4ae056b604">
+            <button class="btn-sm btn btn-outline-primary" data-target="#21645b98-4d78-405b-b7c5-5e0a6d920e6b" data-toggle="collapse" id="ad84f99b-5b71-4305-9de4-b376648f77ae" onclick="return false;" type="button">
              Returns
             </button>
            </div>
           </div>
-          <span class="text-muted" id="7988aa37-b936-4241-a738-360d2eb3e680">
+          <span class="text-muted" id="94ed9bfa-9428-4fb0-8310-2f6c611ff976">
            Configuring input for entering password.
           </span>
-          <pre id="8d2b3d62-ec93-47da-82ea-6beec8e5de39"><code class="python">for_password()</code></pre>
-          <div class="ml-3 collapse" id="6e3b4ad3-b1c4-4e13-99b3-a4e4a8442699">
-           <h6 id="986118f9-70b2-46bb-927c-0c6b86f7dcef">
+          <pre id="ea221b6d-01ec-490d-96ad-ee51ec9bfb92"><code class="python">for_password()</code></pre>
+          <div class="ml-3 collapse" id="21645b98-4d78-405b-b7c5-5e0a6d920e6b">
+           <h6 id="511bec6e-0052-44f8-98be-a077fb15a930">
             <strong>
              Returns
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="ab5ea99d-aade-4c6f-b1e9-c6d45c17e436">
+           <table class="table table-sm bg-light" id="788e4ce7-ce8b-457f-a474-582c39cea037">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -3120,67 +3185,68 @@
               <td>
                The instance of this class.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3" id="0977bd13-6782-4518-9da4-c30090c48620">
-           <h6 id="e6430b2c-ebde-4517-b588-89de4f208ec5">
+          <div class="ml-3" id="21955efe-cbd7-4814-87ea-cf8f4a62ef7a">
+           <h6 id="8aebe285-4df0-4200-afe6-ccd65a73b7ed">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="b6a7acc7-e71b-4b69-8c76-a02cadeef340"><code class="python">from bootwrap import Form, TextInput
+           <pre id="abacbfee-eacd-45f3-9a43-bc88f7ef51fc"><code class="python">from bootwrap import Form, TextInput
 
 Form(
     TextInput('Password', 'password', '********').for_password()
-)</code></pre>
+)
+</code></pre>
           </div>
-          <div class="ml-3" id="d05966cf-d3ee-4425-840c-46abf6b1aa25">
-           <form enctype="multipart/form-data" id="b432acdd-1868-4ebd-88bf-33092d537795" method="POST">
+          <div class="ml-3" id="0499164f-d815-42be-9d65-ce37d47525a5">
+           <form enctype="multipart/form-data" id="6cdc3a2b-91b1-4445-b1e4-57181e32d700" method="POST">
             <div class="form-group row">
-             <label class="col-sm-2 col-form-label d-flex align-items-center" for="a50a44e2-b7c3-4d2b-a4e6-7f8f38bdfae5">
+             <label class="col-sm-4 col-form-label d-flex align-items-center" for="96b14799-326b-4ddb-ba1c-3b3efa11ed91">
               Password
              </label>
-             <div class="col-sm-10 d-flex align-items-center">
-              <input class="form-control" id="a50a44e2-b7c3-4d2b-a4e6-7f8f38bdfae5" name="password" type="password" value="********"/>
+             <div class="col-sm-8 d-flex align-items-center">
+              <input class="form-control" id="96b14799-326b-4ddb-ba1c-3b3efa11ed91" name="password" type="password" value="********"/>
              </div>
             </div>
            </form>
           </div>
          </div>
-         <div class="mt-5" id="88a5da3e-9d35-4b47-9969-f73832f4ebc5">
-          <div class="d-flex justify-content-between" id="60a5078c-0677-4204-84f8-d1ed9d7f5a31">
-           <h4 id="df356099-47ba-435d-9ad2-cddf1365364d">
+         <div class="mt-5" id="044e4408-2670-4f5b-83ae-dc146f737895">
+          <div class="d-flex justify-content-between" id="1e7d46dc-33c2-4417-a71d-f89e43721c4e">
+           <h4 id="4849b576-7779-40c2-86cf-6021051507c8">
             Method
-            <span class="text-primary" id="a9053e7e-41be-49a5-a2b0-15422f730081">
+            <span class="text-primary" id="211e7408-0733-47df-9e90-b994653e3fb5">
              with_multirows
             </span>
            </h4>
-           <div id="cff7a6d8-a11e-47c0-9615-5b5f7a4deac3">
-            <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#2c7d6856-4572-43e9-a51c-7b70fa052c2e" data-toggle="collapse" id="23fd2341-4d5c-4b13-9c06-ed26a1c76fde" onclick="return false;" type="button">
+           <div id="677db036-818b-47e9-be32-87ef344edb74">
+            <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#3c1f368f-f303-46f7-9e94-89c640bbca88" data-toggle="collapse" id="10d654c4-7b5b-43ab-bfe3-e39eb9beb4b7" onclick="return false;" type="button">
              Argument
             </button>
-            <button class="btn-sm btn btn-outline-primary" data-target="#33d29644-8315-475c-8a4c-1b6addd6dc1c" data-toggle="collapse" id="e3384deb-5f27-4627-a055-08fd0ee0566a" onclick="return false;" type="button">
+            <button class="btn-sm btn btn-outline-primary" data-target="#4df2b75d-7d8d-4e5e-ab9b-70901ba25e6f" data-toggle="collapse" id="2b60faa4-8e83-4a9d-81b1-55512006ba68" onclick="return false;" type="button">
              Returns
             </button>
            </div>
           </div>
-          <span class="text-muted" id="3effa28a-c7f1-43d8-8c20-a41f9db36133">
+          <span class="text-muted" id="7b196eb5-68f3-4874-9725-20cb6bc1e310">
            Sets the number of rows.
           </span>
-          <pre id="c7097366-10fb-41a8-9a0b-1df18c005dca"><code class="python">with_multirows(n)</code></pre>
-          <div class="ml-3 collapse" id="2c7d6856-4572-43e9-a51c-7b70fa052c2e">
-           <h6 id="7db2ee62-57d4-4474-9d29-dbd736edb125">
+          <pre id="84885e62-833b-40c8-92cd-124361383a67"><code class="python">with_multirows(n)</code></pre>
+          <div class="ml-3 collapse" id="3c1f368f-f303-46f7-9e94-89c640bbca88">
+           <h6 id="d226cc4b-8cbb-4859-bfe2-1f0aa4847ebf">
             <strong>
              Arguments
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="1e0b7c0e-3e5d-4af9-81c0-b48b0d1737ee">
+           <table class="table table-sm bg-light" id="c106f55f-5fe4-41d7-9418-0a96b088f97a">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -3205,21 +3271,21 @@
               <td>
                The number of rows to set.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3 collapse" id="33d29644-8315-475c-8a4c-1b6addd6dc1c">
-           <h6 id="1925afe7-7ee0-4135-bd96-34e179de8525">
+          <div class="ml-3 collapse" id="4df2b75d-7d8d-4e5e-ab9b-70901ba25e6f">
+           <h6 id="040c91ef-7ef7-4904-a8e8-b00223259ad8">
             <strong>
              Returns
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="2401879a-609d-478f-8f83-6b0a28a0c57a">
+           <table class="table table-sm bg-light" id="4646a9ad-78a9-465c-aa2c-81ee84b61bac">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -3244,69 +3310,70 @@
               <td>
                The instance of this class.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3" id="691bcc8e-58ba-4794-8420-762186add253">
-           <h6 id="1bcab388-f421-4f60-bf35-7cfe24bdcc09">
+          <div class="ml-3" id="ddde4633-b122-4b5f-97c2-4817cd0716af">
+           <h6 id="6f8f18ad-807f-4faf-908c-d2eecda5a7b3">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="496da799-0059-40fc-a9f3-aca404f0c3db"><code class="python">from bootwrap import Form, TextInput
+           <pre id="c6d6aa34-cb6c-4404-a819-0be3843e920c"><code class="python">from bootwrap import Form, TextInput
 
 Form(
     TextInput('Text', 'text').with_multirows(3)
-)</code></pre>
+)
+</code></pre>
           </div>
-          <div class="ml-3" id="c2eca04a-f654-480d-8439-26dd1eb5ed9b">
-           <form enctype="multipart/form-data" id="bcc6216c-856b-4bcf-bbc0-91a6fdf8437e" method="POST">
+          <div class="ml-3" id="7acaf5a8-abdf-4b72-88f8-c48c45429dd6">
+           <form enctype="multipart/form-data" id="1c4f6582-cc37-451b-b3f7-6c890102b87a" method="POST">
             <div class="form-group row">
-             <label class="col-sm-2 col-form-label d-flex align-items-center" for="960f18e4-09f0-4e86-ae28-4a3bb3a0e928">
+             <label class="col-sm-4 col-form-label d-flex align-items-center" for="5c8ff5ff-7000-4e42-b83c-9fc54cef19c6">
               Text
              </label>
-             <div class="col-sm-10 d-flex align-items-center">
-              <textarea class="form-control" id="960f18e4-09f0-4e86-ae28-4a3bb3a0e928" name="text" rows="3">
+             <div class="col-sm-8 d-flex align-items-center">
+              <textarea class="form-control" id="5c8ff5ff-7000-4e42-b83c-9fc54cef19c6" name="text" rows="3">
                     
                 </textarea>
              </div>
             </div>
            </form>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="6a70564d-76b9-4f89-a2f6-20b801b6573b">
-        <div class="mt-5" id="244beefd-0554-4d9e-9342-75f84290f7c1">
-         <div class="d-flex justify-content-between" id="dde0bd6d-5555-4ce6-ba7b-e6ec24141bf1">
-          <h1 id="4474a7d5-cf97-45a7-8c4c-e3f9c6889f52">
+       <div class="tab-pane fade" id="c0c5bab6-43ae-45b4-a0d9-e2e703e4aee5">
+        <div class="mt-5" id="4fb30838-c4da-43f4-aa15-2fa145317eab">
+         <div class="d-flex justify-content-between" id="5e66119a-226d-4a9c-9c07-166e9cbe2d07">
+          <h1 id="4b278c8e-a738-4d21-9a38-2f1ca39f414e">
            Class
-           <span class="text-primary" id="f833b715-9954-491b-a265-ff84f0514e02">
+           <span class="text-primary" id="75b5e01d-9eea-455d-aa02-2a221ec50019">
             NumericInput
            </span>
           </h1>
-          <div id="7b106ca0-fa46-415e-adde-2362b549344c">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#02ba2bd5-c37b-4aa1-b168-1566c01051e6" data-toggle="collapse" id="5880466c-ac02-4ff7-9814-1d57c418547a" onclick="return false;" type="button">
+          <div id="c3ff996b-226f-4162-bcbf-20186263364d">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#da134c16-6042-4954-9bcd-963fa3cc1dcf" data-toggle="collapse" id="e62b48cc-c888-474a-af9a-abef6093460e" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="7ee6093a-96de-4749-b99b-03bf5b3a2d16">
+         <span class="text-muted" id="a9a3dc4a-db58-480d-82c2-31892ece61eb">
           A numeric input.
          </span>
-         <pre id="8d09c8e1-f7a4-4117-8842-d6ab207faed4"><code class="python">NumericInput(label, name, value=None, placeholder=None)</code></pre>
-         <div class="ml-3 collapse" id="02ba2bd5-c37b-4aa1-b168-1566c01051e6">
-          <h6 id="fefb0f9a-4487-4da7-8f20-4f6c3f503cb8">
+         <pre id="931e98d2-aac3-4dd1-8fb5-c8b00d7b4ad7"><code class="python">NumericInput(label, name, value=None, placeholder=None)</code></pre>
+         <div class="ml-3 collapse" id="da134c16-6042-4954-9bcd-963fa3cc1dcf">
+          <h6 id="0f1578e4-b8d9-498c-8945-d00ad4ff0df1">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="5f0d9832-4580-4bda-8c95-9578cb442f6c">
+          <table class="table table-sm bg-light" id="c11609de-a777-4f8c-88bd-e839c530d832">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -3376,105 +3443,106 @@
              <td>
               The input placeholder.
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <p id="f437b124-3729-42e8-9e69-5b176f0f006a">
+         <p id="7c1de734-a54d-4b00-a435-ff0c0c00a216">
           Use the
           <code>
            as_disabled()
           </code>
           function to prevent the user from entering data
     to the
           <code>
            NumericInput
           </code>
           component.
          </p>
-         <div class="ml-3" id="ffb47e5a-3c10-4b31-bddd-79271ec1be32">
-          <h6 id="7314995e-3004-4f35-9cba-3a66a658f33a">
+         <div class="ml-3" id="95928b0e-db64-4411-9e17-dc40e3803055">
+          <h6 id="d5445387-ae97-4a93-b35b-d354dce8b633">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="a8bda151-c280-48cf-943a-a13d262bdf42"><code class="python">from bootwrap import Form, TextInput
+          <pre id="a27cb9c4-decf-4740-af36-35d61a7dfe90"><code class="python">from bootwrap import Form, NumericInput
 
 Form(
     NumericInput('Number1', 'number'),
     NumericInput('Number2', 'number', placeholder='type here'),
     NumericInput('Number3', 'number', 123),
     NumericInput('Number4', 'number').as_disabled()
-)</code></pre>
+)
+</code></pre>
          </div>
-         <div class="ml-3" id="e860b709-af97-4598-aa99-7a2e04b08f55">
-          <form enctype="multipart/form-data" id="d678d2f5-dbc7-424b-8ce1-9bb75ce90a68" method="POST">
+         <div class="ml-3" id="f9352ed8-06f9-42aa-b21b-507d78a73bf0">
+          <form enctype="multipart/form-data" id="c19b68e6-adc5-498a-96c3-ce8dea28a6b5" method="POST">
            <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center" for="2b73c635-19c9-4dd8-a3b0-88194864c751">
+            <label class="col-sm-4 col-form-label d-flex align-items-center" for="143df711-8902-4189-b7cf-6d3cc87e9553">
              Number1
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
-             <input class="form-control" id="2b73c635-19c9-4dd8-a3b0-88194864c751" name="number" type="number"/>
+            <div class="col-sm-8 d-flex align-items-center">
+             <input class="form-control" id="143df711-8902-4189-b7cf-6d3cc87e9553" name="number" type="number"/>
             </div>
            </div>
            <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center" for="76762c85-09a6-4ea4-a0c6-9513bde834e2">
+            <label class="col-sm-4 col-form-label d-flex align-items-center" for="5e1c471f-4fa6-4caf-b30b-4ada5ae3ac3d">
              Number2
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
-             <input class="form-control" id="76762c85-09a6-4ea4-a0c6-9513bde834e2" name="number" placeholder="type here" type="number"/>
+            <div class="col-sm-8 d-flex align-items-center">
+             <input class="form-control" id="5e1c471f-4fa6-4caf-b30b-4ada5ae3ac3d" name="number" placeholder="type here" type="number"/>
             </div>
            </div>
            <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center" for="ae7de23e-6576-4bc0-a41d-be7f71bde3a9">
+            <label class="col-sm-4 col-form-label d-flex align-items-center" for="627fee12-c7b5-4ed5-81b9-66b605f2ba62">
              Number3
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
-             <input class="form-control" id="ae7de23e-6576-4bc0-a41d-be7f71bde3a9" name="number" type="number" value="123"/>
+            <div class="col-sm-8 d-flex align-items-center">
+             <input class="form-control" id="627fee12-c7b5-4ed5-81b9-66b605f2ba62" name="number" type="number" value="123"/>
             </div>
            </div>
            <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center" for="e599207a-5782-4e40-baf4-f85317847014">
+            <label class="col-sm-4 col-form-label d-flex align-items-center" for="003d6c2f-3e83-46f6-a7be-a796487be5e3">
              Number4
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
-             <input class="form-control" disabled="" id="e599207a-5782-4e40-baf4-f85317847014" name="number" type="number"/>
+            <div class="col-sm-8 d-flex align-items-center">
+             <input class="form-control" disabled="" id="003d6c2f-3e83-46f6-a7be-a796487be5e3" name="number" type="number"/>
             </div>
            </div>
           </form>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="e2790200-471a-46f6-a282-53f9a693e531">
-        <div class="mt-5" id="94711cb1-48f7-4c62-9788-5a4a3d821370">
-         <div class="d-flex justify-content-between" id="07c27ca7-de89-4349-9231-14442ef4edd4">
-          <h1 id="922516b2-34b9-4286-9d62-6474eef367fd">
+       <div class="tab-pane fade" id="fb4c3830-15e3-4f92-8f80-f7f24ce90fb5">
+        <div class="mt-5" id="6ca80f08-ce4d-4557-8209-c494ee1c87de">
+         <div class="d-flex justify-content-between" id="267f1a55-c41f-451a-8f1b-86f2b95258b9">
+          <h1 id="84f19015-5d2b-43fc-a315-94129fd3da3d">
            Class
-           <span class="text-primary" id="fd40ec4c-9120-4f93-8c2b-d855db90cbe9">
+           <span class="text-primary" id="1ad876da-1cb6-47fd-a9ab-6145d2dfa6d8">
             SelectInput
            </span>
           </h1>
-          <div id="7068b762-c878-45c0-bf61-cf602355455b">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#ccf2f18e-8f43-443a-9a6f-759cf1073b6c" data-toggle="collapse" id="2f821b95-1b11-40e8-aeae-1ccb2e86b73d" onclick="return false;" type="button">
+          <div id="4bd99b1e-e38f-4636-9d17-3fb389d46811">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#586a5718-d132-4e1d-88aa-7caac7f8521d" data-toggle="collapse" id="e4599e7b-d6c9-495c-a1aa-67e0ab6ebf1e" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="e3c780c1-33f3-4490-91c8-8496e0a60b00">
+         <span class="text-muted" id="2ecd1e7e-9580-49d4-bda8-09001792e3e8">
           A select input.
          </span>
-         <pre id="5d76618e-18c8-4ed1-b695-d6a5aa5df438"><code class="python">SelectInput(label, name, value=None, options=None)</code></pre>
-         <div class="ml-3 collapse" id="ccf2f18e-8f43-443a-9a6f-759cf1073b6c">
-          <h6 id="ce233ac5-f520-41e3-95f0-1aad11fa7d01">
+         <pre id="6fe31376-0809-4c35-9421-24783170dc50"><code class="python">SelectInput(label, name, value=None, options=None)</code></pre>
+         <div class="ml-3 collapse" id="586a5718-d132-4e1d-88aa-7caac7f8521d">
+          <h6 id="0a96cc17-daa0-4069-a620-a4aaa363404e">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="745f6a6a-fbde-44a7-81ba-6ccdc37beaed">
+          <table class="table table-sm bg-light" id="3880606d-678a-4ac8-9345-8593f6cbd61b">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -3544,110 +3612,111 @@
              <td>
               The input options.
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <p id="95d9ce46-9a97-4d74-853d-8b36aea8a057">
+         <p id="cc2e0f82-4fc6-4342-a498-4cef5115f0a7">
           Use the
           <code>
            as_disabled()
           </code>
           function to prevent the user from entering data
     to the
           <code>
            SelectInput
           </code>
           component.
          </p>
-         <div class="ml-3" id="9965e050-48b3-4d35-8701-b7e5a00cab5c">
-          <h6 id="b440fe67-48ef-4915-86da-469559aa98c6">
+         <div class="ml-3" id="e20eaa6f-8766-44db-a4a4-18fe415e47e9">
+          <h6 id="cd27f625-0aa5-4fd0-8f76-26da34bd03b0">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="b438a6bf-b8e0-4615-aab9-cfedaab205ec"><code class="python">from bootwrap import Form, SelectInput
+          <pre id="99a14f0d-dadb-4762-8660-6fdc285c7731"><code class="python">from bootwrap import Form, SelectInput
 
 options = [
     SelectInput.Option('One', 1),
     SelectInput.Option('Two', 2),
     SelectInput.Option('Three', 3, disabled=True)
 ]
 
 Form(
-    SelectInput('Selector1', 'choice', 2, options)
+    SelectInput('Selector1', 'choice', 2, options),
     SelectInput('Selector2', 'choice', 2, options).as_disabled()
-)</code></pre>
+)
+</code></pre>
          </div>
-         <div class="ml-3" id="bb889dc6-2998-4ba3-a13b-704340158afc">
-          <form enctype="multipart/form-data" id="eceb2da3-db31-45b1-bdb8-2d8c07e2ac57" method="POST">
+         <div class="ml-3" id="969453b1-1ac3-49e5-911d-509a4967ae20">
+          <form enctype="multipart/form-data" id="8e4bb9f2-51f8-4142-a277-68cac67cd7d6" method="POST">
            <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center" for="ad98f947-fd16-47bf-8667-07e2a1af3262">
+            <label class="col-sm-4 col-form-label d-flex align-items-center" for="cef810d1-e36d-4990-8353-2ca82d528160">
              Selector1
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
-             <select autocomplete="off" class="form-control" id="ad98f947-fd16-47bf-8667-07e2a1af3262" name="choice">
-              <option id="4db25561-391c-4d72-8fe8-b495d1aacf23" value="1">
+            <div class="col-sm-8 d-flex align-items-center">
+             <select autocomplete="off" class="form-control" id="cef810d1-e36d-4990-8353-2ca82d528160" name="choice">
+              <option id="7c6ba843-faf9-4bd3-a945-c689cef77604" value="1">
                One
               </option>
-              <option id="80ca13c5-def1-4fc9-a0a3-56753a8c1fe4" selected="" value="2">
+              <option id="7a9817bc-5f0d-4e3a-a463-5f7c726ff3f6" selected="" value="2">
                Two
               </option>
-              <option disabled="" id="9a6f95ec-cde5-4d40-98a1-d6a71b2287ee" value="3">
+              <option disabled="" id="784e2203-ddab-4fd5-aab8-cda0e81315b0" value="3">
                Three
               </option>
              </select>
             </div>
            </div>
            <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center" for="c0bc9b0a-a002-42dc-bf7a-51b4642a1360">
+            <label class="col-sm-4 col-form-label d-flex align-items-center" for="590fb479-64d3-43c6-ab27-8178a94a1b46">
              Selector2
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
-             <select autocomplete="off" class="form-control" disabled="" id="c0bc9b0a-a002-42dc-bf7a-51b4642a1360" name="choice">
-              <option id="4db25561-391c-4d72-8fe8-b495d1aacf23" value="1">
+            <div class="col-sm-8 d-flex align-items-center">
+             <select autocomplete="off" class="form-control" disabled="" id="590fb479-64d3-43c6-ab27-8178a94a1b46" name="choice">
+              <option id="7c6ba843-faf9-4bd3-a945-c689cef77604" value="1">
                One
               </option>
-              <option id="80ca13c5-def1-4fc9-a0a3-56753a8c1fe4" selected="" value="2">
+              <option id="7a9817bc-5f0d-4e3a-a463-5f7c726ff3f6" selected="" value="2">
                Two
               </option>
-              <option disabled="" id="9a6f95ec-cde5-4d40-98a1-d6a71b2287ee" value="3">
+              <option disabled="" id="784e2203-ddab-4fd5-aab8-cda0e81315b0" value="3">
                Three
               </option>
              </select>
             </div>
            </div>
           </form>
          </div>
-         <div class="mt-5" id="05a04fc9-3cd8-429f-89ff-8b9a2283664d">
-          <div class="d-flex justify-content-between" id="d9f30e2a-8547-450f-bec6-e20617aa299f">
-           <h4 id="05b5925b-6562-44d7-a834-d82715aad54f">
+         <div class="mt-5" id="7f8a3200-9437-45bc-b985-e5b153b7ec66">
+          <div class="d-flex justify-content-between" id="c56f1ce0-89a7-43c4-855f-07ac79906d1a">
+           <h4 id="42bfb19c-eba6-41e2-80e9-a9f4ec644108">
             Method
-            <span class="text-primary" id="8fc25f87-583c-4c86-9483-798e0e8b9d79">
+            <span class="text-primary" id="6ba8b4d5-b122-43bb-a1df-85da99ac6d68">
              as_radio
             </span>
            </h4>
-           <div id="bb6fcbdb-aa18-4836-9e76-72dffcef2415">
-            <button class="btn-sm btn btn-outline-primary" data-target="#13cfe8b7-c77c-4dff-8203-dc6a620ef2a1" data-toggle="collapse" id="6f553138-392d-4f43-a5f0-cd561a92409b" onclick="return false;" type="button">
+           <div id="64302697-3676-472d-98a9-9975f925fa10">
+            <button class="btn-sm btn btn-outline-primary" data-target="#921c7026-fc3f-4748-9ab0-5cc052fe3466" data-toggle="collapse" id="c707ef65-fbce-435d-b689-c8f1669a6cf8" onclick="return false;" type="button">
              Returns
             </button>
            </div>
           </div>
-          <span class="text-muted" id="9d19f4eb-f948-4a82-b710-4230b28d5ded">
+          <span class="text-muted" id="2f3e9174-37cc-4480-b4f1-03c322e2aac4">
            Makes selection in a form of radio buttons.
           </span>
-          <pre id="7b7b217f-14f4-47a8-a9cc-b0d515492aed"><code class="python">as_radio()</code></pre>
-          <div class="ml-3 collapse" id="13cfe8b7-c77c-4dff-8203-dc6a620ef2a1">
-           <h6 id="2ba902d7-1c82-4ecb-a441-63579f1607ff">
+          <pre id="8d82b7ea-4b11-4fca-bffd-cb0329642776"><code class="python">as_radio()</code></pre>
+          <div class="ml-3 collapse" id="921c7026-fc3f-4748-9ab0-5cc052fe3466">
+           <h6 id="9befa2bc-4062-4164-b259-8382c5826091">
             <strong>
              Returns
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="516e2934-3a2a-4447-b016-85f63a5baaf4">
+           <table class="table table-sm bg-light" id="26fce005-5dbd-410b-82a7-5f398d523e9c">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -3672,94 +3741,95 @@
               <td>
                The instance of this class.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3" id="1ffb4d72-fae9-43d0-891c-1d86a9a218ea">
-           <h6 id="2b940f73-1f61-491d-b160-b35db1afd5e5">
+          <div class="ml-3" id="aa98b5c7-7a40-4e7b-839e-e73fea640652">
+           <h6 id="2fa4cd25-287a-4f0b-9205-b17272d60fce">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="a15a8556-0f02-41db-a52a-5371ea485934"><code class="python">from bootwrap import Form, SelectInput
+           <pre id="c2239872-6106-4b0b-9fa7-7f3c5efc6c4a"><code class="python">from bootwrap import Form, SelectInput
 
 options = [
     SelectInput.Option('One', 1),
     SelectInput.Option('Two', 2),
     SelectInput.Option('Three', 3, disabled=True)
 ]
 
 Form(
     SelectInput('Selector', 'choice', 2, options).as_radio()
-)</code></pre>
+)
+</code></pre>
           </div>
-          <div class="ml-3" id="6e9f7eb6-91ea-4a59-84c6-7cb996719141">
-           <form enctype="multipart/form-data" id="12fa7452-999d-497d-bfe1-19223117447e" method="POST">
+          <div class="ml-3" id="32d27074-389b-4758-8a21-6edb9f241b98">
+           <form enctype="multipart/form-data" id="40ba6dfc-8e1e-474c-aa78-6e80404e2cba" method="POST">
             <div class="form-group row">
-             <label class="col-sm-2 col-form-label d-flex align-items-center" for="054ada86-badf-4774-b83b-ac4876d6dc48">
+             <label class="col-sm-4 col-form-label d-flex align-items-center" for="6476625f-964d-42f3-8f49-71323ea07a2c">
               Selector
              </label>
-             <div class="col-sm-10 d-flex align-items-center">
+             <div class="col-sm-8 d-flex align-items-center">
               <div class="form-check mr-3">
-               <input autocomplete="off" class="form-check-input" id="2b87f2d5-f44d-41e5-ae31-d240bd9cc6e4" name="choice" type="radio" value="1"/>
-               <label class="form-check-label mr-1" for="2b87f2d5-f44d-41e5-ae31-d240bd9cc6e4">
+               <input autocomplete="off" class="form-check-input" id="7fc8e31f-6d0d-4581-a014-7668d8d29fbc" name="choice" type="radio" value="1"/>
+               <label class="form-check-label mr-1" for="7fc8e31f-6d0d-4581-a014-7668d8d29fbc">
                 One
                </label>
               </div>
               <div class="form-check mr-3">
-               <input autocomplete="off" checked="" class="form-check-input" id="9afaab25-f0a1-4bc4-bee3-cd6077c95e16" name="choice" type="radio" value="2"/>
-               <label class="form-check-label mr-1" for="9afaab25-f0a1-4bc4-bee3-cd6077c95e16">
+               <input autocomplete="off" checked="" class="form-check-input" id="faa83683-53c8-4a25-b976-4e4a1b29b839" name="choice" type="radio" value="2"/>
+               <label class="form-check-label mr-1" for="faa83683-53c8-4a25-b976-4e4a1b29b839">
                 Two
                </label>
               </div>
               <div class="form-check mr-3">
-               <input autocomplete="off" class="form-check-input" disabled="" id="7e091488-107a-4ca3-875d-043a0be47580" name="choice" type="radio" value="3"/>
-               <label class="form-check-label mr-1" for="7e091488-107a-4ca3-875d-043a0be47580">
+               <input autocomplete="off" class="form-check-input" disabled="" id="6aa8ab8a-da30-4c4c-816b-ffdf03828220" name="choice" type="radio" value="3"/>
+               <label class="form-check-label mr-1" for="6aa8ab8a-da30-4c4c-816b-ffdf03828220">
                 Three
                </label>
               </div>
              </div>
             </div>
            </form>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="26fccd40-b42a-476f-9fe9-55c162893a03">
-        <div class="mt-5" id="da488371-ed84-4a94-a091-55bfff832bdc">
-         <div class="d-flex justify-content-between" id="968a31a9-5111-4a28-b77d-466bea4ea3c5">
-          <h1 id="17622129-b1a4-4fb6-8627-da82ccf9e14d">
+       <div class="tab-pane fade" id="92519a90-1163-4949-b82a-dec5f4658ec9">
+        <div class="mt-5" id="130a3bcb-7864-4de6-b7bb-b5b8a19f368a">
+         <div class="d-flex justify-content-between" id="faa8ba2a-ff63-4714-b9a6-8bfb96ce9fe9">
+          <h1 id="2e4038dc-dbed-4a7d-805e-844bfdbce7fb">
            Class
-           <span class="text-primary" id="f0d2a6f1-aae9-4741-a55a-bc3e5ea35d15">
+           <span class="text-primary" id="14d41e47-36e6-47a6-a493-63a18cff50f7">
             SelectInput.Option
            </span>
           </h1>
-          <div id="77536010-31a4-4da6-89d2-9c800eb662ef">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#822a00c1-df4b-4a0a-9280-5958fe41b95d" data-toggle="collapse" id="8c7888e4-bcfd-489a-8464-31db520220ee" onclick="return false;" type="button">
+          <div id="f8a32471-d26b-40ea-848f-7d9cc98eb741">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#42723ec9-4d42-4768-8ef2-7f36a50d8d95" data-toggle="collapse" id="d77a846b-6d08-46c3-a7cd-61d32086a499" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="dbdd1b9c-6ab6-40a4-9a7f-43c47919b5e0">
+         <span class="text-muted" id="b2fe444d-2feb-4e4d-ba22-8c202008c597">
           An option used by
           <code>
            SelectInput
           </code>
           .
          </span>
-         <pre id="74b5c83c-3a62-4baf-9492-b9bf27d719a8"><code class="python">SelectInput.Option(name, value, disabled=False)</code></pre>
-         <div class="ml-3 collapse" id="822a00c1-df4b-4a0a-9280-5958fe41b95d">
-          <h6 id="e6882e4d-4e3d-4f18-a4d9-f6e8359f4a61">
+         <pre id="463b76cb-0048-4350-93de-59d8200d4070"><code class="python">SelectInput.Option(name, value, disabled=False)</code></pre>
+         <div class="ml-3 collapse" id="42723ec9-4d42-4768-8ef2-7f36a50d8d95">
+          <h6 id="a711a9ef-4107-4cab-b959-1158c6e1ddbb">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="9407e373-c61e-4c0b-b5e8-db882806a749">
+          <table class="table table-sm bg-light" id="6a4080df-43b0-49d3-88d5-ae180785b423">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -3818,75 +3888,75 @@
               makes the option disabled (in other words
                 user will not be able to choose this option).
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <div class="mt-5" id="f08b1b19-d86d-42aa-bb0b-8a3ba970450b">
-          <h4 id="31cb825c-93d8-4422-9e97-fd43f3cbae52">
+         <div class="mt-5" id="2af361af-7062-488d-800b-c6c98934ebd1">
+          <h4 id="9cff31ba-b86c-4a1c-999c-f40cf3ab3d7f">
            Property
-           <span class="text-primary" id="943cd1c3-f687-422e-adaf-249cae68225d">
+           <span class="text-primary" id="0ea363ad-522a-4f49-aba0-51fbfc09bd88">
             disabled
            </span>
           </h4>
-          <span class="text-muted" id="f3c68ba1-5688-4315-812b-e101f8709fc5">
+          <span class="text-muted" id="79ebcc6e-415f-4dfd-b355-b79cc1f67e7a">
            None
           </span>
          </div>
-         <div class="mt-5" id="26a488b8-80c3-48f4-add6-66b1b742b663">
-          <h4 id="59474f7e-36f3-43bc-9033-c4bd825f4493">
+         <div class="mt-5" id="38b48b40-902e-45dd-8980-252b91ef83c0">
+          <h4 id="33b5f450-7107-46d4-9af3-4f2b7b50e0d0">
            Property
-           <span class="text-primary" id="d8a8c756-3aef-4839-9c59-bb277f9abe74">
+           <span class="text-primary" id="d70c6264-78ed-4d99-b481-555321b75e0c">
             name
            </span>
           </h4>
-          <span class="text-muted" id="c6879ae8-928f-4062-8fc9-1ba48483cd10">
+          <span class="text-muted" id="5aaf0866-62a7-44d3-b61b-5965b27a48f9">
            None
           </span>
          </div>
-         <div class="mt-5" id="c97647b9-80c6-45b0-9a0b-37914b4147d7">
-          <h4 id="53c17823-6c47-456f-b463-7b21d2dcffad">
+         <div class="mt-5" id="737a280a-0a8e-4c3f-a899-43c30dca92ef">
+          <h4 id="1a89a392-3567-4e1e-a079-a6b4213d3526">
            Property
-           <span class="text-primary" id="e0b1e3ab-034e-44f3-afbc-30e2244babaf">
+           <span class="text-primary" id="0b705e94-6e05-44f7-a7a6-ee3ead3d47a7">
             value
            </span>
           </h4>
-          <span class="text-muted" id="a5d704c9-d34a-402f-b9c8-b6752c4a3cca">
+          <span class="text-muted" id="f5ddbef9-2a19-476d-8ea9-694f19c6b8d7">
            None
           </span>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="c4bb12d8-b3c2-425b-b6a2-a69c7ca8604c">
-        <div class="mt-5" id="1a3d757c-3ce9-49ab-9b4a-ad5390edfdef">
-         <div class="d-flex justify-content-between" id="ecd5f26a-3b5e-49f5-adc7-ba92f381a845">
-          <h1 id="df169b10-0cf6-4acb-b849-bbfb8ec8d1fd">
+       <div class="tab-pane fade" id="2d325dac-243f-43fd-9b89-f4034d175837">
+        <div class="mt-5" id="987daf0e-5582-460a-90ff-53a1a78d237e">
+         <div class="d-flex justify-content-between" id="d91ca1a3-f204-47c6-9ddf-e9e841ea629a">
+          <h1 id="6424dab5-123d-4bff-be54-7652022967fd">
            Class
-           <span class="text-primary" id="47deb2ac-b401-4ea9-82dd-f063e29297e0">
+           <span class="text-primary" id="fa7c3957-1482-4d26-a2ef-b876e62e9a2b">
             HiddenInput
            </span>
           </h1>
-          <div id="b8ed9c63-7189-48e9-9940-4428afae948c">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#03f4984d-93e4-475e-adac-f86ec43e4a29" data-toggle="collapse" id="072e957e-5712-4e93-b7d9-7c4341510e9f" onclick="return false;" type="button">
+          <div id="5a9b1ebd-f928-4799-9491-19a9fac675ed">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#c3a0b1cc-5137-44b6-b5b2-d85908cf65c2" data-toggle="collapse" id="c157e6ff-9cb2-417a-b62f-f3689ef003c3" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="fd6384c9-aae3-47c5-812d-2302672bb104">
+         <span class="text-muted" id="3659ea8b-57a7-42f4-a93d-c41ab9f50c47">
           A hidden input.
          </span>
-         <pre id="cabfaba9-270d-49b3-a36a-d87ab92edb7e"><code class="python">HiddenInput(name, value=None)</code></pre>
-         <div class="ml-3 collapse" id="03f4984d-93e4-475e-adac-f86ec43e4a29">
-          <h6 id="e2157886-9da7-47b6-9b8b-a1ccbf8ecc94">
+         <pre id="8fe464ed-9a97-4923-8203-2acbba54fc34"><code class="python">HiddenInput(name, value=None)</code></pre>
+         <div class="ml-3 collapse" id="c3a0b1cc-5137-44b6-b5b2-d85908cf65c2">
+          <h6 id="a072c80c-9ab8-4275-a075-7007f387f3e9">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="9f2b18cf-30f2-4f36-a3d8-d28d25118b87">
+          <table class="table table-sm bg-light" id="99f37547-4936-459a-9ae0-6373d79b75d9">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -3926,54 +3996,55 @@
              <td>
               The input value.
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <div class="ml-3" id="fb603134-a1f7-4a90-86d2-56534c2e2574">
-          <h6 id="5762886d-047e-4941-9242-c4532666bef6">
+         <div class="ml-3" id="5cd5f581-a895-4d73-8344-220ff0ddb65c">
+          <h6 id="34260dc7-8a03-4144-ab2b-599fba7e5e51">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="bac918e8-891c-45bd-8d71-f9c676e0c8d0"><code class="python">from bootwrap import Form, SelectInput
+          <pre id="a001f3ff-7e6e-4f22-a2a3-4dac3c112607"><code class="python">from bootwrap import Form, SelectInput
 
 Form(
     HiddenInput('token', '123')
-)</code></pre>
+)
+</code></pre>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="223e9820-15a1-4fb4-8942-f7b4fea2009c">
-        <div class="mt-5" id="c0317746-b850-485c-a475-1ee7b226622b">
-         <div class="d-flex justify-content-between" id="6fd1f4de-3fa4-4516-a49e-0e736ed5075a">
-          <h1 id="07151b80-0fb3-4e11-b5ae-fb43a144acbc">
+       <div class="tab-pane fade" id="f8c73225-c95f-4444-a9e8-540c16a26bac">
+        <div class="mt-5" id="6733291b-86e7-4b43-bd47-318ab42a9378">
+         <div class="d-flex justify-content-between" id="09820658-26e8-4988-9730-43c08a41df54">
+          <h1 id="5d8c3ba3-6569-46c6-ba76-1c0443d90ed7">
            Class
-           <span class="text-primary" id="04eb476b-323b-47c5-8826-69a4b5aa11f9">
+           <span class="text-primary" id="b0eabe03-c23e-4d52-891d-42226add1323">
             FileInput
            </span>
           </h1>
-          <div id="02b57e8c-a253-4247-8049-da15a09fadf9">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#0811713f-3a23-4889-9b5f-975c0d05fff0" data-toggle="collapse" id="e4f4bc24-1ece-4750-80b0-73a786b9aced" onclick="return false;" type="button">
+          <div id="80bd043a-3a7b-449e-9cb1-e6caa18a505e">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#d0495c26-032b-4be8-8590-a5b811192d6b" data-toggle="collapse" id="dc6aaae9-343b-4a85-9ab4-201632c945e5" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="46fb7e5c-4753-4b4d-b5e8-fd1861c271b4">
+         <span class="text-muted" id="6f076dd5-3fd8-4fc4-9115-a918897b6c3d">
           A file input.
          </span>
-         <pre id="4d478b94-77ba-4bdd-bcbc-d1b06ca13dc6"><code class="python">FileInput(label, name)</code></pre>
-         <div class="ml-3 collapse" id="0811713f-3a23-4889-9b5f-975c0d05fff0">
-          <h6 id="9fa2dae7-5478-47c5-9164-4e77c41975b8">
+         <pre id="3a004f52-03de-483e-84cc-c2cdeae05d38"><code class="python">FileInput(label, name)</code></pre>
+         <div class="ml-3 collapse" id="d0495c26-032b-4be8-8590-a5b811192d6b">
+          <h6 id="6f184119-9176-4763-8c63-e4d5e6cdcfe4">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="b03e76a1-03e8-468d-adc1-5797c5974f5e">
+          <table class="table table-sm bg-light" id="5145fcbc-0dc3-4f22-9937-80f506bfd2c2">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -4013,128 +4084,129 @@
              <td>
               The input name.
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <p id="c9bfbec1-c341-47d4-ba21-908a57080cec">
+         <p id="a65a3186-1487-485d-9d4b-7ba90a42bb34">
           Use the
           <code>
            as_disabled()
           </code>
           function to prevent the user from entering data
     to the
           <code>
            FileInput
           </code>
           component.
          </p>
-         <div class="ml-3" id="8d65c852-e418-445c-a4f6-df1591b40f05">
-          <h6 id="76a1fa97-1f1a-40b6-931e-759aac5dc224">
+         <div class="ml-3" id="6cda07de-a8b7-4768-ba5f-a114c76467fd">
+          <h6 id="5d91f595-6dfb-4b9f-8013-c90282206ce2">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="cd61a134-81cc-4261-b7fc-2efbbf09760b"><code class="python">from bootwrap import Form, FileInput
+          <pre id="e2561b99-a580-42da-a826-8feb08657240"><code class="python">from bootwrap import Form, FileInput
 
-output = Form(
+Form(
     FileInput('File', 'file'),
     FileInput('File', 'file').as_disabled()
-)</code></pre>
+)
+</code></pre>
          </div>
-         <div class="ml-3" id="ffb5ab18-b46c-427b-ac3e-2f7958622fd3">
-          <form enctype="multipart/form-data" id="7cd8995f-4ee5-4174-8249-ac162987cae2" method="POST">
+         <div class="ml-3" id="b65b073d-d8f5-4a9c-a9f9-8e31fa374c83">
+          <form enctype="multipart/form-data" id="2c50d635-733e-4786-a197-c7ebe8f31612" method="POST">
            <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center" for="c92a3400-8b5e-4747-9121-86917bdbfffd">
+            <label class="col-sm-4 col-form-label d-flex align-items-center" for="11e880d3-72ff-4744-933d-823359a6280a">
              File
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
+            <div class="col-sm-8 d-flex align-items-center">
              <div class="input-group">
               <span class="form-control input-group-append">
               </span>
               <div class="input-group-append">
                <span class="btn btn-secondary" onclick="$(this).parent().find('input[type=file]').click();">
                 Browse
                </span>
-               <input id="c92a3400-8b5e-4747-9121-86917bdbfffd" name="file" onchange="$(this).parent().parent().find('.form-control').html($(this).val().split(/[\|/]/).pop());" style="display: none;" type="file"/>
+               <input id="11e880d3-72ff-4744-933d-823359a6280a" name="file" onchange="$(this).parent().parent().find('.form-control').html($(this).val().split(/[\|/]/).pop());" style="display: none;" type="file"/>
               </div>
              </div>
             </div>
            </div>
            <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center" for="1430ba2f-087b-4e2a-a7c2-db0ab973afb3">
+            <label class="col-sm-4 col-form-label d-flex align-items-center" for="530f32be-c22a-400d-be4d-6c4f0556be00">
              File
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
+            <div class="col-sm-8 d-flex align-items-center">
              <div class="input-group">
               <span class="form-control input-group-append">
               </span>
               <div class="input-group-append">
                <span class="btn btn-secondary disabled" onclick="$(this).parent().find('input[type=file]').click();">
                 Browse
                </span>
-               <input disabled="" id="1430ba2f-087b-4e2a-a7c2-db0ab973afb3" name="file" onchange="$(this).parent().parent().find('.form-control').html($(this).val().split(/[\|/]/).pop());" style="display: none;" type="file"/>
+               <input disabled="" id="530f32be-c22a-400d-be4d-6c4f0556be00" name="file" onchange="$(this).parent().parent().find('.form-control').html($(this).val().split(/[\|/]/).pop());" style="display: none;" type="file"/>
               </div>
              </div>
             </div>
            </div>
           </form>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="f0970b4c-6f15-48d3-9246-d8d245af3e57">
-     <div id="265eb924-fbfa-4deb-9749-670b3f77b592">
+    <div class="tab-pane fade" id="4793739d-4728-4d95-a8e8-324923a67504">
+     <div id="b3686b16-d9fe-4a8d-a8e0-78a17321a887">
       <hr/>
-      <ul class="nav" id="9cd34902-a865-4cbb-87cc-db7f623ae817" role="tablist">
+      <ul class="nav" id="b401b649-1785-41d7-b9a4-4fe3869e8e3a" role="tablist">
        <li class="nav-item">
-        <a class="nav-link active" data-target="#05f2292c-0bed-4098-a641-ade322bcd7ff" data-toggle="tab" href="#05f2292c-0bed-4098-a641-ade322bcd7ff" id="73fb721d-e160-4831-8233-1a790f932f1a" role="tab">
-         <span class="text-secondary" id="151c9546-0a10-41bb-911f-b58135cf72ec">
+        <a class="nav-link active" data-target="#c23b2590-c0b7-4609-b779-1b79cb15cc91" data-toggle="tab" href="#c23b2590-c0b7-4609-b779-1b79cb15cc91" id="92495c7b-03ec-4bce-9049-5e98dcb84235" role="tab">
+         <span class="text-secondary" id="1ea4be3c-e336-426a-a290-ebf64b176ab1">
           Icon
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#27176909-960c-479a-b89b-a4a6d18d7f05" data-toggle="tab" href="#27176909-960c-479a-b89b-a4a6d18d7f05" id="0ac95010-c581-44ad-aef1-c88840d6a330" role="tab">
-         <span class="text-secondary" id="1dbc4ee1-53fe-4f44-b265-05b855de9b06">
+        <a class="nav-link" data-target="#7ab63f00-dd8e-4673-80f0-30471aff2f3d" data-toggle="tab" href="#7ab63f00-dd8e-4673-80f0-30471aff2f3d" id="2dd5560e-f692-44c0-ae09-887d0c3db59c" role="tab">
+         <span class="text-secondary" id="163e5db5-ad97-440e-9f51-209998139d01">
           Spinner
          </span>
         </a>
        </li>
       </ul>
       <div class="tab-content">
-       <div class="tab-pane fade active show" id="05f2292c-0bed-4098-a641-ade322bcd7ff">
-        <div class="mt-5" id="8b45f456-b6ab-4ba9-a7a5-c7d8e5006173">
-         <div class="d-flex justify-content-between" id="eb6292a0-2b88-44a6-90a2-7cb3e2bf5c7a">
-          <h1 id="43d01d2c-d190-4876-9ca5-73bc90beea51">
+       <div class="tab-pane fade active show" id="c23b2590-c0b7-4609-b779-1b79cb15cc91">
+        <div class="mt-5" id="943998cf-4dad-47c6-9ca3-b562fac9d967">
+         <div class="d-flex justify-content-between" id="01b2f04a-f190-4c7f-af85-e4d408ca0b94">
+          <h1 id="63cf298a-3fdf-447a-b439-97e3defe88f3">
            Class
-           <span class="text-primary" id="7ea3ed7e-a24e-465f-afe3-0854a61fa058">
+           <span class="text-primary" id="a60e6114-6e47-4631-b04d-aec651ec8015">
             Icon
            </span>
           </h1>
-          <div id="3906afe6-1cba-416c-8c91-2fc7d82778ea">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#3ecf69bd-e7cd-48a6-b2f0-3c0b0ca027c4" data-toggle="collapse" id="48c6f11d-3488-4772-ad86-f80b6a7b7a09" onclick="return false;" type="button">
+          <div id="0a687cb2-7da3-4a9b-a43e-c421ab5188af">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#fb6c457f-b37a-4c21-8149-4632d43eb081" data-toggle="collapse" id="0aa2ecbc-2bad-4f44-99a8-45b500cbf200" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="5ea1e163-b222-481a-b229-3ee030c8bb4a">
+         <span class="text-muted" id="57321925-0d15-402a-9301-d20909b3d48f">
           An icon.
          </span>
-         <pre id="19baabf1-161f-4db7-a51d-519e2eb96c6e"><code class="python">Icon(name)</code></pre>
-         <div class="ml-3 collapse" id="3ecf69bd-e7cd-48a6-b2f0-3c0b0ca027c4">
-          <h6 id="83102679-35b9-4ae5-bb19-3be44cb8033a">
+         <pre id="999c73ed-c2ef-47eb-a7aa-41ad76d477f2"><code class="python">Icon(name)</code></pre>
+         <div class="ml-3 collapse" id="fb6c457f-b37a-4c21-8149-4632d43eb081">
+          <h6 id="f80a092f-d0d9-446d-ac71-f340a052bcd7">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="d7def840-b1dd-474f-a35d-b88bc2bbff88">
+          <table class="table table-sm bg-light" id="0837a959-cf26-49b1-92c0-df0ffa1bb83c">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -4159,93 +4231,99 @@
              <td>
               The icon name.
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <div class="ml-3" id="4b6c8b6a-98a1-4929-8474-82b7ac601e85">
-          <h6 id="91bafaf7-2176-4e53-a990-ded684356b17">
+         <div class="ml-3" id="d04a5f63-e206-4666-aea9-7e8e26575f34">
+          <h6 id="919930ab-6983-4339-92d3-e611101e5675">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="3c1e88bb-663e-4c89-907d-e59604d40b79"><code class="python">from bootwrap import Icon
+          <pre id="39644831-6f27-4897-8953-321f0082a49d"><code class="python">from bootwrap import Icon, Panel
 
-Icon("fas fa-folder")
-Icon("fas fa-folder").as_primary()
-Icon("fas fa-folder").as_secondary()
-Icon("fas fa-folder").as_success()
-Icon("fas fa-folder").as_warning()
-Icon("fas fa-folder").as_danger()
-Icon("fas fa-folder").as_info()
-Icon("fas fa-folder").as_light()
-Icon("fas fa-folder").as_dark()</code></pre>
-         </div>
-         <div class="ml-3" id="4085a399-b692-4378-8739-3d383efea4c9">
-          <div id="886ff77e-74f9-45bc-a08b-c3fb07a63704">
-           <i class="fas fa-folder" id="fd695ed0-866b-4086-a835-be645af38e43">
+Panel(
+    Icon("fas fa-folder"),
+    Icon("fas fa-folder").as_primary(),
+    Icon("fas fa-folder").as_secondary(),
+    Icon("fas fa-folder").as_success(),
+    Icon("fas fa-folder").as_warning(),
+    Icon("fas fa-folder").as_danger(),
+    Icon("fas fa-folder").as_info(),
+    Icon("fas fa-folder").as_light(),
+    Icon("fas fa-folder").as_dark()
+)
+</code></pre>
+         </div>
+         <div class="ml-3" id="0629de27-f49e-4e70-8783-fedfd4fe90f4">
+          <div id="cb11e656-ff88-453e-8bf0-e6cbfcca90cd">
+           <i class="fas fa-folder" id="67e9d770-02ed-48db-961a-2e1cf77a5053">
            </i>
-           <i class="fas fa-folder text-primary" id="5c6a9b26-6ead-43ef-8055-00c833c425ce">
+           <i class="fas fa-folder text-primary" id="d3ca1224-d4da-4ed4-9f3a-786548f0d16c">
            </i>
-           <i class="fas fa-folder text-secondary" id="c8af8cf6-fe86-497a-9a7f-e1d5e9393d19">
+           <i class="fas fa-folder text-secondary" id="945215e0-aab9-41c4-bdb1-616711f2900b">
            </i>
-           <i class="fas fa-folder text-success" id="8dd83d46-b08d-4bef-a1d7-4a294f8e3e55">
+           <i class="fas fa-folder text-success" id="c49cacc3-b30a-4bf9-b871-159e008919bd">
            </i>
-           <i class="fas fa-folder text-warning" id="dcf06660-ac21-4249-984a-61e53bc5049a">
+           <i class="fas fa-folder text-warning" id="cc099e1a-af57-451b-a2b8-ffea623dca1e">
            </i>
-           <i class="fas fa-folder text-danger" id="d20dd90e-57bb-4bb0-a65a-c3a7e373799f">
+           <i class="fas fa-folder text-danger" id="b4bba540-e1c5-465f-8fb8-1b3b1d244c3f">
            </i>
-           <i class="fas fa-folder text-info" id="b0a2bc68-30b9-465e-bf81-8be96f3a5c36">
+           <i class="fas fa-folder text-info" id="0e7b0390-3f2f-476f-87c9-755181f9af30">
            </i>
-           <i class="fas fa-folder text-light" id="85356271-c994-498e-9f43-d9b0c4dd4d07">
+           <i class="fas fa-folder text-light" id="9e50503b-9d55-4211-8880-2bcdc99f001d">
            </i>
-           <i class="fas fa-folder text-dark" id="7e3323d0-bdaf-4dfe-a0d6-bf041f29bbdc">
+           <i class="fas fa-folder text-dark" id="803f25fd-483e-46fd-a86a-c44e3311545e">
            </i>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="27176909-960c-479a-b89b-a4a6d18d7f05">
-        <div class="mt-5" id="1d1aa9cc-9e9d-4784-8ede-ccc4a615102d">
-         <div class="d-flex justify-content-between" id="d7237cda-d5ef-44c1-a9e0-3674321c58a1">
-          <h1 id="fe58ca69-c3fa-400a-9f41-36b6dcb23210">
+       <div class="tab-pane fade" id="7ab63f00-dd8e-4673-80f0-30471aff2f3d">
+        <div class="mt-5" id="de712359-a4bb-44e6-bdb0-6f60d8adb5a9">
+         <div class="d-flex justify-content-between" id="a6044197-fe6f-4102-987c-2b7a01f9c225">
+          <h1 id="ac2b5a8f-5038-4954-b511-a268e5c942ff">
            Class
-           <span class="text-primary" id="15009ed6-be4a-4b67-9741-27f6307038e1">
+           <span class="text-primary" id="9e24ab5b-65e9-4106-8aa4-b6ae27b282ca">
             Spinner
            </span>
           </h1>
-          <div id="f1b9af10-c087-4eda-9ce9-901dc75379d9">
+          <div id="9695d5ca-7f91-4724-9221-1bddc68c55d2">
           </div>
          </div>
-         <span class="text-muted" id="20955e98-54fc-4a8d-97dd-8302245fdd12">
+         <span class="text-muted" id="6ffa30cb-91ae-4038-83fa-8264c870b4c3">
           A spinner icon.
          </span>
-         <pre id="f0de940c-cf35-4086-b3bb-04a4c8a8ad42"><code class="python">Spinner()</code></pre>
-         <div class="ml-3" id="30873ed5-a502-4ed2-9508-77b5c16747fe">
-          <h6 id="8461f142-486d-449a-b3a1-15926f65448d">
+         <pre id="c3a7f20b-a9da-44c5-a47d-0973a583277f"><code class="python">Spinner()</code></pre>
+         <div class="ml-3" id="e00701f4-f9ed-4a72-9d15-97b68dd09aee">
+          <h6 id="ca62e937-27cb-41c2-b13f-c820ac68c4c3">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="11009599-8a23-4aeb-bb2d-199b579883a5"><code class="python">from bootwrap import Spinner
+          <pre id="31a10082-c62c-43c3-940f-99ab7be8c18a"><code class="python">from bootwrap import Spinner, Panel
 
-Spinner()
-Spinner().as_primary()
-Spinner().as_secondary()
-Spinner().as_success()
-Spinner().as_warning()
-Spinner().as_danger()
-Spinner().as_info()
-Spinner().as_light()
-Spinner().as_dark()</code></pre>
-         </div>
-         <div class="ml-3" id="68b92249-55d8-4965-8049-4ab30855be46">
-          <div id="151c9434-a1a3-417f-9c0c-2b65840f4392">
-           <span class="spinner" id="8cb9eb8d-97e9-44ec-8724-2d70b1c2ceff">
+Panel(
+    Spinner(),
+    Spinner().as_primary(),
+    Spinner().as_secondary(),
+    Spinner().as_success(),
+    Spinner().as_warning(),
+    Spinner().as_danger(),
+    Spinner().as_info(),
+    Spinner().as_light(),
+    Spinner().as_dark()
+)
+</code></pre>
+         </div>
+         <div class="ml-3" id="1072ff3b-979c-4e18-9293-c5430e0005cc">
+          <div id="ad20d6e8-f317-4587-b59b-954720d1c1e4">
+           <span class="spinner" id="52bfac52-5208-4e72-beb9-f4b1af80c1b7">
            </span>
            <style>
             @keyframes spinner-border {
                     to { transform: rotate(360deg); }
                 }
 
                 .spinner{
@@ -4256,15 +4334,15 @@
                     border: .15em solid currentColor;
                     border-right-color: transparent;
                     border-radius: 50%;
                     -webkit-animation: spinner-border .75s linear infinite;
                     animation: spinner-border .75s linear infinite;
                 }
            </style>
-           <span class="spinner text-primary" id="d43eea84-c7fd-4590-b673-7c906313ce09">
+           <span class="spinner text-primary" id="c2206fcf-552f-4ef7-9a92-2f5243f69ee7">
            </span>
            <style>
             @keyframes spinner-border {
                     to { transform: rotate(360deg); }
                 }
 
                 .spinner{
@@ -4275,15 +4353,15 @@
                     border: .15em solid currentColor;
                     border-right-color: transparent;
                     border-radius: 50%;
                     -webkit-animation: spinner-border .75s linear infinite;
                     animation: spinner-border .75s linear infinite;
                 }
            </style>
-           <span class="spinner text-secondary" id="85dbce33-aebe-452b-bff0-f125f342ffb7">
+           <span class="spinner text-secondary" id="4176c399-29b8-445a-9317-0c3de685ea0a">
            </span>
            <style>
             @keyframes spinner-border {
                     to { transform: rotate(360deg); }
                 }
 
                 .spinner{
@@ -4294,15 +4372,15 @@
                     border: .15em solid currentColor;
                     border-right-color: transparent;
                     border-radius: 50%;
                     -webkit-animation: spinner-border .75s linear infinite;
                     animation: spinner-border .75s linear infinite;
                 }
            </style>
-           <span class="spinner text-success" id="a9011dc0-07e7-4fc3-b438-dced18089e27">
+           <span class="spinner text-success" id="9ee44f17-b10e-48ec-8c42-3153a218e2b1">
            </span>
            <style>
             @keyframes spinner-border {
                     to { transform: rotate(360deg); }
                 }
 
                 .spinner{
@@ -4313,15 +4391,15 @@
                     border: .15em solid currentColor;
                     border-right-color: transparent;
                     border-radius: 50%;
                     -webkit-animation: spinner-border .75s linear infinite;
                     animation: spinner-border .75s linear infinite;
                 }
            </style>
-           <span class="spinner text-warning" id="2ce97cb5-1d8b-4dd0-94b3-1bc3e5ae8fd2">
+           <span class="spinner text-warning" id="6492dc89-a776-4e7c-804a-70fca1d69a5c">
            </span>
            <style>
             @keyframes spinner-border {
                     to { transform: rotate(360deg); }
                 }
 
                 .spinner{
@@ -4332,15 +4410,15 @@
                     border: .15em solid currentColor;
                     border-right-color: transparent;
                     border-radius: 50%;
                     -webkit-animation: spinner-border .75s linear infinite;
                     animation: spinner-border .75s linear infinite;
                 }
            </style>
-           <span class="spinner text-danger" id="b16540de-87f0-4e10-8031-1026604129a1">
+           <span class="spinner text-danger" id="21aa0fe1-1779-4b63-a74c-2a5f420b6e2a">
            </span>
            <style>
             @keyframes spinner-border {
                     to { transform: rotate(360deg); }
                 }
 
                 .spinner{
@@ -4351,15 +4429,15 @@
                     border: .15em solid currentColor;
                     border-right-color: transparent;
                     border-radius: 50%;
                     -webkit-animation: spinner-border .75s linear infinite;
                     animation: spinner-border .75s linear infinite;
                 }
            </style>
-           <span class="spinner text-info" id="882bfdc4-38a9-4bbd-a4f4-0cffc770ecdc">
+           <span class="spinner text-info" id="bc8b120b-49a9-4a70-aa4e-6edbff916b82">
            </span>
            <style>
             @keyframes spinner-border {
                     to { transform: rotate(360deg); }
                 }
 
                 .spinner{
@@ -4370,15 +4448,15 @@
                     border: .15em solid currentColor;
                     border-right-color: transparent;
                     border-radius: 50%;
                     -webkit-animation: spinner-border .75s linear infinite;
                     animation: spinner-border .75s linear infinite;
                 }
            </style>
-           <span class="spinner text-light" id="ae322c9a-f98e-42d3-867e-5bc22b8ae756">
+           <span class="spinner text-light" id="6677171a-431e-459c-88e2-18a501fff0a3">
            </span>
            <style>
             @keyframes spinner-border {
                     to { transform: rotate(360deg); }
                 }
 
                 .spinner{
@@ -4389,15 +4467,15 @@
                     border: .15em solid currentColor;
                     border-right-color: transparent;
                     border-radius: 50%;
                     -webkit-animation: spinner-border .75s linear infinite;
                     animation: spinner-border .75s linear infinite;
                 }
            </style>
-           <span class="spinner text-dark" id="a66cc7dd-7a54-4eea-a5a7-fe850e5fb376">
+           <span class="spinner text-dark" id="861a5d4f-f1de-4599-9919-8cb3ec77282d">
            </span>
            <style>
             @keyframes spinner-border {
                     to { transform: rotate(360deg); }
                 }
 
                 .spinner{
@@ -4415,40 +4493,40 @@
           </div>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="b352e040-ea7d-49e4-bb59-511ba97910dc">
-     <div class="mt-5" id="2f7011fc-6ff1-4588-b7a6-2d886f0347e0">
-      <div class="d-flex justify-content-between" id="95f72de6-cbd7-4201-b606-de0442f6af4e">
-       <h1 id="13341ec2-435b-4057-a87d-57819ae2ff5d">
+    <div class="tab-pane fade" id="5a85ba07-f6ac-42e5-a6e7-472caf5cd771">
+     <div class="mt-5" id="010240f3-b0b2-4aba-a0aa-2f5edb383356">
+      <div class="d-flex justify-content-between" id="97a08f0c-cee9-481e-a8ef-aee49335e8e1">
+       <h1 id="f3d9fded-0a5d-47ab-936e-56d7d7511c57">
         Class
-        <span class="text-primary" id="e8fcb3bc-2e54-4948-9706-396638324902">
+        <span class="text-primary" id="5d1e0aad-d94a-41c3-bd6f-c0544ca42039">
          Image
         </span>
        </h1>
-       <div id="99f5c03f-d42b-4745-83dc-b98a767d5440">
-        <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#8b5b6ff7-0549-4ec5-bbdb-69872da49ad4" data-toggle="collapse" id="b27dba38-cf1c-49d1-9ced-9b9ca4e82471" onclick="return false;" type="button">
+       <div id="6362c8d8-17d8-44b3-860b-f573283f2a82">
+        <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#c3e84a2a-1fc1-47ab-8814-2b8c417cecbb" data-toggle="collapse" id="ec83f7e7-23f6-41d5-87e5-d1ff8868c3b6" onclick="return false;" type="button">
          Argument
         </button>
        </div>
       </div>
-      <span class="text-muted" id="59b1d51a-f637-4d8a-886f-14c184d452a6">
+      <span class="text-muted" id="f33611fb-f451-4735-8bb4-b732fbd77eba">
        A web component for an image.
       </span>
-      <pre id="df2ef881-a2ba-4f95-be7d-1802921838d4"><code class="python">Image(src, width=None, height=None, alt=None)</code></pre>
-      <div class="ml-3 collapse" id="8b5b6ff7-0549-4ec5-bbdb-69872da49ad4">
-       <h6 id="1c7d1dff-b883-46aa-9dd9-c0a5e08b307a">
+      <pre id="7359ede9-22ac-4c0c-842c-51f30d2f00e4"><code class="python">Image(src, width=None, height=None, alt=None)</code></pre>
+      <div class="ml-3 collapse" id="c3e84a2a-1fc1-47ab-8814-2b8c417cecbb">
+       <h6 id="63a9ca0f-ae76-460e-a15c-1152e456658e">
         <strong>
          Arguments
         </strong>
        </h6>
-       <table class="table table-sm bg-light" id="3478446a-c217-4b60-adfb-efb0758581d3">
+       <table class="table table-sm bg-light" id="6fe58726-3bf5-473d-b253-6d6476a2d90a">
         <thead>
          <tr>
           <th scope="col">
            Name
           </th>
           <th scope="col">
            Type
@@ -4518,75 +4596,76 @@
           <td>
            The alt text.
           </td>
          </tr>
         </tbody>
        </table>
       </div>
-      <div class="ml-3" id="96ef1082-e3c5-4415-9553-ef47701bffd1">
-       <h6 id="05900cc0-2082-40cd-89af-1128c18f5cc7">
+      <div class="ml-3" id="ee149a0d-65af-4d55-b21a-87e1ed3e68c4">
+       <h6 id="27b1c97c-06d4-42d7-9e65-25aba07097bd">
         <strong>
          Example
         </strong>
        </h6>
-       <pre id="5f5c3bf4-9d23-494a-98ca-4feeda450c91"><code class="python">from bootwrap import Image
+       <pre id="97c0634c-209c-4618-9b58-b01b9e7bd6cf"><code class="python">from bootwrap import Image
 
-Image("logo.png", width=64, height=64, alt="Bootwarp Logo")</code></pre>
+Image("logo.png")
+</code></pre>
       </div>
-      <div class="ml-3" id="f3aa207a-7435-4446-bce9-beabcd012e28">
-       <img id="06694a21-0ba4-4b80-a8d2-60d45ccbe25d" src="logo.png"/>
+      <div class="ml-3" id="28e86544-1111-49ba-8aed-1cfa6c16947f">
+       <img id="17bec690-4cf1-4136-bb5e-9ab2e29ccd98" src="logo.png"/>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="cd637315-f984-4528-a9e2-3a5a1c7d0f82">
-     <div id="55539229-9f86-4484-b17a-fa4d85431891">
+    <div class="tab-pane fade" id="f70d9d6c-0f05-4f07-a4ca-2a50856faa9b">
+     <div id="3c2524cb-e2f6-4ada-b927-6c3647f750c6">
       <hr/>
-      <ul class="nav" id="6a546da6-97ba-4ff0-9288-e791987407c6" role="tablist">
+      <ul class="nav" id="a75cbc04-9e0d-4b58-9e19-fd7f689a5818" role="tablist">
        <li class="nav-item">
-        <a class="nav-link active" data-target="#ba1413f5-db0c-4d50-bf39-212ea3ce9eec" data-toggle="tab" href="#ba1413f5-db0c-4d50-bf39-212ea3ce9eec" id="3eec3321-b3f5-4f1e-b6d3-4e2471a03386" role="tab">
-         <span class="text-secondary" id="bd0db0fe-a378-4926-a083-33bda31217be">
+        <a class="nav-link active" data-target="#eb836698-aaed-4918-a565-e884e9b6a87c" data-toggle="tab" href="#eb836698-aaed-4918-a565-e884e9b6a87c" id="23955b3c-960d-4324-98bd-5e1f1c5e8075" role="tab">
+         <span class="text-secondary" id="02a8a6b7-d701-48da-a05a-dc25ba043a3e">
           Javascript
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#a720be62-ed0d-4e63-a9b6-65e04292f6d8" data-toggle="tab" href="#a720be62-ed0d-4e63-a9b6-65e04292f6d8" id="058a6b2a-3253-4807-8a91-88716ddc2c85" role="tab">
-         <span class="text-secondary" id="8ba57488-51fb-4e89-9fdf-4070e95a0ad7">
+        <a class="nav-link" data-target="#c6e93ebc-8f9e-44e4-b81e-7feea2351143" data-toggle="tab" href="#c6e93ebc-8f9e-44e4-b81e-7feea2351143" id="980c7a60-f628-4ebc-a45b-a5452761b29c" role="tab">
+         <span class="text-secondary" id="ddbdb802-1b41-49fc-ab17-67f347b3e202">
           jQuery
          </span>
         </a>
        </li>
       </ul>
       <div class="tab-content">
-       <div class="tab-pane fade active show" id="ba1413f5-db0c-4d50-bf39-212ea3ce9eec">
-        <div class="mt-5" id="a5fdb0e2-41f1-4ec7-91b6-1482c9c5b768">
-         <div class="d-flex justify-content-between" id="2cf9d59b-3cf4-4fa0-a0c5-0eb270995930">
-          <h1 id="3a3dc25e-9a7f-4493-92bc-188477c738ff">
+       <div class="tab-pane fade active show" id="eb836698-aaed-4918-a565-e884e9b6a87c">
+        <div class="mt-5" id="15b57149-688c-4444-9d1a-c76626ef29fb">
+         <div class="d-flex justify-content-between" id="11a88695-bf05-4ba5-a63e-c4df1ee24f4d">
+          <h1 id="87db6efe-1704-405f-9c20-f1f2c21f03a4">
            Class
-           <span class="text-primary" id="705a9e1c-308d-43f9-bca8-bb5419012045">
+           <span class="text-primary" id="6f78772b-0414-4a38-bf4d-1e864dfaf319">
             Javascript
            </span>
           </h1>
-          <div id="256dee40-e6e1-4298-9657-87671c69de20">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#a3d59c2e-1398-4428-b8a4-28bfd0573d8c" data-toggle="collapse" id="899300e1-6124-48ea-bc3b-b1a0195bc102" onclick="return false;" type="button">
+          <div id="8ffd72e9-334f-47d7-a6ac-8e8978e7f890">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#f845c815-bf9e-467c-9316-bf3b3a4f7e1c" data-toggle="collapse" id="bdf770e3-2f62-4f75-a614-91e0d4ed6069" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="cd3b23eb-bfce-421f-8f61-46d5fc478016">
+         <span class="text-muted" id="bddd3073-707a-4af4-a145-a03e015bdb41">
           A web component for a javascript.
          </span>
-         <pre id="6a62868a-9475-4430-b433-a427da455777"><code class="python">Javascript(src=None, script=None, submap=None)</code></pre>
-         <div class="ml-3 collapse" id="a3d59c2e-1398-4428-b8a4-28bfd0573d8c">
-          <h6 id="32a6d223-e0e2-4ddc-a1db-45c6b8fff621">
+         <pre id="97a2aeac-703e-4d67-a8de-76d336181bdc"><code class="python">Javascript(src=None, script=None, submap=None)</code></pre>
+         <div class="ml-3 collapse" id="f845c815-bf9e-467c-9316-bf3b3a4f7e1c">
+          <h6 id="30cfd6ad-7670-4488-a1f1-d2171e157574">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="f9ff3ef9-85f1-4daf-acaf-754732f52af2">
+          <table class="table table-sm bg-light" id="9f8a52ee-843e-4e82-8243-f22c80b86d49">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -4643,149 +4722,149 @@
               The map with substitutions, binding the javascript
             with Python objects.
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <div class="ml-3" id="710b1ef8-6e43-45dc-8ae6-b52179e6abcb">
-          <h6 id="308d2ffa-e9ee-4c51-b50e-eaf0b16c550e">
+         <div class="ml-3" id="fa8b4165-6e2c-4ff8-a99d-ae0ce270a925">
+          <h6 id="2ccf3bc5-d01d-468f-afb7-79c1953ee0b8">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="5a4f9ef3-33e5-4797-a342-2e538a804b83"><code class="python">from bootwrap import Page, Javascript
+          <pre id="2329408d-1f89-4e42-9cf5-eaf1ec89d91a"><code class="python">from bootwrap import Page, Javascript
 
 my_page = Page(
     ...
     resources = [
         Javascript("https://ajax...0/jquery.min.js")
     ]
     ...
-)</code></pre>
+)
+</code></pre>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="a720be62-ed0d-4e63-a9b6-65e04292f6d8">
-        <div class="mt-3" id="ce80c145-aa2e-4bb6-823a-3a68fde7fde7">
-         <div id="ce687c27-91c4-4325-a8ec-0d4be76e92f3">
+       <div class="tab-pane fade" id="c6e93ebc-8f9e-44e4-b81e-7feea2351143">
+        <div class="mt-3" id="577011c0-707a-4830-ac15-fb691621993e">
+         <div id="cfc99523-7c4c-4612-b5d4-164c484b709f">
           <div class="row">
            <div class="col-md">
-            <div id="6195d64d-3b56-420a-8c51-265d369b7b27">
-             <h1 id="3d01e68c-34fc-464b-9de8-3be8d0ab2af9">
+            <div id="7c431e67-bd42-456d-8e09-99ca8093fa57">
+             <h1 id="86633590-76fe-47e0-8990-be4e0eaa84be">
               jQuery
              </h1>
             </div>
            </div>
            <div class="col-md">
-            <div id="f6d7de7c-087c-48eb-91e4-a4c9ae20aef7">
+            <div id="3152d9c6-2bd6-4434-98d0-1833bab6d3ed">
             </div>
            </div>
           </div>
          </div>
-         <div id="aeb9ff2e-4bdd-4a43-a765-d9a952ea2cf5">
+         <div id="fb27174b-e50d-4aa9-a15a-18216a4eda5a">
           <div class="row">
            <div class="col-md">
-            <div id="e3107eb8-9a6a-4f7a-8d67-151ae1341b7b">
-             <p id="c568e689-5081-4eb3-8e88-f49c5d0f7158">
+            <div id="c68e0f1f-6094-4a89-90f6-08ef09bed3ca">
+             <p id="7d93c10b-b463-4856-8cbb-16fc9f88a33e">
               Use
               <code>
                Javascript
               </code>
               for creating interactive web content with the help of jQuery.
              </p>
             </div>
            </div>
            <div class="col-md">
-            <div id="6d90f28a-5348-4a0b-93b2-3835d7d05ce8">
-             <pre id="9a9d9e2f-35c2-49bb-b368-fc79a27d37c6"><code class="python">from bootwrap import Javascript, Button, Text
+            <div id="95c1480b-8442-4c6f-881e-1244f6707f11">
+             <pre id="1ac254fd-24aa-482a-b308-a6e8acba875c"><code class="python">from bootwrap import Panel, Javascript, Button, Text
 
 label = Text("Answer:").as_strong()
 answer = Text("unknown").mr(2).ml(2)
 btn_yes = Button("Yes").as_success()
 btn_no = Button("No").as_danger()
 
 action = Javascript(
   script='''
     $("#btn_yes").on("click",function(){
       $("#answer").text("Yes");
     });
     $("#btn_no").on("click",function(){
       $("#answer").text("No");
     });
-  '''
+  ''',
   submap={
     "answer": answer,
     "btn_yes": btn_yes,
     "btn_no": btn_no
   }
 )
-
 Panel(
   label, answer, btn_yes, btn_no, action
 )</code></pre>
-             <div id="57108275-1fe7-4452-a393-a51394af867a">
-              <span id="0c519912-86af-4936-b9b1-3ce16f3c3590">
+             <div id="392f8a1a-061a-4b96-9087-c0665a2b5e03">
+              <span id="055f95de-1103-471e-b904-01873e6568a1">
                <strong>
                 Answer:
                </strong>
               </span>
-              <span class="mr-2 ml-2" id="7e467084-57f8-4ca2-ad4c-5585340d899d">
+              <span class="mr-2 ml-2" id="dc5ebec8-28eb-4b25-ad29-46737533f735">
                unknown
               </span>
-              <button class="btn btn-success" id="ff2ae2d1-b125-4140-a577-73129fb5a86f" onclick="return false;">
+              <button class="btn btn-success" id="fc31edb5-c259-440b-b9af-c6fe80c91e68" onclick="return false;">
                Yes
               </button>
-              <button class="btn btn-danger" id="6bfef9da-971e-4529-b991-c7849041d59a" onclick="return false;">
+              <button class="btn btn-danger" id="01af4821-ca33-4ff4-80bc-02c5357550da" onclick="return false;">
                No
               </button>
               <script type="application/javascript">
-               $("#ff2ae2d1-b125-4140-a577-73129fb5a86f").on("click",function(){
-      $("#7e467084-57f8-4ca2-ad4c-5585340d899d").text("Yes");
+               $("#fc31edb5-c259-440b-b9af-c6fe80c91e68").on("click",function(){
+      $("#dc5ebec8-28eb-4b25-ad29-46737533f735").text("Yes");
     });
-    $("#6bfef9da-971e-4529-b991-c7849041d59a").on("click",function(){
-      $("#7e467084-57f8-4ca2-ad4c-5585340d899d").text("No");
+    $("#01af4821-ca33-4ff4-80bc-02c5357550da").on("click",function(){
+      $("#dc5ebec8-28eb-4b25-ad29-46737533f735").text("No");
     });
               </script>
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="b7b7831a-01df-4d41-b689-dc81d94581b5">
-     <div class="mt-5" id="f31d41fe-b8ad-4b09-9f3a-45772828be04">
-      <div class="d-flex justify-content-between" id="ce835a07-6d46-4fed-9e71-623dfd5a5c59">
-       <h1 id="e8013f5a-c96e-4f09-a93b-7c2a49e1cc54">
+    <div class="tab-pane fade" id="124666c1-23fd-47c4-bf7c-e3a88ef242d3">
+     <div class="mt-5" id="acdbc6aa-81d4-4114-81b2-dde028961259">
+      <div class="d-flex justify-content-between" id="08c9d0db-e424-4e52-96a1-0cce1b6f628a">
+       <h1 id="ee3ab8e8-c67f-4b5d-a90d-dd5e1e6c0988">
         Class
-        <span class="text-primary" id="909c9715-7009-450f-b64f-3ccc8d35910f">
+        <span class="text-primary" id="06f27d30-be1f-4790-839a-311f0a36163a">
          Link
         </span>
        </h1>
-       <div id="83b9e6f5-83c5-41f1-8539-b9cd06611776">
-        <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#9e895fef-aeb4-4455-b9df-c39b1b59950a" data-toggle="collapse" id="15a9700f-26bb-4ff2-8cc8-999bc686c01c" onclick="return false;" type="button">
+       <div id="5e9da25f-af17-4cd9-9fee-caebac855c6f">
+        <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#15c19ea4-a6f2-4329-9cea-5a0002cbae89" data-toggle="collapse" id="4fecf294-7266-4eaf-9a07-fffdbecf032d" onclick="return false;" type="button">
          Argument
         </button>
        </div>
       </div>
-      <span class="text-muted" id="c069aab7-640a-4b1e-b5e5-ba2b21558d2e">
+      <span class="text-muted" id="7c43e0d3-9999-409e-9e98-8effb3465e12">
        A web component for an external resource link.
       </span>
-      <pre id="79f15031-00ac-4c1b-b234-298b409d5f26"><code class="python">Link(href, rel='stylesheet', ctype='text/css')</code></pre>
-      <div class="ml-3 collapse" id="9e895fef-aeb4-4455-b9df-c39b1b59950a">
-       <h6 id="740a3963-e666-49ff-8a51-23ef4a54e90f">
+      <pre id="c04b44e8-2333-4ebb-87dc-becbccea7baa"><code class="python">Link(href, rel='stylesheet', ctype='text/css')</code></pre>
+      <div class="ml-3 collapse" id="15c19ea4-a6f2-4329-9cea-5a0002cbae89">
+       <h6 id="16a4d348-18a2-4115-8ce2-3c9f879e89f8">
         <strong>
          Arguments
         </strong>
        </h6>
-       <table class="table table-sm bg-light" id="31ee43b3-41c8-4b6e-90df-f988854e99a9">
+       <table class="table table-sm bg-light" id="052c331e-70c2-4ff0-81b6-e0db919f4cd1">
         <thead>
          <tr>
           <th scope="col">
            Name
           </th>
           <th scope="col">
            Type
@@ -4843,82 +4922,83 @@
            This attribute is used to define the type of the content
             linked to (from MDN WebDoc).
           </td>
          </tr>
         </tbody>
        </table>
       </div>
-      <p id="7991eca7-5ce9-45b5-89f7-f6a5c2cb2f39">
+      <p id="95fe4def-9161-4974-b3b9-2f1af9150d4f">
        See https://developer.mozilla.org/en-US/docs/Web/HTML/Element/link
     for more information.
       </p>
-      <div class="ml-3" id="3163d2e5-8b0c-47f1-806a-474af98d1df6">
-       <h6 id="d0e6c691-95b1-4c37-b97c-b5c0cb21490d">
+      <div class="ml-3" id="ede9cd50-bf3f-4752-a565-509958beb190">
+       <h6 id="f0b78c3f-65e1-4388-a22a-ef0412ab1411">
         <strong>
          Example
         </strong>
        </h6>
-       <pre id="b89d3b99-2148-47d9-a2af-f6b0b2414f0e"><code class="python">from bootwrap import Page, Link
+       <pre id="3073f073-cce1-437f-baa9-285bc16a44e0"><code class="python">from bootwrap import Page, Link
 
 my_page = Page(
     ...
     resources = [
         Link("https://cdnjs.cloudflare.com/.../all.min.css")
     ]
     ...
-)</code></pre>
+)
+</code></pre>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="53f05ef7-9272-4e4e-b02d-ab119d10972f">
-     <div id="383b0d68-a80f-43f7-8222-051462d6a522">
+    <div class="tab-pane fade" id="8e2eb34a-4f9e-4d8b-9754-6dd7a2eb2aea">
+     <div id="463106eb-e704-4967-a879-2805d56c57ea">
       <hr/>
-      <ul class="nav" id="a20d2ae1-46ca-46c4-a1ed-473da22e152d" role="tablist">
+      <ul class="nav" id="0826f497-6007-42ef-9e02-f7004d6f5668" role="tablist">
        <li class="nav-item">
-        <a class="nav-link active" data-target="#d59d1d7b-8ff6-48d6-8e75-0e7e98d19a22" data-toggle="tab" href="#d59d1d7b-8ff6-48d6-8e75-0e7e98d19a22" id="e99fd36b-e985-4fb7-a4a1-4700091933a4" role="tab">
-         <span class="text-secondary" id="d4d3fa15-fde4-4430-bcfa-2d33bdd843cd">
+        <a class="nav-link active" data-target="#286ec72d-abe9-4fe8-ab01-ea180538d6c8" data-toggle="tab" href="#286ec72d-abe9-4fe8-ab01-ea180538d6c8" id="4e62a097-8b99-4b0d-9cee-edba687a1a11" role="tab">
+         <span class="text-secondary" id="19229529-1c3c-4829-a751-0c47d709c6c2">
           List
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#1b781953-2ad8-4ad6-8eec-54b7b8872568" data-toggle="tab" href="#1b781953-2ad8-4ad6-8eec-54b7b8872568" id="21a2fa4a-d3c0-4cb8-b892-c93a00d2dba0" role="tab">
-         <span class="text-secondary" id="c4dec2df-e021-4f4c-aae9-17dc857fd242">
+        <a class="nav-link" data-target="#9a238933-3f99-40a7-aca9-aac5672f8c70" data-toggle="tab" href="#9a238933-3f99-40a7-aca9-aac5672f8c70" id="d70f108e-bfaf-4c7a-beca-9204ed404b1b" role="tab">
+         <span class="text-secondary" id="28f10457-aaef-417b-982e-b7d38592a9c7">
           List.Item
          </span>
         </a>
        </li>
       </ul>
       <div class="tab-content">
-       <div class="tab-pane fade active show" id="d59d1d7b-8ff6-48d6-8e75-0e7e98d19a22">
-        <div class="mt-5" id="a01311dc-d23b-4001-9a20-cb364d50d9b3">
-         <div class="d-flex justify-content-between" id="dbe17a58-1699-4808-9b44-398d992e091a">
-          <h1 id="6542ac51-88ad-40af-880f-caa5112ce60d">
+       <div class="tab-pane fade active show" id="286ec72d-abe9-4fe8-ab01-ea180538d6c8">
+        <div class="mt-5" id="cfb0af29-7825-4015-a9d2-f6e4670216b4">
+         <div class="d-flex justify-content-between" id="620ad3e2-3cf7-4c74-8524-0e1a677d7b1f">
+          <h1 id="871a8d21-2374-4875-9c14-8c14e64bb9a2">
            Class
-           <span class="text-primary" id="335adc42-0dab-4f29-a4e2-731fa3c7d8ee">
+           <span class="text-primary" id="ef1463f8-496e-47d2-bdc8-28465c4630bc">
             List
            </span>
           </h1>
-          <div id="a8b8f91c-2cc6-4dc6-8fd0-4e92cc6ab15d">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#a1816e66-7c2b-4d7a-abc2-5d382ca55635" data-toggle="collapse" id="63199806-32e8-4c39-b20c-3c246c270799" onclick="return false;" type="button">
+          <div id="4e248e8d-9ec3-4af0-aef8-c72b0788e884">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#29ac8712-faeb-4277-9282-cf3314cbc245" data-toggle="collapse" id="fd59c069-60f3-4325-83bb-a9795ed38718" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="e27a7ee8-76ee-43e6-84f0-b90ff5abf244">
+         <span class="text-muted" id="6ff77603-d2d3-4275-b5dc-1cdf7adb1d6e">
           A web component for a list of items.
          </span>
-         <pre id="31633dbc-3f73-4864-aead-ee7e9923498e"><code class="python">List(*items)</code></pre>
-         <div class="ml-3 collapse" id="a1816e66-7c2b-4d7a-abc2-5d382ca55635">
-          <h6 id="4777195f-4433-410a-a776-d55710938e70">
+         <pre id="744bb292-176d-460c-8580-451993c2f758"><code class="python">List(*items)</code></pre>
+         <div class="ml-3 collapse" id="29ac8712-faeb-4277-9282-cf3314cbc245">
+          <h6 id="66c120c9-be91-417d-8dcd-fcaa6fd6be7c">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="829b9f96-a76f-4653-8e98-cc5dd5f1732f">
+          <table class="table table-sm bg-light" id="bf3bdfbd-6bf8-47db-aab2-19e9d9e99bd5">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -4951,24 +5031,24 @@
               </code>
               elements.
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <div class="ml-3" id="ba5321f7-c25c-4e57-8089-7f2ce851d071">
-          <h6 id="ec1e7311-00d9-4172-9273-b45e55d7b92b">
+         <div class="ml-3" id="44f9e0b2-006a-45c2-b1f3-84078c9c1dba">
+          <h6 id="4f3112ae-626a-443a-abaa-acb976a038a3">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="56e83d6a-507a-4f21-844f-3e118684b61a"><code class="python">from bootwrap import Button, List, Image
+          <pre id="32ac53ca-1f50-4eaf-b905-1001b7937ad5"><code class="python">from bootwrap import Button, List, Image
 
 actions = [
-    Button("Buy"),
+    Button("Buy").as_success(),
     Button("Sell"),
     Button("Transfer")
 ]
 
 List(
     List.Item(
         "Google (NASDAQ: GOOGL)",
@@ -4987,153 +5067,154 @@
     List.Item(
         "Amazon (NASDAQ: AMZN)",
         description= "Price for a single Amazon share",
         figure=Image("amazon-logo.png", width=32, height=32),
         marker="12:04:58 12/01/2021"
     ).add_menu(*actions).pack_actions().link(
         "https://www.amazon.com")
-)</code></pre>
+)
+</code></pre>
          </div>
-         <div class="ml-3" id="86996ca4-6ec3-4ddd-9299-54f5c1ddf959">
-          <div class="list-group" id="12d43d40-09c1-48a5-945f-8e3e14622161">
-           <a class="list-group-item list-group-item-action flex-column align-items-start active" href="https://www.google.com" id="16d93dae-4e9f-43ca-a461-cf5d7a5f7966">
+         <div class="ml-3" id="19b914ce-f6d0-40fa-bb8c-c76a2511794e">
+          <div class="list-group" id="6c8d3d66-d21e-4dea-a2fd-d887cf53618d">
+           <a class="list-group-item list-group-item-action flex-column align-items-start active" href="https://www.google.com" id="d3e1e1dc-64e9-4e8b-b40f-31bea0dfaae4">
             <div class="d-flex w-100 justify-content-between">
-             <img height="32" id="4d7a9dff-4303-4b3d-89ef-446503d079b8" src="google-logo.png" width="32"/>
+             <img height="32" id="6f19b491-fe81-4cea-bdaf-b4a99ff88460" src="google-logo.png" width="32"/>
              <div class="ml-2 mr-2 w-100">
               <div class="d-flex w-100 justify-content-between">
-               <h5 id="4fa81bd9-2992-495f-a024-924efc9e0e43">
+               <h5 id="e017e69a-df10-46b1-a1ae-5796f0b16ae0">
                 Google (NASDAQ: GOOGL)
                </h5>
-               <span id="a142c783-6789-4e1a-bbcd-4476163f5614">
+               <span id="46e15c4a-dd90-4838-9f8f-449817a656ed">
                 <small>
                  12:04:58 12/01/2021
                 </small>
                </span>
               </div>
               Price for a single Google share
              </div>
              <div class="d-flex align-items-start">
               <div class="btn-group">
-               <i class="btn fas fa-ellipsis-v" data-toggle="dropdown" id="83b0142e-b677-40f5-8544-a93ee278cf2c" onclick="return false;" style="cursor: pointer">
+               <i class="btn fas fa-ellipsis-v" data-toggle="dropdown" id="90efb7e3-0ed9-441b-8c6d-fb61ad7b06d2" onclick="return false;" style="cursor: pointer">
                </i>
                <div class="dropdown-menu dropdown-menu-right">
-                <button class="dropdown-item btn btn-success" id="d5cbff73-1934-4ede-aaa6-36727d676609" onclick="return false;">
+                <button class="dropdown-item btn btn-success" id="0cdf3f5d-5d71-42f9-96c4-8e0dc6f6eb02" onclick="return false;">
                  Buy
                 </button>
-                <button class="dropdown-item btn" id="02ff6a29-b463-46b0-b21e-4013fa9d9420" onclick="return false;">
+                <button class="dropdown-item btn" id="f8216cd7-ca4a-4e6a-bac8-e395344d9f47" onclick="return false;">
                  Sell
                 </button>
-                <button class="dropdown-item btn" id="cc221d7f-8e09-4a75-90a7-20c514854c20" onclick="return false;">
+                <button class="dropdown-item btn" id="f90ed4a8-5313-47a0-b639-1e26bbfc4b13" onclick="return false;">
                  Transfer
                 </button>
                </div>
               </div>
              </div>
             </div>
            </a>
-           <a class="list-group-item list-group-item-action flex-column align-items-start" href="https://www.linkedin.com" id="9b7584b6-c20f-4c2c-928a-ffbd5a377035">
+           <a class="list-group-item list-group-item-action flex-column align-items-start" href="https://www.linkedin.com" id="7180a95e-50b1-40ed-a408-f6ce0428fc8b">
             <div class="d-flex w-100 justify-content-between">
-             <img height="32" id="5c0f5320-3d74-42f0-b941-4ee8f83cf91f" src="linkedin-logo.png" width="32"/>
+             <img height="32" id="4d953565-a636-445e-bbf0-53803f5ba835" src="linkedin-logo.png" width="32"/>
              <div class="ml-2 mr-2 w-100">
               <div class="d-flex w-100 justify-content-between">
-               <h5 id="d6b56f1b-fc41-40d9-a08c-6bdcecb24adc">
+               <h5 id="a31f6267-9ffb-4385-b987-7adfb2d286e6">
                 LinkedIn (NASDAQ: LNKD)
                </h5>
-               <span id="01e0ffe7-a9d1-47ef-b85e-2e33dc04ca98">
+               <span id="e60ab82a-403f-478e-9cbc-9b90649e11ac">
                 <small>
                  12:04:58 12/01/2021
                 </small>
                </span>
               </div>
               Price for a single LinkedIn share
              </div>
              <div class="d-flex align-items-start">
               <div class="btn-group">
-               <i class="btn fas fa-ellipsis-v" data-toggle="dropdown" id="9fe32691-ac40-486c-abc3-b71b40616d9f" onclick="return false;" style="cursor: pointer">
+               <i class="btn fas fa-ellipsis-v" data-toggle="dropdown" id="8ee34676-04f0-4e26-a3b6-d32172b6a519" onclick="return false;" style="cursor: pointer">
                </i>
                <div class="dropdown-menu dropdown-menu-right">
-                <button class="dropdown-item btn btn-success" id="d5cbff73-1934-4ede-aaa6-36727d676609" onclick="return false;">
+                <button class="dropdown-item btn btn-success" id="0cdf3f5d-5d71-42f9-96c4-8e0dc6f6eb02" onclick="return false;">
                  Buy
                 </button>
-                <button class="dropdown-item btn" id="02ff6a29-b463-46b0-b21e-4013fa9d9420" onclick="return false;">
+                <button class="dropdown-item btn" id="f8216cd7-ca4a-4e6a-bac8-e395344d9f47" onclick="return false;">
                  Sell
                 </button>
-                <button class="dropdown-item btn" id="cc221d7f-8e09-4a75-90a7-20c514854c20" onclick="return false;">
+                <button class="dropdown-item btn" id="f90ed4a8-5313-47a0-b639-1e26bbfc4b13" onclick="return false;">
                  Transfer
                 </button>
                </div>
               </div>
              </div>
             </div>
            </a>
-           <a class="list-group-item list-group-item-action flex-column align-items-start" href="https://www.amazon.com" id="810c3be3-de94-4c99-816c-bc8ab83622bb">
+           <a class="list-group-item list-group-item-action flex-column align-items-start" href="https://www.amazon.com" id="ea274ded-abe7-41ff-98c8-29d957c6ceaa">
             <div class="d-flex w-100 justify-content-between">
-             <img height="32" id="6be986f2-c452-487d-a539-f8aa0399dede" src="amazon-logo.png" width="32"/>
+             <img height="32" id="eb09d6ab-d2b3-49c9-8e78-592a7a80d29e" src="amazon-logo.png" width="32"/>
              <div class="ml-2 mr-2 w-100">
               <div class="d-flex w-100 justify-content-between">
-               <h5 id="47715ed8-51c2-4dfc-9110-c741d10245a4">
+               <h5 id="c618ea04-5a09-4a0c-aec4-ee120c3e79d8">
                 Amazon (NASDAQ: AMZN)
                </h5>
-               <span id="da5140aa-c401-4b73-8fbb-97f315bd0c3d">
+               <span id="0fe90b7c-1c89-45f6-bda1-0339c00134bf">
                 <small>
                  12:04:58 12/01/2021
                 </small>
                </span>
               </div>
               Price for a single Amazon share
              </div>
              <div class="d-flex align-items-start">
               <div class="btn-group">
-               <i class="btn fas fa-ellipsis-v" data-toggle="dropdown" id="5b3fd6d1-4b73-47ea-a9e2-5b5713e09505" onclick="return false;" style="cursor: pointer">
+               <i class="btn fas fa-ellipsis-v" data-toggle="dropdown" id="c4baeb23-87e5-4bbc-acf3-6cf373809c42" onclick="return false;" style="cursor: pointer">
                </i>
                <div class="dropdown-menu dropdown-menu-right">
-                <button class="dropdown-item btn btn-success" id="d5cbff73-1934-4ede-aaa6-36727d676609" onclick="return false;">
+                <button class="dropdown-item btn btn-success" id="0cdf3f5d-5d71-42f9-96c4-8e0dc6f6eb02" onclick="return false;">
                  Buy
                 </button>
-                <button class="dropdown-item btn" id="02ff6a29-b463-46b0-b21e-4013fa9d9420" onclick="return false;">
+                <button class="dropdown-item btn" id="f8216cd7-ca4a-4e6a-bac8-e395344d9f47" onclick="return false;">
                  Sell
                 </button>
-                <button class="dropdown-item btn" id="cc221d7f-8e09-4a75-90a7-20c514854c20" onclick="return false;">
+                <button class="dropdown-item btn" id="f90ed4a8-5313-47a0-b639-1e26bbfc4b13" onclick="return false;">
                  Transfer
                 </button>
                </div>
               </div>
              </div>
             </div>
            </a>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="1b781953-2ad8-4ad6-8eec-54b7b8872568">
-        <div class="mt-5" id="00abfdf4-eb2f-46a4-8bb7-e06bed8562b8">
-         <div class="d-flex justify-content-between" id="28d63ca8-18d2-4e3d-b442-ab338e2f66ef">
-          <h1 id="4d588632-51f7-480a-85da-4124efabbad9">
+       <div class="tab-pane fade" id="9a238933-3f99-40a7-aca9-aac5672f8c70">
+        <div class="mt-5" id="da3cde81-a96c-4597-90f7-47e898d3dae3">
+         <div class="d-flex justify-content-between" id="ee9c226f-68ab-44f9-8a45-bfc890365cf5">
+          <h1 id="0548c486-0d04-4f64-89e2-63d65192d189">
            Class
-           <span class="text-primary" id="c1523b37-c49a-4012-bc05-8264c61fa726">
+           <span class="text-primary" id="8bc1f27a-1744-442e-ab21-4d67040535a8">
             List.Item
            </span>
           </h1>
-          <div id="4176c5e1-021d-48a5-8015-67c6005dafb4">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#f671c8cb-a05d-4701-a147-4295326816b5" data-toggle="collapse" id="b444822e-1119-4489-9c00-a298d15b66e2" onclick="return false;" type="button">
+          <div id="7edc1e2b-b846-4f53-9fd4-8c2ebc7be643">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#57840089-11ae-45c9-8421-2c9974349510" data-toggle="collapse" id="534af4f3-bc51-4f44-b644-a251a97dd474" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="ad63253b-ebc1-4400-8b92-80242b894869">
+         <span class="text-muted" id="89eaeb3c-d077-40ed-b1b9-5f831b676b56">
           A list item.
          </span>
-         <pre id="312739a0-8bdc-43db-9a8e-ff573b9e0691"><code class="python">List.Item(title, description=None, marker=None, figure=None)</code></pre>
-         <div class="ml-3 collapse" id="f671c8cb-a05d-4701-a147-4295326816b5">
-          <h6 id="73b3fa40-a9d6-4be9-a92e-1839c36c091a">
+         <pre id="9866a7dc-aa78-453a-923f-07c3eaba0672"><code class="python">List.Item(title, description=None, marker=None, figure=None)</code></pre>
+         <div class="ml-3 collapse" id="57840089-11ae-45c9-8421-2c9974349510">
+          <h6 id="d6063d60-3ce3-4ed8-bf6c-517daff37a93">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="cfa61fce-1f1b-44ab-b087-60f68373b3a3">
+          <table class="table table-sm bg-light" id="777b39e2-7108-45a6-8efe-fffa25426688">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -5203,262 +5284,265 @@
              <td>
               The item figure.
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <div class="ml-3" id="02ab5841-4bc0-405c-96bf-d245c7c7782a">
-          <h6 id="4343f0f7-f8e9-4a12-8a92-b3474613b061">
+         <div class="ml-3" id="e29624b9-a07a-4cf2-ba3e-876c43ddf02c">
+          <h6 id="571f8dfe-668f-4ef4-8b97-aec392af806f">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="def81b8c-257a-4022-b38c-1c07c73c29c6"><code class="python">from bootwrap import Button, List, Image
+          <pre id="0d76d4cd-d44d-48b4-b71c-1dc96167e0f4"><code class="python">from bootwrap import Button, List, Image
 
 actions = [
     Button("Buy"),
     Button("Sell"),
     Button("Transfer")
 ]
 
 List.Item(
     "Google (NASDAQ: GOOGL)",
     description= "Price for a single Google share",
     figure=Image("google-logo.png", width=32, height=32),
     marker="12:04:58 12/01/2021"
 ).add_menu(*actions).link(
-    "https://www.google.com")</code></pre>
+    "https://www.google.com")
+</code></pre>
          </div>
-         <div class="ml-3" id="7e911bcd-2ad2-4cc0-9931-86bd7b467c91">
-          <a class="list-group-item list-group-item-action flex-column align-items-start" href="https://www.google.com" id="7a24691c-548b-4626-9cc1-7ae6a23ecfca">
+         <div class="ml-3" id="2d447d4e-5ac2-4833-80ee-ad2802d41412">
+          <a class="list-group-item list-group-item-action flex-column align-items-start" href="https://www.google.com" id="78dfa4dd-fef8-48bd-ae79-9540487c3828">
            <div class="d-flex w-100 justify-content-between">
-            <img height="32" id="bcc6345e-ddac-4a67-8d8c-886dde5dd0bc" src="google-logo.png" width="32"/>
+            <img height="32" id="283ebce7-da49-449b-bee3-f5dd6ad443d2" src="google-logo.png" width="32"/>
             <div class="ml-2 mr-2 w-100">
              <div class="d-flex w-100 justify-content-between">
-              <h5 id="13f7b132-c491-443c-8a3a-381d845fdfd3">
+              <h5 id="34f87f2b-a783-4e4c-bd9b-fd44dbd64d5c">
                Google (NASDAQ: GOOGL)
               </h5>
-              <span id="6e77991f-ebd3-4bcd-8a7f-e71b4be6d281">
+              <span id="ab146a96-64b5-4770-99ce-729937cf1a77">
                <small>
                 12:04:58 12/01/2021
                </small>
               </span>
              </div>
              Price for a single Google share
             </div>
             <div class="d-flex align-items-start">
-             <button class="ml-1 btn" id="139a05cf-9129-4ed1-a3e1-884df54792af" onclick="return false;">
+             <button class="ml-1 btn" id="b3b2290d-c703-470e-84e4-5d7ce8224f91" onclick="return false;">
               Buy
              </button>
-             <button class="ml-1 btn" id="5ef13cef-f0cf-4195-b5c0-721e09218141" onclick="return false;">
+             <button class="ml-1 btn" id="3bbd286e-c5a9-43c9-8b03-4e8f7f49ecde" onclick="return false;">
               Sell
              </button>
-             <button class="ml-1 btn" id="fedeb265-c1b9-457f-8305-79cda5322bb2" onclick="return false;">
+             <button class="ml-1 btn" id="ad33bf76-5702-4ec0-806a-22a21961b383" onclick="return false;">
               Transfer
              </button>
             </div>
            </div>
           </a>
          </div>
-         <div class="mt-5" id="b359e98d-d0a8-49f4-b8bc-4ffc5bd40408">
-          <div class="d-flex justify-content-between" id="1363da24-6830-4c57-a659-ac9f7426c24e">
-           <h4 id="3feffd2d-f8fe-4196-9bef-231e63a45209">
+         <div class="mt-5" id="8cf1f997-492d-4f3d-b932-38e0501c1770">
+          <div class="d-flex justify-content-between" id="149fc34b-dd1f-48ef-8343-013e653ab147">
+           <h4 id="68bc4d34-84f4-4352-82ae-1895da56e452">
             Method
-            <span class="text-primary" id="70d88b57-d2a1-4c31-b836-254e1bbcb3d5">
+            <span class="text-primary" id="c9f83603-f63c-48e9-b13f-9513695712b6">
              as_selected
             </span>
            </h4>
-           <div id="869707c0-3f9c-46e3-b79f-88aec6a3a506">
+           <div id="b34e6efa-f428-4e70-99e7-da7257131f37">
            </div>
           </div>
-          <span class="text-muted" id="08558ed6-35bf-4575-b523-3ec05bc50057">
+          <span class="text-muted" id="7193b69f-c3e4-480d-9b59-a2338e83bbb2">
            Makes a list item selected.
           </span>
-          <pre id="a8438bef-59c4-4f80-a75b-ea38074d7a38"><code class="python">as_selected()</code></pre>
-          <div class="ml-3" id="60b69cac-ca6d-41e4-8eba-2de05eec9e87">
-           <h6 id="e12ff481-734e-4ff8-bc32-ce3855b8c9c5">
+          <pre id="f9dc5312-6387-4651-bc50-8ef516a1a504"><code class="python">as_selected()</code></pre>
+          <div class="ml-3" id="eccc7b23-73d0-4359-a200-3d6d1d64a661">
+           <h6 id="652305b1-28cf-49c6-818b-a5706f5a9ecf">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="bdb41b35-54b7-4281-baa7-ffa4eb2d6568"><code class="python">from bootwrap import Button, List, Image
+           <pre id="60c7177f-a6f6-4d0a-82b2-c430e3ae7078"><code class="python">from bootwrap import Button, List, Image
 
 actions = [
     Button("Buy"),
     Button("Sell"),
     Button("Transfer")
 ]
 
 List.Item(
     "Google (NASDAQ: GOOGL)",
     description= "Price for a single Google share",
     figure=Image("google-logo.png", width=32, height=32),
     marker="12:04:58 12/01/2021"
 ).add_menu(*actions).as_selected().link(
-    "https://www.google.com")</code></pre>
+    "https://www.google.com")
+</code></pre>
           </div>
-          <div class="ml-3" id="60d774e1-d661-43db-9bf5-b76836a42c5f">
-           <a class="list-group-item list-group-item-action flex-column align-items-start active" href="https://www.google.com" id="c8e64c78-3c91-49ae-b771-04e4e30e7207">
+          <div class="ml-3" id="724caf5f-749b-43d5-881b-11c4eaccf025">
+           <a class="list-group-item list-group-item-action flex-column align-items-start active" href="https://www.google.com" id="2789eac7-99e5-4b93-80b1-e0e24190d0e1">
             <div class="d-flex w-100 justify-content-between">
-             <img height="32" id="9336ed78-d983-4419-a8cc-5d46cc448412" src="google-logo.png" width="32"/>
+             <img height="32" id="6ab58e5a-d068-47a5-a7ee-d610d839448b" src="google-logo.png" width="32"/>
              <div class="ml-2 mr-2 w-100">
               <div class="d-flex w-100 justify-content-between">
-               <h5 id="081c21a9-66ab-4073-b5ca-70a4e0c922b2">
+               <h5 id="e18bdeda-d883-4a10-99e7-3af4cd49c927">
                 Google (NASDAQ: GOOGL)
                </h5>
-               <span id="7953f2fd-70a7-4ac6-8e9a-2bf006664724">
+               <span id="1de52a7e-7fff-4084-b9b4-504c89ef6789">
                 <small>
                  12:04:58 12/01/2021
                 </small>
                </span>
               </div>
               Price for a single Google share
              </div>
              <div class="d-flex align-items-start">
-              <button class="ml-1 btn" id="482cb71b-dd7b-4b80-825f-700f6e91573a" onclick="return false;">
+              <button class="ml-1 btn" id="4b5e0f3f-f51b-4c81-a7e1-64ceca2c9c86" onclick="return false;">
                Buy
               </button>
-              <button class="ml-1 btn" id="3e26eb57-a2ce-4252-ae6c-b15e92a0cfa2" onclick="return false;">
+              <button class="ml-1 btn" id="87e1d999-1194-4657-943a-778131969663" onclick="return false;">
                Sell
               </button>
-              <button class="ml-1 btn" id="9070b66a-8578-42d7-90ac-063f9c6379c5" onclick="return false;">
+              <button class="ml-1 btn" id="bb54f022-e906-4595-ba69-f63179065b4b" onclick="return false;">
                Transfer
               </button>
              </div>
             </div>
            </a>
           </div>
          </div>
-         <div class="mt-5" id="131c25de-8576-474c-a182-2ae20ccb9886">
-          <div class="d-flex justify-content-between" id="c8ec05d0-81f6-4b7e-8757-7351e60982c0">
-           <h4 id="dd53bd4c-e4f7-4da9-b1f0-4e424e1f2776">
+         <div class="mt-5" id="f0248b3f-bb42-4619-9659-c3a3db8eade9">
+          <div class="d-flex justify-content-between" id="c4320689-d8af-4d9b-b323-a026a8c90a55">
+           <h4 id="1e816794-0b3a-4388-8f53-baa2a86ba64c">
             Method
-            <span class="text-primary" id="656677e1-a871-4d4c-9ad4-cfe7ba38f5ed">
+            <span class="text-primary" id="476374f8-a4d4-4145-9472-bf8e3024c955">
              pack_actions
             </span>
            </h4>
-           <div id="0a0e7eac-34a4-4276-b569-9478b5eb5516">
+           <div id="e7b18473-d0df-4f63-929e-b8ca58f4bacf">
            </div>
           </div>
-          <span class="text-muted" id="8c79b385-8d9f-415c-a552-eb5eb1ac8a40">
+          <span class="text-muted" id="652c92f9-89f3-403d-a161-fef472a292c6">
            Makes item actions packed under a drop-down menu.
           </span>
-          <pre id="496d4915-379e-4734-bbf5-a2f7a97f9be0"><code class="python">pack_actions()</code></pre>
-          <div class="ml-3" id="f62e04de-b06c-4f51-95a3-f1236407dbc8">
-           <h6 id="006ad53a-a249-4bd5-947c-fee939c898f0">
+          <pre id="295128ca-8115-4d8e-b42b-f0c22348ae60"><code class="python">pack_actions()</code></pre>
+          <div class="ml-3" id="a2a8291e-ce49-4526-a26f-3e4ae94a4aaa">
+           <h6 id="45a85f22-d62c-4113-b6f7-9d767e189208">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="aca05441-26ba-4a78-9730-4cd28b3d3129"><code class="python">from bootwrap import Button, List, Image
+           <pre id="cd84a556-3e5f-4b73-90c5-76285b387dda"><code class="python">from bootwrap import Button, List, Image
 
 actions = [
     Button("Buy"),
     Button("Sell"),
     Button("Transfer")
 ]
 
 List.Item(
     "Google (NASDAQ: GOOGL)",
     description= "Price for a single Google share",
     figure=Image("google-logo.png", width=32, height=32),
     marker="12:04:58 12/01/2021"
 ).add_menu(*actions).pack_actions().link(
-    "https://www.google.com")</code></pre>
+    "https://www.google.com")
+</code></pre>
           </div>
-          <div class="ml-3" id="af8af166-a334-44bd-abcb-c2379eab5c54">
-           <a class="list-group-item list-group-item-action flex-column align-items-start" href="https://www.google.com" id="968eb228-89a6-4bbf-944c-2282b818c577">
+          <div class="ml-3" id="93aae63a-c5aa-480c-9c3d-6971076a05d3">
+           <a class="list-group-item list-group-item-action flex-column align-items-start" href="https://www.google.com" id="d902692c-146f-49b4-a5b0-62b65ed64601">
             <div class="d-flex w-100 justify-content-between">
-             <img height="32" id="b27b241a-0ffa-454a-a0bf-800b70186f52" src="google-logo.png" width="32"/>
+             <img height="32" id="51c7fc8a-62aa-490a-95b1-1289b7ee4120" src="google-logo.png" width="32"/>
              <div class="ml-2 mr-2 w-100">
               <div class="d-flex w-100 justify-content-between">
-               <h5 id="07a77a29-0cec-4aea-81ef-eaf9b3a6f49e">
+               <h5 id="31c399b5-905b-4950-ab51-5723490af600">
                 Google (NASDAQ: GOOGL)
                </h5>
-               <span id="b5b08fe8-bf00-47c8-a1e6-b1fd3eab3d73">
+               <span id="7cdf3663-3935-47ee-8bae-e97635bdbabd">
                 <small>
                  12:04:58 12/01/2021
                 </small>
                </span>
               </div>
               Price for a single Google share
              </div>
              <div class="d-flex align-items-start">
               <div class="btn-group">
-               <i class="btn fas fa-ellipsis-v" data-toggle="dropdown" id="0e7c89c2-ff55-41fb-b1aa-a37d1c3c7aa8" onclick="return false;" style="cursor: pointer">
+               <i class="btn fas fa-ellipsis-v" data-toggle="dropdown" id="157c8cab-a5b6-424e-9b02-6872e50c1055" onclick="return false;" style="cursor: pointer">
                </i>
                <div class="dropdown-menu dropdown-menu-right">
-                <button class="dropdown-item btn" id="5686641a-4276-43da-8847-80459048c6fa" onclick="return false;">
+                <button class="dropdown-item btn" id="36d93799-dc1a-42b7-8ca2-f86309c6abea" onclick="return false;">
                  Buy
                 </button>
-                <button class="dropdown-item btn" id="f2e76e8c-fa47-44bb-a25d-08aa925c2cde" onclick="return false;">
+                <button class="dropdown-item btn" id="31195588-0288-4543-9bbe-a353d2126ee2" onclick="return false;">
                  Sell
                 </button>
-                <button class="dropdown-item btn" id="a45f2352-398b-4afb-9882-ad5123d77139" onclick="return false;">
+                <button class="dropdown-item btn" id="73fa3baa-682b-4851-8ea7-0fd3fa689e65" onclick="return false;">
                  Transfer
                 </button>
                </div>
               </div>
              </div>
             </div>
            </a>
           </div>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="38b3263d-faca-45ad-922d-44f57f4e893b">
-     <div id="d68aa7de-beef-4895-ac95-0a97dfb23fd7">
+    <div class="tab-pane fade" id="2e0eddbe-00fc-4f38-ac91-e546f0ed51fe">
+     <div id="0e1bad9b-5a95-44e2-be5e-01fb1f8b2382">
       <hr/>
-      <ul class="nav" id="c779c838-3a2d-4569-97c8-c0ca467591c0" role="tablist">
+      <ul class="nav" id="6f97e032-8268-40c4-acaa-d6d39837f67c" role="tablist">
        <li class="nav-item">
-        <a class="nav-link active" data-target="#025b8530-6380-43dc-a6ac-33450a7112e3" data-toggle="tab" href="#025b8530-6380-43dc-a6ac-33450a7112e3" id="1dfc307c-d956-457c-86ed-d7864f3a63e3" role="tab">
-         <span class="text-secondary" id="6bdd31e7-c400-438f-a84e-e80b0570fede">
+        <a class="nav-link active" data-target="#e0d95546-9a2a-4bc6-9ae5-385742bfbe5a" data-toggle="tab" href="#e0d95546-9a2a-4bc6-9ae5-385742bfbe5a" id="7c187006-a9d3-4e2e-97cc-a0121e311c65" role="tab">
+         <span class="text-secondary" id="39dfd00f-dae3-41dc-92c9-26a656521f26">
           Navigation
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#e90285fb-d080-4ac0-bc39-03e0aca74ea7" data-toggle="tab" href="#e90285fb-d080-4ac0-bc39-03e0aca74ea7" id="52fed965-189b-4e63-a849-18f731d5b370" role="tab">
-         <span class="text-secondary" id="8862b039-4547-4a8b-9226-a2daebca882e">
+        <a class="nav-link" data-target="#4c47dbe5-9112-4b0b-bca6-11e2dd40a0e0" data-toggle="tab" href="#4c47dbe5-9112-4b0b-bca6-11e2dd40a0e0" id="134da052-3384-41eb-bc1e-68321ffadc8d" role="tab">
+         <span class="text-secondary" id="8031f77a-06ee-4fe1-ba0b-4d2b6d3d34eb">
           Navigation.Item
          </span>
         </a>
        </li>
       </ul>
       <div class="tab-content">
-       <div class="tab-pane fade active show" id="025b8530-6380-43dc-a6ac-33450a7112e3">
-        <div class="mt-5" id="27beff8f-a94b-4a86-99ef-b7b783608ca5">
-         <div class="d-flex justify-content-between" id="fa13013c-b4ab-4d43-8935-462e91697529">
-          <h1 id="d9dc5285-51cd-4661-aeef-08ba1b7032bf">
+       <div class="tab-pane fade active show" id="e0d95546-9a2a-4bc6-9ae5-385742bfbe5a">
+        <div class="mt-5" id="e209d526-a689-43dd-a128-cfc9194e9ed7">
+         <div class="d-flex justify-content-between" id="86eb73d9-abb6-4a0f-a1ab-ac2afeda974e">
+          <h1 id="76cda439-1c97-4a5b-9e1f-f7c219f2ff48">
            Class
-           <span class="text-primary" id="5ba246a8-9474-43df-97b7-8e08b22f8880">
+           <span class="text-primary" id="a2a7a00a-0be3-4532-ba0f-817fa8c19a6c">
             Navigation
            </span>
           </h1>
-          <div id="9213dba7-a8e8-44a8-9e73-b4a8fcfb7cd3">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#dda1f00c-0895-41dd-a5e6-cbcc6dc342a6" data-toggle="collapse" id="4e643ebf-6f9e-4c8b-9ff2-8db7552f9406" onclick="return false;" type="button">
+          <div id="2e614f77-a615-457e-9642-326ed9ddc61f">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#69327648-951a-44c3-993e-fc7a83ee0320" data-toggle="collapse" id="887187eb-a953-4cbd-8fb6-7505082ee7d9" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="6096cc7f-c519-4928-8e08-10e27a0f7359">
+         <span class="text-muted" id="eca943cf-7180-4724-8681-972a1958a88f">
           A web component for navigation.
          </span>
-         <pre id="eed43b34-40a5-49cf-afbd-6883c0568a2c"><code class="python">Navigation(*items)</code></pre>
-         <div class="ml-3 collapse" id="dda1f00c-0895-41dd-a5e6-cbcc6dc342a6">
-          <h6 id="9871d2aa-965c-4bc1-9dc8-fdfd7a841abc">
+         <pre id="e8472137-af20-47f7-9fd1-893063a990ea"><code class="python">Navigation(*items)</code></pre>
+         <div class="ml-3 collapse" id="69327648-951a-44c3-993e-fc7a83ee0320">
+          <h6 id="a5dcf047-0bf0-4677-8242-4a3eb62e8ae4">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="e3e4c967-8c13-4e95-8bb5-46db4963ec83">
+          <table class="table table-sm bg-light" id="a75b72ff-c577-4371-a66e-8c907098e8a8">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -5487,83 +5571,84 @@
               </code>
               .
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <div class="ml-3" id="ae4bb2c4-504c-40d3-b5fc-0d35458920d2">
-          <h6 id="6031225b-9292-4a33-b16a-6dad24001ad3">
+         <div class="ml-3" id="4c3783dc-c65d-4bc0-9f76-738646abd35b">
+          <h6 id="9e5ca4e3-cacb-4b96-96bf-3d3007f2c661">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="0ca53f68-30fd-4ef6-a168-1048c27ab1c2"><code class="python">from bootwrap import Navigation
+          <pre id="34fdfceb-bc2f-44e4-87fe-442b55f1c6f3"><code class="python">from bootwrap import Navigation
 
 Navigation(
     Navigation.Item('Chapter 1', 'Text 1', True),
     Navigation.Item('Chapter 2', 'Text 2'),
     Navigation.Item('Chapter 3', 'Text 3')
-)</code></pre>
+)
+</code></pre>
          </div>
-         <div class="ml-3" id="09636373-a091-4d37-bb0e-5e60bfab1819">
-          <ul class="nav" id="8243c677-3e22-4175-85a1-8e92c4785353" role="tablist">
+         <div class="ml-3" id="ec198140-dedd-4963-9848-85f34c0ff69d">
+          <ul class="nav" id="30cba287-9c0c-4366-99af-16662cf1a644" role="tablist">
            <li class="nav-item">
-            <a class="nav-link active" data-target="#35fcae99-e9eb-4546-9a4b-2b23a43e730f" data-toggle="tab" href="#35fcae99-e9eb-4546-9a4b-2b23a43e730f" id="7b88e2df-45d1-400e-babe-1fc6c092d088" role="tab">
+            <a class="nav-link active" data-target="#a67854eb-1696-49c3-9527-9857c42c1907" data-toggle="tab" href="#a67854eb-1696-49c3-9527-9857c42c1907" id="ef9900c9-2fa6-4733-8124-03aeded08d72" role="tab">
              Chapter 1
             </a>
            </li>
            <li class="nav-item">
-            <a class="nav-link" data-target="#18d0934a-15c6-48a4-96bd-077362ecd658" data-toggle="tab" href="#18d0934a-15c6-48a4-96bd-077362ecd658" id="cf3e48a5-ea04-4edf-a8f2-de8e4e34b7f6" role="tab">
+            <a class="nav-link" data-target="#b7d2a780-d0e7-41b2-8ff0-6c999873b352" data-toggle="tab" href="#b7d2a780-d0e7-41b2-8ff0-6c999873b352" id="33e22191-a5d1-4655-9b6b-e62d25845250" role="tab">
              Chapter 2
             </a>
            </li>
            <li class="nav-item">
-            <a class="nav-link" data-target="#d15d6465-48d2-4f05-8c45-eeec7ae7827d" data-toggle="tab" href="#d15d6465-48d2-4f05-8c45-eeec7ae7827d" id="78444d2b-c7b4-4a5a-a236-aae348943e19" role="tab">
+            <a class="nav-link" data-target="#9ee1bd76-5045-49dd-8c45-272ca2257893" data-toggle="tab" href="#9ee1bd76-5045-49dd-8c45-272ca2257893" id="90a079cd-8286-4dfc-9b26-91ad4a09c3db" role="tab">
              Chapter 3
             </a>
            </li>
           </ul>
           <div class="tab-content">
-           <div class="tab-pane fade active show" id="35fcae99-e9eb-4546-9a4b-2b23a43e730f">
+           <div class="tab-pane fade active show" id="a67854eb-1696-49c3-9527-9857c42c1907">
             Text 1
            </div>
-           <div class="tab-pane fade" id="18d0934a-15c6-48a4-96bd-077362ecd658">
+           <div class="tab-pane fade" id="b7d2a780-d0e7-41b2-8ff0-6c999873b352">
             Text 2
            </div>
-           <div class="tab-pane fade" id="d15d6465-48d2-4f05-8c45-eeec7ae7827d">
+           <div class="tab-pane fade" id="9ee1bd76-5045-49dd-8c45-272ca2257893">
             Text 3
            </div>
           </div>
          </div>
-         <div class="mt-5" id="6d671edf-65a9-403a-9338-f63ed24492d8">
-          <div class="d-flex justify-content-between" id="a4a958e0-37b4-40e1-bbe9-cc2f381d5638">
-           <h4 id="749accff-a91d-40a7-b8ee-6eaa981e7830">
+         <div class="mt-5" id="c6bea685-959c-4edb-a564-37884e7bb653">
+          <div class="d-flex justify-content-between" id="4f15f7f3-aeca-4b66-bd12-750a9bf8a0c7">
+           <h4 id="9e2ef530-0d91-4986-a606-972d1946ef72">
             Method
-            <span class="text-primary" id="8be88d3b-f4a7-41d6-bda3-ef268b2af7f7">
+            <span class="text-primary" id="a8a71267-99c4-4af6-87bd-be0bec16965e">
              as_pills
             </span>
            </h4>
-           <div id="6177090d-cd38-409f-a9c1-c7e4257aa3ce">
-            <button class="btn-sm btn btn-outline-primary" data-target="#43500682-e43a-424b-9c0c-5b8ed84a24c4" data-toggle="collapse" id="471a74fe-db0a-4f28-a4de-f07ee3e7348b" onclick="return false;" type="button">
+           <div id="7cf9a189-962b-4146-8b67-ca35c55086c0">
+            <button class="btn-sm btn btn-outline-primary" data-target="#927d3d0b-1e9d-4bc5-b4ae-7493a2c924e8" data-toggle="collapse" id="5f1ff11e-34d2-462e-8aea-c3c723fd5f60" onclick="return false;" type="button">
              Returns
             </button>
            </div>
           </div>
-          <span class="text-muted" id="239df0c8-7874-4771-b4b5-ea3100e05c82">
+          <span class="text-muted" id="3fe28a69-74c3-4884-b20f-9ea0485d7f5f">
            Makes the navigation controls looks like buttons.
           </span>
-          <pre id="00b233ff-985a-443b-b707-cf1c7e2f9df9"><code class="python">as_pills()</code></pre>
-          <div class="ml-3 collapse" id="43500682-e43a-424b-9c0c-5b8ed84a24c4">
-           <h6 id="c53ff4f1-cb12-488a-95f7-3035c011f686">
+          <pre id="5e9701d4-5a62-40b8-b583-a394c23f5dea"><code class="python">as_pills()</code></pre>
+          <div class="ml-3 collapse" id="927d3d0b-1e9d-4bc5-b4ae-7493a2c924e8">
+           <h6 id="61939198-2629-427a-81a1-b481b8ad45fa">
             <strong>
              Returns
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="af4cbe03-11d2-496a-bbcb-d7077214bdf4">
+           <table class="table table-sm bg-light" id="80678ec8-3536-4ab9-acd3-ac5466b1f76e">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -5588,84 +5673,85 @@
               <td>
                The instance of this class.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3" id="7a1b2e15-0808-4fc9-97d3-f1a19e0c3452">
-           <h6 id="6a14ce31-87fa-48b5-9797-64b070dc6c7d">
+          <div class="ml-3" id="494928fb-ef84-43c7-b51c-70de35f2cfac">
+           <h6 id="7754dc13-e41a-4f9c-8835-2d9383b62b21">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="07a01cdf-df7e-4a50-bbdd-2d926d947968"><code class="python">from bootwrap import Navigation
+           <pre id="19f92588-75e4-43e9-928e-d828a1e1120b"><code class="python">from bootwrap import Navigation
 
 Navigation(
     Navigation.Item('Chapter 1', 'Text 1', True),
     Navigation.Item('Chapter 2', 'Text 2'),
     Navigation.Item('Chapter 3', 'Text 3')
-).as_pills()</code></pre>
+).as_pills()
+</code></pre>
           </div>
-          <div class="ml-3" id="56dc2908-c564-4da0-b067-7dbb280c264a">
-           <ul class="nav nav-pills" id="87c0bbad-0e66-4c10-953b-f367c47c9d37" role="tablist">
+          <div class="ml-3" id="56f44129-09a4-46b7-b575-fde0a503d700">
+           <ul class="nav nav-pills" id="c1ccda4f-e276-4030-a157-af71fdb4d679" role="tablist">
             <li class="nav-item">
-             <a class="nav-link active" data-target="#ebf3eead-9ef3-4207-a557-9c7726bb978a" data-toggle="tab" href="#ebf3eead-9ef3-4207-a557-9c7726bb978a" id="937a9096-32f3-4ae6-886c-1d21bf2a3cc7" role="tab">
+             <a class="nav-link active" data-target="#b5ca0b53-f08a-4ba3-9c0f-111d8461c060" data-toggle="tab" href="#b5ca0b53-f08a-4ba3-9c0f-111d8461c060" id="ad8778f0-444c-4a3b-afd3-2377fd3e4633" role="tab">
               Chapter 1
              </a>
             </li>
             <li class="nav-item">
-             <a class="nav-link" data-target="#32685e99-40fb-48be-9b54-2e1f2e82a9b9" data-toggle="tab" href="#32685e99-40fb-48be-9b54-2e1f2e82a9b9" id="06d0c78a-7992-43a2-b38f-318f078365a2" role="tab">
+             <a class="nav-link" data-target="#934e10ce-4852-4b45-93f8-51fd5c4f1641" data-toggle="tab" href="#934e10ce-4852-4b45-93f8-51fd5c4f1641" id="fd54e060-fad7-476a-a914-f8617445c2fd" role="tab">
               Chapter 2
              </a>
             </li>
             <li class="nav-item">
-             <a class="nav-link" data-target="#d2995456-c1fa-49d7-ad72-d1142083b283" data-toggle="tab" href="#d2995456-c1fa-49d7-ad72-d1142083b283" id="25a40da7-bb32-4cdc-bf4e-29030de2a8ab" role="tab">
+             <a class="nav-link" data-target="#20355b83-7c5f-43d0-8995-23c4aaa28932" data-toggle="tab" href="#20355b83-7c5f-43d0-8995-23c4aaa28932" id="fb61533b-5a1b-4c27-9ea1-b3c8c361b22a" role="tab">
               Chapter 3
              </a>
             </li>
            </ul>
            <div class="tab-content">
-            <div class="tab-pane fade active show" id="ebf3eead-9ef3-4207-a557-9c7726bb978a">
+            <div class="tab-pane fade active show" id="b5ca0b53-f08a-4ba3-9c0f-111d8461c060">
              Text 1
             </div>
-            <div class="tab-pane fade" id="32685e99-40fb-48be-9b54-2e1f2e82a9b9">
+            <div class="tab-pane fade" id="934e10ce-4852-4b45-93f8-51fd5c4f1641">
              Text 2
             </div>
-            <div class="tab-pane fade" id="d2995456-c1fa-49d7-ad72-d1142083b283">
+            <div class="tab-pane fade" id="20355b83-7c5f-43d0-8995-23c4aaa28932">
              Text 3
             </div>
            </div>
           </div>
          </div>
-         <div class="mt-5" id="c5d49733-c400-467a-a91c-91bec39ab1bd">
-          <div class="d-flex justify-content-between" id="84d7ae4d-2171-4fa5-a402-e0dd851f90c4">
-           <h4 id="8fa5b48e-ffbe-4b7d-863c-0ba79903bbc0">
+         <div class="mt-5" id="cc85ea64-e01c-47c8-8390-ea067184f098">
+          <div class="d-flex justify-content-between" id="90c9b2aa-4da8-4d92-9171-9ab00ee48adf">
+           <h4 id="ae874bfd-c129-478c-b5a6-cb72d97e8a6a">
             Method
-            <span class="text-primary" id="c0b42ae9-0eb4-4dce-b93f-b486c59c7879">
+            <span class="text-primary" id="974ad8e0-ab9d-415d-becd-9d196848b0d3">
              as_tabs
             </span>
            </h4>
-           <div id="bfa82992-c715-4b9e-b296-3ff3aa3848f2">
-            <button class="btn-sm btn btn-outline-primary" data-target="#589bee48-cc53-4871-86bd-4da8301ccdc1" data-toggle="collapse" id="bf04b008-a52c-4913-9fc0-18f1cc6bdb29" onclick="return false;" type="button">
+           <div id="97b19845-abb4-49b6-82ca-d193cf23d7be">
+            <button class="btn-sm btn btn-outline-primary" data-target="#c77b94ce-2192-49d5-9fd1-c8eb3cf86160" data-toggle="collapse" id="3c85a06c-a33e-4f49-a18e-0765dcfd0032" onclick="return false;" type="button">
              Returns
             </button>
            </div>
           </div>
-          <span class="text-muted" id="9c19d05a-0b9e-45d0-8687-522c8888a938">
+          <span class="text-muted" id="afe222ac-07dd-429d-9878-6de5a38d904e">
            Makes the navigation controls looks like buttons.
           </span>
-          <pre id="b6c9b429-a917-4394-a0af-1e12fc9b8fe8"><code class="python">as_tabs()</code></pre>
-          <div class="ml-3 collapse" id="589bee48-cc53-4871-86bd-4da8301ccdc1">
-           <h6 id="bfba8e86-0ae8-43b3-966d-d1fdab2f8633">
+          <pre id="b9910c53-c667-45dd-a891-d7fe1599dd29"><code class="python">as_tabs()</code></pre>
+          <div class="ml-3 collapse" id="c77b94ce-2192-49d5-9fd1-c8eb3cf86160">
+           <h6 id="32fe9e86-c552-4d83-ad7f-eb340fffeef0">
             <strong>
              Returns
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="b6f7fc12-fb1f-47c9-8da6-9a9644d51500">
+           <table class="table table-sm bg-light" id="e33cd49d-cc59-4267-9c82-75548f829856">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -5690,84 +5776,85 @@
               <td>
                The instance of this class.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3" id="31abec31-0cda-4ba5-8c32-e363bb96a636">
-           <h6 id="31421fa2-7979-4822-8213-3cb1e37f139b">
+          <div class="ml-3" id="2caac777-3c8a-4985-8c17-a2b4f49a1452">
+           <h6 id="2fe0eb89-541a-447c-bd1d-9d1d5bfa4b8f">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="82fb8565-6fa4-4761-b557-facf81dcbb84"><code class="python">from bootwrap import Navigation
+           <pre id="29be6834-ad54-4161-ad39-00611f4ca059"><code class="python">from bootwrap import Navigation
 
 Navigation(
     Navigation.Item('Chapter 1', 'Text 1', True),
     Navigation.Item('Chapter 2', 'Text 2'),
     Navigation.Item('Chapter 3', 'Text 3')
-).as_tabs()</code></pre>
+).as_tabs()
+</code></pre>
           </div>
-          <div class="ml-3" id="36b057ca-f0c6-4172-a5a8-f9fc3d0ccae2">
-           <ul class="nav nav-tabs" id="66ee380a-63e5-4c19-912f-63244bd97677" role="tablist">
+          <div class="ml-3" id="38281e08-978b-4424-8478-161f9d4cb560">
+           <ul class="nav nav-tabs" id="fa5b717e-427d-412a-b9f0-f07e1000a542" role="tablist">
             <li class="nav-item">
-             <a class="nav-link active" data-target="#0b8568c9-eac2-4fc0-a364-9a4f8cc55c8a" data-toggle="tab" href="#0b8568c9-eac2-4fc0-a364-9a4f8cc55c8a" id="3ffae2b2-e66c-4566-a48a-b5c16d38b8a7" role="tab">
+             <a class="nav-link active" data-target="#f529e123-5c92-432f-8fb5-2e73ccf8c2d7" data-toggle="tab" href="#f529e123-5c92-432f-8fb5-2e73ccf8c2d7" id="37491a7b-a8ae-4ff4-9267-0cb9b67f9c0f" role="tab">
               Chapter 1
              </a>
             </li>
             <li class="nav-item">
-             <a class="nav-link" data-target="#c09b0b6b-0980-402c-997d-ac80c7afc9c6" data-toggle="tab" href="#c09b0b6b-0980-402c-997d-ac80c7afc9c6" id="39b1c084-02c9-423c-9b54-b824c2a72ad4" role="tab">
+             <a class="nav-link" data-target="#3aa7d74f-f19c-4383-9a65-5766fd6362ed" data-toggle="tab" href="#3aa7d74f-f19c-4383-9a65-5766fd6362ed" id="fb1e9e16-3925-466e-b4b4-3e7adafa0007" role="tab">
               Chapter 2
              </a>
             </li>
             <li class="nav-item">
-             <a class="nav-link" data-target="#fa317664-006f-44a0-9746-b8f238f45f46" data-toggle="tab" href="#fa317664-006f-44a0-9746-b8f238f45f46" id="2d40e312-0f59-49e4-b8d0-800cd669d611" role="tab">
+             <a class="nav-link" data-target="#c3aac4ef-b37d-4c0b-93ad-dbcf51c92963" data-toggle="tab" href="#c3aac4ef-b37d-4c0b-93ad-dbcf51c92963" id="0c257d3a-fb17-4e5c-afec-a64723662333" role="tab">
               Chapter 3
              </a>
             </li>
            </ul>
            <div class="tab-content">
-            <div class="tab-pane fade active show" id="0b8568c9-eac2-4fc0-a364-9a4f8cc55c8a">
+            <div class="tab-pane fade active show" id="f529e123-5c92-432f-8fb5-2e73ccf8c2d7">
              Text 1
             </div>
-            <div class="tab-pane fade" id="c09b0b6b-0980-402c-997d-ac80c7afc9c6">
+            <div class="tab-pane fade" id="3aa7d74f-f19c-4383-9a65-5766fd6362ed">
              Text 2
             </div>
-            <div class="tab-pane fade" id="fa317664-006f-44a0-9746-b8f238f45f46">
+            <div class="tab-pane fade" id="c3aac4ef-b37d-4c0b-93ad-dbcf51c92963">
              Text 3
             </div>
            </div>
           </div>
          </div>
-         <div class="mt-5" id="f79945bd-eff1-4432-ab7d-d526ffb66eb3">
-          <div class="d-flex justify-content-between" id="a724b99e-1cae-4afa-8fd9-11bae6791c30">
-           <h4 id="816a0bcd-b162-4733-a575-825df8edff45">
+         <div class="mt-5" id="d9d80ee3-79e0-462f-b53a-c5402ef007e1">
+          <div class="d-flex justify-content-between" id="9a1b1b66-a047-4432-a9f4-b8e844fa4eeb">
+           <h4 id="389a5d41-47f9-4745-a97e-edb5932c538d">
             Method
-            <span class="text-primary" id="3ddbc6d9-fe4d-4d20-8266-3fa81f0270b1">
+            <span class="text-primary" id="27fe23e9-ebbc-4c49-b57e-34126d842bca">
              as_vertical
             </span>
            </h4>
-           <div id="fb3d9b49-cf1c-46cd-879e-e53caca9c272">
-            <button class="btn-sm btn btn-outline-primary" data-target="#15ad7dc9-e3db-4b61-8dba-d763de768022" data-toggle="collapse" id="b0517052-b562-4d78-b310-27e4c4cc1e4d" onclick="return false;" type="button">
+           <div id="7a91e72d-e20a-4307-8fa7-7f0dde3d95b4">
+            <button class="btn-sm btn btn-outline-primary" data-target="#43b5ec05-cbe4-484e-8ef7-b9f3db443826" data-toggle="collapse" id="e5382dc6-d62a-4497-afe7-a565abf41876" onclick="return false;" type="button">
              Returns
             </button>
            </div>
           </div>
-          <span class="text-muted" id="a0256654-db76-410f-a82a-600964ef39e0">
+          <span class="text-muted" id="350997ab-fd25-4720-a3f2-0f4fcabda3ad">
            Makes the navigation vertical.
           </span>
-          <pre id="f68997ad-4add-4814-9495-6219496ca85d"><code class="python">as_vertical()</code></pre>
-          <div class="ml-3 collapse" id="15ad7dc9-e3db-4b61-8dba-d763de768022">
-           <h6 id="104ecd90-8981-43e2-ae92-12d6bc378a5d">
+          <pre id="580e2e30-5750-4149-9409-cbcd01779a27"><code class="python">as_vertical()</code></pre>
+          <div class="ml-3 collapse" id="43b5ec05-cbe4-484e-8ef7-b9f3db443826">
+           <h6 id="6eb0ff5c-2981-40f3-a538-8cef0ba0c9dc">
             <strong>
              Returns
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="789dd743-1bac-4ea7-ab24-cb55adcaa9df">
+           <table class="table table-sm bg-light" id="173a8d72-42b1-4d60-9c52-6364ce121344">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -5792,143 +5879,144 @@
               <td>
                The instance of this class.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3" id="8fc09fb4-c653-4dc2-bad7-7ce24ecdba65">
-           <h6 id="cce78783-69e8-469a-a9bd-5a3b2df9a47a">
+          <div class="ml-3" id="1a9e4c84-d356-4fe2-9207-13e616bff8ef">
+           <h6 id="1b249a6f-c068-475d-972a-559771ed5607">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="40e625da-b107-4cd6-ac8f-26f81693fd5e"><code class="python">from bootwrap import Navigation
+           <pre id="db02f043-5cf4-4d79-a235-75efb5da5e0b"><code class="python">from bootwrap import Navigation
 
 Navigation(
     Navigation.Item('Chapter 1', 'Text 1', True),
     Navigation.Item('Chapter 2', 'Text 2'),
     Navigation.Item('Chapter 3', 'Text 3')
-).as_vertical()</code></pre>
+).as_vertical()
+</code></pre>
           </div>
-          <div class="ml-3" id="b3514244-80c6-49d3-9a0d-06f16730b5bc">
+          <div class="ml-3" id="945dc044-2d85-43f4-9c76-ecc42c54abca">
            <div class="d-flex">
-            <ul class="nav flex-column" id="786c4adc-423b-47ed-b840-ac3b0cf85099" role="tablist">
+            <ul class="nav flex-column" id="d3f61683-e598-42f5-88db-0aca30f75471" role="tablist">
              <li class="nav-item">
-              <a class="nav-link active" data-target="#5000977f-26d8-487b-a125-7f7eb411c81e" data-toggle="tab" href="#5000977f-26d8-487b-a125-7f7eb411c81e" id="62e63ad9-ef57-43f5-9426-a9f3c8468d93" role="tab">
+              <a class="nav-link active" data-target="#e12e9c4e-a87a-45b7-bc41-1ca81fdcdd84" data-toggle="tab" href="#e12e9c4e-a87a-45b7-bc41-1ca81fdcdd84" id="60487452-e068-4781-bf9f-479604912710" role="tab">
                Chapter 1
               </a>
              </li>
              <li class="nav-item">
-              <a class="nav-link" data-target="#50ac0d36-5afd-458e-894a-bc87ebd5396c" data-toggle="tab" href="#50ac0d36-5afd-458e-894a-bc87ebd5396c" id="0d5d76eb-eac0-4081-abe3-e661dd57ac7e" role="tab">
+              <a class="nav-link" data-target="#2c2eb52c-4c14-4c75-90a8-b63cfb55e23f" data-toggle="tab" href="#2c2eb52c-4c14-4c75-90a8-b63cfb55e23f" id="1324de17-f180-4f65-b23e-c87ee8af286d" role="tab">
                Chapter 2
               </a>
              </li>
              <li class="nav-item">
-              <a class="nav-link" data-target="#5fefdccc-0881-433b-a191-658f35e17daf" data-toggle="tab" href="#5fefdccc-0881-433b-a191-658f35e17daf" id="5d517906-8c6a-4e68-9ef7-8b599eefabf4" role="tab">
+              <a class="nav-link" data-target="#eba331fc-fa2f-4c4a-9b17-b6e6c09f50cf" data-toggle="tab" href="#eba331fc-fa2f-4c4a-9b17-b6e6c09f50cf" id="0a584c4c-5921-423a-b0ff-279c3e3dcb1e" role="tab">
                Chapter 3
               </a>
              </li>
             </ul>
             <div class="tab-content">
-             <div class="tab-pane fade active show" id="5000977f-26d8-487b-a125-7f7eb411c81e">
+             <div class="tab-pane fade active show" id="e12e9c4e-a87a-45b7-bc41-1ca81fdcdd84">
               Text 1
              </div>
-             <div class="tab-pane fade" id="50ac0d36-5afd-458e-894a-bc87ebd5396c">
+             <div class="tab-pane fade" id="2c2eb52c-4c14-4c75-90a8-b63cfb55e23f">
               Text 2
              </div>
-             <div class="tab-pane fade" id="5fefdccc-0881-433b-a191-658f35e17daf">
+             <div class="tab-pane fade" id="eba331fc-fa2f-4c4a-9b17-b6e6c09f50cf">
               Text 3
              </div>
             </div>
            </div>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="e90285fb-d080-4ac0-bc39-03e0aca74ea7">
-        <div class="mt-5" id="60004618-b22c-4614-aa45-e24bd595159c">
-         <div class="d-flex justify-content-between" id="76b6484c-a3ad-4355-85b2-1ad2a8d9c374">
-          <h1 id="a6b87a93-6f21-48c4-be7e-ea447d1370ac">
+       <div class="tab-pane fade" id="4c47dbe5-9112-4b0b-bca6-11e2dd40a0e0">
+        <div class="mt-5" id="865a130e-75d2-49d3-ade4-f03fea93fb33">
+         <div class="d-flex justify-content-between" id="7c7cd6ae-05bc-4eab-902f-90a5bc7357e7">
+          <h1 id="ce149afe-ec5e-43d9-9c1d-263be9aee331">
            Class
-           <span class="text-primary" id="a110d7eb-a3f9-4c5d-9f81-c0c9f82828a3">
+           <span class="text-primary" id="62f1934e-3768-485b-b383-39a68bbe3714">
             Navigation.Item
            </span>
           </h1>
-          <div id="6717874f-8c4c-4350-8fb8-87681962aa29">
+          <div id="33716185-ffe3-4bbc-aa64-be18e6d381a6">
           </div>
          </div>
-         <span class="text-muted" id="33eac1a2-b9b1-420b-89ed-b94320335a5a">
+         <span class="text-muted" id="675c561d-1e83-453c-9936-2bbce50fb7bf">
           None
          </span>
-         <pre id="8ebdcbe2-efde-434b-ac7c-edcc135fb093"><code class="python">Navigation.Item(name, content, active=False)</code></pre>
-         <div class="mt-5" id="34e310cb-5b5d-4a30-bf12-4f2e66364088">
-          <h4 id="c5b3d425-9fca-4009-81a9-e3347c2e95fc">
+         <pre id="02cf311c-0873-4032-bc1a-b504fc2f3190"><code class="python">Navigation.Item(name, content, active=False)</code></pre>
+         <div class="mt-5" id="22d15ea4-2031-46d6-8ca0-9ee5d419b8d6">
+          <h4 id="11b641f1-8709-465a-bd6b-f520376932a6">
            Property
-           <span class="text-primary" id="91978a43-02fa-40e7-9234-b3acb84fb990">
+           <span class="text-primary" id="97e97a2e-f7ab-4ab2-89a6-6fe4253668ac">
             active
            </span>
           </h4>
-          <span class="text-muted" id="1fb24c4f-3ae0-4793-a5d3-58ef8650bf54">
+          <span class="text-muted" id="cfaefa89-5c51-4db0-817e-5661476c07ce">
            None
           </span>
          </div>
-         <div class="mt-5" id="2588c9f6-69de-4202-aedb-1971de046a19">
-          <h4 id="2adec194-ba09-4b37-9b62-1674b2be984d">
+         <div class="mt-5" id="80ee56da-e200-40be-aa39-c0624cf483c1">
+          <h4 id="66ed49d8-6afa-4ac3-8ea2-276554fe743b">
            Property
-           <span class="text-primary" id="1f6a8e14-5c25-4b22-bd93-cff4b023fc95">
+           <span class="text-primary" id="64f7db30-98a7-4dc0-b663-7e364aa7e6d3">
             content
            </span>
           </h4>
-          <span class="text-muted" id="4576e903-9489-46f8-a32b-855e5e7e26a1">
+          <span class="text-muted" id="45101028-f658-433c-9668-cd3ea39d80eb">
            None
           </span>
          </div>
-         <div class="mt-5" id="66f3f50d-136e-4339-b6fc-9094b133dd5f">
-          <h4 id="fb06e49c-5727-4b32-a8ea-f39262d4a481">
+         <div class="mt-5" id="e95b8804-51f8-45dd-8974-a10950a8ab86">
+          <h4 id="e3c03629-3cba-42ef-bbb2-80ee11908bfd">
            Property
-           <span class="text-primary" id="ce1e3b8e-33af-4166-9b1d-b7b6c26207cc">
+           <span class="text-primary" id="311b0529-0f65-4f68-8d08-27840e31718b">
             name
            </span>
           </h4>
-          <span class="text-muted" id="3c20fe6f-10c9-49ee-925f-9faa88d2ef87">
+          <span class="text-muted" id="28fad79f-784a-4d9e-be9b-9d3bfb6f0e64">
            None
           </span>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="bfe157cf-f2ed-4ea9-bcf1-4ef6d300462f">
-     <div class="mt-5" id="2b477959-afd9-48ec-9c33-22f546b83046">
-      <div class="d-flex justify-content-between" id="c7114cb6-4507-42b3-96a9-6d3f90e38913">
-       <h1 id="e8e64b84-c74b-4f69-ab7f-5d8d02025a85">
+    <div class="tab-pane fade" id="f7091e9c-ac2e-41c2-99ac-4022059d7445">
+     <div class="mt-5" id="5090deec-97f7-4dcc-8985-9d2b756994df">
+      <div class="d-flex justify-content-between" id="a7d643ce-8b1b-4acb-8790-03b13703087b">
+       <h1 id="05abf152-5d16-4dd8-81bb-f1edd0f3f34a">
         Class
-        <span class="text-primary" id="bbcacb52-7fe4-4c91-8d2b-9f974c4af429">
+        <span class="text-primary" id="9f836034-87e1-4df8-8495-2584ebe7f5e7">
          Panel
         </span>
        </h1>
-       <div id="7fdf7212-c7d0-4055-8f35-331c45c048b9">
-        <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#faffe7d1-78d1-4276-ae96-3632f1d97633" data-toggle="collapse" id="3434add7-661b-4399-a089-9cc60fcf0403" onclick="return false;" type="button">
+       <div id="c1e2ce19-e6b4-4362-9ebe-1ae96dbb26ff">
+        <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#206f5879-3a3a-4484-bbc6-1c8cda60d582" data-toggle="collapse" id="c844a12e-6e9f-4ee5-b6e7-75ab0ab02159" onclick="return false;" type="button">
          Argument
         </button>
        </div>
       </div>
-      <span class="text-muted" id="cab3bc69-081f-4c3f-92c2-e454825d3f50">
+      <span class="text-muted" id="24767441-ec75-4ccf-8b33-54db223b87e9">
        A web component for a panel.
       </span>
-      <pre id="e902811f-01bf-426a-9d8c-ae9095964fe8"><code class="python">Panel(*components)</code></pre>
-      <div class="ml-3 collapse" id="faffe7d1-78d1-4276-ae96-3632f1d97633">
-       <h6 id="d0f74578-05fa-4711-81a9-cdb549505f91">
+      <pre id="93630a5d-b51e-4aee-b8e7-912a856c2ea4"><code class="python">Panel(*components)</code></pre>
+      <div class="ml-3 collapse" id="206f5879-3a3a-4484-bbc6-1c8cda60d582">
+       <h6 id="5e290abc-9490-4680-be9d-4f85ecd6f3b7">
         <strong>
          Arguments
         </strong>
        </h6>
-       <table class="table table-sm bg-light" id="609df45a-fdf0-4756-a618-97258cb0c4c0">
+       <table class="table table-sm bg-light" id="17a78108-8010-423a-a707-091a0dc86723">
         <thead>
          <tr>
           <th scope="col">
            Name
           </th>
           <th scope="col">
            Type
@@ -5957,66 +6045,67 @@
            </code>
            .
           </td>
          </tr>
         </tbody>
        </table>
       </div>
-      <div class="ml-3" id="d9400255-d561-4c54-bde7-5e39b146f58f">
-       <h6 id="adf2159a-a22d-4dc2-83c0-e92f82bbbc8c">
+      <div class="ml-3" id="a957ec8d-44c8-4c33-a26f-5959e3e094b3">
+       <h6 id="3537bb39-8c48-423d-9db3-a739b4e9284f">
         <strong>
          Example
         </strong>
        </h6>
-       <pre id="4d547bc0-5cec-4e2e-a61a-6537b888c547"><code class="python">from bootwrap import Text, Panel
+       <pre id="941cfcf3-21ee-4809-8f5e-2fe013cc698c"><code class="python">from bootwrap import Text, Panel
 
-comp1 = Text("Component 1")
-comp2 = Text("Component 2")
-comp3 = Text("Component 3")
+comp1 = Text("Component 1").add_classes("border").ml(1)
+comp2 = Text("Component 2").add_classes("border").ml(1)
+comp3 = Text("Component 3").add_classes("border").ml(1)
 
-Panel(comp1, comp2, comp3)</code></pre>
+Panel(comp1, comp2, comp3)
+</code></pre>
       </div>
-      <div class="ml-3" id="b8e3f0ee-4aec-4041-8fcb-1cda06e70ca6">
-       <div id="831d2d1e-5d50-4f42-a2ea-94e804cb16cd">
-        <span class="border ml-1" id="b8d1a8ae-5ba4-46b6-b1b0-5b95175d6b27">
+      <div class="ml-3" id="b368d7b8-ed6f-45d0-a9ff-ff011671fc03">
+       <div id="d4a53100-1455-4110-9b54-064bbe574fac">
+        <span class="border ml-1" id="1712d8af-2036-45fb-b119-f14df591dac8">
          Component 1
         </span>
-        <span class="border ml-1" id="ee032c6d-855d-4263-8583-10d20c6ce33a">
+        <span class="border ml-1" id="d8b3a050-ba01-4d3a-9a4d-5d5c5e752d4e">
          Component 2
         </span>
-        <span class="border ml-1" id="24ce4810-936a-4935-b43e-242566b830ec">
+        <span class="border ml-1" id="6e96accc-498a-453e-874e-a9f3ba60417d">
          Component 3
         </span>
        </div>
       </div>
-      <div class="mt-5" id="2399dcea-2ca8-402c-93fb-6d6e560debc3">
-       <div class="d-flex justify-content-between" id="7674dd72-47d9-45f8-b080-3f0bc0bee53e">
-        <h4 id="7d866bb1-a496-4772-8937-a582f9c72174">
+      <div class="mt-5" id="b2cce849-8825-4c74-8e93-a8811e41b02f">
+       <div class="d-flex justify-content-between" id="e2eb7c3f-3608-4906-a886-11d48bbf2ca8">
+        <h4 id="31216d87-bf5e-4910-be50-61a6b2d4b81f">
          Method
-         <span class="text-primary" id="dd792503-ae53-494b-83d6-b23b7b9e35f1">
+         <span class="text-primary" id="b9b0f044-eb5d-4e25-a5c9-c17838fa220d">
           as_collapse
          </span>
         </h4>
-        <div id="1e4c07e3-bdef-4e54-8584-323a9cc8cee6">
-         <button class="btn-sm btn btn-outline-primary" data-target="#0c21abfd-0ac6-4261-8ce6-1ee286b72391" data-toggle="collapse" id="45b2069f-ef18-4efa-9166-ddd5fc616cf3" onclick="return false;" type="button">
+        <div id="02d794d0-ec97-43ec-8147-ad9277fedf6d">
+         <button class="btn-sm btn btn-outline-primary" data-target="#89c62454-8320-4500-b907-1919292ac3fa" data-toggle="collapse" id="f1793fc3-4d43-4e38-aa6c-09a72482e6d5" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="b2270d1d-47ac-4c78-aca3-91fe8e86acd6">
+       <span class="text-muted" id="ae5a7458-f47e-43b3-9625-d6ae7668f794">
         Makes the panel collapsed.
        </span>
-       <pre id="37a4ab84-d3d8-407e-a055-5acad56d104d"><code class="python">as_collapse()</code></pre>
-       <div class="ml-3 collapse" id="0c21abfd-0ac6-4261-8ce6-1ee286b72391">
-        <h6 id="ca0269a3-3dd2-46d0-b5c5-fceb26e09740">
+       <pre id="68e5ec1f-1d37-4284-a141-b8a583e8b559"><code class="python">as_collapse()</code></pre>
+       <div class="ml-3 collapse" id="89c62454-8320-4500-b907-1919292ac3fa">
+        <h6 id="be86232c-39d7-49d8-9785-40a18a2a5bd5">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="5352ca57-63c3-4646-bc81-3cc30b35df35">
+        <table class="table table-sm bg-light" id="3a9025d8-95e1-4ab5-a28f-895f486db25a">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -6042,40 +6131,40 @@
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
       </div>
-      <div class="mt-5" id="82a64652-c7d4-447a-b841-3e124e862406">
-       <div class="d-flex justify-content-between" id="80a6eccc-9292-4ba3-8bfa-12be74db72c8">
-        <h4 id="d495ea3e-9b84-4d52-a93e-3e7ab9b345c7">
+      <div class="mt-5" id="318f7bf6-9983-40ad-b88b-4a066678333c">
+       <div class="d-flex justify-content-between" id="e043289b-ec53-48e6-a70a-81afea7e220e">
+        <h4 id="5e72efcc-23e7-4a6b-b24b-bb0e56c39cdc">
          Method
-         <span class="text-primary" id="b7ea10a1-10b1-4613-bf61-bb151c681c56">
+         <span class="text-primary" id="133657d1-213f-49b7-8ec9-9c851ad8a1af">
           horizontal
          </span>
         </h4>
-        <div id="3e838e4c-5e97-479d-8546-62b2a625a2d7">
-         <button class="btn-sm btn btn-outline-primary" data-target="#eb0e79e8-ae51-43c8-99da-652e904b41f8" data-toggle="collapse" id="5000ac46-045e-4bd6-a3c0-3f3472e88173" onclick="return false;" type="button">
+        <div id="a6e8055a-deae-427f-9fc2-7f1e5ad4bc33">
+         <button class="btn-sm btn btn-outline-primary" data-target="#84442c1c-caa2-4faf-9477-256bb7553200" data-toggle="collapse" id="60c928ac-533c-4708-85ff-20e79ffcbcac" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="4531e9e5-4d19-4e37-9d7d-19d1516137bc">
+       <span class="text-muted" id="838cbc44-e33b-46fc-8940-3920d7eca40b">
         Makes the panel with the horizontal arrangement of encapsulating
         elements
        </span>
-       <pre id="ca5043b6-1c7b-45bf-a7d0-c338cc79be2d"><code class="python">horizontal()</code></pre>
-       <div class="ml-3 collapse" id="eb0e79e8-ae51-43c8-99da-652e904b41f8">
-        <h6 id="8973a705-e553-4a27-8567-d94a5ad0d48a">
+       <pre id="fff36d14-17ae-4dcf-a53c-8cd4c0211ebb"><code class="python">horizontal()</code></pre>
+       <div class="ml-3 collapse" id="84442c1c-caa2-4faf-9477-256bb7553200">
+        <h6 id="95c0ad98-15d2-4073-96f8-6cf3b199617d">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="3c47fd87-2518-4fa3-915f-84d77305fa21">
+        <table class="table table-sm bg-light" id="13722424-8593-47a2-b7b6-b4eea731d01c">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -6100,76 +6189,77 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="5991d4b0-e573-481b-9264-ce6c7189f1ce">
-        <h6 id="b6683444-2fff-49c9-b28c-bd0871832e60">
+       <div class="ml-3" id="c61ffd8d-a5a4-4c59-ae97-eb6b4a22c82c">
+        <h6 id="b5785844-9acc-4658-8c30-f59c441f4e8d">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="226ee23f-0f2c-4113-aeb1-f83e76905b54"><code class="python">from bootwrap import Text, Panel
+        <pre id="e3cba007-7a67-454d-9369-8230763f0d57"><code class="python">from bootwrap import Text, Panel
 
-comp1 = Text("Component 1")
-comp2 = Text("Component 2")
-comp3 = Text("Component 3")
+comp1 = Text("Component 1").add_classes("border")
+comp2 = Text("Component 2").add_classes("border")
+comp3 = Text("Component 3").add_classes("border")
 
-Panel(comp1, comp2, comp3).horizontal()</code></pre>
+Panel(comp1, comp2, comp3).horizontal()
+</code></pre>
        </div>
-       <div class="ml-3" id="f09efdf4-da97-4abb-9fd0-19d7138cc0e3">
-        <div id="26f3f417-2bfa-4711-9b2e-fe542e72888c">
+       <div class="ml-3" id="d03b9bbb-5b5f-4c71-bf7b-afc9d51a67c8">
+        <div id="ee90bd17-053e-47eb-a449-64efccc9e9d1">
          <div class="row">
           <div class="col-md">
-           <span class="border" id="07adc940-ddba-4439-a8a4-06b5d1b23adb">
+           <span class="border" id="7e8a34cf-d61c-4f0c-af62-ad606a90f1ed">
             Component 1
            </span>
           </div>
           <div class="col-md">
-           <span class="border" id="0aca3b50-2b0f-4da3-a13a-83b94abc87dc">
+           <span class="border" id="0a64c99a-e71a-4d28-acee-83f9c3bebb82">
             Component 2
            </span>
           </div>
           <div class="col-md">
-           <span class="border" id="6a6443d7-afa7-4224-80ce-7112ded53404">
+           <span class="border" id="ac1c14bd-8cce-4c0f-9f79-6662c432d413">
             Component 3
            </span>
           </div>
          </div>
         </div>
        </div>
       </div>
-      <div class="mt-5" id="c376e1b2-c4e7-4f34-8c40-68c0b0a76581">
-       <div class="d-flex justify-content-between" id="fb94eee8-f1bf-4175-84fe-6250ef3369ee">
-        <h4 id="e49dcc97-c49a-4519-9443-31e5142d87bb">
+      <div class="mt-5" id="cd33ea73-9215-4b07-8a72-1341a05c90bb">
+       <div class="d-flex justify-content-between" id="fe1f8a9b-d9e9-4d66-89c2-b3fbca49ae44">
+        <h4 id="b0e8620c-c34b-4e39-8f62-cfcd92f37b10">
          Method
-         <span class="text-primary" id="1f3b2d47-db29-4e3a-8903-ab2d836b43cb">
+         <span class="text-primary" id="ef927c78-bd33-4fa7-88b0-2dbd6304c056">
           vertical
          </span>
         </h4>
-        <div id="ed9fb76a-107d-4aae-82da-541f8e3b7913">
-         <button class="btn-sm btn btn-outline-primary" data-target="#8d3e57b8-6a8f-49ac-b277-d88455e415f3" data-toggle="collapse" id="9723cf66-a5a9-4f6f-a311-30d4ad17a559" onclick="return false;" type="button">
+        <div id="b24a5ab4-8c79-4701-be9c-36c2a8595ebc">
+         <button class="btn-sm btn btn-outline-primary" data-target="#be1560ff-8177-4484-9ddb-f8f8e3833974" data-toggle="collapse" id="0a7b1399-27f9-4622-9fdd-bc93b3fc0408" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="1b000534-8db4-45ab-8aa5-2d72fc63b1e4">
+       <span class="text-muted" id="29a6766b-05ab-45bb-9520-5ad74f4e698d">
         Makes the panel with the vertical arrangement of encapsulating
         elements
        </span>
-       <pre id="88c3f5fd-fe27-493a-ad46-7d2ff690ab8d"><code class="python">vertical()</code></pre>
-       <div class="ml-3 collapse" id="8d3e57b8-6a8f-49ac-b277-d88455e415f3">
-        <h6 id="caaf70bf-8b0a-4b91-8700-8c07d92cad59">
+       <pre id="ec21d7f9-2c64-4425-bc2b-de2df96a1f68"><code class="python">vertical()</code></pre>
+       <div class="ml-3 collapse" id="be1560ff-8177-4484-9ddb-f8f8e3833974">
+        <h6 id="6cc9be71-b2fa-4a04-8018-f2e4f4926c9e">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="fc56a65a-76a2-4e7c-95db-c9f50491b014">
+        <table class="table table-sm bg-light" id="544a7d2c-66e7-4403-80bb-8ad872a37b00">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -6194,150 +6284,154 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="e83e9a20-804a-4b7b-8b10-0eeb01160feb">
-        <h6 id="87e83fa7-762e-4366-95b2-00445642058a">
+       <div class="ml-3" id="f11cb27c-8eb6-4330-94ca-67c23dd69618">
+        <h6 id="dc141406-945c-4eff-9e1d-460d22bbb11f">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="b1a4e5d7-1cf5-4ad5-8c21-86f5b573933d"><code class="python">from bootwrap import Text, Panel
+        <pre id="f1c7d18e-ddfb-4658-a703-c7c950a3d777"><code class="python">from bootwrap import Text, Panel
 
-comp1 = Text("Component 1")
-comp2 = Text("Component 2")
-comp3 = Text("Component 3")
+comp1 = Text("Component 1").add_classes("border")
+comp2 = Text("Component 2").add_classes("border")
+comp3 = Text("Component 3").add_classes("border")
 
-Panel(comp1, comp2, comp3).vertical()</code></pre>
+Panel(comp1, comp2, comp3).vertical()
+</code></pre>
        </div>
-       <div class="ml-3" id="766e646c-01d9-45cf-97a5-0d584ac5796d">
-        <div id="5f6d4267-452b-49f4-973f-368861bf8ed4">
+       <div class="ml-3" id="ac30cf0d-95e9-4e09-a13b-4b0c63e3ba91">
+        <div id="c79dd728-183c-4397-b6eb-c5c8e5f5aef1">
          <div class="row">
           <div class="col-md">
-           <span class="border" id="2b61a619-46df-4d10-bc62-1a3f54a4191e">
+           <span class="border" id="4cfe1dcd-e609-4aed-896a-b46af3e5a3ac">
             Component 1
            </span>
           </div>
          </div>
          <div class="row">
           <div class="col-md">
-           <span class="border" id="898140c6-cf4f-4ca5-9534-4bc5710af81a">
+           <span class="border" id="a7f63e5b-24c9-4b89-ada6-194e2e41089e">
             Component 2
            </span>
           </div>
          </div>
          <div class="row">
           <div class="col-md">
-           <span class="border" id="d62c352d-43a8-4d97-877a-42e5098adebb">
+           <span class="border" id="36bbadc3-b0b9-4fec-9c34-8df61381406c">
             Component 3
            </span>
           </div>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="6dc2e0f8-dd9b-4e2f-ad92-c8c98acc78d8">
-     <div class="mt-5" id="a1de0c54-a8bf-4464-b723-b1b78e001dc2">
-      <div class="d-flex justify-content-between" id="69363987-a19c-484e-aeb9-cce145d70093">
-       <h1 id="1b01ee77-6a35-4306-b8e1-f8d08abe5e20">
+    <div class="tab-pane fade" id="5dff1a6c-3836-464a-9083-5f34c8806812">
+     <div class="mt-5" id="a5d21f53-bb2b-4436-87ed-d4a742a845c0">
+      <div class="d-flex justify-content-between" id="8bd87c6b-6f55-4121-84a5-4916e06a6c96">
+       <h1 id="1ca854ac-bab5-48cf-815e-5e0c4911f945">
         Class
-        <span class="text-primary" id="8623c18f-f8a4-4b8f-a9c0-20c760e4fc47">
+        <span class="text-primary" id="aeefedf7-7bc8-4caf-a0f9-7b75e6b9297f">
          Separator
         </span>
        </h1>
-       <div id="93a77f55-6add-49a2-a160-15b78eb7e289">
+       <div id="b70ac6d0-68e9-4ed7-ac05-af031c8b338a">
        </div>
       </div>
-      <span class="text-muted" id="179a2dbd-dc7e-490e-9552-22f2e50ba54a">
+      <span class="text-muted" id="c0db2f40-0f26-4da9-ae15-70aec696fe70">
        A horizontal line separator.
       </span>
-      <pre id="07d9bd57-8609-4a5c-9dd6-1dd2b49cd7ee"><code class="python">Separator()</code></pre>
-      <div class="ml-3" id="32fe870a-ddac-4bde-8851-b182e478806b">
-       <h6 id="dd90445d-2d3e-4550-bf79-282f8e3c71cc">
+      <pre id="404f1ede-b77c-4f5e-b089-edaff4b7232e"><code class="python">Separator()</code></pre>
+      <div class="ml-3" id="a0abca18-ccc6-42b7-b58e-8c99ab22b613">
+       <h6 id="29959b2c-5f26-488f-adad-57662d309d3c">
         <strong>
          Example
         </strong>
        </h6>
-       <pre id="52b547e3-4d07-403c-b72b-33590eaace87"><code class="python">from bootwrap import Separator, Text
+       <pre id="33f0e2d0-0a71-47f6-b211-a668ece83550"><code class="python">from bootwrap import Panel, Separator, Text
 
-Text("Top Text")
-Separator()
-Text("Bottom Text")</code></pre>
+Panel(
+    Text("Top Text"),
+    Separator(),
+    Text("Bottom Text")
+)
+</code></pre>
       </div>
-      <div class="ml-3" id="c8c0aeb1-c679-422a-af29-7f843d3e947d">
-       <div id="e21f3d23-1519-4d17-859d-658eb4c24194">
-        <span id="a17b3782-56a7-4c5d-b066-6a68d7e09dc7">
+      <div class="ml-3" id="ba268805-357c-493c-8275-777961c41416">
+       <div id="f84f0575-4926-47e9-8b02-e1fb78dfd008">
+        <span id="de14411a-2759-4b11-ae46-1105af57eae0">
          Top Text
         </span>
         <hr/>
-        <span id="8ab01620-8f94-49b1-b5bd-305e086a2479">
+        <span id="3fdddbb8-bd8f-4414-b782-7143f0cf7a34">
          Bottom Text
         </span>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="3dfa68b6-c865-4f48-9383-91ffdadc3312">
-     <div id="0142db8f-6c95-416f-acc4-13dc1be148c6">
+    <div class="tab-pane fade" id="b123cf21-44bd-42fe-97e2-17d6c9e47217">
+     <div id="ca22a283-edec-4edb-a00b-090754df902f">
       <hr/>
-      <ul class="nav" id="3901b22e-229c-4a31-aaa3-246e8ab58d9f" role="tablist">
+      <ul class="nav" id="d2790de2-e821-4b8a-9bf1-b7e61ba1ddd2" role="tablist">
        <li class="nav-item">
-        <a class="nav-link active" data-target="#766c3ebc-978f-4d82-972a-0bdfedb7d9d3" data-toggle="tab" href="#766c3ebc-978f-4d82-972a-0bdfedb7d9d3" id="2023f517-8c09-41d7-bb07-6cbef50ca80c" role="tab">
-         <span class="text-secondary" id="424820f9-8ad5-4280-9757-059ac3901a93">
+        <a class="nav-link active" data-target="#07b6b2fa-87fe-4b36-806b-05cfb8557643" data-toggle="tab" href="#07b6b2fa-87fe-4b36-806b-05cfb8557643" id="ed8eb5fb-3760-4f94-99c2-cd6f77b700ca" role="tab">
+         <span class="text-secondary" id="f00d772f-0205-485c-a830-a21269ebc146">
           Table
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#bd3bcf8c-434c-4d6a-9af3-7c0ba0e06d94" data-toggle="tab" href="#bd3bcf8c-434c-4d6a-9af3-7c0ba0e06d94" id="7bc0682d-a498-49fd-9ad0-df774fa11fb7" role="tab">
-         <span class="text-secondary" id="b2261065-4ae7-4f44-9f6e-de07bd229ef2">
+        <a class="nav-link" data-target="#7b9cafff-ea63-49bd-9b45-e434165dd55f" data-toggle="tab" href="#7b9cafff-ea63-49bd-9b45-e434165dd55f" id="a8cce6e6-629d-48a2-9f8d-240bc3054a68" role="tab">
+         <span class="text-secondary" id="862b3cb3-c849-4eb9-beb6-f25449717d70">
           Table.Head
          </span>
         </a>
        </li>
        <li class="nav-item">
-        <a class="nav-link" data-target="#09054bdb-40f3-4f14-86d9-1d5b40a60d08" data-toggle="tab" href="#09054bdb-40f3-4f14-86d9-1d5b40a60d08" id="8a4ba18a-f897-4808-b748-2564adc0beb5" role="tab">
-         <span class="text-secondary" id="188cf90c-3ace-49bb-93ef-bc2f122ef593">
+        <a class="nav-link" data-target="#b524c283-63f8-43cb-8c2d-408e66c65d8c" data-toggle="tab" href="#b524c283-63f8-43cb-8c2d-408e66c65d8c" id="e388855b-3f81-4c83-90f6-9319560e2027" role="tab">
+         <span class="text-secondary" id="f5d2938f-292c-4311-b81a-dc151c9d17dc">
           Table.Body
          </span>
         </a>
        </li>
       </ul>
       <div class="tab-content">
-       <div class="tab-pane fade active show" id="766c3ebc-978f-4d82-972a-0bdfedb7d9d3">
-        <div class="mt-5" id="93175ff5-84a5-44b3-beb9-c2b380ca682e">
-         <div class="d-flex justify-content-between" id="89f5b268-2cf7-41ad-879e-c4a1e3873276">
-          <h1 id="7f5d6627-20b1-48d6-84c1-79d6e421aa53">
+       <div class="tab-pane fade active show" id="07b6b2fa-87fe-4b36-806b-05cfb8557643">
+        <div class="mt-5" id="5e01d626-276d-414c-bb75-dd38e0c12f78">
+         <div class="d-flex justify-content-between" id="75aec8c1-befe-4481-afe3-74bedd8a5294">
+          <h1 id="1b9dcb1b-b40c-4b81-a685-a4787b5b8cf8">
            Class
-           <span class="text-primary" id="4b4673d8-5109-4a32-9455-433bb963d708">
+           <span class="text-primary" id="880ced6d-6651-46b4-b129-c9e50ba243ec">
             Table
            </span>
           </h1>
-          <div id="74210323-4a4c-4777-ac2f-3b64a9980e51">
-           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#fb774246-cf3a-4db6-9a03-b457049f7cd3" data-toggle="collapse" id="f674b9b1-9dce-4763-880b-8a2680d7408c" onclick="return false;" type="button">
+          <div id="a40080da-66c6-4e29-9d92-d9439e31daca">
+           <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#6acf8f75-81e7-484b-9207-8d9e5716c309" data-toggle="collapse" id="f50154e3-e20d-4f8f-bf9b-16b0226feb16" onclick="return false;" type="button">
             Argument
            </button>
           </div>
          </div>
-         <span class="text-muted" id="1e05eb10-8c27-49e9-9346-18f43ad0e182">
+         <span class="text-muted" id="6f56e01b-d1bb-479e-959e-8d2aacd31550">
           A web component for a table.
          </span>
-         <pre id="f6b3f811-3955-4757-8fc2-bc7c1874a521"><code class="python">Table(head, body)</code></pre>
-         <div class="ml-3 collapse" id="fb774246-cf3a-4db6-9a03-b457049f7cd3">
-          <h6 id="553ab004-4869-4d91-b456-f841557baa77">
+         <pre id="23eb24ff-cb88-4d36-994b-89cfefb873fa"><code class="python">Table(head, body)</code></pre>
+         <div class="ml-3 collapse" id="6acf8f75-81e7-484b-9207-8d9e5716c309">
+          <h6 id="6163ef9a-6ab1-43cb-b4a2-bbb5fa207e01">
            <strong>
             Arguments
            </strong>
           </h6>
-          <table class="table table-sm bg-light" id="2ba604d0-d057-4b58-a1db-f17ab23047a9">
+          <table class="table table-sm bg-light" id="56eef7fe-d602-4db0-9c05-81c7c7afd0d0">
            <thead>
             <tr>
              <th scope="col">
               Name
              </th>
              <th scope="col">
               Type
@@ -6377,33 +6471,34 @@
              <td>
               The table body (2D array).
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <div class="ml-3" id="3b38e916-3bd4-4700-bc71-a95adf21cea9">
-          <h6 id="71d3837f-6f05-4df9-b4af-5798f45ea185">
+         <div class="ml-3" id="448d7730-2992-4fc7-8382-94acaf45a376">
+          <h6 id="66dc8158-9cf1-4c38-a07e-7ba9a62e9339">
            <strong>
             Example
            </strong>
           </h6>
-          <pre id="42ec90da-7d77-4e06-802f-ac7adc8699fa"><code class="python">from bootwrap import Table
+          <pre id="ce9cbb0b-0369-441b-8e74-3c2985f8714b"><code class="python">from bootwrap import Table
 
 Table(
     ["Column 1", "Column 2", "Column 3"],
     [
         ["Value 11", "Value 12", "Value 13"],
         ["Value 21", "Value 22", "Value 23"],
         ["Value 31", "Value 32", "Value 33"],
     ]
-)</code></pre>
+)
+</code></pre>
          </div>
-         <div class="ml-3" id="e6a5604f-2f2b-42e7-8719-d415b295981c">
-          <table class="table" id="8ee51fa6-bfc3-438a-894a-6ec3c07a0b92">
+         <div class="ml-3" id="9badb30f-9b28-4879-805b-856fc506101f">
+          <table class="table" id="528f0ec0-fd8c-4244-b1e6-d8ef6b4e5d0b">
            <thead>
             <tr>
              <th scope="col">
               Column 1
              </th>
              <th scope="col">
               Column 2
@@ -6446,61 +6541,61 @@
              <td>
               Value 33
              </td>
             </tr>
            </tbody>
           </table>
          </div>
-         <div class="mt-5" id="7ffd0d84-d67b-44fd-b630-2b6e2eb9f446">
-          <h4 id="52590438-095e-42e1-9f4f-494e11c4a429">
+         <div class="mt-5" id="7ac872b2-3b8c-400f-a586-bb2827575754">
+          <h4 id="e2d9bf6f-ca35-4bca-a494-f036d65d0f2c">
            Property
-           <span class="text-primary" id="819d787a-1df1-4671-897f-fdfeed4a27b1">
+           <span class="text-primary" id="8e67570c-9562-434d-99ac-21aeb400837b">
             body
            </span>
           </h4>
-          <span class="text-muted" id="52975d5d-b973-4758-8a3f-79c48c2ef1d1">
+          <span class="text-muted" id="e3058937-08a2-45d4-9f4d-da3b1fe2da17">
            The table body.
           </span>
          </div>
-         <div class="mt-5" id="3f9e6d58-b871-4bf4-9f9d-1f16eaa44fcd">
-          <h4 id="a5ad0eac-8547-489a-9dd2-c48bb0c3c8a4">
+         <div class="mt-5" id="b35147f4-2fec-49ad-9226-30888e3b9e04">
+          <h4 id="64662b3e-cf30-4c05-90fe-2da9e34b03b5">
            Property
-           <span class="text-primary" id="c7433d89-7021-4b9d-aa0f-d146230f4ea6">
+           <span class="text-primary" id="b0a6b520-a31f-4b2e-9a3d-34ce25b8fe79">
             head
            </span>
           </h4>
-          <span class="text-muted" id="4223c65e-e875-415e-a5cd-9d1a1594e773">
+          <span class="text-muted" id="638d9cf4-712b-44a5-9395-47a5a7e60a99">
            The table head.
           </span>
          </div>
-         <div class="mt-5" id="e4896475-5d6e-44c2-9726-eda3fb03690b">
-          <div class="d-flex justify-content-between" id="af504a6c-0a59-426a-9978-5023abfbeb3a">
-           <h4 id="d92bd7e7-d664-4d52-a5a2-eca68d23f6dd">
+         <div class="mt-5" id="c27e1c80-6d79-490b-ac77-a29ed3e75fc8">
+          <div class="d-flex justify-content-between" id="8e4952a6-4c0e-4476-b158-e6fc06b9b166">
+           <h4 id="145803a3-6c13-46ee-83ec-bfcfffcb0577">
             Method
-            <span class="text-primary" id="073278a2-dace-491e-b63f-7edc9bd60962">
+            <span class="text-primary" id="e1db310b-d5a1-4ebe-addf-2f13b6ce262d">
              as_bordered
             </span>
            </h4>
-           <div id="775a0b68-122e-49ab-804a-5aa57e553d57">
-            <button class="btn-sm btn btn-outline-primary" data-target="#53ce8aec-de3e-4d44-837a-900452abdf63" data-toggle="collapse" id="0585b563-6666-4f59-bbfc-53d6de348280" onclick="return false;" type="button">
+           <div id="f3e3139a-a24f-4951-8d08-bd21601c22a1">
+            <button class="btn-sm btn btn-outline-primary" data-target="#86b0e6ad-798e-4bf5-bb7e-8c85152df4e5" data-toggle="collapse" id="9e104ff3-2c25-4e0f-b515-c431f2e2dec6" onclick="return false;" type="button">
              Returns
             </button>
            </div>
           </div>
-          <span class="text-muted" id="e58ba32e-590c-4e83-93b2-9c13110c2082">
+          <span class="text-muted" id="3672e1e5-c439-411a-844a-1ccd9db3a8ac">
            Adds borders on all sides of the table and cells.
           </span>
-          <pre id="c25421a1-5f8b-44b6-8c0e-509d1a860510"><code class="python">as_bordered()</code></pre>
-          <div class="ml-3 collapse" id="53ce8aec-de3e-4d44-837a-900452abdf63">
-           <h6 id="97774800-0ba9-45df-a67f-403f021f86a0">
+          <pre id="64f91456-09f9-42c0-9eb5-210d11e7ce4b"><code class="python">as_bordered()</code></pre>
+          <div class="ml-3 collapse" id="86b0e6ad-798e-4bf5-bb7e-8c85152df4e5">
+           <h6 id="c0e3b83b-d857-4d81-b4f0-0f8ef48a6204">
             <strong>
              Returns
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="fbd7ac35-5dfb-4316-ba1e-408a5a1d1773">
+           <table class="table table-sm bg-light" id="0e659ecb-9cc8-41ee-97a3-7a3a305fa027">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -6525,33 +6620,34 @@
               <td>
                The instance of this class.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3" id="40e99068-3fd7-444e-8675-90e628b2d406">
-           <h6 id="8d7bdef0-341b-4b6f-a05d-0a6d476033ef">
+          <div class="ml-3" id="67000025-9d68-4776-a8f1-b51be06ef7c0">
+           <h6 id="c73f2985-8e4a-4e15-a6fe-f4ff0c3e9f52">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="e1dcf515-fafa-4fd4-b965-05d0182a53fa"><code class="python">from bootwrap import Table
+           <pre id="a851ea2e-91e9-44c1-9c5b-ba9ff841a13e"><code class="python">from bootwrap import Table
 
 Table(
     ["Column 1", "Column 2", "Column 3"],
     [
         ["Value 11", "Value 12", "Value 13"],
         ["Value 21", "Value 22", "Value 23"],
         ["Value 31", "Value 32", "Value 33"],
     ]
-).as_bordered()</code></pre>
+).as_bordered()
+</code></pre>
           </div>
-          <div class="ml-3" id="f9fd3287-55d2-490c-b373-ac81c909ef2c">
-           <table class="table table-bordered" id="bede6b15-0e4e-43e7-8267-edf861efca08">
+          <div class="ml-3" id="e114c290-6b24-49c9-ab12-1a8b8496ced4">
+           <table class="table table-bordered" id="283be520-deeb-4645-825d-c5b13a2dfca6">
             <thead>
              <tr>
               <th scope="col">
                Column 1
               </th>
               <th scope="col">
                Column 2
@@ -6595,39 +6691,39 @@
                Value 33
               </td>
              </tr>
             </tbody>
            </table>
           </div>
          </div>
-         <div class="mt-5" id="d0202bc5-ca82-4592-8602-991ce490048c">
-          <div class="d-flex justify-content-between" id="0c3a239d-a8d9-4b4a-86e0-bf73705161d1">
-           <h4 id="ff2ff8be-4e66-4ba6-aee9-368933e952c7">
+         <div class="mt-5" id="7ef14dd6-c0f8-4404-b9e7-8f648e7bffca">
+          <div class="d-flex justify-content-between" id="8a936ec9-2a59-42d1-bc4a-7be84615f183">
+           <h4 id="02da5b61-f6f5-40d0-b520-d710a645bfe1">
             Method
-            <span class="text-primary" id="f3805d2b-8666-4dce-ac07-6f32de2a5a60">
+            <span class="text-primary" id="650ccec3-1437-483d-9d77-ed2c204c7e00">
              as_dark
             </span>
            </h4>
-           <div id="b338755c-2dee-40b6-af06-997c7959b3f1">
-            <button class="btn-sm btn btn-outline-primary" data-target="#002b150e-5502-4d44-a6a5-15a5954906b0" data-toggle="collapse" id="b40290ad-7eb4-4d35-864b-f46f787ab740" onclick="return false;" type="button">
+           <div id="d0c15992-5cfb-4a98-abda-f341af3dd9ff">
+            <button class="btn-sm btn btn-outline-primary" data-target="#5b106cea-41f1-4549-aecc-483fa7453c31" data-toggle="collapse" id="9ea4b14e-10e4-45e6-8ca7-9076138189fb" onclick="return false;" type="button">
              Returns
             </button>
            </div>
           </div>
-          <span class="text-muted" id="1978b367-ff4c-40d7-9a01-a034b173e821">
+          <span class="text-muted" id="f5b4fdd2-1d18-478c-b66d-ce5432a3015c">
            Inverts the colors—with light text on dark backgrounds.
           </span>
-          <pre id="67eb3ab7-4b70-4c5c-942a-50d64f0d78db"><code class="python">as_dark()</code></pre>
-          <div class="ml-3 collapse" id="002b150e-5502-4d44-a6a5-15a5954906b0">
-           <h6 id="547a186c-f3b9-4d19-b2c9-d8648fb001ee">
+          <pre id="909f4fe4-9198-4024-aaa4-1e98033f5a96"><code class="python">as_dark()</code></pre>
+          <div class="ml-3 collapse" id="5b106cea-41f1-4549-aecc-483fa7453c31">
+           <h6 id="c8cb7584-dd0a-494b-92da-df044eb15006">
             <strong>
              Returns
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="8304c468-b22b-4887-9f83-2eb99f0e09ed">
+           <table class="table table-sm bg-light" id="822902cd-8433-4c1f-bc88-a2b3a9f7acb8">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -6652,33 +6748,34 @@
               <td>
                The instance of this class.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3" id="d1612ce7-0424-4951-beff-905fedc74abc">
-           <h6 id="304594ee-c545-4c00-9b40-fcc659cea071">
+          <div class="ml-3" id="7bb163f2-6682-4c68-ad21-db07dd53124d">
+           <h6 id="c65f04cb-9df7-4929-81d8-86afad080f26">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="35011277-a3e0-47ea-a3bf-d4d51526de75"><code class="python">from bootwrap import Table
+           <pre id="15ae512c-5ae4-4028-b2e6-009529c9e069"><code class="python">from bootwrap import Table
 
 Table(
     ["Column 1", "Column 2", "Column 3"],
     [
         ["Value 11", "Value 12", "Value 13"],
         ["Value 21", "Value 22", "Value 23"],
         ["Value 31", "Value 32", "Value 33"],
     ]
-).as_dark()</code></pre>
+).as_dark()
+</code></pre>
           </div>
-          <div class="ml-3" id="e661664b-0c6b-47a5-b279-9a3647bcfc7a">
-           <table class="table table-dark" id="b86cf646-7bb2-4669-b9ad-8e2bf334ade3">
+          <div class="ml-3" id="aa1d6394-6e9d-4f4c-b5d8-a38d90cd0c45">
+           <table class="table table-dark" id="6e5ea714-8e12-4dd5-90e7-23438a0134c3">
             <thead>
              <tr>
               <th scope="col">
                Column 1
               </th>
               <th scope="col">
                Column 2
@@ -6722,42 +6819,42 @@
                Value 33
               </td>
              </tr>
             </tbody>
            </table>
           </div>
          </div>
-         <div class="mt-5" id="5738845a-823e-4022-bf0b-b76fd11d612a">
-          <div class="d-flex justify-content-between" id="4e05bb4d-a55f-48dd-bd3c-5a820e88ee9f">
-           <h4 id="762fe592-d474-4ec2-b892-91e10124bc3a">
+         <div class="mt-5" id="3fc3aa73-803f-43ff-8086-2b92fa80dbd1">
+          <div class="d-flex justify-content-between" id="bcc4e5e9-1a61-47b8-99e1-41c535eeefaa">
+           <h4 id="b4075455-ecf9-48df-82b9-96cb367dea7a">
             Method
-            <span class="text-primary" id="3e7d4279-56a8-40c5-ae5c-5d579ce0887a">
+            <span class="text-primary" id="44d801dd-2e2b-4d61-bd7a-032f624981ed">
              as_responsive
             </span>
            </h4>
-           <div id="dbc6ebc0-fbe5-4f0f-916d-3f0024bd5df9">
-            <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#3d741f8e-9bc9-467e-b110-33a6585cdc02" data-toggle="collapse" id="8e2befe9-6c81-4a64-84ac-146307a50958" onclick="return false;" type="button">
+           <div id="ad4d08aa-2888-4bc9-909e-8d4409c1e49d">
+            <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#28619d11-bc40-43e5-9f0f-287676c4384c" data-toggle="collapse" id="0601dcba-fc86-41a8-a874-cf600fc9e492" onclick="return false;" type="button">
              Argument
             </button>
-            <button class="btn-sm btn btn-outline-primary" data-target="#7501680e-4a41-4f21-beef-f0928acfa460" data-toggle="collapse" id="d26aed18-7a54-48ec-9da7-1b984c58acfc" onclick="return false;" type="button">
+            <button class="btn-sm btn btn-outline-primary" data-target="#20c7219e-924d-419d-a130-c9852e7dbdb9" data-toggle="collapse" id="08e2e11c-a8d9-4891-a0a9-11206bc9cf72" onclick="return false;" type="button">
              Returns
             </button>
            </div>
           </div>
-          <span class="text-muted" id="4e43bf8b-ab2a-49b2-8d26-bb5e5c125983">
+          <span class="text-muted" id="af0fafe6-b013-418e-bc72-a77e4ca52057">
            Create responsive tables.
           </span>
-          <pre id="f888a25f-374e-419a-bc8a-483287bbf42f"><code class="python">as_responsive(breakpoint=<breakpoint.sm: 'sm'="">)</breakpoint.sm:></code></pre>
-          <div class="ml-3 collapse" id="3d741f8e-9bc9-467e-b110-33a6585cdc02">
-           <h6 id="ed38e42e-764d-4bb4-bc9a-9f71bc95bb47">
+          <pre id="11591115-9f1b-44dc-9f65-8391af04bfae"><code class="python">as_responsive(breakpoint=<breakpoint.sm: 'sm'="">)</breakpoint.sm:></code></pre>
+          <div class="ml-3 collapse" id="28619d11-bc40-43e5-9f0f-287676c4384c">
+           <h6 id="7ef463e5-d580-400c-bb1e-0599d8c9a64d">
             <strong>
              Arguments
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="21415b3a-d943-4459-90be-0c79e5eb76e0">
+           <table class="table table-sm bg-light" id="10a39243-4027-4b3a-b47b-d8531947f14a">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -6782,21 +6879,21 @@
               <td>
                The breakpoint to apply.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3 collapse" id="7501680e-4a41-4f21-beef-f0928acfa460">
-           <h6 id="bcff6c99-7324-4f0c-b0b4-407786d00748">
+          <div class="ml-3 collapse" id="20c7219e-924d-419d-a130-c9852e7dbdb9">
+           <h6 id="a133bd31-44ad-4727-ae52-6a81c1cb935a">
             <strong>
              Returns
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="3d6d7205-933e-4995-a393-23b578faa59e">
+           <table class="table table-sm bg-light" id="fbe900c1-0cb4-4910-9361-e2795b9bdde5">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -6821,33 +6918,34 @@
               <td>
                The instance of this class.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3" id="5a8bcf6a-796e-4d95-a16c-d382aa74c30a">
-           <h6 id="bf80ff6c-1499-44f7-87d2-dffe6e8a057d">
+          <div class="ml-3" id="0b0b778c-a785-46a5-be2c-c65dd461cd71">
+           <h6 id="f8d4b60b-6a34-46a3-a4b1-9250c53bcd9d">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="dacfbfef-b6a2-4172-a63a-ccc44bf1f726"><code class="python">from bootwrap import Table
+           <pre id="25469ed7-11e2-44fb-9e4c-b8427db453de"><code class="python">from bootwrap import Table
 
 Table(
     ["Column 1", "Column 2", "Column 3"],
     [
         ["Value 11", "Value 12", "Value 13"],
         ["Value 21", "Value 22", "Value 23"],
         ["Value 31", "Value 32", "Value 33"],
     ]
-).as_responsive()</code></pre>
+).as_responsive()
+</code></pre>
           </div>
-          <div class="ml-3" id="72f19838-c4b3-4c61-9922-2323978a43cb">
-           <table class="table table-responsive-sm" id="fbf26f1b-0dcb-4a84-b8aa-5b5c94723b0b">
+          <div class="ml-3" id="53b54521-9f16-4bd0-81b0-d7fba9c50451">
+           <table class="table table-responsive-sm" id="f6b6ea4a-69d9-4ecd-99e7-a617b9d8b829">
             <thead>
              <tr>
               <th scope="col">
                Column 1
               </th>
               <th scope="col">
                Column 2
@@ -6891,39 +6989,39 @@
                Value 33
               </td>
              </tr>
             </tbody>
            </table>
           </div>
          </div>
-         <div class="mt-5" id="c73d7c7b-b2c7-43a9-8735-6312bb3f6480">
-          <div class="d-flex justify-content-between" id="ae3f0479-6a54-4182-a79f-f176d289a969">
-           <h4 id="f8bbbbd0-f8d9-4b66-a892-2e424329f1d3">
+         <div class="mt-5" id="683c038f-5f5c-4598-bd08-70f782609e52">
+          <div class="d-flex justify-content-between" id="58fcb687-9406-4fe7-ae2b-f7d0cb1e0919">
+           <h4 id="21ca39af-e6e7-48eb-b85a-9da2adbcb156">
             Method
-            <span class="text-primary" id="92e387a8-c19d-4074-9ad1-1f0c5515f143">
+            <span class="text-primary" id="08965d16-bcda-4368-90b6-31366745e730">
              as_small
             </span>
            </h4>
-           <div id="892d1030-bb34-4afc-a9b0-00261c2f9d5d">
-            <button class="btn-sm btn btn-outline-primary" data-target="#77bbb2ae-55ee-474a-9023-b80d614b73ac" data-toggle="collapse" id="21b22f7d-628b-44d3-bd32-6b5463e2f60e" onclick="return false;" type="button">
+           <div id="812c581e-2bd3-4642-b8b7-198f480c2e64">
+            <button class="btn-sm btn btn-outline-primary" data-target="#47b62304-3a70-460b-8357-1f666b7c5f9a" data-toggle="collapse" id="4287e1f7-b379-4ad0-a9d4-c7ae71b90746" onclick="return false;" type="button">
              Returns
             </button>
            </div>
           </div>
-          <span class="text-muted" id="41cdf8f6-4114-467e-aec7-797e56e8f27e">
+          <span class="text-muted" id="0b347ff0-11d4-42f4-aa78-93a26f3d35fb">
            Make tables more compact by cutting cell padding in half.
           </span>
-          <pre id="a4917718-741e-435d-87a1-d40f23c72d2f"><code class="python">as_small()</code></pre>
-          <div class="ml-3 collapse" id="77bbb2ae-55ee-474a-9023-b80d614b73ac">
-           <h6 id="db37abde-873a-4e2c-b785-5f6183d663da">
+          <pre id="ab889aed-b41f-4624-99e4-56517e3fce90"><code class="python">as_small()</code></pre>
+          <div class="ml-3 collapse" id="47b62304-3a70-460b-8357-1f666b7c5f9a">
+           <h6 id="9fca1a27-9669-4a73-8a77-5d5e10d0262a">
             <strong>
              Returns
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="b0f1f03a-b406-48a0-adcd-ca41037f8385">
+           <table class="table table-sm bg-light" id="f73aad7f-2de8-446f-8e08-a3803c3f24aa">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -6948,33 +7046,34 @@
               <td>
                The instance of this class.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3" id="eba08b2f-6a47-4685-a910-fb248880f7da">
-           <h6 id="53d01179-fe88-4a58-ba62-f57a4aa19ea2">
+          <div class="ml-3" id="67a2b7e9-c182-4401-be0b-985247c35ce1">
+           <h6 id="c6a23186-1748-4426-b4fc-e426bb03ee8e">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="aa60b571-263d-4dba-a8fd-bce34aafddbd"><code class="python">from bootwrap import Table
+           <pre id="3d336813-de75-4f16-873a-0be9c0b85eab"><code class="python">from bootwrap import Table
 
 Table(
     ["Column 1", "Column 2", "Column 3"],
     [
         ["Value 11", "Value 12", "Value 13"],
         ["Value 21", "Value 22", "Value 23"],
         ["Value 31", "Value 32", "Value 33"],
     ]
-).as_small()</code></pre>
+).as_small()
+</code></pre>
           </div>
-          <div class="ml-3" id="ccda296b-7636-4f78-b1e1-b83eb250a129">
-           <table class="table table-sm" id="7fcbb26e-9138-4abe-804f-044a3f6c68ba">
+          <div class="ml-3" id="e340cdd7-df95-482f-ba1b-1d71fe172b45">
+           <table class="table table-sm" id="eec6f6f6-c209-41c0-a109-c373093e7c71">
             <thead>
              <tr>
               <th scope="col">
                Column 1
               </th>
               <th scope="col">
                Column 2
@@ -7018,39 +7117,39 @@
                Value 33
               </td>
              </tr>
             </tbody>
            </table>
           </div>
          </div>
-         <div class="mt-5" id="242f780d-82dd-4c43-b4c8-79853636f12d">
-          <div class="d-flex justify-content-between" id="c5d289a0-63f9-42d2-8fda-663ad07b6bbe">
-           <h4 id="6e2b0f69-0312-4e4b-8e59-94f63f6d3dce">
+         <div class="mt-5" id="b9ea064c-6704-47cb-ac94-7ad6873f2271">
+          <div class="d-flex justify-content-between" id="6be47d46-d453-4a1f-afae-ebfd2c88c7be">
+           <h4 id="90f21db9-527b-474f-b940-dc82b3471485">
             Method
-            <span class="text-primary" id="e48c24b5-a02f-44e8-aec4-6a64a1790606">
+            <span class="text-primary" id="13e3c3e5-383a-4c1d-85e7-7e0721822cd6">
              as_striped
             </span>
            </h4>
-           <div id="669fe720-e679-4f59-a95e-eb8cd3e538fe">
-            <button class="btn-sm btn btn-outline-primary" data-target="#a30b4d4a-629f-4da6-b132-13518ca1daab" data-toggle="collapse" id="f71c3367-7a4c-45b7-87e0-e561290165e4" onclick="return false;" type="button">
+           <div id="37829686-be2d-404d-810c-c07dc815556d">
+            <button class="btn-sm btn btn-outline-primary" data-target="#1cc2cc44-5955-432f-8ce3-1f16d8646a17" data-toggle="collapse" id="1faad6ed-08db-4d79-8f23-7a6290ab2125" onclick="return false;" type="button">
              Returns
             </button>
            </div>
           </div>
-          <span class="text-muted" id="6c111dd7-640c-4635-bcd4-3f54129b0f84">
+          <span class="text-muted" id="a85f8ab2-2d17-4400-ba33-c956b2721377">
            Adds zebra-striping to any table row within the table body.
           </span>
-          <pre id="4f85d901-0f65-41f8-ba96-0831a7ef7b1e"><code class="python">as_striped()</code></pre>
-          <div class="ml-3 collapse" id="a30b4d4a-629f-4da6-b132-13518ca1daab">
-           <h6 id="2004fea7-1569-4fa1-9a76-4a562887632e">
+          <pre id="e6283c4f-2195-4e3a-af96-91141cae38e3"><code class="python">as_striped()</code></pre>
+          <div class="ml-3 collapse" id="1cc2cc44-5955-432f-8ce3-1f16d8646a17">
+           <h6 id="f119cf7c-3c2d-4b3c-b3b8-f169c3fc571e">
             <strong>
              Returns
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="e8c90c91-a9b6-4ca6-91a4-139f4a186a97">
+           <table class="table table-sm bg-light" id="b4379378-4657-43bd-bd4b-0c6f81b6bfc5">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -7075,33 +7174,34 @@
               <td>
                The instance of this class.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3" id="86a04abc-1193-49dd-8af1-ca5ff8d208c7">
-           <h6 id="15a078ec-3079-467e-9c33-091b88d29bdc">
+          <div class="ml-3" id="78494823-e51f-4fb8-8dbf-904102395065">
+           <h6 id="0bf4e6f8-e8eb-443d-9069-2c66454bfcd8">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="429862d0-dcd5-4063-b172-709171ce19f6"><code class="python">from bootwrap import Table
+           <pre id="a602b6a0-06d2-4c6d-84e6-2c82d02a881d"><code class="python">from bootwrap import Table
 
 Table(
     ["Column 1", "Column 2", "Column 3"],
     [
         ["Value 11", "Value 12", "Value 13"],
         ["Value 21", "Value 22", "Value 23"],
         ["Value 31", "Value 32", "Value 33"],
     ]
-).as_striped()</code></pre>
+).as_striped()
+</code></pre>
           </div>
-          <div class="ml-3" id="26e0aa50-b261-4c05-a291-8ea9143cfc39">
-           <table class="table table-striped" id="8b63563a-60bb-4af1-b2f8-8c8966c97b50">
+          <div class="ml-3" id="55044214-ce0e-499f-afe7-f382f3d9bfd3">
+           <table class="table table-striped" id="bf3016e6-f28d-454e-89a0-1fe2cefbd90c">
             <thead>
              <tr>
               <th scope="col">
                Column 1
               </th>
               <th scope="col">
                Column 2
@@ -7147,65 +7247,68 @@
              </tr>
             </tbody>
            </table>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="bd3bcf8c-434c-4d6a-9af3-7c0ba0e06d94">
-        <div class="mt-5" id="35570cba-dc3b-47ee-b515-af07900170df">
-         <div class="d-flex justify-content-between" id="d0c9e82c-fe9f-444d-87b8-1eca03bdbab5">
-          <h1 id="018e0774-a0e6-4150-9ad7-67be80df41e6">
+       <div class="tab-pane fade" id="7b9cafff-ea63-49bd-9b45-e434165dd55f">
+        <div class="mt-5" id="6b2d4763-4ce8-4c00-9b34-2ccb1654e4fe">
+         <div class="d-flex justify-content-between" id="c3b79999-430e-4107-90c4-cbb02ff85e7c">
+          <h1 id="805247ea-baf1-4132-a590-c56a37765a7b">
            Class
-           <span class="text-primary" id="528b85b3-c30b-478d-ad80-008139bd9fa6">
+           <span class="text-primary" id="63f9cb0a-6a67-40af-b1c9-119d5bee1612">
             Table.Head
            </span>
           </h1>
-          <div id="38ae1528-1bca-45b3-b566-961df7b52f80">
+          <div id="8cfdfca9-2754-4029-ac7f-2478de292b4a">
           </div>
          </div>
-         <span class="text-muted" id="9591d89f-1f08-4fec-9ea4-9997ddd68979">
+         <span class="text-muted" id="865ef738-cdd3-4db1-ab99-4aa0a01d44a1">
           The table head.
          </span>
-         <pre id="9535575e-fe82-46b8-884a-626e366a8d02"><code class="python">Table.Head(head)</code></pre>
-         <div class="mt-5" id="9edb04f0-19d6-4162-a621-387c4c617310">
-          <div class="d-flex justify-content-between" id="677b98e1-a6db-4d64-979d-32bdf91cc011">
-           <h4 id="cec0f05a-42c8-48e4-9b05-218a98690047">
+         <pre id="c6c738d3-65fd-47c4-9383-31f9fd81c03f"><code class="python">Table.Head(head)</code></pre>
+         <div class="mt-5" id="1eed58c4-a08d-4896-97df-ee311590859b">
+          <div class="d-flex justify-content-between" id="755b1d4c-3c27-4d81-b968-d985e38a213f">
+           <h4 id="8c53370f-bbc7-4fb9-a12c-e899895265d7">
             Method
-            <span class="text-primary" id="ec1edaba-15c2-4669-bdc8-bd02fb85acbc">
+            <span class="text-primary" id="5c06a43a-bb9b-4c20-aac0-1fe8bd8a618f">
              as_dark
             </span>
            </h4>
-           <div id="be3a1d77-b00e-407e-a7a6-a401abb6a5ca">
+           <div id="b06a5f61-b9b8-46da-8856-6f6d6dff4977">
            </div>
           </div>
-          <span class="text-muted" id="f02fa614-955a-4474-924c-d84a8d8bba52">
+          <span class="text-muted" id="875b076c-3789-4e75-a9fd-8d09c2ac22c5">
            Makes the table head appears as dark gray.
           </span>
-          <pre id="025dd9dd-0b58-423d-b80b-d5055efff537"><code class="python">as_dark()</code></pre>
-          <div class="ml-3" id="6188b4aa-8e04-4791-bc6b-7db2f964abbf">
-           <h6 id="f9703598-98e7-4348-a5be-69124898d403">
+          <pre id="5a50ba41-62e7-42bf-847f-8876b35cd681"><code class="python">as_dark()</code></pre>
+          <div class="ml-3" id="599a0288-7d40-4895-bc47-d8c8a3bf41cf">
+           <h6 id="10f08f71-22fd-4a2f-8880-40c809576a78">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="2ec0110f-84a5-4dce-9a86-6596afaf03e6"><code class="python">from bootwrap import Table
+           <pre id="da471920-7ba1-4043-ac0c-0a495b1bfbf1"><code class="python">from bootwrap import Table
 
 table = Table(
     ["Column 1", "Column 2", "Column 3"],
     [
         ["Value 11", "Value 12", "Value 13"],
         ["Value 21", "Value 22", "Value 23"],
         ["Value 31", "Value 32", "Value 33"],
     ]
 )
-table.head.as_dark()</code></pre>
+table.head.as_dark()
+
+table
+</code></pre>
           </div>
-          <div class="ml-3" id="52512ecb-cdfa-4602-9b33-a49d31def0a9">
-           <table class="table" id="5d111edd-78d8-4064-b247-f1d0ab63fb52">
+          <div class="ml-3" id="0c41bc0f-21cb-449d-a694-67aab8ba2376">
+           <table class="table" id="241434f1-60a9-4f21-a238-e018c92d786c">
             <thead class="thead-dark">
              <tr>
               <th scope="col">
                Column 1
               </th>
               <th scope="col">
                Column 2
@@ -7249,49 +7352,52 @@
                Value 33
               </td>
              </tr>
             </tbody>
            </table>
           </div>
          </div>
-         <div class="mt-5" id="b55cab2d-c863-40b8-8b35-3c7acf202855">
-          <div class="d-flex justify-content-between" id="f781ad42-0f41-494c-9e55-d699169b5fc6">
-           <h4 id="24cbc8cf-58c7-46b8-94aa-5fc9732696c4">
+         <div class="mt-5" id="a6f7ae42-0bab-4631-bd4c-e01dfe4c6c4e">
+          <div class="d-flex justify-content-between" id="357a7b43-0d7c-47bb-991c-52fe1a510126">
+           <h4 id="ed76eac5-19e6-4834-a78f-9f3d601a95f2">
             Method
-            <span class="text-primary" id="71fb79ff-b462-4598-ae9b-b6f608c2a50c">
+            <span class="text-primary" id="13b30fdf-58f8-4175-98ab-6196cc94fc30">
              as_light
             </span>
            </h4>
-           <div id="aa3c7900-0b1e-436e-8d2f-e5b037c67a8a">
+           <div id="fadb6dc7-b10d-4c09-a1e8-d233dc95b5c1">
            </div>
           </div>
-          <span class="text-muted" id="4347fc5d-8e5c-4ded-91ed-af1e326bcc3a">
+          <span class="text-muted" id="e74f023e-cc5c-4472-b9df-24ce6bebf078">
            Makes the table head appears as light gray.
           </span>
-          <pre id="8daf74d8-4273-4660-b89a-005cd854afd5"><code class="python">as_light()</code></pre>
-          <div class="ml-3" id="03ace2a5-8f02-4d06-94cf-039608575b25">
-           <h6 id="742a127f-3ac0-44ff-b1b0-1fa58349b657">
+          <pre id="0ee2c425-425d-4754-a218-d7ddd7e3b34a"><code class="python">as_light()</code></pre>
+          <div class="ml-3" id="642abc1d-0ba9-4519-8b09-35527f22338a">
+           <h6 id="d7e15793-be0f-4afc-811f-b83e9d26f6d3">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="78e7bcf8-baa3-4d29-ad2b-8a646652932b"><code class="python">from bootwrap import Table
+           <pre id="34e110dc-f18b-47e1-a7ac-89d97cab3406"><code class="python">from bootwrap import Table
 
 table = Table(
     ["Column 1", "Column 2", "Column 3"],
     [
         ["Value 11", "Value 12", "Value 13"],
         ["Value 21", "Value 22", "Value 23"],
         ["Value 31", "Value 32", "Value 33"],
     ]
 )
-table.head.as_light()</code></pre>
+table.head.as_light()
+
+table
+</code></pre>
           </div>
-          <div class="ml-3" id="e9dd6197-65c6-4a8e-9d58-1b78e2c3f464">
-           <table class="table" id="f1179bd8-3935-41e6-904e-229eb17e6b81">
+          <div class="ml-3" id="103353be-5278-42f5-8cbf-bcba31de62d8">
+           <table class="table" id="87dac225-bd9c-42d3-bbfc-c75ece3f3744">
             <thead class="thead-light">
              <tr>
               <th scope="col">
                Column 1
               </th>
               <th scope="col">
                Column 2
@@ -7337,55 +7443,55 @@
              </tr>
             </tbody>
            </table>
           </div>
          </div>
         </div>
        </div>
-       <div class="tab-pane fade" id="09054bdb-40f3-4f14-86d9-1d5b40a60d08">
-        <div class="mt-5" id="aa7aabf5-97f5-41a8-bf70-caa80772b088">
-         <div class="d-flex justify-content-between" id="55f9b07f-dd25-45e7-a8df-0ae5c891b3b8">
-          <h1 id="6ec3e6bc-2c1a-4ffd-b072-282405277d96">
+       <div class="tab-pane fade" id="b524c283-63f8-43cb-8c2d-408e66c65d8c">
+        <div class="mt-5" id="14848e18-566f-474e-83b0-3cfd60ea5a97">
+         <div class="d-flex justify-content-between" id="9924f48e-d772-424e-a73c-15cf3b4353cb">
+          <h1 id="1f026517-bac2-43bf-8949-b75a7c1a9b1e">
            Class
-           <span class="text-primary" id="4da05177-d940-4c63-af24-c00c2096ac30">
+           <span class="text-primary" id="f62075fe-ccf9-4c18-aecc-36fc9cc4ca96">
             Table.Body
            </span>
           </h1>
-          <div id="83709e68-c445-4d0f-aab0-4f2fd73c0b99">
+          <div id="48940f19-6490-48f8-abcc-4bb8ae0ab00f">
           </div>
          </div>
-         <span class="text-muted" id="f9903f4f-b814-4419-889b-7d79e6ccecc8">
+         <span class="text-muted" id="5e5d83c8-4d3a-4b5b-af29-ef8d0bf6624d">
           The table body.
          </span>
-         <pre id="e7ec7ba4-fb84-4e17-816d-8b5dc41819cc"><code class="python">Table.Body(body)</code></pre>
-         <div class="mt-5" id="20969295-fdd1-4da5-b6b1-85afe8128e00">
-          <div class="d-flex justify-content-between" id="d8761149-1809-4680-82a2-71edf81a8cc6">
-           <h4 id="7ea51cc5-8690-48a0-9be1-5f43d2705810">
+         <pre id="d291fb0c-992f-432f-b785-619991bbba77"><code class="python">Table.Body(body)</code></pre>
+         <div class="mt-5" id="29caccba-4f11-43d1-b152-6988a39d09d1">
+          <div class="d-flex justify-content-between" id="ba7959f6-7163-42c3-b012-3320f15e9283">
+           <h4 id="f632c684-ca38-47e8-bc45-3bd7959569a8">
             Method
-            <span class="text-primary" id="72b54dcf-c359-4312-90de-73688c1459aa">
+            <span class="text-primary" id="d1d5eb57-d615-446d-b4e6-8fecee3648be">
              transform
             </span>
            </h4>
-           <div id="81046422-a902-40f7-9eb5-5606ec723b3a">
-            <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#11d9a021-c685-4870-add6-65dbd9f59277" data-toggle="collapse" id="b2e14a9e-c7a0-4ee8-b5e1-1ed55b10a0c4" onclick="return false;" type="button">
+           <div id="52f83e8f-40fb-4c74-b135-71f8050ded80">
+            <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#86136256-3a05-4766-9de1-3e0569c6000a" data-toggle="collapse" id="36454bdb-84e5-4e64-aa09-478018047884" onclick="return false;" type="button">
              Argument
             </button>
            </div>
           </div>
-          <span class="text-muted" id="f59be339-bffe-4273-9c64-15517119000e">
+          <span class="text-muted" id="2c5658e8-5dcc-4149-b7b3-0575a5bb3a94">
            Defines a function to transform a cell value
           </span>
-          <pre id="b27742f0-0662-425e-922b-bee51b0991d1"><code class="python">transform(index, entity, fn)</code></pre>
-          <div class="ml-3 collapse" id="11d9a021-c685-4870-add6-65dbd9f59277">
-           <h6 id="88364ffd-ae77-49f0-9885-162bf0b2011b">
+          <pre id="d78c5bc9-ed34-4bf5-bb9c-07c1bd1696c7"><code class="python">transform(index, entity, fn)</code></pre>
+          <div class="ml-3 collapse" id="86136256-3a05-4766-9de1-3e0569c6000a">
+           <h6 id="70a6c41a-5803-482e-b868-e167ccb52e58">
             <strong>
              Arguments
             </strong>
            </h6>
-           <table class="table table-sm bg-light" id="ceb6779b-51c7-4f91-b720-9490a440eeb7">
+           <table class="table table-sm bg-light" id="7e0838f2-5154-4c83-bedd-8fd6916013ae">
             <thead>
              <tr>
               <th scope="col">
                Name
               </th>
               <th scope="col">
                Type
@@ -7442,21 +7548,21 @@
               <td>
                The function to use for transformation.
               </td>
              </tr>
             </tbody>
            </table>
           </div>
-          <div class="ml-3" id="26b2bf26-3da2-457a-b303-0705e2bcb7f7">
-           <h6 id="833b2db2-269d-4dc8-8a4c-17380ac10ddc">
+          <div class="ml-3" id="0d3fc4d2-2c3b-4ea2-b136-3d8658c4f306">
+           <h6 id="2ecff6c7-a66b-4f71-ad45-6fcfea6a20ae">
             <strong>
              Example
             </strong>
            </h6>
-           <pre id="91d8c2a6-4407-4dfc-a6a8-69c5fd2c0dca"><code class="python">from bootwrap import Table, TableEntity, Text
+           <pre id="293083c8-fd82-45b1-a509-44f4c7272964"><code class="python">from bootwrap import Table, TableEntity, Text
 
 table = Table(
     ["Column 1", "Column 2", "Column 3"],
     [
         ["val1", "int", "this is a description for val1;"],
         ["val2", "str", "this is a description for val2;"],
         ["val3", "bool", "this is a description for val3;"],
@@ -7474,18 +7580,22 @@
     TableEntity.ROW,
     lambda v: "bg-warning" if v == "val2" else ""
 )
 
 table.body.transform(
     1,
     TableEntity.VALUE,
-    lambda v: f"<code>{v}</code>"</code></pre>
+    lambda v: f"<code>{v}</code>"
+)
+
+table
+</code></pre>
           </div>
-          <div class="ml-3" id="9ba67e2a-846b-4a86-aff4-c7a375e33dd8">
-           <table class="table" id="4fd3c3ba-7220-45ec-9add-1378fb89e79c">
+          <div class="ml-3" id="d2b01c4f-96f5-4ab9-83b4-4f6fe22c3612">
+           <table class="table" id="c2fe5361-fcea-450f-bcc6-f6656c1a1d96">
             <thead>
              <tr>
               <th scope="col">
                Column 1
               </th>
               <th scope="col">
                Column 2
@@ -7540,40 +7650,40 @@
           </div>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="tab-pane fade" id="ea7d5a24-6909-4527-96c9-1333b9dd6d5b">
-     <div class="mt-5" id="fd77ebbc-aca1-4bff-bdb1-e11ff5c47d6f">
-      <div class="d-flex justify-content-between" id="06de22ac-4787-4f3b-9750-4885d0fcff8c">
-       <h1 id="31d10f33-fbdf-4174-bd88-01cac339d750">
+    <div class="tab-pane fade" id="d1653cdc-cb70-47ca-a06f-cfb4fde1e2b3">
+     <div class="mt-5" id="3eb8f591-7b04-4321-8885-460d8b65db14">
+      <div class="d-flex justify-content-between" id="c6867beb-b003-4b47-88fa-e0dc977a87a3">
+       <h1 id="0ba0f41c-da8b-4a5e-a009-5f8cfa5b7fdc">
         Class
-        <span class="text-primary" id="e78f1486-e971-4403-85e8-95b183ef112b">
+        <span class="text-primary" id="c8a1f859-b1a5-4d67-a295-008c2a64faf0">
          Text
         </span>
        </h1>
-       <div id="534eb958-70dc-4678-8888-e93174a41ff6">
-        <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#22320544-a9e7-4d1a-b2b5-7074f8d02aeb" data-toggle="collapse" id="f5f22253-1112-4c37-b442-146e65b7d85a" onclick="return false;" type="button">
+       <div id="61e795d2-1396-4ae8-b378-e7b87d3310ee">
+        <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#0f402af7-9251-4aac-afed-aa13d1947627" data-toggle="collapse" id="062d4738-0f48-46a0-b031-9422f8ce84ad" onclick="return false;" type="button">
          Argument
         </button>
        </div>
       </div>
-      <span class="text-muted" id="a7193a4b-3f98-47de-afbd-91cf13ae4b13">
+      <span class="text-muted" id="bf30edc0-9008-403c-8d75-10c387e24009">
        A web component for a text.
       </span>
-      <pre id="35fb3eed-749c-4bbf-b5d5-ec9408d159b3"><code class="python">Text(content)</code></pre>
-      <div class="ml-3 collapse" id="22320544-a9e7-4d1a-b2b5-7074f8d02aeb">
-       <h6 id="84082ef2-baf7-46ae-b40b-dbf0addddf93">
+      <pre id="d4443e81-edd5-4821-8d6a-b3853033b0e2"><code class="python">Text(content)</code></pre>
+      <div class="ml-3 collapse" id="0f402af7-9251-4aac-afed-aa13d1947627">
+       <h6 id="3233a537-2e0d-439e-88bb-b6a98dba1874">
         <strong>
          Arguments
         </strong>
        </h6>
-       <table class="table table-sm bg-light" id="77d063a7-1652-4e29-9e4d-827147fb7acd">
+       <table class="table table-sm bg-light" id="3bf54b7c-0a83-4754-a349-11dc12994c01">
         <thead>
          <tr>
           <th scope="col">
            Name
           </th>
           <th scope="col">
            Type
@@ -7598,54 +7708,55 @@
           <td>
            The textual content.
           </td>
          </tr>
         </tbody>
        </table>
       </div>
-      <div class="ml-3" id="533430f3-8297-4ff6-99b2-2209efee4ae8">
-       <h6 id="e0f3eb8d-bf3f-4d28-b00e-39485e5fd29f">
+      <div class="ml-3" id="37823772-efd8-44bf-b17b-da7fe1dbf29a">
+       <h6 id="7d983c48-b916-42b2-b5f2-9ed2b0317b5d">
         <strong>
          Example
         </strong>
        </h6>
-       <pre id="03ef8684-26ca-47d9-b177-80c4a4cf86ed"><code class="python">from bootwrap import Text
+       <pre id="514085c1-4277-4eed-8c46-9471f68e5f2c"><code class="python">from bootwrap import Text
 
-Text("Normal text")</code></pre>
+Text("Normal text")
+</code></pre>
       </div>
-      <div class="ml-3" id="8af763b2-8d65-45b1-beef-523af87875e9">
-       <span id="9521180e-bcd5-4d12-9d39-9d7e68a19d3a">
+      <div class="ml-3" id="9ff2c185-8c32-455f-bb62-beccdea7d92c">
+       <span id="3fed6448-dd82-4201-ad3c-18afb1869f36">
         Normal text
        </span>
       </div>
-      <div class="mt-5" id="f55ee016-7b1b-4c72-ab8d-20219dea6d98">
-       <div class="d-flex justify-content-between" id="871d5ea5-04ce-4de7-a40c-90067bcdb64f">
-        <h4 id="7020b244-6d53-4ab0-9fca-834506aa9440">
+      <div class="mt-5" id="8a7966dd-0be2-43df-83a3-01ce7c4c3d46">
+       <div class="d-flex justify-content-between" id="f2a84c23-377b-46fd-bca5-188c4e4a4c17">
+        <h4 id="49b5303e-2584-4ce2-a69c-4fb2331db8aa">
          Method
-         <span class="text-primary" id="2d7ce8c0-b270-4dfc-aef9-f224939bdb97">
+         <span class="text-primary" id="1e71dcee-ca66-492e-8c4a-36713406d4b8">
           as_code
          </span>
         </h4>
-        <div id="b526f1c0-dd5f-4a96-87d9-b51ef26fa195">
-         <button class="btn-sm btn btn-outline-primary" data-target="#b22c5d32-14cf-412f-af7c-a7404a0f5aee" data-toggle="collapse" id="b762d7e6-9686-41a8-9309-2393f4478173" onclick="return false;" type="button">
+        <div id="49139466-ee2c-4479-b8d4-457898929e7f">
+         <button class="btn-sm btn btn-outline-primary" data-target="#0ee28d13-c953-420f-89f4-1e1eeafa2080" data-toggle="collapse" id="ddf3d08b-eacf-4e74-a64b-cb131dbf344f" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="a13685bf-9bd5-41ff-91ef-5dc92954e90f">
+       <span class="text-muted" id="f04af25a-73e6-47e6-9c4b-9dfff2c6c20e">
         Makes the text wrap as a code snippet.
        </span>
-       <pre id="fcedcab6-7319-43fd-b946-8345244b1728"><code class="python">as_code()</code></pre>
-       <div class="ml-3 collapse" id="b22c5d32-14cf-412f-af7c-a7404a0f5aee">
-        <h6 id="2660aa70-718c-411b-b079-432d4dc28a89">
+       <pre id="7bcb1ebf-ec7b-4444-bb0f-50f02701c23b"><code class="python">as_code()</code></pre>
+       <div class="ml-3 collapse" id="0ee28d13-c953-420f-89f4-1e1eeafa2080">
+        <h6 id="c083d40b-df43-414f-8d2c-5f15a71d075a">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="fa826257-b01c-447b-86c2-1fb081991005">
+        <table class="table table-sm bg-light" id="20eadc5b-f49b-47d4-846b-144e79e7270b">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -7670,56 +7781,57 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="649c0ee3-d130-4497-a5df-d087e76bf713">
-        <h6 id="cc623f9d-9635-4416-9219-80a994f06b09">
+       <div class="ml-3" id="d364ef6b-c9ae-4d1b-938a-c29942457339">
+        <h6 id="a8774ad2-aa32-4526-ba44-00df62be576a">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="f71adba7-7bef-4b77-8c44-a0fff750291b"><code class="python">from bootwrap import Text
+        <pre id="6a3aaad7-6ace-459a-9a78-88ec5730a79a"><code class="python">from bootwrap import Panel, Text
 
-Text("print('Hello world!')").as_code()</code></pre>
+Text("print('Hello world!')").as_code()
+</code></pre>
        </div>
-       <div class="ml-3" id="e1bf1e3b-cd71-413f-b314-bdf4654bdf2a">
-        <pre id="72a75a53-20a2-4a2c-b338-1df4cf063859"><code class="python">print('Hello world!')</code></pre>
+       <div class="ml-3" id="188cd254-77e3-438e-a028-94aa5c184112">
+        <pre id="1efafba6-7d17-42e5-a654-37808e05f078"><code class="python">print('Hello world!')</code></pre>
        </div>
       </div>
-      <div class="mt-5" id="cf784132-a026-45a0-a0f1-373f643b46d6">
-       <div class="d-flex justify-content-between" id="ca525a2b-3e36-4dd4-b610-e2ca71ca2f04">
-        <h4 id="75910bfb-986f-4109-b3ab-cc14c787916d">
+      <div class="mt-5" id="28ca5849-4f08-4d68-87b4-393b31961653">
+       <div class="d-flex justify-content-between" id="f6b06dfe-b05f-41f2-9350-dca571abd24d">
+        <h4 id="276f9fa2-7480-4eac-bcf8-40d0f6a78e02">
          Method
-         <span class="text-primary" id="d64da661-ac72-4403-9b93-3750a1b5920d">
+         <span class="text-primary" id="85dcd843-8bff-4ea0-ba87-d67ac8f0f83a">
           as_heading
          </span>
         </h4>
-        <div id="1192bb59-938d-42a0-81b9-63ed2a466e63">
-         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#17bd49bc-cf07-4233-97bf-99801232b89c" data-toggle="collapse" id="eaefc672-6e7c-4a94-84f1-323221b287a2" onclick="return false;" type="button">
+        <div id="912439b9-6e33-44bf-84bb-4d23cc17ee54">
+         <button class="ml-1 mr-1 btn-sm btn btn-outline-primary" data-target="#e185d322-db2a-4a80-8003-475ae758ed16" data-toggle="collapse" id="69892b71-81a6-466e-b969-c283ecebccb9" onclick="return false;" type="button">
           Argument
          </button>
-         <button class="btn-sm btn btn-outline-primary" data-target="#719f4c71-0d30-4724-816e-08700dcbdb15" data-toggle="collapse" id="4726f21f-fcce-4173-8625-06521ac2e56c" onclick="return false;" type="button">
+         <button class="btn-sm btn btn-outline-primary" data-target="#6cadc084-7136-4222-a7fb-75c049eaa16e" data-toggle="collapse" id="3a7ed0cc-4b76-4336-bdda-09f1067a1390" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="f96a8861-b6e5-49f7-a980-0e500f90d3e3">
+       <span class="text-muted" id="a2d77537-cee5-421f-8d5e-ada364f7d72b">
         Makes the text as heading.
        </span>
-       <pre id="6d96e31e-2146-4bce-b9e2-a30c0d82f30e"><code class="python">as_heading(level)</code></pre>
-       <div class="ml-3 collapse" id="17bd49bc-cf07-4233-97bf-99801232b89c">
-        <h6 id="7be0ae13-3bbc-4a1a-9b63-51d1c571d6a9">
+       <pre id="337fc262-c642-4a2c-a757-1e02c5ae2386"><code class="python">as_heading(level)</code></pre>
+       <div class="ml-3 collapse" id="e185d322-db2a-4a80-8003-475ae758ed16">
+        <h6 id="127423a5-a39f-47f3-88f8-a5b706c9ada1">
          <strong>
           Arguments
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="a99f4b1d-2cd8-4df3-8d4a-7f2b39b01ea4">
+        <table class="table table-sm bg-light" id="04931295-b195-48a3-91a3-4ab985411cd3">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -7744,21 +7856,21 @@
            <td>
             The heading level;
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3 collapse" id="719f4c71-0d30-4724-816e-08700dcbdb15">
-        <h6 id="4979fb8f-6afc-4bd9-840c-ddc694465be8">
+       <div class="ml-3 collapse" id="6cadc084-7136-4222-a7fb-75c049eaa16e">
+        <h6 id="69dac425-05b4-4810-98e0-c49e71356ff5">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="ba41ee52-ff15-44f6-a0b4-6581a8e3dd56">
+        <table class="table table-sm bg-light" id="78edec75-53db-41a5-bffb-114dac68422b">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -7783,77 +7895,80 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="90fbb03f-c1b0-4cad-a39b-2327a112708c">
-        <h6 id="e1282d3d-d948-4884-8fee-3532f287cf26">
+       <div class="ml-3" id="2c25da0f-839a-445b-b61c-d7ee6d453fb9">
+        <h6 id="f810f5fe-5fc2-474c-b4fc-036787772db4">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="a21f2783-96ed-44f3-91dd-1c4289a28af9"><code class="python">from bootwrap import Text
+        <pre id="7a39d9d5-9130-44e2-8b91-e84b822eacf5"><code class="python">from bootwrap import Panel, Text
 
-Text("Header text 1").as_heading(1)
-Text("Header text 2").as_heading(2)
-Text("Header text 3").as_heading(3)
-Text("Header text 4").as_heading(4)
-Text("Header text 5").as_heading(5)
-Text("Header text 6").as_heading(6)</code></pre>
-       </div>
-       <div class="ml-3" id="46e4cc56-dec3-48a2-9e3e-04028e4036ac">
-        <div id="61fc59ff-e21a-40cb-acbf-e53ca5797bd4">
-         <h1 id="e40c01a3-7a8f-4f58-997f-8141286c2d65">
+Panel(
+    Text("Header text 1").as_heading(1),
+    Text("Header text 2").as_heading(2),
+    Text("Header text 3").as_heading(3),
+    Text("Header text 4").as_heading(4),
+    Text("Header text 5").as_heading(5),
+    Text("Header text 6").as_heading(6)
+)
+</code></pre>
+       </div>
+       <div class="ml-3" id="a8700806-b5bb-4755-83a8-a8c6bf0de804">
+        <div id="fc8bef28-b080-46a0-82b1-b74af76b6200">
+         <h1 id="24cafa38-2134-4904-9272-6e00916253e8">
           Header text 1
          </h1>
-         <h2 id="a327f434-ae81-4902-837a-4dd427811fa8">
+         <h2 id="9ad2b8be-7103-47c3-9257-34d5febe3a3b">
           Header text 2
          </h2>
-         <h3 id="318c85bf-c528-474f-a331-aa572f876151">
+         <h3 id="71286885-ea0e-4667-9440-631f8d1c1e7f">
           Header text 3
          </h3>
-         <h4 id="39b6514e-0a99-43c2-a707-a872fcd3691e">
+         <h4 id="6dcdd705-05f4-459d-b961-9b94c796e6d3">
           Header text 4
          </h4>
-         <h5 id="42a424a4-279e-4775-abb6-2bb6fca600d7">
+         <h5 id="b06e4010-a0b9-43ef-83eb-d8e8347f7fac">
           Header text 5
          </h5>
-         <h6 id="ba588325-ab49-43e0-9d6a-39477438cd4d">
+         <h6 id="02a63a56-4828-41e2-833a-d360534cf123">
           Header text 6
          </h6>
         </div>
        </div>
       </div>
-      <div class="mt-5" id="eb603041-c7bc-46bb-8b6b-2c3928467058">
-       <div class="d-flex justify-content-between" id="f8c267a2-f7ca-4e8a-b6fb-3e42574f2467">
-        <h4 id="f88238e2-96c4-4b4c-93c2-8c8012602201">
+      <div class="mt-5" id="bc9fd717-1676-4354-91fe-3b12373746e8">
+       <div class="d-flex justify-content-between" id="b10b65bf-417c-450f-8e24-52a4f28e0ceb">
+        <h4 id="6a41f63d-1b65-45e2-a3af-fa0c1c1a23b1">
          Method
-         <span class="text-primary" id="ff1ab0bd-5dbf-423f-8f4c-a7b917da8095">
+         <span class="text-primary" id="63e9021c-bc6a-4572-bbe6-e02e197808d9">
           as_muted
          </span>
         </h4>
-        <div id="9057e112-ef0d-4830-bbb2-3415f808130c">
-         <button class="btn-sm btn btn-outline-primary" data-target="#2bb09abd-d4de-44c7-aa66-daad150ae618" data-toggle="collapse" id="b8009737-1665-451d-872d-676120f90002" onclick="return false;" type="button">
+        <div id="a900724b-cae0-4c49-8385-e3564f528f13">
+         <button class="btn-sm btn btn-outline-primary" data-target="#0e6c21d6-3430-432d-8b74-8e3da3678942" data-toggle="collapse" id="bb1345fe-b9d4-440d-ae8d-5a8c9764019b" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="14238cc5-4984-4850-82b4-162fbb55bb1e">
+       <span class="text-muted" id="4881f5ce-e982-444d-b178-9ccaf2c6994e">
         Makes the text muted.
        </span>
-       <pre id="602207d2-c9a9-4c4f-b730-eb1cf973ddbd"><code class="python">as_muted()</code></pre>
-       <div class="ml-3 collapse" id="2bb09abd-d4de-44c7-aa66-daad150ae618">
-        <h6 id="70931bb0-15a7-448d-a14a-d3a877d814f9">
+       <pre id="4f97cfe2-b99c-47f0-8ab1-07b433c08953"><code class="python">as_muted()</code></pre>
+       <div class="ml-3 collapse" id="0e6c21d6-3430-432d-8b74-8e3da3678942">
+        <h6 id="b5eedbbe-30cb-4fa2-8df3-5d5d5d7cca93">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="9f9a3460-00af-43a2-8eb0-85bd539064c5">
+        <table class="table table-sm bg-light" id="ad298b98-43b9-4c81-a31a-acfded1a702a">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -7878,55 +7993,56 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="19f6fc5c-3139-4b7d-95f6-7a57f1a4380c">
-        <h6 id="8e6dd3e0-725a-49f7-8937-6d7870d5e742">
+       <div class="ml-3" id="2c0a3828-6ca1-4d92-b0c2-937deed302a0">
+        <h6 id="93ddb1b2-5ea8-4537-9853-7952d13d3adc">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="8785580e-bd0e-4d9f-ab60-6d1d73b936ea"><code class="python">from bootwrap import Text
+        <pre id="005aa174-145c-428c-a5e2-8f9ea8664d3c"><code class="python">from bootwrap import Text
 
-Text("Muted text").as_muted()</code></pre>
+Text("Muted text").as_muted()
+</code></pre>
        </div>
-       <div class="ml-3" id="128123db-eb1f-47bd-8adb-6b70eb63472c">
-        <span class="text-muted" id="bef64452-9994-42ec-ada0-c64b85526791">
+       <div class="ml-3" id="15605e65-8fe9-4381-9152-ef3347a81795">
+        <span class="text-muted" id="64837071-d2f8-4ccc-a677-bb3d6a9bae05">
          Muted text
         </span>
        </div>
       </div>
-      <div class="mt-5" id="60a82318-5775-41a8-9d0c-6dd1539edf0a">
-       <div class="d-flex justify-content-between" id="2a18df2a-045b-4337-b086-47411c0bbf60">
-        <h4 id="845aa4e6-e902-4fc0-84e3-e28534e0b040">
+      <div class="mt-5" id="53d7fde7-adea-4770-8b01-7567daf999c0">
+       <div class="d-flex justify-content-between" id="34195980-34c1-4c75-a991-fabf97067dd8">
+        <h4 id="5bd30e5e-1b1a-43d8-a29f-69eaa980f1dc">
          Method
-         <span class="text-primary" id="5045f7b1-043f-4209-a662-fc4680e15762">
+         <span class="text-primary" id="46041fcd-632b-445b-8e94-a88021b60f14">
           as_paragraph
          </span>
         </h4>
-        <div id="f77434c0-bba4-4a79-81b7-03913b24e455">
-         <button class="btn-sm btn btn-outline-primary" data-target="#2e8000b6-4dc6-4618-b0f7-9b277cbc7cfb" data-toggle="collapse" id="fedc9f84-6894-4182-ac6c-4e6ade053a15" onclick="return false;" type="button">
+        <div id="ffc890c3-b441-47ec-8e1a-09d24b85fcae">
+         <button class="btn-sm btn btn-outline-primary" data-target="#8ff23104-5c26-4b2d-a85f-c037f3f473c5" data-toggle="collapse" id="3c9bcdd4-673c-4311-b59a-1279ae27f72f" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="270b9dd8-5815-4d4a-a948-56eab30895ac">
+       <span class="text-muted" id="04e0510a-8918-413b-b841-61a9c69766b2">
         Makes the text wrap in a paragraph.
        </span>
-       <pre id="f955068e-fce8-4963-bb3b-674fb5acf6dc"><code class="python">as_paragraph()</code></pre>
-       <div class="ml-3 collapse" id="2e8000b6-4dc6-4618-b0f7-9b277cbc7cfb">
-        <h6 id="06c5405f-94b4-4118-aa37-7f30c8909f5b">
+       <pre id="9f3ba716-1fe4-475b-86f7-cd060ead8019"><code class="python">as_paragraph()</code></pre>
+       <div class="ml-3 collapse" id="8ff23104-5c26-4b2d-a85f-c037f3f473c5">
+        <h6 id="7872f307-4329-4f85-9657-63bd75018db9">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="8d30940f-8067-4dbb-9973-f3e17336639c">
+        <table class="table table-sm bg-light" id="f63318b2-d7a6-40fc-81dc-d5d9c653b3d2">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -7951,65 +8067,68 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="25b0fe0c-4366-4a37-b409-315efe99c4e6">
-        <h6 id="7511ba96-7a5f-4539-abf1-4b9c7e76e9f0">
+       <div class="ml-3" id="a0427006-8017-4abb-ba51-774e17421e9e">
+        <h6 id="3d920510-d79d-4443-93ee-708086f27a64">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="ed66715b-572e-49ac-80ca-2f59443f1a40"><code class="python">from bootwrap import Text
+        <pre id="4c4188f7-0a3b-4cda-a31c-387e3b10aa30"><code class="python">from bootwrap import Panel, Text
 
-Text("Paragraph 1").as_paragraph()
-Text("Paragraph 2").as_paragraph()
-Text("Paragraph 3").as_paragraph()</code></pre>
-       </div>
-       <div class="ml-3" id="15c5a0dd-0173-4cec-b364-664d5330dfc0">
-        <div id="9f2436b2-742c-4596-a675-220002d92033">
-         <p id="7475453e-724e-4bfa-9a4b-407dc74c74c3">
+Panel(
+    Text("Paragraph 1").as_paragraph(),
+    Text("Paragraph 2").as_paragraph(),
+    Text("Paragraph 3").as_paragraph()
+)
+</code></pre>
+       </div>
+       <div class="ml-3" id="e51d675d-b83b-4358-acfb-95e5cea254c3">
+        <div id="88acc6df-539b-4b24-bc53-599a0b0f7340">
+         <p id="3c4f6f81-9594-49eb-b082-1d81be15b3e3">
           Paragraph 1
          </p>
-         <p id="2ac4b0ea-2936-48a3-928a-6a803994a768">
+         <p id="5ec49445-8764-4514-855f-2c8b7f4ac708">
           Paragraph 2
          </p>
-         <p id="5f999419-0a27-4535-8de5-e39dc071c9ad">
+         <p id="1f5ccd89-4aa6-4f8c-9690-d805eb938a56">
           Paragraph 3
          </p>
         </div>
        </div>
       </div>
-      <div class="mt-5" id="d1cfacdf-ab44-41d8-97a2-9a7f3a79a210">
-       <div class="d-flex justify-content-between" id="8803794d-ed11-423f-a37b-16a90af4600a">
-        <h4 id="3c5be739-d205-48b5-9e62-847ad764a402">
+      <div class="mt-5" id="7ab27574-aa70-4508-928c-e5f1a2da3042">
+       <div class="d-flex justify-content-between" id="02fdeedb-eddd-4cde-9b55-c6f669d00ff7">
+        <h4 id="2923cfa1-0532-44db-b0e8-2d8b87e143ef">
          Method
-         <span class="text-primary" id="b462abf0-05d1-48ae-b798-f40228901abf">
+         <span class="text-primary" id="3be02288-2c75-4363-8cfc-715ca5db4216">
           as_small
          </span>
         </h4>
-        <div id="5f559b4d-e49b-41a7-81fa-98eb19c31fca">
-         <button class="btn-sm btn btn-outline-primary" data-target="#dbdf33e8-8a85-4235-afc2-24a4c13a217e" data-toggle="collapse" id="d35283c6-cd6a-4433-b975-710dd2096ad2" onclick="return false;" type="button">
+        <div id="95515e3e-f60c-411c-99b0-3e3892fd84e8">
+         <button class="btn-sm btn btn-outline-primary" data-target="#584c61af-b241-40db-93cb-4153e40b5ead" data-toggle="collapse" id="1ba959bf-9fc5-4758-89ea-04148e962695" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="0a72cace-627f-46dd-9515-8dd2a7345f46">
+       <span class="text-muted" id="2e24b84e-796e-446e-ad5d-4934d1d6987b">
         Makes the text as small.
        </span>
-       <pre id="364739dc-7de0-4a78-831a-4aebead3de3a"><code class="python">as_small()</code></pre>
-       <div class="ml-3 collapse" id="dbdf33e8-8a85-4235-afc2-24a4c13a217e">
-        <h6 id="308313eb-1de1-471c-9afe-17d1c7b44def">
+       <pre id="bf699b3a-8bea-400b-9210-43c43b3a759e"><code class="python">as_small()</code></pre>
+       <div class="ml-3 collapse" id="584c61af-b241-40db-93cb-4153e40b5ead">
+        <h6 id="5ef613cf-8415-44d7-bf90-b98f9cdf060f">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="1afeccf7-186d-4d7a-a5b1-4d8c209534e3">
+        <table class="table table-sm bg-light" id="06de4fb4-2e27-4792-b335-bfeb84ac6b4f">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -8034,57 +8153,58 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="2b2f1366-ea39-405a-a229-214d68499011">
-        <h6 id="5fbec913-e4e5-4039-b5db-c753f840676b">
+       <div class="ml-3" id="33bd7022-67b3-4891-bc07-08d20f16bc9a">
+        <h6 id="eca4a650-2857-45ab-bb9e-b72aedd1c30f">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="9aa65604-6c29-4c47-88f6-f98b93f378f1"><code class="python">from bootwrap import Text
+        <pre id="0b129563-9910-482f-be74-78195f16d40e"><code class="python">from bootwrap import Text
 
-Text("Small text").as_small()</code></pre>
+Text("Small text").as_small()
+</code></pre>
        </div>
-       <div class="ml-3" id="3a4842bb-9d0e-498b-9e3a-8fa11fbfcb12">
-        <span id="8d91d060-071c-4325-b4c2-26ec5e0b26d3">
+       <div class="ml-3" id="cd2409cb-e07c-46ba-8047-55e9c384ec18">
+        <span id="56d47d66-e242-4439-8cec-28c248b61768">
          <small>
           Small text
          </small>
         </span>
        </div>
       </div>
-      <div class="mt-5" id="7da2ee65-35e8-4140-8c0a-de17f7f8ae93">
-       <div class="d-flex justify-content-between" id="a31b2abe-a4fe-4ce3-97d7-6ff4ad912ab5">
-        <h4 id="8701af3e-00ba-4364-9bfb-334221f531eb">
+      <div class="mt-5" id="908dcd6e-1857-4c8a-808a-6dce2d906166">
+       <div class="d-flex justify-content-between" id="8b7388bd-9a96-4ebd-b7b4-2fb27556adca">
+        <h4 id="b549f537-672d-421a-8b4f-8713b608bf39">
          Method
-         <span class="text-primary" id="222a177c-c693-42e1-b456-9454ca2c313a">
+         <span class="text-primary" id="cdd09ac1-72e5-4eb7-94ef-edd6ffdecf04">
           as_strong
          </span>
         </h4>
-        <div id="f86c11ce-8dd8-4f00-81e4-f31129df14c7">
-         <button class="btn-sm btn btn-outline-primary" data-target="#96bb0d15-836f-4a0d-8bb7-d3513cc4d0dd" data-toggle="collapse" id="88c08edd-f78a-4e12-a403-613aae18fa90" onclick="return false;" type="button">
+        <div id="17b33eb6-664b-43d3-bc2a-bf57be042b2c">
+         <button class="btn-sm btn btn-outline-primary" data-target="#b2e2e464-450b-4490-9b2a-c3d5ef8c8efe" data-toggle="collapse" id="63eb2f4e-77ad-4b3a-af82-d847326fbe9a" onclick="return false;" type="button">
           Returns
          </button>
         </div>
        </div>
-       <span class="text-muted" id="9a37beae-93ef-4093-80eb-a3d09d69f8b0">
+       <span class="text-muted" id="356ab50d-20c7-4e28-8236-0aaf3e4a3591">
         Makes the text as strong.
        </span>
-       <pre id="941f43a9-c6b2-4b14-8b9f-75ad6e78b892"><code class="python">as_strong()</code></pre>
-       <div class="ml-3 collapse" id="96bb0d15-836f-4a0d-8bb7-d3513cc4d0dd">
-        <h6 id="f5695418-73e8-40ab-96ed-e1468052bade">
+       <pre id="5b89662a-71d3-4443-b88b-946039aaeca2"><code class="python">as_strong()</code></pre>
+       <div class="ml-3 collapse" id="b2e2e464-450b-4490-9b2a-c3d5ef8c8efe">
+        <h6 id="a5d6c0ce-b78c-4ccb-b716-277f3b090619">
          <strong>
           Returns
          </strong>
         </h6>
-        <table class="table table-sm bg-light" id="2ee2c276-ddec-4e76-b966-d86ea9017fd8">
+        <table class="table table-sm bg-light" id="82487310-f5a9-419b-8481-167294cbd9a5">
          <thead>
           <tr>
            <th scope="col">
             Name
            </th>
            <th scope="col">
             Type
@@ -8109,34 +8229,38 @@
            <td>
             The instance of this class.
            </td>
           </tr>
          </tbody>
         </table>
        </div>
-       <div class="ml-3" id="6452b54a-6267-4230-9df1-cfeaa7f30fa3">
-        <h6 id="e8718cde-ddbb-40cd-a378-3fadc77c6c77">
+       <div class="ml-3" id="847c6977-49d2-460c-ba0a-fcf4a31b523f">
+        <h6 id="cded2aa6-21ef-4d0b-9e62-92799d2caee8">
          <strong>
           Example
          </strong>
         </h6>
-        <pre id="cdea0a5a-86d2-43c2-8419-561b43eeb601"><code class="python">from bootwrap import Text
+        <pre id="da6f57dd-260a-4959-be56-de3f03d1318c"><code class="python">from bootwrap import Text
 
-Text("Strong text").as_strong()</code></pre>
+Text("Strong text").as_strong()
+</code></pre>
        </div>
-       <div class="ml-3" id="0eb32a75-1ab8-4012-b503-e8e02327429b">
-        <span id="30d21ed0-b8bf-4114-9029-4a8dab2fef29">
+       <div class="ml-3" id="475d8091-fa10-4e0e-bf5b-82bc3cc33ac4">
+        <span id="0c9eefdb-d4ca-479c-bb3b-1d2a3018d0f4">
          <strong>
           Strong text
          </strong>
         </span>
        </div>
       </div>
      </div>
     </div>
    </div>
   </div>
  </body>
  <script>
   hljs.initHighlightingOnLoad();
  </script>
+ <style>
+  :root{--container-margin-top: 90px}html{  width: 100%;  height: 100%; }  body{  background-color: var(--body-background-color);  background-image: var(--body-background-image);  background-position: var(--body-background-position);  background-size: var(--body-background-size);  -webkit-background-size: var(--body-background-size);  -moz-background-size: var(--body-background-size);  -o-background-size: var(--body-background-size);  background-repeat: var(--body-background-repeat);  background-origin: var(--body-background-origin);  background-clip: var(--body-background-clip);  background-attachment: var(--body-background-attachment); }  .container-fluid{  margin-top: var(--container-margin-top); }  .auth{  width: 400px;  margin-top: 150px }  @media only screen and (max-width: 420px){  body{  background-image: none;  }   .auth{  width: 100%;  margin-top: 0px  } }  .grid-container {  display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); }  .card {  margin-top: 10px; }
+ </style>
 </html>
```

#### html2text {}

```diff
@@ -35,91 +35,116 @@
 NNaammee  TTyyppee             DDeessccrriippttiioonn
 inner str|WebComponent The object wrapped by the anchor.
 The Anchor component is used for creating a hyperlink to pages, files, email
 addresses, locations on the same page, or other web-resources defined by a URL
 address. The Bootwrap also uses the Anchor in conjunction with other
 components, for example, in creating a navigation menu.
 ** EExxaammppllee **
+from bootwrap import Anchor
 Anchor('Google Search').link('https://www.google.com/')
 _G_o_o_g_l_e_ _S_e_a_r_c_h
 ************ AAppppeeaarraannccee ************
 Change Anchor appearance using the following functions as_primary() ,
 as_secondary() , as_success() , as_warning() , as_danger() , as_info() ,
 as_light() , and as_dark() .
-Anchor("Primary").as_primary()
-Anchor("Secondary").as_secondary()
-Anchor("Success").as_success()
-Anchor("Warning").as_warning()
-Anchor("Danger").as_danger()
-Anchor("Info").as_info()
-Anchor("Light").as_light()
-Anchor("Dark").as_dark()
+from bootwrap import Panel, Anchor
+panel = Panel(
+  Anchor("Primary").link("#").as_primary(),
+  Anchor("Secondary").link("#").as_secondary(),
+  Anchor("Success").link("#").as_success(),
+  Anchor("Warning").link("#").as_warning(),
+  Anchor("Danger").link("#").as_danger(),
+  Anchor("Info").link("#").as_info(),
+  Anchor("Light").link("#").as_light(),
+  Anchor("Dark").link("#").as_dark()
+)
+for anchor in panel:
+  anchor.mb(1)
+panel
 _P_r_i_m_a_r_y_ _S_e_c_o_n_d_a_r_y_ _S_u_c_c_e_s_s_ _W_a_r_n_i_n_g_ _D_a_n_g_e_r_ _I_n_f_o_ _L_i_g_h_t_ _D_a_r_k
 ************ LLiinnkk RReessoouurrccee ************
 Associate Anchor with a hyperlink using the link() function.
-Anchor("Google Search").link("https://www.google.com/")
+from bootwrap import Panel, Anchor
+Panel(
+    Anchor("Google Search").link("https://www.google.com/")
+)
 _G_o_o_g_l_e_ _S_e_a_r_c_h
 ************ OOppeenn DDiiaalloogg ************
 Use Anchor to open a dialog using the toggle() function.
+from bootwrap import Panel, Dialog, Anchor
 dialog = Dialog(
   "Greeting",
   "Hello World!"
 )
 anchor = Anchor("Say Hello").toggle(dialog)
+Panel(dialog, anchor)
 **** GGrreeeettiinngg ****
 ×
 Hello World!
 _S_a_y_ _H_e_l_l_o
 ************ CClloossee DDiiaalloogg ************
 Use Anchor to close a dialog using the dismiss() function.
+from bootwrap import Panel, Dialog, Anchor
 dialog = Dialog(
   "Greeting",
   "Hello World!",
   Anchor("Bye").dismiss()
 )
 anchor = Anchor("Say Hello").toggle(dialog)
+Panel(dialog, anchor)
 **** GGrreeeettiinngg ****
 ×
 Hello World!
 _B_y_e
 _S_a_y_ _H_e_l_l_o
 ************ EExxppaanndd//CCoollllaappssee PPaanneell ************
 Use Anchor to expand/collapse a panel using the toggle() function.
+from bootwrap import Panel, Anchor
 quote = Panel(
   "Sometimes life is going to hit you in " +
   "the head with a brick. Don’t lose faith."
 ).as_collapse()
-Anchor("Steve Jobs Quote").toggle(quote)
+Panel(
+  Anchor("Steve Jobs Quote").toggle(quote),
+  quote
+)
 _S_t_e_v_e_ _J_o_b_s_ _Q_u_o_t_e
 Sometimes life is going to hit you in the head with a brick. Don’t lose faith.
 ===============================================================================
     * _B_a_d_g_e
     * _A_p_p_e_a_r_a_n_c_e
 ************ CCllaassss BBaaddggee ************
 Argument
 A web component for a badge.
 Badge(label)
 ** AArrgguummeennttss **
 NNaammee  TTyyppee DDeessccrriippttiioonn
 label str  The badge label (text showing inside a badge).
 ** EExxaammppllee **
+from bootwrap import Badge
 Badge('Some Badge')
 Some Badge
 ************ AAppppeeaarraannccee ************
 Change Badge appearance using the following functions as_primary() ,
 as_secondary() , as_success() , as_warning() , as_danger() , as_info() ,
 as_light() , and as_dark() .
-Badge("Primary").as_primary()
-Badge("Secondary").as_secondary()
-Badge("Success").as_success()
-Badge("Warning").as_warning()
-Badge("Danger").as_danger()
-Badge("Info").as_info()
-Badge("Light").as_light()
-Badge("Dark").as_dark()
+from bootwrap import Panel, Badge
+panel = Panel(
+  Badge("Primary").as_primary(),
+  Badge("Secondary").as_secondary(),
+  Badge("Success").as_success(),
+  Badge("Warning").as_warning(),
+  Badge("Danger").as_danger(),
+  Badge("Info").as_info(),
+  Badge("Light").as_light(),
+  Badge("Dark").as_dark()
+)
+for anchor in panel:
+  anchor.mb(1)
+panel
 Primary Secondary Success Warning Danger Info Light Dark
 ===============================================================================
     * _B_u_t_t_o_n
     * _A_p_p_e_a_r_a_n_c_e
     * _O_u_t_l_i_n_e
     * _D_i_s_a_b_l_e
     * _L_i_n_k_ _R_e_s_o_u_r_c_e
@@ -133,90 +158,118 @@
 Button(name)
 ** AArrgguummeennttss **
 NNaammee TTyyppee DDeessccrriippttiioonn
 name str  The button name.
 Without applying a stylized method Button will be appearing very similar to the
 Anchor .
 ** EExxaammppllee **
+from bootwrap import Button
 Button('Google Search').link('https://www.google.com/')
 _G_o_o_g_l_e_ _S_e_a_r_c_h
 ************ AAppppeeaarraannccee ************
 Change Button appearance using the following functions as_primary() ,
 as_secondary() , as_success() , as_warning() , as_danger() , as_info() ,
 as_light() , and as_dark() .
-Button("Primary").as_primary()
-Button("Secondary").as_secondary()
-Button("Success").as_success()
-Button("Warning").as_warning()
-Button("Danger").as_danger()
-Button("Info").as_info()
-Button("Light").as_light()
-Button("Dark").as_dark()
+from bootwrap import Panel, Button
+panel = Panel(
+  Button("Primary").link("#").as_primary(),
+  Button("Secondary").link("#").as_secondary(),
+  Button("Success").link("#").as_success(),
+  Button("Warning").link("#").as_warning(),
+  Button("Danger").link("#").as_danger(),
+  Button("Info").link("#").as_info(),
+  Button("Light").link("#").as_light(),
+  Button("Dark").link("#").as_dark()
+)
+for anchor in panel:
+  anchor.mb(1)
+panel
 _P_r_i_m_a_r_y_ _S_e_c_o_n_d_a_r_y_ _S_u_c_c_e_s_s_ _W_a_r_n_i_n_g_ _D_a_n_g_e_r_ _I_n_f_o_ _L_i_g_h_t_ _D_a_r_k
 ************ OOuuttlliinnee ************
 Make Button without filling with surrounded by color border using the following
 function as primary() .
-Button("Primary").as_primary().as_outline()
-Button("Secondary").as_secondary().as_outline()
-Button("Success").as_success().as_outline()
-Button("Warning").as_warning().as_outline()
-Button("Danger").as_danger().as_outline()
-Button("Info").as_info().as_outline()
-Button("Light").as_light().as_outline()
-Button("Dark").as_dark().as_outline()
+from bootwrap import Panel, Button
+panel = Panel(
+  Button("Primary").link("#").as_primary().as_outline(),
+  Button("Secondary").link("#").as_secondary().as_outline(),
+  Button("Success").link("#").as_success().as_outline(),
+  Button("Warning").link("#").as_warning().as_outline(),
+  Button("Danger").link("#").as_danger().as_outline(),
+  Button("Info").link("#").as_info().as_outline(),
+  Button("Light").link("#").as_light().as_outline(),
+  Button("Dark").link("#").as_dark().as_outline()
+)
+for anchor in panel:
+  anchor.mb(1)
+panel
 _P_r_i_m_a_r_y_ _S_e_c_o_n_d_a_r_y_ _S_u_c_c_e_s_s_ _W_a_r_n_i_n_g_ _D_a_n_g_e_r_ _I_n_f_o_ _L_i_g_h_t_ _D_a_r_k
 ************ DDiissaabbllee ************
 But default the Button always enabled. Use the as_disabled() function to make
 the Button disabled. Disable status prevent user to initiate any action
 assigned to the Button .
-Button("Enabled").as_primary()
-Button("Disabled").as_primary().as_disabled()
+from bootwrap import Panel, Button
+Panel(
+  Button("Enabled").as_primary(),
+  Button("Disabled").as_primary().as_disabled()
+)
 Enabled Disabled
 ************ LLiinnkk RReessoouurrccee ************
 Associate Button with a hyperlink using the link() function.
-Button("Google Search").as_primary().link("https://www.google.com/")
+from bootwrap import Panel, Button
+Panel(
+    Button("Google Search").as_primary().link("https://www.google.com/")
+)
 _G_o_o_g_l_e_ _S_e_a_r_c_h
 ************ OOppeenn DDiiaalloogg ************
 Use Button to open a dialog using the toggle() function.
+from bootwrap import Panel, Dialog, Button
 dialog = Dialog(
   "Greeting",
   "Hello World!"
 )
 button = Button("Say Hello").as_primary().toggle(dialog)
+Panel(dialog, button)
 **** GGrreeeettiinngg ****
 ×
 Hello World!
 Say Hello
 ************ CClloossee DDiiaalloogg ************
 Use Button to close a dialog using the dismiss() function.
+from bootwrap import Panel, Dialog, Button
 dialog = Dialog(
   "Greeting",
   "Hello World!",
   Button("Bye").as_primary().dismiss()
 )
 button = Button("Say Hello").as_primary().toggle(dialog)
+Panel(dialog, button)
 **** GGrreeeettiinngg ****
 ×
 Hello World!
 Bye
 Say Hello
 ************ EExxppaanndd//CCoollllaappssee PPaanneell ************
 Use Button to expand/collapse a panel using the toggle() function.
+from bootwrap import Panel, Button
 quote = Panel(
   "Sometimes life is going to hit you in " +
   "the head with a brick. Don’t lose faith."
 ).as_collapse()
-Button("Steve Jobs Quote").as_primary().toggle(quote)
+Panel(
+  Button("Steve Jobs Quote").as_primary().toggle(quote),
+  quote
+)
 Steve Jobs Quote
 Sometimes life is going to hit you in the head with a brick. Don’t lose faith.
 ************ SSuubbmmiitt AAccttiioonn ************
 Use Button to submit form content using the submit() function.
 NNoottee:: to make a form submit do not forget to use the Form function on_submit()
 , which specifies a URL that handles the post request. For more information
 view the Form documentation.
+from bootwrap import Form, TextInput, Button
 Form(
   TextInput("Email", "email", "my@email.com").for_email(),
   Button("Send").as_primary().submit()
 )
 Email
 [Unknown INPUT type]
 Send
@@ -258,29 +311,29 @@
         "Amazon (NASDAQ: AMZN)",
         description= "Price for a single Amazon share",
         figure=Image("amazon-logo.png", width=128).mt(3),
         marker="12:04:58 12/01/2021"
     ).add_menu(*actions).pack_actions().link(
         "https://www.amazon.com")
 )
-_[_g_o_o_g_l_e_-_l_o_g_o_._p_n_g_]
-_1_2_:_0_4_:_5_8_ _1_2_/_0_1_/_2_0_2_1
-_**_**_ _GG_oo_oo_gg_ll_ee_ _((_NN_AA_SS_DD_AA_QQ_::_ _GG_OO_OO_GG_LL_))_ _**_**
-_P_r_i_c_e_ _f_o_r_ _a_ _s_i_n_g_l_e_ _G_o_o_g_l_e_ _s_h_a_r_e
-_B_u_y_ _S_e_l_l_ _T_r_a_n_s_f_e_r
-_[_l_i_n_k_e_d_i_n_-_l_o_g_o_._p_n_g_]
-_1_2_:_0_4_:_5_8_ _1_2_/_0_1_/_2_0_2_1
-_**_**_ _LL_ii_nn_kk_ee_dd_II_nn_ _((_NN_AA_SS_DD_AA_QQ_::_ _LL_NN_KK_DD_))_ _**_**
-_P_r_i_c_e_ _f_o_r_ _a_ _s_i_n_g_l_e_ _L_i_n_k_e_d_I_n_ _s_h_a_r_e
-_B_u_y_ _S_e_l_l_ _T_r_a_n_s_f_e_r
-_[_a_m_a_z_o_n_-_l_o_g_o_._p_n_g_]
-_1_2_:_0_4_:_5_8_ _1_2_/_0_1_/_2_0_2_1
-_**_**_ _AA_mm_aa_zz_oo_nn_ _((_NN_AA_SS_DD_AA_QQ_::_ _AA_MM_ZZ_NN_))_ _**_**
-_P_r_i_c_e_ _f_o_r_ _a_ _s_i_n_g_l_e_ _A_m_a_z_o_n_ _s_h_a_r_e
-_B_u_y_ _S_e_l_l_ _T_r_a_n_s_f_e_r
+[google-logo.png]
+12:04:58 12/01/2021
+**** GGooooggllee ((NNAASSDDAAQQ:: GGOOOOGGLL)) ****
+Price for a single Google share
+Buy Sell Transfer
+[linkedin-logo.png]
+12:04:58 12/01/2021
+**** LLiinnkkeeddIInn ((NNAASSDDAAQQ:: LLNNKKDD)) ****
+Price for a single LinkedIn share
+Buy Sell Transfer
+[amazon-logo.png]
+12:04:58 12/01/2021
+**** AAmmaazzoonn ((NNAASSDDAAQQ:: AAMMZZNN)) ****
+Price for a single Amazon share
+Buy Sell Transfer
 ************ CCllaassss DDeecckk..CCaarrdd ************
 Argument
 A deck card.
 Deck.Card(title, description=None, marker=None, figure=None)
 ** AArrgguummeennttss **
 NNaammee        TTyyppee             DDeessccrriippttiioonn
 title       str|WebComponent The card title.
@@ -299,19 +352,19 @@
 Deck.Card(
     "Google (NASDAQ: GOOGL)",
     description= "Price for a single Google share",
     figure=Image("google-logo.png", width=128).mt(3),
     marker="12:04:58 12/01/2021"
 ).add_menu(*actions).link(
     "https://www.google.com")
-_[_g_o_o_g_l_e_-_l_o_g_o_._p_n_g_]
-_1_2_:_0_4_:_5_8_ _1_2_/_0_1_/_2_0_2_1
-_**_**_ _GG_oo_oo_gg_ll_ee_ _((_NN_AA_SS_DD_AA_QQ_::_ _GG_OO_OO_GG_LL_))_ _**_**
-_P_r_i_c_e_ _f_o_r_ _a_ _s_i_n_g_l_e_ _G_o_o_g_l_e_ _s_h_a_r_e
-_B_u_y_ _S_e_l_l_ _T_r_a_n_s_f_e_r
+[google-logo.png]
+12:04:58 12/01/2021
+**** GGooooggllee ((NNAASSDDAAQQ:: GGOOOOGGLL)) ****
+Price for a single Google share
+Buy Sell Transfer
 ****** MMeetthhoodd ppaacckk__aaccttiioonnss ******
 Makes item actions packed under a drop-down menu.
 pack_actions()
 ** EExxaammppllee **
 from bootwrap import Button, Deck, Image
 
 actions = [
@@ -323,90 +376,94 @@
 Deck.Card(
     "Google (NASDAQ: GOOGL)",
     description= "Price for a single Google share",
     figure=Image("google-logo.png", width=128).mt(3),
     marker="12:04:58 12/01/2021"
 ).add_menu(*actions).pack_actions().link(
     "https://www.google.com")
-_[_g_o_o_g_l_e_-_l_o_g_o_._p_n_g_]
-_1_2_:_0_4_:_5_8_ _1_2_/_0_1_/_2_0_2_1
-_**_**_ _GG_oo_oo_gg_ll_ee_ _((_NN_AA_SS_DD_AA_QQ_::_ _GG_OO_OO_GG_LL_))_ _**_**
-_P_r_i_c_e_ _f_o_r_ _a_ _s_i_n_g_l_e_ _G_o_o_g_l_e_ _s_h_a_r_e
-_B_u_y_ _S_e_l_l_ _T_r_a_n_s_f_e_r
+[google-logo.png]
+12:04:58 12/01/2021
+**** GGooooggllee ((NNAASSDDAAQQ:: GGOOOOGGLL)) ****
+Price for a single Google share
+Buy Sell Transfer
 ===============================================================================
     * _D_i_a_l_o_g
     * _Q_u_e_s_t_i_o_n_ _D_i_a_l_o_g
     * _C_o_m_p_l_e_x_ _D_i_a_l_o_g
 ************ CCllaassss DDiiaalloogg ************
 Argument
 A dialog.
 Dialog(title, content, *actions)
 ** AArrgguummeennttss **
 NNaammee     TTyyppee             DDeessccrriippttiioonn
 title    str              The dialog title.
 content  str|WebComponent The content inside a dialog window to show.
 *actions list             The dialog actions.
 ** EExxaammppllee **
-from bootwrap import Dialog, Button
+from bootwrap import Panel, Dialog, Button
 
 dialog = Dialog(
     'Greeting',
     'Hello World!',
     Button('Bye').dismiss()
 )
 button = Button('Say Hello').toggle(dialog)
+
+Panel(dialog, button)
 **** GGrreeeettiinngg ****
 ×
 Hello World!
 Bye
 Say Hello
 ************ QQuueessttiioonn DDiiaalloogg ************
 An example of how Dialog can be used for confirming a specific action. Make
 sure that you provide a correct URL, which CCoonnffiirrmm Button linked to. You can
 specify define this URL something like this local/
 file_system?file_id=1234567&action=delete
-from bootwrap import Dialog, Button
+from bootwrap import Panel, Dialog, Button
 
 dialog = Dialog(
   "Delete File",
-  "Are you sure?",
-  Button("Confirm").as_danger().link("url/to/act")
+  "Are you sure that you want to delete this file?",
+  Button("Confirm").as_danger().dismiss(),
   Button("Cancel").dismiss()
 ).as_danger()
 
 button = Button("Delete").as_danger().toggle(dialog)
+
+Panel(dialog, button)
 **** DDeelleettee FFiillee ****
 ×
 Are you sure that you want to delete this file?
 Confirm Cancel
 Delete
 ************ CCoommpplleexx DDiiaalloogg ************
 An example of how Dialog can be used for buying shares. It contains a web Form
 where a user can specify an amount (in Dollars) for buying shares. When the
 user presses the BBuuyy Button , the form will be submitted to the server (at url/
 to/act ). If the user selects CCaanncceell , the dialog will be closed, discarding
 the buying action.
-from bootwrap import Form, NumericInput, Dialog, Button
+from bootwrap import Panel, Form, NumericInput, Dialog, Button
 
 dialog = Dialog(
     "Buy Company Shares",
     Form(
         NumericInput(
             "Amount($)",
             "amount",
-            placeholder=\
-              "enter an amount for buying shares"
+            placeholder="enter an amount for buying shares"
         ),
         Button("Cancel").add_classes("float-right").dismiss(),
-        Button("Buy").add_classes("float-right).mr(2).as_success().
-          submit()
-    ).on_submit("url/to/act")
+        Button("Buy").add_classes("float-right").mr(2).as_success().
+          dismiss()
+    )
 )
-
 button = Button("Buy Shares").as_primary().toggle(dialog)
+
+Panel(dialog, button)
 **** BBuuyy CCoommppaannyy SShhaarreess ****
 ×
 Amount($)
 [Unknown INPUT type]
 Cancel Buy
 Buy Shares
 ===============================================================================
@@ -560,15 +617,15 @@
 label       str  The input label
 name        str  The input name.
 value       obj  The input value.
 placeholder str  The input placeholder.
 Use the as_disabled() function to prevent the user from entering data to the
 NumericInput component.
 ** EExxaammppllee **
-from bootwrap import Form, TextInput
+from bootwrap import Form, NumericInput
 
 Form(
     NumericInput('Number1', 'number'),
     NumericInput('Number2', 'number', placeholder='type here'),
     NumericInput('Number3', 'number', 123),
     NumericInput('Number4', 'number').as_disabled()
 )
@@ -598,15 +655,15 @@
 options = [
     SelectInput.Option('One', 1),
     SelectInput.Option('Two', 2),
     SelectInput.Option('Three', 3, disabled=True)
 ]
 
 Form(
-    SelectInput('Selector1', 'choice', 2, options)
+    SelectInput('Selector1', 'choice', 2, options),
     SelectInput('Selector2', 'choice', 2, options).as_disabled()
 )
 Selector1
 [One of: One/Two/Three]
 Selector2
 [One of: One/Two/Three]
 ****** MMeetthhoodd aass__rraaddiioo ******
@@ -671,15 +728,15 @@
 label str  The input label
 name  str  The input name.
 Use the as_disabled() function to prevent the user from entering data to the
 FileInput component.
 ** EExxaammppllee **
 from bootwrap import Form, FileInput
 
-output = Form(
+Form(
     FileInput('File', 'file'),
     FileInput('File', 'file').as_disabled()
 )
 File
 Browse[File]
 File
 Browse[File]
@@ -690,54 +747,58 @@
 Argument
 An icon.
 Icon(name)
 ** AArrgguummeennttss **
 NNaammee TTyyppee DDeessccrriippttiioonn
 name str  The icon name.
 ** EExxaammppllee **
-from bootwrap import Icon
+from bootwrap import Icon, Panel
 
-Icon("fas fa-folder")
-Icon("fas fa-folder").as_primary()
-Icon("fas fa-folder").as_secondary()
-Icon("fas fa-folder").as_success()
-Icon("fas fa-folder").as_warning()
-Icon("fas fa-folder").as_danger()
-Icon("fas fa-folder").as_info()
-Icon("fas fa-folder").as_light()
-Icon("fas fa-folder").as_dark()
+Panel(
+    Icon("fas fa-folder"),
+    Icon("fas fa-folder").as_primary(),
+    Icon("fas fa-folder").as_secondary(),
+    Icon("fas fa-folder").as_success(),
+    Icon("fas fa-folder").as_warning(),
+    Icon("fas fa-folder").as_danger(),
+    Icon("fas fa-folder").as_info(),
+    Icon("fas fa-folder").as_light(),
+    Icon("fas fa-folder").as_dark()
+)
 ************ CCllaassss SSppiinnnneerr ************
 A spinner icon.
 Spinner()
 ** EExxaammppllee **
-from bootwrap import Spinner
+from bootwrap import Spinner, Panel
 
-Spinner()
-Spinner().as_primary()
-Spinner().as_secondary()
-Spinner().as_success()
-Spinner().as_warning()
-Spinner().as_danger()
-Spinner().as_info()
-Spinner().as_light()
-Spinner().as_dark()
+Panel(
+    Spinner(),
+    Spinner().as_primary(),
+    Spinner().as_secondary(),
+    Spinner().as_success(),
+    Spinner().as_warning(),
+    Spinner().as_danger(),
+    Spinner().as_info(),
+    Spinner().as_light(),
+    Spinner().as_dark()
+)
 ************ CCllaassss IImmaaggee ************
 Argument
 A web component for an image.
 Image(src, width=None, height=None, alt=None)
 ** AArrgguummeennttss **
 NNaammee   TTyyppee DDeessccrriippttiioonn
 src    obj  The image source to show.
 width  int  The image width.
 height int  The image height.
 alt    str  The alt text.
 ** EExxaammppllee **
 from bootwrap import Image
 
-Image("logo.png", width=64, height=64, alt="Bootwarp Logo")
+Image("logo.png")
 [logo.png]
 ===============================================================================
     * _J_a_v_a_s_c_r_i_p_t
     * _j_Q_u_e_r_y
 ************ CCllaassss JJaavvaassccrriipptt ************
 Argument
 A web component for a javascript.
@@ -756,37 +817,36 @@
     resources = [
         Javascript("https://ajax...0/jquery.min.js")
     ]
     ...
 )
 ************ jjQQuueerryy ************
 Use Javascript for creating interactive web content with the help of jQuery.
-from bootwrap import Javascript, Button, Text
+from bootwrap import Panel, Javascript, Button, Text
 
 label = Text("Answer:").as_strong()
 answer = Text("unknown").mr(2).ml(2)
 btn_yes = Button("Yes").as_success()
 btn_no = Button("No").as_danger()
 
 action = Javascript(
   script='''
     $("#btn_yes").on("click",function(){
       $("#answer").text("Yes");
     });
     $("#btn_no").on("click",function(){
       $("#answer").text("No");
     });
-  '''
+  ''',
   submap={
     "answer": answer,
     "btn_yes": btn_yes,
     "btn_no": btn_no
   }
 )
-
 Panel(
   label, answer, btn_yes, btn_no, action
 )
 AAnnsswweerr:: unknown Yes No
 ************ CCllaassss LLiinnkk ************
 Argument
 A web component for an external resource link.
@@ -821,15 +881,15 @@
 ** AArrgguummeennttss **
 NNaammee   TTyyppee DDeessccrriippttiioonn
 *items list The list of List.Item elements.
 ** EExxaammppllee **
 from bootwrap import Button, List, Image
 
 actions = [
-    Button("Buy"),
+    Button("Buy").as_success(),
     Button("Sell"),
     Button("Transfer")
 ]
 
 List(
     List.Item(
         "Google (NASDAQ: GOOGL)",
@@ -1049,17 +1109,17 @@
 Panel(*components)
 ** AArrgguummeennttss **
 NNaammee        TTyyppee DDeessccrriippttiioonn
 *components list The list of WebComponent .
 ** EExxaammppllee **
 from bootwrap import Text, Panel
 
-comp1 = Text("Component 1")
-comp2 = Text("Component 2")
-comp3 = Text("Component 3")
+comp1 = Text("Component 1").add_classes("border").ml(1)
+comp2 = Text("Component 2").add_classes("border").ml(1)
+comp3 = Text("Component 3").add_classes("border").ml(1)
 
 Panel(comp1, comp2, comp3)
 Component 1 Component 2 Component 3
 ****** MMeetthhoodd aass__ccoollllaappssee ******
 Returns
 Makes the panel collapsed.
 as_collapse()
@@ -1072,17 +1132,17 @@
 horizontal()
 ** RReettuurrnnss **
 NNaammee TTyyppee DDeessccrriippttiioonn
 obj  self The instance of this class.
 ** EExxaammppllee **
 from bootwrap import Text, Panel
 
-comp1 = Text("Component 1")
-comp2 = Text("Component 2")
-comp3 = Text("Component 3")
+comp1 = Text("Component 1").add_classes("border")
+comp2 = Text("Component 2").add_classes("border")
+comp3 = Text("Component 3").add_classes("border")
 
 Panel(comp1, comp2, comp3).horizontal()
 Component 1
 Component 2
 Component 3
 ****** MMeetthhoodd vveerrttiiccaall ******
 Returns
@@ -1090,31 +1150,33 @@
 vertical()
 ** RReettuurrnnss **
 NNaammee TTyyppee DDeessccrriippttiioonn
 obj  self The instance of this class.
 ** EExxaammppllee **
 from bootwrap import Text, Panel
 
-comp1 = Text("Component 1")
-comp2 = Text("Component 2")
-comp3 = Text("Component 3")
+comp1 = Text("Component 1").add_classes("border")
+comp2 = Text("Component 2").add_classes("border")
+comp3 = Text("Component 3").add_classes("border")
 
 Panel(comp1, comp2, comp3).vertical()
 Component 1
 Component 2
 Component 3
 ************ CCllaassss SSeeppaarraattoorr ************
 A horizontal line separator.
 Separator()
 ** EExxaammppllee **
-from bootwrap import Separator, Text
+from bootwrap import Panel, Separator, Text
 
-Text("Top Text")
-Separator()
-Text("Bottom Text")
+Panel(
+    Text("Top Text"),
+    Separator(),
+    Text("Bottom Text")
+)
 Top Text
 ===============================================================================
 Bottom Text
 ===============================================================================
     * _T_a_b_l_e
     * _T_a_b_l_e_._H_e_a_d
     * _T_a_b_l_e_._B_o_d_y
@@ -1272,14 +1334,16 @@
     [
         ["Value 11", "Value 12", "Value 13"],
         ["Value 21", "Value 22", "Value 23"],
         ["Value 31", "Value 32", "Value 33"],
     ]
 )
 table.head.as_dark()
+
+table
 CCoolluummnn 11 CCoolluummnn 22 CCoolluummnn 33
 Value 11 Value 12 Value 13
 Value 21 Value 22 Value 23
 Value 31 Value 32 Value 33
 ****** MMeetthhoodd aass__lliigghhtt ******
 Makes the table head appears as light gray.
 as_light()
@@ -1291,14 +1355,16 @@
     [
         ["Value 11", "Value 12", "Value 13"],
         ["Value 21", "Value 22", "Value 23"],
         ["Value 31", "Value 32", "Value 33"],
     ]
 )
 table.head.as_light()
+
+table
 CCoolluummnn 11 CCoolluummnn 22 CCoolluummnn 33
 Value 11 Value 12 Value 13
 Value 21 Value 22 Value 23
 Value 31 Value 32 Value 33
 ************ CCllaassss TTaabbllee..BBooddyy ************
 The table body.
 Table.Body(body)
@@ -1335,14 +1401,17 @@
     lambda v: "bg-warning" if v == "val2" else ""
 )
 
 table.body.transform(
     1,
     TableEntity.VALUE,
     lambda v: f"{v}"
+)
+
+table
 CCoolluummnn 11 CCoolluummnn 22 CCoolluummnn 33
 val1     int      this is a description for val1;
 val2     str      this is a description for val2;
 val3     bool     this is a description for val3;
 ************ CCllaassss TTeexxtt ************
 Argument
 A web component for a text.
@@ -1359,37 +1428,39 @@
 Returns
 Makes the text wrap as a code snippet.
 as_code()
 ** RReettuurrnnss **
 NNaammee TTyyppee DDeessccrriippttiioonn
 obj  self The instance of this class.
 ** EExxaammppllee **
-from bootwrap import Text
+from bootwrap import Panel, Text
 
 Text("print('Hello world!')").as_code()
 print('Hello world!')
 ****** MMeetthhoodd aass__hheeaaddiinngg ******
 Argument Returns
 Makes the text as heading.
 as_heading(level)
 ** AArrgguummeennttss **
 NNaammee  TTyyppee DDeessccrriippttiioonn
 level int  The heading level;
 ** RReettuurrnnss **
 NNaammee TTyyppee DDeessccrriippttiioonn
 obj  self The instance of this class.
 ** EExxaammppllee **
-from bootwrap import Text
+from bootwrap import Panel, Text
 
-Text("Header text 1").as_heading(1)
-Text("Header text 2").as_heading(2)
-Text("Header text 3").as_heading(3)
-Text("Header text 4").as_heading(4)
-Text("Header text 5").as_heading(5)
-Text("Header text 6").as_heading(6)
+Panel(
+    Text("Header text 1").as_heading(1),
+    Text("Header text 2").as_heading(2),
+    Text("Header text 3").as_heading(3),
+    Text("Header text 4").as_heading(4),
+    Text("Header text 5").as_heading(5),
+    Text("Header text 6").as_heading(6)
+)
 ************ HHeeaaddeerr tteexxtt 11 ************
 ********** HHeeaaddeerr tteexxtt 22 **********
 ******** HHeeaaddeerr tteexxtt 33 ********
 ****** HHeeaaddeerr tteexxtt 44 ******
 **** HHeeaaddeerr tteexxtt 55 ****
 ** HHeeaaddeerr tteexxtt 66 **
 ****** MMeetthhoodd aass__mmuutteedd ******
@@ -1408,19 +1479,21 @@
 Returns
 Makes the text wrap in a paragraph.
 as_paragraph()
 ** RReettuurrnnss **
 NNaammee TTyyppee DDeessccrriippttiioonn
 obj  self The instance of this class.
 ** EExxaammppllee **
-from bootwrap import Text
+from bootwrap import Panel, Text
 
-Text("Paragraph 1").as_paragraph()
-Text("Paragraph 2").as_paragraph()
-Text("Paragraph 3").as_paragraph()
+Panel(
+    Text("Paragraph 1").as_paragraph(),
+    Text("Paragraph 2").as_paragraph(),
+    Text("Paragraph 3").as_paragraph()
+)
 Paragraph 1
 Paragraph 2
 Paragraph 3
 ****** MMeetthhoodd aass__ssmmaallll ******
 Returns
 Makes the text as small.
 as_small()
```

### Comparing `bootwrap-1.0.0/docs/config/base.yaml` & `bootwrap-1.0.1/docs/config/base.yaml`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/docs/config/components.yaml` & `bootwrap-1.0.1/docs/config/components.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -9,23 +9,14 @@
   - class: Anchor
 
   - title: Appearance
     description:
       - Change <code>Anchor</code> appearance using the following functions <code>as_primary()</code>, <code>as_secondary()</code>, <code>as_success()</code>, <code>as_warning()</code>, <code>as_danger()</code>, <code>as_info()</code>, <code>as_light()</code>, and <code>as_dark()</code>.
     code: |
       @right
-      Anchor("Primary").as_primary()
-      Anchor("Secondary").as_secondary()
-      Anchor("Success").as_success()
-      Anchor("Warning").as_warning()
-      Anchor("Danger").as_danger()
-      Anchor("Info").as_info()
-      Anchor("Light").as_light()
-      Anchor("Dark").as_dark()
-    evaluation: |
       from bootwrap import Panel, Anchor
       panel = Panel(
         Anchor("Primary").link("#").as_primary(),
         Anchor("Secondary").link("#").as_secondary(),
         Anchor("Success").link("#").as_success(),
         Anchor("Warning").link("#").as_warning(),
         Anchor("Danger").link("#").as_danger(),
@@ -38,72 +29,51 @@
       output = panel
 
   - title: Link Resource
     description: 
       - Associate <code>Anchor</code> with a hyperlink using the <code>link()</code> function.
     code: |
       @right
-      Anchor("Google Search").link("https://www.google.com/")
-    evaluation: |
       from bootwrap import Panel, Anchor
       output = Panel(
           Anchor("Google Search").link("https://www.google.com/")
       )
 
   - title: Open Dialog
     description: 
       - Use <code>Anchor</code> to open a dialog using the <code>toggle()</code> function.
     code: |
       @right
-      dialog = Dialog(
-        "Greeting",
-        "Hello World!"
-      )
-      anchor = Anchor("Say Hello").toggle(dialog)   
-    evaluation: |
       from bootwrap import Panel, Dialog, Anchor
       dialog = Dialog(
         "Greeting",
         "Hello World!"
       )
       anchor = Anchor("Say Hello").toggle(dialog)
       output = Panel(dialog, anchor)
 
   - title: Close Dialog
     description: 
       - Use <code>Anchor</code> to close a dialog using the <code>dismiss()</code> function.
     code: |
       @right
-      dialog = Dialog(
-        "Greeting",
-        "Hello World!",
-        Anchor("Bye").dismiss()
-      )
-      anchor = Anchor("Say Hello").toggle(dialog)   
-    evaluation: |
       from bootwrap import Panel, Dialog, Anchor
       dialog = Dialog(
         "Greeting",
         "Hello World!",
         Anchor("Bye").dismiss()
       )
       anchor = Anchor("Say Hello").toggle(dialog)  
       output = Panel(dialog, anchor)
 
   - title: Expand/Collapse Panel
     description: 
       - Use <code>Anchor</code> to expand/collapse a panel using the <code>toggle()</code> function.
     code: |
       @right
-      quote = Panel(
-        "Sometimes life is going to hit you in " +
-        "the head with a brick. Don’t lose faith."
-      ).as_collapse()
-      Anchor("Steve Jobs Quote").toggle(quote)
-    evaluation: |
       from bootwrap import Panel, Anchor
       quote = Panel(
         "Sometimes life is going to hit you in " +
         "the head with a brick. Don’t lose faith."
       ).as_collapse()
       output = Panel(
         Anchor("Steve Jobs Quote").toggle(quote),
@@ -116,23 +86,14 @@
   - class: Badge
 
   - title: Appearance
     description:
       - Change <code>Badge</code> appearance using the following functions <code>as_primary()</code>, <code>as_secondary()</code>, <code>as_success()</code>, <code>as_warning()</code>, <code>as_danger()</code>, <code>as_info()</code>, <code>as_light()</code>, and <code>as_dark()</code>.
     code: |
       @right
-      Badge("Primary").as_primary()
-      Badge("Secondary").as_secondary()
-      Badge("Success").as_success()
-      Badge("Warning").as_warning()
-      Badge("Danger").as_danger()
-      Badge("Info").as_info()
-      Badge("Light").as_light()
-      Badge("Dark").as_dark()
-    evaluation: |
       from bootwrap import Panel, Badge
       panel = Panel(
         Badge("Primary").as_primary(),
         Badge("Secondary").as_secondary(),
         Badge("Success").as_success(),
         Badge("Warning").as_warning(),
         Badge("Danger").as_danger(),
@@ -150,23 +111,14 @@
   - class: Button
 
   - title: Appearance
     description:
       - Change <code>Button</code> appearance using the following functions <code>as_primary()</code>, <code>as_secondary()</code>, <code>as_success()</code>, <code>as_warning()</code>, <code>as_danger()</code>, <code>as_info()</code>, <code>as_light()</code>, and <code>as_dark()</code>.
     code: |
       @right
-      Button("Primary").as_primary()
-      Button("Secondary").as_secondary()
-      Button("Success").as_success()
-      Button("Warning").as_warning()
-      Button("Danger").as_danger()
-      Button("Info").as_info()
-      Button("Light").as_light()
-      Button("Dark").as_dark()
-    evaluation: |
       from bootwrap import Panel, Button
       panel = Panel(
         Button("Primary").link("#").as_primary(),
         Button("Secondary").link("#").as_secondary(),
         Button("Success").link("#").as_success(),
         Button("Warning").link("#").as_warning(),
         Button("Danger").link("#").as_danger(),
@@ -179,23 +131,14 @@
       output = panel
 
   - title: Outline
     description:
       - Make <code>Button</code> without filling with surrounded by color border using the following function <code>as primary()</code>.
     code: |
       @right
-      Button("Primary").as_primary().as_outline()
-      Button("Secondary").as_secondary().as_outline()
-      Button("Success").as_success().as_outline()
-      Button("Warning").as_warning().as_outline()
-      Button("Danger").as_danger().as_outline()
-      Button("Info").as_info().as_outline()
-      Button("Light").as_light().as_outline()
-      Button("Dark").as_dark().as_outline()
-    evaluation: |
       from bootwrap import Panel, Button
       panel = Panel(
         Button("Primary").link("#").as_primary().as_outline(),
         Button("Secondary").link("#").as_secondary().as_outline(),
         Button("Success").link("#").as_success().as_outline(),
         Button("Warning").link("#").as_warning().as_outline(),
         Button("Danger").link("#").as_danger().as_outline(),
@@ -208,86 +151,62 @@
       output = panel
 
   - title: Disable
     description:
       - But default the <code>Button</code> always enabled. Use the <code>as_disabled()</code> function to make the <code>Button</code> disabled. Disable status prevent user to initiate any action assigned to the <code>Button</code>.
     code: |
       @right
-      Button("Enabled").as_primary()
-      Button("Disabled").as_primary().as_disabled()
-    evaluation: |
       from bootwrap import Panel, Button
       output = Panel(
         Button("Enabled").as_primary(),
         Button("Disabled").as_primary().as_disabled()
       )
 
   - title: Link Resource
     description: 
       - Associate <code>Button</code> with a hyperlink using the <code>link()</code> function.
     code: |
       @right
-      Button("Google Search").as_primary().link("https://www.google.com/")
-    evaluation: |
       from bootwrap import Panel, Button
       output = Panel(
           Button("Google Search").as_primary().link("https://www.google.com/")
       )
 
   - title: Open Dialog
     description: 
       - Use <code>Button</code> to open a dialog using the <code>toggle()</code> function.
     code: |
       @right
-      dialog = Dialog(
-        "Greeting",
-        "Hello World!"
-      )
-      button = Button("Say Hello").as_primary().toggle(dialog)   
-    evaluation: |
       from bootwrap import Panel, Dialog, Button
       dialog = Dialog(
         "Greeting",
         "Hello World!"
       )
       button = Button("Say Hello").as_primary().toggle(dialog)
       output = Panel(dialog, button)
 
   - title: Close Dialog
     description: 
       - Use <code>Button</code> to close a dialog using the <code>dismiss()</code> function.
     code: |
       @right
-      dialog = Dialog(
-        "Greeting",
-        "Hello World!",
-        Button("Bye").as_primary().dismiss()
-      )
-      button = Button("Say Hello").as_primary().toggle(dialog)   
-    evaluation: |
       from bootwrap import Panel, Dialog, Button
       dialog = Dialog(
         "Greeting",
         "Hello World!",
         Button("Bye").as_primary().dismiss()
       )
       button = Button("Say Hello").as_primary().toggle(dialog)  
       output = Panel(dialog, button)
 
   - title: Expand/Collapse Panel
     description: 
       - Use <code>Button</code> to expand/collapse a panel using the <code>toggle()</code> function.
     code: |
       @right
-      quote = Panel(
-        "Sometimes life is going to hit you in " +
-        "the head with a brick. Don’t lose faith."
-      ).as_collapse()
-      Button("Steve Jobs Quote").as_primary().toggle(quote)
-    evaluation: |
       from bootwrap import Panel, Button
       quote = Panel(
         "Sometimes life is going to hit you in " +
         "the head with a brick. Don’t lose faith."
       ).as_collapse()
       output = Panel(
         Button("Steve Jobs Quote").as_primary().toggle(quote),
@@ -296,19 +215,14 @@
 
   - title: Submit Action
     description: 
       - Use <code>Button</code> to submit form content using the <code>submit()</code> function.
       - <strong>Note:</strong> to make a form submit do not forget to use the <code>Form</code> function <code>on_submit()</code>, which specifies a URL that handles the post request. For more information view the <code>Form</code> documentation.
     code: |
       @right
-      Form(
-        TextInput("Email", "email", "my@email.com").for_email(),
-        Button("Send").as_primary().submit()
-      )   
-    evaluation: |
       from bootwrap import Form, TextInput, Button
       output = Form(
         TextInput("Email", "email", "my@email.com").for_email(),
         Button("Send").as_primary().submit()
       )
 
 
@@ -324,25 +238,14 @@
   - class: Dialog
 
   - title: Question Dialog
     description:
       - An example of how <code>Dialog</code> can be used for confirming a specific action. Make sure that you provide a correct URL, which <strong>Confirm</strong> <code>Button</code> linked to. You can specify define this URL something like this <code>local/file_system?file_id=1234567&action=delete</code> 
     code: |
       @right
-      from bootwrap import Dialog, Button
-
-      dialog = Dialog(
-        "Delete File",
-        "Are you sure?",
-        Button("Confirm").as_danger().link("url/to/act")
-        Button("Cancel").dismiss()
-      ).as_danger()
-
-      button = Button("Delete").as_danger().toggle(dialog)   
-    evaluation: |
       from bootwrap import Panel, Dialog, Button
 
       dialog = Dialog(
         "Delete File",
         "Are you sure that you want to delete this file?",
         Button("Confirm").as_danger().dismiss(),
         Button("Cancel").dismiss()
@@ -353,33 +256,14 @@
       output = Panel(dialog, button)
 
   - title: Complex Dialog
     description:
       - An example of how <code>Dialog</code> can be used for buying shares. It contains a web <code>Form</code> where a user can specify an amount (in Dollars) for buying shares. When the user presses the <strong>Buy</strong> <code>Button</code>, the form will be submitted to the server (at <code>url/to/act</code>). If the user selects <strong>Cancel</strong>, the dialog will be closed, discarding the buying action.
     code: |
       @right
-      from bootwrap import Form, NumericInput, Dialog, Button
-
-      dialog = Dialog(
-          "Buy Company Shares",
-          Form(
-              NumericInput(
-                  "Amount($)",
-                  "amount",
-                  placeholder=\
-                    "enter an amount for buying shares"
-              ),
-              Button("Cancel").add_classes("float-right").dismiss(),
-              Button("Buy").add_classes("float-right).mr(2).as_success().
-                submit()
-          ).on_submit("url/to/act")
-      )
-
-      button = Button("Buy Shares").as_primary().toggle(dialog)     
-    evaluation: |
       from bootwrap import Panel, Form, NumericInput, Dialog, Button
 
       dialog = Dialog(
           "Buy Company Shares",
           Form(
               NumericInput(
                   "Amount($)",
@@ -417,42 +301,14 @@
 
   - title: jQuery
     description:
       - Use <code>Javascript</code> for creating interactive web content with the help of jQuery.
 
     code: |
       @right
-
-      from bootwrap import Javascript, Button, Text
-
-      label = Text("Answer:").as_strong()
-      answer = Text("unknown").mr(2).ml(2)
-      btn_yes = Button("Yes").as_success()
-      btn_no = Button("No").as_danger()
-
-      action = Javascript(
-        script='''
-          $("#btn_yes").on("click",function(){
-            $("#answer").text("Yes");
-          });
-          $("#btn_no").on("click",function(){
-            $("#answer").text("No");
-          });
-        '''
-        submap={
-          "answer": answer,
-          "btn_yes": btn_yes,
-          "btn_no": btn_no
-        }
-      )
-      
-      Panel(
-        label, answer, btn_yes, btn_no, action
-      )
-    evaluation: |
       from bootwrap import Panel, Javascript, Button, Text
 
       label = Text("Answer:").as_strong()
       answer = Text("unknown").mr(2).ml(2)
       btn_yes = Button("Yes").as_success()
       btn_no = Button("No").as_danger()
```

### Comparing `bootwrap-1.0.0/docs/config/home.yaml` & `bootwrap-1.0.1/docs/config/home.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     - <h2 class="text-muted">Pure Python wrapper for one of the most popular front-end toolkit Bootstrap, allowing quick and easy prototyping of web-based user interfaces</h2>
   image:
     file: flash.png
     height: 300
 
 - title: Installation
   description: 
-    - "Use the following command to install Python Bootwrap (<span class='text-danger'>Please note, the PIP install is currently unavailable. The first version of Python Bootstrap should be released toward the end of March 2021.</span>)"
+    - "Use the following command to install Python Bootwrap:"
   code:
     ~$ pip install bootwrap
 
 - title: Single-Page Application
   description:
     - "A single-page Bootwrap application looks something like this:"
   code: |
```

### Comparing `bootwrap-1.0.0/docs/config/layout.yaml` & `bootwrap-1.0.1/docs/config/layout.yaml`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/docs/doc_app.py` & `bootwrap-1.0.1/docs/doc_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 The web-application for showing the project documentation.
 """
 
 import os
+import re
 import textwrap
 import pathlib
 import glob
 
 import yaml
 
 from flask import Flask, Markup
@@ -94,15 +95,20 @@
     web component can be used.
 
     Args:
         code (str): The code fragment to show.
     """
 
     def __init__(self, code):
-        super().__init__('Example', bw.Text(code.rstrip()).as_code())
+        super().__init__(
+            'Example',
+            bw.Text(
+                re.sub(r'(^\n\s)*output\s*=\s*', '', code)
+            ).as_code()
+        )
 
 
 class DemoDoc(BlockDoc):
     """A component to render an example.
 
     Renders an example code to provide a user with the look and feel for
     the component(s).
@@ -126,20 +132,19 @@
     Args:
         doc (dict): The documentation about a property. For more information
             about the property-documentation, see the `docgen` module.
     """
 
     def __init__(self, doc):
         wc_example = None
+        wc_demo = None
         if len(doc['example']) > 0:
             wc_example = ExampleDoc(doc['example'])
-
-        wc_demo = None
-        if len(doc['demo']) > 0:
-            wc_demo = DemoDoc(doc['demo'])
+            if re.search(r'(^\s)*output\s*=\s*', doc['example']):
+                wc_demo = DemoDoc(doc['example'])
 
         wc_title = bw.Text(
             'Property ' + str(bw.Text(doc['name']).as_primary())
         ).as_heading(4)
 
         wc_summary = bw.Text(doc['summary']).as_muted()
 
@@ -187,20 +192,19 @@
             wc_returns_btn = bw.Button('Returns').\
                 as_primary().\
                 as_outline().\
                 add_classes('btn-sm').\
                 toggle(wc_returns)
 
         wc_example = None
+        wc_demo = None
         if len(doc['example']) > 0:
             wc_example = ExampleDoc(doc['example'])
-
-        wc_demo = None
-        if len(doc['demo']) > 0:
-            wc_demo = DemoDoc(doc['demo'])
+            if re.search(r'(^\s)*output\s*=\s*', doc['example']):
+                wc_demo = DemoDoc(doc['example'])
 
         wc_title = bw.Panel(
             bw.Text(
                 'Method ' + str(bw.Text(doc['name']).as_primary())
             ).as_heading(4),
             bw.Panel(wc_arguments_btn, wc_returns_btn)
         ).add_classes('d-flex justify-content-between')
@@ -258,20 +262,19 @@
             wc_returns_btn = bw.Button('Returns').\
                 as_primary().\
                 as_outline().\
                 add_classes('btn-sm').\
                 toggle(wc_returns)
 
         wc_example = None
+        wc_demo = None
         if len(doc['example']) > 0:
             wc_example = ExampleDoc(doc['example'])
-
-        wc_demo = None
-        if len(doc['demo']) > 0:
-            wc_demo = DemoDoc(doc['demo'])
+            if re.search(r'(^\s)*output\s*=\s*', doc['example']):
+                wc_demo = DemoDoc(doc['example'])
 
         wc_title = bw.Panel(
             bw.Text(
                 'Class ' + str(bw.Text(self.__name).as_primary())
             ).as_heading(1),
             bw.Panel(wc_arguments_btn, wc_returns_btn)
         ).add_classes('d-flex justify-content-between')
@@ -367,29 +370,34 @@
                     width=doc['image'].get('width'),
                     height=doc['image'].get('height')
                 )
             ).add_classes('text-center')
 
         code_left = None
         code_right = None
+        evaluation = None
         if 'code' in doc:
             c = doc['code']
-            if '@right' in c:
-                c = c.replace('@right', '').strip()
+
+            is_right = '@right' in c
+
+            c = c.replace('@right', '').replace('@left', '').strip()
+
+            if re.search(r'(^\s)*output\s*=\s*', c):
+                loc = {}
+                exec(c, {}, loc)
+                evaluation = loc['output']
+
+            c = re.sub(r'(^\n\s)*output\s*=\s*', '', c)
+
+            if is_right:
                 code_right = bw.Text(c).as_code()
             else:
-                c = c.replace('@left', '').strip()
                 code_left = bw.Text(c).as_code()
 
-        evaluation = None
-        if 'evaluation' in doc:
-            loc = {}
-            exec(doc['evaluation'], {}, loc)
-            evaluation = loc['output']
-
         description = []
         if 'description' in doc:
             for paragraph in doc['description']:
                 description.append(bw.Text(paragraph).as_paragraph())
 
         super().__init__(
             bw.Panel(
```

### Comparing `bootwrap-1.0.0/docs/doc_generator.py` & `bootwrap-1.0.1/docs/doc_generator.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/docs/favicon.ico` & `bootwrap-1.0.1/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/docs/flash.png` & `bootwrap-1.0.1/docs/flash.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/docs/google-logo.png` & `bootwrap-1.0.1/demo/googl-logo.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/docs/index.html` & `bootwrap-1.0.1/docs/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!DOCTYPE html>
 <html lang="en">
  <head>
   <meta charset="utf-8"/>
-  <meta container="width=device-width, initial-scale=1,
+  <meta content="width=device-width, initial-scale=1,
                         shrink-to-fit=no" name="viewport"/>
   <link href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" rel="stylesheet" type="text/css"/>
   <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.8.2/css/all.min.css" rel="stylesheet" type="text/css"/>
   <link href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.5.0/styles/default.min.css" rel="stylesheet" type="text/css"/>
   <link href="favicon.ico" rel="icon" type="image/x-icon"/>
   <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.0/jquery.min.js" type="application/javascript">
   </script>
@@ -17,154 +17,150 @@
   <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.5.0/highlight.min.js" type="application/javascript">
   </script>
   <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.5.0/languages/python.min.js" type="application/javascript">
   </script>
  </head>
  <body>
   <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
-   <img alt="Bootwrap Logo" id="9a198304-bd57-4141-aa08-cd59d3ef8273" src="logo.png" width="32"/>
-   <span class="text-light" id="31f8408a-172f-4821-a8af-05b3805c9360">
+   <img alt="Bootwrap Logo" id="1ccddb16-881f-4616-b7bd-9a92b912e9f2" src="logo.png" width="32"/>
+   <span class="text-light" id="11c4dff3-d27f-4b9c-9a65-f84fc178ef94">
     <strong>
      Bootwrap
     </strong>
    </span>
    <button aria-controls="menu" aria-expanded="false" aria-label="Toggle menu" class="navbar-toggler" data-target="#menu" data-toggle="collapse" type="button">
     <span class="navbar-toggler-icon">
     </span>
    </button>
    <div class="collapse navbar-collapse" id="menu">
     <ul class="navbar-nav mr-auto">
      <li class="nav-item">
-      <a class="ml-2 nav-link" href="index.html" id="3da794b2-696e-41ee-9fe6-ccf91f216bc8">
+      <a class="ml-2 nav-link" href="index.html" id="fa100db1-c515-40f6-b812-2a6a9d357469">
        Home
       </a>
      </li>
      <li class="nav-item">
-      <a class="ml-2 nav-link" href="layout.html" id="f448c284-fd95-4257-9550-910346d16729">
+      <a class="ml-2 nav-link" href="layout.html" id="63940be9-bd98-4f17-8f91-c4895c407814">
        Layout
       </a>
      </li>
      <li class="nav-item">
-      <a class="ml-2 nav-link" href="base.html" id="d0a05c1f-564a-424c-b188-bcfcdd591a96">
+      <a class="ml-2 nav-link" href="base.html" id="da9f4476-9168-45c2-ae44-2d9b4dc6dab6">
        Base
       </a>
      </li>
      <li class="nav-item">
-      <a class="ml-2 nav-link" href="components.html" id="3ead3d89-a42e-4126-9af9-064c0974bfd8">
+      <a class="ml-2 nav-link" href="components.html" id="58be4996-6ca9-4c31-aea1-031c1f535246">
        Components
       </a>
      </li>
     </ul>
-    <a class="ml-2 btn btn-outline-light" href="https://github.com/mmgalushka/bootwrap" id="e929b597-0217-4672-b89a-6ee390c4ffac" role="button">
+    <a class="ml-2 btn btn-outline-light" href="https://github.com/mmgalushka/bootwrap" id="541ab39a-8bf5-44ed-88df-5bd683bace82" role="button">
      GitHub
     </a>
    </div>
   </nav>
-  <div class="container" style="margin-top: 90px;">
-   <div id="78d02415-f76d-4f1b-8c6a-ab183d1e8db1">
-    <div class="mt-3" id="17f2300c-bd6b-4655-ae7d-1a5a8e33fa9e">
-     <div id="4cde077a-bb4e-406a-8cb5-1b94fad7aa26">
+  <div class="container-fluid">
+   <div id="4696420f-861c-4acb-a614-8f538a90a5ee">
+    <div class="mt-3" id="de419bc8-2495-451f-ac91-870160fdf39b">
+     <div id="6dd2ef8b-6184-4256-9336-1db9f68d5e8e">
       <div class="row">
        <div class="col-md">
-        <div id="5cd9026c-3f87-4f42-a585-8b469c282b5e">
-         <h1 id="997a9b7d-001d-4bd3-b179-1a77cf07f256">
+        <div id="2ead2dc9-776b-4d88-820b-eecafb9a1f36">
+         <h1 id="38dc2ce3-ffa5-4374-bbdb-d29e48074422">
           <span class="display-4">
            Bootwrap
           </span>
          </h1>
         </div>
        </div>
        <div class="col-md">
-        <div id="8c096a1c-de38-4506-898c-dcc6dd70509f">
+        <div id="70ec59e1-9e9e-4a65-b78d-8c140054c6c3">
         </div>
        </div>
       </div>
      </div>
-     <div id="1c0ccead-5b89-47db-8097-ff5c41b9108a">
+     <div id="92944e3b-fa6e-4580-928d-2215909aeedf">
       <div class="row">
        <div class="col-md">
-        <div id="47e3beca-c1a5-4bda-9b3e-249adb2aac5c">
-         <p id="7ac51815-cac7-42f2-a4d3-f72ff93ff7c5">
+        <div id="09219c67-b67d-494c-b2c7-346cdd4b0d03">
+         <p id="b89f2f99-a66a-4840-8813-ad95a673e2c1">
           <h2 class="text-muted">
            Pure Python wrapper for one of the most popular front-end toolkit Bootstrap, allowing quick and easy prototyping of web-based user interfaces
           </h2>
          </p>
         </div>
        </div>
        <div class="col-md">
-        <div id="9d9f4690-b404-445c-b2c6-12d9cde666ad">
-         <div class="text-center" id="352e8a9b-864b-43f0-8f1d-bfd6651ee3d5">
-          <img height="300" id="01651ee5-c908-4836-b24d-6aab5326801c" src="flash.png"/>
+        <div id="fc706181-6f9c-4395-ab9a-b89bbf138b72">
+         <div class="text-center" id="aa4a9d72-137e-42c2-801c-d8e1f8d3b922">
+          <img height="300" id="edf35874-835c-474d-8551-d031ec162b3f" src="flash.png"/>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="mt-3" id="c49ba2b2-8892-4b8c-be88-0b1f52801060">
-     <div id="1242334f-ca4b-4696-87ed-f8d58b0d439d">
+    <div class="mt-3" id="18458b4c-5052-48ab-b2c1-f727a0bad0fa">
+     <div id="9b8fa21b-37ea-4e7e-a4cb-431fe3cda775">
       <div class="row">
        <div class="col-md">
-        <div id="5fabd969-eade-458e-9ae3-6980e667b06e">
-         <h1 id="60fd1116-f0cb-4914-b469-615e30fe539c">
+        <div id="679f9901-a3e1-4a10-8336-5f90d2214964">
+         <h1 id="237c307f-959c-4bf8-8948-039c838d320c">
           Installation
          </h1>
         </div>
        </div>
        <div class="col-md">
-        <div id="38baace9-b181-4afb-876e-1ee975011770">
+        <div id="1a559bdf-8c2d-46bd-b7b2-cd78557967ef">
         </div>
        </div>
       </div>
      </div>
-     <div id="8e2791a8-afca-4d95-adfa-281444583f24">
+     <div id="890359c5-6979-46dc-aae4-373f8cc48a8d">
       <div class="row">
        <div class="col-md">
-        <div id="99db3603-03a5-4a3f-b109-5f27c98b51da">
-         <p id="523c408e-192b-4515-857c-2b75c2c8d3c4">
-          Use the following command to install Python Bootwrap (
-          <span class="text-danger">
-           Please note, the PIP install is currently unavailable. The first version of Python Bootstrap should be released toward the end of March 2021.
-          </span>
-          )
+        <div id="8641f78d-cc6a-45bb-acb4-ebed688d30dd">
+         <p id="c6e584af-85a3-4cb4-aab0-7b6003ca381f">
+          Use the following command to install Python Bootwrap:
          </p>
-         <pre id="027d2fe1-3133-4239-92e9-df6464c2a4aa"><code class="python">~$ pip install bootwrap</code></pre>
+         <pre id="a07d889c-a977-41cc-a729-b355d5384069"><code class="python">~$ pip install bootwrap</code></pre>
         </div>
        </div>
        <div class="col-md">
-        <div id="d1cc8814-9869-4cd3-bc7c-8df9681770f4">
+        <div id="4e28e1bc-b447-4ff0-8a4b-da10eebf754d">
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="mt-3" id="00122eee-80ed-4692-b258-cac9bd2c33f6">
-     <div id="cc0bb365-0e78-480e-a3c5-e25fc3687cda">
+    <div class="mt-3" id="dbc5fc44-5043-45b5-b6b2-51bb1bd2d707">
+     <div id="6b376206-eeb1-4b06-9e1d-2a4849b7ae31">
       <div class="row">
        <div class="col-md">
-        <div id="215b5302-c7df-4ad1-9dee-3112b0ea87b6">
-         <h1 id="5bf5eaa6-95d7-4f87-b0e2-329527249cf8">
+        <div id="b16c06fa-cfd8-4a99-9697-5e6115a7a3db">
+         <h1 id="778f0b1c-dc8c-42ee-a2dd-f2aeb54a1367">
           Single-Page Application
          </h1>
         </div>
        </div>
        <div class="col-md">
-        <div id="731a34df-9000-4afa-9d1b-a81b64b88ddc">
+        <div id="0b76af6a-0be7-4d91-8bbe-fb66221cd329">
         </div>
        </div>
       </div>
      </div>
-     <div id="664bf58d-2b61-44ca-bec8-79f5d78f3940">
+     <div id="ded7c058-910a-498a-bee3-a24d666d8332">
       <div class="row">
        <div class="col-md">
-        <div id="d60d9b6a-ec44-4cf9-bc48-4cfa3ff32e07">
-         <p id="dcf5c41b-4fc8-410a-9d50-8a6b3f22ffa5">
+        <div id="f4e40ed4-59bb-491c-8df6-2c4060c24055">
+         <p id="a3413a8e-f841-46da-84d8-492becead16f">
           A single-page Bootwrap application looks something like this:
          </p>
-         <pre id="097a9cd5-77ed-4b4d-901f-488f84268126"><code class="python">from flask import Flask, Markup
+         <pre id="b3fc28be-610d-4a55-96cb-532dbbbf3205"><code class="python">from flask import Flask, Markup
 from bootwrap import Page, Text
 
 app = Flask(__name__)
 
 @app.route('/')
 def hello_world():
     return Markup(
@@ -172,47 +168,47 @@
     )
 
 if __name__ == '__main__':
     app.run(debug=True)</code></pre>
         </div>
        </div>
        <div class="col-md">
-        <div id="ae9cb290-1460-4ad9-b6e2-6606ea608aac">
-         <div class="text-center" id="60c04564-4211-48ed-bff6-a556acb28507">
-          <img height="200" id="ff74c5dc-58f1-440d-bd63-e9409b5f319d" src="single-page-app.png"/>
+        <div id="bd5f37ee-9ada-43dc-959d-15fc8bf59ae4">
+         <div class="text-center" id="b845a17e-b06b-45ae-a824-e5c353da65a4">
+          <img height="200" id="788f619d-62ab-4334-afb3-19d4fce41575" src="single-page-app.png"/>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="mt-3" id="9526c825-fb02-4bd2-a0e8-2c46caab2443">
-     <div id="df6da8e6-6905-4ddc-9139-70e184972cfa">
+    <div class="mt-3" id="99fc7e2f-7595-467f-878b-679806f59e71">
+     <div id="a7b49eea-c121-4f83-988e-e3b09c897cb5">
       <div class="row">
        <div class="col-md">
-        <div id="1ac4d8d5-081f-4d91-90cc-87c7d12457df">
-         <h1 id="d34ac71f-9712-4dba-aa4c-0274a1e59a4b">
+        <div id="3a5c3ed5-c8a5-454d-ba08-a5e0435f5c84">
+         <h1 id="9bf4fb4d-b947-47cc-9507-d561b23a6e45">
           Multi-Pages Application
          </h1>
         </div>
        </div>
        <div class="col-md">
-        <div id="487d7914-2dab-4341-9889-780afd0daa3b">
+        <div id="74c05da7-c3fb-406c-8150-53221c400f34">
         </div>
        </div>
       </div>
      </div>
-     <div id="3532d584-9128-4f98-bcfb-ada356476304">
+     <div id="aca8fc82-9447-48a7-b56c-2a533013cb7f">
       <div class="row">
        <div class="col-md">
-        <div id="37cd5e34-83a7-4727-a9e2-aebdd02f4e6f">
-         <p id="7281144a-e12d-4b19-b106-adae3dfe7c43">
+        <div id="b8533a77-c7d5-49f6-aa63-d241e0bfbfe3">
+         <p id="51738b4c-5c78-476b-a3b4-ac83a816b16d">
           A multi-pages Bootwrap application looks something like this:
          </p>
-         <pre id="8966c5e7-a88f-44e8-86e9-860e5996399c"><code class="python">from flask import Flask, Markup
+         <pre id="54d9e5ab-fd12-4142-9085-862a75a5872c"><code class="python">from flask import Flask, Markup
 from bootwrap import (
   Page, Menu, Image, Anchor, Button, Text
 )
 
 # Both 'logo.png' and 'favicon.ico' are
 # stored in 'docs' folder
 app = Flask(
@@ -284,23 +280,26 @@
     )
 
 if __name__ == '__main__':
     app.run(debug=True)</code></pre>
         </div>
        </div>
        <div class="col-md">
-        <div id="851979f1-169a-4829-8577-e4fb808ad885">
-         <div class="text-center" id="08ddfb57-1b9d-447a-a30d-bcb031e497c4">
-          <img height="200" id="6aec082a-cf2a-4852-9276-62dcf3b85dbe" src="multi-pages-app.png"/>
+        <div id="5937baa4-4a04-4dac-9a29-e9ec1bd2c3cb">
+         <div class="text-center" id="3fd5bc06-660d-4e1f-8b56-ade9f1d686f3">
+          <img height="200" id="1a48a418-34cf-4949-bfc6-6b03fcd0f336" src="multi-pages-app.png"/>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
    </div>
   </div>
  </body>
  <script>
   hljs.initHighlightingOnLoad();
  </script>
+ <style>
+  :root{--container-margin-top: 90px}html{  width: 100%;  height: 100%; }  body{  background-color: var(--body-background-color);  background-image: var(--body-background-image);  background-position: var(--body-background-position);  background-size: var(--body-background-size);  -webkit-background-size: var(--body-background-size);  -moz-background-size: var(--body-background-size);  -o-background-size: var(--body-background-size);  background-repeat: var(--body-background-repeat);  background-origin: var(--body-background-origin);  background-clip: var(--body-background-clip);  background-attachment: var(--body-background-attachment); }  .container-fluid{  margin-top: var(--container-margin-top); }  .auth{  width: 400px;  margin-top: 150px }  @media only screen and (max-width: 420px){  body{  background-image: none;  }   .auth{  width: 100%;  margin-top: 0px  } }  .grid-container {  display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); }  .card {  margin-top: 10px; }
+ </style>
 </html>
```

#### html2text {}

```diff
@@ -6,17 +6,15 @@
 _G_i_t_H_u_b
 ************ BBoooottwwrraapp ************
 ********** PPuurree PPyytthhoonn wwrraappppeerr ffoorr oonnee ooff tthhee mmoosstt ppooppuullaarr ffrroonntt--eenndd ttoooollkkiitt
 BBoooottssttrraapp,, aalllloowwiinngg qquuiicckk aanndd eeaassyy pprroottoottyyppiinngg ooff wweebb--bbaasseedd uusseerr iinntteerrffaacceess
 **********
 [flash.png]
 ************ IInnssttaallllaattiioonn ************
-Use the following command to install Python Bootwrap ( Please note, the PIP
-install is currently unavailable. The first version of Python Bootstrap should
-be released toward the end of March 2021. )
+Use the following command to install Python Bootwrap:
 ~$ pip install bootwrap
 ************ SSiinnggllee--PPaaggee AApppplliiccaattiioonn ************
 A single-page Bootwrap application looks something like this:
 from flask import Flask, Markup
 from bootwrap import Page, Text
 
 app = Flask(__name__)
```

### Comparing `bootwrap-1.0.0/docs/layout.html` & `bootwrap-1.0.1/docs/layout.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!DOCTYPE html>
 <html lang="en">
  <head>
   <meta charset="utf-8"/>
-  <meta container="width=device-width, initial-scale=1,
+  <meta content="width=device-width, initial-scale=1,
                         shrink-to-fit=no" name="viewport"/>
   <link href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" rel="stylesheet" type="text/css"/>
   <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.8.2/css/all.min.css" rel="stylesheet" type="text/css"/>
   <link href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.5.0/styles/default.min.css" rel="stylesheet" type="text/css"/>
   <link href="favicon.ico" rel="icon" type="image/x-icon"/>
   <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.0/jquery.min.js" type="application/javascript">
   </script>
@@ -17,196 +17,199 @@
   <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.5.0/highlight.min.js" type="application/javascript">
   </script>
   <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.5.0/languages/python.min.js" type="application/javascript">
   </script>
  </head>
  <body>
   <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
-   <img alt="Bootwrap Logo" id="db46fa03-11d5-4968-b84a-2350906ebda7" src="logo.png" width="32"/>
-   <span class="text-light" id="6f1ef572-5958-4625-8e02-a7609e6f6ae1">
+   <img alt="Bootwrap Logo" id="91ed8920-db7d-4711-8a0a-72ee748d9fc6" src="logo.png" width="32"/>
+   <span class="text-light" id="00e6969c-c396-4b3b-96a8-9854f566ef3e">
     <strong>
      Bootwrap
     </strong>
    </span>
    <button aria-controls="menu" aria-expanded="false" aria-label="Toggle menu" class="navbar-toggler" data-target="#menu" data-toggle="collapse" type="button">
     <span class="navbar-toggler-icon">
     </span>
    </button>
    <div class="collapse navbar-collapse" id="menu">
     <ul class="navbar-nav mr-auto">
      <li class="nav-item">
-      <a class="ml-2 nav-link" href="index.html" id="28d99c9f-6acd-4169-b4f7-f0521761bc67">
+      <a class="ml-2 nav-link" href="index.html" id="2b377927-c8a0-42e2-ba37-b24193cdb601">
        Home
       </a>
      </li>
      <li class="nav-item">
-      <a class="ml-2 nav-link" href="layout.html" id="9d76f680-b307-4b0a-bf4e-eca020ab3f7b">
+      <a class="ml-2 nav-link" href="layout.html" id="f299f0e4-3783-4e21-9dc8-32ffe87a3d9c">
        Layout
       </a>
      </li>
      <li class="nav-item">
-      <a class="ml-2 nav-link" href="base.html" id="f0316425-82fe-41a6-84e8-ac3cd30d6803">
+      <a class="ml-2 nav-link" href="base.html" id="56323570-da98-40f1-9e9c-53364d70b7b9">
        Base
       </a>
      </li>
      <li class="nav-item">
-      <a class="ml-2 nav-link" href="components.html" id="3786df0c-ef8c-446b-a676-3e582efcd27e">
+      <a class="ml-2 nav-link" href="components.html" id="ed687b2a-27f5-40cd-8f54-bf97239ebf0c">
        Components
       </a>
      </li>
     </ul>
-    <a class="ml-2 btn btn-outline-light" href="https://github.com/mmgalushka/bootwrap" id="992d470b-6fc5-4fae-8188-0a1a68967707" role="button">
+    <a class="ml-2 btn btn-outline-light" href="https://github.com/mmgalushka/bootwrap" id="0003ef41-d8c1-4b55-8a0c-32c5059d60b4" role="button">
      GitHub
     </a>
    </div>
   </nav>
-  <div class="container" style="margin-top: 90px;">
-   <div id="f5a352cb-a29b-459f-96e7-3e2ba9748da3">
-    <div class="mt-3" id="52210bc8-1458-46eb-abee-123a1a6f94ce">
-     <div id="f7465efd-f214-4c59-836a-672ffecd3d79">
+  <div class="container-fluid">
+   <div id="bd9142e9-3582-46ed-b35a-d4a5ec244497">
+    <div class="mt-3" id="2cde731c-4991-4de9-9937-e5653ddfe506">
+     <div id="32d3dcc3-95be-4d72-a433-5d1262cb13d4">
       <div class="row">
        <div class="col-md">
-        <div id="c27095d9-1e97-48ae-9913-e6bcf894cea5">
-         <h1 id="cccafebb-6526-48c8-9434-df391328b3c1">
+        <div id="81484c09-87c6-46be-9007-3c6438fcd310">
+         <h1 id="d4aeab3b-eaa0-48e7-b350-c4866d42e0d1">
           Layout
          </h1>
         </div>
        </div>
        <div class="col-md">
-        <div id="93c71313-6455-426a-89a7-6d1879c3a495">
+        <div id="4def03cb-1e9f-4845-a21a-b64c8be5e30a">
         </div>
        </div>
       </div>
      </div>
-     <div id="e350f64a-9313-43e9-b99b-6465def492a7">
+     <div id="27f8d99c-21d9-4fe5-afb2-e6e0d10666d7">
       <div class="row">
        <div class="col-md">
-        <div id="6cdb14fb-84c9-488b-99c5-1368d6feefec">
-         <p id="a2a86fd8-3c64-480c-b755-02fec7aebc09">
+        <div id="3cc59aa5-8990-41b0-8126-f849e313b902">
+         <p id="c3759808-9379-43da-b1a1-26407de9e5f1">
           To simplify the process of developing Web UI, Bootwrap uses the predefined layout which consists  of two elements
           <code>
            Page
           </code>
           and
           <code>
            Menu
           </code>
           .
          </p>
-         <p id="3bae920c-aff6-41e1-81f3-170f8e436407">
+         <p id="15828b9e-62b3-428a-979f-a2ff590c1a25">
           <strong>
            Note:
           </strong>
           if your application does not require the top-level menu it can be discarded.
          </p>
         </div>
        </div>
        <div class="col-md">
-        <div id="53d246d4-d90b-4ab1-b9b6-7c0bfd106dfa">
-         <div class="text-center" id="46aad420-85ca-4a63-b0e3-4d583a5a3f91">
-          <img height="200" id="5a8082e8-8637-49b9-b4c7-525ec54f5a09" src="layout.png"/>
+        <div id="fd31fd37-7d28-4f85-90e3-997ad0989131">
+         <div class="text-center" id="3edc9919-dd36-4fe4-b38c-b814aa334f58">
+          <img height="200" id="58e5b25a-db1a-485a-9001-2a6c4197ddee" src="layout.png"/>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="mt-3" id="bfc50190-5c7b-4789-a005-ad88ce3cf128">
-     <div id="7c516a2e-e9a6-4171-ae11-16717eff0bb8">
+    <div class="mt-3" id="855d81ab-e503-4eba-9773-c35a7953d221">
+     <div id="c74ab02a-0068-4119-8d3e-f9fd9c40eb0d">
       <div class="row">
        <div class="col-md">
-        <div id="a77dc86e-31fe-4ce0-96e0-4876e44e8b87">
-         <h1 id="9aedb9d1-4145-466b-8fd5-81d5cc7393bc">
+        <div id="0437c34e-8f2f-4a69-91ce-446f9053785e">
+         <h1 id="29cd0b02-8c65-4d13-8732-b7cdb3fb53a3">
           Page
          </h1>
         </div>
        </div>
        <div class="col-md">
-        <div id="d8d97a17-56fc-45cd-8014-869337f647ad">
+        <div id="70da9430-47fb-4e4f-a10e-af1bcd33a605">
         </div>
        </div>
       </div>
      </div>
-     <div id="8cb72773-5246-4586-a2a1-44a19e62bcc6">
+     <div id="b70f9398-13d3-4e49-a28c-17fc0ab4dc4e">
       <div class="row">
        <div class="col-md">
-        <div id="6a503a15-41a0-46ce-8402-7776a37aeb5c">
-         <p id="27be6307-7b27-4295-b409-9b619b14139b">
+        <div id="8abdc82f-5840-4d61-a7aa-0472a4df01a0">
+         <p id="f792f3d4-fe75-488f-a18b-8d309219c37b">
           The container could be any element inheriting
           <code>
            WebComponent
           </code>
           class. Typically for hosting  other custom interface elements is used
           <code>
            Panel
           </code>
           .
          </p>
-         <pre id="5609b9a7-8081-46af-8ae5-d8017ad65a7e"><code class="python">from bootwrap import Page
+         <pre id="62c3f1ac-d00c-4701-9b5f-13a072a0de3e"><code class="python">from bootwrap import Page
 
 page = Page(
   favicon=..., title=..., resources=..., menu=...,
   container=...
 )</code></pre>
         </div>
        </div>
        <div class="col-md">
-        <div id="59f3168a-d948-4c3f-a66d-9ef92df2d2ca">
-         <div class="text-center" id="9116c3f9-7111-4e27-9536-16887b7c0864">
-          <img height="250" id="1dc11150-e939-47ac-88f8-237cce162bbc" src="page.png"/>
+        <div id="e9949b0c-92ad-4a10-9e21-84ef13eb457e">
+         <div class="text-center" id="dda5bc57-69cb-4fa7-ba87-87b97d9eb566">
+          <img height="250" id="b07fe878-1722-49d7-acd8-906060bbce9c" src="page.png"/>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
-    <div class="mt-3" id="6f2e772d-88e6-43de-bbfd-495704f9dd70">
-     <div id="07abd22f-0e2b-437b-b1af-acebe1e3ec7c">
+    <div class="mt-3" id="b47ecc41-f8c7-4b2b-a76b-939f305f8eb6">
+     <div id="64b7eb35-d8b2-4dbb-b7eb-94be9ddafde1">
       <div class="row">
        <div class="col-md">
-        <div id="22d91b85-f239-47ed-878d-daac8732ca01">
-         <h1 id="d9a839fa-6bc8-43d6-ad45-5364c120aceb">
+        <div id="39805470-7070-4fa0-8644-82efcbb5d8b1">
+         <h1 id="cf5e2ec4-6499-4409-9014-6010ffa3d80f">
           Menu
          </h1>
         </div>
        </div>
        <div class="col-md">
-        <div id="962d72c6-fcae-4e1f-b66e-c999a09497c7">
+        <div id="7a51fe13-4944-47fe-a24f-96379a61d323">
         </div>
        </div>
       </div>
      </div>
-     <div id="c1336fb7-d985-4564-965e-ac2365901075">
+     <div id="2694d329-9c59-40eb-b597-b0ee5795b3bb">
       <div class="row">
        <div class="col-md">
-        <div id="6a8e56f1-f14e-450a-963f-01d9d7ba682d">
-         <p id="ec01c15b-37b5-4c47-96a5-e3a7e0efdf26">
+        <div id="52efaecf-86e6-4a8b-b8ef-82449fbaa0a2">
+         <p id="66627388-89a8-4374-863a-be5b23e772a5">
           The menu represents the top-level navigation bar containing anchors and actions allowing to switch between different application
           <code>
            Page
           </code>
           s.
          </p>
-         <pre id="6a14e6ab-00e7-484f-bc94-8dc0808e4b04"><code class="python">from bootwrap import Menu
+         <pre id="16adca3c-5c27-434b-9d60-36a285948cf3"><code class="python">from bootwrap import Menu
 
 menu = Menu(
   logo=..., brand=..., anchors=...,  actions=...
 )</code></pre>
         </div>
        </div>
        <div class="col-md">
-        <div id="614e046f-4fdc-4f2f-bbc2-78a5f76e9cfd">
-         <div class="text-center" id="6ca552af-8cff-43c3-8b5e-d9fa2c68c066">
-          <img height="100" id="c1ca56ab-a052-4e12-b685-5fec77164f7c" src="menu.png"/>
+        <div id="8df4f554-4fb7-4f5a-a5b4-eee3e900d4db">
+         <div class="text-center" id="7c2b1f9a-9459-40b2-b2e5-c893fe3b4a49">
+          <img height="100" id="f1e87a94-5143-4337-81e8-9fe933c2e8bc" src="menu.png"/>
          </div>
         </div>
        </div>
       </div>
      </div>
     </div>
    </div>
   </div>
  </body>
  <script>
   hljs.initHighlightingOnLoad();
  </script>
+ <style>
+  :root{--container-margin-top: 90px}html{  width: 100%;  height: 100%; }  body{  background-color: var(--body-background-color);  background-image: var(--body-background-image);  background-position: var(--body-background-position);  background-size: var(--body-background-size);  -webkit-background-size: var(--body-background-size);  -moz-background-size: var(--body-background-size);  -o-background-size: var(--body-background-size);  background-repeat: var(--body-background-repeat);  background-origin: var(--body-background-origin);  background-clip: var(--body-background-clip);  background-attachment: var(--body-background-attachment); }  .container-fluid{  margin-top: var(--container-margin-top); }  .auth{  width: 400px;  margin-top: 150px }  @media only screen and (max-width: 420px){  body{  background-image: none;  }   .auth{  width: 100%;  margin-top: 0px  } }  .grid-container {  display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); }  .card {  margin-top: 10px; }
+ </style>
 </html>
```

### Comparing `bootwrap-1.0.0/docs/layout.png` & `bootwrap-1.0.1/docs/layout.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/docs/linkedin-logo.png` & `bootwrap-1.0.1/demo/lnkd-logo.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/docs/logo.png` & `bootwrap-1.0.1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/docs/menu.png` & `bootwrap-1.0.1/docs/menu.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/docs/multi-pages-app.png` & `bootwrap-1.0.1/docs/multi-pages-app.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/docs/page.png` & `bootwrap-1.0.1/docs/page.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/docs/single-page-app.png` & `bootwrap-1.0.1/docs/single-page-app.png`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/helper.sh` & `bootwrap-1.0.1/helper.sh`

 * *Files 5% similar despite different names*

```diff
@@ -11,27 +11,26 @@
 
 action_usage(){
     echo -e "    ____              __ _       __                "
     echo -e "   / __ )____  ____  / /| |     / /________ _____  "
     echo -e "  / __  / __ \/ __ \/ __/ | /| / / ___/ __ '/ __ \ "
     echo -e " / /_/ / /_/ / /_/ / /_ | |/ |/ / /  / /_/ / /_/ / "
     echo -e "/_____/\____/\____/\__/ |__/|__/_/   \__,_/ .___/  "
-    echo -e "                                         /_/       " 
+    echo -e "Python + Bootstrap                       /_/       " 
     echo -e ""                                          
     echo -e "${BOLD}System Commands:${NC}"
     echo -e "   ${CMD}init${NC} initializers environment;"
     echo -e "   ${CMD}test${OPT} ...${NC} runs tests;"
     echo -e "      ${OPT}-m <MARK> ${NC}runs tests for mark;"
     echo -e "      ${OPT}-c ${NC}generates code coverage summary;"
     echo -e "      ${OPT}-r ${NC}generates code coverage report;"
     echo -e "   ${CMD}preview${NC} runs web-server with documentation preview;"
     echo -e "   ${CMD}docs${NC} generates documentation (HTML-pages);"
     echo -e "   ${CMD}demo${NC} runs web-server with showcase project;" 
-    echo -e "   ${CMD}build${NC} generates distribution archives;"
-    echo -e "   ${CMD}stage${NC} deploys Bootwrap to Test Python Package Index;"  
+    echo -e "   ${CMD}build${NC} generates distribution archives;"  
 }
 
 action_init(){
     if [ -d .venv ];
         then
             rm -r .venv
     fi
@@ -82,27 +81,14 @@
 }
 
 action_build(){
     source .venv/bin/activate
     python -m build
 }
 
-action_stage(){
-    source .venv/bin/activate
-    read -p "Do you wish to stage Bootwrap to https://test.pypi.org (y/n)? " answer
-    case ${answer:0:1} in
-        y|Y )
-            python3 -m twine upload --repository testpypi dist/*
-        ;;
-        * )
-            echo -e "Aborted!"
-        ;;
-    esac
-}
-
 # =============================================================================
 # HELPER COMMANDS SELECTOR
 # =============================================================================
 case $1 in
     init)
         action_init
     ;;
@@ -117,16 +103,13 @@
     ;;
     demo)
         action_demo
     ;;
     build)
         action_build
     ;;
-    stage)
-        action_stage
-    ;;
     *)
         action_usage
     ;;
 esac  
 
 exit 0
```

### Comparing `bootwrap-1.0.0/main.py` & `bootwrap-1.0.1/main.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/pytest.ini` & `bootwrap-1.0.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/setup.py` & `bootwrap-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/tests/helper.py` & `bootwrap-1.0.1/tests/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,23 +128,24 @@
 
             raise TagAttributesNotMatchError(
                 f'{self_attrs_names} != {other_attrs_names}')
 
         # Checks that tags data are matched.
         self_data = self.__data.replace(" ", "")
         other_data = other.__data.replace(" ", "")
-        if self_data != other_data:
-            raise TagDataNotMatchError(f'{self_data} != {other_data}')
-
-        # Checks that children tags are matched.
-        if len(self.__tags) != len(other.__tags):
-            raise TagChildrenNotMatchError(
-                f'{len(self.__tags)} != {len(other.__tags)}')
-        for child_self_tag, child_other_tag in zip(self.__tags, other.__tags):
-            assert child_self_tag == child_other_tag
+        if self_data.strip() != '...' and other_data.strip() != '...':
+            if self_data != other_data:
+                raise TagDataNotMatchError(f'{self_data} != {other_data}')
+
+            # Checks that children tags are matched.
+            if len(self.__tags) != len(other.__tags):
+                raise TagChildrenNotMatchError(
+                    f'{len(self.__tags)} != {len(other.__tags)}')
+            for child_self_tag, child_other_tag in zip(self.__tags, other.__tags):
+                assert child_self_tag == child_other_tag
 
         # Tags are the same.
         return True
 
     def add_attr(self, attr):
         """Adds an attribute.
```

### Comparing `bootwrap-1.0.0/tests/test_anchor.py` & `bootwrap-1.0.1/tests/test_anchor.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/tests/test_base.py` & `bootwrap-1.0.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/tests/test_button.py` & `bootwrap-1.0.1/tests/test_button.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,16 +182,15 @@
 @pytest.mark.button
 def test_submit_button():
     button = Button('Somename').submit()
     actual = HelperHTMLParser.parse(str(button))
     expected = HelperHTMLParser.parse(f'''
         <button id="{button.identifier}"
             class="btn"
-            type="submit"
-            onclick="return false;">
+            type="submit">
             Somename
         </button>
     ''')
     assert actual == expected
 
 
 @pytest.mark.button
```

### Comparing `bootwrap-1.0.0/tests/test_deck.py` & `bootwrap-1.0.1/tests/test_deck.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         'sometitle',
         description='somedescr',
         figure=Icon('someicon'),
         marker="somemarker",
     )
     actual = HelperHTMLParser.parse(str(card))
     expected = HelperHTMLParser.parse(f'''
-        <a id="{card.identifier}" class="card">
+        <div id="{card.identifier}" class="card">
             <div class="row justify-content-center">
                 <i id="..." class="someicon"></i>
             </div>
             <div class="card-body">
                 <div class="text-right mb-2">
                     <span id="..."
                         class="text-muted"><small>somemarker</small>
@@ -31,76 +31,76 @@
                 </div>
                 <h5 id="..."
                     class="card-title">
                     sometitle
                 </h5>
                 somedescr
             </div>
-        </a>
+        </div>
     ''')
     assert actual == expected
 
     # Tests a custom deck card.
     card = Deck.Card(
         Text('sometitle'),
         description=Text('somedescr'),
         figure=Icon('someicon'),
         marker=Text("somemarker")
     )
     actual = HelperHTMLParser.parse(str(card))
     expected = HelperHTMLParser.parse(f'''
-        <a id="{card.identifier}" class="card">
+        <div id="{card.identifier}" class="card">
             <div class="row justify-content-center">
                 <i id="..." class="someicon"></i>
             </div>
             <div class="card-body">
                 <div class="text-right mb-2">
                     <span id="...">somemarker</span>
                 </div>
                 <span id="..." class="card-title">sometitle</span>
                 <span id="..." >somedescr</span>
             </div>
-        </a>
+        </div>
     ''')
     assert actual == expected
 
     # Tests an unpacked deck card actions.
     actions = [Button('A'), Button('B')]
     card = Deck.Card('sometitle').add_menu(*actions)
     actual = HelperHTMLParser.parse(str(card))
     expected = HelperHTMLParser.parse(f'''
-        <a id="{card.identifier}" class="card">
+        <div id="{card.identifier}" class="card">
             <div class="row justify-content-center"></div>
             <div class="card-body">
                 <h5 id="..." class="card-title">
                     sometitle
                 </h5>
             </div>
             <div class="card-footer text-right">
                 <button id="..."
-                    class="ml-1 btn"
+                    class="btn"
                     onclick="return false;">
                     A
                 </button>
                 <button id="..."
-                    class="ml-1 btn"
+                    class="btn"
                     onclick="return false;">
                     B
                 </button>
             </div>
-        </a>
+        </div>
     ''')
     assert actual == expected
 
     # Tests a packed deck card actions.
     actions = [Button('A'), Button('B')]
     card = Deck.Card('sometitle').add_menu(*actions).pack_actions()
     actual = HelperHTMLParser.parse(str(card))
     expected = HelperHTMLParser.parse(f'''
-        <a id="{card.identifier}" class="card">
+        <div id="{card.identifier}" class="card">
             <div class="row justify-content-center"></div>
             <div class="card-body">
                 <h5 id="..." class="card-title">
                     sometitle
                 </h5>
             </div>
             <div class="card-footer text-right">
@@ -121,56 +121,81 @@
                             class="dropdown-item btn"
                             onclick="return false;">
                             B
                         </button>
                     </div>
                 </div>
             </div>
-        </a>
+        </div>
+    ''')
+    assert actual == expected
+
+    # Tests a linked deck card.
+    card = Deck.Card(
+        'sometitle',
+        description='somedescr',
+        figure=Icon('someicon'),
+        marker="somemarker",
+    ).link('somewhere')
+    actual = HelperHTMLParser.parse(str(card))
+    expected = HelperHTMLParser.parse(f'''
+        <div id="{card.identifier}" class="card">
+            <div class="row justify-content-center" onclick="location.href='somewhere';">
+                <i id="..." class="someicon"></i>
+            </div>
+            <div class="card-body"  onclick="location.href='somewhere';">
+                <div class="text-right mb-2">
+                    <span id="..."
+                        class="text-muted"><small>somemarker</small>
+                    </span>
+                </div>
+                <h5 id="..."
+                    class="card-title">
+                    sometitle
+                </h5>
+                somedescr
+            </div>
+        </div>
     ''')
     assert actual == expected
 
 
 @pytest.mark.deck
 def test_deck():
     dk = Deck(
         Deck.Card('sometitle1'),
         Deck.Card('sometitle2'),
         Deck.Card('sometitle3')
     )
     actual = HelperHTMLParser.parse(str(dk))
     expected = HelperHTMLParser.parse(f'''
         <div id="{dk.identifier}" class="card-deck grid-container">
-            <a id="..." class="card">
+            <div id="..." class="card">
                 <div class="row justify-content-center"></div>
                 <div class="card-body">
                     <h5 id="..." class="card-title">sometitle1</h5>
                 </div>
-            </a>
-            <a id="..." class="card">
+            </div>
+            <div id="..." class="card">
                 <div class="row justify-content-center"></div>
                 <div class="card-body">
                     <h5 id="..." class="card-title">sometitle2</h5>
                 </div>
-            </a>
-            <a id="..." class="card">
+            </div>
+            <div id="..." class="card">
                 <div class="row justify-content-center"></div>
                 <div class="card-body">
                     <h5 id="..." class="card-title">sometitle3</h5>
                 </div>
-            </a>
+            </div>
         </div>
     ''' + '''
         <style>
-            a.card {
-                text-decoration: none;
-            }
-
-            a.card, a.card:visited, a.card:hover, a.card:active {
-                color: inherit;
+            div.card {
+                cursor:pointer
             }
         </style>
     ''')
     assert actual == expected
 
     with pytest.raises(TypeError):
         Deck("somecard")
```

### Comparing `bootwrap-1.0.0/tests/test_dialog.py` & `bootwrap-1.0.1/tests/test_dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,15 @@
                             aria-label="Close">
                             <span aria-hidden="true">&times;</span>
                         </button>
                     </div>
                     <div class="modal-body">
                         <button id="..."
                             class="btn"
-                            type="submit"
-                            onclick="return false;">
+                            type="submit">
                             submit
                         </button>
                     </div>
                 </div>
             </div>
         </div>
     ''')
```

### Comparing `bootwrap-1.0.0/tests/test_form.py` & `bootwrap-1.0.1/tests/test_form.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,19 +48,19 @@
 
     # the label on the same row as input...
     generic = GenericInput('somelabel', 'somename').\
         add_classes('someclass')
     actual = HelperHTMLParser.parse(str(generic))
     expected = HelperHTMLParser.parse(f'''
         <div class="form-group someclass row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center"
+            <label class="col-sm-4 col-form-label d-flex align-items-center"
                 for="{generic.identifier}">
                 somelabel
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
+            <div class="col-sm-8 d-flex align-items-center">
                 <xyz id="{generic.identifier}">somename</xyz>
             </div>
         </div>
     ''')
     assert actual == expected
 
     # the label on the top, input at the bottom...
@@ -94,19 +94,19 @@
 
 @pytest.mark.form
 def test_checkbox_input():
     checkbox = CheckboxInput('somelabel', 'somename')
     actual = HelperHTMLParser.parse(str(checkbox))
     expected = HelperHTMLParser.parse(f'''
         <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center"
+            <label class="col-sm-4 col-form-label d-flex align-items-center"
                 for="{checkbox.identifier}">
                 somelabel
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
+            <div class="col-sm-8 d-flex align-items-center">
                 <input id="{checkbox.identifier}"
                     name="somename"
                     type="checkbox"
                     class="form-check-input"
                     autocomplete="off"/>
             </div>
         </div>
@@ -114,19 +114,19 @@
     assert actual == expected
 
     checkbox = CheckboxInput('somelabel', 'somename', True).\
         as_disabled()
     actual = HelperHTMLParser.parse(str(checkbox))
     expected = HelperHTMLParser.parse(f'''
         <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center"
+            <label class="col-sm-4 col-form-label d-flex align-items-center"
                 for="{checkbox.identifier}">
                 somelabel
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
+            <div class="col-sm-8 d-flex align-items-center">
             <input id="{checkbox.identifier}"
                 name="somename"
                 type="checkbox"
                 class="form-check-input"
                 autocomplete="off" checked disabled/>
             </div>
         </div>
@@ -139,19 +139,19 @@
     # testing text-input...
     text = TextInput(
         'somelabel', 'somename', 'somevalue', placeholder='someplaceholder'
     )
     actual = HelperHTMLParser.parse(str(text))
     expected = HelperHTMLParser.parse(f'''
         <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center"
+            <label class="col-sm-4 col-form-label d-flex align-items-center"
                 for="{text.identifier}">
                 somelabel
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
+            <div class="col-sm-8 d-flex align-items-center">
                 <input id="{text.identifier}"
                     name="somename"
                     value="somevalue"
                     type="text"
                     class="form-control"
                     placeholder="someplaceholder"/>
             </div>
@@ -160,38 +160,38 @@
     assert actual == expected
 
     # testing email-input...
     email = TextInput('somelabel', 'somename').for_email()
     actual = HelperHTMLParser.parse(str(email))
     expected = HelperHTMLParser.parse(f'''
         <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center"
+            <label class="col-sm-4 col-form-label d-flex align-items-center"
                 for="{email.identifier}">
                 somelabel
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
+            <div class="col-sm-8 d-flex align-items-center">
                 <input id="{email.identifier}"
                     name="somename"
                     type="email"
                     class="form-control"/>
             </div>
         </div>
     ''')
     assert actual == expected
 
     # testing password-input...
     password = TextInput('somelabel', 'somename').for_password()
     actual = HelperHTMLParser.parse(str(password))
     expected = HelperHTMLParser.parse(f'''
         <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center"
+            <label class="col-sm-4 col-form-label d-flex align-items-center"
                 for="{password.identifier}">
                 somelabel
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
+            <div class="col-sm-8 d-flex align-items-center">
                 <input id="{password.identifier}"
                     name="somename"
                     type="password"
                     class="form-control"/>
             </div>
         </div>
     ''')
@@ -211,20 +211,20 @@
 
 
 @pytest.mark.form
 def test_text_area():
     def get_expected(element, disabled=False):
         return f'''
             <div class="form-group row">
-                <label class="col-sm-2 col-form-label d-flex
+                <label class="col-sm-4 col-form-label d-flex
                     align-items-center"
                     for="{element.identifier}">
                     somelabel
                 </label>
-                <div class="col-sm-10 d-flex align-items-center">
+                <div class="col-sm-8 d-flex align-items-center">
                     <textarea id="{element.identifier}"
                         name="somename"
                         class="form-control"
                         rows=5
                         {'disabled' if disabled else ''}
                         >somevalue</textarea>
                 </div>
@@ -250,19 +250,19 @@
 def test_numeric_input():
     numeric = NumericInput(
         'somelabel', 'somename', 'somevalue', placeholder='someplaceholder'
     )
     actual = HelperHTMLParser.parse(str(numeric))
     expected = HelperHTMLParser.parse(f'''
         <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center"
+            <label class="col-sm-4 col-form-label d-flex align-items-center"
                 for="{numeric.identifier}">
                 somelabel
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
+            <div class="col-sm-8 d-flex align-items-center">
                 <input id="{numeric.identifier}"
                     name="somename"
                     value="somevalue"
                     type="number"
                     class="form-control"
                     placeholder="someplaceholder"/>
             </div>
@@ -278,19 +278,19 @@
     options = [option_0, option_1]
 
     # testing select-input...
     select = SelectInput('somelabel', 'somename', 0, options)
     actual = HelperHTMLParser.parse(str(select))
     expected = HelperHTMLParser.parse(f'''
         <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center"
+            <label class="col-sm-4 col-form-label d-flex align-items-center"
                 for="{select.identifier}">
                 somelabel
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
+            <div class="col-sm-8 d-flex align-items-center">
                 <select id="{select.identifier}"
                     name="somename"
                     class="form-control"
                     autocomplete="off">
                     <option id="{option_0.identifier}"
                         value=0
                         selected
@@ -304,19 +304,19 @@
     ''')
     assert actual == expected
 
     select = SelectInput('somelabel', 'somename', 0, options).as_disabled()
     actual = HelperHTMLParser.parse(str(select))
     expected = HelperHTMLParser.parse(f'''
         <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center"
+            <label class="col-sm-4 col-form-label d-flex align-items-center"
                 for="{select.identifier}">
                 somelabel
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
+            <div class="col-sm-8 d-flex align-items-center">
                 <select id="{select.identifier}"
                     name="somename"
                     class="form-control"
                     autocomplete="off"
                     disabled>
                     <option id="{option_0.identifier}"
                         value=0
@@ -339,19 +339,19 @@
     options = [option_0, option_1]
 
     # testing select-input...
     radio = SelectInput('somelabel', 'somename', 0, options).as_radio()
     actual = HelperHTMLParser.parse(str(radio))
     expected = HelperHTMLParser.parse(f'''
         <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center"
+            <label class="col-sm-4 col-form-label d-flex align-items-center"
                 for="{radio.identifier}">
                 somelabel
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
+            <div class="col-sm-8 d-flex align-items-center">
                 <div class="form-check mr-3">
                     <input id="{option_0.identifier}"
                         name="somename"
                         value=0
                         type="radio"
                         class="form-check-input"
                         autocomplete="off"
@@ -396,19 +396,19 @@
 @pytest.mark.form
 def test_file_input():
     regexp = r'/[\|/]/'
     file = FileInput('somelabel', 'somename').add_classes('someclass')
     actual = HelperHTMLParser.parse(str(file))
     expected = HelperHTMLParser.parse(f'''
         <div class="form-group someclass row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center"
+            <label class="col-sm-4 col-form-label d-flex align-items-center"
                 for="{file.identifier}">
                 somelabel
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
+            <div class="col-sm-8 d-flex align-items-center">
                 <div class="input-group">
                     <span class="form-control input-group-append"></span>
                     <div class="input-group-append">
                         <span class="btn btn-secondary"
                             onclick="$(this).parent().find('input[type=file]').click();">
                             Browse
                         </span>
@@ -424,19 +424,19 @@
     ''')
     assert actual == expected
 
     file = FileInput('somelabel', 'somename').as_disabled()
     actual = HelperHTMLParser.parse(str(file))
     expected = HelperHTMLParser.parse(f'''
         <div class="form-group row">
-            <label class="col-sm-2 col-form-label d-flex align-items-center"
+            <label class="col-sm-4 col-form-label d-flex align-items-center"
                 for="{file.identifier}">
                 somelabel
             </label>
-            <div class="col-sm-10 d-flex align-items-center">
+            <div class="col-sm-8 d-flex align-items-center">
                 <div class="input-group">
                     <span class="form-control input-group-append"></span>
                     <div class="input-group-append">
                         <span class="btn btn-secondary disabled"
                             onclick="$(this).parent().find('input[type=file]').click();">
                             Browse
                         </span>
```

### Comparing `bootwrap-1.0.0/tests/test_helper.py` & `bootwrap-1.0.1/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/tests/test_icon.py` & `bootwrap-1.0.1/tests/test_icon.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/tests/test_image.py` & `bootwrap-1.0.1/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/tests/test_javascript.py` & `bootwrap-1.0.1/tests/test_javascript.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/tests/test_link.py` & `bootwrap-1.0.1/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/tests/test_list.py` & `bootwrap-1.0.1/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/tests/test_menu.py` & `bootwrap-1.0.1/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/tests/test_navigation.py` & `bootwrap-1.0.1/tests/test_navigation.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/tests/test_page.py` & `bootwrap-1.0.1/tests/test_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Test for bootwrap/components/page.py
+Test for bootwrap/page.py
 """
 
 import pytest
 
 from bootwrap import Page, Link, Javascript, Menu, Text
 from .helper import HelperHTMLParser
 
@@ -15,22 +15,31 @@
         resources=[
             Link('https//someresource.com/some.css'),
             Javascript('https//someresource.com/some.js')
         ],
         title='Some Title',
         menu=Menu(logo='somelogo.jpg'),
         container=Text('sometext')
+    ).background(
+        color='somevalue',
+        image='somevalue',
+        position='somevalue',
+        size='somevalue',
+        repeat='somevalue',
+        origin='somevalue',
+        clip='somevalue',
+        attachment='somevalue'
     )
     actual = HelperHTMLParser.parse(page.__html__())
     expected = HelperHTMLParser.parse(f''' 
         <!DOCTYPE html>
         <html lang="en">
             <head>
                 <meta charset="utf-8"/>
-                <meta name="viewport" container="width=device-width, initial-scale=1, shrink-to-fit=no"/>
+                <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no"/>
                 
                 <link rel="stylesheet"
                     type="text/css"
                     href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"/>
                 <link rel="stylesheet"
                     type="text/css"
                     href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.8.2/css/all.min.css"/>
@@ -73,21 +82,22 @@
                         <span class="navbar-toggler-icon"></span>
                     </button>
                     
                     <div class="collapse navbar-collapse" id="menu">
                         <ul class="navbar-nav mr-auto"></ul>
                     </div>
                 </nav>
-                <div class="container" style="margin-top: 90px;">
+                <div class="container-fluid">
                     <span id="...">
                         sometext
                     </span>
                 </div>
             </body>
-            <script>hljs.initHighlightingOnLoad();</script>
+            <script>...</script>
+            <style>...</style>
         </html>
     ''')  # NOQA
     assert actual == expected
 
     with pytest.raises(TypeError):
         Page(resources=[Text('Some Title')]).__html__()
```

### Comparing `bootwrap-1.0.0/tests/test_panel.py` & `bootwrap-1.0.1/tests/test_panel.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/tests/test_table.py` & `bootwrap-1.0.1/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/tests/test_text.py` & `bootwrap-1.0.1/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `bootwrap-1.0.0/tests/test_utils.py` & `bootwrap-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

