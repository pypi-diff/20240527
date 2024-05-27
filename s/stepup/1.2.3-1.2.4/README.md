# Comparing `tmp/stepup-1.2.3.tar.gz` & `tmp/stepup-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepup-1.2.3.tar", last modified: Sun May 19 11:05:50 2024, max compression
+gzip compressed data, was "stepup-1.2.4.tar", last modified: Mon May 27 07:21:40 2024, max compression
```

## Comparing `stepup-1.2.3.tar` & `stepup-1.2.4.tar`

### file list

```diff
@@ -1,950 +1,978 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.324799 stepup-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-19 11:05:46.000000 stepup-1.2.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.180800 stepup-1.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.192800 stepup-1.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-19 11:05:46.000000 stepup-1.2.3/.github/workflows/mkdocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-19 11:05:46.000000 stepup-1.2.3/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-19 11:05:46.000000 stepup-1.2.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-19 11:05:46.000000 stepup-1.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-19 11:05:46.000000 stepup-1.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 11:05:46.000000 stepup-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-19 11:05:50.324799 stepup-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-19 11:05:46.000000 stepup-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.196800 stepup-1.2.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.196800 stepup-1.2.3/docs/advanced_topics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.200800 stepup-1.2.3/docs/advanced_topics/amending_static_inputs/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_static_inputs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_static_inputs/config.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      149 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_static_inputs/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_static_inputs/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_static_inputs/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_static_inputs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.200800 stepup-1.2.3/docs/advanced_topics/amending_steps/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_steps/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_steps/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      262 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_steps/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_steps/stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_steps/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_steps.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.200800 stepup-1.2.3/docs/advanced_topics/blocked_steps/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/blocked_steps/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/blocked_steps/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      161 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/blocked_steps/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/blocked_steps/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/blocked_steps.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.200800 stepup-1.2.3/docs/advanced_topics/cyclic_dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/cyclic_dependencies/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/cyclic_dependencies/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/cyclic_dependencies/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/cyclic_dependencies/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/cyclic_dependencies.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.200800 stepup-1.2.3/docs/advanced_topics/environment_variables/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/environment_variables/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      141 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/environment_variables/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       91 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/environment_variables/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/environment_variables/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/environment_variables.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.200800 stepup-1.2.3/docs/advanced_topics/here_and_root/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/here_and_root/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/here_and_root/main.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.200800 stepup-1.2.3/docs/advanced_topics/here_and_root/source/
--rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/here_and_root/source/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.200800 stepup-1.2.3/docs/advanced_topics/here_and_root/source/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/here_and_root/source/sub/example.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/here_and_root/source/sub/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/here_and_root/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/here_and_root.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/introduction.md
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/manual_cleaning.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.204800 stepup-1.2.3/docs/advanced_topics/optional_steps/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      438 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps/generate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps/matplotlibrc
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    62512 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps/plot_logmap.png
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.204800 stepup-1.2.3/docs/advanced_topics/pools/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/pools/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/pools/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      195 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/pools/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/pools/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/pools.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.204800 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/bar.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/foo.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/graph_creator.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/graph_supplier.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.204800 stepup-1.2.3/docs/advanced_topics/static_named_glob/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.204800 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch1/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch1/sec1_1_introduction.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch1/sec1_2_objectives.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch1/unused.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.204800 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch2/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch2/sec2_1_mathematical_requisites.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch2/sec2_2_theory.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.208800 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch3/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch3/sec3_1_applications.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch3/sec3_2_discussion.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.208800 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch4/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch4/sec4_1_summary.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      647 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob.md
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/stepup_root.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.208800 stepup-1.2.3/docs/advanced_topics/variable_substitution/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/variable_substitution/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/variable_substitution/dst_foo.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/variable_substitution/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      186 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/variable_substitution/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/variable_substitution/src_foo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/variable_substitution/stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/variable_substitution/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/variable_substitution.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.208800 stepup-1.2.3/docs/advanced_topics/volatile_outputs/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/volatile_outputs/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/volatile_outputs/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       96 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/volatile_outputs/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/volatile_outputs/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/volatile_outputs.md
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/clean_stdout.sed
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/development.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.212800 stepup-1.2.3/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/automatic_cleaning.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.212800 stepup-1.2.3/docs/getting_started/copy_mkdir/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/copy_mkdir/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/copy_mkdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/copy_mkdir/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/copy_mkdir/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/copy_mkdir.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.212800 stepup-1.2.3/docs/getting_started/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/dependencies/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/dependencies/graph_creator.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/dependencies/graph_supplier.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      286 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/dependencies/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      233 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/dependencies/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/dependencies/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/dependencies.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.212800 stepup-1.2.3/docs/getting_started/distributed_plans/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/distributed_plans/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/distributed_plans/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/distributed_plans/part1.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/distributed_plans/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/distributed_plans/stdout.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.212800 stepup-1.2.3/docs/getting_started/distributed_plans/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/distributed_plans/sub/part2.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/distributed_plans/sub/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/distributed_plans.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.212800 stepup-1.2.3/docs/getting_started/first_step/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/first_step/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      218 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/first_step/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       81 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/first_step/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/first_step/stdout1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/first_step/stdout2.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/first_step/stdout3.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/first_step.md
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/interactive_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/introduction.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.216800 stepup-1.2.3/docs/getting_started/no_rules/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/no_rules/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/no_rules/lower1.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/no_rules/lower2.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/no_rules/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/no_rules/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/no_rules/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/no_rules.md
--rw-r--r--   0 runner    (1001) docker     (127)    16830 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/processes.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.216800 stepup-1.2.3/docs/getting_started/script_multiple/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/ebbr.csv
--rw-r--r--   0 runner    (1001) docker     (127)    13550 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/ebos.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)      199 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/matplotlibrc
--rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      963 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    60027 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/plot_ebbr.png
--rw-r--r--   0 runner    (1001) docker     (127)    69904 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/plot_ebos.png
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.216800 stepup-1.2.3/docs/getting_started/script_single/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_single/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_single/config.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      509 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_single/generate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_single/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_single/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_single/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_single.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.216800 stepup-1.2.3/docs/getting_started/static_files/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_files/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_files/limerick.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      152 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_files/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      154 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_files/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_files/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_files.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.220800 stepup-1.2.3/docs/getting_started/static_glob/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.220800 stepup-1.2.3/docs/getting_started/static_glob/src/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob/src/bar.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob/src/foo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.220800 stepup-1.2.3/docs/getting_started/static_glob_conditional/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob_conditional/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.220800 stepup-1.2.3/docs/getting_started/static_glob_conditional/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob_conditional/dataset/bigfile.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      232 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob_conditional/expensive.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob_conditional/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      339 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob_conditional/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob_conditional/stdout1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob_conditional/stdout2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob_conditional.md
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/license.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1847 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.220800 stepup-1.2.3/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/reference/interactive.md
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/reference/stepup.core.api.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/reference/stepup.core.interact.md
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/reference/stepup.core.nglob.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/run_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-19 11:05:46.000000 stepup-1.2.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-19 11:05:46.000000 stepup-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:05:50.324799 stepup-1.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.184800 stepup-1.2.3/stepup/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.224800 stepup-1.2.3/stepup/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/assoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)    19597 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/cascade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/deferred_glob.py
--rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/director.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    12834 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/interact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    28646 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/nglob.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16280 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12450 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/script.py
--rw-r--r--   0 runner    (1001) docker     (127)    27140 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/tui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    19965 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    32855 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.324799 stepup-1.2.3/stepup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-19 11:05:50.000000 stepup-1.2.3/stepup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    33367 2024-05-19 11:05:50.000000 stepup-1.2.3/stepup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:05:50.000000 stepup-1.2.3/stepup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-19 11:05:50.000000 stepup-1.2.3/stepup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-19 11:05:50.000000 stepup-1.2.3/stepup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 11:05:50.000000 stepup-1.2.3/stepup.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.228800 stepup-1.2.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.228800 stepup-1.2.3/tests/cases/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.228800 stepup-1.2.3/tests/cases/amend/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/expected_graph_04.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/expected_stdout_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/expected_stdout_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/inp1.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2563 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      250 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.232800 stepup-1.2.3/tests/cases/amend_delay/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1755 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      308 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      307 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.232800 stepup-1.2.3/tests/cases/amend_env_vars/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_env_vars/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_env_vars/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_env_vars/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_env_vars/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_env_vars/foo.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      845 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_env_vars/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      100 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_env_vars/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_env_vars/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.232800 stepup-1.2.3/tests/cases/amend_missing/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_missing/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_missing/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_missing/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_missing/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      715 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_missing/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_missing/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_missing/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.232800 stepup-1.2.3/tests/cases/amend_outdir_pending/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_outdir_pending/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_outdir_pending/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_outdir_pending/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_outdir_pending/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_outdir_pending/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_outdir_pending/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_outdir_pending/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.236800 stepup-1.2.3/tests/cases/amend_voldir_pending/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_voldir_pending/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_voldir_pending/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_voldir_pending/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_voldir_pending/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_voldir_pending/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_voldir_pending/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_voldir_pending/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.236800 stepup-1.2.3/tests/cases/deferred_glob1/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1538 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.236800 stepup-1.2.3/tests/cases/deferred_glob1/static/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/static/data1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/static/data2.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.236800 stepup-1.2.3/tests/cases/deferred_glob1/static/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/static/sub/bar.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/static/sub/foo.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.236800 stepup-1.2.3/tests/cases/deferred_glob2/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1137 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/plan_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.236800 stepup-1.2.3/tests/cases/deferred_glob2/static/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/static/data1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/static/data2.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.240800 stepup-1.2.3/tests/cases/deferred_glob2/static/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/static/sub/bar.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/static/sub/foo.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.240800 stepup-1.2.3/tests/cases/deferred_subdir/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.240800 stepup-1.2.3/tests/cases/deferred_subdir/sub/
--rwxr-xr-x   0 runner    (1001) docker     (127)      119 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/sub/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/sub/unused.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/sub/used.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.244799 stepup-1.2.3/tests/cases/env_vars/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/demovars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_graph_04.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_graph_05.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_stdout_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_stdout_b.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_stdout_c.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_stdout_d.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_variables_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_variables_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_variables_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_variables_04.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_variables_05.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3862 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      183 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/printvars.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/variables_01.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/variables_02.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.244799 stepup-1.2.3/tests/cases/env_vars_amend/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/demovars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1351 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.244799 stepup-1.2.3/tests/cases/env_vars_path/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/FOO.md
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/FOO.txt
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1580 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      480 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.248799 stepup-1.2.3/tests/cases/env_vars_subs/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_subs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_subs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_subs/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_subs/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      769 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_subs/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      159 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_subs/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.248799 stepup-1.2.3/tests/cases/env_vars_subs/sub/
--rwxr-xr-x   0 runner    (1001) docker     (127)      133 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_subs/sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.248799 stepup-1.2.3/tests/cases/env_vars_workdir/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_workdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_workdir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_workdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_workdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_workdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      355 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_workdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.248799 stepup-1.2.3/tests/cases/env_vars_workdir/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_workdir/sub/input.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.248799 stepup-1.2.3/tests/cases/error_cyclic_late/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_cyclic_late/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_cyclic_late/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_cyclic_late/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_cyclic_late/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      744 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_cyclic_late/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_cyclic_late/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.248799 stepup-1.2.3/tests/cases/error_deferred_nonexisting/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_deferred_nonexisting/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_deferred_nonexisting/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_deferred_nonexisting/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      726 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_deferred_nonexisting/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_deferred_nonexisting/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.252800 stepup-1.2.3/tests/cases/error_env_var/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_env_var/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_env_var/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_env_var/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_env_var/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_env_var/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      124 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_env_var/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.252800 stepup-1.2.3/tests/cases/error_main_fails/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1369 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      101 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/plan_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.252800 stepup-1.2.3/tests/cases/error_not_executable/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_not_executable/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_not_executable/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_not_executable/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_not_executable/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_not_executable/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.252800 stepup-1.2.3/tests/cases/error_overlap_deferred/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_overlap_deferred/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_overlap_deferred/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_overlap_deferred/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_overlap_deferred/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      717 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_overlap_deferred/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_overlap_deferred/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.256800 stepup-1.2.3/tests/cases/error_static_dir/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_static_dir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_static_dir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_static_dir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_static_dir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_static_dir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_static_dir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.256800 stepup-1.2.3/tests/cases/error_static_dir/subdir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_static_dir/subdir/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.256800 stepup-1.2.3/tests/cases/error_step/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_step/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_step/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_step/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_step/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_step/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_step/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.256800 stepup-1.2.3/tests/cases/here/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/here/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/here/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/here/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/here/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      877 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/here/main.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.256800 stepup-1.2.3/tests/cases/here/source/
--rwxr-xr-x   0 runner    (1001) docker     (127)      198 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/here/source/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.256800 stepup-1.2.3/tests/cases/here/source/www/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/here/source/www/index.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/here/source/www/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.256800 stepup-1.2.3/tests/cases/makedirs/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/makedirs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/makedirs/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      457 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/makedirs/bunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/makedirs/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/makedirs/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      763 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/makedirs/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/makedirs/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.260800 stepup-1.2.3/tests/cases/mkdir/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.260800 stepup-1.2.3/tests/cases/mkdir/exists/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir/exists/.keep
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      237 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.260800 stepup-1.2.3/tests/cases/mkdir_error/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir_error/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir_error/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir_error/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir_error/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir_error/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       79 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir_error/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.260800 stepup-1.2.3/tests/cases/nodata/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/expected_stdout_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/expected_stdout_b.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1820 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/original.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      259 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.264799 stepup-1.2.3/tests/cases/noplan/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/noplan/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/noplan/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/noplan/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      283 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/noplan/main.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.264799 stepup-1.2.3/tests/cases/nostatic/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nostatic/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nostatic/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nostatic/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nostatic/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1947 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nostatic/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nostatic/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.264799 stepup-1.2.3/tests/cases/not_cyclic/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/not_cyclic/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/not_cyclic/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/not_cyclic/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/not_cyclic/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/not_cyclic/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/not_cyclic/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1539 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/not_cyclic/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      211 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/not_cyclic/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.268799 stepup-1.2.3/tests/cases/optional_convert/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/expected_graph_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/expected_graph_b.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/expected_graph_c.txt
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/expected_stdout_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/expected_stdout_b.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1865 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/raw_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/raw_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/raw_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/raw_04.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.268799 stepup-1.2.3/tests/cases/output_not_created/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/output_not_created/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/output_not_created/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/output_not_created/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/output_not_created/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      780 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/output_not_created/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/output_not_created/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.268799 stepup-1.2.3/tests/cases/pending/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pending/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pending/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pending/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pending/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pending/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      143 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pending/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.268799 stepup-1.2.3/tests/cases/permissions_file_rerun/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_file_rerun/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_file_rerun/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_file_rerun/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_file_rerun/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_file_rerun/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_file_rerun/input.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1351 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_file_rerun/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_file_rerun/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.272799 stepup-1.2.3/tests/cases/permissions_plan_rerun/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_rerun/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_rerun/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_rerun/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_rerun/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_rerun/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1137 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_rerun/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_rerun/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.272799 stepup-1.2.3/tests/cases/permissions_plan_rerun/sub/
--rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_rerun/sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.272799 stepup-1.2.3/tests/cases/permissions_plan_restart/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1465 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.272799 stepup-1.2.3/tests/cases/permissions_plan_restart/sub/
--rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.272799 stepup-1.2.3/tests/cases/permissions_step_rerun/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_rerun/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_rerun/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_rerun/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_rerun/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_rerun/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1115 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_rerun/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_rerun/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_rerun/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.276799 stepup-1.2.3/tests/cases/permissions_step_restart/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1383 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.276799 stepup-1.2.3/tests/cases/pool/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pool/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pool/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pool/expected_graph.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      741 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pool/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pool/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pool/r.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.276799 stepup-1.2.3/tests/cases/reqdir_missing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/reqdir_missing/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/reqdir_missing/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/reqdir_missing/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/reqdir_missing/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/reqdir_missing/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      136 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/reqdir_missing/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.280799 stepup-1.2.3/tests/cases/restart_blocked/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/expensive.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/initial.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1377 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/plan_blocked.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/plan_unblocked.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.280799 stepup-1.2.3/tests/cases/restart_changes/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1719 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      301 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      301 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/plan_02.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/source_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/source_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/source_both.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.280799 stepup-1.2.3/tests/cases/restart_deferred_glob/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1269 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.280799 stepup-1.2.3/tests/cases/restart_deferred_glob/static/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/static/foo.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.284799 stepup-1.2.3/tests/cases/restart_nochanges/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_nochanges/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_nochanges/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_nochanges/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_nochanges/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_nochanges/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_nochanges/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1391 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_nochanges/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      296 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_nochanges/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.284799 stepup-1.2.3/tests/cases/restart_orphan/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_orphan/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_orphan/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_orphan/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_orphan/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_orphan/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_orphan/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_orphan/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_orphan/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.284799 stepup-1.2.3/tests/cases/restart_outdated_amend/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1465 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.288799 stepup-1.2.3/tests/cases/restart_output/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1291 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/original.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.288799 stepup-1.2.3/tests/cases/script_cases/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases/helper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      396 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases/work.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.288799 stepup-1.2.3/tests/cases/script_cases_settings/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/helper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      422 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/work.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.292799 stepup-1.2.3/tests/cases/script_single/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_single/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_single/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_single/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_single/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      792 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_single/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      193 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_single/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.292799 stepup-1.2.3/tests/cases/script_single/work/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_single/work/config.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      554 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_single/work/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.292799 stepup-1.2.3/tests/cases/static/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static/original.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       81 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.292799 stepup-1.2.3/tests/cases/static_abs/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_abs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_abs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_abs/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_abs/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_abs/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_abs/original.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_abs/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.292799 stepup-1.2.3/tests/cases/static_dir/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_dir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_dir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_dir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_dir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      748 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_dir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       76 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_dir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.296799 stepup-1.2.3/tests/cases/static_glob/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/expected_stdout_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/expected_stdout_b.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2012 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.296799 stepup-1.2.3/tests/cases/static_nglob/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.296799 stepup-1.2.3/tests/cases/static_nglob/ch-1-intro/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/ch-1-intro/sec-1-1-blabla.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/ch-1-intro/sec-1-2-some-more.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.296799 stepup-1.2.3/tests/cases/static_nglob/ch-2-theory/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/ch-2-theory/sec-2-1-basics.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.296799 stepup-1.2.3/tests/cases/static_nglob/ch-3-conclusions/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/ch-3-conclusions/sec-3-1-summary.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/ch-3-conclusions/sec-3-2-outlook.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18883 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18883 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3657 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      972 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/sec-2-2.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.300799 stepup-1.2.3/tests/cases/static_nglob_partial/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/expected_graph_04.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/expected_stdout_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/expected_stdout_b.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2458 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.300799 stepup-1.2.3/tests/cases/static_nglob_subdir/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      895 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.300799 stepup-1.2.3/tests/cases/static_nglob_subdir/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/sub/inp1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/sub/inp2.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.300799 stepup-1.2.3/tests/cases/subdir/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/subdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/subdir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/subdir/example.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/subdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/subdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      789 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/subdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/subdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.304799 stepup-1.2.3/tests/cases/subdir/sub/
--rwxr-xr-x   0 runner    (1001) docker     (127)      450 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/subdir/sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.304799 stepup-1.2.3/tests/cases/watch_blocked/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/expensive.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/initial.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/plan_blocked.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/plan_unblocked.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.304799 stepup-1.2.3/tests/cases/watch_boot/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_boot/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_boot/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_boot/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_boot/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_boot/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1136 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_boot/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_boot/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_boot/plan_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.308799 stepup-1.2.3/tests/cases/watch_chain/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/config_01.json
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/config_02.json
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1222 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      546 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/use_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.308799 stepup-1.2.3/tests/cases/watch_input/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/first.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1093 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/second.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.312799 stepup-1.2.3/tests/cases/watch_middle/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/original.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      235 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      247 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/plan_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.312799 stepup-1.2.3/tests/cases/watch_mixed/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/backup.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      978 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      219 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/plan_full.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/plan_trimmed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.316799 stepup-1.2.3/tests/cases/watch_nochanges/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_nochanges/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_nochanges/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_nochanges/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_nochanges/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_nochanges/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_nochanges/input.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1029 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_nochanges/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_nochanges/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.316799 stepup-1.2.3/tests/cases/watch_outdated_amend1/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend1/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend1/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend1/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1224 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend1/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend1/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend1/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.320799 stepup-1.2.3/tests/cases/watch_outdated_amend2/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend2/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend2/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend2/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1413 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend2/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      331 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend2/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend2/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.320799 stepup-1.2.3/tests/cases/watch_output/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/input.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1073 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/second.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.324799 stepup-1.2.3/tests/cases/watch_wanted/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1691 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      328 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/plan_02.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/core_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/echo_server_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/echo_server_stdio.py
--rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_assoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_cascade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)    21270 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_nglob.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    65157 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.620907 stepup-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-27 07:21:33.000000 stepup-1.2.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.480908 stepup-1.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.492908 stepup-1.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-27 07:21:33.000000 stepup-1.2.4/.github/workflows/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-27 07:21:33.000000 stepup-1.2.4/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-27 07:21:33.000000 stepup-1.2.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-27 07:21:33.000000 stepup-1.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-27 07:21:33.000000 stepup-1.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 07:21:33.000000 stepup-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-27 07:21:40.620907 stepup-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-27 07:21:33.000000 stepup-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.496908 stepup-1.2.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.496908 stepup-1.2.4/docs/advanced_topics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.496908 stepup-1.2.4/docs/advanced_topics/amending_static_inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/amending_static_inputs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/amending_static_inputs/config.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      149 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/amending_static_inputs/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/amending_static_inputs/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/amending_static_inputs/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/amending_static_inputs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.500908 stepup-1.2.4/docs/advanced_topics/amending_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/amending_steps/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/amending_steps/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      262 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/amending_steps/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/amending_steps/stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/amending_steps/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/amending_steps.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.500908 stepup-1.2.4/docs/advanced_topics/blocked_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/blocked_steps/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/blocked_steps/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      161 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/blocked_steps/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/blocked_steps/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/blocked_steps.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.500908 stepup-1.2.4/docs/advanced_topics/cyclic_dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/cyclic_dependencies/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/cyclic_dependencies/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/cyclic_dependencies/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/cyclic_dependencies/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/cyclic_dependencies.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.500908 stepup-1.2.4/docs/advanced_topics/environment_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/environment_variables/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      141 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/environment_variables/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       91 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/environment_variables/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/environment_variables/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/environment_variables.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.500908 stepup-1.2.4/docs/advanced_topics/here_and_root/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/here_and_root/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/here_and_root/main.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.500908 stepup-1.2.4/docs/advanced_topics/here_and_root/source/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/here_and_root/source/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.500908 stepup-1.2.4/docs/advanced_topics/here_and_root/source/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/here_and_root/source/sub/example.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/here_and_root/source/sub/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/here_and_root/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/here_and_root.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/manual_cleaning.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.500908 stepup-1.2.4/docs/advanced_topics/optional_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/optional_steps/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      438 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/optional_steps/generate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/optional_steps/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/optional_steps/matplotlibrc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/optional_steps/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/optional_steps/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62512 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/optional_steps/plot_logmap.png
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/optional_steps/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/optional_steps.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.504908 stepup-1.2.4/docs/advanced_topics/pools/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/pools/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/pools/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      195 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/pools/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/pools/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/pools.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.504908 stepup-1.2.4/docs/advanced_topics/static_deferred_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_deferred_glob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_deferred_glob/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_deferred_glob/foo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_deferred_glob/graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_deferred_glob/graph_creator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_deferred_glob/graph_supplier.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_deferred_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_deferred_glob/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_deferred_glob/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_deferred_glob.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.504908 stepup-1.2.4/docs/advanced_topics/static_named_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_named_glob/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.504908 stepup-1.2.4/docs/advanced_topics/static_named_glob/ch1/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_named_glob/ch1/sec1_1_introduction.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_named_glob/ch1/sec1_2_objectives.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_named_glob/ch1/unused.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.504908 stepup-1.2.4/docs/advanced_topics/static_named_glob/ch2/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_named_glob/ch2/sec2_1_mathematical_requisites.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_named_glob/ch2/sec2_2_theory.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.504908 stepup-1.2.4/docs/advanced_topics/static_named_glob/ch3/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_named_glob/ch3/sec3_1_applications.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_named_glob/ch3/sec3_2_discussion.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.504908 stepup-1.2.4/docs/advanced_topics/static_named_glob/ch4/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_named_glob/ch4/sec4_1_summary.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_named_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      647 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_named_glob/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_named_glob/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/static_named_glob.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/stepup_root.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.508908 stepup-1.2.4/docs/advanced_topics/variable_substitution/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/variable_substitution/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/variable_substitution/dst_foo.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/variable_substitution/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      186 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/variable_substitution/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/variable_substitution/src_foo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/variable_substitution/stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/variable_substitution/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/variable_substitution.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.508908 stepup-1.2.4/docs/advanced_topics/volatile_outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/volatile_outputs/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/volatile_outputs/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       96 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/volatile_outputs/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/volatile_outputs/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/advanced_topics/volatile_outputs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/clean_stdout.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/development.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.508908 stepup-1.2.4/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/automatic_cleaning.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.508908 stepup-1.2.4/docs/getting_started/copy_mkdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/copy_mkdir/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/copy_mkdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/copy_mkdir/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/copy_mkdir/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/copy_mkdir.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.512908 stepup-1.2.4/docs/getting_started/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/dependencies/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/dependencies/graph_creator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/dependencies/graph_supplier.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      286 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/dependencies/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      233 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/dependencies/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/dependencies/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/dependencies.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.512908 stepup-1.2.4/docs/getting_started/distributed_plans/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/distributed_plans/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/distributed_plans/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/distributed_plans/part1.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/distributed_plans/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/distributed_plans/stdout.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.512908 stepup-1.2.4/docs/getting_started/distributed_plans/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/distributed_plans/sub/part2.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/distributed_plans/sub/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/distributed_plans.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.512908 stepup-1.2.4/docs/getting_started/first_step/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/first_step/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      218 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/first_step/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       81 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/first_step/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/first_step/stdout1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/first_step/stdout2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/first_step/stdout3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/first_step.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/interactive_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/introduction.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.512908 stepup-1.2.4/docs/getting_started/no_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/no_rules/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/no_rules/lower1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/no_rules/lower2.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/no_rules/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/no_rules/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/no_rules/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/no_rules.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16830 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/processes.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.516908 stepup-1.2.4/docs/getting_started/script_multiple/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_multiple/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_multiple/ebbr.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    13550 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_multiple/ebos.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)      199 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_multiple/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_multiple/matplotlibrc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_multiple/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      963 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_multiple/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60027 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_multiple/plot_ebbr.png
+-rw-r--r--   0 runner    (1001) docker     (127)    69904 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_multiple/plot_ebos.png
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_multiple/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_multiple.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.516908 stepup-1.2.4/docs/getting_started/script_single/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_single/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_single/config.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      509 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_single/generate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_single/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_single/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_single/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/script_single.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.516908 stepup-1.2.4/docs/getting_started/static_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_files/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_files/limerick.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      152 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_files/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      154 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_files/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_files/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_files.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.516908 stepup-1.2.4/docs/getting_started/static_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_glob/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_glob/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.516908 stepup-1.2.4/docs/getting_started/static_glob/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_glob/src/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_glob/src/foo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_glob/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_glob.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.520908 stepup-1.2.4/docs/getting_started/static_glob_conditional/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_glob_conditional/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.520908 stepup-1.2.4/docs/getting_started/static_glob_conditional/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_glob_conditional/dataset/bigfile.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      232 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_glob_conditional/expensive.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_glob_conditional/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      339 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_glob_conditional/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_glob_conditional/stdout1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_glob_conditional/stdout2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/getting_started/static_glob_conditional.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/license.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1847 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.520908 stepup-1.2.4/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/reference/interactive.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/reference/stepup.core.api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/reference/stepup.core.interact.md
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/reference/stepup.core.nglob.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-05-27 07:21:33.000000 stepup-1.2.4/docs/run_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-27 07:21:33.000000 stepup-1.2.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-27 07:21:33.000000 stepup-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:21:40.620907 stepup-1.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.484908 stepup-1.2.4/stepup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.524908 stepup-1.2.4/stepup/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20528 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/assoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19309 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/cascade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/deferred_glob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18192 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/interact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29835 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/nglob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12450 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28979 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/tui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19974 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33062 2024-05-27 07:21:33.000000 stepup-1.2.4/stepup/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.620907 stepup-1.2.4/stepup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-27 07:21:40.000000 stepup-1.2.4/stepup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34377 2024-05-27 07:21:40.000000 stepup-1.2.4/stepup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:21:40.000000 stepup-1.2.4/stepup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-27 07:21:40.000000 stepup-1.2.4/stepup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-27 07:21:40.000000 stepup-1.2.4/stepup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 07:21:40.000000 stepup-1.2.4/stepup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.528908 stepup-1.2.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.528908 stepup-1.2.4/tests/cases/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.528908 stepup-1.2.4/tests/cases/amend/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend/expected_graph_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend/expected_stdout_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend/expected_stdout_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend/inp1.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2563 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      250 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.532908 stepup-1.2.4/tests/cases/amend_delay/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_delay/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_delay/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_delay/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_delay/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_delay/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_delay/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1755 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_delay/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      308 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_delay/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      307 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_delay/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.532908 stepup-1.2.4/tests/cases/amend_env_vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_env_vars/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_env_vars/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_env_vars/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_env_vars/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_env_vars/foo.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      845 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_env_vars/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      100 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_env_vars/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_env_vars/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.532908 stepup-1.2.4/tests/cases/amend_missing/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_missing/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_missing/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_missing/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_missing/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      715 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_missing/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_missing/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_missing/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.536908 stepup-1.2.4/tests/cases/amend_outdir_pending/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_outdir_pending/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_outdir_pending/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_outdir_pending/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_outdir_pending/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_outdir_pending/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_outdir_pending/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_outdir_pending/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.536908 stepup-1.2.4/tests/cases/amend_self_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_self_static/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2153 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_self_static/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_self_static/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      211 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_self_static/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.536908 stepup-1.2.4/tests/cases/amend_voldir_pending/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_voldir_pending/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_voldir_pending/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_voldir_pending/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_voldir_pending/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_voldir_pending/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_voldir_pending/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/amend_voldir_pending/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.536908 stepup-1.2.4/tests/cases/deferred_glob1/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob1/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob1/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob1/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob1/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1538 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob1/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob1/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.536908 stepup-1.2.4/tests/cases/deferred_glob1/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob1/static/data1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob1/static/data2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.536908 stepup-1.2.4/tests/cases/deferred_glob1/static/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob1/static/sub/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob1/static/sub/foo.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.540908 stepup-1.2.4/tests/cases/deferred_glob2/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob2/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob2/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob2/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1137 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob2/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob2/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob2/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.540908 stepup-1.2.4/tests/cases/deferred_glob2/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob2/static/data1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob2/static/data2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.540908 stepup-1.2.4/tests/cases/deferred_glob2/static/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob2/static/sub/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_glob2/static/sub/foo.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.540908 stepup-1.2.4/tests/cases/deferred_subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_subdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.540908 stepup-1.2.4/tests/cases/deferred_subdir/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      119 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_subdir/sub/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_subdir/sub/unused.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/deferred_subdir/sub/used.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.544908 stepup-1.2.4/tests/cases/env_vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/demovars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/expected_graph_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/expected_graph_05.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/expected_stdout_b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/expected_stdout_c.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/expected_stdout_d.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/expected_variables_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/expected_variables_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/expected_variables_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/expected_variables_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/expected_variables_05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3862 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      183 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/printvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/variables_01.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars/variables_02.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.544908 stepup-1.2.4/tests/cases/env_vars_amend/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_amend/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_amend/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_amend/demovars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_amend/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_amend/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_amend/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_amend/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1351 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_amend/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_amend/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.548908 stepup-1.2.4/tests/cases/env_vars_path/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_path/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_path/FOO.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_path/FOO.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_path/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_path/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_path/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_path/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_path/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1580 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_path/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      480 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_path/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.548908 stepup-1.2.4/tests/cases/env_vars_subs/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_subs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_subs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_subs/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_subs/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      769 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_subs/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      159 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_subs/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.548908 stepup-1.2.4/tests/cases/env_vars_subs/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      133 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_subs/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.548908 stepup-1.2.4/tests/cases/env_vars_workdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_workdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_workdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_workdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_workdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_workdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      355 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_workdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.548908 stepup-1.2.4/tests/cases/env_vars_workdir/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/env_vars_workdir/sub/input.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.552908 stepup-1.2.4/tests/cases/error_cyclic_late/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_cyclic_late/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_cyclic_late/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_cyclic_late/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_cyclic_late/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      744 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_cyclic_late/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_cyclic_late/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.552908 stepup-1.2.4/tests/cases/error_deferred_nonexisting/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_deferred_nonexisting/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_deferred_nonexisting/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_deferred_nonexisting/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      726 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_deferred_nonexisting/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_deferred_nonexisting/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.552908 stepup-1.2.4/tests/cases/error_env_var/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_env_var/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_env_var/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_env_var/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_env_var/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_env_var/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      124 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_env_var/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.552908 stepup-1.2.4/tests/cases/error_main_fails/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_main_fails/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_main_fails/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_main_fails/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_main_fails/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_main_fails/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_main_fails/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1369 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_main_fails/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      101 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_main_fails/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_main_fails/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.556908 stepup-1.2.4/tests/cases/error_not_executable/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_not_executable/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_not_executable/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_not_executable/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_not_executable/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_not_executable/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.556908 stepup-1.2.4/tests/cases/error_overlap_deferred/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_overlap_deferred/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_overlap_deferred/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_overlap_deferred/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_overlap_deferred/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      717 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_overlap_deferred/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_overlap_deferred/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.556908 stepup-1.2.4/tests/cases/error_static_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_static_dir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_static_dir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_static_dir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_static_dir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_static_dir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_static_dir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.556908 stepup-1.2.4/tests/cases/error_static_dir/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_static_dir/subdir/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.556908 stepup-1.2.4/tests/cases/error_step/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_step/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_step/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_step/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_step/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_step/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/error_step/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.560908 stepup-1.2.4/tests/cases/here/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/here/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/here/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/here/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/here/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      877 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/here/main.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.560908 stepup-1.2.4/tests/cases/here/source/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      198 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/here/source/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.560908 stepup-1.2.4/tests/cases/here/source/www/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/here/source/www/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/here/source/www/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.560908 stepup-1.2.4/tests/cases/makedirs/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/makedirs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/makedirs/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      457 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/makedirs/bunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/makedirs/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/makedirs/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      763 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/makedirs/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/makedirs/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.560908 stepup-1.2.4/tests/cases/mkdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/mkdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/mkdir/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.560908 stepup-1.2.4/tests/cases/mkdir/exists/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/mkdir/exists/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/mkdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/mkdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/mkdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      237 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/mkdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.560908 stepup-1.2.4/tests/cases/mkdir_error/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/mkdir_error/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/mkdir_error/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/mkdir_error/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/mkdir_error/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/mkdir_error/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       79 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/mkdir_error/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.564908 stepup-1.2.4/tests/cases/nodata/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/nodata/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/nodata/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/nodata/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/nodata/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/nodata/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/nodata/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/nodata/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1820 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/nodata/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/nodata/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      259 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/nodata/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.564908 stepup-1.2.4/tests/cases/noplan/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/noplan/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/noplan/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/noplan/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      283 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/noplan/main.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.564908 stepup-1.2.4/tests/cases/nostatic/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/nostatic/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/nostatic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/nostatic/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/nostatic/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1947 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/nostatic/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/nostatic/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.568908 stepup-1.2.4/tests/cases/not_cyclic/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/not_cyclic/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/not_cyclic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/not_cyclic/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/not_cyclic/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/not_cyclic/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/not_cyclic/expected_graph_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/not_cyclic/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/not_cyclic/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2153 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/not_cyclic/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      211 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/not_cyclic/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.568908 stepup-1.2.4/tests/cases/optional_convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/optional_convert/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/optional_convert/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/optional_convert/expected_graph_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/optional_convert/expected_graph_b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/optional_convert/expected_graph_c.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/optional_convert/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/optional_convert/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1865 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/optional_convert/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/optional_convert/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/optional_convert/raw_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/optional_convert/raw_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/optional_convert/raw_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/optional_convert/raw_04.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.568908 stepup-1.2.4/tests/cases/output_not_created/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/output_not_created/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/output_not_created/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/output_not_created/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/output_not_created/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      780 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/output_not_created/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/output_not_created/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.568908 stepup-1.2.4/tests/cases/pending/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pending/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pending/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pending/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pending/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pending/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      143 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pending/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.572908 stepup-1.2.4/tests/cases/permissions_file_rerun/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_file_rerun/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_file_rerun/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_file_rerun/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_file_rerun/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_file_rerun/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_file_rerun/input.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1351 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_file_rerun/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_file_rerun/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.572908 stepup-1.2.4/tests/cases/permissions_plan_rerun/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_rerun/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_rerun/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_rerun/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_rerun/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_rerun/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1137 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_rerun/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_rerun/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.572908 stepup-1.2.4/tests/cases/permissions_plan_rerun/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_rerun/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.572908 stepup-1.2.4/tests/cases/permissions_plan_restart/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_restart/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_restart/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_restart/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_restart/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_restart/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_restart/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1465 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_restart/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_restart/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.572908 stepup-1.2.4/tests/cases/permissions_plan_restart/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_plan_restart/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.576908 stepup-1.2.4/tests/cases/permissions_step_rerun/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_rerun/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_rerun/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_rerun/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_rerun/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_rerun/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1115 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_rerun/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_rerun/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_rerun/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.576908 stepup-1.2.4/tests/cases/permissions_step_restart/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_restart/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_restart/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_restart/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_restart/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_restart/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_restart/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1383 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_restart/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_restart/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/permissions_step_restart/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.576908 stepup-1.2.4/tests/cases/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pool/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pool/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pool/expected_graph.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      741 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pool/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pool/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pool/r.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.580908 stepup-1.2.4/tests/cases/pool_restart/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pool_restart/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pool_restart/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pool_restart/expected_graph_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pool_restart/expected_graph_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pool_restart/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pool_restart/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1369 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pool_restart/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/pool_restart/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.580908 stepup-1.2.4/tests/cases/reqdir_missing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/reqdir_missing/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/reqdir_missing/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/reqdir_missing/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/reqdir_missing/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/reqdir_missing/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      136 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/reqdir_missing/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.580908 stepup-1.2.4/tests/cases/restart_blocked/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_blocked/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_blocked/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_blocked/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_blocked/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_blocked/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_blocked/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_blocked/expensive.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_blocked/initial.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1377 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_blocked/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_blocked/plan_blocked.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_blocked/plan_unblocked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.584908 stepup-1.2.4/tests/cases/restart_changes/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_changes/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_changes/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_changes/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_changes/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_changes/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_changes/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1719 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_changes/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      301 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_changes/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      301 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_changes/plan_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_changes/source_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_changes/source_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_changes/source_both.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.584908 stepup-1.2.4/tests/cases/restart_deferred_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_deferred_glob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_deferred_glob/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_deferred_glob/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_deferred_glob/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_deferred_glob/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_deferred_glob/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1269 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_deferred_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_deferred_glob/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.584908 stepup-1.2.4/tests/cases/restart_deferred_glob/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_deferred_glob/static/foo.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.584908 stepup-1.2.4/tests/cases/restart_nochanges/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_nochanges/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_nochanges/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_nochanges/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_nochanges/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_nochanges/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_nochanges/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1391 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_nochanges/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      296 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_nochanges/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.588908 stepup-1.2.4/tests/cases/restart_orphan/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_orphan/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_orphan/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_orphan/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_orphan/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_orphan/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_orphan/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_orphan/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_orphan/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.588908 stepup-1.2.4/tests/cases/restart_outdated_amend/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_outdated_amend/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_outdated_amend/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_outdated_amend/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_outdated_amend/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_outdated_amend/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_outdated_amend/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1465 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_outdated_amend/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_outdated_amend/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_outdated_amend/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.588908 stepup-1.2.4/tests/cases/restart_output/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_output/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_output/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_output/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_output/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_output/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1291 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_output/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_output/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/restart_output/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.592908 stepup-1.2.4/tests/cases/script_cases/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases/helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      396 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases/work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.592908 stepup-1.2.4/tests/cases/script_cases_settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases_settings/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases_settings/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases_settings/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases_settings/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases_settings/helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases_settings/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases_settings/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases_settings/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      422 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_cases_settings/work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.592908 stepup-1.2.4/tests/cases/script_single/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_single/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_single/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_single/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_single/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      792 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_single/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      193 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_single/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.592908 stepup-1.2.4/tests/cases/script_single/work/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_single/work/config.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      554 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/script_single/work/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.592908 stepup-1.2.4/tests/cases/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       81 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.596907 stepup-1.2.4/tests/cases/static_abs/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_abs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_abs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_abs/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_abs/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_abs/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_abs/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_abs/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.596907 stepup-1.2.4/tests/cases/static_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_dir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_dir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_dir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_dir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      748 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_dir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       76 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_dir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.596907 stepup-1.2.4/tests/cases/static_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_glob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_glob/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_glob/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_glob/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_glob/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_glob/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_glob/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2012 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_glob/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.600907 stepup-1.2.4/tests/cases/static_nglob/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.600907 stepup-1.2.4/tests/cases/static_nglob/ch-1-intro/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob/ch-1-intro/sec-1-1-blabla.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob/ch-1-intro/sec-1-2-some-more.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.600907 stepup-1.2.4/tests/cases/static_nglob/ch-2-theory/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob/ch-2-theory/sec-2-1-basics.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.600907 stepup-1.2.4/tests/cases/static_nglob/ch-3-conclusions/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob/ch-3-conclusions/sec-3-1-summary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob/ch-3-conclusions/sec-3-2-outlook.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18883 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18883 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3657 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      972 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob/sec-2-2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.600907 stepup-1.2.4/tests/cases/static_nglob_partial/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_partial/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_partial/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_partial/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_partial/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_partial/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_partial/expected_graph_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_partial/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_partial/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2458 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_partial/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_partial/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.600907 stepup-1.2.4/tests/cases/static_nglob_recursive/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_recursive/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_recursive/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.600907 stepup-1.2.4/tests/cases/static_nglob_recursive/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.604907 stepup-1.2.4/tests/cases/static_nglob_recursive/data/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_recursive/data/sub/test3.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_recursive/data/test1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_recursive/data/test2.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_recursive/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_recursive/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_recursive/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_recursive/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.604907 stepup-1.2.4/tests/cases/static_nglob_subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_subdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      895 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.604907 stepup-1.2.4/tests/cases/static_nglob_subdir/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_subdir/sub/inp1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_subdir/sub/inp2.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/static_nglob_subdir/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.604907 stepup-1.2.4/tests/cases/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/subdir/example.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/subdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      789 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.604907 stepup-1.2.4/tests/cases/subdir/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      450 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/subdir/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.608908 stepup-1.2.4/tests/cases/watch_blocked/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_blocked/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_blocked/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_blocked/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_blocked/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_blocked/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_blocked/expensive.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_blocked/initial.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_blocked/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_blocked/plan_blocked.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_blocked/plan_unblocked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.608908 stepup-1.2.4/tests/cases/watch_boot/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_boot/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_boot/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_boot/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_boot/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_boot/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1136 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_boot/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_boot/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_boot/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.608908 stepup-1.2.4/tests/cases/watch_chain/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_chain/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_chain/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_chain/config_01.json
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_chain/config_02.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_chain/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_chain/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_chain/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1222 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_chain/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_chain/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      546 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_chain/use_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.612908 stepup-1.2.4/tests/cases/watch_input/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_input/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_input/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_input/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_input/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_input/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_input/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_input/first.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1093 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_input/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_input/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_input/second.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.612908 stepup-1.2.4/tests/cases/watch_middle/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_middle/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_middle/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_middle/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_middle/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_middle/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_middle/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_middle/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_middle/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      235 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_middle/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      247 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_middle/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.612908 stepup-1.2.4/tests/cases/watch_mixed/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_mixed/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_mixed/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_mixed/backup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_mixed/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_mixed/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_mixed/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      978 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_mixed/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      219 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_mixed/plan_full.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_mixed/plan_trimmed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.616907 stepup-1.2.4/tests/cases/watch_nochanges/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_nochanges/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_nochanges/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_nochanges/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_nochanges/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_nochanges/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_nochanges/input.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1029 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_nochanges/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_nochanges/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.616907 stepup-1.2.4/tests/cases/watch_outdated_amend1/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_outdated_amend1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_outdated_amend1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_outdated_amend1/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_outdated_amend1/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_outdated_amend1/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1224 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_outdated_amend1/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_outdated_amend1/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_outdated_amend1/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.616907 stepup-1.2.4/tests/cases/watch_outdated_amend2/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_outdated_amend2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_outdated_amend2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_outdated_amend2/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_outdated_amend2/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_outdated_amend2/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1413 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_outdated_amend2/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      331 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_outdated_amend2/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_outdated_amend2/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.620907 stepup-1.2.4/tests/cases/watch_output/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_output/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_output/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_output/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_output/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_output/input.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1073 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_output/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_output/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_output/second.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:40.620907 stepup-1.2.4/tests/cases/watch_wanted/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_wanted/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_wanted/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_wanted/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_wanted/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_wanted/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_wanted/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1691 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_wanted/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      328 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_wanted/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/cases/watch_wanted/plan_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/core_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/echo_server_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/echo_server_stdio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/test_assoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/test_cascade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23443 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/test_nglob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/test_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65425 2024-05-27 07:21:33.000000 stepup-1.2.4/tests/test_workflow.py
```

### Comparing `stepup-1.2.3/.github/workflows/release.yaml` & `stepup-1.2.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/.pre-commit-config.yaml` & `stepup-1.2.4/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -21,16 +21,16 @@
       args: ["--autofix", "--no-sort-keys"]
     - id: trailing-whitespace
 - repo: https://github.com/Lucas-C/pre-commit-hooks
   rev: v1.5.5
   hooks:
     - id: remove-crlf
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.4.3
+  rev: v0.4.5
   hooks:
     - id: ruff-format
     - id: ruff
       args: ["--fix", "--show-fixes"]
 - repo: https://github.com/python-jsonschema/check-jsonschema
-  rev: 0.28.2
+  rev: 0.28.4
   hooks:
     - id: check-github-workflows
```

### Comparing `stepup-1.2.3/LICENSE` & `stepup-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/PKG-INFO` & `stepup-1.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepup
-Version: 1.2.3
+Version: 1.2.4
 Summary: StepUp Core provides the basic framework for the StepUp build tool
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-core/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-core/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-core/
 Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-core/changelog/
 Classifier: Environment :: Console
```

### Comparing `stepup-1.2.3/README.md` & `stepup-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/amending_static_inputs/stdout.txt` & `stepup-1.2.4/docs/advanced_topics/amending_static_inputs/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/amending_static_inputs.md` & `stepup-1.2.4/docs/advanced_topics/amending_static_inputs.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/amending_steps/stdout.txt` & `stepup-1.2.4/docs/advanced_topics/amending_steps/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/amending_steps.md` & `stepup-1.2.4/docs/advanced_topics/amending_steps.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/blocked_steps/stdout.txt` & `stepup-1.2.4/docs/advanced_topics/blocked_steps/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/blocked_steps.md` & `stepup-1.2.4/docs/advanced_topics/blocked_steps.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/cyclic_dependencies/stdout.txt` & `stepup-1.2.4/docs/advanced_topics/cyclic_dependencies/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/cyclic_dependencies.md` & `stepup-1.2.4/docs/advanced_topics/cyclic_dependencies.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/environment_variables/stdout.txt` & `stepup-1.2.4/docs/advanced_topics/environment_variables/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/environment_variables.md` & `stepup-1.2.4/docs/advanced_topics/environment_variables.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/here_and_root/stdout.txt` & `stepup-1.2.4/docs/advanced_topics/here_and_root/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/here_and_root.md` & `stepup-1.2.4/docs/advanced_topics/here_and_root.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/manual_cleaning.md` & `stepup-1.2.4/docs/advanced_topics/manual_cleaning.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/optional_steps/plot_logmap.png` & `stepup-1.2.4/docs/advanced_topics/optional_steps/plot_logmap.png`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/optional_steps/stdout.txt` & `stepup-1.2.4/docs/advanced_topics/optional_steps/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/optional_steps.md` & `stepup-1.2.4/docs/advanced_topics/optional_steps.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/pools/stdout.txt` & `stepup-1.2.4/docs/advanced_topics/pools/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/pools.md` & `stepup-1.2.4/docs/advanced_topics/pools.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/static_deferred_glob/graph.txt` & `stepup-1.2.4/docs/advanced_topics/static_deferred_glob/graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/static_deferred_glob/graph_creator.svg` & `stepup-1.2.4/docs/advanced_topics/static_deferred_glob/graph_creator.svg`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/static_deferred_glob/graph_supplier.svg` & `stepup-1.2.4/docs/advanced_topics/static_deferred_glob/graph_supplier.svg`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/static_deferred_glob/stdout.txt` & `stepup-1.2.4/docs/advanced_topics/static_deferred_glob/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/static_deferred_glob.md` & `stepup-1.2.4/docs/advanced_topics/static_deferred_glob.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/static_named_glob/plan.py` & `stepup-1.2.4/docs/advanced_topics/static_named_glob/plan.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/static_named_glob/stdout.txt` & `stepup-1.2.4/docs/advanced_topics/static_named_glob/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/static_named_glob.md` & `stepup-1.2.4/docs/advanced_topics/static_named_glob.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/stepup_root.md` & `stepup-1.2.4/docs/advanced_topics/stepup_root.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/variable_substitution.md` & `stepup-1.2.4/docs/advanced_topics/variable_substitution.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/advanced_topics/volatile_outputs.md` & `stepup-1.2.4/docs/advanced_topics/volatile_outputs.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/changelog.md` & `stepup-1.2.4/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,27 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.2.4] - 2024-05-27
+
+### Changed
+
+- Include "hidden" files when globbing.
+
+### Fixed
+
+- Do not refuse to replay unchanged step that declares its own static inputs.
+- Make recursive glob consistent with Python's built-in glob in `step.core.nglob`.
+- Pool definitions are stored in workflow and replayed correctly when a step is skipped.
+
+
 ## [1.2.3] - 2024-05-19
 
 ### Changed
 
 - Completed and revised docstrings in `stepup.core.nglob`,
   and added this module to the reference documentation.
```

### Comparing `stepup-1.2.3/docs/development.md` & `stepup-1.2.4/docs/development.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/automatic_cleaning.md` & `stepup-1.2.4/docs/getting_started/automatic_cleaning.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/copy_mkdir/stdout.txt` & `stepup-1.2.4/docs/getting_started/copy_mkdir/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/copy_mkdir.md` & `stepup-1.2.4/docs/getting_started/copy_mkdir.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/dependencies/graph_creator.svg` & `stepup-1.2.4/docs/getting_started/dependencies/graph_creator.svg`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/dependencies/graph_supplier.svg` & `stepup-1.2.4/docs/getting_started/dependencies/graph_supplier.svg`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/dependencies/stdout.txt` & `stepup-1.2.4/docs/getting_started/dependencies/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/dependencies.md` & `stepup-1.2.4/docs/getting_started/dependencies.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/distributed_plans/stdout.txt` & `stepup-1.2.4/docs/getting_started/distributed_plans/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/distributed_plans.md` & `stepup-1.2.4/docs/getting_started/distributed_plans.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/first_step/stdout1.txt` & `stepup-1.2.4/docs/getting_started/first_step/stdout1.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/first_step.md` & `stepup-1.2.4/docs/getting_started/first_step.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/interactive_usage.md` & `stepup-1.2.4/docs/getting_started/interactive_usage.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/introduction.md` & `stepup-1.2.4/docs/getting_started/introduction.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/no_rules/stdout.txt` & `stepup-1.2.4/docs/getting_started/no_rules/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/no_rules.md` & `stepup-1.2.4/docs/getting_started/no_rules.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/processes.svg` & `stepup-1.2.4/docs/getting_started/processes.svg`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/script_multiple/ebbr.csv` & `stepup-1.2.4/docs/getting_started/script_multiple/ebbr.csv`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/script_multiple/ebos.csv` & `stepup-1.2.4/docs/getting_started/script_multiple/ebos.csv`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/script_multiple/plot.py` & `stepup-1.2.4/docs/getting_started/script_multiple/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-import matplotlib
+import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.dates import DateFormatter
 
 from stepup.core.script import driver
 
 
@@ -20,15 +20,15 @@
         "inp": ["matplotlibrc", f"{airport}.csv"],
         "out": f"plot_{airport}.png",
         "airport": airport,
     }
 
 
 def run(inp, out, airport):
-    matplotlib.rc_file(inp[0])
+    mpl.rc_file(inp[0])
     dtype = [("dt", "datetime64[s]"), ("tmpc", "f8")]
     data = np.loadtxt(inp[1], dtype=dtype, delimiter=",", skiprows=1).T
     fig, ax = plt.subplots()
     ax.plot(data["dt"], data["tmpc"])
     ax.xaxis.set_major_formatter(DateFormatter("%d"))
     ax.set_xlabel("Day of the month February 2024")
     ax.set_xlim(data["dt"][0], data["dt"][-1])
```

### Comparing `stepup-1.2.3/docs/getting_started/script_multiple/plot_ebbr.png` & `stepup-1.2.4/docs/getting_started/script_multiple/plot_ebbr.png`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/script_multiple/plot_ebos.png` & `stepup-1.2.4/docs/getting_started/script_multiple/plot_ebos.png`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/script_multiple/stdout.txt` & `stepup-1.2.4/docs/getting_started/script_multiple/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/script_multiple.md` & `stepup-1.2.4/docs/getting_started/script_multiple.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/script_single.md` & `stepup-1.2.4/docs/getting_started/script_single.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/static_files.md` & `stepup-1.2.4/docs/getting_started/static_files.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/static_glob/stdout.txt` & `stepup-1.2.4/docs/getting_started/static_glob/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/static_glob.md` & `stepup-1.2.4/docs/getting_started/static_glob.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/static_glob_conditional/stdout1.txt` & `stepup-1.2.4/docs/getting_started/static_glob_conditional/stdout1.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/getting_started/static_glob_conditional.md` & `stepup-1.2.4/docs/getting_started/static_glob_conditional.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/index.md` & `stepup-1.2.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/installation.md` & `stepup-1.2.4/docs/installation.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/license.md` & `stepup-1.2.4/docs/license.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/plan.py` & `stepup-1.2.4/docs/plan.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/reference/interactive.md` & `stepup-1.2.4/docs/reference/interactive.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/reference/stepup.core.api.md` & `stepup-1.2.4/docs/reference/stepup.core.api.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/docs/run_example.py` & `stepup-1.2.4/docs/run_example.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/mkdocs.yml` & `stepup-1.2.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/pyproject.toml` & `stepup-1.2.4/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -51,25 +51,40 @@
 [project.scripts]
 stepup = "stepup.core.tui:main"
 cleanup = "stepup.core.cleanup:main"
 
 [tool.pytest.ini_options]
 addopts = "-n auto"
 
-[tool.black]
-line-length = 100
-target-version = ['py311']
-
 [tool.ruff]
 line-length = 100
 target-version = "py311"
 
 [tool.ruff.lint]
-select = ["E", "F", "UP", "B", "SIM", "I", "PGH", "PL", "RUF", "C"]
-ignore = ["PLR0911", "PLR0912", "PLR0913", "PLR0915", "PLR2004", "PLW2901", "C901"]
+select = [
+    "A", "B", "BLE", "C4", "E", "EXE", "F", "I", "ICN", "ISC", "N", "NPY", "PERF", "PIE", "PL",
+    "PT", "PYI", "RET", "RSE", "RUF", "SIM", "TRY", "UP", "W"
+]
+ignore = [
+    "PLR0904",  # https://docs.astral.sh/ruff/rules/too-many-public-methods/
+    "PLR0911",  # https://docs.astral.sh/ruff/rules/too-many-return-statements/
+    "PLR0912",  # https://docs.astral.sh/ruff/rules/too-many-branches/
+    "PLR0913",  # https://docs.astral.sh/ruff/rules/too-many-arguments/
+    "PLR0914",  # https://docs.astral.sh/ruff/rules/too-many-locals/
+    "PLR0915",  # https://docs.astral.sh/ruff/rules/too-many-statements/
+    "PLR0916",  # https://docs.astral.sh/ruff/rules/too-many-boolean-expressions/
+    "PLR0917",  # https://docs.astral.sh/ruff/rules/too-many-positional/
+    "PLR2004",  # https://docs.astral.sh/ruff/rules/magic-value-comparison/
+    "PLW2901",  # https://docs.astral.sh/ruff/rules/redefined-loop-name/
+    "PT011",  # https://docs.astral.sh/ruff/rules/pytest-raises-too-broad/
+    "RET503",  # https://docs.astral.sh/ruff/rules/implicit-return/
+    "TRY003",  # https://docs.astral.sh/ruff/rules/raise-vanilla-args/
+    "TRY300",  # https://docs.astral.sh/ruff/rules/try-consider-else/
+    "TRY301",  # https://docs.astral.sh/ruff/rules/raise-within-try/
+]
 
 [tool.setuptools]
 packages = ["stepup"]
 
 [tool.setuptools_scm]
 write_to = "stepup/core/_version.py"
 version_scheme = "post-release"
```

### Comparing `stepup-1.2.3/stepup/core/__init__.py` & `stepup-1.2.4/stepup/core/__init__.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/stepup/core/api.py` & `stepup-1.2.4/stepup/core/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,34 +177,35 @@
     if _defer:
         if _required:
             raise ValueError("Combination of options not supported: _defer=True, _required=True")
         if len(subs) > 0:
             raise ValueError("Named wildcards are not supported in deferred globs.")
         tr_patterns = [translate(su_pattern) for su_pattern in su_patterns]
         RPC_CLIENT.call.defer(_get_step_key(), tr_patterns)
-    else:
-        # Collect all matches
-        nglob_multi = NGlobMulti.from_patterns(su_patterns, subs)
-        nglob_multi.glob()
-        if _required and len(nglob_multi.results) == 0:
-            raise FileNotFoundError("Could not find any matching paths on the filesystem.")
-
-        # Send static paths
-        static_paths = nglob_multi.files()
-        if len(static_paths) > 0:
-            check_inp_paths(static_paths)
-            tr_static_paths = [translate(static_path) for static_path in static_paths]
-            RPC_CLIENT.call.static(_get_step_key(), tr_static_paths)
-
-        # Unstructure the nglob_multi and translate all paths before sending it to the director.
-        lookup = lookupdict()
-        ngm_data = nglob_multi.unstructure(lookup)
-        tr_strings = [str(translate(path)) for path in lookup.get_list()]
-        RPC_CLIENT.call.nglob(_get_step_key(), ngm_data, tr_strings)
-        return nglob_multi
+        return None
+
+    # Collect all matches
+    nglob_multi = NGlobMulti.from_patterns(su_patterns, subs)
+    nglob_multi.glob()
+    if _required and len(nglob_multi.results) == 0:
+        raise FileNotFoundError("Could not find any matching paths on the filesystem.")
+
+    # Send static paths
+    static_paths = nglob_multi.files()
+    if len(static_paths) > 0:
+        check_inp_paths(static_paths)
+        tr_static_paths = [translate(static_path) for static_path in static_paths]
+        RPC_CLIENT.call.static(_get_step_key(), tr_static_paths)
+
+    # Unstructure the nglob_multi and translate all paths before sending it to the director.
+    lookup = lookupdict()
+    ngm_data = nglob_multi.unstructure(lookup)
+    tr_strings = [str(translate(path)) for path in lookup.get_list()]
+    RPC_CLIENT.call.nglob(_get_step_key(), ngm_data, tr_strings)
+    return nglob_multi
 
 
 def _str_to_list(arg: Collection[str] | str) -> list[str]:
     return [arg] if isinstance(arg, str) else list(arg)
 
 
 def step(
@@ -279,16 +280,15 @@
         workdir = translate(subs(workdir))
     amend(env=sorted(amended_env_vars))
     command = CaseSensitiveTemplate(command).safe_substitute(
         inp=" ".join(myrelpath(inp_path, workdir) for inp_path in inp_paths),
         out=" ".join(myrelpath(out_path, workdir) for out_path in out_paths),
         vol=" ".join(myrelpath(vol_path, workdir) for vol_path in vol_paths),
     )
-    return RPC_CLIENT(
-        "step",
+    return RPC_CLIENT.call.step(
         _get_step_key(),
         command,
         inp_paths,
         env_vars,
         out_paths,
         vol_paths,
         workdir,
@@ -304,15 +304,15 @@
     Parameters
     ----------
     name
         The name of the pool.
     size
         The pool size.
     """
-    RPC_CLIENT.call.pool(name, size)
+    RPC_CLIENT.call.pool(_get_step_key(), name, size)
 
 
 def amend(
     *,
     inp: Collection[str] | str = (),
     env: Collection[str] | str = (),
     out: Collection[str] | str = (),
@@ -356,16 +356,15 @@
         return True
     env_vars = set(env_vars)
     with subs_env_vars() as subs:
         su_inp_paths = [subs(inp_path) for inp_path in inp_paths]
         tr_inp_paths = [translate(inp_path) for inp_path in su_inp_paths]
         tr_out_paths = [translate(subs(out_path)) for out_path in out_paths]
         tr_vol_paths = [translate(subs(vol_path)) for vol_path in vol_paths]
-    keep_going = RPC_CLIENT(
-        "amend",
+    keep_going = RPC_CLIENT.call.amend(
         _get_step_key(),
         tr_inp_paths,
         sorted(env_vars),
         tr_out_paths,
         tr_vol_paths,
     )
     if keep_going:
@@ -608,10 +607,9 @@
 
 def _get_step_key():
     """Get the current step key from the STEPUP_STEP_KEY environment variable."""
     stepup_step_key = os.getenv("STEPUP_STEP_KEY")
     if stepup_step_key is None:
         if isinstance(RPC_CLIENT, DummySyncRPCClient):
             return "dummy:"
-        else:
-            raise RuntimeError("The STEPUP_STEP_KEY environment variable is not defined.")
+        raise RuntimeError("The STEPUP_STEP_KEY environment variable is not defined.")
     return stepup_step_key
```

### Comparing `stepup-1.2.3/stepup/core/assoc.py` & `stepup-1.2.4/stepup/core/assoc.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/stepup/core/asyncio.py` & `stepup-1.2.4/stepup/core/asyncio.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/stepup/core/cascade.py` & `stepup-1.2.4/stepup/core/cascade.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 @attrs.define
 class Node:
     """Parent class of node-specific information and actions."""
 
     _key: str = attrs.field(init=False, default="todo:")
 
     @classproperty
-    def kind(cls):
+    def kind(cls):  # noqa: N805
         return cls.__name__.lower()
 
     @classmethod
     def key_tail(cls, data: dict[str, Any], lookup: list[str] | None = None) -> str:
         """Subclasses must implement the key tail and accept both JSON or attrs dicts."""
         raise NotImplementedError
 
@@ -73,23 +73,20 @@
         raise NotImplementedError
 
     def format_properties(self, cascade: "Cascade") -> Iterator[tuple[str, str]]:
         raise NotImplementedError
 
     def recycle(self, cascade: "Cascade", old: Self | None):
         """Copy useful information from older orphaned version of the node, if any."""
-        pass
 
     def orphan(self, cascade: "Cascade"):
         """This method is called when the creator of a node is set to Creator.vacuum."""
-        pass
 
     def cleanup(self, cascade: "Cascade"):
         """Perform a cleanup right before the orphaned node is removed from the graph."""
-        pass
 
 
 @attrs.define
 class Root(Node):
     """The top-level creator in the cascade."""
 
     _version: str = attrs.field()
@@ -283,21 +280,27 @@
             else:
                 lines.append(key)
             for name, value in node.format_properties(self):
                 lines.append(f"{name:>20s} = {value!s}")
             pairs = []
             if not (creator_key == "vacuum:" or key == "root:"):
                 pairs.append(("created by", creator_key))
-            for other_key in self.get_suppliers(key, include_orphans=True):
-                pairs.append(("consumes", other_key))
-            for other_key in self.get_products(key, include_orphans=True):
-                if other_key != "root:":
-                    pairs.append(("creates", other_key))
-            for other_key in self.get_consumers(key, include_orphans=True):
-                pairs.append(("supplies", other_key))
+            pairs.extend(
+                ("consumes", other_key)
+                for other_key in self.get_suppliers(key, include_orphans=True)
+            )
+            pairs.extend(
+                ("creates", other_key)
+                for other_key in self.get_products(key, include_orphans=True)
+                if other_key != "root:"
+            )
+            pairs.extend(
+                ("supplies", other_key)
+                for other_key in self.get_consumers(key, include_orphans=True)
+            )
             for role, other_key in pairs:
                 if other_key == "vacuum:":
                     continue
                 if self.get_creator(other_key) == "vacuum:":
                     lines.append(f"{role:>20s}   ({other_key})")
                 else:
                     lines.append(f"{role:>20s}   {other_key}")
@@ -397,16 +400,15 @@
         - This method is rather slow and only called when there is a known problem.
           It is helpful because it provides more useful (and expensive) feedback.
         - This method only consider supplier-consumer edges.
         """
         lines = []
         for cycle in self._iter_cycles(src_key, dst_key):
             lines.append("cycle:")
-            for key in cycle:
-                lines.append(f"  {key}")
+            lines.extend(f"  {key}" for key in cycle)
             lines.append("")
         if len(lines) > 0:
             lines[:0] = [
                 "New relation introduces cyclic dependency",
                 "",
                 f"src = {src_key}",
                 f"dst = {dst_key}",
@@ -465,21 +467,14 @@
         self.nodes[node.key] = node
         self.kinds.add(kind, node.key)
         node.recycle(self, old)
         # Add creator relation, if creator is known
         _check_key(creator_key, self.node_classes)
         if creator_key not in self.nodes:
             raise ValueError(f"Non-existing creator: {creator_key}")
-        try:
-            self.check_cyclic(creator_key, node.key)
-        except Exception:
-            # Instead of creating the cycle, the node is created as an orphan,
-            # to make sure the graph remains meaningful. All nodes must have a creator.
-            self.products.add("vacuum:", node.key)
-            raise
         self.products.add(creator_key, node.key)
         return node.key
 
     def supply(self, supplier_key, consumer_key):
         """Create a supplier-consumer relation."""
         _check_key(supplier_key, self.node_classes)
         _check_key(consumer_key, self.node_classes)
```

### Comparing `stepup-1.2.3/stepup/core/cleanup.py` & `stepup-1.2.4/stepup/core/cleanup.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/stepup/core/deferred_glob.py` & `stepup-1.2.4/stepup/core/deferred_glob.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     _ngm: NGlobMulti = attrs.field()
 
     #
     # Getters
     #
 
     @classproperty
-    def kind(cls):
+    def kind(cls):  # noqa: N805
         return "dg"
 
     @property
     def ngm(self) -> NGlobMulti:
         return self._ngm
 
     #
```

### Comparing `stepup-1.2.3/stepup/core/director.py` & `stepup-1.2.4/stepup/core/director.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,16 +134,15 @@
     return parser.parse_args()
 
 
 def interpret_num_workers(num_workers: Decimal) -> int:
     """Convert the command-line argument num-workers into an integer."""
     if num_workers.as_tuple().exponent < 0:
         return int(len(os.sched_getaffinity(0)) * num_workers)
-    else:
-        return int(num_workers)
+    return int(num_workers)
 
 
 WORKFLOW_OH_NO = """
 This is most likely a bug.
 Please open an issue at https://github.com/reproducible-reporting/stepup-core/issues
 Copy paste the traceback below and explain how to reproduce the problem.
 The broken workflow file was copied to {}.
@@ -191,15 +190,15 @@
     workflow = None
     if path_workflow.exists():
         try:
             workflow = Workflow.from_file(path_workflow)
             workflow.check_consistency()
             workflow.dissolve(not explain_rerun)
             await reporter("WORKFLOW", f"Loaded from {path_workflow}")
-        except Exception as exc:
+        except Exception as exc:  # noqa: BLE001
             traceback_fmt = "".join(traceback.format_exception(type(exc), exc, exc.__traceback__))
             path_workflow_bug = path_workflow.parent / "workflow-bug.mpk"
             shutil.copy(path_workflow, path_workflow_bug)
             message = WORKFLOW_OH_NO.format(path_workflow_bug)
             if workflow is not None:
                 path_graph_bug = path_workflow.parent / "graph-bug.txt"
                 with open(path_graph_bug, "w") as fh:
@@ -323,21 +322,17 @@
         pool: str | None,
         block: bool,
     ) -> str:
         """Create a step in the workflow.
 
         Notes
         -----
-        This is an RPC wrapper for `Workflow.define_step` with a few additional sanity checks:
-        - The pool must exist.
+        This is an RPC wrapper for `Workflow.define_step` with an additional sanity check:
         - The working directory must exist.
         """
-        # If the pool is unknown, raise an error
-        if not self._scheduler.has_pool(pool):
-            raise GraphError(f"Unknown pool name: {pool}")
         if not workdir.endswith(os.sep):
             raise GraphError(f"A working directory must end with a separator, got: {workdir}")
         with self._dissolve_if_graph_changed():
             return self._workflow.define_step(
                 creator_key,
                 command,
                 inp_paths,
@@ -347,22 +342,22 @@
                 workdir,
                 optional,
                 pool,
                 block,
             )
 
     @allow_rpc
-    def pool(self, name: str, size: int):
+    def pool(self, step_key: str, name: str, size: int):
         """Define a pool with given name and size.
 
         Notes
         -----
         This is an RPC wrapper for `Scheduler.set_pool`.
         """
-        self._scheduler.set_pool(name, size)
+        self._workflow.set_pool(step_key, name, size)
 
     @allow_rpc
     def amend(
         self,
         step_key: str,
         inp_paths: list[str],
         env_vars: set[str],
@@ -536,19 +531,18 @@
         if os.path.isfile(path_director_log):
             with open(path_director_log) as fh:
                 line = fh.readline()
                 if line.startswith("SOCKET"):
                     path_socket = Path(line[6:].strip())
                     if len(path_socket) > 2 and path_socket.exists():
                         return path_socket
-                    else:
-                        message = (
-                            f"Socket {path_socket} read from {path_director_log} does not exist. "
-                            "Stepup not running?"
-                        )
+                    message = (
+                        f"Socket {path_socket} read from {path_director_log} does not exist. "
+                        "Stepup not running?"
+                    )
                 else:
                     message = f"File {path_director_log} does not start with SOCKET line."
         else:
             message = f"File {path_director_log} not found."
         if secs == 0.0:
             print("Trying to contact StepUp director process.", file=sys.stderr)
         secs += 0.1
```

### Comparing `stepup-1.2.3/stepup/core/exceptions.py` & `stepup-1.2.4/stepup/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/stepup/core/file.py` & `stepup-1.2.4/stepup/core/file.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/stepup/core/hash.py` & `stepup-1.2.4/stepup/core/hash.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,24 +200,23 @@
     _digest: bytes = attrs.field()
     _inp_digest: bytes = attrs.field()
 
     @classmethod
     def structure(cls, state, strings: list[str]):
         if len(state) == 2:
             return StepHash(*state)
-        elif len(state) == 5:
+        if len(state) == 5:
             return ExtendedStepHash(
                 state[0],
                 state[1],
                 {strings[path]: FileHash.structure(data) for path, data in state[2]},
                 state[3],
                 {strings[path]: FileHash.structure(data) for path, data in state[4]},
             )
-        else:
-            TypeError(f"Cannot structure as StepHash: {state}")
+        TypeError(f"Cannot structure as StepHash: {state}")
 
     def unstructure(self, lookup: dict[str, int]) -> list:
         return [self.digest, self.inp_digest]
 
     @property
     def digest(self) -> bytes:
         return self._digest
@@ -261,16 +260,15 @@
     inp_hashes: list[tuple[str, FileHash]],
     env_var_values: list[tuple[str, str | None]],
     out_hashes: list[tuple[str, FileHash]],
 ):
     args = _compute_step_digest(step_key, inp_hashes, env_var_values, out_hashes)
     if extended:
         return ExtendedStepHash(*args)
-    else:
-        return StepHash(*args[:2])
+    return StepHash(*args[:2])
 
 
 def compare_step_hashes(old_hash: StepHash, new_hash: StepHash) -> tuple[str, str]:
     chl = []
     sml = []
     _compare_step_digests(chl, sml, old_hash, new_hash)
     if isinstance(old_hash, ExtendedStepHash) and isinstance(new_hash, ExtendedStepHash):
@@ -363,16 +361,15 @@
         changes.append(f"digest {_fmt_digest(old_hash.digest)} ➜ {_fmt_digest(new_hash.digest)}")
     if old_hash.size != new_hash.size:
         changes.append(f"size {old_hash.size} ➜ {new_hash.size}")
     if old_hash.mode != new_hash.mode:
         changes.append(f"mode {stat.filemode(old_hash.mode)} ➜ {stat.filemode(new_hash.mode)}")
     if len(changes) > 0:
         return True, (f"Modified {label} hash", f"{path} ({', '.join(changes)})")
-    else:
-        return False, (f"Same {label} hash", path)
+    return False, (f"Same {label} hash", path)
 
 
 def _fmt_digest(digest: bytes) -> str:
     if len(digest) == 1:
         if digest == b"u":
             return "UNKNOWN"
         if digest == b"d":
```

### Comparing `stepup-1.2.3/stepup/core/job.py` & `stepup-1.2.4/stepup/core/job.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 if TYPE_CHECKING:
     from .scheduler import Scheduler
     from .worker import WorkerClient
     from .workflow import Workflow
 
 
-__all__ = ("Job", "ValidateAmendedJob", "TryReplayJob", "RunJob")
+__all__ = ("Job", "SetPoolJob", "ValidateAmendedJob", "TryReplayJob", "RunJob")
 
 
 @attrs.define
 class Job:
     @property
     def pool(self) -> str | None:
         raise NotImplementedError
@@ -47,15 +47,34 @@
         raise NotImplementedError
 
     def finalize(self, result, scheduler: "Scheduler", workflow: "Workflow"):
         raise NotImplementedError
 
 
 @attrs.define
+class SetPoolJob(Job):
+    """This is a stub: the scheduler uses it to set the pool, never executes on the worker."""
+
+    _pool: str = attrs.field()
+    _size: int = attrs.field()
+
+    @property
+    def pool(self) -> str | None:
+        # Setting a pool never requires a pool.
+        return None
+
+    @property
+    def set_pool_args(self) -> tuple[str, int]:
+        return (self._pool, self._size)
+
+
+@attrs.define
 class ValidateAmendedJob(Job):
+    """Validate that amended inputs have not changed yet, or schedule for rerun."""
+
     _step_key: str = attrs.field()
     _pool: str | None = attrs.field()
 
     @property
     def pool(self) -> str | None:
         # A validation of amended inputs never has pool restrictions.
         # The pool attribute is only used to schedule a real run in the correct
@@ -74,14 +93,16 @@
             run_job = RunJob(self._step_key, self._pool)
             scheduler.inqueue.put_nowait(run_job)
             scheduler.changed.set()
 
 
 @attrs.define
 class TryReplayJob(Job):
+    """Simulate the execution of a job, if inputs and outputs have not changed."""
+
     _step_key: str = attrs.field()
     _pool: str | None = attrs.field()
 
     @property
     def pool(self) -> str | None:
         # A replay never has pool restrictions.
         # The pool attribute is only used to schedule a real run in the correct
@@ -100,14 +121,16 @@
             run_job = RunJob(self._step_key, self._pool)
             scheduler.inqueue.put_nowait(run_job)
             scheduler.changed.set()
 
 
 @attrs.define
 class RunJob(Job):
+    """Actually execute a job."""
+
     _step_key: str = attrs.field()
     _pool: str | None = attrs.field()
 
     @property
     def pool(self) -> str | None:
         return self._pool
```

### Comparing `stepup-1.2.3/stepup/core/nglob.py` & `stepup-1.2.4/stepup/core/nglob.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,26 @@
 import re
 from collections.abc import Collection, Iterable, Iterator
 from typing import Any, Self
 
 import attrs
 from path import Path
 
-RE_NAMED_WILD = re.compile(r"(\[.*?]|\$\{\*[a-zA-Z0-9_]*?}|[*]{1,2}|[?])")
+RE_WILD_PARTS = [
+    r"^[*][*]$",  # recursive ** wildcard, full string
+    r"^[*][*](?=/)",  # recursive ** wildcard, leading
+    r"(?<=/)[*][*]$",  # recursive ** wildcard, trailing
+    r"(?<=/)[*][*](?=/)",  # recursive ** wildcard, middle
+    r"\[.*?]",  # anonymous [abc] wildcard
+    r"[*]",  # anonymous * wildcard
+    r"[?]",  # anonymous ? wildcard
+    r"\$\{\*[a-zA-Z0-9_]*?}",  # named wildcard
+]
+
+RE_NAMED_WILD = re.compile("(" + "|".join(RE_WILD_PARTS) + ")")
 
 
 __all__ = (
     "NGlobMatch",
     "NGlobSingle",
     "NGlobMulti",
     "convert_nglob_to_regex",
@@ -284,15 +295,21 @@
 
         Yields
         ------
         values
             A tuple with substring matching the named wildcards,
             only this combination of names was not present yet.
         """
-        yield from self.extend(glob.glob(self._glob_pattern, recursive=True))
+        paths = []
+        for path in glob.iglob(self._glob_pattern, recursive=True, include_hidden=True):
+            path = Path(path)
+            if path.is_dir():
+                path = path / ""
+            paths.append(path)
+        yield from self.extend(paths)
 
 
 def has_wildcards(pattern: str) -> bool:
     """Test if a glob pattern has anonymous or named wildcards."""
     return RE_NAMED_WILD.search(pattern) is not None
 
 
@@ -321,21 +338,20 @@
     _has_wildcards: bool = attrs.field(init=False)
     _results: dict[tuple[str, ...], list[set[Path]]] = attrs.field(init=False, factory=dict)
 
     @_subs.default
     def _default_subs(self):
         if len(self._nglob_singles) == 0:
             return {}
-        else:
-            subs = self._nglob_singles[0].subs
-            for other in self._nglob_singles[1:]:
-                if other.subs != subs:
-                    raise ValueError("Searches in one NGlobMulti must use the same substitutions")
-                other._subs = subs
-            return subs
+        subs = self._nglob_singles[0].subs
+        for other in self._nglob_singles[1:]:
+            if other.subs != subs:
+                raise ValueError("Searches in one NGlobMulti must use the same substitutions")
+            other._subs = subs
+        return subs
 
     @_used_names.default
     def _default_used_names(self) -> tuple[str, ...]:
         result = set()
         for ngs in self._nglob_singles:
             result.update(ngs.used_names)
         return tuple(sorted(result))
@@ -594,16 +610,15 @@
         """True when there are some items in the `results` attribute."""
         return len(self.results) > 0
 
     def __iter__(self) -> Iterator[str | NGlobMatch]:
         """Iterates over `self.matches` if there are named wildcards, else over `self.files`."""
         if len(self._used_names) > 0:
             return self.matches()
-        else:
-            return iter(self.files())
+        return iter(self.files())
 
     def may_match(self, path):
         """Return True if the path matches one of the NGlobSingle instances.
 
         This means that it may be path contributing to a consistent match of NGlobMulti.
         When added, it will show up in the result of the `files` method,
         and it may affect the outcome of the `matches` method.
@@ -682,42 +697,61 @@
         It also contains symbolic groups to extract values
         corresponding to named wildcards
         and to impose consistency when the same name appears multiple times.
     """
     if subs is None:
         subs = {}
     parts = []
+    # Last non-empty part matched by re.split
+    last = None
+    # Names encountered so far
     encountered = set()
     for i, part in enumerate(RE_NAMED_WILD.split(pattern)):
         if i % 2 == 0:
-            # Not a wildcard: escape regex characters.
-            parts.append(re.escape(part))
+            if len(part) > 0:
+                # Not a wildcard: escape regex characters.
+                parts.append(re.escape(part))
         else:
             # A (named) wildcard: replace with corresponding regex.
+            replace = False
+            regex = None
             if part == "?":
-                regex = r"[^/]"
+                if last not in ["*", "**"]:
+                    regex = r"[^/]"
             elif part == "*":
-                regex = r"[^/]*"
+                if last not in ["*", "**"]:
+                    if last == "?":
+                        replace = True
+                    regex = r"[^/]*"
             elif part == "**":
-                regex = r".*"
+                if last != "**":
+                    regex = r".*"
+                    if last in ["*", "?"]:
+                        replace = True
             elif part.startswith("[") and part.endswith("]"):
                 regex = rf"[^{part[2:-1]}]" if part[1] == "!" else rf"[{part[1:-1]}]"
             elif part.startswith("${*") and part.endswith("}"):
                 if not allow_names:
                     raise ValueError(f"Named wildcards not allowed in {pattern}")
                 name = part[3:-1]
                 if name in encountered:
                     regex = rf"(?P={name})"
                 else:
                     part_regex = convert_nglob_to_regex(subs.get(name, "*"), {}, False)
                     regex = rf"(?P<{name}>{part_regex})"
                     encountered.add(name)
             else:
                 raise ValueError(f"Cannot convert wildcard to regex: {part}")
-            parts.append(regex)
+            if regex is not None:
+                if replace:
+                    parts[-1] = regex
+                else:
+                    parts.append(regex)
+        if len(part) > 0:
+            last = part
     return "".join(parts)
 
 
 def convert_nglob_to_glob(pattern: str, subs: dict[str, str] | None = None) -> str:
     """Convert nglob wildcards to ordinary ones, compatible with builtin glob and fnmatch modules.
 
     Parameters
```

### Comparing `stepup-1.2.3/stepup/core/pytest.py` & `stepup-1.2.4/stepup/core/pytest.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/stepup/core/reporter.py` & `stepup-1.2.4/stepup/core/reporter.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/stepup/core/rpc.py` & `stepup-1.2.4/stepup/core/rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,17 +97,18 @@
     try:
         call_id = int.from_bytes(await reader.readexactly(8))
         size = int.from_bytes(await reader.readexactly(8))
         if size == 0:
             body = None
         else:
             body = await reader.readexactly(size)
-        return call_id, body
     except asyncio.IncompleteReadError:
         return None, None
+    else:
+        return call_id, body
 
 
 async def _send_rpc_message(writer: asyncio.StreamWriter, call_id: int, message: bytes | None):
     writer.write(call_id.to_bytes(8))
     if message is None:
         writer.write((0).to_bytes(8))
     else:
@@ -159,20 +160,19 @@
     """Receive requests from RPC clients and create corresponding tasks."""
     tasks = set()
     si = stoppable_iterator(_recv_rpc_message, stop_event, (reader,))
     async for call_id, request in si:
         if call_id is None or request is None:
             stop_event.set()
             break
-        else:
-            name, args, kwargs = pickle.loads(request)
-            task_name = f"RPC:{name}-{call_id}"
-            task = asyncio.create_task(_handle_request(handler, name, args, kwargs), name=task_name)
-            tasks.add(task)
-            task.add_done_callback(partial(_queue_done, call_id, tasks, queue))
+        name, args, kwargs = pickle.loads(request)
+        task_name = f"RPC:{name}-{call_id}"
+        task = asyncio.create_task(_handle_request(handler, name, args, kwargs), name=task_name)
+        tasks.add(task)
+        task.add_done_callback(partial(_queue_done, call_id, tasks, queue))
 
 
 async def _handle_request(handler, name: str, args: list, kwargs: dict) -> tuple[Any, bool]:
     """Handle an RPC request from the client."""
     try:
         # print(fmt_rpc_call(name, args, kwargs))
         # Get the function, or raise RPCError
@@ -190,15 +190,15 @@
         except TypeError as exc:
             raise RPCError(f"Invalid arguments: {fmt_rpc_call(name, args, kwargs)}") from exc
         bound.apply_defaults()
         result = call(*bound.args, **bound.kwargs)
         if asyncio.iscoroutinefunction(call):
             result = await result
         return result, False
-    except Exception as exc:
+    except Exception as exc:  # noqa: BLE001
         message = "".join(traceback.format_exception(type(exc), exc, exc.__traceback__))
         return message, True
 
 
 def _queue_done(call_id: int, tasks: set[asyncio.Task], queue: asyncio.Queue, task: asyncio.Task):
     """Put replies of completed tasks on queue for send loop."""
     tasks.discard(task)
@@ -276,17 +276,16 @@
     _recv_data: dict[int, bytes] = attrs.field(init=False, factory=dict)
     _recv_stop: asyncio.Event = attrs.field(init=False, factory=asyncio.Event)
     _recv_task: asyncio.Task = attrs.field(init=False)
     _wait_on_close: list[Awaitable[Any]] = attrs.field(factory=list)
 
     @_recv_task.default
     def _default_recv_task(self):
-        task = asyncio.create_task(self._client_rpc_recv_loop(), name="client-rpc-recv-loop")
-        # Store reference to task to prevent garbage collection while client is alive.
-        return task
+        # Keep reference to task to prevent garbage collection while client is alive.
+        return asyncio.create_task(self._client_rpc_recv_loop(), name="client-rpc-recv-loop")
 
     async def _client_rpc_recv_loop(self):
         si = stoppable_iterator(_recv_rpc_message, self._recv_stop, (self.reader,))
         async for call_id, response in si:
             if call_id is None:
                 self._recv_stop.set()
                 break
@@ -459,16 +458,15 @@
     def _recv_rpc_message(self, expected_call_id: int) -> bytes:
         call_id = int.from_bytes(self._readexactly(8))
         if call_id != expected_call_id:
             raise ValueError(f"Expected call_id {expected_call_id}, got {call_id}")
         size = int.from_bytes(self._readexactly(8))
         if size == 0:
             raise ValueError("RPC clients should never receive a closing message.")
-        body = self._readexactly(size)
-        return body
+        return self._readexactly(size)
 
     def _readexactly(self, size: int) -> bytes:
         """Keep reading from the socket until (at least) size bytes were received.
 
         Parameters
         ----------
         size
@@ -485,15 +483,15 @@
             The bytes read from the socket of the requested size.
             Any additional data received from the socket is stored for the
             following call to `_readexactly`.
         """
         while len(self._partial_recv) < size:
             fragment = self._socket.recv(4096)
             if len(fragment) == 0:
-                raise ConnectionResetError()
+                raise ConnectionResetError
             self._partial_recv += fragment
         result = self._partial_recv[:size]
         self._partial_recv = self._partial_recv[size:]
         return result
 
 
 @attrs.define
```

### Comparing `stepup-1.2.3/stepup/core/runner.py` & `stepup-1.2.4/stepup/core/runner.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/stepup/core/scheduler.py` & `stepup-1.2.4/stepup/core/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 """The `Scheduler` plans the execution of jobs by the worker processes."""
 
 import asyncio
 import itertools
 
 import attrs
 
-from .job import Job
+from .job import Job, SetPoolJob
 
 __all__ = ("Pool", "Scheduler")
 
 
 @attrs.define
 class Pool:
     """A single pool of which the scheduler can contain several"""
@@ -109,15 +109,18 @@
         self.changed.set()
 
     def pop_runnable_job(self) -> tuple[Job | None, str | None]:
         """Return a runnable step and its pool (or None)."""
         if not self._onhold:
             while self.inqueue.qsize() > 0:
                 job = self.inqueue.get_nowait()
-                if job.pool is None:
+                if isinstance(job, SetPoolJob):
+                    # Shortcut that allows workflow to set a pool.
+                    self.set_pool(*job.set_pool_args)
+                elif job.pool is None:
                     self._main_pool.queue.put_nowait(job)
                 else:
                     self._pools[job.pool].queue.put_nowait(job)
         for pool_name, pool in self._pools.items():
             if self._main_pool.available and pool.available and pool.queue.qsize() > 0:
                 job = pool.queue.get_nowait()
                 self.acquire_pool(pool_name)
```

### Comparing `stepup-1.2.3/stepup/core/script.py` & `stepup-1.2.4/stepup/core/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,36 +92,34 @@
                 step(
                     f"./{script_path} run -- '{argstr}'",
                     inp=inp_paths,
                     out=out_paths,
                     optional=args.optional,
                 )
         return 0
-    elif args.cmd == "cases":
+    if args.cmd == "cases":
         if wrapper.has_single:
             print(f"./{script_path} run")
         if wrapper.has_cases:
             for case_args, case_kwargs in wrapper.generate_cases():
                 argstr = wrapper.format(*case_args, **case_kwargs)
                 print(f"./{script_path} run -- '{argstr}'")
         return 0
-    elif args.cmd == "run":
+    if args.cmd == "run":
         if args.string == "":
             if not wrapper.has_single:
                 raise RuntimeError(f"Script has no info function: {script_path}")
             info = wrapper.filter_info(wrapper.get_info())
             return wrapper.run(**info)
-        else:
-            if not wrapper.has_cases:
-                raise RuntimeError(f"Script has no case_info function: {script_path}")
-            case_args, case_kwargs = wrapper.parse(args.string)
-            info = wrapper.filter_info(wrapper.get_case_info(*case_args, **case_kwargs))
-            return wrapper.run(**info)
-    else:
-        raise NotImplementedError
+        if not wrapper.has_cases:
+            raise RuntimeError(f"Script has no case_info function: {script_path}")
+        case_args, case_kwargs = wrapper.parse(args.string)
+        info = wrapper.filter_info(wrapper.get_case_info(*case_args, **case_kwargs))
+        return wrapper.run(**info)
+    raise NotImplementedError
 
 
 def parse_args(script_path: str) -> argparse.Namespace:
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser(
         prog=script_path, description=f"StepUp driver for script {script_path}."
     )
```

### Comparing `stepup-1.2.3/stepup/core/step.py` & `stepup-1.2.4/stepup/core/step.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,41 +66,56 @@
     # Amended while running the step
     amend_args: dict = attrs.field(factory=dict)
     # Created while running the step
     static_paths: list[str] = attrs.field(factory=list)
     steps_args: list[dict] = attrs.field(factory=list)
     nglob_multis: list[NGlobMulti] = attrs.field(factory=list)
     deferred_glob_args: list[list[str]] = attrs.field(factory=list)
+    defined_pools: dict[str, int] = attrs.field(factory=dict)
 
 
 @attrs.define
 class Step(Node):
+    # - Core attributes
+    #   - Shell command to execute in this step
     _command: str = attrs.field()
+    #   - Work directory where the step command is executed
     _workdir: str = attrs.field()
+    #   - If set, concurrency is limited by the pool size (see scheduler module)
     _pool: str | None = attrs.field(kw_only=True, default=None)
-    # When True, the step will behave as it never has all dependencies satisfied.
-    # This is convenient for lowering the build time when working on intermediate steps.
+    #   - When True, the step will behave as it never has all dependencies satisfied.
+    #     This is convenient for lowering the build time when working on intermediate steps.
     _block: bool = attrs.field(kw_only=True, default=False)
 
-    # Augment information in Workflow instance
+    # - Augment information in Workflow instance
+    #   - From amend(inp=...)
     _amended_suppliers: set[str] = attrs.field(kw_only=True, factory=set)
+    #   - From amend(out=..., vol=...)
     _amended_consumers: set[str] = attrs.field(kw_only=True, factory=set)
 
-    # Extra information, not in Workflow instance
+    # - Extra information, not in Workflow instance
+    #   - env var names when step was defined
     _initial_env_vars: set[str] = attrs.field(kw_only=True, factory=set)
+    #   - env var names amended while executing
     _amended_env_vars: set[str] = attrs.field(kw_only=True, factory=set)
+    #   - named globs used while running step
     _nglob_multis: list[NGlobMulti] = attrs.field(kw_only=True, factory=list)
+    #   - pools defined by this step
+    _defined_pools: dict[str, int] = attrs.field(kw_only=True, factory=dict)
 
-    # List of missing amended files causing reschedule
+    # - Related to execution
+    #   - List of missing amended files causing reschedule
     reschedule_due_to: set[str] = attrs.field(init=False, factory=set)
-    # Flow to validate the amended inputs, e.g. because inputs may have changed.
+    #   - Flag to validate the amended inputs, e.g. because inputs may have changed.
     validate_amended: bool = attrs.field(init=False, default=True)
 
-    # Attributes for skipping steps whose inputs and outputs have not changed on disk.
+    # - Attributes for skipping steps whose inputs and outputs have not changed on disk.
+    #   - Digests of executed step (inputs, outputs, ...)
     _hash: StepHash | None = attrs.field(kw_only=True, default=None)
+    #   - All information needed to replay a job without executing it
     _recording: StepRecording | None = attrs.field(kw_only=True, default=None)
 
     #
     # Getters
     #
 
     @property
@@ -136,14 +151,18 @@
         return self._amended_env_vars
 
     @property
     def nglob_multis(self) -> list[NGlobMulti]:
         return self._nglob_multis
 
     @property
+    def defined_pools(self) -> dict[str, int]:
+        return self._defined_pools
+
+    @property
     def hash(self) -> StepHash:
         return self._hash
 
     @property
     def recording(self) -> StepRecording:
         return self._recording
 
@@ -188,14 +207,17 @@
         if ngm_datas is not None:
             kwargs["nglob_multis"] = [
                 NGlobMulti.structure(ngm_data, strings) for ngm_data in ngm_datas
             ]
         hash_ = data.get("h")
         if hash_ is not None:
             kwargs["hash"] = StepHash.structure(hash_, strings)
+        defined_pools = data.get("dp")
+        if defined_pools is not None:
+            kwargs["defined_pools"] = defined_pools
         step = cls(**kwargs)
         workflow.step_states[step.key] = state
         workflow.step_mandatory[step.key] = mandatory
         if ngm_datas is not None:
             workflow.step_keys_with_nglob.add(step.key)
         return step
 
@@ -218,14 +240,16 @@
             data["as"] = sorted(lookup[key] for key in self._amended_suppliers)
         if len(self._amended_consumers) > 0:
             data["ac"] = sorted(lookup[key] for key in self._amended_consumers)
         if len(self._amended_env_vars) > 0:
             data["ai"] = sorted(self._amended_env_vars)
         if len(self._nglob_multis) > 0:
             data["g"] = [nglob_multi.unstructure(lookup) for nglob_multi in self._nglob_multis]
+        if len(self.defined_pools) > 0:
+            data["dp"] = self.defined_pools.copy()
         if self._hash is not None:
             data["h"] = self._hash.unstructure(lookup)
         return data
 
     def format_properties(self, workflow: "Workflow") -> Iterator[tuple[str, str]]:
         yield "workdir", self._workdir
         yield "command", self._command
@@ -251,14 +275,16 @@
             label = ""
         label = "env_var (amended)"
         for env_var in sorted(self._amended_env_vars):
             yield label, env_var
             label = ""
         for ngm in self._nglob_multis:
             yield "ngm", f"{[ngs.pattern for ngs in ngm.nglob_singles]} {ngm.subs}"
+        for pool, size in sorted(self.defined_pools.items()):
+            yield "defined pool", f"{pool}={size}"
         if self._hash is not None:
             l1, l2 = format_digest(self._hash.digest)
             yield "digest", l1
             yield "", l2
             l1, l2 = format_digest(self._hash.inp_digest)
             yield "inp_digest", l1
             yield "", l2
@@ -463,18 +489,26 @@
             for file_key in self._amended_suppliers
         )
         if has_amended_pending and self.validate_amended:
             job = ValidateAmendedJob(self._key, self._pool)
         else:
             for file_key in workflow.get_suppliers(self.key, kind="file", include_orphans=True):
                 if workflow.is_orphan(file_key):
-                    return
-                state = workflow.get_file(file_key).get_state(workflow)
-                if state not in (FileState.BUILT, FileState.STATIC):
-                    return
+                    if self._recording is None:
+                        # If there is no recording that could undo
+                        # the orphaned state, the step cannot be queued
+                        return
+                    if file_key[5:] not in self._recording.static_paths:
+                        # If the orphaned file is not a recorded static
+                        # file, the step cannot be queued.
+                        return
+                else:
+                    state = workflow.get_file(file_key).get_state(workflow)
+                    if state not in (FileState.BUILT, FileState.STATIC):
+                        return
             if self._hash is None or self._recording is None:
                 job = RunJob(self._key, self._pool)
             else:
                 job = TryReplayJob(self._key, self._pool)
         self.set_state(workflow, StepState.QUEUED)
         self.reschedule_due_to = set()
         self.validate_amended = False
@@ -594,14 +628,15 @@
             recording.steps_args.append(step_args)
         for ngm in self.nglob_multis:
             recording.nglob_multis.append(ngm)
         for dg_key in workflow.get_products(self.key, "dg"):
             dg = workflow.get_deferred_glob(dg_key)
             patterns = [ngs.pattern for ngs in dg.ngm.nglob_singles]
             recording.deferred_glob_args.append(patterns)
+        recording.defined_pools = self._defined_pools.copy()
         self._recording = recording
 
     def replay_amend(self, workflow: "Workflow"):
         """Restore amended paths from a previous execution.
 
         This should be done as early as possible, to keep the rest of the workflow informed.
         """
@@ -642,14 +677,16 @@
             raise ValueError("The recorded key is not consistent with the step key")
         for file_key in workflow.get_products(self.key, kind="file"):
             file = workflow.get_file(file_key)
             if file.get_state(workflow) in (FileState.MISSING, FileState.BUILT):
                 raise ValueError("Upon replay, output files cannot be MISSING or BUILT")
         recording = self._recording
         # Restore as if the step executed
+        for pool, size in recording.defined_pools.items():
+            workflow.set_pool(self.key, pool, size)
         workflow.declare_static(self.key, recording.static_paths)
         for step_args in recording.steps_args:
             workflow.define_step(**step_args)
         for ngm in recording.nglob_multis:
             workflow.register_nglob(self.key, ngm)
         for patterns in recording.deferred_glob_args:
             workflow.defer_glob(self.key, patterns)
```

### Comparing `stepup-1.2.3/stepup/core/tui.py` & `stepup-1.2.4/stepup/core/tui.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,21 +175,21 @@
         AsyncReadChar() as readchar,
     ):
         async for ch in stoppable_iterator(readchar, stop_event):
             if ch == "q":
                 await reporter("KEYBOARD", "Waiting for workers to complete before shutdown.")
                 await client.call.shutdown()
                 break
-            elif ch == "d":
-                await reporter("KEYBOARD", "Draining the scheduler and waiting for workers.")
-                await client.call.drain()
-            elif ch == "j":
+            if ch == "j":
                 await reporter("KEYBOARD", "Waiting for the runner to complete to shutdown.")
                 await client.call.join()
                 break
+            if ch == "d":
+                await reporter("KEYBOARD", "Draining the scheduler and waiting for workers.")
+                await client.call.drain()
             elif ch == "r":
                 await reporter("KEYBOARD", "Restarting the runner.")
                 async with asyncio.timeout(5):
                     await client.call.run()
             elif ch == "g":
                 async with asyncio.timeout(5):
                     await client.call.graph("graph")
```

### Comparing `stepup-1.2.3/stepup/core/utils.py` & `stepup-1.2.4/stepup/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,26 +159,26 @@
 
 #
 # Miscellaneous
 #
 
 
 # Adapted from https://stackoverflow.com/a/39542816/494584
-class classproperty(property):
+class classproperty(property):  # noqa: N801
     def __get__(self, obj, objtype=None):
         return super().__get__(objtype)
 
     def __set__(self, obj, value):
         super().__set__(type(obj), value)
 
     def __delete__(self, obj):
         super().__delete__(type(obj))
 
 
-class lookupdict(dict):
+class lookupdict(dict):  # noqa: N801
     """Dictionary assigning enumerated values to keys."""
 
     def __missing__(self, key):
         if not isinstance(key, str):
             raise TypeError("lookupdict only supports string keys")
         size = len(self)
         self[str(key)] = size
```

### Comparing `stepup-1.2.3/stepup/core/watcher.py` & `stepup-1.2.4/stepup/core/watcher.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/stepup/core/worker.py` & `stepup-1.2.4/stepup/core/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         await self.client.close()
 
     #
     # Functions called by jobs
     #
 
     async def validate_amended_job(self, step_key: str) -> bool:
-        """Test if the inputs have changed, which would invalidate the amended step info.
+        """Test if the inputs (hashes) have changed, which would invalidate the amended step info.
 
         Parameters
         ----------
         step_key
             The step whose amended inputs need validation.
 
         Returns
```

### Comparing `stepup-1.2.3/stepup/core/workflow.py` & `stepup-1.2.4/stepup/core/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 from .assoc import Assoc, many_to_one
 from .cascade import Cascade, Node, get_kind
 from .deferred_glob import DeferredGlob
 from .exceptions import GraphError
 from .file import File, FileState
 from .hash import ExtendedStepHash, FileHash
+from .job import SetPoolJob
 from .nglob import NGlobMulti
 from .step import Mandatory, Step, StepState
 from .utils import lookupdict, myparent
 
 __all__ = ("Workflow",)
 
 
@@ -163,17 +164,19 @@
             elif node.kind == "file":
                 props = " shape=rect fillcolor=9"
             elif node.kind == "dg":
                 props = " shape=octagon fillcolor=7"
             else:
                 props = " shape=hexagon fillcolor=6"
             lines.append(f"  {lookup[key]} [label={label}{props}]")
-            for other in edges.get(key, ()):
-                if other != key:
-                    lines.append(f"  {lookup[key]} -> {lookup[other]}")
+            lines.extend(
+                f"  {lookup[key]} -> {lookup[other]}"
+                for other in edges.get(key, ())
+                if other != key
+            )
         lines.append("}")
         return "\n".join(lines)
 
     def format_dot_creator(self):
         """Return the creator-product graph in GraphViz DOT format."""
         return self._format_dot_generic("empty", True, self.products)
 
@@ -245,36 +248,33 @@
     #
     # Run phase
     #
 
     def _check_step_key(self, step_key: str, argname: str, allow_root=False):
         """Check the creator or step key in the methods below."""
         if not isinstance(step_key, str):
-            raise ValueError(f"{argname} must be a string, got: {type(step_key)}")
+            raise TypeError(f"{argname} must be a string, got: {type(step_key)}")
         if step_key not in self.nodes:
             raise ValueError(f"Unknown {argname}: '{step_key}'")
         if self.is_orphan(step_key):
             raise ValueError(f"{argname} is orphan: '{step_key}'")
         if allow_root and step_key == "root:":
             return
-        if not (step_key.startswith("step:") or step_key.startswith("dg:")):
+        if not (step_key.startswith(("step:", "dg:"))):
             allowed = "step, dg or root" if allow_root else "step or dg"
             raise ValueError(f"{argname} is not a {allowed}: '{step_key}'")
 
     def supply_parent(self, file: File) -> tuple[str | None, bool, bool]:
         parent_path = myparent(file.path)
         if parent_path is None:
             return None, True, False
         return self.supply_file(file.key, parent_path, new=False)
 
     def matching_deferred_glob(self, path: str) -> DeferredGlob | None:
-        dgs = []
-        for dg in self.get_deferred_globs():
-            if dg.ngm.may_match(path):
-                dgs.append(dg)
+        dgs = [dg for dg in self.get_deferred_globs() if dg.ngm.may_match(path)]
         if len(dgs) > 1:
             raise GraphError(f"Multiple deferred globs match: {path}")
         if len(dgs) == 1:
             return dgs[0]
         return None
 
     @staticmethod
@@ -328,15 +328,15 @@
         if new_relation:
             self.supply(file_key, step_key)
         elif new:
             raise GraphError(f"Supplying file already exists: {path}")
         return file_key, available, new_relation
 
     def create_file(self, creator_key: str, path: str, file_state: FileState) -> str:
-        """Create (or recycle) a file with a PENDING or VOLATILE file state.
+        """Create (or recycle) a file with a STATIC, PENDING or VOLATILE file state.
 
         Parameters
         ----------
         creator_key
             The creating step, deferred glob.
         path
             The (normalized path). Directories must have trailing slashes.
@@ -442,18 +442,16 @@
                         raise GraphError(f"Static path has no static parent path node: {path}")
                 except ValueError as exc:
                     parent_path = myparent(path)
                     if parent_path not in paths:
                         raise GraphError(f"Static path has no parent path node: {path}") from exc
 
             file_key = f"file:{path}"
-            if file_key in self.nodes:
-                if file_key in self.nodes and not self.is_orphan(file_key):
-                    raise GraphError(f"Static path already exists: {path}")
-                self.check_cyclic(creator_key, file_key)
+            if file_key in self.nodes and not self.is_orphan(file_key):
+                raise GraphError(f"Static path already exists: {path}")
         # Make the actual changes
         self.graph_changed = True
         return [self.create_file(creator_key, path, FileState.STATIC) for path in paths]
 
     def check_inputs_outputs(
         self,
         step_key: str,
@@ -604,14 +602,21 @@
             step.infer_mandatory(self)
         else:
             step.imply_mandatory_suppliers(self)
             step.queue_if_appropriate(self)
 
         return step_key
 
+    def set_pool(self, step_key: str, pool: str, size: int):
+        """Set the pool size and keep the information in the step to support replay."""
+        step = self.get_step(step_key)
+        step.defined_pools[pool] = size
+        self.job_queue.put_nowait(SetPoolJob(pool, size))
+        self.job_queue_changed.set()
+
     def amend_step(
         self,
         step_key: str,
         inp_paths: Collection[str] = (),
         env_vars: Collection[str] = (),
         out_paths: Collection[str] = (),
         vol_paths: Collection[str] = (),
```

### Comparing `stepup-1.2.3/stepup.egg-info/PKG-INFO` & `stepup-1.2.4/stepup.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepup
-Version: 1.2.3
+Version: 1.2.4
 Summary: StepUp Core provides the basic framework for the StepUp build tool
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-core/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-core/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-core/
 Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-core/changelog/
 Classifier: Environment :: Console
```

### Comparing `stepup-1.2.3/stepup.egg-info/SOURCES.txt` & `stepup-1.2.4/stepup.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -271,14 +271,18 @@
 tests/cases/amend_outdir_pending/.gitignore
 tests/cases/amend_outdir_pending/README.md
 tests/cases/amend_outdir_pending/demo.py
 tests/cases/amend_outdir_pending/expected_graph.txt
 tests/cases/amend_outdir_pending/expected_stdout.txt
 tests/cases/amend_outdir_pending/main.sh
 tests/cases/amend_outdir_pending/plan.py
+tests/cases/amend_self_static/.gitignore
+tests/cases/amend_self_static/main.sh
+tests/cases/amend_self_static/plan.py
+tests/cases/amend_self_static/step.py
 tests/cases/amend_voldir_pending/.gitignore
 tests/cases/amend_voldir_pending/README.md
 tests/cases/amend_voldir_pending/demo.py
 tests/cases/amend_voldir_pending/expected_graph.txt
 tests/cases/amend_voldir_pending/expected_stdout.txt
 tests/cases/amend_voldir_pending/main.sh
 tests/cases/amend_voldir_pending/plan.py
@@ -469,15 +473,17 @@
 tests/cases/nostatic/main.sh
 tests/cases/nostatic/plan.py
 tests/cases/not_cyclic/.gitignore
 tests/cases/not_cyclic/README.md
 tests/cases/not_cyclic/expected_graph_01.txt
 tests/cases/not_cyclic/expected_graph_02.txt
 tests/cases/not_cyclic/expected_graph_03.txt
-tests/cases/not_cyclic/expected_stdout.txt
+tests/cases/not_cyclic/expected_graph_04.txt
+tests/cases/not_cyclic/expected_stdout_a.txt
+tests/cases/not_cyclic/expected_stdout_b.txt
 tests/cases/not_cyclic/main.sh
 tests/cases/not_cyclic/plan.py
 tests/cases/optional_convert/.gitignore
 tests/cases/optional_convert/README.md
 tests/cases/optional_convert/expected_graph_a.txt
 tests/cases/optional_convert/expected_graph_b.txt
 tests/cases/optional_convert/expected_graph_c.txt
@@ -545,14 +551,22 @@
 tests/cases/permissions_step_restart/step.py
 tests/cases/pool/.gitignore
 tests/cases/pool/README.md
 tests/cases/pool/expected_graph.txt
 tests/cases/pool/main.sh
 tests/cases/pool/plan.py
 tests/cases/pool/r.txt
+tests/cases/pool_restart/.gitignore
+tests/cases/pool_restart/README.md
+tests/cases/pool_restart/expected_graph_1.txt
+tests/cases/pool_restart/expected_graph_2.txt
+tests/cases/pool_restart/expected_stdout_a.txt
+tests/cases/pool_restart/expected_stdout_b.txt
+tests/cases/pool_restart/main.sh
+tests/cases/pool_restart/plan.py
 tests/cases/reqdir_missing/.gitignore
 tests/cases/reqdir_missing/README.md
 tests/cases/reqdir_missing/expected_graph.txt
 tests/cases/reqdir_missing/expected_stdout.txt
 tests/cases/reqdir_missing/main.sh
 tests/cases/reqdir_missing/plan.py
 tests/cases/restart_blocked/.gitignore
@@ -694,14 +708,23 @@
 tests/cases/static_nglob_partial/expected_graph_02.txt
 tests/cases/static_nglob_partial/expected_graph_03.txt
 tests/cases/static_nglob_partial/expected_graph_04.txt
 tests/cases/static_nglob_partial/expected_stdout_a.txt
 tests/cases/static_nglob_partial/expected_stdout_b.txt
 tests/cases/static_nglob_partial/main.sh
 tests/cases/static_nglob_partial/plan.py
+tests/cases/static_nglob_recursive/.gitignore
+tests/cases/static_nglob_recursive/README.md
+tests/cases/static_nglob_recursive/expected_graph.txt
+tests/cases/static_nglob_recursive/expected_stdout.txt
+tests/cases/static_nglob_recursive/main.sh
+tests/cases/static_nglob_recursive/plan.py
+tests/cases/static_nglob_recursive/data/test1.txt
+tests/cases/static_nglob_recursive/data/test2.dat
+tests/cases/static_nglob_recursive/data/sub/test3.xyz
 tests/cases/static_nglob_subdir/.gitignore
 tests/cases/static_nglob_subdir/README.md
 tests/cases/static_nglob_subdir/expected_graph.txt
 tests/cases/static_nglob_subdir/expected_stdout.txt
 tests/cases/static_nglob_subdir/main.sh
 tests/cases/static_nglob_subdir/plan.py
 tests/cases/static_nglob_subdir/sub/inp1.txt
```

### Comparing `stepup-1.2.3/tests/cases/README.md` & `stepup-1.2.4/tests/cases/README.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/amend/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/amend/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend/expected_graph_03.txt` & `stepup-1.2.4/tests/cases/amend/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend/expected_graph_04.txt` & `stepup-1.2.4/tests/cases/amend/expected_graph_04.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend/expected_stdout_01.txt` & `stepup-1.2.4/tests/cases/amend/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend/expected_stdout_02.txt` & `stepup-1.2.4/tests/cases/amend/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend/expected_stdout_03.txt` & `stepup-1.2.4/tests/cases/amend/expected_stdout_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend/main.sh` & `stepup-1.2.4/tests/cases/amend/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend_delay/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/amend_delay/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend_delay/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/amend_delay/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend_delay/expected_graph_03.txt` & `stepup-1.2.4/tests/cases/amend_delay/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend_delay/expected_stdout.txt` & `stepup-1.2.4/tests/cases/amend_delay/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend_delay/main.sh` & `stepup-1.2.4/tests/cases/amend_delay/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend_env_vars/expected_graph.txt` & `stepup-1.2.4/tests/cases/amend_env_vars/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend_env_vars/main.sh` & `stepup-1.2.4/tests/cases/amend_env_vars/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend_missing/expected_graph.txt` & `stepup-1.2.4/tests/cases/amend_missing/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend_missing/expected_stdout.txt` & `stepup-1.2.4/tests/cases/amend_missing/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend_missing/main.sh` & `stepup-1.2.4/tests/cases/amend_missing/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend_outdir_pending/expected_graph.txt` & `stepup-1.2.4/tests/cases/amend_outdir_pending/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend_outdir_pending/expected_stdout.txt` & `stepup-1.2.4/tests/cases/amend_outdir_pending/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend_outdir_pending/main.sh` & `stepup-1.2.4/tests/cases/amend_outdir_pending/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend_voldir_pending/expected_graph.txt` & `stepup-1.2.4/tests/cases/amend_voldir_pending/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend_voldir_pending/expected_stdout.txt` & `stepup-1.2.4/tests/cases/amend_voldir_pending/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/amend_voldir_pending/main.sh` & `stepup-1.2.4/tests/cases/amend_voldir_pending/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/deferred_glob1/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/deferred_glob1/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/deferred_glob1/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/deferred_glob1/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/deferred_glob1/main.sh` & `stepup-1.2.4/tests/cases/deferred_glob1/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/deferred_glob2/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/deferred_glob2/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/deferred_glob2/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/deferred_glob2/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/deferred_glob2/expected_stdout.txt` & `stepup-1.2.4/tests/cases/deferred_glob2/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/deferred_glob2/main.sh` & `stepup-1.2.4/tests/cases/deferred_glob2/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/deferred_subdir/expected_graph.txt` & `stepup-1.2.4/tests/cases/deferred_subdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/deferred_subdir/main.sh` & `stepup-1.2.4/tests/cases/deferred_subdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/env_vars/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/env_vars/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars/expected_graph_03.txt` & `stepup-1.2.4/tests/cases/env_vars/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars/expected_graph_04.txt` & `stepup-1.2.4/tests/cases/env_vars/expected_graph_04.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars/expected_graph_05.txt` & `stepup-1.2.4/tests/cases/env_vars/expected_graph_05.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars/expected_stdout_a.txt` & `stepup-1.2.4/tests/cases/env_vars/expected_stdout_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars/expected_stdout_b.txt` & `stepup-1.2.4/tests/cases/env_vars/expected_stdout_b.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars/expected_stdout_c.txt` & `stepup-1.2.4/tests/cases/env_vars/expected_stdout_c.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars/expected_stdout_d.txt` & `stepup-1.2.4/tests/cases/env_vars/expected_stdout_d.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars/main.sh` & `stepup-1.2.4/tests/cases/env_vars/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars_amend/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/env_vars_amend/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars_amend/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/env_vars_amend/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars_amend/expected_stdout_02.txt` & `stepup-1.2.4/tests/cases/env_vars_amend/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars_amend/main.sh` & `stepup-1.2.4/tests/cases/env_vars_amend/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars_path/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/env_vars_path/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars_path/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/env_vars_path/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars_path/expected_stdout_01.txt` & `stepup-1.2.4/tests/cases/env_vars_path/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars_path/expected_stdout_02.txt` & `stepup-1.2.4/tests/cases/env_vars_path/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars_path/main.sh` & `stepup-1.2.4/tests/cases/env_vars_path/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars_subs/expected_graph.txt` & `stepup-1.2.4/tests/cases/env_vars_subs/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars_subs/expected_stdout.txt` & `stepup-1.2.4/tests/cases/env_vars_subs/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars_subs/main.sh` & `stepup-1.2.4/tests/cases/env_vars_subs/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars_workdir/expected_graph.txt` & `stepup-1.2.4/tests/cases/env_vars_workdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/env_vars_workdir/main.sh` & `stepup-1.2.4/tests/cases/env_vars_workdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_cyclic_late/expected_graph.txt` & `stepup-1.2.4/tests/cases/static_dir/expected_graph.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 root:
              version = v1
+             creates   file:./
+             creates   file:plan.py
+             creates   step:./plan.py
 
-(file:plan.py)
+file:plan.py
                 path = plan.py
                state = STATIC
-            consumes   (file:./)
+          created by   root:
+            consumes   file:./
+            supplies   step:./plan.py
 
-(file:./)
+file:./
                 path = ./
                state = STATIC
-            supplies   (file:plan.py)
-            supplies   (file:second)
+          created by   root:
+            supplies   file:plan.py
+            supplies   file:subdir/
+            supplies   step:./plan.py
 
-(step:./plan.py)
+step:./plan.py
              workdir = ./
              command = ./plan.py
-               state = PENDING
+               state = SUCCEEDED
+          created by   root:
+            consumes   file:./
+            consumes   file:plan.py
+             creates   file:subdir/
 
-(step:cat first > second)
-             workdir = ./
-             command = cat first > second
-               state = PENDING
-
-(file:first)
-                path = first
-               state = PENDING
-
-(file:second)
-                path = second
-               state = PENDING
-            consumes   (file:./)
-
-(step:cat second > first)
-             workdir = ./
-             command = cat second > first
-               state = PENDING
+file:subdir/
+                path = subdir/
+               state = STATIC
+          created by   step:./plan.py
+            consumes   file:./
```

### Comparing `stepup-1.2.3/tests/cases/error_cyclic_late/expected_stdout.txt` & `stepup-1.2.4/tests/cases/error_cyclic_late/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_cyclic_late/main.sh` & `stepup-1.2.4/tests/cases/error_cyclic_late/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_deferred_nonexisting/expected_stdout.txt` & `stepup-1.2.4/tests/cases/error_deferred_nonexisting/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_deferred_nonexisting/main.sh` & `stepup-1.2.4/tests/cases/error_deferred_nonexisting/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_env_var/expected_graph.txt` & `stepup-1.2.4/tests/cases/error_env_var/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_env_var/expected_stdout.txt` & `stepup-1.2.4/tests/cases/error_env_var/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_env_var/main.sh` & `stepup-1.2.4/tests/cases/error_env_var/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_main_fails/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/error_main_fails/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_main_fails/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/error_main_fails/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_main_fails/expected_stdout_02.txt` & `stepup-1.2.4/tests/cases/error_main_fails/expected_stdout_02.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
   WORKFLOW │ Loaded from .stepup/workflow.mpk.xz
   DIRECTOR │ Launched worker 0
      PHASE │ run
     NOSKIP │ ./plan.py
 ──────────────────────────── Changes causing rerun ─────────────────────────────
-Modified step hash   extended, digest 53ca023c ➜ 59506490, inp_digset 53ca023c ➜ 59506490
-Modified inp hash    plan.py (digest 98e52b4a ➜ 6057f437, size 101 ➜ 46)
+Modified step hash   extended, digest 53ca023c ➜ c618f004, inp_digset 53ca023c ➜ c618f004
+Modified inp hash    plan.py (digest 98e52b4a ➜ 52421150, size 101 ➜ 44)
 ────────────────────────────── Remained the same ───────────────────────────────
 Same inp hash        ./
 ────────────────────────────────────────────────────────────────────────────────
      START │ ./plan.py
       FAIL │ ./plan.py
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               ./plan.py
```

### Comparing `stepup-1.2.3/tests/cases/error_main_fails/main.sh` & `stepup-1.2.4/tests/cases/error_main_fails/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_not_executable/expected_stdout.txt` & `stepup-1.2.4/tests/cases/error_not_executable/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_overlap_deferred/expected_stdout.txt` & `stepup-1.2.4/tests/cases/error_overlap_deferred/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_overlap_deferred/main.sh` & `stepup-1.2.4/tests/cases/error_overlap_deferred/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_static_dir/expected_graph.txt` & `stepup-1.2.4/tests/cases/error_static_dir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_static_dir/expected_stdout.txt` & `stepup-1.2.4/tests/cases/error_static_dir/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_static_dir/main.sh` & `stepup-1.2.4/tests/cases/error_static_dir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_step/expected_graph.txt` & `stepup-1.2.4/tests/cases/error_step/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_step/expected_stdout.txt` & `stepup-1.2.4/tests/cases/error_step/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/error_step/main.sh` & `stepup-1.2.4/tests/cases/error_step/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/here/expected_graph.txt` & `stepup-1.2.4/tests/cases/here/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/here/expected_stdout.txt` & `stepup-1.2.4/tests/cases/here/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/here/main.sh` & `stepup-1.2.4/tests/cases/here/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/makedirs/expected_graph.txt` & `stepup-1.2.4/tests/cases/makedirs/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/makedirs/main.sh` & `stepup-1.2.4/tests/cases/makedirs/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/mkdir/expected_graph.txt` & `stepup-1.2.4/tests/cases/mkdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/mkdir/main.sh` & `stepup-1.2.4/tests/cases/mkdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/mkdir_error/expected_graph.txt` & `stepup-1.2.4/tests/cases/mkdir_error/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/mkdir_error/expected_stdout.txt` & `stepup-1.2.4/tests/cases/mkdir_error/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/mkdir_error/main.sh` & `stepup-1.2.4/tests/cases/mkdir_error/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/nodata/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/nodata/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/nodata/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/nodata/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/nodata/expected_graph_03.txt` & `stepup-1.2.4/tests/cases/nodata/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/nodata/expected_stdout_a.txt` & `stepup-1.2.4/tests/cases/nodata/expected_stdout_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/nodata/expected_stdout_b.txt` & `stepup-1.2.4/tests/cases/nodata/expected_stdout_b.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/nodata/main.sh` & `stepup-1.2.4/tests/cases/nodata/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/noplan/expected_stdout.txt` & `stepup-1.2.4/tests/cases/noplan/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/nostatic/expected_graph.txt` & `stepup-1.2.4/tests/cases/nostatic/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/nostatic/expected_stdout.txt` & `stepup-1.2.4/tests/cases/nostatic/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/nostatic/main.sh` & `stepup-1.2.4/tests/cases/nostatic/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/not_cyclic/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/not_cyclic/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/not_cyclic/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/not_cyclic/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/not_cyclic/expected_graph_03.txt` & `stepup-1.2.4/tests/cases/not_cyclic/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/not_cyclic/expected_stdout.txt` & `stepup-1.2.4/tests/cases/not_cyclic/expected_stdout_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/not_cyclic/main.sh` & `stepup-1.2.4/tests/cases/amend_self_static/main.sh`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 echo "hello" > input.txt
-stepup -w 1 plan.py & # > current_stdout.txt &
+stepup -w 1 plan.py & # > current_stdout_a.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
 # Get the graph after completion of the pending steps.
@@ -56,7 +56,32 @@
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f input.txt ]] || exit -1
 grep bye output.txt
 
 # Wait for background processes, if any.
 wait
+
+# Do nothig and run again
+stepup -w 1 plan.py & # > current_stdout_b.txt &
+
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
+# Get the graph after completion of the pending steps.
+python3 - << EOD
+from stepup.core.interact import *
+wait()
+graph("current_graph_04")
+join()
+EOD
+
+# Check files that are expected to be present and/or missing.
+[[ -f plan.py ]] || exit -1
+[[ -f input.txt ]] || exit -1
+grep bye output.txt
+grep BUILT current_graph_04.txt
+
+# Wait for background processes, if any.
+wait
```

### Comparing `stepup-1.2.3/tests/cases/optional_convert/expected_graph_a.txt` & `stepup-1.2.4/tests/cases/optional_convert/expected_graph_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/optional_convert/expected_graph_b.txt` & `stepup-1.2.4/tests/cases/optional_convert/expected_graph_b.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/optional_convert/expected_graph_c.txt` & `stepup-1.2.4/tests/cases/optional_convert/expected_graph_c.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/optional_convert/expected_stdout_a.txt` & `stepup-1.2.4/tests/cases/optional_convert/expected_stdout_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/optional_convert/main.sh` & `stepup-1.2.4/tests/cases/optional_convert/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/output_not_created/expected_graph.txt` & `stepup-1.2.4/tests/cases/output_not_created/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/output_not_created/expected_stdout.txt` & `stepup-1.2.4/tests/cases/output_not_created/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/output_not_created/main.sh` & `stepup-1.2.4/tests/cases/output_not_created/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/pending/expected_graph.txt` & `stepup-1.2.4/tests/cases/pending/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/pending/expected_stdout.txt` & `stepup-1.2.4/tests/cases/pending/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/pending/main.sh` & `stepup-1.2.4/tests/cases/pending/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_file_rerun/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/permissions_file_rerun/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_file_rerun/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/permissions_file_rerun/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_file_rerun/expected_stdout.txt` & `stepup-1.2.4/tests/cases/permissions_file_rerun/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_file_rerun/main.sh` & `stepup-1.2.4/tests/cases/permissions_file_rerun/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_plan_rerun/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/permissions_plan_rerun/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_plan_rerun/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/permissions_plan_rerun/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_plan_rerun/expected_stdout.txt` & `stepup-1.2.4/tests/cases/permissions_plan_rerun/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_plan_rerun/main.sh` & `stepup-1.2.4/tests/cases/permissions_plan_rerun/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_plan_restart/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/permissions_plan_restart/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_plan_restart/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/permissions_plan_restart/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_plan_restart/expected_stdout_01.txt` & `stepup-1.2.4/tests/cases/permissions_plan_restart/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_plan_restart/expected_stdout_02.txt` & `stepup-1.2.4/tests/cases/permissions_plan_restart/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_plan_restart/main.sh` & `stepup-1.2.4/tests/cases/permissions_plan_restart/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_step_rerun/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/permissions_step_rerun/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_step_rerun/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/permissions_step_rerun/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_step_rerun/expected_stdout.txt` & `stepup-1.2.4/tests/cases/permissions_step_rerun/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_step_rerun/main.sh` & `stepup-1.2.4/tests/cases/permissions_step_rerun/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_step_restart/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/permissions_step_restart/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_step_restart/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/permissions_step_restart/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_step_restart/expected_stdout_01.txt` & `stepup-1.2.4/tests/cases/permissions_step_restart/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_step_restart/expected_stdout_02.txt` & `stepup-1.2.4/tests/cases/permissions_step_restart/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/permissions_step_restart/main.sh` & `stepup-1.2.4/tests/cases/permissions_step_restart/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/pool/expected_graph.txt` & `stepup-1.2.4/tests/cases/pool/expected_graph.txt`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
             supplies   step:echo 1; mv r.txt u.txt; sleep 0.1; mv u.txt r.txt
             supplies   step:echo 2; mv r.txt u.txt; sleep 0.1; mv u.txt r.txt
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
+        defined pool = transform=1
           created by   root:
             consumes   file:./
             consumes   file:plan.py
              creates   step:echo 1; mv r.txt u.txt; sleep 0.1; mv u.txt r.txt
              creates   step:echo 2; mv r.txt u.txt; sleep 0.1; mv u.txt r.txt
 
 step:echo 1; mv r.txt u.txt; sleep 0.1; mv u.txt r.txt
```

### Comparing `stepup-1.2.3/tests/cases/pool/main.sh` & `stepup-1.2.4/tests/cases/pool/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/reqdir_missing/expected_graph.txt` & `stepup-1.2.4/tests/cases/reqdir_missing/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/reqdir_missing/expected_stdout.txt` & `stepup-1.2.4/tests/cases/reqdir_missing/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/reqdir_missing/main.sh` & `stepup-1.2.4/tests/cases/reqdir_missing/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_blocked/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/restart_blocked/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_blocked/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/restart_blocked/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_blocked/expected_stdout_01.txt` & `stepup-1.2.4/tests/cases/restart_blocked/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_blocked/expected_stdout_02.txt` & `stepup-1.2.4/tests/cases/restart_blocked/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_blocked/main.sh` & `stepup-1.2.4/tests/cases/restart_blocked/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_changes/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/restart_changes/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_changes/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/restart_changes/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_changes/expected_stdout_02.txt` & `stepup-1.2.4/tests/cases/restart_changes/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_changes/main.sh` & `stepup-1.2.4/tests/cases/restart_changes/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_deferred_glob/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/restart_deferred_glob/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_deferred_glob/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/restart_deferred_glob/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_deferred_glob/expected_stdout_01.txt` & `stepup-1.2.4/tests/cases/restart_deferred_glob/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_deferred_glob/expected_stdout_02.txt` & `stepup-1.2.4/tests/cases/restart_deferred_glob/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_deferred_glob/main.sh` & `stepup-1.2.4/tests/cases/restart_deferred_glob/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_nochanges/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/restart_nochanges/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_nochanges/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/restart_nochanges/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_nochanges/expected_stdout_01.txt` & `stepup-1.2.4/tests/cases/restart_nochanges/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_nochanges/expected_stdout_02.txt` & `stepup-1.2.4/tests/cases/restart_nochanges/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_nochanges/main.sh` & `stepup-1.2.4/tests/cases/restart_nochanges/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_orphan/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/restart_orphan/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_orphan/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/restart_orphan/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_orphan/expected_stdout_02.txt` & `stepup-1.2.4/tests/cases/restart_orphan/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_orphan/main.sh` & `stepup-1.2.4/tests/cases/restart_orphan/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_outdated_amend/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/restart_outdated_amend/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_outdated_amend/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/restart_outdated_amend/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_outdated_amend/expected_stdout_02.txt` & `stepup-1.2.4/tests/cases/restart_outdated_amend/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_outdated_amend/main.sh` & `stepup-1.2.4/tests/cases/restart_outdated_amend/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_output/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/restart_output/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_output/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/restart_output/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_output/expected_stdout_02.txt` & `stepup-1.2.4/tests/cases/restart_output/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/restart_output/main.sh` & `stepup-1.2.4/tests/cases/restart_output/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/script_cases/expected_graph.txt` & `stepup-1.2.4/tests/cases/script_cases/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/script_cases/main.sh` & `stepup-1.2.4/tests/cases/script_cases/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/script_cases_settings/README.md` & `stepup-1.2.4/tests/cases/script_cases_settings/README.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/script_cases_settings/expected_graph.txt` & `stepup-1.2.4/tests/cases/script_cases_settings/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/script_cases_settings/main.sh` & `stepup-1.2.4/tests/cases/script_cases_settings/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/script_single/expected_graph.txt` & `stepup-1.2.4/tests/cases/script_single/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/script_single/expected_stdout.txt` & `stepup-1.2.4/tests/cases/script_single/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/script_single/main.sh` & `stepup-1.2.4/tests/cases/script_single/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/script_single/work/generate.py` & `stepup-1.2.4/tests/cases/script_single/work/generate.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static/expected_graph.txt` & `stepup-1.2.4/tests/cases/static/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static/main.sh` & `stepup-1.2.4/tests/cases/static/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_abs/expected_graph.txt` & `stepup-1.2.4/tests/cases/static_abs/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_abs/main.sh` & `stepup-1.2.4/tests/cases/static_abs/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_dir/expected_graph.txt` & `stepup-1.2.4/tests/cases/watch_wanted/expected_graph_03.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,25 +11,25 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
+            supplies   file:input2.txt
             supplies   file:plan.py
-            supplies   file:subdir/
             supplies   step:./plan.py
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
           created by   root:
             consumes   file:./
             consumes   file:plan.py
-             creates   file:subdir/
+             creates   file:input2.txt
 
-file:subdir/
-                path = subdir/
+file:input2.txt
+                path = input2.txt
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
```

### Comparing `stepup-1.2.3/tests/cases/static_dir/main.sh` & `stepup-1.2.4/tests/cases/static_dir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_glob/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/static_glob/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_glob/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/static_glob/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_glob/expected_graph_03.txt` & `stepup-1.2.4/tests/cases/static_glob/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_glob/expected_stdout_a.txt` & `stepup-1.2.4/tests/cases/static_glob/expected_stdout_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_glob/expected_stdout_b.txt` & `stepup-1.2.4/tests/cases/static_glob/expected_stdout_b.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_glob/main.sh` & `stepup-1.2.4/tests/cases/static_glob/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_nglob/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/static_nglob/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_nglob/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/static_nglob/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_nglob/expected_stdout.txt` & `stepup-1.2.4/tests/cases/static_nglob/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_nglob/main.sh` & `stepup-1.2.4/tests/cases/static_nglob/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_nglob/plan.py` & `stepup-1.2.4/tests/cases/static_nglob/plan.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_nglob_partial/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/static_nglob_partial/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_nglob_partial/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/static_nglob_partial/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_nglob_partial/expected_graph_03.txt` & `stepup-1.2.4/tests/cases/static_nglob_partial/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_nglob_partial/expected_graph_04.txt` & `stepup-1.2.4/tests/cases/static_nglob_partial/expected_graph_04.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_nglob_partial/expected_stdout_a.txt` & `stepup-1.2.4/tests/cases/static_nglob_partial/expected_stdout_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_nglob_partial/expected_stdout_b.txt` & `stepup-1.2.4/tests/cases/static_nglob_partial/expected_stdout_b.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_nglob_partial/main.sh` & `stepup-1.2.4/tests/cases/static_nglob_partial/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_nglob_subdir/expected_graph.txt` & `stepup-1.2.4/tests/cases/static_nglob_subdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/static_nglob_subdir/main.sh` & `stepup-1.2.4/tests/cases/static_nglob_subdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/subdir/expected_graph.txt` & `stepup-1.2.4/tests/cases/subdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/subdir/expected_stdout.txt` & `stepup-1.2.4/tests/cases/subdir/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/subdir/main.sh` & `stepup-1.2.4/tests/cases/subdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_blocked/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/watch_blocked/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_blocked/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/watch_blocked/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_blocked/expected_stdout.txt` & `stepup-1.2.4/tests/cases/watch_blocked/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_blocked/main.sh` & `stepup-1.2.4/tests/cases/watch_blocked/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_boot/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/watch_boot/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_boot/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/watch_boot/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_boot/expected_stdout.txt` & `stepup-1.2.4/tests/cases/watch_boot/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_boot/main.sh` & `stepup-1.2.4/tests/cases/watch_boot/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_chain/README.md` & `stepup-1.2.4/tests/cases/watch_chain/README.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_chain/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/watch_chain/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_chain/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/watch_chain/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_chain/expected_stdout.txt` & `stepup-1.2.4/tests/cases/watch_chain/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_chain/main.sh` & `stepup-1.2.4/tests/cases/watch_chain/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_chain/use_config.py` & `stepup-1.2.4/tests/cases/watch_chain/use_config.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_input/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/watch_input/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_input/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/watch_input/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_input/expected_graph_03.txt` & `stepup-1.2.4/tests/cases/watch_input/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_input/expected_stdout.txt` & `stepup-1.2.4/tests/cases/watch_input/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_input/main.sh` & `stepup-1.2.4/tests/cases/watch_input/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_middle/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/watch_middle/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_middle/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/watch_middle/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_middle/expected_graph_03.txt` & `stepup-1.2.4/tests/cases/watch_middle/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_middle/expected_stdout.txt` & `stepup-1.2.4/tests/cases/watch_middle/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_middle/main.sh` & `stepup-1.2.4/tests/cases/watch_middle/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_mixed/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/watch_mixed/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_mixed/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/watch_mixed/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_mixed/expected_stdout.txt` & `stepup-1.2.4/tests/cases/watch_mixed/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_mixed/main.sh` & `stepup-1.2.4/tests/cases/watch_mixed/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_nochanges/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/watch_nochanges/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_nochanges/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/watch_nochanges/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_nochanges/main.sh` & `stepup-1.2.4/tests/cases/watch_nochanges/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_outdated_amend1/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/watch_outdated_amend1/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_outdated_amend1/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/watch_outdated_amend1/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_outdated_amend1/expected_stdout.txt` & `stepup-1.2.4/tests/cases/watch_outdated_amend1/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_outdated_amend1/main.sh` & `stepup-1.2.4/tests/cases/watch_outdated_amend1/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_outdated_amend2/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/watch_outdated_amend2/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_outdated_amend2/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/watch_outdated_amend2/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_outdated_amend2/expected_stdout.txt` & `stepup-1.2.4/tests/cases/watch_outdated_amend2/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_outdated_amend2/main.sh` & `stepup-1.2.4/tests/cases/watch_outdated_amend2/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_output/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/watch_output/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_output/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/watch_output/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_output/expected_stdout.txt` & `stepup-1.2.4/tests/cases/watch_output/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_output/main.sh` & `stepup-1.2.4/tests/cases/watch_output/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_wanted/expected_graph_01.txt` & `stepup-1.2.4/tests/cases/watch_wanted/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_wanted/expected_graph_02.txt` & `stepup-1.2.4/tests/cases/watch_wanted/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_wanted/expected_graph_03.txt` & `stepup-1.2.4/tests/cases/pool_restart/expected_graph_1.txt`

 * *Files 27% similar despite different names*

```diff
@@ -11,25 +11,38 @@
             consumes   file:./
             supplies   step:./plan.py
 
 file:./
                 path = ./
                state = STATIC
           created by   root:
-            supplies   file:input2.txt
+            supplies   file:bar.txt
             supplies   file:plan.py
             supplies   step:./plan.py
+            supplies   step:echo foo > bar.txt
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
+        defined pool = random=1
           created by   root:
             consumes   file:./
             consumes   file:plan.py
-             creates   file:input2.txt
+             creates   step:echo foo > bar.txt
 
-file:input2.txt
-                path = input2.txt
-               state = STATIC
+step:echo foo > bar.txt
+             workdir = ./
+             command = echo foo > bar.txt
+               state = SUCCEEDED
+                pool = random
           created by   step:./plan.py
             consumes   file:./
+             creates   file:bar.txt
+            supplies   file:bar.txt
+
+file:bar.txt
+                path = bar.txt
+               state = BUILT
+          created by   step:echo foo > bar.txt
+            consumes   file:./
+            consumes   step:echo foo > bar.txt
```

### Comparing `stepup-1.2.3/tests/cases/watch_wanted/expected_stdout.txt` & `stepup-1.2.4/tests/cases/watch_wanted/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/cases/watch_wanted/main.sh` & `stepup-1.2.4/tests/cases/watch_wanted/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/conftest.py` & `stepup-1.2.4/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,10 +69,10 @@
             try:
                 yield result
             finally:
                 await result("join")
         await director
 
 
-@pytest.fixture
+@pytest.fixture()
 def path_tmp(tmpdir: str) -> Path:
     return Path(tmpdir)
```

### Comparing `stepup-1.2.3/tests/core_common.py` & `stepup-1.2.4/tests/core_common.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/echo_server_socket.py` & `stepup-1.2.4/tests/echo_server_socket.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/echo_server_stdio.py` & `stepup-1.2.4/tests/echo_server_stdio.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/test_assoc.py` & `stepup-1.2.4/tests/test_assoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 MAX_CASES = [(None, None), (1, 2), (2, 1), (2, None), (None, 2), (1, None), (None, 1)]
 MAX_CASES_SRC_MULTI = [case for case in MAX_CASES if case[1] != 1]
 MAX_CASES_DST_MULTI = [case for case in MAX_CASES if case[0] != 1]
 MAX_CASES_MULTI = [case for case in MAX_CASES if case[0] != 1 and case[1] != 1]
 
 
-@pytest.mark.parametrize("dst_max, src_max", MAX_CASES)
+@pytest.mark.parametrize(("dst_max", "src_max"), MAX_CASES)
 def test_empty(dst_max, src_max):
     a = Assoc(dst_max, src_max)
     if dst_max is None:
         assert a._max is None
     else:
         assert a._max == dst_max
     if src_max is None:
@@ -46,15 +46,15 @@
     assert len(a) == 0
     assert list(a.inverse.items()) == []
     assert list(a.inverse.pairs()) == []
     assert list(a.inverse.keys()) == []
     assert len(a.inverse) == 0
 
 
-@pytest.mark.parametrize("dst_max, src_max", MAX_CASES)
+@pytest.mark.parametrize(("dst_max", "src_max"), MAX_CASES)
 @pytest.mark.parametrize("discard", ["pair", "all", "inverse_all"])
 def test_modify_1(dst_max, src_max, discard):
     a = Assoc(dst_max, src_max)
     a.add(1, "a")
     a[2] = "b"
     with pytest.raises(KeyError):
         _ = a[3]
@@ -112,15 +112,15 @@
         assert list(a.inverse.items()) == [("b", 2)]
     else:
         assert list(a.inverse.items()) == [("b", {2})]
     assert list(a.inverse.keys()) == ["b"]
     assert len(a.inverse) == 1
 
 
-@pytest.mark.parametrize("dst_max, src_max", MAX_CASES_DST_MULTI)
+@pytest.mark.parametrize(("dst_max", "src_max"), MAX_CASES_DST_MULTI)
 def test_modify_2_dst(dst_max, src_max):
     a = Assoc(dst_max, src_max)
     a.add(1, "a")
     a.add(2, "b")
     a.add(1, "a+")
     assert 1 in a
     assert 3 not in a
@@ -170,15 +170,15 @@
                 ("b", {2}),
                 ("c", {1}),
                 ("d", {1}),
                 ("e", {1}),
             ]
 
 
-@pytest.mark.parametrize("dst_max, src_max", MAX_CASES_SRC_MULTI)
+@pytest.mark.parametrize(("dst_max", "src_max"), MAX_CASES_SRC_MULTI)
 def test_modify_2_src(dst_max, src_max):
     a = Assoc(dst_max, src_max)
     a.add(1, "a")
     a.add(1, "a")
     a.add(2, "b")
     a.add(3, "a")
     if dst_max == 1:
@@ -191,15 +191,15 @@
     assert list(a.keys()) == [1, 2, 3]
     assert len(a) == 3
     assert list(a.inverse.items()) == [("a", {1, 3}), ("b", {2})]
     assert list(a.inverse.keys()) == ["a", "b"]
     assert len(a.inverse) == 2
 
 
-@pytest.mark.parametrize("dst_max, src_max", MAX_CASES_MULTI)
+@pytest.mark.parametrize(("dst_max", "src_max"), MAX_CASES_MULTI)
 def test_modify_2_dst_src(dst_max, src_max):
     a = Assoc(dst_max, src_max)
     a.add(1, "a")
     a.add(2, "b")
     a.add(3, "a")
     a.add(1, "c")
     a.add(1, "c")
```

### Comparing `stepup-1.2.3/tests/test_basics.py` & `stepup-1.2.4/tests/test_basics.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,31 +24,31 @@
 import pytest
 from path import Path
 
 from stepup.core.exceptions import RPCError
 from stepup.core.rpc import AsyncRPCClient
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_unknown_instruction(client: AsyncRPCClient):
     with open("DONE.txt", "w") as fh:
         fh.write("done")
     with pytest.raises(RPCError):
         await client("instruction_that_does_not_exist")
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_missing_argument(client: AsyncRPCClient):
     with open("DONE.txt", "w") as fh:
         fh.write("done")
     with pytest.raises(RPCError):
         await client("static")
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_wrong_type(client: AsyncRPCClient):
     with open("DONE.txt", "w") as fh:
         fh.write("done")
     with pytest.raises(RPCError):
         await client("static", 5)
 
 
@@ -87,15 +87,15 @@
 def _check_graph(path, expected):
     with open(path) as fh:
         cur = fh.read()
         cur = re.sub(r" {10}(inp_| {4})digest = [ 0-9a-f]{71}\n {21}= [ 0-9a-f]{71}\n", "", cur)
         assert cur == expected
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_from_scratch(client: AsyncRPCClient, tmpdir: str):
     with open("DONE.txt", "w") as fh:
         fh.write("done")
     await client("wait")
     prefix_graph = Path(tmpdir) / "graph"
     await client("graph", prefix_graph)
     _check_graph(prefix_graph + ".txt", FROM_SCRATCH_GRAPH)
@@ -137,15 +137,15 @@
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
 
 """
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_static(client: AsyncRPCClient, tmpdir: str):
     try:
         with open("foo", "w") as fh:
             fh.write("bar")
         step_key_plan = "step:./plan.py"
         await client("static", step_key_plan, ["foo"])
     finally:
@@ -214,15 +214,15 @@
           created by   step:cp -v original.txt copy.txt
             consumes   file:./
             consumes   step:cp -v original.txt copy.txt
 
 """
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_copy(client: AsyncRPCClient, tmpdir: str):
     try:
         with open("original.txt", "w") as fh:
             fh.write("Hello world!")
         step_key_plan = "step:./plan.py"
         step_key_copy = await client(
             "step",
```

### Comparing `stepup-1.2.3/tests/test_cascade.py` & `stepup-1.2.4/tests/test_cascade.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/test_cases.py` & `stepup-1.2.4/tests/test_cases.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     "name",
     [
         "amend",
         "amend_delay",
         "amend_env_vars",
         "amend_missing",
         "amend_outdir_pending",
+        "amend_self_static",
         "amend_voldir_pending",
         "deferred_glob1",
         "deferred_glob2",
         "deferred_subdir",
         "env_vars",
         "env_vars_amend",
         "env_vars_path",
@@ -67,14 +68,15 @@
         "pending",
         "permissions_file_rerun",
         "permissions_plan_rerun",
         "permissions_plan_restart",
         "permissions_step_rerun",
         "permissions_step_restart",
         "pool",
+        "pool_restart",
         "restart_blocked",
         "restart_changes",
         "restart_deferred_glob",
         "restart_nochanges",
         "restart_outdated_amend",
         "restart_output",
         "restart_orphan",
@@ -84,14 +86,15 @@
         "script_single",
         "static",
         "static_abs",
         "static_dir",
         "static_glob",
         "static_nglob",
         "static_nglob_partial",
+        "static_nglob_recursive",
         "static_nglob_subdir",
         "subdir",
         "watch_blocked",
         "watch_boot",
         "watch_chain",
         "watch_input",
         "watch_middle",
@@ -99,10 +102,10 @@
         "watch_nochanges",
         "watch_outdated_amend1",
         "watch_outdated_amend2",
         "watch_output",
         "watch_wanted",
     ],
 )
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_example(tmpdir, name: str):
     await run_example(Path("tests/cases") / name, tmpdir, OVERWRITE_EXPECTED)
```

### Comparing `stepup-1.2.3/tests/test_hash.py` & `stepup-1.2.4/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/test_nglob.py` & `stepup-1.2.4/tests/test_nglob.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,26 +49,28 @@
 
 
 @pytest.mark.parametrize("pattern", ["[aaa", "blub"])
 def test_has_wildcards_false(pattern):
     assert not has_wildcards(pattern)
 
 
-@pytest.mark.parametrize("pattern", ["foo*", "*", "?", "**", "ls/ff**f/", "num[0-9]"])
+@pytest.mark.parametrize(
+    "pattern", ["foo*", "*", "?", "**", "ls/ff**f/", "./**/help.txt", "num[0-9]"]
+)
 def test_has_anonymous_wildcards_true(pattern):
     assert has_anonymous_wildcards(pattern)
 
 
 @pytest.mark.parametrize("pattern", ["bar_${*foo}", "[aaa", "blub"])
 def test_has_anonymous_wildcards_false(pattern):
     assert not has_anonymous_wildcards(pattern)
 
 
 @pytest.mark.parametrize(
-    "pattern, names",
+    ("pattern", "names"),
     [
         ("bar_${*foo}", ["foo"]),
         ("bar_*foo", []),
         ("{*bar}_$*foo", []),
         ("${*bar}_${*foo}", ["bar", "foo"]),
     ],
 )
@@ -176,30 +178,30 @@
     assert ngs.results == {(): set(paths)}
     lookup = lookupdict()
     data = msgpack.packb(ngs.unstructure(lookup))
     assert ngs == NGlobSingle.structure(msgpack.unpackb(data), lookup.get_list())
 
 
 @pytest.mark.parametrize(
-    "patterns, subs",
+    ("patterns", "subs"),
     [
         (["inp*.txt"], {}),
         (["${*inp}.txt"], {}),
         (["${*inp}.txt"], {"inp": "???"}),
         (["${*inp}.txt", "*.out"], {"inp": "foo"}),
         (["${*inp}.txt", "${*out}.txt"], {"inp": "foo"}),
     ],
 )
 def test_nglob_multi_has_wildcards_true(patterns, subs):
     ngs = tuple(NGlobSingle(pattern, subs) for pattern in patterns)
     assert NGlobMulti(ngs).has_wildcards
 
 
 @pytest.mark.parametrize(
-    "patterns, subs",
+    ("patterns", "subs"),
     [
         (["inp.txt"], {}),
         (["${inp}.txt"], {}),
         (["${*inp}.txt"], {"inp": "foo"}),
         (["inp.txt", "${*out}.txt"], {"out": "bar"}),
     ],
 )
@@ -328,83 +330,94 @@
     assert not ngm.will_change(set(), {"thi.txt"})
     assert not ngm.will_change(set(), {"thi_x.pdf"})
     assert ngm.will_change(set(), {"thi.txt", "thi_x.pdf"})
     assert not ngm.will_change(set(), {"k.loog"})
 
 
 @pytest.mark.parametrize(
-    "string, matches",
+    ("string", "matches"),
     [
         ("foo*", ["*"]),
-        ("foo**", ["**"]),
+        ("foo**", ["*", "*"]),
         ("foo${*bar}", ["${*bar}"]),
         ("*foo${*bar}", ["*", "${*bar}"]),
-        ("***foo${*bar}", ["**", "*", "${*bar}"]),
-        ("**spam*foo${*bar}", ["**", "*", "${*bar}"]),
-        ("*spam**foo${*bar}", ["*", "**", "${*bar}"]),
-        ("*${*spam}**foo${*bar}", ["*", "${*spam}", "**", "${*bar}"]),
+        ("***foo${*bar}", ["*", "*", "*", "${*bar}"]),
+        ("**spam*foo${*bar}", ["*", "*", "*", "${*bar}"]),
+        ("*spam**foo${*bar}", ["*", "*", "*", "${*bar}"]),
+        ("*${*spam}**foo${*bar}", ["*", "${*spam}", "*", "*", "${*bar}"]),
         ("*foo?", ["*", "?"]),
         ("?foo??", ["?", "?", "?"]),
         ("?foo[ab]?", ["?", "[ab]", "?"]),
         ("?foo[a-z][0-9][^?][?]?", ["?", "[a-z]", "[0-9]", "[^?]", "[?]", "?"]),
         ("foo[?]", ["[?]"]),
         ("foo[*]", ["[*]"]),
         ("foo[${*ab}]", ["[${*ab}]"]),
         ("foo[[]a]", ["[[]"]),
+        ("**/", ["**"]),
+        ("/**", ["**"]),
+        ("**", ["**"]),
+        ("./**/*.txt", ["**", "*"]),
     ],
 )
 def test_nglob_wild(string, matches):
     assert re.findall(RE_NAMED_WILD, string) == matches
 
 
 @pytest.mark.parametrize(
-    "pattern, normal",
+    ("pattern", "normal"),
     [
         ("generic/${*ch}/*.md", "generic/*/*.md"),
         ("generic/*${*ch}/*.md", "generic/*/*.md"),
         ("generic/${*ch}*/*.md", "generic/*/*.md"),
         ("generic/*${*ch}*/*.md", "generic/*/*.md"),
-        ("generic/*${*ch}**/*.md", "generic/**/*.md"),
-        ("generic/**${*ch}*/*.md", "generic/**/*.md"),
-        ("generic/**${*ch}**/*.md", "generic/**/*.md"),
+        ("generic/*${*ch}**/*.md", "generic/*/*.md"),
+        ("generic/**${*ch}*/*.md", "generic/*/*.md"),
+        ("generic/**${*ch}**/*.md", "generic/*/*.md"),
         ("generic/${*ch}${*foo}/*.md", "generic/*/*.md"),
         ("generic/${*ch}-${*foo}/*.md", "generic/*-*/*.md"),
         ("generic/${*ch}/${*foo}/*.md", "generic/*/*/*.md"),
         ("${*generic}/ch${*foo}/*.md", "*/ch*/*.md"),
         ("generic/ch${*foo}/${*md}", "generic/ch*/*"),
         ("generic/${*md}${*ch}/${*md}", "generic/*/*"),
         ("generic/${*md}?/${*md}", "generic/*/*"),
-        ("generic/**?/?${*md}", "generic/**/*"),
-        ("generic/?**/*?", "generic/**/*"),
+        ("generic/**?/?${*md}", "generic/*/*"),
+        ("generic/?**/*?", "generic/*/*"),
+        ("generic/**/*?", "generic/**/*"),
         ("generic/${*md}[a[b]/?[*]", "generic/*[a[b]/?[*]"),
+        ("**/${*name}.txt", "**/*.txt"),
+        ("foo/**/${*name}.txt", "foo/**/*.txt"),
+        ("${*sub}/**", "*/**"),
+        ("${*sub}/**/", "*/**/"),
+        ("data**", "data*"),
     ],
 )
 def test_nglob_to_glob(pattern, normal):
     assert convert_nglob_to_glob(pattern) == normal
 
 
 @pytest.mark.parametrize(
-    "pattern, subs, normal",
+    ("pattern", "subs", "normal"),
     [
         (
             "${*generic}/${*ch}/*.md",
             {"generic": "?[ab]*", "ch": "s_*_*"},
             "?[ab]*/s_*_*/*.md",
         ),
         ("${*a}${*b}/ab", {"a": "a*"}, "a*/ab"),
         ("${*a}${*b}/ab", {"a": "a*", "b": "?b"}, "a*b/ab"),
-        ("${*a}${*b}${*a}/ab", {"a": "?a*", "b": "**b*"}, "?a**b*a*/ab"),
+        ("${*a}${*b}${*a}/ab", {"a": "?a*", "b": "**b*"}, "?a*b*a*/ab"),
+        ("${*a}/ab", {"a": "**/*a"}, "**/*a/ab"),
     ],
 )
 def test_nglob_to_glob_subs(pattern, subs, normal):
     assert convert_nglob_to_glob(pattern, subs) == normal
 
 
 @pytest.mark.parametrize(
-    "pattern, regex",
+    ("pattern", "regex"),
     [
         ("generic/${*ch}/*.md", r"generic/(?P<ch>[^/]*)/[^/]*\.md"),
         ("generic/${*ch}/?.md", r"generic/(?P<ch>[^/]*)/[^/]\.md"),
         ("generic/${*ch}/[abc].md", r"generic/(?P<ch>[^/]*)/[abc]\.md"),
         ("generic/${*ch}/[!abc].md", r"generic/(?P<ch>[^/]*)/[^abc]\.md"),
         (
             "generic/${*ch}${*foo}/*.md",
@@ -416,64 +429,68 @@
         ),
         (
             "generic/${*ch}/${*foo}/*.md",
             r"generic/(?P<ch>[^/]*)/(?P<foo>[^/]*)/[^/]*\.md",
         ),
         (
             "generic/${*ch}**${*foo}/*.md",
-            r"generic/(?P<ch>[^/]*).*(?P<foo>[^/]*)/[^/]*\.md",
+            r"generic/(?P<ch>[^/]*)[^/]*(?P<foo>[^/]*)/[^/]*\.md",
         ),
         (
             "generic/${*ch}**/${*foo}/*.md",
-            r"generic/(?P<ch>[^/]*).*/(?P<foo>[^/]*)/[^/]*\.md",
+            r"generic/(?P<ch>[^/]*)[^/]*/(?P<foo>[^/]*)/[^/]*\.md",
         ),
         (
             "${*generic}/ch${*foo}/*.md",
             r"(?P<generic>[^/]*)/ch(?P<foo>[^/]*)/[^/]*\.md",
         ),
         ("generic/ch${*foo}/${*md}", r"generic/ch(?P<foo>[^/]*)/(?P<md>[^/]*)"),
         ("generic/${*md}${*ch}/${*md}", "generic/(?P<md>[^/]*)(?P<ch>[^/]*)/(?P=md)"),
+        ("data**", "data[^/]*"),
     ],
 )
 def test_nglob_to_regex(pattern, regex):
     assert convert_nglob_to_regex(pattern) == regex
 
 
 @pytest.mark.parametrize(
-    "pattern, subs, regex",
+    ("pattern", "subs", "regex"),
     [
         (
             "prefix_${*year}",
             {"year": "[0-9][0-9][0-9][0-9]"},
             r"prefix_(?P<year>[0-9][0-9][0-9][0-9])",
         ),
         (
             "latex-${*name}/${*name}.tex",
             {"name": "?*"},
-            r"latex\-(?P<name>[^/][^/]*)/(?P=name)\.tex",
+            r"latex\-(?P<name>[^/]*)/(?P=name)\.tex",
         ),
     ],
 )
 def test_nglob_to_regex_subs(pattern, subs, regex):
     assert convert_nglob_to_regex(pattern, subs) == regex
 
 
 def test_nglob_to_regex_groups():
-    regex = re.compile(convert_nglob_to_regex("generic/${*ch}**/${*foo}/*.md"))
+    regex = re.compile(convert_nglob_to_regex("generic/${*ch}/**/${*foo}/*.md"))
     match_ = regex.fullmatch("generic/ch1/some/some/name/file.md")
     assert match_.groups() == ("ch1", "name")
 
 
 def _make_files(paths: Collection[str]):
     for path in paths:
         path = Path(path)
-        if len(path.parent) > 0:
-            path.parent.makedirs_p()
-        with open(path, "w"):
-            pass
+        if path.endswith("/"):
+            path.makedirs_p()
+        else:
+            if len(path.parent) > 0:
+                path.parent.makedirs_p()
+            with open(path, "w"):
+                pass
 
 
 def _check_ngm_multi(tmpdir, patterns, subs, paths, used_names, results):
     ngm1 = NGlobMulti.from_patterns(patterns, subs)
     assert ngm1.used_names == used_names
     assert ngm1.subs == subs
     assert ngm1.has_wildcards
@@ -589,14 +606,80 @@
     results = {
         ("a", "egg"): [{"a/foo.txt"}, {"other/egg.txt"}],
         ("b", "egg"): [{"b/foo.txt"}, {"other/egg.txt"}],
     }
     _check_ngm_multi(tmpdir, patterns, subs, paths, used_names, results)
 
 
+def test_recursive1(tmpdir):
+    _check_ngm_multi(
+        tmpdir,
+        patterns=["data/**"],
+        subs={},
+        paths=["data/", "data/sub/", "data/sub/part1.txt", "data/part2.txt"],
+        used_names=(),
+        results={(): [{"data/", "data/sub/", "data/sub/part1.txt", "data/part2.txt"}]},
+    )
+
+
+def test_recursive2(tmpdir):
+    _check_ngm_multi(
+        tmpdir,
+        patterns=["data**"],
+        subs={},
+        paths=["data/", "data/sub/", "data/sub/part1.txt", "data/part2.txt"],
+        used_names=(),
+        results={},
+    )
+
+
+def test_recursive3(tmpdir):
+    _check_ngm_multi(
+        tmpdir,
+        patterns=["data**/"],
+        subs={},
+        paths=["data/", "data/sub/", "data/sub/part1.txt", "data/part2.txt"],
+        used_names=(),
+        results={(): [{"data/"}]},
+    )
+
+
+def test_recursive4(tmpdir):
+    _check_ngm_multi(
+        tmpdir,
+        patterns=["**.txt"],
+        subs={},
+        paths=["data/", "data/sub/", "data/sub/part1.txt", "data/part2.txt"],
+        used_names=(),
+        results={},
+    )
+
+
+def test_recursive5(tmpdir):
+    _check_ngm_multi(
+        tmpdir,
+        patterns=["**/*.txt"],
+        subs={},
+        paths=["data/", "data/sub/", "data/sub/part1.txt", "data/part2.txt"],
+        used_names=(),
+        results={(): [{"data/sub/part1.txt", "data/part2.txt"}]},
+    )
+
+
+def test_hidden(tmpdir):
+    _check_ngm_multi(
+        tmpdir,
+        patterns=["*.txt"],
+        subs={},
+        paths=["visible.txt", ".hidden.txt"],
+        used_names=(),
+        results={(): [{"visible.txt", ".hidden.txt"}]},
+    )
+
+
 def test_may_match():
     patterns = ["subdir*/", "foo*.txt"]
     ngm = NGlobMulti.from_patterns(patterns)
     assert not ngm.may_match("subdir/foo.txt")
     assert not ngm.may_match("foo.log")
     assert ngm.may_match("subdir1/")
     assert ngm.may_match("foo1.txt")
```

### Comparing `stepup-1.2.3/tests/test_rpc.py` & `stepup-1.2.4/tests/test_rpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,40 +78,40 @@
 
 @pytest_asyncio.fixture()
 async def sc(socket_server_path):
     async with await AsyncRPCClient.socket(socket_server_path) as client:
         yield client
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_pipe_simple_args(pc):
     assert await pc.call.echo("hello") == "pipe: hello"
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_stdio_simple_args(ic):
     assert await ic.call.echo("hello") == "stdio: hello"
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_socket_simple_args(sc):
     assert await sc.call.echo("hello") == "socket: hello"
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_pipe_simple_kwargs(pc):
     assert await pc.call.echo(msg="hello") == "pipe: hello"
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_stdio_simple_kwargs(ic):
     assert await ic.call.echo(msg="hello") == "stdio: hello"
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_socket_simple_kwargs(sc):
     assert await sc.call.echo(msg="hello") == "socket: hello"
 
 
 LCG_CASES = [
     ((1, 71, 45, 91), {}, 65),
     ((1, 71, 45), {}, 65),
@@ -119,87 +119,87 @@
     ((1,), {}, 65),
     ((1,), {"multiplier": 45}, 65),
     ((1, 71, 32), {}, 52),
     ((1,), {"multiplier": 32}, 52),
 ]
 
 
-@pytest.mark.asyncio
-@pytest.mark.parametrize("args, kwargs, result", LCG_CASES)
+@pytest.mark.asyncio()
+@pytest.mark.parametrize(("args", "kwargs", "result"), LCG_CASES)
 async def test_pipe_lcg_kwargs(pc, args, kwargs, result):
     assert await pc.call.lcg(*args, **kwargs) == result
 
 
-@pytest.mark.asyncio
-@pytest.mark.parametrize("args, kwargs, result", LCG_CASES)
+@pytest.mark.asyncio()
+@pytest.mark.parametrize(("args", "kwargs", "result"), LCG_CASES)
 async def test_stdio_lcg_kwargs(ic, args, kwargs, result):
     assert await ic.call.lcg(*args, **kwargs) == result
 
 
-@pytest.mark.asyncio
-@pytest.mark.parametrize("args, kwargs, result", LCG_CASES)
+@pytest.mark.asyncio()
+@pytest.mark.parametrize(("args", "kwargs", "result"), LCG_CASES)
 async def test_socket_lcg_kwargs(sc, args, kwargs, result):
     assert await sc.call.lcg(*args, **kwargs) == result
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_pipe_seq(pc):
     assert await pc.call.echo("hello", 0.1) == "pipe: hello"
     assert await pc.call.echo("world") == "pipe: world"
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_stdio_seq(ic):
     assert await ic.call.echo("hello", 0.1) == "stdio: hello"
     assert await ic.call.echo("world") == "stdio: world"
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_socket_seq(sc):
     assert await sc.call.echo("hello", 0.1) == "socket: hello"
     assert await sc.call.echo("world") == "socket: world"
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_pipe_par1(pc):
     expected = ["pipe: hello", "pipe: world"]
     assert await asyncio.gather(pc.call.echo("hello", 0.1), pc.call.echo("world")) == expected
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_stdio_par1(ic):
     expected = ["stdio: hello", "stdio: world"]
     assert await asyncio.gather(ic.call.echo("hello", 0.1), ic.call.echo("world")) == expected
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_socket_par1(sc):
     expected = ["socket: hello", "socket: world"]
     assert await asyncio.gather(sc.call.echo("hello", 0.1), sc.call.echo("world")) == expected
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_pipe_par2(pc):
     expected = ["pipe: hello", "pipe: world"]
     assert await asyncio.gather(pc.call.echo("hello"), pc.call.echo("world", 0.1)) == expected
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_stdio_par2(ic):
     expected = ["stdio: hello", "stdio: world"]
     assert await asyncio.gather(ic.call.echo("hello"), ic.call.echo("world", 0.1)) == expected
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_socket_par2(sc):
     expected = ["socket: hello", "socket: world"]
     assert await asyncio.gather(sc.call.echo("hello"), sc.call.echo("world", 0.1)) == expected
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_socket_multi_clients(socket_server_path):
     r1, w1 = await asyncio.open_unix_connection(socket_server_path)
     async with AsyncRPCClient(r1, w1) as c1:
         r2, w2 = await asyncio.open_unix_connection(socket_server_path)
         async with AsyncRPCClient(r2, w2) as c2:
             assert await c1.call.echo("hello", 0.1) == "socket: hello"
             assert await c2.call.echo("world") == "socket: world"
@@ -216,15 +216,15 @@
         assert client.call.echo("world", _rpc_timeout=5) == "socket: world"
         assert client.call.lcg(1, multiplier=32, _rpc_timeout=5) == 52
         with pytest.raises(TimeoutError):
             client.call.echo("hello", delay=0.5, _rpc_timeout=0.1)
 
 
 @pytest.mark.parametrize(
-    "name, args, kwargs, result",
+    ("name", "args", "kwargs", "result"),
     [
         ("foo", ["gg", 1], {}, "foo('gg', 1)"),
         ("bar", [], {"a": 1, "b": [3, 4, "qq"]}, "bar(a=1, b=[3, 4, 'qq'])"),
         ("none", [], {}, "none()"),
         ("mixed", [()], {"_q": 5}, "mixed((), _q=5)"),
     ],
 )
@@ -232,17 +232,17 @@
     assert fmt_rpc_call(name, args, kwargs) == result
 
 
 def test_fmt_rpc_call_noargs():
     assert fmt_rpc_call("foo", [], {}) == "foo()"
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_pipe_not_allowed(pc):
     with pytest.raises(RPCError):
         assert await pc.call.not_allowed()
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 async def test_pipe_not_defined(pc):
     with pytest.raises(RPCError):
         assert await pc.call.not_defined()
```

### Comparing `stepup-1.2.3/tests/test_scheduler.py` & `stepup-1.2.4/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.3/tests/test_utils.py` & `stepup-1.2.4/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     mynormpath,
     myparent,
     myrelpath,
 )
 
 
 @pytest.mark.parametrize(
-    "inp, out",
+    ("inp", "out"),
     [
         ("./foo", "foo"),
         ("./dir/", "dir/"),
         (".", "."),
         ("./", "./"),
         ("/foo/", "/foo/"),
         ("/foo", "/foo"),
@@ -48,15 +48,15 @@
     ],
 )
 def test_mynormpath(inp: str, out: str):
     assert mynormpath(inp) == out
 
 
 @pytest.mark.parametrize(
-    "inp, start, out",
+    ("inp", "start", "out"),
     [
         ("/foo/bar/", "/foo", "bar/"),
         ("/foo/bar", "/foo", "bar"),
         ("/foo/sub/../extra/some", "/foo/bar", "../extra/some"),
         ("/foo/sub/../extra/some/", "/foo/bar", "../extra/some/"),
     ],
 )
@@ -78,15 +78,15 @@
     assert myabsolute(inp, is_dir=True).endswith("/")
     if inp.endswith("/"):
         assert myabsolute(inp).endswith("/")
     assert myabsolute(inp).normpath() == Path(inp).absolute()
 
 
 @pytest.mark.parametrize(
-    "inp, out",
+    ("inp", "out"),
     [
         ("foo/bar", "foo/"),
         ("foo/bar/", "foo/"),
         ("foo/bar/egg.txt", "foo/bar/"),
         ("foo/", "./"),
         ("foo", "./"),
         (".", None),
```

### Comparing `stepup-1.2.3/tests/test_workflow.py` & `stepup-1.2.4/tests/test_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,21 +42,21 @@
     for step in workflow.get_steps():
         if step.get_state(workflow) == StepState.SUCCEEDED:
             assert step._hash is not None
             assert step._recording is not None
     return workflow
 
 
-@pytest.fixture
+@pytest.fixture()
 def wfs() -> Workflow:
     """A workflow from scratch, no plan.py"""
     return Workflow.from_scratch()
 
 
-@pytest.fixture
+@pytest.fixture()
 def wfp() -> Workflow:
     """A workflow with a boots step plan.py"""
     workflow = Workflow.from_scratch()
     workflow.declare_static("root:", ["plan.py", "./"])
     workflow.define_step("root:", "./plan.py", ["plan.py"])
     assert list(workflow.nodes) == ["root:", "vacuum:", "file:./", "file:plan.py", "step:./plan.py"]
     return workflow
@@ -1228,15 +1228,14 @@
 
 
 def test_cyclic_two_steps(wfp):
     plan_key = "step:./plan.py"
     wfp.define_step(plan_key, "cat first > second", inp_paths=["first"], out_paths=["second"])
     with pytest.raises(GraphError):
         wfp.define_step(plan_key, "cat second > first", inp_paths=["second"], out_paths=["first"])
-    assert wfp.is_orphan("file:first")
 
 
 def test_optional_imply(wfp):
     # Define sequence of steps: optional -> mandatory
     plan_key = "step:./plan.py"
     step1_key = wfp.define_step(plan_key, "prog1", out_paths=["foo"], optional=True)
     step1 = wfp.get_step(step1_key)
@@ -1628,7 +1627,17 @@
     plan_key = "step:./plan.py"
     step_key = wfp.define_step(plan_key, "script", out_paths=["sub/"])
     wfp.amend_step(step_key, out_paths=["sub/foo/"], vol_paths=["sub/foo/bar"])
     step = wfp.get_step(step_key)
     assert step.get_inp_paths(wfp) == ["./"]
     assert step.get_out_paths(wfp) == ["sub/", "sub/foo/"]
     assert step.get_vol_paths(wfp) == ["sub/foo/bar"]
+
+
+def test_set_pool(wfp):
+    plan_key = "step:./plan.py"
+    wfp.set_pool(plan_key, "random", 2)
+    plan = wfp.get_step(plan_key)
+    assert plan.defined_pools == {"random": 2}
+    plan.update_recording(wfp)
+    assert plan.recording.defined_pools == {"random": 2}
+    check_workflow_unstructure(wfp)
```

