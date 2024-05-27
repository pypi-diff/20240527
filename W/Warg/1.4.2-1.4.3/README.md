# Comparing `tmp/Warg-1.4.2.tar.gz` & `tmp/warg-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Warg-1.4.2.tar", last modified: Tue Feb 27 12:07:27 2024, max compression
+gzip compressed data, was "warg-1.4.3.tar", last modified: Mon May 27 10:59:33 2024, max compression
```

## Comparing `Warg-1.4.2.tar` & `warg-1.4.3.tar`

### file list

```diff
@@ -1,141 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.955745 Warg-1.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.927745 Warg-1.4.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-02-27 12:07:24.000000 Warg-1.4.2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:24.000000 Warg-1.4.2/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-27 12:07:24.000000 Warg-1.4.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-27 12:07:24.000000 Warg-1.4.2/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-02-27 12:07:24.000000 Warg-1.4.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-27 12:07:24.000000 Warg-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-02-27 12:07:27.955745 Warg-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-02-27 12:07:24.000000 Warg-1.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-27 12:07:24.000000 Warg-1.4.2/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.951745 Warg-1.4.2/Warg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-02-27 12:07:27.000000 Warg-1.4.2/Warg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-02-27 12:07:27.000000 Warg-1.4.2/Warg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 12:07:27.000000 Warg-1.4.2/Warg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-02-27 12:07:27.000000 Warg-1.4.2/Warg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-27 12:07:27.000000 Warg-1.4.2/Warg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.931745 Warg-1.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-27 12:07:24.000000 Warg-1.4.2/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-02-27 12:07:24.000000 Warg-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-27 12:07:24.000000 Warg-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-27 12:07:27.955745 Warg-1.4.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     7556 2024-02-27 12:07:24.000000 Warg-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.931745 Warg-1.4.2/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)      506 2024-02-27 12:07:24.000000 Warg-1.4.2/tests/test_arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1223 2024-02-27 12:07:24.000000 Warg-1.4.2/tests/test_ast_ops.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      946 2024-02-27 12:07:24.000000 Warg-1.4.2/tests/test_auto_dict.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      570 2024-02-27 12:07:24.000000 Warg-1.4.2/tests/test_collective.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      408 2024-02-27 12:07:24.000000 Warg-1.4.2/tests/test_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2072 2024-02-27 12:07:24.000000 Warg-1.4.2/tests/test_gdkc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      938 2024-02-27 12:07:24.000000 Warg-1.4.2/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-02-27 12:07:24.000000 Warg-1.4.2/tests/test_iteration.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11703 2024-02-27 12:07:24.000000 Warg-1.4.2/tests/test_kw_passing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:24.000000 Warg-1.4.2/tests/test_mapping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       96 2024-02-27 12:07:24.000000 Warg-1.4.2/tests/test_mixins.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11335 2024-02-27 12:07:24.000000 Warg-1.4.2/tests/test_nod.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1656 2024-02-27 12:07:24.000000 Warg-1.4.2/tests/test_post_init.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      643 2024-02-27 12:07:24.000000 Warg-1.4.2/tests/test_singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.935745 Warg-1.4.2/warg/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2802 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5557 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.939745 Warg-1.4.2/warg/ast_ops/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/ast_ops/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      339 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/ast_ops/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6097 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/ast_ops/arg_indentifier.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10127 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/ast_ops/first_arg_identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.939745 Warg-1.4.2/warg/bases/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/bases/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      305 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/bases/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3398 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/bases/property_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4352 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/boolean_tests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1027 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/business.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.939745 Warg-1.4.2/warg/colors/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/colors/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      339 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/colors/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1765 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/colors/color_conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10205 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/colors/css_colors.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      598 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/colors/label_colors.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5660 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/config_shell.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2700 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/context_wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1261 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/contexts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.939745 Warg-1.4.2/warg/data_structures/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/data_structures/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/data_structures/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1825 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/data_structures/auto_dict.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2778 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/data_structures/mappings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16620 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/data_structures/named_ordered_dictionary.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28731 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/data_structures/ordered_set.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      513 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/data_structures/sequences.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      666 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/datetimes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      754 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.943745 Warg-1.4.2/warg/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/decorators/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      415 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.943745 Warg-1.4.2/warg/decorators/caching/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/decorators/caching/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      333 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/decorators/caching/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5304 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/decorators/caching/look_up_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2528 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/decorators/caching/property_caching.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      629 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/decorators/exporting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1570 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/decorators/hashing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15444 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/decorators/kw_passing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7234 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/decorators/timing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/decorators/wrapping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1687 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10477 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4297 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/gdkc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.943745 Warg-1.4.2/warg/generators/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/generators/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/generators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      844 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/generators/cyclic_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/generators/escaping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1931 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/generators/filtering.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2261 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/generators/mapping_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      904 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/generators/numbers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/generators/testing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4358 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/generators/zipping_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/iteration.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1281 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/manipulation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2638 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/map_itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.947745 Warg-1.4.2/warg/math_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/math_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      343 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/math_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      379 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/math_utilities/multiples.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1739 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/math_utilities/ordinals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1378 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/math_utilities/powers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.947745 Warg-1.4.2/warg/metas/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/metas/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      322 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/metas/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      897 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/metas/post_init.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3298 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/metas/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.947745 Warg-1.4.2/warg/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/mixins/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/mixins/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1052 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/mixins/dict_mixins.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      819 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/mixins/ordinal_index_mixin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/mixins/private.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6187 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/ode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.947745 Warg-1.4.2/warg/os_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/os_utilities/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      419 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/os_utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1963 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/os_utilities/filtering.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/os_utilities/os_platform.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6098 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/os_utilities/path_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2598 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/os_utilities/path_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2815 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/os_utilities/platform_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 12:07:27.951745 Warg-1.4.2/warg/packages/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/packages/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      418 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/packages/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4940 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/packages/editable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/packages/namespaces.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2240 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/packages/pip_parsing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10335 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/packages/reloading.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5376 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/packages/satisfaction.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4040 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/packages/versioning.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1743 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/replication.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1257 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/strings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1138 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/text.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2012 2024-02-27 12:07:24.000000 Warg-1.4.2/warg/typing_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.233152 warg-1.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.213152 warg-1.4.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-27 10:59:27.000000 warg-1.4.3/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:27.000000 warg-1.4.3/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 10:59:27.000000 warg-1.4.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 10:59:27.000000 warg-1.4.3/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-05-27 10:59:27.000000 warg-1.4.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-27 10:59:27.000000 warg-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-05-27 10:59:33.233152 warg-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-27 10:59:27.000000 warg-1.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-27 10:59:27.000000 warg-1.4.3/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.229152 warg-1.4.3/Warg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-05-27 10:59:33.000000 warg-1.4.3/Warg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-27 10:59:33.000000 warg-1.4.3/Warg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 10:59:33.000000 warg-1.4.3/Warg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-27 10:59:33.000000 warg-1.4.3/Warg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 10:59:33.000000 warg-1.4.3/Warg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.213152 warg-1.4.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-27 10:59:27.000000 warg-1.4.3/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-27 10:59:27.000000 warg-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-27 10:59:27.000000 warg-1.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 10:59:33.233152 warg-1.4.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7556 2024-05-27 10:59:27.000000 warg-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.213152 warg-1.4.3/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      506 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_arguments.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1223 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_ast_ops.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_auto_dict.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      570 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_collective.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      408 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2072 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_gdkc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      938 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_iteration.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11703 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_kw_passing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_mapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       96 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_mixins.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11335 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_nod.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1656 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_post_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      643 2024-05-27 10:59:27.000000 warg-1.4.3/tests/test_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.217152 warg-1.4.3/warg/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 10:59:27.000000 warg-1.4.3/warg/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2839 2024-05-27 10:59:27.000000 warg-1.4.3/warg/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5576 2024-05-27 10:59:27.000000 warg-1.4.3/warg/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.217152 warg-1.4.3/warg/ast_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 10:59:27.000000 warg-1.4.3/warg/ast_ops/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      339 2024-05-27 10:59:27.000000 warg-1.4.3/warg/ast_ops/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6097 2024-05-27 10:59:27.000000 warg-1.4.3/warg/ast_ops/arg_indentifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10127 2024-05-27 10:59:27.000000 warg-1.4.3/warg/ast_ops/first_arg_identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.217152 warg-1.4.3/warg/bases/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 10:59:27.000000 warg-1.4.3/warg/bases/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      305 2024-05-27 10:59:27.000000 warg-1.4.3/warg/bases/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3398 2024-05-27 10:59:27.000000 warg-1.4.3/warg/bases/property_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4352 2024-05-27 10:59:27.000000 warg-1.4.3/warg/boolean_tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1027 2024-05-27 10:59:27.000000 warg-1.4.3/warg/business.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.221152 warg-1.4.3/warg/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 10:59:27.000000 warg-1.4.3/warg/colors/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      339 2024-05-27 10:59:27.000000 warg-1.4.3/warg/colors/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1765 2024-05-27 10:59:27.000000 warg-1.4.3/warg/colors/color_conversion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10205 2024-05-27 10:59:27.000000 warg-1.4.3/warg/colors/css_colors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      598 2024-05-27 10:59:27.000000 warg-1.4.3/warg/colors/label_colors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5660 2024-05-27 10:59:27.000000 warg-1.4.3/warg/config_shell.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2700 2024-05-27 10:59:27.000000 warg-1.4.3/warg/context_wrapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1261 2024-05-27 10:59:27.000000 warg-1.4.3/warg/contexts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.221152 warg-1.4.3/warg/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 10:59:27.000000 warg-1.4.3/warg/data_structures/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-27 10:59:27.000000 warg-1.4.3/warg/data_structures/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1825 2024-05-27 10:59:27.000000 warg-1.4.3/warg/data_structures/auto_dict.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3146 2024-05-27 10:59:27.000000 warg-1.4.3/warg/data_structures/mappings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16773 2024-05-27 10:59:27.000000 warg-1.4.3/warg/data_structures/named_ordered_dictionary.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28731 2024-05-27 10:59:27.000000 warg-1.4.3/warg/data_structures/ordered_set.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      513 2024-05-27 10:59:27.000000 warg-1.4.3/warg/data_structures/sequences.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      666 2024-05-27 10:59:27.000000 warg-1.4.3/warg/datetimes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      754 2024-05-27 10:59:27.000000 warg-1.4.3/warg/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.221152 warg-1.4.3/warg/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      415 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.221152 warg-1.4.3/warg/decorators/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/caching/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      333 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/caching/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5267 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/caching/look_up_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2528 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/caching/property_caching.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      629 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/exporting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1570 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/hashing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15454 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/kw_passing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7234 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/timing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-05-27 10:59:27.000000 warg-1.4.3/warg/decorators/wrapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1687 2024-05-27 10:59:27.000000 warg-1.4.3/warg/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11719 2024-05-27 10:59:27.000000 warg-1.4.3/warg/functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4335 2024-05-27 10:59:27.000000 warg-1.4.3/warg/gdkc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.225152 warg-1.4.3/warg/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      844 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/cyclic_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/escaping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1931 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/filtering.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2261 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/mapping_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      904 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/numbers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/testing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4358 2024-05-27 10:59:27.000000 warg-1.4.3/warg/generators/zipping_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-05-27 10:59:27.000000 warg-1.4.3/warg/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-27 10:59:27.000000 warg-1.4.3/warg/logging_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1281 2024-05-27 10:59:27.000000 warg-1.4.3/warg/manipulation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2602 2024-05-27 10:59:27.000000 warg-1.4.3/warg/map_itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.225152 warg-1.4.3/warg/math_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 10:59:27.000000 warg-1.4.3/warg/math_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      343 2024-05-27 10:59:27.000000 warg-1.4.3/warg/math_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      379 2024-05-27 10:59:27.000000 warg-1.4.3/warg/math_utilities/multiples.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1739 2024-05-27 10:59:27.000000 warg-1.4.3/warg/math_utilities/ordinals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1378 2024-05-27 10:59:27.000000 warg-1.4.3/warg/math_utilities/powers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.225152 warg-1.4.3/warg/metas/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 10:59:27.000000 warg-1.4.3/warg/metas/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      322 2024-05-27 10:59:27.000000 warg-1.4.3/warg/metas/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      897 2024-05-27 10:59:27.000000 warg-1.4.3/warg/metas/post_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3298 2024-05-27 10:59:27.000000 warg-1.4.3/warg/metas/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.225152 warg-1.4.3/warg/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-27 10:59:27.000000 warg-1.4.3/warg/mixins/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-05-27 10:59:27.000000 warg-1.4.3/warg/mixins/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1052 2024-05-27 10:59:27.000000 warg-1.4.3/warg/mixins/dict_mixins.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      819 2024-05-27 10:59:27.000000 warg-1.4.3/warg/mixins/ordinal_index_mixin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-05-27 10:59:27.000000 warg-1.4.3/warg/mixins/private.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6187 2024-05-27 10:59:27.000000 warg-1.4.3/warg/ode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.229152 warg-1.4.3/warg/os_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 10:59:27.000000 warg-1.4.3/warg/os_utilities/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      419 2024-05-27 10:59:27.000000 warg-1.4.3/warg/os_utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1963 2024-05-27 10:59:27.000000 warg-1.4.3/warg/os_utilities/filtering.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-05-27 10:59:27.000000 warg-1.4.3/warg/os_utilities/os_platform.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6097 2024-05-27 10:59:27.000000 warg-1.4.3/warg/os_utilities/path_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2598 2024-05-27 10:59:27.000000 warg-1.4.3/warg/os_utilities/path_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2815 2024-05-27 10:59:27.000000 warg-1.4.3/warg/os_utilities/platform_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:59:33.229152 warg-1.4.3/warg/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 10:59:27.000000 warg-1.4.3/warg/packages/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      418 2024-05-27 10:59:27.000000 warg-1.4.3/warg/packages/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4975 2024-05-27 10:59:27.000000 warg-1.4.3/warg/packages/editable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-27 10:59:27.000000 warg-1.4.3/warg/packages/namespaces.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2276 2024-05-27 10:59:27.000000 warg-1.4.3/warg/packages/pip_parsing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10370 2024-05-27 10:59:27.000000 warg-1.4.3/warg/packages/reloading.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6303 2024-05-27 10:59:27.000000 warg-1.4.3/warg/packages/satisfaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4135 2024-05-27 10:59:27.000000 warg-1.4.3/warg/packages/versioning.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1743 2024-05-27 10:59:27.000000 warg-1.4.3/warg/plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-05-27 10:59:27.000000 warg-1.4.3/warg/replication.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1257 2024-05-27 10:59:27.000000 warg-1.4.3/warg/strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1138 2024-05-27 10:59:27.000000 warg-1.4.3/warg/text.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2012 2024-05-27 10:59:27.000000 warg-1.4.3/warg/typing_extension.py
```

### Comparing `Warg-1.4.2/.github/CODE_OF_CONDUCT.md` & `warg-1.4.3/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/LICENSE.md` & `warg-1.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/PKG-INFO` & `warg-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Warg
-Version: 1.4.2
+Version: 1.4.3
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/warg
 Download-URL: https://github.com/pything/warg/releases
 Author: Christian Heider Lindbjerg
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Lindbjerg
 Maintainer-email: christian.heider@alexandra.dk
@@ -22,51 +22,51 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: setup
 Requires-Dist: pytest-runner; extra == "setup"
-Provides-Extra: dev
-Requires-Dist: black>=18.9b0; extra == "dev"
-Requires-Dist: sphinx; extra == "dev"
-Requires-Dist: pip>=19.0.3; extra == "dev"
-Requires-Dist: pytest-cov>=2.6.1; extra == "dev"
-Requires-Dist: twine>=1.13.0; extra == "dev"
-Requires-Dist: tox; extra == "dev"
-Requires-Dist: pytest-runner; extra == "dev"
-Requires-Dist: apppath; extra == "dev"
-Requires-Dist: coveralls>=1.6.0; extra == "dev"
-Requires-Dist: wheel>=0.38.0; extra == "dev"
-Requires-Dist: pytest>=4.3.0; extra == "dev"
-Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
-Requires-Dist: warg; extra == "dev"
 Provides-Extra: tests
 Requires-Dist: pytest>=4.3.0; extra == "tests"
-Requires-Dist: tox; extra == "tests"
 Requires-Dist: pytest-cov>=2.6.1; extra == "tests"
+Requires-Dist: tox; extra == "tests"
 Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: apppath; extra == "docs"
 Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
+Requires-Dist: apppath; extra == "docs"
 Requires-Dist: warg; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Provides-Extra: dev
+Requires-Dist: pytest>=4.3.0; extra == "dev"
+Requires-Dist: pytest-runner; extra == "dev"
+Requires-Dist: twine>=1.13.0; extra == "dev"
+Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
+Requires-Dist: black>=18.9b0; extra == "dev"
+Requires-Dist: coveralls>=1.6.0; extra == "dev"
+Requires-Dist: pytest-cov>=2.6.1; extra == "dev"
+Requires-Dist: apppath; extra == "dev"
+Requires-Dist: wheel>=0.38.0; extra == "dev"
+Requires-Dist: warg; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: pip>=19.0.3; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 Provides-Extra: all
-Requires-Dist: sphinx; extra == "all"
-Requires-Dist: pip>=19.0.3; extra == "all"
-Requires-Dist: pytest-cov>=2.6.1; extra == "all"
-Requires-Dist: sphinxcontrib-programoutput; extra == "all"
-Requires-Dist: twine>=1.13.0; extra == "all"
-Requires-Dist: tox; extra == "all"
+Requires-Dist: pytest>=4.3.0; extra == "all"
 Requires-Dist: pytest-runner; extra == "all"
-Requires-Dist: apppath; extra == "all"
+Requires-Dist: twine>=1.13.0; extra == "all"
+Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: black>=18.9b0; extra == "all"
 Requires-Dist: coveralls>=1.6.0; extra == "all"
+Requires-Dist: pytest-cov>=2.6.1; extra == "all"
+Requires-Dist: apppath; extra == "all"
 Requires-Dist: wheel>=0.38.0; extra == "all"
-Requires-Dist: pytest>=4.3.0; extra == "all"
-Requires-Dist: black>=18.9b0; extra == "all"
 Requires-Dist: warg; extra == "all"
+Requires-Dist: sphinx; extra == "all"
+Requires-Dist: pip>=19.0.3; extra == "all"
+Requires-Dist: tox; extra == "all"
 
 <!--![warg](.github/images/warg.svg)-->
 
 <p align="center">
   <img src=".github/images/warg.svg" alt='Warg' />
 </p>
```

### Comparing `Warg-1.4.2/README.md` & `warg-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/SECURITY.md` & `warg-1.4.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/Warg.egg-info/PKG-INFO` & `warg-1.4.3/Warg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Warg
-Version: 1.4.2
+Version: 1.4.3
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/warg
 Download-URL: https://github.com/pything/warg/releases
 Author: Christian Heider Lindbjerg
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Lindbjerg
 Maintainer-email: christian.heider@alexandra.dk
@@ -22,51 +22,51 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: setup
 Requires-Dist: pytest-runner; extra == "setup"
-Provides-Extra: dev
-Requires-Dist: black>=18.9b0; extra == "dev"
-Requires-Dist: sphinx; extra == "dev"
-Requires-Dist: pip>=19.0.3; extra == "dev"
-Requires-Dist: pytest-cov>=2.6.1; extra == "dev"
-Requires-Dist: twine>=1.13.0; extra == "dev"
-Requires-Dist: tox; extra == "dev"
-Requires-Dist: pytest-runner; extra == "dev"
-Requires-Dist: apppath; extra == "dev"
-Requires-Dist: coveralls>=1.6.0; extra == "dev"
-Requires-Dist: wheel>=0.38.0; extra == "dev"
-Requires-Dist: pytest>=4.3.0; extra == "dev"
-Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
-Requires-Dist: warg; extra == "dev"
 Provides-Extra: tests
 Requires-Dist: pytest>=4.3.0; extra == "tests"
-Requires-Dist: tox; extra == "tests"
 Requires-Dist: pytest-cov>=2.6.1; extra == "tests"
+Requires-Dist: tox; extra == "tests"
 Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: apppath; extra == "docs"
 Requires-Dist: sphinxcontrib-programoutput; extra == "docs"
+Requires-Dist: apppath; extra == "docs"
 Requires-Dist: warg; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Provides-Extra: dev
+Requires-Dist: pytest>=4.3.0; extra == "dev"
+Requires-Dist: pytest-runner; extra == "dev"
+Requires-Dist: twine>=1.13.0; extra == "dev"
+Requires-Dist: sphinxcontrib-programoutput; extra == "dev"
+Requires-Dist: black>=18.9b0; extra == "dev"
+Requires-Dist: coveralls>=1.6.0; extra == "dev"
+Requires-Dist: pytest-cov>=2.6.1; extra == "dev"
+Requires-Dist: apppath; extra == "dev"
+Requires-Dist: wheel>=0.38.0; extra == "dev"
+Requires-Dist: warg; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: pip>=19.0.3; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 Provides-Extra: all
-Requires-Dist: sphinx; extra == "all"
-Requires-Dist: pip>=19.0.3; extra == "all"
-Requires-Dist: pytest-cov>=2.6.1; extra == "all"
-Requires-Dist: sphinxcontrib-programoutput; extra == "all"
-Requires-Dist: twine>=1.13.0; extra == "all"
-Requires-Dist: tox; extra == "all"
+Requires-Dist: pytest>=4.3.0; extra == "all"
 Requires-Dist: pytest-runner; extra == "all"
-Requires-Dist: apppath; extra == "all"
+Requires-Dist: twine>=1.13.0; extra == "all"
+Requires-Dist: sphinxcontrib-programoutput; extra == "all"
+Requires-Dist: black>=18.9b0; extra == "all"
 Requires-Dist: coveralls>=1.6.0; extra == "all"
+Requires-Dist: pytest-cov>=2.6.1; extra == "all"
+Requires-Dist: apppath; extra == "all"
 Requires-Dist: wheel>=0.38.0; extra == "all"
-Requires-Dist: pytest>=4.3.0; extra == "all"
-Requires-Dist: black>=18.9b0; extra == "all"
 Requires-Dist: warg; extra == "all"
+Requires-Dist: sphinx; extra == "all"
+Requires-Dist: pip>=19.0.3; extra == "all"
+Requires-Dist: tox; extra == "all"
 
 <!--![warg](.github/images/warg.svg)-->
 
 <p align="center">
   <img src=".github/images/warg.svg" alt='Warg' />
 </p>
```

### Comparing `Warg-1.4.2/Warg.egg-info/SOURCES.txt` & `warg-1.4.3/Warg.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 warg/contexts.py
 warg/datetimes.py
 warg/debug.py
 warg/exceptions.py
 warg/functions.py
 warg/gdkc.py
 warg/iteration.py
+warg/logging_utilities.py
 warg/manipulation.py
 warg/map_itertools.py
 warg/ode.py
 warg/plugin.py
 warg/replication.py
 warg/strings.py
 warg/text.py
```

### Comparing `Warg-1.4.2/pyproject.toml` & `warg-1.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/setup.py` & `warg-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-from typing import List, Sequence, Union, TextIO
+from typing import List, Sequence, TextIO, Union
 
 
 def python_version_check(major: int = 3, minor: int = 7):
     """description"""
     import sys
 
     assert sys.version_info.major == major and sys.version_info.minor >= minor, (
```

### Comparing `Warg-1.4.2/tests/test_ast_ops.py` & `warg-1.4.3/tests/test_ast_ops.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/tests/test_auto_dict.py` & `warg-1.4.3/tests/test_auto_dict.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 
 __author__ = "Christian Heider Lindbjerg"
 __doc__ = r"""
 
            Created on 21/12/2019
            """
 
-from warg.data_structures.auto_dict import (
-    AutoDict,
-    sanitise_auto_dict,
-    recursive_default_dict_print,
-)
+from warg.data_structures.auto_dict import AutoDict, recursive_default_dict_print, sanitise_auto_dict
 
 
 def test_a():
     ad = AutoDict()
 
     ad["b"]["b"]["c"]["b"]["c"] = {}
     ad["c"] = 1
```

### Comparing `Warg-1.4.2/tests/test_collective.py` & `warg-1.4.3/tests/test_collective.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __author__ = "Christian Heider Lindbjerg"
 __doc__ = r"""
 
            Created on 09/03/2020
            """
 
-from warg import kws_sink, prod, sink, evaluate_context
+from warg import evaluate_context, kws_sink, prod, sink
 
 
 def test_a():
     print(evaluate_context(kws_sink, "str"))
     print(evaluate_context(kws_sink, 2))
     print(evaluate_context(kws_sink, 2.2))
```

### Comparing `Warg-1.4.2/tests/test_gdkc.py` & `warg-1.4.3/tests/test_gdkc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-from typing import Sequence, MutableMapping, Any
+from typing import Any, MutableMapping, Sequence
 
 import pytest
 
 from warg.gdkc import GeneralisedDelayedKwargConstruction
 
 __author__ = "Christian Heider Lindbjerg"
 __doc__ = r"""
```

### Comparing `Warg-1.4.2/tests/test_imports.py` & `warg-1.4.3/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/tests/test_iteration.py` & `warg-1.4.3/tests/test_iteration.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/tests/test_kw_passing.py` & `warg-1.4.3/tests/test_kw_passing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 import inspect
-from typing import Sequence, MutableMapping, Any
+from typing import Any, MutableMapping, Sequence
 
 from warg.decorators.kw_passing import (
     drop_unused_kws,
     passes_kws_to,
     super_init_pass_on_kws,
 )
```

### Comparing `Warg-1.4.2/tests/test_nod.py` & `warg-1.4.3/tests/test_nod.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/tests/test_post_init.py` & `warg-1.4.3/tests/test_post_init.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-from typing import Sequence, MutableMapping, Any
+from typing import Any, MutableMapping, Sequence
 
 from warg import drop_unused_kws
 from warg.metas.post_init import PostInit
 
 __author__ = "Christian Heider Lindbjerg"
 __doc__ = r"""
            """
```

### Comparing `Warg-1.4.2/tests/test_singleton.py` & `warg-1.4.3/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/__init__.py` & `warg-1.4.3/warg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     from importlib_metadata import PackageNotFoundError
     from importlib_resources import files
 
 
 __project__ = "Warg"
 
 __author__ = "Christian Heider Lindbjerg"
-__version__ = "1.4.2"
+__version__ = "1.4.3"
 __doc__ = r"""
 Created on 27/04/2019
 
 @author: cnheider
 
 """
 
@@ -57,14 +57,15 @@
     from .replication import *
     from .strings import *
     from .contexts import *
     from .config_shell import *
     from .colors import *
     from .packages import *
     from .iteration import *
+    from .logging_utilities import *
 except ImportError as ix:
     this_package_name = Path(__file__).parent.name
     this_package_reqs = Path(__file__).parent.parent / f"requirements.txt"
     if this_package_reqs.exists():
         print(
             f"Make sure requirements is installed for {this_package_name}, see {this_package_reqs}"
         )  # TODO: PARSE WHAT is missing and print
```

### Comparing `Warg-1.4.2/warg/arguments.py` & `warg-1.4.3/warg/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 __all__ = [
     "to_lower_properties",
     "get_upper_case_vars_or_protected_of",
     "config_to_mapping",
     "add_bool_arg",
     "check_for_duplicates_in_args",
     "UpperAttrMetaclass",
+    "str_to_bool",
 ]
 
 
 class UpperAttrMetaclass(type):
     """
     Upper case all attributes if not __private"""
```

### Comparing `Warg-1.4.2/warg/ast_ops/arg_indentifier.py` & `warg-1.4.3/warg/ast_ops/arg_indentifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
            Created on 26-01-2021
            """
 
 __all__ = ["ArgIdentifier", "get_arg_names", "cprinta", "cprintz"]
 
 import ast
-from typing import Optional, Any, Callable
+from typing import Any, Callable, Optional
 
 
 class ArgIdentifier(ast.NodeVisitor):
     """description"""
 
     def __init__(
         self,
```

### Comparing `Warg-1.4.2/warg/ast_ops/first_arg_identifier.py` & `warg-1.4.3/warg/ast_ops/first_arg_identifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
            Created on 26-01-2021
            """
 
 __all__ = ["FirstArgIdentifier", "get_first_arg_name", "cprint"]
 
 import ast
-from typing import Optional, Any, Callable
+from typing import Any, Callable, Optional
 
 
 def recurse_first_args(args):
     """
 
     :param args:
     :type args:
```

### Comparing `Warg-1.4.2/warg/bases/property_settings.py` & `warg-1.4.3/warg/bases/property_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 __doc__ = r"""
 
            Created on 17/03/2020
            """
 __all__ = ["PropertySettings"]
 
 from collections.abc import Mapping
-from typing import Dict, MutableMapping, Any
+from typing import Any, Dict, MutableMapping
 
 from warg import NOD
 
 
 class PropertySettings(
     # Mapping
 ):
```

### Comparing `Warg-1.4.2/warg/boolean_tests.py` & `warg-1.4.3/warg/boolean_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "is_none_or_zero_or_negative_or_mod_zero",
     "xor",
     "xnor",
     "nand",
 ]
 
 import math
-from typing import Any, Optional, Callable
+from typing import Any, Callable, Optional
 
 from warg import Number
 from warg.decorators import drop_unused_kws, passes_kws_to
 
 
 @drop_unused_kws
 def is_positive_and_mod_zero(
```

### Comparing `Warg-1.4.2/warg/business.py` & `warg-1.4.3/warg/business.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 __author__ = "Christian Heider Lindbjerg"
 __doc__ = r"""
 
            Created on 17/03/2020
            """
 
 from itertools import cycle
-from typing import Iterable, Callable
+from typing import Callable, Iterable
 
 
 def busy_indicator(
     *,
     stream: Callable = print,
     indicator_interval: int = 1,
     phases: Iterable[str] = ("◑", "◒", "◐", "◓"),
```

### Comparing `Warg-1.4.2/warg/colors/color_conversion.py` & `warg-1.4.3/warg/colors/color_conversion.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/colors/css_colors.py` & `warg-1.4.3/warg/colors/css_colors.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/colors/label_colors.py` & `warg-1.4.3/warg/colors/label_colors.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/config_shell.py` & `warg-1.4.3/warg/config_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
            Created on 17/03/2020
            """
 __all__ = ["PlaybackShell", "ConfigShell"]
 
 import cmd
 from pathlib import Path
-from typing import MutableMapping, Optional, Callable
+from typing import Callable, MutableMapping, Optional
 
-from warg import passes_kws_to, PropertySettings
+from warg import PropertySettings, passes_kws_to
 
 
 class PlaybackShell(cmd.Cmd):
     """description"""
 
     intro = "Type help or ? to list commands.\n"
     default_file_path = Path("playback.cmd")
```

### Comparing `Warg-1.4.2/warg/context_wrapper.py` & `warg-1.4.3/warg/context_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
            Created on 01/07/2020
            """
 
 __all__ = ["ContextWrapper", "NopContext"]
 
 import contextlib
 import inspect
-from typing import Callable, Sequence, Mapping, Optional, ContextManager
+from typing import Callable, ContextManager, Mapping, Optional, Sequence
 
 
 class NopContext(contextlib.AbstractContextManager):
     def __enter__(self):
         return
 
     def __exit__(self, exc_type, exc_val, exc_tb):
```

### Comparing `Warg-1.4.2/warg/contexts.py` & `warg-1.4.3/warg/contexts.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/data_structures/auto_dict.py` & `warg-1.4.3/warg/data_structures/auto_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 __author__ = "Christian Heider Lindbjerg"
 __doc__ = r"""
 
            Created on 21/12/2019
            """
 
 from collections import defaultdict
-from typing import Dict, Optional, Mapping
+from typing import Dict, Mapping, Optional
 
 __all__ = [
     "AutoDict",
     "sanitise_auto_dict",
     "recursive_default_dict_print",
     "recursive_default_dict",
 ]
```

### Comparing `Warg-1.4.2/warg/data_structures/mappings.py` & `warg-1.4.3/warg/data_structures/mappings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-from typing import Mapping, Iterable, Hashable, Dict, Callable, MutableMapping
+from typing import Callable, Dict, Hashable, Iterable, Mapping, MutableMapping
 
 __all__ = [
     "invert_mapping",
     "invert_dict",
     "AppendingDict",
     "pivot_dict_object",
     "pivot_dict",
@@ -102,14 +102,34 @@
     :param key:
     :return:
     :rtype:
     """
     return {getattr(v, key): k for k, v in d.items()}
 
 
+def to_dict(m: Mapping) -> dict:
+    o = {}
+    for k, v in m.items():
+        if isinstance(v, Mapping):
+            o[k] = to_dict(v)
+        else:
+            o[k] = v
+    return o
+
+
 if __name__ == "__main__":
     print(invert_mapping({"a": 1, "b": 2}))
 
     print(invert_mapping({"a": 2, "b": 2, "c": 3, "d": 4}))
     print(invert_dict({"a": 2, "b": 2, "c": 3, "d": 4}))
 
+    def uhasdu():
+        from warg.data_structures.named_ordered_dictionary import NOD
+
+        a = NOD({"b": NOD(c=1)})
+
+        print(a)
+        print(a.as_dict())
+
+    uhasdu()
+
     # print(pivot_dict_object({"a": 2, "b": 2, "c": 3, "d": 4}, "id"))
```

### Comparing `Warg-1.4.2/warg/data_structures/named_ordered_dictionary.py` & `warg-1.4.3/warg/data_structures/named_ordered_dictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 
 from typing import (
     Any,
     ItemsView,
     Iterable,
     KeysView,
     List,
+    Mapping,
     MutableMapping,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     ValuesView,
-    Mapping,
 )
+from copy import deepcopy
 
 __author__ = "Christian Heider Lindbjerg"
 
 __all__ = ["NamedOrderedDictionary", "NOD"]
 
+from warg.data_structures.mappings import to_dict
+
 LOCALS = (
     "as_list",
     "as_dict",
     "as_tuples",
     "as_flat_tuples",
     "add_unnamed_arg",
     "dict_of",
@@ -153,15 +156,20 @@
         return list(self.__dict__.values())
 
     def as_dict(self) -> dict:
         """
 
         :return:
         :rtype:"""
-        return self.__dict__
+
+        # dict_ = deepcopy(self.__dict__)
+
+        dict_ = to_dict(self.__dict__)
+
+        return dict_
 
     def as_tuples(self) -> List[Tuple[Any, Any]]:
         """
 
         :return:
         :rtype:"""
         return [(k, v) for (k, v) in self.__dict__.items()]
```

### Comparing `Warg-1.4.2/warg/data_structures/ordered_set.py` & `warg-1.4.3/warg/data_structures/ordered_set.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/data_structures/sequences.py` & `warg-1.4.3/warg/data_structures/sequences.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/datetimes.py` & `warg-1.4.3/warg/datetimes.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/debug.py` & `warg-1.4.3/warg/debug.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 __doc__ = r"""
 
            Created on 09/03/2020
            """
 
 __all__ = ["evaluate_context"]
 
-from typing import Any, Callable, MutableMapping, Tuple, List, Dict
+from typing import Any, Callable, Dict, List, MutableMapping, Tuple
 
 
 def evaluate_context(
     x: Any, *args: Any, **kwargs: MutableMapping[str, Any]
 ) -> Tuple[List, Dict, object, type]:
     """
```

### Comparing `Warg-1.4.2/warg/decorators/caching/look_up_table.py` & `warg-1.4.3/warg/decorators/caching/look_up_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,15 @@
 __doc__ = r"""
           Automatically generates a look up data
 
            Created on 06/03/2020
            """
 
 from time import sleep, time
-from typing import (
-    Iterable,
-    Mapping,
-    Set,
-    Tuple,
-    Sequence,
-    MutableMapping,
-    Any,
-    Callable,
-)
+from typing import Any, Callable, Iterable, Mapping, MutableMapping, Sequence, Set, Tuple
 
 from warg.decorators.hashing import make_hash
 
 global_table = {}
 
 __all__ = ["add_lut", "look_up", "look_up_args", "look_up_kws"]
```

### Comparing `Warg-1.4.2/warg/decorators/caching/property_caching.py` & `warg-1.4.3/warg/decorators/caching/property_caching.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/decorators/exporting.py` & `warg-1.4.3/warg/decorators/exporting.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/decorators/hashing.py` & `warg-1.4.3/warg/decorators/hashing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/decorators/kw_passing.py` & `warg-1.4.3/warg/decorators/kw_passing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 #!/usr/bin/env python3
 import functools
 import inspect
+import logging
 import types
 from functools import wraps
-from logging import warning
-from typing import (
-    Dict,
-    MutableMapping,
-    Sequence,
-    Tuple,
-    Any,
-    Callable,
-    Optional,
-    Iterable,
-)
+from typing import Any, Callable, Dict, Iterable, MutableMapping, Optional, Sequence, Tuple
 
 __author__ = "Christian Heider Lindbjerg"
 __doc__ = r"""
           The concept "kw passing" implemented here lets one make a contract with the caller that all
           kwargs with be passed onwards to a receiver, this lets the caller inspect available kwargs of the
           the receiver function allowing for autocompletion, typing and documentation fetching.
            """
@@ -33,14 +24,17 @@
     "pack_args",
     "pack_kws",
     "pack_args_and_kws",
     "AlsoDecorator",
 ]
 
 
+logger = logging.getLogger(__name__)
+
+
 # noinspection PyUnresolvedReferences
 def to_keyword_only(val: inspect.Parameter) -> inspect.Parameter:
     """
 
     :param val:
     :type val:
     :return:
@@ -97,15 +91,15 @@
         passing_params[var_kw_key] = var_kw
 
         no_var_kw = True
         for k, v in receiver_params.items():
             if v.kind == inspect._ParameterKind.VAR_KEYWORD:
                 no_var_kw = False
         if no_var_kw:
-            warning(
+            logger.warning(
                 f"Receiver {receiver_func} with {receiver_params} does not acceptable arbitrary kwargs although "
                 f"from_func will pass "
                 f"all "
                 f"kwargs onwards TypeErrors might occur, to fix this let this receiver accept any arbitrary "
                 f"kwargs by adding ..,**kwargs): to the receivers function declaration"
             )
 
@@ -134,15 +128,15 @@
         for rf in receiver_funcs:
             passing_sig, new_params = eval_sig_kw_params(passing_sig, rf, keep_from_var_kw)
             if no_pass_filter:  # DOES NOT ENFORCE NO PASS OF ARGUMENTS
                 for k in no_pass_filter:
                     if k in new_params:
                         new_params.pop(k)
                     else:
-                        warning(f"{k} is not in signature of {rf}")
+                        logger.warning(f"{k} is not in signature of {rf}")
             passing_sig = passing_sig.replace(parameters=list(new_params.values()))
         passing_func.__signature__ = passing_sig
         return passing_func
 
     return _func
 
 
@@ -454,15 +448,15 @@
                 return f(*args, **kwargs)
 
         kept = {}
         for k, v in kwargs.items():
             if k in from_sig.parameters.keys():
                 kept[k] = v
             else:
-                warning(f"dropped {k} with value {v} from call of {f}")
+                logger.warning(f"dropped {k} with value {v} from call of {f}")
 
         return f(*args, **kept)
 
     return wrapper
 
 
 class AlsoDecorator:
```

### Comparing `Warg-1.4.2/warg/decorators/timing.py` & `warg-1.4.3/warg/decorators/timing.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 __all__ = ["timeit", "StopWatch"]
 
 import contextlib
 import functools
 import time
 import typing
 from functools import wraps
-from typing import Sequence, MutableMapping, Any
+from typing import Any, MutableMapping, Sequence
 
 
 def timeit(f: typing.Callable) -> typing.Callable:
     """
 
     :param f:
     :type f:
```

### Comparing `Warg-1.4.2/warg/decorators/wrapping.py` & `warg-1.4.3/warg/decorators/wrapping.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/exceptions.py` & `warg-1.4.3/warg/exceptions.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/functions.py` & `warg-1.4.3/warg/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,33 +31,25 @@
     "most_common_substrings",
     "mappings_agreement_reduce",
 ]
 
 import ctypes
 import operator
 import sys
+import webbrowser
 from collections import defaultdict
 from copy import deepcopy
-from functools import reduce
-from pathlib import Path
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Iterable,
-    Iterator,
-    Mapping,
-    Sequence,
-    Tuple,
-    List,
-    Union,
-    Optional,
-)
 from difflib import SequenceMatcher
+from functools import reduce
 from itertools import product
+from pathlib import Path
+from typing import Any, Callable, Dict, Iterable, Iterator, List, Mapping, Optional, Sequence, Tuple, Union
+
+import requests
+
 from warg.contexts import Suppress
 from warg.decorators import drop_unused_kws
 from warg.typing_extension import Number
 
 
 def int_limits(c_int_type: Any) -> Tuple[int, int]:
     signed = c_int_type(-1).value < c_int_type(0).value
@@ -408,14 +400,50 @@
     for k, v in m2.items():
         if k not in out:
             out[k] = v
 
     return out
 
 
+def open_uri_resource(uri: str) -> str:
+    """Opens the default web browser.
+    Qt offers PyQt5.QtWebEngineWidgets (QWebEngineView, QWebEngineSettings) but they are not
+    available from pyQGIS
+
+    """
+
+    path = Path(uri)
+
+    if path.exists() and path.is_file():
+        uri = f"file:///{path.absolute()}"
+        msg = uri
+        webbrowser.open_new_tab(uri)
+    else:
+        try:
+            uri = f'https://{uri.lstrip("https://")}'
+            r = requests.head(uri)
+            if r.ok:  # it is a boolean
+                try:
+                    webbrowser.open_new_tab(uri)
+                    msg = uri
+                except webbrowser.Error as e:
+                    msg = f"Webbrowser error: {e}"
+
+            elif r.status_code == 404:
+                msg = f'HTTP Error 404: Page not found.<br>The following URL may be broken or dead:<br><br><a href="{uri}">{uri}</a>'
+
+            else:
+                msg = f'Error with URL<br><br><a href="{uri}">{uri}</a>'
+
+        except requests.ConnectionError as e:
+            msg = f'URL <a href="{uri}">{uri}</a> could not be opened.<br><br>Is your internet connection up and working?'
+
+    return msg
+
+
 if __name__ == "__main__":
 
     def asud() -> None:
         """
         :rtype: None
         """
         a = {"b": 1, "h": 2}
@@ -446,12 +474,15 @@
         ij = ([10, 29], [(2, 3, 4), [[12, 4, 5]], ((2, 92, 90))], [])
         print(to_list(ij))
 
     def i8jsadi2j():
         ij = ([10, 29], [(2, 3, 4), [[12, 4, 5]], ((2, 92, 90))], [])
         print(to_tuple(ij))
 
-    i8jsadij()
-    i8jsadi2j()
+    # i8jsadij()
+    # i8jsadi2j()
     # asud()
     # asidj()
     # asjdnasid()
+
+    # print(open_uri_resource(__file__))
+    print(open_uri_resource("dr.dk"))
```

### Comparing `Warg-1.4.2/warg/gdkc.py` & `warg-1.4.3/warg/gdkc.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 __doc__ = """
 Generalised wrapper for delayed construction of class objects. Encapsulates kwargs and callable constructor with the option of modifying construction arguments before construction is finally performed.
 
 """
 
 __all__ = ["GeneralisedDelayedKwargConstruction", "GDKC"]
 
+
 import logging
-from typing import Any, Mapping, MutableMapping, Sequence, Callable
+from typing import Any, Callable, Mapping, MutableMapping, Sequence
+
+logger = logging.getLogger(__name__)
 
 
 class GeneralisedDelayedKwargConstruction:
     """
     A generalised class for setting up kwargs for later construction of an instance of an object
     [constructor, args, kwargs]
     """
@@ -64,15 +67,15 @@
             [
                 f"Overwriting {k} with the value {v} in construction of {self.constructor}"
                 for (k, v), b in zip(kwargs.items(), self.kwargs.keys())
                 if k == b
             ]
         )
         if war != "":
-            logging.warning(war)
+            logger.warning(war)
 
         self.kwargs.update(kwargs)
         try:
             return self.constructor(*args, **self.kwargs)
         except TypeError as e:
             e.args += (f"in construction of {self.constructor}",)
             raise e
```

### Comparing `Warg-1.4.2/warg/generators/cyclic_generators.py` & `warg-1.4.3/warg/generators/cyclic_generators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 import itertools
-from math import sin, cos
+from math import cos, sin
 from typing import Iterable
 
 from warg import Number
 
 __all__ = ["sin_gen", "cos_gen", "loop"]
 
 loop = itertools.cycle
```

### Comparing `Warg-1.4.2/warg/generators/escaping.py` & `warg-1.4.3/warg/generators/escaping.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/generators/filtering.py` & `warg-1.4.3/warg/generators/filtering.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 __author__ = "Christian Heider Lindbjerg"
 __doc__ = r"""
 
            Created on 18-01-2021
            """
 
 from enum import Enum
-from typing import Iterable, Any
+from typing import Any, Iterable
 
 __all__ = ["FilterModeEnum", "symbol_filter"]
 
 
 # from sorcery import assigned_names # PURE!
```

### Comparing `Warg-1.4.2/warg/generators/mapping_generator.py` & `warg-1.4.3/warg/generators/mapping_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-from typing import Any, Iterable, Mapping, Tuple, Callable
+from typing import Any, Callable, Iterable, Mapping, Tuple
 
 __author__ = "Christian Heider Lindbjerg"
 __doc__ = r"""
 
            Created on 11/11/2019
            """
```

### Comparing `Warg-1.4.2/warg/generators/numbers.py` & `warg-1.4.3/warg/generators/numbers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 import random
-from typing import Iterable, Tuple, Callable, List
+from typing import Callable, Iterable, List, Tuple
 
 from warg import Number
 
 __all__ = ["n_uint_mix", "n_uint_mix_generator_builder", "n_uint_mix_generator"]
 
 
 def n_uint_mix(mix: Iterable[Number]) -> List[Number]:
```

### Comparing `Warg-1.4.2/warg/generators/zipping_generator.py` & `warg-1.4.3/warg/generators/zipping_generator.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/iteration.py` & `warg-1.4.3/warg/iteration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-from typing import Callable, Iterable, List, Sequence, Any, Tuple
+from typing import Any, Callable, Iterable, List, Sequence, Tuple
 
 __all__ = ["pairs", "chunks", "leaf_apply", "leaf_type_apply"]
 
 
 def pairs(s: Sequence) -> Tuple[Any, Any]:
     """
     Iterate over a list in overlapping pairs.
```

### Comparing `Warg-1.4.2/warg/manipulation.py` & `warg-1.4.3/warg/manipulation.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 __doc__ = r"""
 
            Created on 23/07/2020
            """
 
 __all__ = ["recursive_flatten"]
 
-from typing import Sequence, Iterable
+from typing import Iterable, Sequence
 
 
 def recursive_flatten_seq(seq: Sequence) -> Sequence:
     """Depth first flatten"""
     if not seq:  # is empty Sequence
         return seq
     if isinstance(seq[0], Sequence):
```

### Comparing `Warg-1.4.2/warg/map_itertools.py` & `warg-1.4.3/warg/map_itertools.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "map_product",
     "map_permutations",
     "map_combinations",
     "map_combinations_with_replacement",
 ]
 
 import itertools
-from typing import Any, Callable, Iterable, List, Mapping, Sequence, Tuple
+from typing import Any, Mapping, Tuple
 
 
 def map_value_product(dicts: Mapping) -> Any:
     """description"""
     return (dict(zip(dicts, x)) for x in itertools.product(*dicts.values()))
```

### Comparing `Warg-1.4.2/warg/math_utilities/ordinals.py` & `warg-1.4.3/warg/math_utilities/ordinals.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/math_utilities/powers.py` & `warg-1.4.3/warg/math_utilities/powers.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/metas/post_init.py` & `warg-1.4.3/warg/metas/post_init.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 __doc__ = r"""
 
            Created on 11/12/2019
            """
 
 __all__ = ["PostInit"]
 
-from typing import Sequence, MutableMapping, Any
+from typing import Any, MutableMapping, Sequence
 
 
 class PostInit(type):
     """
     define a new metaclass which overrides the "__call__" function"""
 
     def __call__(cls, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]) -> object:
```

### Comparing `Warg-1.4.2/warg/metas/singleton.py` & `warg-1.4.3/warg/metas/singleton.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 @author: cnheider
 """
 
 __all__ = ["SingletonBase", "SingletonMeta", "key_singleton", "singleton"]
 
 import functools
 from functools import wraps
-from typing import Any, Sequence, MutableMapping, Callable
+from typing import Any, Callable, MutableMapping, Sequence
 
 
 class SingletonBase:
     """
     A base class for creating singleton class where all subtypes(Derivations) should also return the first
     and only
     instantiation of a particular singleton base type, if this property is not wanted consider using the
```

### Comparing `Warg-1.4.2/warg/mixins/dict_mixins.py` & `warg-1.4.3/warg/mixins/dict_mixins.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/mixins/ordinal_index_mixin.py` & `warg-1.4.3/warg/mixins/ordinal_index_mixin.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 __author__ = "Christian Heider Lindbjerg"
 __doc__ = ""
 
 __all__ = [
     "OrdinalIndexingDictMixin",
 ]
 
-from typing import Union, Any
+from typing import Any, Union
 
 
 class OrdinalIndexingDictMixin:
     """
     Mixin class for indexing a class instance __dict__ (SortedDict) with both integer (ordinal) indexing or
     key:str attributes (non-ordinal) access."""
```

### Comparing `Warg-1.4.2/warg/ode.py` & `warg-1.4.3/warg/ode.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/os_utilities/filtering.py` & `warg-1.4.3/warg/os_utilities/filtering.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
            """
 
 __all__ = ["is_excluded", "is_python_package", "is_python_module", "negate"]
 
 import re
 from functools import wraps
 from pathlib import Path
-from typing import Callable, Sequence, MutableMapping, Union, Any
+from typing import Any, Callable, MutableMapping, Sequence, Union
 
 
 def is_python_module(path: Path) -> bool:
     """
     Check if path is a python module
     """
     path = Path(path)
```

### Comparing `Warg-1.4.2/warg/os_utilities/os_platform.py` & `warg-1.4.3/warg/os_utilities/os_platform.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/os_utilities/path_functions.py` & `warg-1.4.3/warg/os_utilities/path_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     "keep_last_n_modified",
 ]
 
 import collections
 import os
 from itertools import cycle
 from pathlib import Path
-
-from typing import Iterable, Union, Callable
+from typing import Callable, Iterable, Union
 
 
 def path_join(*p: Union[Path, str]) -> Path:
     """
     Drop-in replacement for os.path.join, returning a Path instead
 
     :param p: Sequence of path components to be joined
```

### Comparing `Warg-1.4.2/warg/os_utilities/path_utilities.py` & `warg-1.4.3/warg/os_utilities/path_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
            """
 
 import os
 import subprocess
 from pathlib import Path
 from typing import Optional
 
-from warg.os_utilities.os_platform import is_windows, is_mac, has_x_server
+from warg.os_utilities.os_platform import has_x_server, is_mac, is_windows
 
 __all__ = ["latest_file", "exist_any_extension", "system_open_path"]
 
 
 def system_open_path(path: Path, *, verbose: bool = False) -> None:
     """
     Use system defaults for opening path/uris
```

### Comparing `Warg-1.4.2/warg/os_utilities/platform_selection.py` & `warg-1.4.3/warg/os_utilities/platform_selection.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/packages/editable.py` & `warg-1.4.3/warg/packages/editable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python3
 import json
-import logging
 
 try:
     from importlib.metadata import Distribution, PackageNotFoundError, PathDistribution
 except (ModuleNotFoundError, ImportError) as e:
     from importlib_metadata import Distribution, PackageNotFoundError, PathDistribution
 
 __all__ = [
@@ -12,15 +11,17 @@
     "package_is_editable",
     "get_dist_package_location",
     "get_package_location",
 ]
 
 from pathlib import Path
 from typing import Optional
+import logging
 
+logger = logging.getLogger(__name__)
 VERBOSE = False
 
 
 # noinspection PyProtectedMember
 def dist_is_editable(dist: Distribution) -> bool:
     """
     Return True if given Distribution is an editable installation.
@@ -81,26 +82,26 @@
     try:
         dist = Distribution.from_name(package_name)
 
         return dist_is_editable(dist)
 
     except PackageNotFoundError as p:
         if VERBOSE:
-            logging.info(p)
+            logger.info(p)
 
 
 def get_package_location(package_name: str) -> Path:
     try:
         dist = Distribution.from_name(package_name)
         if dist:
             return get_dist_package_location(dist)
 
     except PackageNotFoundError as p:
         if VERBOSE:
-            logging.info(p)
+            logger.info(p)
 
 
 # noinspection PyProtectedMember
 def get_dist_package_location(dist: Distribution) -> Optional[Path]:
     """
     FULL OF ASSUMPTIONS!
```

### Comparing `Warg-1.4.2/warg/packages/namespaces.py` & `warg-1.4.3/warg/packages/namespaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from types import ModuleType
-from typing import Any, Dict
-
 import importlib
 import pkgutil
+from types import ModuleType
+from typing import Any, Dict
 
 __all__ = ["import_submodules", "import_submodule_alls"]
 
 
 def import_submodules(package: Any, recursive: bool = True) -> Dict[str, ModuleType]:
     """Import all submodules of a module, recursively, including subpackages
```

### Comparing `Warg-1.4.2/warg/packages/pip_parsing.py` & `warg-1.4.3/warg/packages/pip_parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 import logging
 from pathlib import Path
 from typing import Union
 from urllib.parse import urlparse
 
+logger = logging.getLogger(__name__)
 from warg.functions import sink
 
 __all__ = ["get_requirements_from_file"]
 
 try:
     # from packaging.requirements import Requirement
 
@@ -61,13 +62,13 @@
             file_path = str(file_path)
 
         parsed_reqs = [get_reqed(ir) for ir in parse_requirements(file_path, session=session)]
 
         return [p for p in parsed_reqs if p]
 
 except (ModuleNotFoundError, ImportError) as e:
-    logging.error(e)
+    logger.error(e)
     get_requirements_from_file = sink
     # print('You version of python is to old!')
 
 if __name__ == "__main__":
     print(get_requirements_from_file(Path(__file__).parent.parent.parent / "requirements.txt"))
```

### Comparing `Warg-1.4.2/warg/packages/reloading.py` & `warg-1.4.3/warg/packages/reloading.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,21 @@
 
 import importlib
 import logging
 import sys
 from importlib import reload
 from importlib.util import find_spec
 from pathlib import Path
-from typing import Optional, Any, Union, List, Iterable, Callable
+from typing import Any, Callable, Iterable, List, Optional, Union
 from warnings import warn
 
 from warg.decorators import passes_kws_to
 
+logger = logging.getLogger(__name__)
+
 IGNORE = """
 PRELOADED_MODULES = set()
 def init():
   # local imports to keep things neat
   from sys import modules
 
   global PRELOADED_MODULES
@@ -107,18 +109,18 @@
     :return:
     """
     try:
         for mod in sys.modules.values():
             reload(mod)
     except Exception as e:
         if verbose:
-            logging.error(mod)
+            logger.error(mod)
         if catch_exceptions:
             if verbose:
-                logging.error(e)
+                logger.error(e)
         else:
             raise e
 
 
 def import_file(path: Path, from_list=None) -> Any:
     """
     Import a module given its filename, works both on absolute and relative paths
@@ -338,15 +340,15 @@
     if not inclusion_test:
         if position:
             sys.path.insert(position, str_path)
         else:
             sys.path.append(str_path)
     else:
         if verbose:
-            logging.warning(f"{path} is already in sys path")
+            logger.warning(f"{path} is already in sys path")
 
 
 def is_module_available(module: str) -> bool:
     """Returns True if module is available.
 
 
     :param module: Name of the module to be checked.
```

### Comparing `Warg-1.4.2/warg/packages/satisfaction.py` & `warg-1.4.3/warg/packages/satisfaction.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,21 +7,23 @@
            """
 
 __all__ = [
     "install_requirements_from_file",
 ]
 
 import logging
+
 import os
 import subprocess
 import sys
-from enum import Enum
+from enum import Enum, auto
 from pathlib import Path
 from typing import Optional
 
+logger = logging.getLogger(__name__)
 
 # from warg import is_windows # avoid dependency import not standard python pkgs.
 CUR_OS = sys.platform
 IS_WIN = any(CUR_OS.startswith(i) for i in ["win32", "cygwin"])
 IS_MAC = CUR_OS.startswith("darwin")
 VERBOSE = False
 
@@ -30,21 +32,28 @@
 def catching_callable(*args, **kwargs):
     try:
         # subprocess.check_call(*args, **kwargs)
         output = subprocess.check_output(*args, **kwargs)
         # subprocess.run(*args,**kwargs)
     except subprocess.CalledProcessError as e:
         output = (e.stderr, e.stdout, e)
-    logging.warning(output)
+    logger.warning(output)
 
 
 SP_CALLABLE = catching_callable  # subprocess.call
 DEFAULT_PIP_INDEX = os.environ.get("PIP_INDEX_URL", "https://pypi.org/pypi/")
 
 
+class InstallStrategyEnum(Enum):
+    """ """
+
+    uninstall_first = auto()  # TODO: HOW MANY TIME TO DO THIS?
+    just_install = auto()
+
+
 def is_pip_installed():
     pip_present = True
     try:
         import pip
     except ImportError:
         pip_present = False
     return pip_present
@@ -60,39 +69,44 @@
     fallback = True
 
     if IS_WIN:
         try_path = interpreter_path.parent / "python.exe"
         if not try_path.exists():
             try_path = interpreter_path.parent / "python3.exe"
             if not try_path.exists():
-                logging.error(f"Could not find python {try_path}")
+                logger.error(f"Could not find python {try_path}")
                 if not fallback:
                     return None
             else:
                 return try_path
         else:
             return try_path
 
     elif IS_MAC:
         try_path = interpreter_path.parent / "bin" / "python"
         if not try_path.exists():
             try_path = interpreter_path.parent / "bin" / "python3"
             if not try_path.exists():
-                logging.error(f"Could not find python {try_path}")
+                logger.error(f"Could not find python {try_path}")
                 if not fallback:
                     return None
             else:
                 return try_path
         else:
             return try_path
 
     return interpreter_path
 
 
-def install_pip_if_not_present(always_upgrade: bool = True):
+def install_pip_if_not_present(
+    always_upgrade: bool = True, install_strategy: InstallStrategyEnum = InstallStrategyEnum.just_install
+):
+    if install_strategy == InstallStrategyEnum.uninstall_first:
+        ...  # TODO: Implement
+
     if not is_pip_installed() or always_upgrade:
         if False:
             import ensurepip
 
             ensurepip.bootstrap(upgrade=True)
         else:
             SP_CALLABLE(
@@ -127,14 +141,39 @@
     only_if_needed = "only-if-needed"
 
 
 # subprocess.Popen(**ADDITIONAL_PIPE_KWS)
 # ADDITIONAL_PIPE_KWS = dict(stderr=subprocess.PIPE,stdout=subprocess.PIPE, stdin=subprocess.PIPE)
 
 
+def pip_programatic_install(package):
+    """
+    not supported
+    :param package:
+    :return:
+    """
+    import importlib
+
+    try:
+        importlib.import_module(package)
+    except ImportError:
+        import pip
+
+        if hasattr(pip, "main"):
+            pip.main(["install", package])
+        else:
+            pip._internal.main(["install", package])
+    finally:
+        globals()[package] = importlib.import_module(package)
+        import site
+        from importlib import reload
+
+        reload(site)
+
+
 def install_requirements_from_file(
     requirements_path: Path,
     upgrade: Optional[bool] = None,
     upgrade_strategy: UpgradeStrategyEnum = UpgradeStrategyEnum.only_if_needed,
 ) -> None:
     """
     Install requirements from a requirements.txt file.
@@ -157,14 +196,17 @@
 
     if True:
         args += ["--user"]
 
     if upgrade:
         args += ["--upgrade"]
 
+    if True:
+        args += ["--ignore-installed"]
+
     if upgrade_strategy:
         args += ["--upgrade-strategy", upgrade_strategy.value]
 
     if False:
         import pip
 
         pip.main(args)
@@ -175,12 +217,12 @@
     elif True:
         install_pip_if_not_present()
 
         if is_pip_installed():
             SP_CALLABLE([str(get_embedded_python_interpreter_path()), "-m", "pip", *args])
 
         else:
-            logging.info("PIP IS STILL MISSING!")
+            logger.info("PIP IS STILL MISSING!")
 
 
 if __name__ == "__main__":
     print(get_embedded_python_interpreter_path())
```

### Comparing `Warg-1.4.2/warg/packages/versioning.py` & `warg-1.4.3/warg/packages/versioning.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #!/usr/bin/env python3
 
 __all__ = ["get_version"]
 
+import datetime
 import logging
 from pathlib import Path
-import datetime
-from logging import warning
+
+logger = logging.getLogger(__name__)
 
 
 class NotGitException(Exception):
     pass
 
 
 def get_version(version: str, append_time: bool = False, verbose: bool = False, context: Path = None) -> str:
     """
 
+    :param context:
     :param verbose:
     :param version:
     :param append_time:
     :return:
     """
 
     if not version:
@@ -28,20 +30,22 @@
         import subprocess
 
         if context is None:
             import inspect
             import os
 
             caller_parent = Path(os.path.abspath((inspect.stack()[1])[1])).resolve().parent
+
         else:
             context = Path(context)
             if context.is_file():
                 caller_parent = context.parent
             else:
                 caller_parent = context
+
         if (caller_parent / ".git").exists() and (caller_parent / ".git").is_dir():
             git_version = (
                 subprocess.check_output(
                     [
                         "git",
                         "describe",
                         "--always",
@@ -49,40 +53,45 @@
                         "origin/HEAD",
                     ],
                     cwd=caller_parent,
                 )
                 .strip()
                 .decode()
             )
+
             current_git_version = (
                 subprocess.check_output(
                     [
                         "git",
                         "describe",
                         "--always",
                         "--dirty",
                     ],
                     cwd=caller_parent,
                 )
                 .strip()
                 .decode()
             )
+
             if "dirty" in current_git_version:
-                warning(f"{caller_parent} git is dirty, {current_git_version}")
+                logger.warning(f"{caller_parent} git is dirty, {current_git_version}")
 
             if git_version.split("-")[0] != version:
                 msg = f"{caller_parent} git version {git_version} does not match __version__" f" {version}"
-                warning(msg)
+                logger.warning(msg)
                 assert git_version.split("-")[0] == version, msg
+
             else:
                 if verbose:
                     msg = f"{caller_parent} git version {git_version} matches __version__" f" {version}"
-                    logging.info(msg)
+                    logger.info(msg)
+
         else:
             raise NotGitException
+
     except:
         if append_time:
             now = datetime.datetime.utcnow()
             date_version = now.strftime("%Y%m%d%H%M%S")
             # date_version = time.time()
 
             if version:
@@ -97,15 +106,17 @@
                 # uses the 'basic' ISO8601 format for both its date and time components
                 # to avoid issues with the colon character (ISO requires that date and
                 # time components of a date-time string must be uniformly basic or
                 # extended, which is why the date component does not have dashes.)
                 #
                 # Publications using datetime versions should only be made from master
                 # to represent the HEAD moving forward.
-                warning(f"Environment variable VERSION is not set, only using datetime: {date_version}")
+                logger.warning(
+                    f"Environment variable VERSION is not set, only using datetime: {date_version}"
+                )
 
                 # warn(f'Environment variable VERSION is not set, only using timestamp: {version}')
 
             version = f"{version}.{date_version}"
 
     return version
```

### Comparing `Warg-1.4.2/warg/plugin.py` & `warg-1.4.3/warg/plugin.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/replication.py` & `warg-1.4.3/warg/replication.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/strings.py` & `warg-1.4.3/warg/strings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/text.py` & `warg-1.4.3/warg/text.py`

 * *Files identical despite different names*

### Comparing `Warg-1.4.2/warg/typing_extension.py` & `warg-1.4.3/warg/typing_extension.py`

 * *Files identical despite different names*

