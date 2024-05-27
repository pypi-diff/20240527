# Comparing `tmp/warg-1.4.3.tar.gz` & `tmp/warg-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warg-1.4.3.tar", last modified: Mon May 27 10:59:33 2024, max compression
+gzip compressed data, was "warg-1.4.4.tar", last modified: Mon May 27 11:22:47 2024, max compression
```

## Comparing `warg-1.4.3.tar` & `warg-1.4.4.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.233152 warg-1.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.213152 warg-1.4.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-27 10:59:27.000000 warg-1.4.3/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:27.000000 warg-1.4.3/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 10:59:27.000000 warg-1.4.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 10:59:27.000000 warg-1.4.3/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-05-27 10:59:27.000000 warg-1.4.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-27 10:59:27.000000 warg-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-05-27 10:59:33.233152 warg-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-27 10:59:27.000000 warg-1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-27 10:59:27.000000 warg-1.4.3/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.229152 warg-1.4.3/Warg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-05-27 10:59:33.000000 warg-1.4.3/Warg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-27 10:59:33.000000 warg-1.4.3/Warg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 10:59:33.000000 warg-1.4.3/Warg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-27 10:59:33.000000 warg-1.4.3/Warg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 10:59:33.000000 warg-1.4.3/Warg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.213152 warg-1.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-27 10:59:27.000000 warg-1.4.3/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-27 10:59:27.000000 warg-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-27 10:59:27.000000 warg-1.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 10:59:33.233152 warg-1.4.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     7556 2024-05-27 10:59:27.000000 warg-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.213152 warg-1.4.3/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)      506 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1223 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_ast_ops.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_auto_dict.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      570 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_collective.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      408 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2072 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_gdkc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      938 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_iteration.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11703 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_kw_passing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_mapping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       96 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_mixins.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11335 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_nod.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1656 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_post_init.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      643 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.217152 warg-1.4.3/warg/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 10:59:27.000000 warg-1.4.3/warg/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2839 2024-05-27 10:59:27.000000 warg-1.4.3/warg/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5576 2024-05-27 10:59:27.000000 warg-1.4.3/warg/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.217152 warg-1.4.3/warg/ast_ops/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 10:59:27.000000 warg-1.4.3/warg/ast_ops/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      339 2024-05-27 10:59:27.000000 warg-1.4.3/warg/ast_ops/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6097 2024-05-27 10:59:27.000000 warg-1.4.3/warg/ast_ops/arg_indentifier.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10127 2024-05-27 10:59:27.000000 warg-1.4.3/warg/ast_ops/first_arg_identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.217152 warg-1.4.3/warg/bases/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 10:59:27.000000 warg-1.4.3/warg/bases/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      305 2024-05-27 10:59:27.000000 warg-1.4.3/warg/bases/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3398 2024-05-27 10:59:27.000000 warg-1.4.3/warg/bases/property_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4352 2024-05-27 10:59:27.000000 warg-1.4.3/warg/boolean_tests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1027 2024-05-27 10:59:27.000000 warg-1.4.3/warg/business.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.221152 warg-1.4.3/warg/colors/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 10:59:27.000000 warg-1.4.3/warg/colors/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      339 2024-05-27 10:59:27.000000 warg-1.4.3/warg/colors/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1765 2024-05-27 10:59:27.000000 warg-1.4.3/warg/colors/color_conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10205 2024-05-27 10:59:27.000000 warg-1.4.3/warg/colors/css_colors.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      598 2024-05-27 10:59:27.000000 warg-1.4.3/warg/colors/label_colors.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5660 2024-05-27 10:59:27.000000 warg-1.4.3/warg/config_shell.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2700 2024-05-27 10:59:27.000000 warg-1.4.3/warg/context_wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1261 2024-05-27 10:59:27.000000 warg-1.4.3/warg/contexts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.221152 warg-1.4.3/warg/data_structures/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 10:59:27.000000 warg-1.4.3/warg/data_structures/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-27 10:59:27.000000 warg-1.4.3/warg/data_structures/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1825 2024-05-27 10:59:27.000000 warg-1.4.3/warg/data_structures/auto_dict.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3146 2024-05-27 10:59:27.000000 warg-1.4.3/warg/data_structures/mappings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16773 2024-05-27 10:59:27.000000 warg-1.4.3/warg/data_structures/named_ordered_dictionary.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28731 2024-05-27 10:59:27.000000 warg-1.4.3/warg/data_structures/ordered_set.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      513 2024-05-27 10:59:27.000000 warg-1.4.3/warg/data_structures/sequences.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      666 2024-05-27 10:59:27.000000 warg-1.4.3/warg/datetimes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      754 2024-05-27 10:59:27.000000 warg-1.4.3/warg/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.221152 warg-1.4.3/warg/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      415 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.221152 warg-1.4.3/warg/decorators/caching/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/caching/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      333 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/caching/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5267 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/caching/look_up_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2528 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/caching/property_caching.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      629 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/exporting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1570 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/hashing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15454 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/kw_passing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7234 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/timing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/wrapping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1687 2024-05-27 10:59:27.000000 warg-1.4.3/warg/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11719 2024-05-27 10:59:27.000000 warg-1.4.3/warg/functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4335 2024-05-27 10:59:27.000000 warg-1.4.3/warg/gdkc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.225152 warg-1.4.3/warg/generators/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      844 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/cyclic_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/escaping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1931 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/filtering.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2261 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/mapping_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      904 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/numbers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/testing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4358 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/zipping_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-05-27 10:59:27.000000 warg-1.4.3/warg/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-27 10:59:27.000000 warg-1.4.3/warg/logging_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1281 2024-05-27 10:59:27.000000 warg-1.4.3/warg/manipulation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2602 2024-05-27 10:59:27.000000 warg-1.4.3/warg/map_itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.225152 warg-1.4.3/warg/math_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 10:59:27.000000 warg-1.4.3/warg/math_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      343 2024-05-27 10:59:27.000000 warg-1.4.3/warg/math_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      379 2024-05-27 10:59:27.000000 warg-1.4.3/warg/math_utilities/multiples.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1739 2024-05-27 10:59:27.000000 warg-1.4.3/warg/math_utilities/ordinals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1378 2024-05-27 10:59:27.000000 warg-1.4.3/warg/math_utilities/powers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.225152 warg-1.4.3/warg/metas/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 10:59:27.000000 warg-1.4.3/warg/metas/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      322 2024-05-27 10:59:27.000000 warg-1.4.3/warg/metas/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      897 2024-05-27 10:59:27.000000 warg-1.4.3/warg/metas/post_init.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3298 2024-05-27 10:59:27.000000 warg-1.4.3/warg/metas/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.225152 warg-1.4.3/warg/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-27 10:59:27.000000 warg-1.4.3/warg/mixins/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-05-27 10:59:27.000000 warg-1.4.3/warg/mixins/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1052 2024-05-27 10:59:27.000000 warg-1.4.3/warg/mixins/dict_mixins.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      819 2024-05-27 10:59:27.000000 warg-1.4.3/warg/mixins/ordinal_index_mixin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-05-27 10:59:27.000000 warg-1.4.3/warg/mixins/private.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6187 2024-05-27 10:59:27.000000 warg-1.4.3/warg/ode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.229152 warg-1.4.3/warg/os_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 10:59:27.000000 warg-1.4.3/warg/os_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      419 2024-05-27 10:59:27.000000 warg-1.4.3/warg/os_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1963 2024-05-27 10:59:27.000000 warg-1.4.3/warg/os_utilities/filtering.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-05-27 10:59:27.000000 warg-1.4.3/warg/os_utilities/os_platform.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6097 2024-05-27 10:59:27.000000 warg-1.4.3/warg/os_utilities/path_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2598 2024-05-27 10:59:27.000000 warg-1.4.3/warg/os_utilities/path_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2815 2024-05-27 10:59:27.000000 warg-1.4.3/warg/os_utilities/platform_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.229152 warg-1.4.3/warg/packages/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 10:59:27.000000 warg-1.4.3/warg/packages/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      418 2024-05-27 10:59:27.000000 warg-1.4.3/warg/packages/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4975 2024-05-27 10:59:27.000000 warg-1.4.3/warg/packages/editable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-27 10:59:27.000000 warg-1.4.3/warg/packages/namespaces.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2276 2024-05-27 10:59:27.000000 warg-1.4.3/warg/packages/pip_parsing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10370 2024-05-27 10:59:27.000000 warg-1.4.3/warg/packages/reloading.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6303 2024-05-27 10:59:27.000000 warg-1.4.3/warg/packages/satisfaction.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4135 2024-05-27 10:59:27.000000 warg-1.4.3/warg/packages/versioning.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1743 2024-05-27 10:59:27.000000 warg-1.4.3/warg/plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-05-27 10:59:27.000000 warg-1.4.3/warg/replication.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1257 2024-05-27 10:59:27.000000 warg-1.4.3/warg/strings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1138 2024-05-27 10:59:27.000000 warg-1.4.3/warg/text.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2012 2024-05-27 10:59:27.000000 warg-1.4.3/warg/typing_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.459638 warg-1.4.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.435638 warg-1.4.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-27 11:22:39.000000 warg-1.4.4/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:39.000000 warg-1.4.4/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 11:22:39.000000 warg-1.4.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 11:22:40.000000 warg-1.4.4/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-05-27 11:22:40.000000 warg-1.4.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-27 11:22:40.000000 warg-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-05-27 11:22:47.459638 warg-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-27 11:22:40.000000 warg-1.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-27 11:22:40.000000 warg-1.4.4/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.455638 warg-1.4.4/Warg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-05-27 11:22:47.000000 warg-1.4.4/Warg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-27 11:22:47.000000 warg-1.4.4/Warg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:22:47.000000 warg-1.4.4/Warg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-27 11:22:47.000000 warg-1.4.4/Warg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 11:22:47.000000 warg-1.4.4/Warg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.439638 warg-1.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-27 11:22:40.000000 warg-1.4.4/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-27 11:22:40.000000 warg-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-27 11:22:40.000000 warg-1.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 11:22:47.463638 warg-1.4.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7556 2024-05-27 11:22:40.000000 warg-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.439638 warg-1.4.4/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      506 2024-05-27 11:22:40.000000 warg-1.4.4/tests/test_arguments.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1223 2024-05-27 11:22:40.000000 warg-1.4.4/tests/test_ast_ops.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-05-27 11:22:40.000000 warg-1.4.4/tests/test_auto_dict.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      570 2024-05-27 11:22:40.000000 warg-1.4.4/tests/test_collective.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      408 2024-05-27 11:22:40.000000 warg-1.4.4/tests/test_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2072 2024-05-27 11:22:40.000000 warg-1.4.4/tests/test_gdkc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      938 2024-05-27 11:22:40.000000 warg-1.4.4/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-27 11:22:40.000000 warg-1.4.4/tests/test_iteration.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11703 2024-05-27 11:22:40.000000 warg-1.4.4/tests/test_kw_passing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:40.000000 warg-1.4.4/tests/test_mapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       96 2024-05-27 11:22:40.000000 warg-1.4.4/tests/test_mixins.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11335 2024-05-27 11:22:40.000000 warg-1.4.4/tests/test_nod.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1656 2024-05-27 11:22:40.000000 warg-1.4.4/tests/test_post_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      643 2024-05-27 11:22:40.000000 warg-1.4.4/tests/test_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.443638 warg-1.4.4/warg/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 11:22:40.000000 warg-1.4.4/warg/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2839 2024-05-27 11:22:40.000000 warg-1.4.4/warg/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5576 2024-05-27 11:22:40.000000 warg-1.4.4/warg/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.443638 warg-1.4.4/warg/ast_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 11:22:40.000000 warg-1.4.4/warg/ast_ops/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      339 2024-05-27 11:22:40.000000 warg-1.4.4/warg/ast_ops/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6097 2024-05-27 11:22:40.000000 warg-1.4.4/warg/ast_ops/arg_indentifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10127 2024-05-27 11:22:40.000000 warg-1.4.4/warg/ast_ops/first_arg_identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.447638 warg-1.4.4/warg/bases/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 11:22:40.000000 warg-1.4.4/warg/bases/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      305 2024-05-27 11:22:40.000000 warg-1.4.4/warg/bases/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3398 2024-05-27 11:22:40.000000 warg-1.4.4/warg/bases/property_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4352 2024-05-27 11:22:40.000000 warg-1.4.4/warg/boolean_tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1027 2024-05-27 11:22:40.000000 warg-1.4.4/warg/business.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.447638 warg-1.4.4/warg/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 11:22:40.000000 warg-1.4.4/warg/colors/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      339 2024-05-27 11:22:40.000000 warg-1.4.4/warg/colors/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1765 2024-05-27 11:22:40.000000 warg-1.4.4/warg/colors/color_conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10205 2024-05-27 11:22:40.000000 warg-1.4.4/warg/colors/css_colors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      598 2024-05-27 11:22:40.000000 warg-1.4.4/warg/colors/label_colors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5660 2024-05-27 11:22:40.000000 warg-1.4.4/warg/config_shell.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2700 2024-05-27 11:22:40.000000 warg-1.4.4/warg/context_wrapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1261 2024-05-27 11:22:40.000000 warg-1.4.4/warg/contexts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.447638 warg-1.4.4/warg/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 11:22:40.000000 warg-1.4.4/warg/data_structures/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-27 11:22:40.000000 warg-1.4.4/warg/data_structures/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1825 2024-05-27 11:22:40.000000 warg-1.4.4/warg/data_structures/auto_dict.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3277 2024-05-27 11:22:40.000000 warg-1.4.4/warg/data_structures/mappings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16773 2024-05-27 11:22:40.000000 warg-1.4.4/warg/data_structures/named_ordered_dictionary.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28731 2024-05-27 11:22:40.000000 warg-1.4.4/warg/data_structures/ordered_set.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      513 2024-05-27 11:22:40.000000 warg-1.4.4/warg/data_structures/sequences.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      666 2024-05-27 11:22:40.000000 warg-1.4.4/warg/datetimes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      754 2024-05-27 11:22:40.000000 warg-1.4.4/warg/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.447638 warg-1.4.4/warg/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 11:22:40.000000 warg-1.4.4/warg/decorators/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      415 2024-05-27 11:22:40.000000 warg-1.4.4/warg/decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.451638 warg-1.4.4/warg/decorators/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 11:22:40.000000 warg-1.4.4/warg/decorators/caching/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      333 2024-05-27 11:22:40.000000 warg-1.4.4/warg/decorators/caching/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5267 2024-05-27 11:22:40.000000 warg-1.4.4/warg/decorators/caching/look_up_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2528 2024-05-27 11:22:40.000000 warg-1.4.4/warg/decorators/caching/property_caching.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      629 2024-05-27 11:22:40.000000 warg-1.4.4/warg/decorators/exporting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1570 2024-05-27 11:22:40.000000 warg-1.4.4/warg/decorators/hashing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15454 2024-05-27 11:22:40.000000 warg-1.4.4/warg/decorators/kw_passing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7234 2024-05-27 11:22:40.000000 warg-1.4.4/warg/decorators/timing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-05-27 11:22:40.000000 warg-1.4.4/warg/decorators/wrapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1687 2024-05-27 11:22:40.000000 warg-1.4.4/warg/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11719 2024-05-27 11:22:40.000000 warg-1.4.4/warg/functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4335 2024-05-27 11:22:40.000000 warg-1.4.4/warg/gdkc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.451638 warg-1.4.4/warg/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 11:22:40.000000 warg-1.4.4/warg/generators/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-05-27 11:22:40.000000 warg-1.4.4/warg/generators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      844 2024-05-27 11:22:40.000000 warg-1.4.4/warg/generators/cyclic_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-27 11:22:40.000000 warg-1.4.4/warg/generators/escaping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1931 2024-05-27 11:22:40.000000 warg-1.4.4/warg/generators/filtering.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2261 2024-05-27 11:22:40.000000 warg-1.4.4/warg/generators/mapping_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      904 2024-05-27 11:22:40.000000 warg-1.4.4/warg/generators/numbers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-05-27 11:22:40.000000 warg-1.4.4/warg/generators/testing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4358 2024-05-27 11:22:40.000000 warg-1.4.4/warg/generators/zipping_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-05-27 11:22:40.000000 warg-1.4.4/warg/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-27 11:22:40.000000 warg-1.4.4/warg/logging_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1281 2024-05-27 11:22:40.000000 warg-1.4.4/warg/manipulation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2602 2024-05-27 11:22:40.000000 warg-1.4.4/warg/map_itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.451638 warg-1.4.4/warg/math_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 11:22:40.000000 warg-1.4.4/warg/math_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      343 2024-05-27 11:22:40.000000 warg-1.4.4/warg/math_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      379 2024-05-27 11:22:40.000000 warg-1.4.4/warg/math_utilities/multiples.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1739 2024-05-27 11:22:40.000000 warg-1.4.4/warg/math_utilities/ordinals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1378 2024-05-27 11:22:40.000000 warg-1.4.4/warg/math_utilities/powers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.451638 warg-1.4.4/warg/metas/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 11:22:40.000000 warg-1.4.4/warg/metas/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      322 2024-05-27 11:22:40.000000 warg-1.4.4/warg/metas/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      897 2024-05-27 11:22:40.000000 warg-1.4.4/warg/metas/post_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3298 2024-05-27 11:22:40.000000 warg-1.4.4/warg/metas/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.455638 warg-1.4.4/warg/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-27 11:22:40.000000 warg-1.4.4/warg/mixins/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-05-27 11:22:40.000000 warg-1.4.4/warg/mixins/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1052 2024-05-27 11:22:40.000000 warg-1.4.4/warg/mixins/dict_mixins.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      819 2024-05-27 11:22:40.000000 warg-1.4.4/warg/mixins/ordinal_index_mixin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-05-27 11:22:40.000000 warg-1.4.4/warg/mixins/private.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6187 2024-05-27 11:22:40.000000 warg-1.4.4/warg/ode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.455638 warg-1.4.4/warg/os_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 11:22:40.000000 warg-1.4.4/warg/os_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      419 2024-05-27 11:22:40.000000 warg-1.4.4/warg/os_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1963 2024-05-27 11:22:40.000000 warg-1.4.4/warg/os_utilities/filtering.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-05-27 11:22:40.000000 warg-1.4.4/warg/os_utilities/os_platform.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6097 2024-05-27 11:22:40.000000 warg-1.4.4/warg/os_utilities/path_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2598 2024-05-27 11:22:40.000000 warg-1.4.4/warg/os_utilities/path_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2815 2024-05-27 11:22:40.000000 warg-1.4.4/warg/os_utilities/platform_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:47.455638 warg-1.4.4/warg/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 11:22:40.000000 warg-1.4.4/warg/packages/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      418 2024-05-27 11:22:40.000000 warg-1.4.4/warg/packages/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4975 2024-05-27 11:22:40.000000 warg-1.4.4/warg/packages/editable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-27 11:22:40.000000 warg-1.4.4/warg/packages/namespaces.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2276 2024-05-27 11:22:40.000000 warg-1.4.4/warg/packages/pip_parsing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10370 2024-05-27 11:22:40.000000 warg-1.4.4/warg/packages/reloading.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6303 2024-05-27 11:22:40.000000 warg-1.4.4/warg/packages/satisfaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4135 2024-05-27 11:22:40.000000 warg-1.4.4/warg/packages/versioning.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1743 2024-05-27 11:22:40.000000 warg-1.4.4/warg/plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-05-27 11:22:40.000000 warg-1.4.4/warg/replication.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1257 2024-05-27 11:22:40.000000 warg-1.4.4/warg/strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1138 2024-05-27 11:22:40.000000 warg-1.4.4/warg/text.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2012 2024-05-27 11:22:40.000000 warg-1.4.4/warg/typing_extension.py
```

### Comparing `warg-1.4.3/.github/CODE_OF_CONDUCT.md` & `warg-1.4.4/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/LICENSE.md` & `warg-1.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/PKG-INFO` & `warg-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Warg
-Version: 1.4.3
+Version: 1.4.4
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/warg
 Download-URL: https://github.com/pything/warg/releases
 Author: Christian Heider Lindbjerg
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Lindbjerg
 Maintainer-email: christian.heider@alexandra.dk
@@ -27,46 +27,46 @@
 Provides-Extra: setup
 Requires-Dist: pytest-runner; extra == "setup"
 Provides-Extra: tests
 Requires-Dist: pytest>=4.3.0; extra == "tests"
 Requires-Dist: pytest-cov>=2.6.1; extra == "tests"
 Requires-Dist: tox; extra == "tests"
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
-Requires-Dist: apppath; extra == "docs"
 Requires-Dist: warg; extra == "docs"
-Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: apppath; extra == "docs"
 Provides-Extra: dev
-Requires-Dist: pytest>=4.3.0; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: black>=18.9b0; extra == "dev"
 Requires-Dist: pytest-runner; extra == "dev"
-Requires-Dist: twine>=1.13.0; extra == "dev"
 Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
-Requires-Dist: black>=18.9b0; extra == "dev"
 Requires-Dist: coveralls>=1.6.0; extra == "dev"
-Requires-Dist: pytest-cov>=2.6.1; extra == "dev"
-Requires-Dist: apppath; extra == "dev"
 Requires-Dist: wheel>=0.38.0; extra == "dev"
-Requires-Dist: warg; extra == "dev"
-Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: pytest-cov>=2.6.1; extra == "dev"
 Requires-Dist: pip>=19.0.3; extra == "dev"
+Requires-Dist: warg; extra == "dev"
+Requires-Dist: apppath; extra == "dev"
 Requires-Dist: tox; extra == "dev"
+Requires-Dist: pytest>=4.3.0; extra == "dev"
+Requires-Dist: twine>=1.13.0; extra == "dev"
 Provides-Extra: all
-Requires-Dist: pytest>=4.3.0; extra == "all"
+Requires-Dist: sphinx; extra == "all"
+Requires-Dist: coveralls>=1.6.0; extra == "all"
+Requires-Dist: black>=18.9b0; extra == "all"
 Requires-Dist: pytest-runner; extra == "all"
-Requires-Dist: twine>=1.13.0; extra == "all"
 Requires-Dist: sphinxcontrib-programoutput; extra == "all"
-Requires-Dist: black>=18.9b0; extra == "all"
-Requires-Dist: coveralls>=1.6.0; extra == "all"
-Requires-Dist: pytest-cov>=2.6.1; extra == "all"
-Requires-Dist: apppath; extra == "all"
 Requires-Dist: wheel>=0.38.0; extra == "all"
-Requires-Dist: warg; extra == "all"
-Requires-Dist: sphinx; extra == "all"
+Requires-Dist: pytest-cov>=2.6.1; extra == "all"
 Requires-Dist: pip>=19.0.3; extra == "all"
+Requires-Dist: warg; extra == "all"
+Requires-Dist: apppath; extra == "all"
 Requires-Dist: tox; extra == "all"
+Requires-Dist: pytest>=4.3.0; extra == "all"
+Requires-Dist: twine>=1.13.0; extra == "all"
 
 <!--![warg](.github/images/warg.svg)-->
 
 <p align="center">
   <img src=".github/images/warg.svg" alt='Warg' />
 </p>
```

### Comparing `warg-1.4.3/README.md` & `warg-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/SECURITY.md` & `warg-1.4.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/Warg.egg-info/PKG-INFO` & `warg-1.4.4/Warg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Warg
-Version: 1.4.3
+Version: 1.4.4
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/warg
 Download-URL: https://github.com/pything/warg/releases
 Author: Christian Heider Lindbjerg
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Lindbjerg
 Maintainer-email: christian.heider@alexandra.dk
@@ -27,46 +27,46 @@
 Provides-Extra: setup
 Requires-Dist: pytest-runner; extra == "setup"
 Provides-Extra: tests
 Requires-Dist: pytest>=4.3.0; extra == "tests"
 Requires-Dist: pytest-cov>=2.6.1; extra == "tests"
 Requires-Dist: tox; extra == "tests"
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
-Requires-Dist: apppath; extra == "docs"
 Requires-Dist: warg; extra == "docs"
-Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: apppath; extra == "docs"
 Provides-Extra: dev
-Requires-Dist: pytest>=4.3.0; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: black>=18.9b0; extra == "dev"
 Requires-Dist: pytest-runner; extra == "dev"
-Requires-Dist: twine>=1.13.0; extra == "dev"
 Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
-Requires-Dist: black>=18.9b0; extra == "dev"
 Requires-Dist: coveralls>=1.6.0; extra == "dev"
-Requires-Dist: pytest-cov>=2.6.1; extra == "dev"
-Requires-Dist: apppath; extra == "dev"
 Requires-Dist: wheel>=0.38.0; extra == "dev"
-Requires-Dist: warg; extra == "dev"
-Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: pytest-cov>=2.6.1; extra == "dev"
 Requires-Dist: pip>=19.0.3; extra == "dev"
+Requires-Dist: warg; extra == "dev"
+Requires-Dist: apppath; extra == "dev"
 Requires-Dist: tox; extra == "dev"
+Requires-Dist: pytest>=4.3.0; extra == "dev"
+Requires-Dist: twine>=1.13.0; extra == "dev"
 Provides-Extra: all
-Requires-Dist: pytest>=4.3.0; extra == "all"
+Requires-Dist: sphinx; extra == "all"
+Requires-Dist: coveralls>=1.6.0; extra == "all"
+Requires-Dist: black>=18.9b0; extra == "all"
 Requires-Dist: pytest-runner; extra == "all"
-Requires-Dist: twine>=1.13.0; extra == "all"
 Requires-Dist: sphinxcontrib-programoutput; extra == "all"
-Requires-Dist: black>=18.9b0; extra == "all"
-Requires-Dist: coveralls>=1.6.0; extra == "all"
-Requires-Dist: pytest-cov>=2.6.1; extra == "all"
-Requires-Dist: apppath; extra == "all"
 Requires-Dist: wheel>=0.38.0; extra == "all"
-Requires-Dist: warg; extra == "all"
-Requires-Dist: sphinx; extra == "all"
+Requires-Dist: pytest-cov>=2.6.1; extra == "all"
 Requires-Dist: pip>=19.0.3; extra == "all"
+Requires-Dist: warg; extra == "all"
+Requires-Dist: apppath; extra == "all"
 Requires-Dist: tox; extra == "all"
+Requires-Dist: pytest>=4.3.0; extra == "all"
+Requires-Dist: twine>=1.13.0; extra == "all"
 
 <!--![warg](.github/images/warg.svg)-->
 
 <p align="center">
   <img src=".github/images/warg.svg" alt='Warg' />
 </p>
```

### Comparing `warg-1.4.3/Warg.egg-info/SOURCES.txt` & `warg-1.4.4/Warg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/pyproject.toml` & `warg-1.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/setup.py` & `warg-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/tests/test_ast_ops.py` & `warg-1.4.4/tests/test_ast_ops.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/tests/test_auto_dict.py` & `warg-1.4.4/tests/test_auto_dict.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/tests/test_collective.py` & `warg-1.4.4/tests/test_collective.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/tests/test_gdkc.py` & `warg-1.4.4/tests/test_gdkc.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/tests/test_imports.py` & `warg-1.4.4/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/tests/test_iteration.py` & `warg-1.4.4/tests/test_iteration.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/tests/test_kw_passing.py` & `warg-1.4.4/tests/test_kw_passing.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/tests/test_nod.py` & `warg-1.4.4/tests/test_nod.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/tests/test_post_init.py` & `warg-1.4.4/tests/test_post_init.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/tests/test_singleton.py` & `warg-1.4.4/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/__init__.py` & `warg-1.4.4/warg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     from importlib_metadata import PackageNotFoundError
     from importlib_resources import files
 
 
 __project__ = "Warg"
 
 __author__ = "Christian Heider Lindbjerg"
-__version__ = "1.4.3"
+__version__ = "1.4.4"
 __doc__ = r"""
 Created on 27/04/2019
 
 @author: cnheider
 
 """
```

### Comparing `warg-1.4.3/warg/arguments.py` & `warg-1.4.4/warg/arguments.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/ast_ops/arg_indentifier.py` & `warg-1.4.4/warg/ast_ops/arg_indentifier.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/ast_ops/first_arg_identifier.py` & `warg-1.4.4/warg/ast_ops/first_arg_identifier.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/bases/property_settings.py` & `warg-1.4.4/warg/bases/property_settings.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/boolean_tests.py` & `warg-1.4.4/warg/boolean_tests.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/business.py` & `warg-1.4.4/warg/business.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/colors/color_conversion.py` & `warg-1.4.4/warg/colors/color_conversion.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/colors/css_colors.py` & `warg-1.4.4/warg/colors/css_colors.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/colors/label_colors.py` & `warg-1.4.4/warg/colors/label_colors.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/config_shell.py` & `warg-1.4.4/warg/config_shell.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/context_wrapper.py` & `warg-1.4.4/warg/context_wrapper.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/contexts.py` & `warg-1.4.4/warg/contexts.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/data_structures/auto_dict.py` & `warg-1.4.4/warg/data_structures/auto_dict.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/data_structures/mappings.py` & `warg-1.4.4/warg/data_structures/mappings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-from typing import Callable, Dict, Hashable, Iterable, Mapping, MutableMapping
+from typing import Callable, Collection, Dict, Hashable, Iterable, Mapping, MutableMapping
 
 __all__ = [
     "invert_mapping",
     "invert_dict",
     "AppendingDict",
     "pivot_dict_object",
     "pivot_dict",
@@ -107,14 +107,16 @@
 
 
 def to_dict(m: Mapping) -> dict:
     o = {}
     for k, v in m.items():
         if isinstance(v, Mapping):
             o[k] = to_dict(v)
+        elif isinstance(v, Collection):
+            o[k] = [to_dict(v_) if isinstance(v, Mapping) else v_ for v_ in v]
         else:
             o[k] = v
     return o
 
 
 if __name__ == "__main__":
     print(invert_mapping({"a": 1, "b": 2}))
```

### Comparing `warg-1.4.3/warg/data_structures/named_ordered_dictionary.py` & `warg-1.4.4/warg/data_structures/named_ordered_dictionary.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/data_structures/ordered_set.py` & `warg-1.4.4/warg/data_structures/ordered_set.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/data_structures/sequences.py` & `warg-1.4.4/warg/data_structures/sequences.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/datetimes.py` & `warg-1.4.4/warg/datetimes.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/debug.py` & `warg-1.4.4/warg/debug.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/decorators/caching/look_up_table.py` & `warg-1.4.4/warg/decorators/caching/look_up_table.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/decorators/caching/property_caching.py` & `warg-1.4.4/warg/decorators/caching/property_caching.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/decorators/exporting.py` & `warg-1.4.4/warg/decorators/exporting.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/decorators/hashing.py` & `warg-1.4.4/warg/decorators/hashing.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/decorators/kw_passing.py` & `warg-1.4.4/warg/decorators/kw_passing.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/decorators/timing.py` & `warg-1.4.4/warg/decorators/timing.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/decorators/wrapping.py` & `warg-1.4.4/warg/decorators/wrapping.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/exceptions.py` & `warg-1.4.4/warg/exceptions.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/functions.py` & `warg-1.4.4/warg/functions.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/gdkc.py` & `warg-1.4.4/warg/gdkc.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/generators/cyclic_generators.py` & `warg-1.4.4/warg/generators/cyclic_generators.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/generators/escaping.py` & `warg-1.4.4/warg/generators/escaping.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/generators/filtering.py` & `warg-1.4.4/warg/generators/filtering.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/generators/mapping_generator.py` & `warg-1.4.4/warg/generators/mapping_generator.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/generators/numbers.py` & `warg-1.4.4/warg/generators/numbers.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/generators/zipping_generator.py` & `warg-1.4.4/warg/generators/zipping_generator.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/iteration.py` & `warg-1.4.4/warg/iteration.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/logging_utilities.py` & `warg-1.4.4/warg/logging_utilities.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/manipulation.py` & `warg-1.4.4/warg/manipulation.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/map_itertools.py` & `warg-1.4.4/warg/map_itertools.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/math_utilities/ordinals.py` & `warg-1.4.4/warg/math_utilities/ordinals.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/math_utilities/powers.py` & `warg-1.4.4/warg/math_utilities/powers.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/metas/post_init.py` & `warg-1.4.4/warg/metas/post_init.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/metas/singleton.py` & `warg-1.4.4/warg/metas/singleton.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/mixins/dict_mixins.py` & `warg-1.4.4/warg/mixins/dict_mixins.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/mixins/ordinal_index_mixin.py` & `warg-1.4.4/warg/mixins/ordinal_index_mixin.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/ode.py` & `warg-1.4.4/warg/ode.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/os_utilities/filtering.py` & `warg-1.4.4/warg/os_utilities/filtering.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/os_utilities/os_platform.py` & `warg-1.4.4/warg/os_utilities/os_platform.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/os_utilities/path_functions.py` & `warg-1.4.4/warg/os_utilities/path_functions.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/os_utilities/path_utilities.py` & `warg-1.4.4/warg/os_utilities/path_utilities.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/os_utilities/platform_selection.py` & `warg-1.4.4/warg/os_utilities/platform_selection.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/packages/editable.py` & `warg-1.4.4/warg/packages/editable.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/packages/namespaces.py` & `warg-1.4.4/warg/packages/namespaces.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/packages/pip_parsing.py` & `warg-1.4.4/warg/packages/pip_parsing.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/packages/reloading.py` & `warg-1.4.4/warg/packages/reloading.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/packages/satisfaction.py` & `warg-1.4.4/warg/packages/satisfaction.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/packages/versioning.py` & `warg-1.4.4/warg/packages/versioning.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/plugin.py` & `warg-1.4.4/warg/plugin.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/replication.py` & `warg-1.4.4/warg/replication.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/strings.py` & `warg-1.4.4/warg/strings.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/text.py` & `warg-1.4.4/warg/text.py`

 * *Files identical despite different names*

### Comparing `warg-1.4.3/warg/typing_extension.py` & `warg-1.4.4/warg/typing_extension.py`

 * *Files identical despite different names*

