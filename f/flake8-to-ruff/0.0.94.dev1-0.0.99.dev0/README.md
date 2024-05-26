# Comparing `tmp/flake8_to_ruff-0.0.94_dev.1.tar.gz` & `tmp/flake8_to_ruff-0.0.99_dev.0.tar.gz`

## Comparing `flake8_to_ruff-0.0.94_dev.1.tar` & `flake8_to_ruff-0.0.99_dev.0.tar`

### file list

```diff
@@ -1,451 +1,460 @@
--rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/Cargo.toml
--rw-r--r--   0      501       20      278 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/.editorconfig
--rw-r--r--   0      501       20     3612 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/.github/workflows/ci.yaml
--rw-r--r--   0      501       20     8967 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/.github/workflows/flake8-to-ruff.yaml
--rw-r--r--   0      501       20     8618 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/.github/workflows/ruff.yaml
--rw-r--r--   0      501       20     3407 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/.gitignore
--rw-r--r--   0      501       20      231 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/.pre-commit-config.yaml
--rw-r--r--   0      501       20     5227 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/CODE_OF_CONDUCT.md
--rw-r--r--   0      501       20     4582 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/CONTRIBUTING.md
--rw-r--r--   0      501       20    82250 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/Cargo.lock
--rw-r--r--   0      501       20     1070 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/LICENSE
--rw-r--r--   0      501       20    34329 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/README.md
--rw-r--r--   0      501       20      475 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/benches/source_code_locator.rs
--rw-r--r--   0      501       20     3261 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/examples/generate_check_code_prefix.rs
--rw-r--r--   0      501       20      942 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/examples/generate_rules_table.rs
--rw-r--r--   0      501       20      568 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/examples/generate_source_code.rs
--rw-r--r--   0      501       20      477 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/examples/print_ast.rs
--rw-r--r--   0      501       20      470 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/examples/print_tokens.rs
--rw-r--r--   0      501       20     1100 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/pyproject.toml
--rw-r--r--   0      501       20      368 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/A001.py
--rw-r--r--   0      501       20      130 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/A002.py
--rw-r--r--   0      501       20      127 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/A003.py
--rw-r--r--   0      501       20      223 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/B002.py
--rw-r--r--   0      501       20     3342 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/B006_B008.py
--rw-r--r--   0      501       20      716 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/B007.py
--rw-r--r--   0      501       20      133 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/B011.py
--rw-r--r--   0      501       20      119 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/B013.py
--rw-r--r--   0      501       20     1364 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/B014.py
--rw-r--r--   0      501       20      829 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/B017.py
--rw-r--r--   0      501       20      446 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/B025.py
--rw-r--r--   0      501       20       30 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/C400.py
--rw-r--r--   0      501       20       29 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/C401.py
--rw-r--r--   0      501       20       69 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/C402.py
--rw-r--r--   0      501       20       31 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/C403.py
--rw-r--r--   0      501       20       71 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/C404.py
--rw-r--r--   0      501       20       71 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/C405.py
--rw-r--r--   0      501       20       81 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/C406.py
--rw-r--r--   0      501       20       66 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/C408.py
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/C409.py
--rw-r--r--   0      501       20       64 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/C410.py
--rw-r--r--   0      501       20       35 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/C411.py
--rw-r--r--   0      501       20       84 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/C413.py
--rw-r--r--   0      501       20      216 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/C414.py
--rw-r--r--   0      501       20      193 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/C415.py
--rw-r--r--   0      501       20       95 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/C416.py
--rw-r--r--   0      501       20      179 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/C417.py
--rw-r--r--   0      501       20    12157 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/D.py
--rw-r--r--   0      501       20      294 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E402.py
--rw-r--r--   0      501       20      786 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E501.py
--rw-r--r--   0      501       20      648 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E711.py
--rw-r--r--   0      501       20      653 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E712.py
--rw-r--r--   0      501       20      540 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E713.py
--rw-r--r--   0      501       20      508 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E714.py
--rw-r--r--   0      501       20      907 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E721.py
--rw-r--r--   0      501       20      327 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E722.py
--rw-r--r--   0      501       20      252 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E731.py
--rw-r--r--   0      501       20      676 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E741.py
--rw-r--r--   0      501       20       78 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E742.py
--rw-r--r--   0      501       20       99 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E743.py
--rw-r--r--   0      501       20       10 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E999.py
--rw-r--r--   0      501       20     1549 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F401_0.py
--rw-r--r--   0      501       20      121 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F401_1.py
--rw-r--r--   0      501       20      242 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F401_2.py
--rw-r--r--   0      501       20      302 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F401_3.py
--rw-r--r--   0      501       20      315 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F401_4.py
--rw-r--r--   0      501       20      126 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F401_5.py
--rw-r--r--   0      501       20       96 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F402.py
--rw-r--r--   0      501       20      152 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F403.py
--rw-r--r--   0      501       20      130 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F404.py
--rw-r--r--   0      501       20      116 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F405.py
--rw-r--r--   0      501       20       87 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F406.py
--rw-r--r--   0      501       20       82 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F407.py
--rw-r--r--   0      501       20      112 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F541.py
--rw-r--r--   0      501       20      144 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F601.py
--rw-r--r--   0      501       20       50 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F602.py
--rw-r--r--   0      501       20       64 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F622.py
--rw-r--r--   0      501       20       58 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F631.py
--rw-r--r--   0      501       20       51 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F632.py
--rw-r--r--   0      501       20       79 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F633.py
--rw-r--r--   0      501       20      122 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F634.py
--rw-r--r--   0      501       20      179 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F701.py
--rw-r--r--   0      501       20      200 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F702.py
--rw-r--r--   0      501       20       76 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F704.py
--rw-r--r--   0      501       20       66 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F706.py
--rw-r--r--   0      501       20      380 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F707.py
--rw-r--r--   0      501       20       74 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F722.py
--rw-r--r--   0      501       20     2196 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F821_0.py
--rw-r--r--   0      501       20      395 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F821_1.py
--rw-r--r--   0      501       20       28 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F822.py
--rw-r--r--   0      501       20      245 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F823.py
--rw-r--r--   0      501       20      159 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F831.py
--rw-r--r--   0      501       20      343 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F841.py
--rw-r--r--   0      501       20       88 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F901.py
--rw-r--r--   0      501       20     1762 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/M001.py
--rw-r--r--   0      501       20      225 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/N801.py
--rw-r--r--   0      501       20      354 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/N802.py
--rw-r--r--   0      501       20       95 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/N803.py
--rw-r--r--   0      501       20      264 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/N804.py
--rw-r--r--   0      501       20      345 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/N805.py
--rw-r--r--   0      501       20       54 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/N806.py
--rw-r--r--   0      501       20      126 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/N807.py
--rw-r--r--   0      501       20      116 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/N811.py
--rw-r--r--   0      501       20      124 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/N812.py
--rw-r--r--   0      501       20      119 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/N813.py
--rw-r--r--   0      501       20      119 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/N814.py
--rw-r--r--   0      501       20       96 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/N815.py
--rw-r--r--   0      501       20       67 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/N816.py
--rw-r--r--   0      501       20       55 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/N817.py
--rw-r--r--   0      501       20      106 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/N818.py
--rw-r--r--   0      501       20       31 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/T201.py
--rw-r--r--   0      501       20      148 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/T203.py
--rw-r--r--   0      501       20      152 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/U001.py
--rw-r--r--   0      501       20      146 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/U002.py
--rw-r--r--   0      501       20       45 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/U003.py
--rw-r--r--   0      501       20      883 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/U004.py
--rw-r--r--   0      501       20      263 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/U005.py
--rw-r--r--   0      501       20      125 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/U006.py
--rw-r--r--   0      501       20      463 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/U007.py
--rw-r--r--   0      501       20     1483 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/U008.py
--rw-r--r--   0      501       20       26 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/W292_0.py
--rw-r--r--   0      501       20       40 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/W292_1.py
--rw-r--r--   0      501       20       27 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/W292_2.py
--rw-r--r--   0      501       20      316 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/W605.py
--rw-r--r--   0      501       20       54 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/__init__.py
--rw-r--r--   0      501       20        0 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/bar/__init__.py
--rw-r--r--   0      501       20        0 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/bar/migrations/__init__.py
--rw-r--r--   0      501       20       90 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/bar/migrations/migration.py
--rw-r--r--   0      501       20     4176 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/canonical_google_examples.py
--rw-r--r--   0      501       20     5315 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/canonical_numpy_examples.py
--rw-r--r--   0      501       20       90 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/directory/also_excluded.py
--rw-r--r--   0      501       20       90 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/excluded.py
--rw-r--r--   0      501       20      716 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_doubles.py
--rw-r--r--   0      501       20      290 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_doubles_class.py
--rw-r--r--   0      501       20      406 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_doubles_function.py
--rw-r--r--   0      501       20      133 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_doubles_module_multiline.py
--rw-r--r--   0      501       20      135 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_doubles_module_singleline.py
--rw-r--r--   0      501       20      772 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_singles.py
--rw-r--r--   0      501       20      290 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_singles_class.py
--rw-r--r--   0      501       20      408 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_singles_function.py
--rw-r--r--   0      501       20      133 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_singles_module_multiline.py
--rw-r--r--   0      501       20      135 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_singles_module_singleline.py
--rw-r--r--   0      501       20       93 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/doubles.py
--rw-r--r--   0      501       20      203 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/doubles_escaped.py
--rw-r--r--   0      501       20      165 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/doubles_multiline_string.py
--rw-r--r--   0      501       20       58 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/doubles_noqa.py
--rw-r--r--   0      501       20      106 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/doubles_wrapped.py
--rw-r--r--   0      501       20       93 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/singles.py
--rw-r--r--   0      501       20      203 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/singles_escaped.py
--rw-r--r--   0      501       20      165 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/singles_multiline_string.py
--rw-r--r--   0      501       20       58 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/singles_noqa.py
--rw-r--r--   0      501       20      106 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/singles_wrapped.py
--rw-r--r--   0      501       20        0 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/foo/__init__.py
--rw-r--r--   0      501       20        0 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/foo/migrations/__init__.py
--rw-r--r--   0      501       20       90 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/foo/migrations/migration.py
--rw-r--r--   0      501       20      444 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/future_annotations.py
--rw-r--r--   0      501       20      632 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/pyproject.toml
--rw-r--r--   0      501       20    12260 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/sections.py
--rw-r--r--   0      501       20       31 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/rust-toolchain.toml
--rw-r--r--   0      501       20      390 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/rustfmt.toml
--rw-r--r--   0      501       20      302 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/scripts/.flake8
--rw-r--r--   0      501       20    37365 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/scripts/poetry.lock
--rw-r--r--   0      501       20      454 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/scripts/pyproject.toml
--rwxr-xr-x   0      501       20     1035 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/scripts/run_flake8.py
--rw-r--r--   0      501       20      565 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/setup.py
--rw-r--r--   0      501       20     4422 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/ast/helpers.rs
--rw-r--r--   0      501       20       87 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/ast/mod.rs
--rw-r--r--   0      501       20     3881 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/ast/operations.rs
--rw-r--r--   0      501       20     4574 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/ast/relocate.rs
--rw-r--r--   0      501       20     2211 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/ast/types.rs
--rw-r--r--   0      501       20    18283 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/ast/visitor.rs
--rw-r--r--   0      501       20     6375 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/autofix/fixer.rs
--rw-r--r--   0      501       20     3383 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/autofix/helpers.rs
--rw-r--r--   0      501       20     1217 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/autofix/mod.rs
--rw-r--r--   0      501       20     4136 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/cache.rs
--rw-r--r--   0      501       20    96891 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/check_ast.rs
--rw-r--r--   0      501       20     9787 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/check_lines.rs
--rw-r--r--   0      501       20     1740 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/check_tokens.rs
--rw-r--r--   0      501       20    69184 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/checks.rs
--rw-r--r--   0      501       20    43059 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/checks_gen.rs
--rw-r--r--   0      501       20     5866 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/cli.rs
--rw-r--r--   0      501       20    36461 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/code_gen.rs
--rw-r--r--   0      501       20     1201 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/cst/helpers.rs
--rw-r--r--   0      501       20       17 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/cst/mod.rs
--rw-r--r--   0      501       20      404 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/docstrings/definition.rs
--rw-r--r--   0      501       20     2428 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/docstrings/extraction.rs
--rw-r--r--   0      501       20     1423 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/docstrings/google.rs
--rw-r--r--   0      501       20     1363 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/docstrings/helpers.rs
--rw-r--r--   0      501       20      122 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/docstrings/mod.rs
--rw-r--r--   0      501       20      908 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/docstrings/numpy.rs
--rw-r--r--   0      501       20     3140 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/docstrings/sections.rs
--rw-r--r--   0      501       20      797 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/docstrings/styles.rs
--rw-r--r--   0      501       20       17 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/mod.rs
--rw-r--r--   0      501       20     1973 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/plugins/assert_false.rs
--rw-r--r--   0      501       20      880 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/plugins/assert_raises_exception.rs
--rw-r--r--   0      501       20     4108 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/plugins/duplicate_exceptions.rs
--rw-r--r--   0      501       20      654 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/plugins/mod.rs
--rw-r--r--   0      501       20     2255 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/plugins/mutable_argument_default.rs
--rw-r--r--   0      501       20      822 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/plugins/redundant_tuple_in_exception_handler.rs
--rw-r--r--   0      501       20      597 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/plugins/unary_prefix_increment.rs
--rw-r--r--   0      501       20     2008 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/plugins/unused_loop_control_variable.rs
--rw-r--r--   0      501       20      759 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_builtins/checks.rs
--rw-r--r--   0      501       20       31 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_builtins/mod.rs
--rw-r--r--   0      501       20       70 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_builtins/types.rs
--rw-r--r--   0      501       20    12248 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_comprehensions/checks.rs
--rw-r--r--   0      501       20       16 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_comprehensions/mod.rs
--rw-r--r--   0      501       20     1068 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_print/checks.rs
--rw-r--r--   0      501       20       29 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_print/mod.rs
--rw-r--r--   0      501       20       49 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_print/plugins/mod.rs
--rw-r--r--   0      501       20     1554 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_print/plugins/print_call.rs
--rw-r--r--   0      501       20    10466 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/checks.rs
--rw-r--r--   0      501       20     3662 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/docstring_detection.rs
--rw-r--r--   0      501       20       63 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/mod.rs
--rw-r--r--   0      501       20     1370 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/settings.rs
--rw-r--r--   0      501       20      737 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles.py.snap
--rw-r--r--   0      501       20      331 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_class.py.snap
--rw-r--r--   0      501       20      737 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_function.py.snap
--rw-r--r--   0      501       20      329 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_module_multiline.py.snap
--rw-r--r--   0      501       20      330 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_module_singleline.py.snap
--rw-r--r--   0      501       20      447 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles.py.snap
--rw-r--r--   0      501       20      446 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles_class.py.snap
--rw-r--r--   0      501       20      318 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles_function.py.snap
--rw-r--r--   0      501       20      190 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles_module_multiline.py.snap
--rw-r--r--   0      501       20      191 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles_module_singleline.py.snap
--rw-r--r--   0      501       20      326 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles.py.snap
--rw-r--r--   0      501       20      178 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles_escaped.py.snap
--rw-r--r--   0      501       20      197 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles_multiline_string.py.snap
--rw-r--r--   0      501       20       67 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles_noqa.py.snap
--rw-r--r--   0      501       20       67 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles_wrapped.py.snap
--rw-r--r--   0      501       20      447 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles.py.snap
--rw-r--r--   0      501       20      446 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles_class.py.snap
--rw-r--r--   0      501       20      318 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles_function.py.snap
--rw-r--r--   0      501       20      190 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles_module_multiline.py.snap
--rw-r--r--   0      501       20      191 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles_module_singleline.py.snap
--rw-r--r--   0      501       20      872 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles.py.snap
--rw-r--r--   0      501       20      331 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_class.py.snap
--rw-r--r--   0      501       20      737 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_function.py.snap
--rw-r--r--   0      501       20      329 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_module_multiline.py.snap
--rw-r--r--   0      501       20      330 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_module_singleline.py.snap
--rw-r--r--   0      501       20      326 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles.py.snap
--rw-r--r--   0      501       20      178 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles_escaped.py.snap
--rw-r--r--   0      501       20      197 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles_multiline_string.py.snap
--rw-r--r--   0      501       20       67 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles_noqa.py.snap
--rw-r--r--   0      501       20       67 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles_wrapped.py.snap
--rw-r--r--   0      501       20     9122 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/fs.rs
--rw-r--r--   0      501       20     2090 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/lib.rs
--rw-r--r--   0      501       20    19253 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/linter.rs
--rw-r--r--   0      501       20      903 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/logging.rs
--rw-r--r--   0      501       20    13885 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/main.rs
--rw-r--r--   0      501       20     1733 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/message.rs
--rw-r--r--   0      501       20     8990 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/noqa.rs
--rw-r--r--   0      501       20     9568 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pep8_naming/checks.rs
--rw-r--r--   0      501       20       34 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pep8_naming/mod.rs
--rw-r--r--   0      501       20     1853 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pep8_naming/settings.rs
--rw-r--r--   0      501       20     3200 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/printer.rs
--rw-r--r--   0      501       20    10683 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pycodestyle/checks.rs
--rw-r--r--   0      501       20       16 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pycodestyle/mod.rs
--rw-r--r--   0      501       20       17 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pydocstyle/mod.rs
--rw-r--r--   0      501       20    60594 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pydocstyle/plugins.rs
--rw-r--r--   0      501       20     9625 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyflakes/checks.rs
--rw-r--r--   0      501       20     4636 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyflakes/fixes.rs
--rw-r--r--   0      501       20       48 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyflakes/mod.rs
--rw-r--r--   0      501       20      362 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyflakes/plugins/assert_tuple.rs
--rw-r--r--   0      501       20      350 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyflakes/plugins/if_tuple.rs
--rw-r--r--   0      501       20      708 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyflakes/plugins/invalid_print_syntax.rs
--rw-r--r--   0      501       20      175 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyflakes/plugins/mod.rs
--rw-r--r--   0      501       20     2925 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/python/builtins.rs
--rw-r--r--   0      501       20      300 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/python/future.rs
--rw-r--r--   0      501       20       50 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/python/mod.rs
--rw-r--r--   0      501       20     7731 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/python/typing.rs
--rw-r--r--   0      501       20     5229 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/checks.rs
--rw-r--r--   0      501       20     4454 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/fixes.rs
--rw-r--r--   0      501       20       59 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/mod.rs
--rw-r--r--   0      501       20     1970 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/deprecated_unittest_alias.rs
--rw-r--r--   0      501       20      676 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/mod.rs
--rw-r--r--   0      501       20     1025 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/super_call_with_parameters.rs
--rw-r--r--   0      501       20      769 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/type_of_primitive.rs
--rw-r--r--   0      501       20      639 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/unnecessary_abspath.rs
--rw-r--r--   0      501       20      571 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/use_pep585_annotation.rs
--rw-r--r--   0      501       20     3378 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/use_pep604_annotation.rs
--rw-r--r--   0      501       20     1315 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/useless_metaclass_type.rs
--rw-r--r--   0      501       20      763 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/useless_object_inheritance.rs
--rw-r--r--   0      501       20     1092 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/types.rs
--rw-r--r--   0      501       20     4057 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/settings/configuration.rs
--rw-r--r--   0      501       20     5741 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/settings/mod.rs
--rw-r--r--   0      501       20     1023 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/settings/options.rs
--rw-r--r--   0      501       20    11361 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/settings/pyproject.rs
--rw-r--r--   0      501       20     3673 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/settings/types.rs
--rw-r--r--   0      501       20     2856 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/settings/user.rs
--rw-r--r--   0      501       20     2445 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__A001_A001.py.snap
--rw-r--r--   0      501       20      986 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__A002_A002.py.snap
--rw-r--r--   0      501       20      319 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__A003_A003.py.snap
--rw-r--r--   0      501       20      289 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B002_B002.py.snap
--rw-r--r--   0      501       20     1394 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B006_B006_B008.py.snap
--rw-r--r--   0      501       20     1174 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B007_B007.py.snap
--rw-r--r--   0      501       20      629 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B011_B011.py.snap
--rw-r--r--   0      501       20      195 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B013_B013.py.snap
--rw-r--r--   0      501       20      964 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B014_B014.py.snap
--rw-r--r--   0      501       20      171 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B017_B017.py.snap
--rw-r--r--   0      501       20      617 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B025_B025.py.snap
--rw-r--r--   0      501       20      171 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C400_C400.py.snap
--rw-r--r--   0      501       20      170 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C401_C401.py.snap
--rw-r--r--   0      501       20      171 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C402_C402.py.snap
--rw-r--r--   0      501       20      178 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C403_C403.py.snap
--rw-r--r--   0      501       20      179 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C404_C404.py.snap
--rw-r--r--   0      501       20      564 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C405_C405.py.snap
--rw-r--r--   0      501       20      568 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C406_C406.py.snap
--rw-r--r--   0      501       20      579 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C408_C408.py.snap
--rw-r--r--   0      501       20      471 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C409_C409.py.snap
--rw-r--r--   0      501       20      608 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C410_C410.py.snap
--rw-r--r--   0      501       20      166 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C411_C411.py.snap
--rw-r--r--   0      501       20      460 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C413_C413.py.snap
--rw-r--r--   0      501       20     2134 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C414_C414.py.snap
--rw-r--r--   0      501       20      597 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C415_C415.py.snap
--rw-r--r--   0      501       20      311 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C416_C416.py.snap
--rw-r--r--   0      501       20     1042 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C417_C417.py.snap
--rw-r--r--   0      501       20      158 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D100_D.py.snap
--rw-r--r--   0      501       20      159 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D101_D.py.snap
--rw-r--r--   0      501       20      380 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D102_D.py.snap
--rw-r--r--   0      501       20      164 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D103_D.py.snap
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D104_D.py.snap
--rw-r--r--   0      501       20      159 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D105_D.py.snap
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D106_D.py.snap
--rw-r--r--   0      501       20      268 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D107_D.py.snap
--rw-r--r--   0      501       20      620 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D201_D.py.snap
--rw-r--r--   0      501       20      618 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D202_D.py.snap
--rw-r--r--   0      501       20      904 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D203_D.py.snap
--rw-r--r--   0      501       20      618 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D204_D.py.snap
--rw-r--r--   0      501       20      600 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D205_D.py.snap
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D206_D.py.snap
--rw-r--r--   0      501       20      630 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D207_D.py.snap
--rw-r--r--   0      501       20      869 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D208_D.py.snap
--rw-r--r--   0      501       20      336 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D209_D.py.snap
--rw-r--r--   0      501       20      949 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D210_D.py.snap
--rw-r--r--   0      501       20      614 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D211_D.py.snap
--rw-r--r--   0      501       20      175 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D212_D.py.snap
--rw-r--r--   0      501       20     2069 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D213_D.py.snap
--rw-r--r--   0      501       20      341 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D214_sections.py.snap
--rw-r--r--   0      501       20      650 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D215_sections.py.snap
--rw-r--r--   0      501       20      635 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D300_D.py.snap
--rw-r--r--   0      501       20     1860 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D400_D.py.snap
--rw-r--r--   0      501       20      162 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D402_D.py.snap
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D403_D.py.snap
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D404_D.py.snap
--rw-r--r--   0      501       20      642 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D405_sections.py.snap
--rw-r--r--   0      501       20     1204 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D406_sections.py.snap
--rw-r--r--   0      501       20     4593 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D407_sections.py.snap
--rw-r--r--   0      501       20      336 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D408_sections.py.snap
--rw-r--r--   0      501       20      677 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D409_sections.py.snap
--rw-r--r--   0      501       20      622 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D410_sections.py.snap
--rw-r--r--   0      501       20      911 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D411_sections.py.snap
--rw-r--r--   0      501       20      356 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D412_sections.py.snap
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D413_sections.py.snap
--rw-r--r--   0      501       20      683 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D414_sections.py.snap
--rw-r--r--   0      501       20     1822 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D415_D.py.snap
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D416_D.py.snap
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D417_canonical_google_examples.py.snap
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D417_canonical_numpy_examples.py.snap
--rw-r--r--   0      501       20     1667 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D417_sections.py.snap
--rw-r--r--   0      501       20      385 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D418_D.py.snap
--rw-r--r--   0      501       20      371 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D419_D.py.snap
--rw-r--r--   0      501       20      174 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E402_E402.py.snap
--rw-r--r--   0      501       20      187 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E501_E501.py.snap
--rw-r--r--   0      501       20     1024 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E711_E711.py.snap
--rw-r--r--   0      501       20     1383 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E712_E712.py.snap
--rw-r--r--   0      501       20      587 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E713_E713.py.snap
--rw-r--r--   0      501       20      369 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E714_E714.py.snap
--rw-r--r--   0      501       20     1868 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E721_E721.py.snap
--rw-r--r--   0      501       20      396 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E722_E722.py.snap
--rw-r--r--   0      501       20      624 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E731_E731.py.snap
--rw-r--r--   0      501       20     3201 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E741_E741.py.snap
--rw-r--r--   0      501       20      414 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E742_E742.py.snap
--rw-r--r--   0      501       20      424 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E743_E743.py.snap
--rw-r--r--   0      501       20      181 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E999_E999.py.snap
--rw-r--r--   0      501       20     2224 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F401_F401_0.py.snap
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F401_F401_1.py.snap
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F401_F401_2.py.snap
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F401_F401_3.py.snap
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F401_F401_4.py.snap
--rw-r--r--   0      501       20     1214 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F401_F401_5.py.snap
--rw-r--r--   0      501       20      342 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F402_F402.py.snap
--rw-r--r--   0      501       20      292 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F403_F403.py.snap
--rw-r--r--   0      501       20      163 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F404_F404.py.snap
--rw-r--r--   0      501       20      347 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F405_F405.py.snap
--rw-r--r--   0      501       20      308 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F406_F406.py.snap
--rw-r--r--   0      501       20      196 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F407_F407.py.snap
--rw-r--r--   0      501       20      419 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F541_F541.py.snap
--rw-r--r--   0      501       20      425 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F601_F601.py.snap
--rw-r--r--   0      501       20      182 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F602_F602.py.snap
--rw-r--r--   0      501       20      167 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F622_F622.py.snap
--rw-r--r--   0      501       20      266 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F631_F631.py.snap
--rw-r--r--   0      501       20      262 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F632_F632.py.snap
--rw-r--r--   0      501       20      164 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F633_F633.py.snap
--rw-r--r--   0      501       20      256 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F634_F634.py.snap
--rw-r--r--   0      501       20      504 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F701_F701.py.snap
--rw-r--r--   0      501       20      519 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F702_F702.py.snap
--rw-r--r--   0      501       20      402 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F704_F704.py.snap
--rw-r--r--   0      501       20      285 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F706_F706.py.snap
--rw-r--r--   0      501       20      402 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F707_F707.py.snap
--rw-r--r--   0      501       20      185 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F722_F722.py.snap
--rw-r--r--   0      501       20     1410 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F821_F821_0.py.snap
--rw-r--r--   0      501       20      545 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F821_F821_1.py.snap
--rw-r--r--   0      501       20      168 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F822_F822.py.snap
--rw-r--r--   0      501       20      173 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F823_F823.py.snap
--rw-r--r--   0      501       20      407 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F831_F831.py.snap
--rw-r--r--   0      501       20      645 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F841_F841.py.snap
--rw-r--r--   0      501       20      284 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F901_F901.py.snap
--rw-r--r--   0      501       20      679 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N801_N801.py.snap
--rw-r--r--   0      501       20      688 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N802_N802.py.snap
--rw-r--r--   0      501       20      298 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N803_N803.py.snap
--rw-r--r--   0      501       20      186 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N804_N804.py.snap
--rw-r--r--   0      501       20      314 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N805_N805.py.snap
--rw-r--r--   0      501       20      328 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N806_N806.py.snap
--rw-r--r--   0      501       20      164 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N807_N807.py.snap
--rw-r--r--   0      501       20      555 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N811_N811.py.snap
--rw-r--r--   0      501       20      568 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N812_N812.py.snap
--rw-r--r--   0      501       20      555 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N813_N813.py.snap
--rw-r--r--   0      501       20      552 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N814_N814.py.snap
--rw-r--r--   0      501       20      475 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N815_N815.py.snap
--rw-r--r--   0      501       20      477 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N816_N816.py.snap
--rw-r--r--   0      501       20      360 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N817_N817.py.snap
--rw-r--r--   0      501       20      180 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N818_N818.py.snap
--rw-r--r--   0      501       20      305 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__T201_T201.py.snap
--rw-r--r--   0      501       20      562 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__T203_T203.py.snap
--rw-r--r--   0      501       20      583 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U001_U001.py.snap
--rw-r--r--   0      501       20      864 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U002_U002.py.snap
--rw-r--r--   0      501       20     1411 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U003_U003.py.snap
--rw-r--r--   0      501       20     5675 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U004_U004.py.snap
--rw-r--r--   0      501       20     1407 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U005_U005.py.snap
--rw-r--r--   0      501       20      608 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U006_U006.py.snap
--rw-r--r--   0      501       20     2314 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U007_U007.py.snap
--rw-r--r--   0      501       20     1442 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U008_U008.py.snap
--rw-r--r--   0      501       20      166 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__W292_W292_0.py.snap
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__W292_W292_1.py.snap
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__W292_W292_2.py.snap
--rw-r--r--   0      501       20      555 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__W605_W605.py.snap
--rw-r--r--   0      501       20      894 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__f841_dummy_variable_rgx.snap
--rw-r--r--   0      501       20      503 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__future_annotations.snap
--rw-r--r--   0      501       20       53 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__init.snap
--rw-r--r--   0      501       20     2011 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__m001.snap
--rw-r--r--   0      501       20     3960 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/source_code_locator.rs
--rw-r--r--   0      501       20     5340 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/visibility.rs
--rw-r--r--   0      501       20     2220 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/tests/integration_test.rs
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 flake8_to_ruff-0.0.94_dev.1/Cargo.toml
--rw-r--r--   0      501       20    74631 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/Cargo.lock
--rw-r--r--   0      501       20     1587 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/README.md
--rw-r--r--   0      501       20     1111 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/pyproject.toml
--rw-r--r--   0      501       20     9084 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/src/converter.rs
--rw-r--r--   0      501       20       95 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/src/lib.rs
--rw-r--r--   0      501       20      853 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/src/main.rs
--rw-r--r--   0      501       20    12359 2022-11-02 03:11:02.000000 flake8_to_ruff-0.0.94_dev.1/src/parser.rs
--rw-r--r--   0        0        0     2619 1970-01-01 00:00:00.000000 flake8_to_ruff-0.0.94_dev.1/PKG-INFO
+-rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/Cargo.toml
+-rw-r--r--   0      501       20      278 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/.editorconfig
+-rw-r--r--   0      501       20     3712 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/.github/workflows/ci.yaml
+-rw-r--r--   0      501       20     8911 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/.github/workflows/flake8-to-ruff.yaml
+-rw-r--r--   0      501       20     8618 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/.github/workflows/ruff.yaml
+-rw-r--r--   0      501       20     3407 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/.gitignore
+-rw-r--r--   0      501       20      231 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/.pre-commit-config.yaml
+-rw-r--r--   0      501       20     5227 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/CODE_OF_CONDUCT.md
+-rw-r--r--   0      501       20     4582 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/CONTRIBUTING.md
+-rw-r--r--   0      501       20    82250 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/Cargo.lock
+-rw-r--r--   0      501       20     1070 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/LICENSE
+-rw-r--r--   0      501       20    35361 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/README.md
+-rw-r--r--   0      501       20      475 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/benches/source_code_locator.rs
+-rw-r--r--   0      501       20     3314 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/examples/generate_check_code_prefix.rs
+-rw-r--r--   0      501       20      942 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/examples/generate_rules_table.rs
+-rw-r--r--   0      501       20      568 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/examples/generate_source_code.rs
+-rw-r--r--   0      501       20      477 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/examples/print_ast.rs
+-rw-r--r--   0      501       20      470 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/examples/print_tokens.rs
+-rw-r--r--   0      501       20     1100 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/pyproject.toml
+-rw-r--r--   0      501       20      368 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/A001.py
+-rw-r--r--   0      501       20      130 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/A002.py
+-rw-r--r--   0      501       20      127 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/A003.py
+-rw-r--r--   0      501       20      223 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/B002.py
+-rw-r--r--   0      501       20     3342 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/B006_B008.py
+-rw-r--r--   0      501       20      716 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/B007.py
+-rw-r--r--   0      501       20      133 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/B011.py
+-rw-r--r--   0      501       20      119 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/B013.py
+-rw-r--r--   0      501       20     1364 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/B014.py
+-rw-r--r--   0      501       20      829 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/B017.py
+-rw-r--r--   0      501       20      446 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/B025.py
+-rw-r--r--   0      501       20       66 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/C400.py
+-rw-r--r--   0      501       20       64 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/C401.py
+-rw-r--r--   0      501       20      106 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/C402.py
+-rw-r--r--   0      501       20       68 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/C403.py
+-rw-r--r--   0      501       20       71 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/C404.py
+-rw-r--r--   0      501       20       71 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/C405.py
+-rw-r--r--   0      501       20       81 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/C406.py
+-rw-r--r--   0      501       20       66 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/C408.py
+-rw-r--r--   0      501       20      107 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/C409.py
+-rw-r--r--   0      501       20       64 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/C410.py
+-rw-r--r--   0      501       20       35 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/C411.py
+-rw-r--r--   0      501       20       84 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/C413.py
+-rw-r--r--   0      501       20      216 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/C414.py
+-rw-r--r--   0      501       20      193 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/C415.py
+-rw-r--r--   0      501       20       95 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/C416.py
+-rw-r--r--   0      501       20      179 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/C417.py
+-rw-r--r--   0      501       20    12157 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/D.py
+-rw-r--r--   0      501       20      294 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E402.py
+-rw-r--r--   0      501       20      786 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E501.py
+-rw-r--r--   0      501       20      648 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E711.py
+-rw-r--r--   0      501       20      653 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E712.py
+-rw-r--r--   0      501       20      540 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E713.py
+-rw-r--r--   0      501       20      508 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E714.py
+-rw-r--r--   0      501       20      907 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E721.py
+-rw-r--r--   0      501       20      327 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E722.py
+-rw-r--r--   0      501       20      252 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E731.py
+-rw-r--r--   0      501       20      676 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E741.py
+-rw-r--r--   0      501       20       78 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E742.py
+-rw-r--r--   0      501       20       99 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E743.py
+-rw-r--r--   0      501       20       10 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E999.py
+-rw-r--r--   0      501       20     1549 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F401_0.py
+-rw-r--r--   0      501       20      121 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F401_1.py
+-rw-r--r--   0      501       20      242 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F401_2.py
+-rw-r--r--   0      501       20      302 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F401_3.py
+-rw-r--r--   0      501       20      315 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F401_4.py
+-rw-r--r--   0      501       20      126 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F401_5.py
+-rw-r--r--   0      501       20       96 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F402.py
+-rw-r--r--   0      501       20      152 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F403.py
+-rw-r--r--   0      501       20      130 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F404.py
+-rw-r--r--   0      501       20      116 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F405.py
+-rw-r--r--   0      501       20       87 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F406.py
+-rw-r--r--   0      501       20       82 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F407.py
+-rw-r--r--   0      501       20      112 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F541.py
+-rw-r--r--   0      501       20      144 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F601.py
+-rw-r--r--   0      501       20       50 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F602.py
+-rw-r--r--   0      501       20       64 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F622.py
+-rw-r--r--   0      501       20       58 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F631.py
+-rw-r--r--   0      501       20       51 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F632.py
+-rw-r--r--   0      501       20       79 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F633.py
+-rw-r--r--   0      501       20      122 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F634.py
+-rw-r--r--   0      501       20      179 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F701.py
+-rw-r--r--   0      501       20      200 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F702.py
+-rw-r--r--   0      501       20       76 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F704.py
+-rw-r--r--   0      501       20       66 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F706.py
+-rw-r--r--   0      501       20      380 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F707.py
+-rw-r--r--   0      501       20       74 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F722.py
+-rw-r--r--   0      501       20     2196 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F821_0.py
+-rw-r--r--   0      501       20      395 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F821_1.py
+-rw-r--r--   0      501       20      259 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F821_2.py
+-rw-r--r--   0      501       20       28 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F822.py
+-rw-r--r--   0      501       20      245 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F823.py
+-rw-r--r--   0      501       20      159 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F831.py
+-rw-r--r--   0      501       20      343 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F841.py
+-rw-r--r--   0      501       20       88 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F901.py
+-rw-r--r--   0      501       20     1762 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/M001.py
+-rw-r--r--   0      501       20      225 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/N801.py
+-rw-r--r--   0      501       20      354 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/N802.py
+-rw-r--r--   0      501       20       95 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/N803.py
+-rw-r--r--   0      501       20      264 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/N804.py
+-rw-r--r--   0      501       20      345 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/N805.py
+-rw-r--r--   0      501       20       64 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/N806.py
+-rw-r--r--   0      501       20      126 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/N807.py
+-rw-r--r--   0      501       20      116 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/N811.py
+-rw-r--r--   0      501       20      124 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/N812.py
+-rw-r--r--   0      501       20      119 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/N813.py
+-rw-r--r--   0      501       20      119 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/N814.py
+-rw-r--r--   0      501       20       96 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/N815.py
+-rw-r--r--   0      501       20       67 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/N816.py
+-rw-r--r--   0      501       20       55 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/N817.py
+-rw-r--r--   0      501       20      106 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/N818.py
+-rw-r--r--   0      501       20       31 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/T201.py
+-rw-r--r--   0      501       20      148 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/T203.py
+-rw-r--r--   0      501       20      152 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/U001.py
+-rw-r--r--   0      501       20      146 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/U002.py
+-rw-r--r--   0      501       20       45 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/U003.py
+-rw-r--r--   0      501       20      883 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/U004.py
+-rw-r--r--   0      501       20      263 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/U005.py
+-rw-r--r--   0      501       20      125 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/U006.py
+-rw-r--r--   0      501       20      463 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/U007.py
+-rw-r--r--   0      501       20     1483 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/U008.py
+-rw-r--r--   0      501       20       26 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/W292_0.py
+-rw-r--r--   0      501       20       40 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/W292_1.py
+-rw-r--r--   0      501       20       27 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/W292_2.py
+-rw-r--r--   0      501       20      316 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/W605.py
+-rw-r--r--   0      501       20       54 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/__init__.py
+-rw-r--r--   0      501       20        0 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/bar/__init__.py
+-rw-r--r--   0      501       20        0 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/bar/migrations/__init__.py
+-rw-r--r--   0      501       20       90 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/bar/migrations/migration.py
+-rw-r--r--   0      501       20     4176 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/canonical_google_examples.py
+-rw-r--r--   0      501       20     5315 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/canonical_numpy_examples.py
+-rw-r--r--   0      501       20       90 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/directory/also_excluded.py
+-rw-r--r--   0      501       20       90 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/excluded.py
+-rw-r--r--   0      501       20      716 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_doubles.py
+-rw-r--r--   0      501       20      290 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_doubles_class.py
+-rw-r--r--   0      501       20      406 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_doubles_function.py
+-rw-r--r--   0      501       20      133 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_doubles_module_multiline.py
+-rw-r--r--   0      501       20      135 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_doubles_module_singleline.py
+-rw-r--r--   0      501       20      772 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_singles.py
+-rw-r--r--   0      501       20      290 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_singles_class.py
+-rw-r--r--   0      501       20      408 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_singles_function.py
+-rw-r--r--   0      501       20      133 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_singles_module_multiline.py
+-rw-r--r--   0      501       20      135 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_singles_module_singleline.py
+-rw-r--r--   0      501       20       93 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/doubles.py
+-rw-r--r--   0      501       20      203 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/doubles_escaped.py
+-rw-r--r--   0      501       20      165 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/doubles_multiline_string.py
+-rw-r--r--   0      501       20       58 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/doubles_noqa.py
+-rw-r--r--   0      501       20      106 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/doubles_wrapped.py
+-rw-r--r--   0      501       20       93 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/singles.py
+-rw-r--r--   0      501       20      203 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/singles_escaped.py
+-rw-r--r--   0      501       20      165 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/singles_multiline_string.py
+-rw-r--r--   0      501       20       58 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/singles_noqa.py
+-rw-r--r--   0      501       20      106 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/singles_wrapped.py
+-rw-r--r--   0      501       20        0 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/foo/__init__.py
+-rw-r--r--   0      501       20        0 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/foo/migrations/__init__.py
+-rw-r--r--   0      501       20       90 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/foo/migrations/migration.py
+-rw-r--r--   0      501       20      444 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/future_annotations.py
+-rw-r--r--   0      501       20      632 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/pyproject.toml
+-rw-r--r--   0      501       20    12260 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/sections.py
+-rw-r--r--   0      501       20        7 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/rust-toolchain
+-rw-r--r--   0      501       20      390 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/rustfmt.toml
+-rw-r--r--   0      501       20      302 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/scripts/.flake8
+-rw-r--r--   0      501       20    37365 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/scripts/poetry.lock
+-rw-r--r--   0      501       20      454 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/scripts/pyproject.toml
+-rwxr-xr-x   0      501       20     1035 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/scripts/run_flake8.py
+-rw-r--r--   0      501       20      565 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/setup.py
+-rw-r--r--   0      501       20     4422 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/ast/helpers.rs
+-rw-r--r--   0      501       20       87 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/ast/mod.rs
+-rw-r--r--   0      501       20     3881 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/ast/operations.rs
+-rw-r--r--   0      501       20     4574 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/ast/relocate.rs
+-rw-r--r--   0      501       20     2211 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/ast/types.rs
+-rw-r--r--   0      501       20    18283 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/ast/visitor.rs
+-rw-r--r--   0      501       20     6495 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/autofix/fixer.rs
+-rw-r--r--   0      501       20     3383 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/autofix/helpers.rs
+-rw-r--r--   0      501       20     1217 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/autofix/mod.rs
+-rw-r--r--   0      501       20     4136 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/cache.rs
+-rw-r--r--   0      501       20   100138 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/check_ast.rs
+-rw-r--r--   0      501       20     9787 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/check_lines.rs
+-rw-r--r--   0      501       20     1740 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/check_tokens.rs
+-rw-r--r--   0      501       20    69859 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/checks.rs
+-rw-r--r--   0      501       20    43083 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/checks_gen.rs
+-rw-r--r--   0      501       20     6185 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/cli.rs
+-rw-r--r--   0      501       20    36461 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/code_gen.rs
+-rw-r--r--   0      501       20     1201 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/cst/helpers.rs
+-rw-r--r--   0      501       20      536 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/cst/matchers.rs
+-rw-r--r--   0      501       20       35 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/cst/mod.rs
+-rw-r--r--   0      501       20      404 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/docstrings/definition.rs
+-rw-r--r--   0      501       20     2428 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/docstrings/extraction.rs
+-rw-r--r--   0      501       20     1423 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/docstrings/google.rs
+-rw-r--r--   0      501       20     1363 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/docstrings/helpers.rs
+-rw-r--r--   0      501       20      122 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/docstrings/mod.rs
+-rw-r--r--   0      501       20      908 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/docstrings/numpy.rs
+-rw-r--r--   0      501       20     3140 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/docstrings/sections.rs
+-rw-r--r--   0      501       20      797 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/docstrings/styles.rs
+-rw-r--r--   0      501       20       17 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/mod.rs
+-rw-r--r--   0      501       20     2046 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/plugins/assert_false.rs
+-rw-r--r--   0      501       20      918 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/plugins/assert_raises_exception.rs
+-rw-r--r--   0      501       20     4108 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/plugins/duplicate_exceptions.rs
+-rw-r--r--   0      501       20      654 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/plugins/mod.rs
+-rw-r--r--   0      501       20     2255 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/plugins/mutable_argument_default.rs
+-rw-r--r--   0      501       20      822 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/plugins/redundant_tuple_in_exception_handler.rs
+-rw-r--r--   0      501       20      635 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/plugins/unary_prefix_increment.rs
+-rw-r--r--   0      501       20     2046 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/plugins/unused_loop_control_variable.rs
+-rw-r--r--   0      501       20      759 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_builtins/checks.rs
+-rw-r--r--   0      501       20       31 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_builtins/mod.rs
+-rw-r--r--   0      501       20       70 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_builtins/types.rs
+-rw-r--r--   0      501       20    15487 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_comprehensions/checks.rs
+-rw-r--r--   0      501       20    21798 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_comprehensions/fixes.rs
+-rw-r--r--   0      501       20       27 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_comprehensions/mod.rs
+-rw-r--r--   0      501       20      949 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_print/checks.rs
+-rw-r--r--   0      501       20       29 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_print/mod.rs
+-rw-r--r--   0      501       20       49 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_print/plugins/mod.rs
+-rw-r--r--   0      501       20     1657 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_print/plugins/print_call.rs
+-rw-r--r--   0      501       20    10466 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/checks.rs
+-rw-r--r--   0      501       20     3662 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/docstring_detection.rs
+-rw-r--r--   0      501       20       63 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/mod.rs
+-rw-r--r--   0      501       20     1382 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/settings.rs
+-rw-r--r--   0      501       20      737 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles.py.snap
+-rw-r--r--   0      501       20      331 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_class.py.snap
+-rw-r--r--   0      501       20      737 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_function.py.snap
+-rw-r--r--   0      501       20      329 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_module_multiline.py.snap
+-rw-r--r--   0      501       20      330 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_module_singleline.py.snap
+-rw-r--r--   0      501       20      447 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles.py.snap
+-rw-r--r--   0      501       20      446 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles_class.py.snap
+-rw-r--r--   0      501       20      318 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles_function.py.snap
+-rw-r--r--   0      501       20      190 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles_module_multiline.py.snap
+-rw-r--r--   0      501       20      191 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_singles_module_singleline.py.snap
+-rw-r--r--   0      501       20      326 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles.py.snap
+-rw-r--r--   0      501       20      178 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles_escaped.py.snap
+-rw-r--r--   0      501       20      197 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles_multiline_string.py.snap
+-rw-r--r--   0      501       20       67 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles_noqa.py.snap
+-rw-r--r--   0      501       20       67 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__doubles_doubles_wrapped.py.snap
+-rw-r--r--   0      501       20      447 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles.py.snap
+-rw-r--r--   0      501       20      446 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles_class.py.snap
+-rw-r--r--   0      501       20      318 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles_function.py.snap
+-rw-r--r--   0      501       20      190 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles_module_multiline.py.snap
+-rw-r--r--   0      501       20      191 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_doubles_module_singleline.py.snap
+-rw-r--r--   0      501       20      872 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles.py.snap
+-rw-r--r--   0      501       20      331 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_class.py.snap
+-rw-r--r--   0      501       20      737 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_function.py.snap
+-rw-r--r--   0      501       20      329 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_module_multiline.py.snap
+-rw-r--r--   0      501       20      330 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_module_singleline.py.snap
+-rw-r--r--   0      501       20      326 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles.py.snap
+-rw-r--r--   0      501       20      178 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles_escaped.py.snap
+-rw-r--r--   0      501       20      197 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles_multiline_string.py.snap
+-rw-r--r--   0      501       20       67 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles_noqa.py.snap
+-rw-r--r--   0      501       20       67 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__singles_singles_wrapped.py.snap
+-rw-r--r--   0      501       20     9122 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/fs.rs
+-rw-r--r--   0      501       20     2144 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/lib.rs
+-rw-r--r--   0      501       20    19321 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/linter.rs
+-rw-r--r--   0      501       20     1989 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/logging.rs
+-rw-r--r--   0      501       20    13963 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/main.rs
+-rw-r--r--   0      501       20     1733 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/message.rs
+-rw-r--r--   0      501       20     8990 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/noqa.rs
+-rw-r--r--   0      501       20     9580 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pep8_naming/checks.rs
+-rw-r--r--   0      501       20       34 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pep8_naming/mod.rs
+-rw-r--r--   0      501       20     1859 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pep8_naming/settings.rs
+-rw-r--r--   0      501       20     3935 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/printer.rs
+-rw-r--r--   0      501       20    10683 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pycodestyle/checks.rs
+-rw-r--r--   0      501       20       16 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pycodestyle/mod.rs
+-rw-r--r--   0      501       20       17 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pydocstyle/mod.rs
+-rw-r--r--   0      501       20    60594 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pydocstyle/plugins.rs
+-rw-r--r--   0      501       20     8873 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyflakes/checks.rs
+-rw-r--r--   0      501       20     4219 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyflakes/fixes.rs
+-rw-r--r--   0      501       20       48 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyflakes/mod.rs
+-rw-r--r--   0      501       20      371 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyflakes/plugins/assert_tuple.rs
+-rw-r--r--   0      501       20      359 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyflakes/plugins/if_tuple.rs
+-rw-r--r--   0      501       20      717 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyflakes/plugins/invalid_print_syntax.rs
+-rw-r--r--   0      501       20      256 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyflakes/plugins/mod.rs
+-rw-r--r--   0      501       20     1205 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyflakes/plugins/raise_not_implemented.rs
+-rw-r--r--   0      501       20     2925 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/python/builtins.rs
+-rw-r--r--   0      501       20      300 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/python/future.rs
+-rw-r--r--   0      501       20       50 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/python/mod.rs
+-rw-r--r--   0      501       20     9789 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/python/typing.rs
+-rw-r--r--   0      501       20     5229 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/checks.rs
+-rw-r--r--   0      501       20     4454 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/fixes.rs
+-rw-r--r--   0      501       20       59 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/mod.rs
+-rw-r--r--   0      501       20     1970 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/deprecated_unittest_alias.rs
+-rw-r--r--   0      501       20      676 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/mod.rs
+-rw-r--r--   0      501       20     1025 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/super_call_with_parameters.rs
+-rw-r--r--   0      501       20      769 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/type_of_primitive.rs
+-rw-r--r--   0      501       20      639 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/unnecessary_abspath.rs
+-rw-r--r--   0      501       20      571 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/use_pep585_annotation.rs
+-rw-r--r--   0      501       20     3378 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/use_pep604_annotation.rs
+-rw-r--r--   0      501       20     1315 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/useless_metaclass_type.rs
+-rw-r--r--   0      501       20      763 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/useless_object_inheritance.rs
+-rw-r--r--   0      501       20     1092 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/types.rs
+-rw-r--r--   0      501       20     4057 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/settings/configuration.rs
+-rw-r--r--   0      501       20     5970 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/settings/mod.rs
+-rw-r--r--   0      501       20     1023 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/settings/options.rs
+-rw-r--r--   0      501       20    11361 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/settings/pyproject.rs
+-rw-r--r--   0      501       20     3714 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/settings/types.rs
+-rw-r--r--   0      501       20     2856 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/settings/user.rs
+-rw-r--r--   0      501       20     2445 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__A001_A001.py.snap
+-rw-r--r--   0      501       20      986 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__A002_A002.py.snap
+-rw-r--r--   0      501       20      319 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__A003_A003.py.snap
+-rw-r--r--   0      501       20      289 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B002_B002.py.snap
+-rw-r--r--   0      501       20     1394 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B006_B006_B008.py.snap
+-rw-r--r--   0      501       20     1174 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B007_B007.py.snap
+-rw-r--r--   0      501       20      629 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B011_B011.py.snap
+-rw-r--r--   0      501       20      195 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B013_B013.py.snap
+-rw-r--r--   0      501       20      964 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B014_B014.py.snap
+-rw-r--r--   0      501       20      171 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B017_B017.py.snap
+-rw-r--r--   0      501       20      617 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B025_B025.py.snap
+-rw-r--r--   0      501       20      638 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C400_C400.py.snap
+-rw-r--r--   0      501       20      636 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C401_C401.py.snap
+-rw-r--r--   0      501       20      644 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C402_C402.py.snap
+-rw-r--r--   0      501       20      652 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C403_C403.py.snap
+-rw-r--r--   0      501       20      179 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C404_C404.py.snap
+-rw-r--r--   0      501       20     1178 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C405_C405.py.snap
+-rw-r--r--   0      501       20     1181 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C406_C406.py.snap
+-rw-r--r--   0      501       20     1189 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C408_C408.py.snap
+-rw-r--r--   0      501       20     1532 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C409_C409.py.snap
+-rw-r--r--   0      501       20     1220 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C410_C410.py.snap
+-rw-r--r--   0      501       20      329 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C411_C411.py.snap
+-rw-r--r--   0      501       20      460 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C413_C413.py.snap
+-rw-r--r--   0      501       20     2134 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C414_C414.py.snap
+-rw-r--r--   0      501       20      597 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C415_C415.py.snap
+-rw-r--r--   0      501       20      618 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C416_C416.py.snap
+-rw-r--r--   0      501       20     1042 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C417_C417.py.snap
+-rw-r--r--   0      501       20      158 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D100_D.py.snap
+-rw-r--r--   0      501       20      159 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D101_D.py.snap
+-rw-r--r--   0      501       20      380 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D102_D.py.snap
+-rw-r--r--   0      501       20      164 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D103_D.py.snap
+-rw-r--r--   0      501       20       53 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D104_D.py.snap
+-rw-r--r--   0      501       20      159 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D105_D.py.snap
+-rw-r--r--   0      501       20       53 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D106_D.py.snap
+-rw-r--r--   0      501       20      268 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D107_D.py.snap
+-rw-r--r--   0      501       20      620 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D201_D.py.snap
+-rw-r--r--   0      501       20      618 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D202_D.py.snap
+-rw-r--r--   0      501       20      904 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D203_D.py.snap
+-rw-r--r--   0      501       20      618 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D204_D.py.snap
+-rw-r--r--   0      501       20      600 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D205_D.py.snap
+-rw-r--r--   0      501       20       53 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D206_D.py.snap
+-rw-r--r--   0      501       20      630 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D207_D.py.snap
+-rw-r--r--   0      501       20      869 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D208_D.py.snap
+-rw-r--r--   0      501       20      336 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D209_D.py.snap
+-rw-r--r--   0      501       20      949 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D210_D.py.snap
+-rw-r--r--   0      501       20      614 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D211_D.py.snap
+-rw-r--r--   0      501       20      175 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D212_D.py.snap
+-rw-r--r--   0      501       20     2069 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D213_D.py.snap
+-rw-r--r--   0      501       20      341 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D214_sections.py.snap
+-rw-r--r--   0      501       20      650 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D215_sections.py.snap
+-rw-r--r--   0      501       20      635 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D300_D.py.snap
+-rw-r--r--   0      501       20     1860 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D400_D.py.snap
+-rw-r--r--   0      501       20      162 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D402_D.py.snap
+-rw-r--r--   0      501       20       53 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D403_D.py.snap
+-rw-r--r--   0      501       20       53 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D404_D.py.snap
+-rw-r--r--   0      501       20      642 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D405_sections.py.snap
+-rw-r--r--   0      501       20     1204 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D406_sections.py.snap
+-rw-r--r--   0      501       20     4593 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D407_sections.py.snap
+-rw-r--r--   0      501       20      336 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D408_sections.py.snap
+-rw-r--r--   0      501       20      677 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D409_sections.py.snap
+-rw-r--r--   0      501       20      622 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D410_sections.py.snap
+-rw-r--r--   0      501       20      911 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D411_sections.py.snap
+-rw-r--r--   0      501       20      356 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D412_sections.py.snap
+-rw-r--r--   0      501       20       53 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D413_sections.py.snap
+-rw-r--r--   0      501       20      683 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D414_sections.py.snap
+-rw-r--r--   0      501       20     1822 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D415_D.py.snap
+-rw-r--r--   0      501       20       53 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D416_D.py.snap
+-rw-r--r--   0      501       20       53 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D417_canonical_google_examples.py.snap
+-rw-r--r--   0      501       20       53 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D417_canonical_numpy_examples.py.snap
+-rw-r--r--   0      501       20     1667 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D417_sections.py.snap
+-rw-r--r--   0      501       20      385 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D418_D.py.snap
+-rw-r--r--   0      501       20      371 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D419_D.py.snap
+-rw-r--r--   0      501       20      174 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E402_E402.py.snap
+-rw-r--r--   0      501       20      187 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E501_E501.py.snap
+-rw-r--r--   0      501       20     1024 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E711_E711.py.snap
+-rw-r--r--   0      501       20     1383 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E712_E712.py.snap
+-rw-r--r--   0      501       20      587 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E713_E713.py.snap
+-rw-r--r--   0      501       20      369 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E714_E714.py.snap
+-rw-r--r--   0      501       20     1868 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E721_E721.py.snap
+-rw-r--r--   0      501       20      396 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E722_E722.py.snap
+-rw-r--r--   0      501       20      624 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E731_E731.py.snap
+-rw-r--r--   0      501       20     3201 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E741_E741.py.snap
+-rw-r--r--   0      501       20      414 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E742_E742.py.snap
+-rw-r--r--   0      501       20      424 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E743_E743.py.snap
+-rw-r--r--   0      501       20      181 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E999_E999.py.snap
+-rw-r--r--   0      501       20     2224 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F401_F401_0.py.snap
+-rw-r--r--   0      501       20       53 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F401_F401_1.py.snap
+-rw-r--r--   0      501       20       53 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F401_F401_2.py.snap
+-rw-r--r--   0      501       20       53 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F401_F401_3.py.snap
+-rw-r--r--   0      501       20       53 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F401_F401_4.py.snap
+-rw-r--r--   0      501       20     1214 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F401_F401_5.py.snap
+-rw-r--r--   0      501       20      342 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F402_F402.py.snap
+-rw-r--r--   0      501       20      292 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F403_F403.py.snap
+-rw-r--r--   0      501       20      163 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F404_F404.py.snap
+-rw-r--r--   0      501       20      347 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F405_F405.py.snap
+-rw-r--r--   0      501       20      308 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F406_F406.py.snap
+-rw-r--r--   0      501       20      196 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F407_F407.py.snap
+-rw-r--r--   0      501       20      419 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F541_F541.py.snap
+-rw-r--r--   0      501       20      425 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F601_F601.py.snap
+-rw-r--r--   0      501       20      182 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F602_F602.py.snap
+-rw-r--r--   0      501       20      167 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F622_F622.py.snap
+-rw-r--r--   0      501       20      266 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F631_F631.py.snap
+-rw-r--r--   0      501       20      262 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F632_F632.py.snap
+-rw-r--r--   0      501       20      164 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F633_F633.py.snap
+-rw-r--r--   0      501       20      256 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F634_F634.py.snap
+-rw-r--r--   0      501       20      504 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F701_F701.py.snap
+-rw-r--r--   0      501       20      519 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F702_F702.py.snap
+-rw-r--r--   0      501       20      402 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F704_F704.py.snap
+-rw-r--r--   0      501       20      285 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F706_F706.py.snap
+-rw-r--r--   0      501       20      402 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F707_F707.py.snap
+-rw-r--r--   0      501       20      185 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F722_F722.py.snap
+-rw-r--r--   0      501       20     1410 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F821_F821_0.py.snap
+-rw-r--r--   0      501       20      545 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F821_F821_1.py.snap
+-rw-r--r--   0      501       20      172 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F821_F821_2.py.snap
+-rw-r--r--   0      501       20      168 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F822_F822.py.snap
+-rw-r--r--   0      501       20      173 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F823_F823.py.snap
+-rw-r--r--   0      501       20      407 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F831_F831.py.snap
+-rw-r--r--   0      501       20      645 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F841_F841.py.snap
+-rw-r--r--   0      501       20      618 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F901_F901.py.snap
+-rw-r--r--   0      501       20      679 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N801_N801.py.snap
+-rw-r--r--   0      501       20      688 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N802_N802.py.snap
+-rw-r--r--   0      501       20      298 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N803_N803.py.snap
+-rw-r--r--   0      501       20      186 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N804_N804.py.snap
+-rw-r--r--   0      501       20      314 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N805_N805.py.snap
+-rw-r--r--   0      501       20      328 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N806_N806.py.snap
+-rw-r--r--   0      501       20      164 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N807_N807.py.snap
+-rw-r--r--   0      501       20      555 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N811_N811.py.snap
+-rw-r--r--   0      501       20      568 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N812_N812.py.snap
+-rw-r--r--   0      501       20      555 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N813_N813.py.snap
+-rw-r--r--   0      501       20      552 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N814_N814.py.snap
+-rw-r--r--   0      501       20      475 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N815_N815.py.snap
+-rw-r--r--   0      501       20      477 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N816_N816.py.snap
+-rw-r--r--   0      501       20      360 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N817_N817.py.snap
+-rw-r--r--   0      501       20      180 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N818_N818.py.snap
+-rw-r--r--   0      501       20      305 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__T201_T201.py.snap
+-rw-r--r--   0      501       20      562 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__T203_T203.py.snap
+-rw-r--r--   0      501       20      583 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U001_U001.py.snap
+-rw-r--r--   0      501       20      864 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U002_U002.py.snap
+-rw-r--r--   0      501       20     1411 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U003_U003.py.snap
+-rw-r--r--   0      501       20     5675 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U004_U004.py.snap
+-rw-r--r--   0      501       20     1407 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U005_U005.py.snap
+-rw-r--r--   0      501       20      608 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U006_U006.py.snap
+-rw-r--r--   0      501       20     2314 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U007_U007.py.snap
+-rw-r--r--   0      501       20     1442 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U008_U008.py.snap
+-rw-r--r--   0      501       20      166 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__W292_W292_0.py.snap
+-rw-r--r--   0      501       20       53 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__W292_W292_1.py.snap
+-rw-r--r--   0      501       20       53 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__W292_W292_2.py.snap
+-rw-r--r--   0      501       20      555 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__W605_W605.py.snap
+-rw-r--r--   0      501       20      894 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__f841_dummy_variable_rgx.snap
+-rw-r--r--   0      501       20      503 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__future_annotations.snap
+-rw-r--r--   0      501       20       53 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__init.snap
+-rw-r--r--   0      501       20     2011 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__m001.snap
+-rw-r--r--   0      501       20     3960 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/source_code_locator.rs
+-rw-r--r--   0      501       20     5340 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/visibility.rs
+-rw-r--r--   0      501       20     2220 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/tests/integration_test.rs
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 flake8_to_ruff-0.0.99_dev.0/Cargo.toml
+-rw-r--r--   0      501       20    74631 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/Cargo.lock
+-rw-r--r--   0      501       20     2353 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/README.md
+-rw-r--r--   0      501       20     1182 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/examples/poetry.ini
+-rw-r--r--   0      501       20      559 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/examples/python-discord.ini
+-rw-r--r--   0      501       20      149 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/examples/requests.ini
+-rw-r--r--   0      501       20     1111 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/pyproject.toml
+-rw-r--r--   0      501       20    14185 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/src/converter.rs
+-rw-r--r--   0      501       20      111 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/src/lib.rs
+-rw-r--r--   0      501       20     1155 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/src/main.rs
+-rw-r--r--   0      501       20    12359 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/src/parser.rs
+-rw-r--r--   0      501       20    11701 2022-11-04 02:27:52.000000 flake8_to_ruff-0.0.99_dev.0/src/plugin.rs
+-rw-r--r--   0        0        0     3385 1970-01-01 00:00:00.000000 flake8_to_ruff-0.0.99_dev.0/PKG-INFO
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/Cargo.toml` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [workspace]
 members = [
-  "crates/flake8_to_ruff",
+    "flake8_to_ruff",
 ]
 
 [package]
 name = "ruff"
-version = "0.0.94"
+version = "0.0.99"
 edition = "2021"
 
 [lib]
 name = "ruff"
 
 [dependencies]
 anyhow = { version = "1.0.60" }
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/.github/workflows/ci.yaml` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/.github/workflows/ci.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions-rs/toolchain@v1
         with:
           profile: minimal
           toolchain: nightly-2022-11-01
+          override: true
           components: rustfmt
       - uses: actions/cache@v3
         env:
           cache-name: cache-cargo
         with:
           path: |
             ~/.cargo/registry
@@ -58,14 +59,15 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions-rs/toolchain@v1
         with:
           profile: minimal
           toolchain: nightly-2022-11-01
+          override: true
           components: clippy
       - uses: actions/cache@v3
         env:
           cache-name: cache-cargo
         with:
           path: |
             ~/.cargo/registry
@@ -82,14 +84,15 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions-rs/toolchain@v1
         with:
           profile: minimal
           toolchain: nightly-2022-11-01
+          override: true
       - uses: actions/cache@v3
         env:
           cache-name: cache-cargo
         with:
           path: |
             ~/.cargo/registry
             ~/.cargo/git
@@ -105,14 +108,15 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions-rs/toolchain@v1
         with:
           profile: minimal
           toolchain: nightly-2022-11-01
+          override: true
       - uses: actions/setup-python@v4
         with:
           python-version: "3.10"
       - run: pip install maturin
       - uses: actions/cache@v3
         env:
           cache-name: cache-cargo
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/.github/workflows/flake8-to-ruff.yaml` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/.github/workflows/flake8-to-ruff.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
           toolchain: stable
           profile: minimal
           default: true
       - name: Build wheels - x86_64
         uses: messense/maturin-action@v1
         with:
           target: x86_64
-          args: --release --out dist --sdist -m ./crates/${{ env.CRATE_NAME }}/Cargo.toml
+          args: --release --out dist --sdist -m ./${{ env.CRATE_NAME }}/Cargo.toml
           maturin-version: "v0.13.0"
       - name: Install built wheel - x86_64
         run: |
           pip install dist/${{ env.CRATE_NAME }}-*.whl --force-reinstall
       - name: Upload wheels
         uses: actions/upload-artifact@v2
         with:
@@ -53,15 +53,15 @@
         with:
           toolchain: stable
           profile: minimal
           default: true
       - name: Build wheels - universal2
         uses: messense/maturin-action@v1
         with:
-          args: --release --universal2 --out dist -m ./crates/${{ env.CRATE_NAME }}/Cargo.toml
+          args: --release --universal2 --out dist -m ./${{ env.CRATE_NAME }}/Cargo.toml
           maturin-version: "v0.13.0"
       - name: Install built wheel - universal2
         run: |
           pip install dist/${{ env.CRATE_NAME }}-*universal2.whl --force-reinstall
       - name: Upload wheels
         uses: actions/upload-artifact@v2
         with:
@@ -85,15 +85,15 @@
           toolchain: stable
           profile: minimal
           default: true
       - name: Build wheels
         uses: messense/maturin-action@v1
         with:
           target: ${{ matrix.target }}
-          args: --release --out dist -m ./crates/${{ env.CRATE_NAME }}/Cargo.toml
+          args: --release --out dist -m ./${{ env.CRATE_NAME }}/Cargo.toml
           maturin-version: "v0.13.0"
       - name: Install built wheel
         shell: bash
         run: |
           python -m pip install dist/${{ env.CRATE_NAME }}-*.whl --force-reinstall
       - name: Upload wheels
         uses: actions/upload-artifact@v2
@@ -113,15 +113,15 @@
           python-version: ${{ env.PYTHON_VERSION }}
           architecture: x64
       - name: Build wheels
         uses: messense/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           manylinux: auto
-          args: --release --out dist -m ./crates/${{ env.CRATE_NAME }}/Cargo.toml
+          args: --release --out dist -m ./${{ env.CRATE_NAME }}/Cargo.toml
           maturin-version: "v0.13.0"
       - name: Install built wheel
         if: matrix.target == 'x86_64'
         run: |
           pip install dist/${{ env.CRATE_NAME }}-*.whl --force-reinstall
       - name: Upload wheels
         uses: actions/upload-artifact@v2
@@ -140,15 +140,15 @@
         with:
           python-version: ${{ env.PYTHON_VERSION }}
       - name: Build wheels
         uses: messense/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           manylinux: auto
-          args: --no-default-features --release --out dist -m ./crates/${{ env.CRATE_NAME }}/Cargo.toml
+          args: --no-default-features --release --out dist -m ./${{ env.CRATE_NAME }}/Cargo.toml
           maturin-version: "v0.13.0"
       - uses: uraimo/run-on-arch-action@v2.0.5
         if: matrix.target != 'ppc64'
         name: Install built wheel
         with:
           arch: ${{ matrix.target }}
           distro: ubuntu20.04
@@ -179,15 +179,15 @@
           python-version: ${{ env.PYTHON_VERSION }}
           architecture: x64
       - name: Build wheels
         uses: messense/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           manylinux: musllinux_1_2
-          args: --release --out dist -m ./crates/${{ env.CRATE_NAME }}/Cargo.toml
+          args: --release --out dist -m ./${{ env.CRATE_NAME }}/Cargo.toml
           maturin-version: "v0.13.0"
       - name: Install built wheel
         if: matrix.target == 'x86_64-unknown-linux-musl'
         uses: addnab/docker-run-action@v3
         with:
           image: alpine:latest
           options: -v ${{ github.workspace }}:/io -w /io
@@ -215,15 +215,15 @@
         with:
           python-version: ${{ env.PYTHON_VERSION }}
       - name: Build wheels
         uses: messense/maturin-action@v1
         with:
           target: ${{ matrix.platform.target }}
           manylinux: musllinux_1_2
-          args: --release --out dist -m ./crates/${{ env.CRATE_NAME }}/Cargo.toml
+          args: --release --out dist -m ./${{ env.CRATE_NAME }}/Cargo.toml
           maturin-version: "v0.13.0"
       - uses: uraimo/run-on-arch-action@master
         name: Install built wheel
         with:
           arch: ${{ matrix.platform.arch }}
           distro: alpine_latest
           githubToken: ${{ github.token }}
@@ -257,15 +257,15 @@
           python-version: pypy${{ matrix.python-version }}
       - name: Build wheels
         uses: messense/maturin-action@v1
         with:
           maturin-version: "v0.13.0"
           target: ${{ matrix.target }}
           manylinux: auto
-          args: --release --out dist -i pypy${{ matrix.python-version }} -m ./crates/${{ env.CRATE_NAME }}/Cargo.toml
+          args: --release --out dist -i pypy${{ matrix.python-version }} -m ./${{ env.CRATE_NAME }}/Cargo.toml
       - name: Install built wheel
         if: matrix.target == 'x86_64'
         run: |
           pip install dist/${{ env.CRATE_NAME }}-*.whl --force-reinstall
       - name: Upload wheels
         uses: actions/upload-artifact@v2
         with:
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/.github/workflows/ruff.yaml` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/.github/workflows/ruff.yaml`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/.gitignore` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/.gitignore`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/CODE_OF_CONDUCT.md` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/CONTRIBUTING.md` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/Cargo.lock` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -916,15 +916,15 @@
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
 name = "flake8-to-ruff"
-version = "0.0.94-dev.1"
+version = "0.0.99-dev.0"
 dependencies = [
  "anyhow",
  "clap 4.0.15",
  "configparser",
  "once_cell",
  "regex",
  "ruff",
@@ -2207,15 +2207,15 @@
  "untrusted",
  "web-sys",
  "winapi 0.3.9",
 ]
 
 [[package]]
 name = "ruff"
-version = "0.0.94"
+version = "0.0.99"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "bincode",
  "cacache",
  "chrono",
  "clap 4.0.15",
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/LICENSE` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/README.md` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,44 +85,86 @@
 ```
 
 Ruff also works with [pre-commit](https://pre-commit.com):
 
 ```yaml
 repos:
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.94
+    rev: v0.0.99
     hooks:
       - id: ruff
 ```
 
 <!-- TODO(charlie): Remove this message a few versions after v0.0.86. -->
 _Note: prior to `v0.0.86`, `ruff-pre-commit` used `lint` (rather than `ruff`) as the hook ID._
 
 ## Configuration
 
-Ruff is configurable both via `pyproject.toml` and the command line.
-
-For example, you could configure Ruff to only enforce a subset of rules with:
+Ruff is configurable both via `pyproject.toml` and the command line. If left unspecified, the
+default configuration is equivalent to:
 
 ```toml
 [tool.ruff]
 line-length = 88
+
+# Enable Flake's "E" and "F" codes by default.
 select = ["E", "F"]
-ignore = ["E501"]
-per-file-ignores = [
-    "__init__.py:F401",
-    "path/to/file.py:F401"
+ignore = []
+
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
 ]
+per-file-ignores = {}
+
+# Allow unused variables when underscore-prefixed.
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+# Assume Python 3.10.
+target-version = "py310"
+```
+
+As an example, the following would configure Ruff to (1) avoid checking for line-length
+violations (`E501`) and (2) ignore unused import rules in `__init__.py` files:
+
+```toml
+[tool.ruff]
+select = ["E", "F"]
+
+# Never enforce `E501`.
+ignore = ["E501"]
+
+# Ignore `F401` violations in any `__init__.py` file, and in `path/to/file.py`.
+per-file-ignores = {"__init__.py" = ["F401"], "path/to/file.py" = ["F401"]}
 ```
 
 Plugin configurations should be expressed as subsections, e.g.:
 
 ```toml
 [tool.ruff]
-line-length = 88
+# Add "Q" to the list of enabled codes.
+select = ["E", "F", "Q"]
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 ```
 
 Alternatively, common configuration settings can be provided via the command-line:
 
@@ -142,14 +184,16 @@
 
 Options:
       --config <CONFIG>
           Path to the `pyproject.toml` file to use for configuration
   -v, --verbose
           Enable verbose logging
   -q, --quiet
+          Only log errors
+  -s, --silent
           Disable all logging (but still exit with status code "1" upon detecting errors)
   -e, --exit-zero
           Exit with status code "0", even upon detecting errors
   -w, --watch
           Run in watch mode by re-running whenever files change
   -f, --fix
           Attempt to automatically fix lint errors
@@ -277,15 +321,15 @@
 | F707 | DefaultExceptNotLast | An `except:` block as not the last exception handler |  |
 | F722 | ForwardAnnotationSyntaxError | Syntax error in forward annotation: `...` |  |
 | F821 | UndefinedName | Undefined name `...` |  |
 | F822 | UndefinedExport | Undefined name `...` in `__all__` |  |
 | F823 | UndefinedLocal | Local variable `...` referenced before assignment |  |
 | F831 | DuplicateArgumentName | Duplicate argument name in function definition |  |
 | F841 | UnusedVariable | Local variable `...` is assigned to but never used |  |
-| F901 | RaiseNotImplemented | `raise NotImplemented` should be `raise NotImplementedError` |  |
+| F901 | RaiseNotImplemented | `raise NotImplemented` should be `raise NotImplementedError` | 🛠 |
 
 ### pycodestyle (error)
 
 | Code | Name | Message | Fix |
 | ---- | ---- | ------- | --- |
 | E402 | ModuleImportNotAtTopOfFile | Module level import not at top of file |  |
 | E501 | LineTooLong | Line too long (89 > 88 characters) |  |
@@ -391,29 +435,29 @@
 | N817 | CamelcaseImportedAsAcronym | Camelcase `...` imported as acronym `...` |  |
 | N818 | ErrorSuffixOnExceptionName | Exception name `...` should be named with an Error suffix |  |
 
 ### flake8-comprehensions
 
 | Code | Name | Message | Fix |
 | ---- | ---- | ------- | --- |
-| C400 | UnnecessaryGeneratorList | Unnecessary generator (rewrite as a `list` comprehension) |  |
-| C401 | UnnecessaryGeneratorSet | Unnecessary generator (rewrite as a `set` comprehension) |  |
-| C402 | UnnecessaryGeneratorDict | Unnecessary generator (rewrite as a `dict` comprehension) |  |
-| C403 | UnnecessaryListComprehensionSet | Unnecessary `list` comprehension (rewrite as a `set` comprehension) |  |
+| C400 | UnnecessaryGeneratorList | Unnecessary generator (rewrite as a `list` comprehension) | 🛠 |
+| C401 | UnnecessaryGeneratorSet | Unnecessary generator (rewrite as a `set` comprehension) | 🛠 |
+| C402 | UnnecessaryGeneratorDict | Unnecessary generator (rewrite as a `dict` comprehension) | 🛠 |
+| C403 | UnnecessaryListComprehensionSet | Unnecessary `list` comprehension (rewrite as a `set` comprehension) | 🛠 |
 | C404 | UnnecessaryListComprehensionDict | Unnecessary `list` comprehension (rewrite as a `dict` comprehension) |  |
-| C405 | UnnecessaryLiteralSet | Unnecessary `(list\|tuple)` literal (rewrite as a `set` literal) |  |
-| C406 | UnnecessaryLiteralDict | Unnecessary `(list\|tuple)` literal (rewrite as a `dict` literal) |  |
-| C408 | UnnecessaryCollectionCall | Unnecessary `(dict\|list\|tuple)` call (rewrite as a literal) |  |
-| C409 | UnnecessaryLiteralWithinTupleCall | Unnecessary `(list\|tuple)` literal passed to `tuple()` (remove the outer call to `tuple()`) |  |
-| C410 | UnnecessaryLiteralWithinListCall | Unnecessary `(list\|tuple)` literal passed to `list()` (rewrite as a `list` literal) |  |
-| C411 | UnnecessaryListCall | Unnecessary `list` call (remove the outer call to `list()`) |  |
+| C405 | UnnecessaryLiteralSet | Unnecessary `(list\|tuple)` literal (rewrite as a `set` literal) | 🛠 |
+| C406 | UnnecessaryLiteralDict | Unnecessary `(list\|tuple)` literal (rewrite as a `dict` literal) | 🛠 |
+| C408 | UnnecessaryCollectionCall | Unnecessary `(dict\|list\|tuple)` call (rewrite as a literal) | 🛠 |
+| C409 | UnnecessaryLiteralWithinTupleCall | Unnecessary `(list\|tuple)` literal passed to `tuple()` (remove the outer call to `tuple()`) | 🛠 |
+| C410 | UnnecessaryLiteralWithinListCall | Unnecessary `(list\|tuple)` literal passed to `list()` (rewrite as a `list` literal) | 🛠 |
+| C411 | UnnecessaryListCall | Unnecessary `list` call (remove the outer call to `list()`) | 🛠 |
 | C413 | UnnecessaryCallAroundSorted | Unnecessary `(list\|reversed)` call around `sorted()` |  |
 | C414 | UnnecessaryDoubleCastOrProcess | Unnecessary `(list\|reversed\|set\|sorted\|tuple)` call within `(list\|set\|sorted\|tuple)()` |  |
 | C415 | UnnecessarySubscriptReversal | Unnecessary subscript reversal of iterable within `(reversed\|set\|sorted)()` |  |
-| C416 | UnnecessaryComprehension | Unnecessary `(list\|set)` comprehension (rewrite using `(list\|set)()`) |  |
+| C416 | UnnecessaryComprehension | Unnecessary `(list\|set)` comprehension (rewrite using `(list\|set)()`) | 🛠 |
 | C417 | UnnecessaryMap | Unnecessary `map` usage (rewrite using a `(list\|set\|dict)` comprehension) |  |
 
 ### flake8-bugbear
 
 | Code | Name | Message | Fix |
 | ---- | ---- | ------- | --- |
 | B002 | UnaryPrefixIncrement | Python does not support the unary prefix increment. |  |
@@ -520,15 +564,15 @@
 - [`flake8-docstrings`](https://pypi.org/project/flake8-docstrings/)
 - [`flake8-builtins`](https://pypi.org/project/flake8-builtins/)
 - [`flake8-super`](https://pypi.org/project/flake8-super/)
 - [`flake8-print`](https://pypi.org/project/flake8-print/)
 - [`flake8-quotes`](https://pypi.org/project/flake8-quotes/)
 - [`flake8-comprehensions`](https://pypi.org/project/flake8-comprehensions/)
 - [`flake8-bugbear`](https://pypi.org/project/flake8-bugbear/) (10/32)
-- [`pyupgrade`](https://pypi.org/project/pyupgrade/) (8/34)
+- [`pyupgrade`](https://pypi.org/project/pyupgrade/) (10/34)
 - [`autoflake`](https://pypi.org/project/autoflake/) (1/7)
 
 Beyond rule-set parity, Ruff suffers from the following limitations vis-à-vis Flake8:
 
 1. Ruff does not yet support a few Python 3.9 and 3.10 language features, including structural
    pattern matching and parenthesized context managers.
 2. Flake8 has a plugin architecture and supports writing custom lint rules. (To date, popular Flake8
@@ -544,15 +588,15 @@
 - [`flake8-super`](https://pypi.org/project/flake8-super/)
 - [`flake8-print`](https://pypi.org/project/flake8-print/)
 - [`flake8-quotes`](https://pypi.org/project/flake8-quotes/)
 - [`flake8-comprehensions`](https://pypi.org/project/flake8-comprehensions/)
 - [`flake8-bugbear`](https://pypi.org/project/flake8-bugbear/) (10/32)
 
 Ruff also implements the functionality that you get from [`yesqa`](https://github.com/asottile/yesqa),
-and a subset of the rules implemented in [`pyupgrade`](https://pypi.org/project/pyupgrade/) (8/34).
+and a subset of the rules implemented in [`pyupgrade`](https://pypi.org/project/pyupgrade/) (10/34).
 
 If you're looking to use Ruff, but rely on an unsupported Flake8 plugin, free to file an Issue.
 
 ### Do I need to install Rust to use Ruff?
 
 Nope! Ruff is available as [`ruff`](https://pypi.org/project/ruff/) on PyPI:
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/examples/generate_check_code_prefix.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/examples/generate_check_code_prefix.rs`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     let mut gen = scope
         .new_enum("CheckCodePrefix")
         .vis("pub")
         .derive("EnumString")
         .derive("Debug")
         .derive("PartialEq")
         .derive("Eq")
+        .derive("PartialOrd")
+        .derive("Ord")
         .derive("Clone")
         .derive("Serialize")
         .derive("Deserialize");
     for (prefix, _) in &prefix_to_codes {
         gen = gen.push_variant(Variant::new(prefix.to_string()));
     }
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/examples/generate_rules_table.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/examples/generate_rules_table.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/examples/generate_source_code.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/examples/generate_source_code.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/pyproject.toml` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/B006_B008.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/B006_B008.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/B007.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/B007.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/B014.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/B014.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/B017.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/B017.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/D.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/D.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E501.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E501.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E711.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E711.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E712.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E712.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E713.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E713.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E721.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E721.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/E741.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/E741.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F401_0.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F401_0.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/F821_0.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/F821_0.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/M001.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/M001.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/U004.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/U004.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/U008.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/U008.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/canonical_google_examples.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/canonical_google_examples.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/canonical_numpy_examples.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/canonical_numpy_examples.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_doubles.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_doubles.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_singles.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/flake8_quotes/docstring_singles.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/pyproject.toml` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/resources/test/fixtures/sections.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/resources/test/fixtures/sections.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/scripts/poetry.lock` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/scripts/poetry.lock`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/scripts/run_flake8.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/scripts/run_flake8.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/setup.py` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/setup.py`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/ast/helpers.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/ast/helpers.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/ast/operations.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/ast/operations.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/ast/relocate.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/ast/relocate.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/ast/types.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/ast/types.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/ast/visitor.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/ast/visitor.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/autofix/fixer.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/autofix/fixer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 use itertools::Itertools;
 use rustpython_parser::ast::Location;
 
 use crate::autofix::{Fix, Patch};
 use crate::checks::Check;
 
+// TODO(charlie): The model here is awkward because `Apply` is only relevant at
+// higher levels in the execution flow.
 #[derive(Hash)]
 pub enum Mode {
     Generate,
     Apply,
     None,
 }
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/autofix/helpers.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/autofix/helpers.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/autofix/mod.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/autofix/mod.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/cache.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/cache.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/check_ast.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/check_ast.rs`

 * *Files 4% similar despite different names*

```diff
@@ -33,21 +33,24 @@
 use crate::visibility::{module_visibility, transition_scope, Modifier, Visibility, VisibleScope};
 use crate::{
     docstrings, flake8_bugbear, flake8_builtins, flake8_comprehensions, flake8_print, pep8_naming,
     pycodestyle, pydocstyle, pyflakes, pyupgrade,
 };
 
 const GLOBAL_SCOPE_INDEX: usize = 0;
-const TRACK_FROM_IMPORTS: [&str; 6] = [
+const TRACK_FROM_IMPORTS: [&str; 9] = [
     "collections",
     "collections.abc",
     "contextlib",
     "re",
     "typing",
+    "typing.io",
     "typing.re",
+    "typing_extensions",
+    "weakref",
 ];
 
 pub struct Checker<'a> {
     // Input data.
     path: &'a Path,
     autofix: &'a fixer::Mode,
     pub(crate) settings: &'a Settings,
@@ -122,20 +125,29 @@
             from_imports: Default::default(),
         }
     }
 
     /// Return `true` if a patch should be generated under the given autofix
     /// `Mode`.
     pub fn patch(&self) -> bool {
-        self.autofix.patch()
+        // TODO(charlie): We can't fix errors in f-strings until RustPython adds
+        // location data.
+        self.autofix.patch() && self.in_f_string.is_none()
     }
 
     /// Return `true` if the `Expr` is a reference to `typing.${target}`.
     pub fn match_typing_module(&self, expr: &Expr, target: &str) -> bool {
         match_name_or_attr_from_module(expr, target, "typing", self.from_imports.get("typing"))
+            || (typing::in_extensions(target)
+                && match_name_or_attr_from_module(
+                    expr,
+                    target,
+                    "typing_extensions",
+                    self.from_imports.get("typing_extensions"),
+                ))
     }
 }
 
 impl<'a, 'b> Visitor<'b> for Checker<'a>
 where
     'b: 'a,
 {
@@ -701,17 +713,15 @@
                         }
                     }
                 }
             }
             StmtKind::Raise { exc, .. } => {
                 if self.settings.enabled.contains(&CheckCode::F901) {
                     if let Some(expr) = exc {
-                        if let Some(check) = pyflakes::checks::raise_not_implemented(expr) {
-                            self.checks.push(check);
-                        }
+                        pyflakes::plugins::raise_not_implemented(self, expr);
                     }
                 }
             }
             StmtKind::AugAssign { target, .. } => {
                 self.handle_node_load(target);
             }
             StmtKind::If { test, .. } => {
@@ -975,142 +985,210 @@
                 {
                     flake8_print::plugins::print_call(self, expr, func);
                 }
 
                 // flake8-comprehensions
                 if self.settings.enabled.contains(&CheckCode::C400) {
                     if let Some(check) = flake8_comprehensions::checks::unnecessary_generator_list(
-                        expr, func, args, keywords,
+                        expr,
+                        func,
+                        args,
+                        keywords,
+                        self.locator,
+                        self.patch(),
+                        self.locate_check(Range::from_located(expr)),
                     ) {
                         self.checks.push(check);
                     };
                 }
 
                 if self.settings.enabled.contains(&CheckCode::C401) {
                     if let Some(check) = flake8_comprehensions::checks::unnecessary_generator_set(
-                        expr, func, args, keywords,
+                        expr,
+                        func,
+                        args,
+                        keywords,
+                        self.locator,
+                        self.patch(),
+                        self.locate_check(Range::from_located(expr)),
                     ) {
                         self.checks.push(check);
                     };
                 }
 
                 if self.settings.enabled.contains(&CheckCode::C402) {
                     if let Some(check) = flake8_comprehensions::checks::unnecessary_generator_dict(
-                        expr, func, args, keywords,
+                        expr,
+                        func,
+                        args,
+                        keywords,
+                        self.locator,
+                        self.patch(),
+                        self.locate_check(Range::from_located(expr)),
                     ) {
                         self.checks.push(check);
                     };
                 }
 
                 if self.settings.enabled.contains(&CheckCode::C403) {
                     if let Some(check) =
                         flake8_comprehensions::checks::unnecessary_list_comprehension_set(
-                            expr, func, args, keywords,
+                            expr,
+                            func,
+                            args,
+                            keywords,
+                            self.locator,
+                            self.patch(),
+                            self.locate_check(Range::from_located(expr)),
                         )
                     {
                         self.checks.push(check);
                     };
                 }
 
                 if self.settings.enabled.contains(&CheckCode::C404) {
                     if let Some(check) =
                         flake8_comprehensions::checks::unnecessary_list_comprehension_dict(
-                            expr, func, args, keywords,
+                            func,
+                            args,
+                            keywords,
+                            self.locate_check(Range::from_located(expr)),
                         )
                     {
                         self.checks.push(check);
                     };
                 }
 
                 if self.settings.enabled.contains(&CheckCode::C405) {
                     if let Some(check) = flake8_comprehensions::checks::unnecessary_literal_set(
-                        expr, func, args, keywords,
+                        expr,
+                        func,
+                        args,
+                        keywords,
+                        self.locator,
+                        self.patch(),
+                        self.locate_check(Range::from_located(expr)),
                     ) {
                         self.checks.push(check);
                     };
                 }
 
                 if self.settings.enabled.contains(&CheckCode::C406) {
                     if let Some(check) = flake8_comprehensions::checks::unnecessary_literal_dict(
-                        expr, func, args, keywords,
+                        expr,
+                        func,
+                        args,
+                        keywords,
+                        self.locator,
+                        self.patch(),
+                        self.locate_check(Range::from_located(expr)),
                     ) {
                         self.checks.push(check);
                     };
                 }
 
                 if self.settings.enabled.contains(&CheckCode::C408) {
                     if let Some(check) = flake8_comprehensions::checks::unnecessary_collection_call(
-                        expr, func, args, keywords,
+                        expr,
+                        func,
+                        args,
+                        keywords,
+                        self.locator,
+                        self.patch(),
+                        self.locate_check(Range::from_located(expr)),
                     ) {
                         self.checks.push(check);
                     };
                 }
 
                 if self.settings.enabled.contains(&CheckCode::C409) {
                     if let Some(check) =
                         flake8_comprehensions::checks::unnecessary_literal_within_tuple_call(
-                            expr, func, args,
+                            expr,
+                            func,
+                            args,
+                            self.locator,
+                            self.patch(),
+                            self.locate_check(Range::from_located(expr)),
                         )
                     {
                         self.checks.push(check);
                     };
                 }
 
                 if self.settings.enabled.contains(&CheckCode::C410) {
                     if let Some(check) =
                         flake8_comprehensions::checks::unnecessary_literal_within_list_call(
-                            expr, func, args,
+                            expr,
+                            func,
+                            args,
+                            self.locator,
+                            self.patch(),
+                            self.locate_check(Range::from_located(expr)),
                         )
                     {
                         self.checks.push(check);
                     };
                 }
 
                 if self.settings.enabled.contains(&CheckCode::C411) {
-                    if let Some(check) =
-                        flake8_comprehensions::checks::unnecessary_list_call(expr, func, args)
-                    {
+                    if let Some(check) = flake8_comprehensions::checks::unnecessary_list_call(
+                        expr,
+                        func,
+                        args,
+                        self.locator,
+                        self.patch(),
+                        self.locate_check(Range::from_located(expr)),
+                    ) {
                         self.checks.push(check);
                     };
                 }
 
                 if self.settings.enabled.contains(&CheckCode::C413) {
                     if let Some(check) =
                         flake8_comprehensions::checks::unnecessary_call_around_sorted(
-                            expr, func, args,
+                            func,
+                            args,
+                            self.locate_check(Range::from_located(expr)),
                         )
                     {
                         self.checks.push(check);
                     };
                 }
 
                 if self.settings.enabled.contains(&CheckCode::C414) {
                     if let Some(check) =
                         flake8_comprehensions::checks::unnecessary_double_cast_or_process(
-                            expr, func, args,
+                            func,
+                            args,
+                            self.locate_check(Range::from_located(expr)),
                         )
                     {
                         self.checks.push(check);
                     };
                 }
 
                 if self.settings.enabled.contains(&CheckCode::C415) {
                     if let Some(check) =
                         flake8_comprehensions::checks::unnecessary_subscript_reversal(
-                            expr, func, args,
+                            func,
+                            args,
+                            self.locate_check(Range::from_located(expr)),
                         )
                     {
                         self.checks.push(check);
                     };
                 }
 
                 if self.settings.enabled.contains(&CheckCode::C417) {
-                    if let Some(check) =
-                        flake8_comprehensions::checks::unnecessary_map(expr, func, args)
-                    {
+                    if let Some(check) = flake8_comprehensions::checks::unnecessary_map(
+                        func,
+                        args,
+                        self.locate_check(Range::from_located(expr)),
+                    ) {
                         self.checks.push(check);
                     };
                 }
 
                 // pyupgrade
                 if self.settings.enabled.contains(&CheckCode::U002)
                     && self.settings.target_version >= PythonVersion::Py310
@@ -1279,15 +1357,20 @@
                     self.visit_expr(expr);
                 }
             }
 
             ExprKind::ListComp { elt, generators } | ExprKind::SetComp { elt, generators } => {
                 if self.settings.enabled.contains(&CheckCode::C416) {
                     if let Some(check) = flake8_comprehensions::checks::unnecessary_comprehension(
-                        expr, elt, generators,
+                        expr,
+                        elt,
+                        generators,
+                        self.locator,
+                        self.patch(),
+                        self.locate_check(Range::from_located(expr)),
                     ) {
                         self.checks.push(check);
                     };
                 }
                 self.push_scope(Scope::new(ScopeKind::Generator))
             }
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/check_lines.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/check_lines.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/check_tokens.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/check_tokens.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/checks.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/checks.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1457,22 +1457,34 @@
                 | CheckKind::NoOverIndentation
                 | CheckKind::NoSurroundingWhitespace
                 | CheckKind::NoUnderIndentation
                 | CheckKind::OneBlankLineAfterClass(_)
                 | CheckKind::OneBlankLineBeforeClass(_)
                 | CheckKind::PPrintFound
                 | CheckKind::PrintFound
+                | CheckKind::RaiseNotImplemented
                 | CheckKind::SectionNameEndsInColon(_)
                 | CheckKind::SectionNotOverIndented(_)
                 | CheckKind::SectionUnderlineAfterName(_)
                 | CheckKind::SectionUnderlineMatchesSectionLength(_)
                 | CheckKind::SectionUnderlineNotOverIndented(_)
                 | CheckKind::SuperCallWithParameters
                 | CheckKind::TypeOfPrimitive(_)
                 | CheckKind::UnnecessaryAbspath
+                | CheckKind::UnnecessaryCollectionCall(_)
+                | CheckKind::UnnecessaryComprehension(_)
+                | CheckKind::UnnecessaryGeneratorDict
+                | CheckKind::UnnecessaryGeneratorList
+                | CheckKind::UnnecessaryGeneratorSet
+                | CheckKind::UnnecessaryListCall
+                | CheckKind::UnnecessaryListComprehensionSet
+                | CheckKind::UnnecessaryLiteralDict(_)
+                | CheckKind::UnnecessaryLiteralSet(_)
+                | CheckKind::UnnecessaryLiteralWithinListCall(_)
+                | CheckKind::UnnecessaryLiteralWithinTupleCall(_)
                 | CheckKind::UnusedImport(_, false)
                 | CheckKind::UnusedLoopControlVariable(_)
                 | CheckKind::UnusedNOQA(_)
                 | CheckKind::UsePEP585Annotation(_)
                 | CheckKind::UsePEP604Annotation
                 | CheckKind::UselessMetaclassType
                 | CheckKind::UselessObjectInheritance(_)
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/checks_gen.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/checks_gen.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 //! File automatically generated by examples/generate_check_code_prefix.rs.
 
 use serde::{Deserialize, Serialize};
 use strum_macros::{AsRefStr, EnumString};
 
 use crate::checks::CheckCode;
 
-#[derive(AsRefStr, EnumString, Debug, PartialEq, Eq, Clone, Serialize, Deserialize)]
+#[derive(
+    AsRefStr, EnumString, Debug, PartialEq, Eq, PartialOrd, Ord, Clone, Serialize, Deserialize,
+)]
 pub enum CheckCodePrefix {
     A,
     A0,
     A00,
     A001,
     A002,
     A003,
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/cli.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/cli.rs`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 use std::path::PathBuf;
 
 use clap::{command, Parser};
 use log::warn;
 use regex::Regex;
 
 use crate::checks_gen::CheckCodePrefix;
+use crate::logging::LogLevel;
 use crate::printer::SerializationFormat;
 use crate::settings::configuration::Configuration;
 use crate::settings::types::{PatternPrefixPair, PythonVersion};
 
 #[derive(Debug, Parser)]
 #[command(author, about = "ruff: An extremely fast Python linter.")]
 #[command(version)]
@@ -89,14 +90,27 @@
     #[arg(long, hide = true)]
     pub autoformat: bool,
     /// The name of the file when passing it through stdin.
     #[arg(long)]
     pub stdin_filename: Option<String>,
 }
 
+/// Map the CLI settings to a `LogLevel`.
+pub fn extract_log_level(cli: &Cli) -> LogLevel {
+    if cli.silent {
+        LogLevel::Silent
+    } else if cli.quiet {
+        LogLevel::Quiet
+    } else if cli.verbose {
+        LogLevel::Verbose
+    } else {
+        LogLevel::Default
+    }
+}
+
 pub enum Warnable {
     Select,
     ExtendSelect,
 }
 
 impl fmt::Display for Warnable {
     fn fmt(&self, fmt: &mut fmt::Formatter) -> fmt::Result {
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/code_gen.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/code_gen.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/cst/helpers.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/cst/helpers.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/docstrings/extraction.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/docstrings/extraction.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/docstrings/google.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/docstrings/google.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/docstrings/helpers.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/docstrings/helpers.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/docstrings/numpy.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/docstrings/numpy.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/docstrings/sections.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/docstrings/sections.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/docstrings/styles.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/docstrings/styles.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/plugins/assert_false.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/plugins/assert_false.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use rustpython_ast::{Constant, Expr, ExprContext, ExprKind, Stmt, StmtKind};
 
-use crate::ast::types::Range;
+use crate::ast::types::{CheckLocator, Range};
 use crate::autofix::Fix;
 use crate::check_ast::Checker;
 use crate::checks::{Check, CheckKind};
 use crate::code_gen::SourceGenerator;
 
 fn assertion_error(msg: &Option<Box<Expr>>) -> Stmt {
     Stmt::new(
@@ -38,15 +38,18 @@
 
 pub fn assert_false(checker: &mut Checker, stmt: &Stmt, test: &Expr, msg: &Option<Box<Expr>>) {
     if let ExprKind::Constant {
         value: Constant::Bool(false),
         ..
     } = &test.node
     {
-        let mut check = Check::new(CheckKind::DoNotAssertFalse, Range::from_located(test));
+        let mut check = Check::new(
+            CheckKind::DoNotAssertFalse,
+            checker.locate_check(Range::from_located(test)),
+        );
         if checker.patch() {
             let mut generator = SourceGenerator::new();
             if let Ok(()) = generator.unparse_stmt(&assertion_error(msg)) {
                 if let Ok(content) = generator.generate() {
                     check.amend(Fix::replacement(
                         content,
                         stmt.location,
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/plugins/assert_raises_exception.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/plugins/assert_raises_exception.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use rustpython_ast::{ExprKind, Stmt, Withitem};
 
 use crate::ast::helpers::match_name_or_attr;
-use crate::ast::types::Range;
+use crate::ast::types::{CheckLocator, Range};
 use crate::check_ast::Checker;
 use crate::checks::{Check, CheckKind};
 
 /// B017
 pub fn assert_raises_exception(checker: &mut Checker, stmt: &Stmt, items: &[Withitem]) {
     if let Some(item) = items.first() {
         let item_context = &item.context_expr;
@@ -13,13 +13,13 @@
             if match_name_or_attr(func, "assertRaises")
                 && args.len() == 1
                 && match_name_or_attr(args.first().unwrap(), "Exception")
                 && item.optional_vars.is_none()
             {
                 checker.add_check(Check::new(
                     CheckKind::NoAssertRaisesException,
-                    Range::from_located(stmt),
+                    checker.locate_check(Range::from_located(stmt)),
                 ));
             }
         }
     }
 }
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/plugins/duplicate_exceptions.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/plugins/duplicate_exceptions.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/plugins/mod.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/plugins/mod.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/plugins/mutable_argument_default.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/plugins/mutable_argument_default.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/plugins/redundant_tuple_in_exception_handler.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/plugins/redundant_tuple_in_exception_handler.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/plugins/unary_prefix_increment.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/plugins/unary_prefix_increment.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 use rustpython_ast::{Expr, ExprKind, Unaryop};
 
-use crate::ast::types::Range;
+use crate::ast::types::{CheckLocator, Range};
 use crate::check_ast::Checker;
 use crate::checks::{Check, CheckKind};
 
 /// B002
 pub fn unary_prefix_increment(checker: &mut Checker, expr: &Expr, op: &Unaryop, operand: &Expr) {
     if matches!(op, Unaryop::UAdd) {
         if let ExprKind::UnaryOp { op, .. } = &operand.node {
             if matches!(op, Unaryop::UAdd) {
                 checker.add_check(Check::new(
                     CheckKind::UnaryPrefixIncrement,
-                    Range::from_located(expr),
+                    checker.locate_check(Range::from_located(expr)),
                 ))
             }
         }
     }
 }
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_bugbear/plugins/unused_loop_control_variable.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_bugbear/plugins/unused_loop_control_variable.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use std::collections::BTreeMap;
 
 use rustpython_ast::{Expr, ExprKind, Stmt};
 
-use crate::ast::types::Range;
+use crate::ast::types::{CheckLocator, Range};
 use crate::ast::visitor;
 use crate::ast::visitor::Visitor;
 use crate::autofix::Fix;
 use crate::check_ast::Checker;
 use crate::checks::{Check, CheckKind};
 
 /// Identify all `ExprKind::Name` nodes in an AST.
@@ -60,15 +60,15 @@
         // Ignore any names that are actually used in the loop body.
         if used_names.contains_key(name) {
             continue;
         }
 
         let mut check = Check::new(
             CheckKind::UnusedLoopControlVariable(name.to_string()),
-            Range::from_located(expr),
+            checker.locate_check(Range::from_located(expr)),
         );
         if checker.patch() {
             // Prefix the variable name with an underscore.
             check.amend(Fix::replacement(
                 format!("_{name}"),
                 expr.location,
                 expr.end_location.unwrap(),
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_builtins/checks.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_builtins/checks.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_comprehensions/checks.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_comprehensions/checks.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+use log::error;
 use num_bigint::BigInt;
 use rustpython_ast::{
     Comprehension, Constant, Expr, ExprKind, Keyword, KeywordData, Located, Unaryop,
 };
 
 use crate::ast::types::Range;
 use crate::checks::{Check, CheckKind};
+use crate::flake8_comprehensions::fixes;
+use crate::source_code_locator::SourceCodeLocator;
 
 fn function_name(func: &Expr) -> Option<&str> {
     if let ExprKind::Name { id, .. } = &func.node {
         Some(id)
     } else {
         None
     }
@@ -45,280 +48,375 @@
 
 /// C400 (`list(generator)`)
 pub fn unnecessary_generator_list(
     expr: &Expr,
     func: &Expr,
     args: &[Expr],
     keywords: &[Keyword],
+    locator: &SourceCodeLocator,
+    fix: bool,
+    location: Range,
 ) -> Option<Check> {
     let argument = exactly_one_argument_with_matching_function("list", func, args, keywords)?;
     if let ExprKind::GeneratorExp { .. } = argument {
-        return Some(Check::new(
-            CheckKind::UnnecessaryGeneratorList,
-            Range::from_located(expr),
-        ));
+        let mut check = Check::new(CheckKind::UnnecessaryGeneratorList, location);
+        if fix {
+            match fixes::fix_unnecessary_generator_list(locator, expr) {
+                Ok(fix) => check.amend(fix),
+                Err(e) => error!("Failed to generate fix: {}", e),
+            }
+        }
+        return Some(check);
     }
     None
 }
 
 /// C401 (`set(generator)`)
 pub fn unnecessary_generator_set(
     expr: &Expr,
     func: &Expr,
     args: &[Expr],
     keywords: &[Keyword],
+    locator: &SourceCodeLocator,
+    fix: bool,
+    location: Range,
 ) -> Option<Check> {
     let argument = exactly_one_argument_with_matching_function("set", func, args, keywords)?;
     if let ExprKind::GeneratorExp { .. } = argument {
-        return Some(Check::new(
-            CheckKind::UnnecessaryGeneratorSet,
-            Range::from_located(expr),
-        ));
+        let mut check = Check::new(CheckKind::UnnecessaryGeneratorSet, location);
+        if fix {
+            match fixes::fix_unnecessary_generator_set(locator, expr) {
+                Ok(fix) => check.amend(fix),
+                Err(e) => error!("Failed to generate fix: {}", e),
+            }
+        }
+        return Some(check);
     }
     None
 }
 
 /// C402 (`dict((x, y) for x, y in iterable)`)
 pub fn unnecessary_generator_dict(
     expr: &Expr,
     func: &Expr,
     args: &[Expr],
     keywords: &[Keyword],
+    locator: &SourceCodeLocator,
+    fix: bool,
+    location: Range,
 ) -> Option<Check> {
     let argument = exactly_one_argument_with_matching_function("dict", func, args, keywords)?;
     if let ExprKind::GeneratorExp { elt, .. } = argument {
         match &elt.node {
             ExprKind::Tuple { elts, .. } if elts.len() == 2 => {
-                return Some(Check::new(
-                    CheckKind::UnnecessaryGeneratorDict,
-                    Range::from_located(expr),
-                ));
+                let mut check = Check::new(CheckKind::UnnecessaryGeneratorDict, location);
+                if fix {
+                    match fixes::fix_unnecessary_generator_dict(locator, expr) {
+                        Ok(fix) => check.amend(fix),
+                        Err(e) => error!("Failed to generate fix: {}", e),
+                    }
+                }
+                return Some(check);
             }
             _ => {}
         }
     }
     None
 }
 
 /// C403 (`set([...])`)
 pub fn unnecessary_list_comprehension_set(
     expr: &Expr,
     func: &Expr,
     args: &[Expr],
     keywords: &[Keyword],
+    locator: &SourceCodeLocator,
+    fix: bool,
+    location: Range,
 ) -> Option<Check> {
     let argument = exactly_one_argument_with_matching_function("set", func, args, keywords)?;
     if let ExprKind::ListComp { .. } = &argument {
-        return Some(Check::new(
-            CheckKind::UnnecessaryListComprehensionSet,
-            Range::from_located(expr),
-        ));
+        let mut check = Check::new(CheckKind::UnnecessaryListComprehensionSet, location);
+        if fix {
+            match fixes::fix_unnecessary_list_comprehension_set(locator, expr) {
+                Ok(fix) => check.amend(fix),
+                Err(e) => error!("Failed to generate fix: {}", e),
+            }
+        }
+        return Some(check);
     }
     None
 }
 
 /// C404 (`dict([...])`)
 pub fn unnecessary_list_comprehension_dict(
-    expr: &Expr,
     func: &Expr,
     args: &[Expr],
     keywords: &[Keyword],
+    location: Range,
 ) -> Option<Check> {
     let argument = exactly_one_argument_with_matching_function("dict", func, args, keywords)?;
     if let ExprKind::ListComp { elt, .. } = &argument {
         match &elt.node {
             ExprKind::Tuple { elts, .. } if elts.len() == 2 => {
                 return Some(Check::new(
                     CheckKind::UnnecessaryListComprehensionDict,
-                    Range::from_located(expr),
+                    location,
                 ));
             }
             _ => {}
         }
     }
     None
 }
 
 /// C405 (`set([1, 2])`)
 pub fn unnecessary_literal_set(
     expr: &Expr,
     func: &Expr,
     args: &[Expr],
     keywords: &[Keyword],
+    locator: &SourceCodeLocator,
+    fix: bool,
+    location: Range,
 ) -> Option<Check> {
     let argument = exactly_one_argument_with_matching_function("set", func, args, keywords)?;
     let kind = match argument {
         ExprKind::List { .. } => "list",
         ExprKind::Tuple { .. } => "tuple",
         _ => return None,
     };
-    Some(Check::new(
-        CheckKind::UnnecessaryLiteralSet(kind.to_string()),
-        Range::from_located(expr),
-    ))
+    let mut check = Check::new(CheckKind::UnnecessaryLiteralSet(kind.to_string()), location);
+    if fix {
+        match fixes::fix_unnecessary_literal_set(locator, expr) {
+            Ok(fix) => check.amend(fix),
+            Err(e) => error!("Failed to generate fix: {}", e),
+        }
+    }
+    Some(check)
 }
 
 /// C406 (`dict([(1, 2)])`)
 pub fn unnecessary_literal_dict(
     expr: &Expr,
     func: &Expr,
     args: &[Expr],
     keywords: &[Keyword],
+    locator: &SourceCodeLocator,
+    fix: bool,
+    location: Range,
 ) -> Option<Check> {
     let argument = exactly_one_argument_with_matching_function("dict", func, args, keywords)?;
     let (kind, elts) = match argument {
         ExprKind::Tuple { elts, .. } => ("tuple", elts),
         ExprKind::List { elts, .. } => ("list", elts),
         _ => return None,
     };
-
-    if let Some(elt) = elts.first() {
-        // dict((1, 2), ...)) or dict([(1, 2), ...])
-        if !matches!(&elt.node, ExprKind::Tuple { elts, .. } if elts.len() == 2) {
-            return None;
-        }
+    // Accept `dict((1, 2), ...))` `dict([(1, 2), ...])`.
+    if !elts
+        .iter()
+        .all(|elt| matches!(&elt.node, ExprKind::Tuple { elts, .. } if elts.len() == 2))
+    {
+        return None;
     }
-
-    Some(Check::new(
+    let mut check = Check::new(
         CheckKind::UnnecessaryLiteralDict(kind.to_string()),
-        Range::from_located(expr),
-    ))
+        location,
+    );
+    if fix {
+        match fixes::fix_unnecessary_literal_dict(locator, expr) {
+            Ok(fix) => check.amend(fix),
+            Err(e) => error!("Failed to generate fix: {}", e),
+        }
+    }
+    Some(check)
 }
 
 /// C408
 pub fn unnecessary_collection_call(
     expr: &Expr,
     func: &Expr,
     args: &[Expr],
     keywords: &[Located<KeywordData>],
+    locator: &SourceCodeLocator,
+    fix: bool,
+    location: Range,
 ) -> Option<Check> {
     if !args.is_empty() {
         return None;
     }
     let id = function_name(func)?;
     match id {
-        "dict" if keywords.is_empty() || keywords.iter().all(|kw| kw.node.arg.is_some()) => (),
+        "dict" if keywords.is_empty() || keywords.iter().all(|kw| kw.node.arg.is_some()) => {
+            // `dict()` or `dict(a=1)` (as opposed to `dict(**a)`)
+        }
         "list" | "tuple" => {
-            // list() or tuple()
+            // `list()` or `tuple()`
         }
         _ => return None,
     };
-    Some(Check::new(
+    let mut check = Check::new(
         CheckKind::UnnecessaryCollectionCall(id.to_string()),
-        Range::from_located(expr),
-    ))
+        location,
+    );
+    if fix {
+        match fixes::fix_unnecessary_collection_call(locator, expr) {
+            Ok(fix) => check.amend(fix),
+            Err(e) => error!("Failed to generate fix: {}", e),
+        }
+    }
+    Some(check)
 }
 
 /// C409
 pub fn unnecessary_literal_within_tuple_call(
     expr: &Expr,
     func: &Expr,
     args: &[Expr],
+    locator: &SourceCodeLocator,
+    fix: bool,
+    location: Range,
 ) -> Option<Check> {
     let argument = first_argument_with_matching_function("tuple", func, args)?;
     let argument_kind = match argument {
         ExprKind::Tuple { .. } => "tuple",
         ExprKind::List { .. } => "list",
         _ => return None,
     };
-    Some(Check::new(
+    let mut check = Check::new(
         CheckKind::UnnecessaryLiteralWithinTupleCall(argument_kind.to_string()),
-        Range::from_located(expr),
-    ))
+        location,
+    );
+    if fix {
+        match fixes::fix_unnecessary_literal_within_tuple_call(locator, expr) {
+            Ok(fix) => check.amend(fix),
+            Err(e) => error!("Failed to generate fix: {}", e),
+        }
+    }
+    Some(check)
 }
 
 /// C410
 pub fn unnecessary_literal_within_list_call(
     expr: &Expr,
     func: &Expr,
     args: &[Expr],
+    locator: &SourceCodeLocator,
+    fix: bool,
+    location: Range,
 ) -> Option<Check> {
     let argument = first_argument_with_matching_function("list", func, args)?;
     let argument_kind = match argument {
         ExprKind::Tuple { .. } => "tuple",
         ExprKind::List { .. } => "list",
         _ => return None,
     };
-    Some(Check::new(
+    let mut check = Check::new(
         CheckKind::UnnecessaryLiteralWithinListCall(argument_kind.to_string()),
-        Range::from_located(expr),
-    ))
+        location,
+    );
+    if fix {
+        match fixes::fix_unnecessary_literal_within_list_call(locator, expr) {
+            Ok(fix) => check.amend(fix),
+            Err(e) => error!("Failed to generate fix: {}", e),
+        }
+    }
+    Some(check)
 }
 
 /// C411
-pub fn unnecessary_list_call(expr: &Expr, func: &Expr, args: &[Expr]) -> Option<Check> {
+pub fn unnecessary_list_call(
+    expr: &Expr,
+    func: &Expr,
+    args: &[Expr],
+    locator: &SourceCodeLocator,
+    fix: bool,
+    location: Range,
+) -> Option<Check> {
     let argument = first_argument_with_matching_function("list", func, args)?;
     if let ExprKind::ListComp { .. } = argument {
-        return Some(Check::new(
-            CheckKind::UnnecessaryListCall,
-            Range::from_located(expr),
-        ));
+        let mut check = Check::new(CheckKind::UnnecessaryListCall, location);
+        if fix {
+            match fixes::fix_unnecessary_list_call(locator, expr) {
+                Ok(fix) => check.amend(fix),
+                Err(e) => error!("Failed to generate fix: {}", e),
+            }
+        }
+        return Some(check);
     }
     None
 }
 
 /// C413
-pub fn unnecessary_call_around_sorted(expr: &Expr, func: &Expr, args: &[Expr]) -> Option<Check> {
+pub fn unnecessary_call_around_sorted(
+    func: &Expr,
+    args: &[Expr],
+    location: Range,
+) -> Option<Check> {
     let outer = function_name(func)?;
     if !(outer == "list" || outer == "reversed") {
         return None;
     }
     if let ExprKind::Call { func, .. } = &args.first()?.node {
         if function_name(func)? == "sorted" {
             return Some(Check::new(
                 CheckKind::UnnecessaryCallAroundSorted(outer.to_string()),
-                Range::from_located(expr),
+                location,
             ));
         }
     }
     None
 }
 
 /// C414
 pub fn unnecessary_double_cast_or_process(
-    expr: &Expr,
     func: &Expr,
     args: &[Expr],
+    location: Range,
 ) -> Option<Check> {
     let outer = function_name(func)?;
     if !["list", "tuple", "set", "reversed", "sorted"].contains(&outer) {
         return None;
     }
 
-    fn new_check(inner: &str, outer: &str, expr: &Expr) -> Check {
+    fn new_check(inner: &str, outer: &str, location: Range) -> Check {
         Check::new(
             CheckKind::UnnecessaryDoubleCastOrProcess(inner.to_string(), outer.to_string()),
-            Range::from_located(expr),
+            location,
         )
     }
 
     if let ExprKind::Call { func, .. } = &args.first()?.node {
         let inner = function_name(func)?;
         // Ex) set(tuple(...))
         if (outer == "set" || outer == "sorted")
             && (inner == "list" || inner == "tuple" || inner == "reversed" || inner == "sorted")
         {
-            return Some(new_check(inner, outer, expr));
+            return Some(new_check(inner, outer, location));
         }
 
         // Ex) list(tuple(...))
         if (outer == "list" || outer == "tuple") && (inner == "list" || inner == "tuple") {
-            return Some(new_check(inner, outer, expr));
+            return Some(new_check(inner, outer, location));
         }
 
         // Ex) set(set(...))
         if outer == "set" && inner == "set" {
-            return Some(new_check(inner, outer, expr));
+            return Some(new_check(inner, outer, location));
         }
     }
     None
 }
 
 /// C415
-pub fn unnecessary_subscript_reversal(expr: &Expr, func: &Expr, args: &[Expr]) -> Option<Check> {
+pub fn unnecessary_subscript_reversal(
+    func: &Expr,
+    args: &[Expr],
+    location: Range,
+) -> Option<Check> {
     let first_arg = args.first()?;
     let id = function_name(func)?;
     if !["set", "sorted", "reversed"].contains(&id) {
         return None;
     }
     if let ExprKind::Subscript { slice, .. } = &first_arg.node {
         if let ExprKind::Slice { lower, upper, step } = &slice.node {
@@ -333,15 +431,15 @@
                             value: Constant::Int(val),
                             ..
                         } = &operand.node
                         {
                             if *val == BigInt::from(1) {
                                 return Some(Check::new(
                                     CheckKind::UnnecessarySubscriptReversal(id.to_string()),
-                                    Range::from_located(expr),
+                                    location,
                                 ));
                             }
                         }
                     }
                 }
             }
         }
@@ -350,14 +448,17 @@
 }
 
 /// C416
 pub fn unnecessary_comprehension(
     expr: &Expr,
     elt: &Expr,
     generators: &[Comprehension],
+    locator: &SourceCodeLocator,
+    fix: bool,
+    location: Range,
 ) -> Option<Check> {
     if generators.len() != 1 {
         return None;
     }
     let generator = &generators[0];
     if !(generator.ifs.is_empty() && generator.is_async == 0) {
         return None;
@@ -368,51 +469,55 @@
         return None;
     }
     let expr_kind = match &expr.node {
         ExprKind::ListComp { .. } => "list",
         ExprKind::SetComp { .. } => "set",
         _ => return None,
     };
-    Some(Check::new(
+    let mut check = Check::new(
         CheckKind::UnnecessaryComprehension(expr_kind.to_string()),
-        Range::from_located(expr),
-    ))
+        location,
+    );
+    if fix {
+        match fixes::fix_unnecessary_comprehension(locator, expr) {
+            Ok(fix) => check.amend(fix),
+            Err(e) => error!("Failed to generate fix: {}", e),
+        }
+    }
+    Some(check)
 }
 
 /// C417
-pub fn unnecessary_map(expr: &Expr, func: &Expr, args: &[Expr]) -> Option<Check> {
-    fn new_check(kind: &str, expr: &Expr) -> Check {
-        Check::new(
-            CheckKind::UnnecessaryMap(kind.to_string()),
-            Range::from_located(expr),
-        )
+pub fn unnecessary_map(func: &Expr, args: &[Expr], location: Range) -> Option<Check> {
+    fn new_check(kind: &str, location: Range) -> Check {
+        Check::new(CheckKind::UnnecessaryMap(kind.to_string()), location)
     }
     let id = function_name(func)?;
     match id {
         "map" => {
             if args.len() == 2 && matches!(&args[0].node, ExprKind::Lambda { .. }) {
-                return Some(new_check("generator", expr));
+                return Some(new_check("generator", location));
             }
         }
         "list" | "set" => {
             if let ExprKind::Call { func, args, .. } = &args.first()?.node {
                 let argument = first_argument_with_matching_function("map", func, args)?;
                 if let ExprKind::Lambda { .. } = argument {
-                    return Some(new_check(id, expr));
+                    return Some(new_check(id, location));
                 }
             }
         }
         "dict" => {
             if args.len() == 1 {
                 if let ExprKind::Call { func, args, .. } = &args[0].node {
                     let argument = first_argument_with_matching_function("map", func, args)?;
                     if let ExprKind::Lambda { body, .. } = &argument {
                         if matches!(&body.node, ExprKind::Tuple { elts, .. } | ExprKind::List { elts, .. } if elts.len() == 2)
                         {
-                            return Some(new_check(id, expr));
+                            return Some(new_check(id, location));
                         }
                     }
                 }
             }
         }
         _ => (),
     }
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_print/plugins/print_call.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_print/plugins/print_call.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 use log::error;
 use rustpython_ast::{Expr, Stmt, StmtKind};
 
+use crate::ast::types::{CheckLocator, Range};
 use crate::autofix::helpers;
 use crate::check_ast::Checker;
 use crate::checks::CheckCode;
 use crate::flake8_print::checks;
 
 pub fn print_call(checker: &mut Checker, expr: &Expr, func: &Expr) {
     if let Some(mut check) = checks::print_call(
         expr,
         func,
         checker.settings.enabled.contains(&CheckCode::T201),
         checker.settings.enabled.contains(&CheckCode::T203),
+        checker.locate_check(Range::from_located(expr)),
     ) {
         if checker.patch() {
             let context = checker.binding_context();
             if matches!(
                 checker.parents[context.defined_by].node,
                 StmtKind::Expr { .. }
             ) {
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/checks.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/checks.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/docstring_detection.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/docstring_detection.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/settings.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/settings.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 //! Settings for the `flake-quotes` plugin.
 
 use serde::{Deserialize, Serialize};
 
-#[derive(Debug, Clone, PartialEq, Eq, Serialize, Deserialize)]
+#[derive(Debug, Clone, PartialEq, Eq, Serialize, Deserialize, Hash)]
 #[serde(deny_unknown_fields, rename_all = "kebab-case")]
 pub enum Quote {
     Single,
     Double,
 }
 
 #[derive(Debug, PartialEq, Eq, Serialize, Deserialize, Default)]
@@ -14,36 +14,36 @@
 pub struct Options {
     pub inline_quotes: Option<Quote>,
     pub multiline_quotes: Option<Quote>,
     pub docstring_quotes: Option<Quote>,
     pub avoid_escape: Option<bool>,
 }
 
-#[derive(Debug)]
+#[derive(Debug, Hash)]
 pub struct Settings {
     pub inline_quotes: Quote,
     pub multiline_quotes: Quote,
     pub docstring_quotes: Quote,
     pub avoid_escape: bool,
 }
 
 impl Settings {
     pub fn from_options(options: Options) -> Self {
         Self {
-            inline_quotes: options.inline_quotes.unwrap_or(Quote::Single),
+            inline_quotes: options.inline_quotes.unwrap_or(Quote::Double),
             multiline_quotes: options.multiline_quotes.unwrap_or(Quote::Double),
             docstring_quotes: options.docstring_quotes.unwrap_or(Quote::Double),
             avoid_escape: options.avoid_escape.unwrap_or(true),
         }
     }
 }
 
 impl Default for Settings {
     fn default() -> Self {
         Self {
-            inline_quotes: Quote::Single,
+            inline_quotes: Quote::Double,
             multiline_quotes: Quote::Double,
             docstring_quotes: Quote::Double,
             avoid_escape: true,
         }
     }
 }
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_function.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__double_docstring_docstring_doubles_function.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_function.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/flake8_quotes/snapshots/ruff__flake8_quotes__checks__tests__single_docstring_docstring_singles_function.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/fs.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/fs.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/lib.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 mod pyflakes;
 mod python;
 mod pyupgrade;
 pub mod settings;
 pub mod source_code_locator;
 pub mod visibility;
 
-/// Run ruff over Python source code directly.
-pub fn check(path: &Path, contents: &str) -> Result<Vec<Check>> {
+/// Run Ruff over Python source code directly.
+pub fn check(path: &Path, contents: &str, autofix: bool) -> Result<Vec<Check>> {
     // Find the project root and pyproject.toml.
     let project_root = pyproject::find_project_root(&[path.to_path_buf()]);
     match &project_root {
         Some(path) => debug!("Found project root at: {:?}", path),
         None => debug!("Unable to identify project root; assuming current directory..."),
     };
     let pyproject = pyproject::find_pyproject_toml(&project_root);
@@ -71,12 +71,12 @@
     // Generate checks.
     let checks = check_path(
         path,
         contents,
         tokens,
         &noqa_line_for,
         &settings,
-        &Mode::None,
+        &if autofix { Mode::Generate } else { Mode::None },
     )?;
 
     Ok(checks)
 }
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/linter.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/linter.rs`

 * *Files 0% similar despite different names*

```diff
@@ -361,14 +361,15 @@
     #[test_case(CheckCode::F702, Path::new("F702.py"); "F702")]
     #[test_case(CheckCode::F704, Path::new("F704.py"); "F704")]
     #[test_case(CheckCode::F706, Path::new("F706.py"); "F706")]
     #[test_case(CheckCode::F707, Path::new("F707.py"); "F707")]
     #[test_case(CheckCode::F722, Path::new("F722.py"); "F722")]
     #[test_case(CheckCode::F821, Path::new("F821_0.py"); "F821_0")]
     #[test_case(CheckCode::F821, Path::new("F821_1.py"); "F821_1")]
+    #[test_case(CheckCode::F821, Path::new("F821_2.py"); "F821_2")]
     #[test_case(CheckCode::F822, Path::new("F822.py"); "F822")]
     #[test_case(CheckCode::F823, Path::new("F823.py"); "F823")]
     #[test_case(CheckCode::F831, Path::new("F831.py"); "F831")]
     #[test_case(CheckCode::F841, Path::new("F841.py"); "F841")]
     #[test_case(CheckCode::F901, Path::new("F901.py"); "F901")]
     #[test_case(CheckCode::N801, Path::new("N801.py"); "N801")]
     #[test_case(CheckCode::N802, Path::new("N802.py"); "N802")]
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/main.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/main.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 use std::collections::BTreeMap;
 use std::io::{self, Read};
 use std::path::{Path, PathBuf};
 use std::process::ExitCode;
 use std::sync::mpsc::channel;
 use std::time::Instant;
 
+#[cfg(not(target_family = "wasm"))]
+use ::ruff::cache;
+use ::ruff::checks::{CheckCode, CheckKind};
+use ::ruff::checks_gen::CheckCodePrefix;
+use ::ruff::cli::{collect_per_file_ignores, extract_log_level, warn_on, Cli, Warnable};
+use ::ruff::fs::iter_python_files;
+use ::ruff::linter::{add_noqa_to_path, autoformat_path, lint_path, lint_stdin};
+use ::ruff::logging::{set_up_logging, LogLevel};
+use ::ruff::message::Message;
+use ::ruff::printer::{Printer, SerializationFormat};
+use ::ruff::settings::configuration::Configuration;
+use ::ruff::settings::types::FilePattern;
+use ::ruff::settings::user::UserConfiguration;
+use ::ruff::settings::{pyproject, Settings};
 use anyhow::Result;
 use clap::Parser;
 use colored::Colorize;
 use log::{debug, error};
 use notify::{raw_watcher, RecursiveMode, Watcher};
 #[cfg(not(target_family = "wasm"))]
 use rayon::prelude::*;
-#[cfg(not(target_family = "wasm"))]
-use ruff::cache;
-use ruff::checks::{CheckCode, CheckKind};
-use ruff::checks_gen::CheckCodePrefix;
-use ruff::cli::{collect_per_file_ignores, warn_on, Cli, Warnable};
-use ruff::fs::iter_python_files;
-use ruff::linter::{add_noqa_to_path, autoformat_path, lint_path, lint_stdin};
-use ruff::logging::set_up_logging;
-use ruff::message::Message;
-use ruff::printer::{Printer, SerializationFormat};
-use ruff::settings::configuration::Configuration;
-use ruff::settings::types::FilePattern;
-use ruff::settings::user::UserConfiguration;
-use ruff::settings::{pyproject, Settings};
-use ruff::tell_user;
 use walkdir::DirEntry;
 
 #[cfg(feature = "update-informer")]
 const CARGO_PKG_NAME: &str = env!("CARGO_PKG_NAME");
 #[cfg(feature = "update-informer")]
 const CARGO_PKG_VERSION: &str = env!("CARGO_PKG_VERSION");
 
@@ -219,18 +218,18 @@
     let duration = start.elapsed();
     debug!("Auto-formatted files in: {:?}", duration);
 
     Ok(modifications)
 }
 
 fn inner_main() -> Result<ExitCode> {
-    let mut cli = Cli::parse();
-    cli.quiet |= cli.silent;
+    let cli = Cli::parse();
 
-    set_up_logging(cli.verbose)?;
+    let log_level = extract_log_level(&cli);
+    set_up_logging(&log_level)?;
 
     // Find the project root and pyproject.toml.
     let project_root = pyproject::find_project_root(&cli.files);
     match &project_root {
         Some(path) => debug!("Found project root at: {:?}", path),
         None => debug!("Unable to identify project root; assuming current directory..."),
     };
@@ -316,15 +315,15 @@
         show_files(&cli.files, &settings);
         return Ok(ExitCode::SUCCESS);
     }
 
     #[cfg(not(target_family = "wasm"))]
     cache::init()?;
 
-    let mut printer = Printer::new(cli.format, cli.verbose);
+    let printer = Printer::new(&cli.format, &log_level);
     if cli.watch {
         if cli.fix {
             eprintln!("Warning: --fix is not enabled in watch mode.");
         }
 
         if cli.add_noqa {
             eprintln!("Warning: --no-qa is not enabled in watch mode.");
@@ -336,79 +335,74 @@
 
         if cli.format != SerializationFormat::Text {
             eprintln!("Warning: --format 'text' is used in watch mode.");
         }
 
         // Perform an initial run instantly.
         printer.clear_screen()?;
-        tell_user!("Starting linter in watch mode...\n");
+        printer.write_to_user("Starting linter in watch mode...\n");
 
         let messages = run_once(&cli.files, &settings, !cli.no_cache, false)?;
-        if !cli.silent {
-            printer.write_continuously(&messages)?;
-        }
+        printer.write_continuously(&messages)?;
 
         // Configure the file watcher.
         let (tx, rx) = channel();
         let mut watcher = raw_watcher(tx)?;
         for file in &cli.files {
             watcher.watch(file, RecursiveMode::Recursive)?;
         }
 
         loop {
             match rx.recv() {
                 Ok(e) => {
                     if let Some(path) = e.path {
                         if path.to_string_lossy().ends_with(".py") {
                             printer.clear_screen()?;
-                            tell_user!("File change detected...\n");
+                            printer.write_to_user("File change detected...\n");
 
                             let messages = run_once(&cli.files, &settings, !cli.no_cache, false)?;
-                            if !cli.silent {
-                                printer.write_continuously(&messages)?;
-                            }
+                            printer.write_continuously(&messages)?;
                         }
                     }
                 }
                 Err(e) => return Err(e.into()),
             }
         }
     } else if cli.add_noqa {
         let modifications = add_noqa(&cli.files, &settings)?;
-        if modifications > 0 {
+        if modifications > 0 && log_level >= LogLevel::Default {
             println!("Added {modifications} noqa directives.");
         }
     } else if cli.autoformat {
         let modifications = autoformat(&cli.files, &settings)?;
-        if modifications > 0 {
+        if modifications > 0 && log_level >= LogLevel::Default {
             println!("Formatted {modifications} files.");
         }
     } else {
-        let (messages, should_print_messages, should_check_updates) =
-            if cli.files == vec![PathBuf::from("-")] {
-                let filename = cli.stdin_filename.unwrap_or_else(|| "-".to_string());
-                let path = Path::new(&filename);
-                (
-                    run_once_stdin(&settings, path, cli.fix)?,
-                    !cli.silent && !cli.fix,
-                    false,
-                )
-            } else {
-                (
-                    run_once(&cli.files, &settings, !cli.no_cache, cli.fix)?,
-                    !cli.silent,
-                    !cli.quiet,
-                )
-            };
-        if should_print_messages {
+        let is_stdin = cli.files == vec![PathBuf::from("-")];
+
+        // Generate lint violations.
+        let messages = if is_stdin {
+            let filename = cli.stdin_filename.unwrap_or_else(|| "-".to_string());
+            let path = Path::new(&filename);
+            run_once_stdin(&settings, path, cli.fix)?
+        } else {
+            run_once(&cli.files, &settings, !cli.no_cache, cli.fix)?
+        };
+
+        // Always try to print violations (the printer itself may suppress output),
+        // unless we're writing fixes via stdin (in which case, the transformed
+        // source code goes to stdout).
+        if !(is_stdin && cli.fix) {
             printer.write_once(&messages)?;
         }
 
+        // Check for updates if we're in a non-silent log level.
         #[cfg(feature = "update-informer")]
-        if should_check_updates {
+        if !is_stdin && log_level >= LogLevel::Default {
             check_for_updates();
         }
 
         if messages.iter().any(|message| !message.fixed) && !cli.exit_zero {
             return Ok(ExitCode::FAILURE);
         }
     }
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/message.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/message.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/noqa.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/noqa.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pep8_naming/checks.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pep8_naming/checks.rs`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 }
 
 /// N806
 pub fn non_lowercase_variable_in_function(scope: &Scope, expr: &Expr, name: &str) -> Option<Check> {
     if !matches!(scope.kind, ScopeKind::Function(FunctionScope { .. })) {
         return None;
     }
-    if !is_lower(name) {
+    if name.to_lowercase() != name {
         return Some(Check::new(
             CheckKind::NonLowercaseVariableInFunction(name.to_string()),
             Range::from_located(expr),
         ));
     }
     None
 }
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pep8_naming/settings.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pep8_naming/settings.rs`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 #[serde(deny_unknown_fields, rename_all = "kebab-case")]
 pub struct Options {
     pub ignore_names: Option<Vec<String>>,
     pub classmethod_decorators: Option<Vec<String>>,
     pub staticmethod_decorators: Option<Vec<String>>,
 }
 
-#[derive(Debug)]
+#[derive(Debug, Hash)]
 pub struct Settings {
     pub ignore_names: Vec<String>,
     pub classmethod_decorators: Vec<String>,
     pub staticmethod_decorators: Vec<String>,
 }
 
 impl Settings {
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pycodestyle/checks.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pycodestyle/checks.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pydocstyle/plugins.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pydocstyle/plugins.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyflakes/checks.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyflakes/checks.rs`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,29 @@
     Arg, Arguments, Cmpop, Constant, Excepthandler, ExcepthandlerKind, Expr, ExprKind, Stmt,
     StmtKind,
 };
 
 use crate::ast::types::{BindingKind, CheckLocator, FunctionScope, Range, Scope, ScopeKind};
 use crate::checks::{Check, CheckKind};
 
-/// F634
-pub fn if_tuple(test: &Expr, location: Range) -> Option<Check> {
+/// F631
+pub fn assert_tuple(test: &Expr, location: Range) -> Option<Check> {
     if let ExprKind::Tuple { elts, .. } = &test.node {
         if !elts.is_empty() {
-            return Some(Check::new(CheckKind::IfTuple, location));
+            return Some(Check::new(CheckKind::AssertTuple, location));
         }
     }
     None
 }
 
-/// F631
-pub fn assert_tuple(test: &Expr, location: Range) -> Option<Check> {
+/// F634
+pub fn if_tuple(test: &Expr, location: Range) -> Option<Check> {
     if let ExprKind::Tuple { elts, .. } = &test.node {
         if !elts.is_empty() {
-            return Some(Check::new(CheckKind::AssertTuple, location));
+            return Some(Check::new(CheckKind::IfTuple, location));
         }
     }
     None
 }
 
 /// F841
 pub fn unused_variables(
@@ -74,41 +74,14 @@
             ));
         }
     }
 
     None
 }
 
-/// F901
-pub fn raise_not_implemented(expr: &Expr) -> Option<Check> {
-    match &expr.node {
-        ExprKind::Call { func, .. } => {
-            if let ExprKind::Name { id, .. } = &func.node {
-                if id == "NotImplemented" {
-                    return Some(Check::new(
-                        CheckKind::RaiseNotImplemented,
-                        Range::from_located(expr),
-                    ));
-                }
-            }
-        }
-        ExprKind::Name { id, .. } => {
-            if id == "NotImplemented" {
-                return Some(Check::new(
-                    CheckKind::RaiseNotImplemented,
-                    Range::from_located(expr),
-                ));
-            }
-        }
-        _ => {}
-    }
-
-    None
-}
-
 /// F831
 pub fn duplicate_arguments(arguments: &Arguments) -> Vec<Check> {
     let mut checks: Vec<Check> = vec![];
 
     // Collect all the arguments into a single vector.
     let mut all_arguments: Vec<&Arg> = arguments
         .args
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyflakes/fixes.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyflakes/fixes.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 use anyhow::Result;
 use libcst_native::{Codegen, ImportNames, NameOrAttribute, SmallStatement, Statement};
 use rustpython_ast::Stmt;
 
-use crate::ast::types::Range;
 use crate::autofix::{helpers, Fix};
 use crate::cst::helpers::compose_module_path;
+use crate::cst::matchers::match_tree;
 use crate::source_code_locator::SourceCodeLocator;
 
 /// Generate a Fix to remove any unused imports from an `import` statement.
 pub fn remove_unused_imports(
     locator: &SourceCodeLocator,
     full_names: &[&str],
     stmt: &Stmt,
     parent: Option<&Stmt>,
     deleted: &[&Stmt],
 ) -> Result<Fix> {
-    let mut tree = match libcst_native::parse_module(
-        locator.slice_source_code_range(&Range::from_located(stmt)),
-        None,
-    ) {
-        Ok(m) => m,
-        Err(_) => return Err(anyhow::anyhow!("Failed to extract CST from source.")),
-    };
+    let mut tree = match_tree(locator, stmt)?;
 
     let body = if let Some(Statement::Simple(body)) = tree.body.first_mut() {
         body
     } else {
-        return Err(anyhow::anyhow!("Expected node to be: Statement::Simple."));
+        return Err(anyhow::anyhow!("Expected node to be: Statement::Simple"));
     };
     let body = if let Some(SmallStatement::Import(body)) = body.body.first_mut() {
         body
     } else {
         return Err(anyhow::anyhow!(
-            "Expected node to be: SmallStatement::ImportFrom."
+            "Expected node to be: SmallStatement::ImportFrom"
         ));
     };
     let aliases = &mut body.names;
 
     // Preserve the trailing comma (or not) from the last entry.
     let trailing_comma = aliases.last().and_then(|alias| alias.comma.clone());
 
@@ -74,39 +68,33 @@
 pub fn remove_unused_import_froms(
     locator: &SourceCodeLocator,
     full_names: &[&str],
     stmt: &Stmt,
     parent: Option<&Stmt>,
     deleted: &[&Stmt],
 ) -> Result<Fix> {
-    let mut tree = match libcst_native::parse_module(
-        locator.slice_source_code_range(&Range::from_located(stmt)),
-        None,
-    ) {
-        Ok(m) => m,
-        Err(_) => return Err(anyhow::anyhow!("Failed to extract CST from source.")),
-    };
+    let mut tree = match_tree(locator, stmt)?;
 
     let body = if let Some(Statement::Simple(body)) = tree.body.first_mut() {
         body
     } else {
-        return Err(anyhow::anyhow!("Expected node to be: Statement::Simple."));
+        return Err(anyhow::anyhow!("Expected node to be: Statement::Simple"));
     };
     let body = if let Some(SmallStatement::ImportFrom(body)) = body.body.first_mut() {
         body
     } else {
         return Err(anyhow::anyhow!(
-            "Expected node to be: SmallStatement::ImportFrom."
+            "Expected node to be: SmallStatement::ImportFrom"
         ));
     };
 
     let aliases = if let ImportNames::Aliases(aliases) = &mut body.names {
         aliases
     } else {
-        return Err(anyhow::anyhow!("Expected node to be: Aliases."));
+        return Err(anyhow::anyhow!("Expected node to be: Aliases"));
     };
 
     // Preserve the trailing comma (or not) from the last entry.
     let trailing_comma = aliases.last().and_then(|alias| alias.comma.clone());
 
     // Identify unused imports from within the `import from`.
     let mut removable = vec![];
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyflakes/plugins/invalid_print_syntax.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyflakes/plugins/invalid_print_syntax.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use rustpython_ast::{Expr, ExprKind};
 
 use crate::ast::types::{Binding, BindingKind, Range};
 use crate::check_ast::Checker;
 use crate::checks::{Check, CheckKind};
 
+/// F633
 pub fn invalid_print_syntax(checker: &mut Checker, left: &Expr) {
     if let ExprKind::Name { id, .. } = &left.node {
         if id == "print" {
             let scope = checker.current_scope();
             if let Some(Binding {
                 kind: BindingKind::Builtin,
                 ..
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/python/builtins.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/python/builtins.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/python/typing.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/python/typing.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,72 @@
 use std::collections::{BTreeMap, BTreeSet};
 
 use once_cell::sync::Lazy;
 use rustpython_ast::{Expr, ExprKind};
 
+// See: https://pypi.org/project/typing-extensions/
+static TYPING_EXTENSIONS: Lazy<BTreeSet<&'static str>> = Lazy::new(|| {
+    BTreeSet::from([
+        "Annotated",
+        "Any",
+        "AsyncContextManager",
+        "AsyncGenerator",
+        "AsyncIterable",
+        "AsyncIterator",
+        "Awaitable",
+        "ChainMap",
+        "ClassVar",
+        "Concatenate",
+        "ContextManager",
+        "Coroutine",
+        "Counter",
+        "DefaultDict",
+        "Deque",
+        "Final",
+        "Literal",
+        "LiteralString",
+        "NamedTuple",
+        "Never",
+        "NewType",
+        "NotRequired",
+        "OrderedDict",
+        "ParamSpec",
+        "ParamSpecArgs",
+        "ParamSpecKwargs",
+        "Protocol",
+        "Required",
+        "Self",
+        "TYPE_CHECKING",
+        "Text",
+        "Type",
+        "TypeAlias",
+        "TypeGuard",
+        "TypeVar",
+        "TypeVarTuple",
+        "TypedDict",
+        "Unpack",
+        "assert_never",
+        "assert_type",
+        "clear_overloads",
+        "final",
+        "get_Type_hints",
+        "get_args",
+        "get_origin",
+        "get_overloads",
+        "is_typeddict",
+        "overload",
+        "reveal_type",
+        "runtime_checkable",
+    ])
+});
+
+pub fn in_extensions(name: &str) -> bool {
+    TYPING_EXTENSIONS.contains(name)
+}
+
 // See: https://docs.python.org/3/library/typing.html
 static IMPORTED_SUBSCRIPTS: Lazy<BTreeMap<&'static str, BTreeSet<&'static str>>> =
     Lazy::new(|| {
         let mut import_map = BTreeMap::new();
         for (name, module) in [
             // `collections`
             ("ChainMap", "collections"),
@@ -44,29 +104,26 @@
             // `re`
             ("Match", "re"),
             ("Pattern", "re"),
             // `typing`
             ("AbstractSet", "typing"),
             ("Annotated", "typing"),
             ("AsyncContextManager", "typing"),
-            ("AsyncContextManager", "typing"),
             ("AsyncGenerator", "typing"),
-            ("AsyncIterable", "typing"),
             ("AsyncIterator", "typing"),
             ("Awaitable", "typing"),
             ("BinaryIO", "typing"),
             ("ByteString", "typing"),
             ("Callable", "typing"),
             ("ChainMap", "typing"),
             ("ClassVar", "typing"),
             ("Collection", "typing"),
             ("Concatenate", "typing"),
             ("Container", "typing"),
             ("ContextManager", "typing"),
-            ("ContextManager", "typing"),
             ("Coroutine", "typing"),
             ("Counter", "typing"),
             ("DefaultDict", "typing"),
             ("Deque", "typing"),
             ("Dict", "typing"),
             ("Final", "typing"),
             ("FrozenSet", "typing"),
@@ -88,26 +145,42 @@
             ("Pattern", "typing"),
             ("Reversible", "typing"),
             ("Sequence", "typing"),
             ("Set", "typing"),
             ("TextIO", "typing"),
             ("Tuple", "typing"),
             ("Type", "typing"),
-            ("Type", "typing"),
             ("TypeGuard", "typing"),
             ("Union", "typing"),
             ("Unpack", "typing"),
             ("ValuesView", "typing"),
             // `typing.io`
             ("BinaryIO", "typing.io"),
             ("IO", "typing.io"),
             ("TextIO", "typing.io"),
             // `typing.re`
             ("Match", "typing.re"),
             ("Pattern", "typing.re"),
+            // `typing_extensions`
+            ("Annotated", "typing_extensions"),
+            ("AsyncContextManager", "typing_extensions"),
+            ("AsyncGenerator", "typing_extensions"),
+            ("AsyncIterable", "typing_extensions"),
+            ("AsyncIterator", "typing_extensions"),
+            ("Awaitable", "typing_extensions"),
+            ("ChainMap", "typing_extensions"),
+            ("ClassVar", "typing_extensions"),
+            ("Concatenate", "typing_extensions"),
+            ("ContextManager", "typing_extensions"),
+            ("Coroutine", "typing_extensions"),
+            ("Counter", "typing_extensions"),
+            ("DefaultDict", "typing_extensions"),
+            ("Deque", "typing_extensions"),
+            ("Literal", "typing_extensions"),
+            ("Type", "typing_extensions"),
             // `weakref`
             ("WeakKeyDictionary", "weakref"),
             ("WeakSet", "weakref"),
             ("WeakValueDictionary", "weakref"),
         ] {
             import_map
                 .entry(name)
@@ -183,15 +256,16 @@
         }
         _ => {}
     }
     None
 }
 
 /// Returns `true` if `Expr` represents a reference to a typing object with a
-/// PEP 585 built-in.
+/// PEP 585 built-in. Note that none of the PEP 585 built-ins are in
+/// `typing_extensions`.
 pub fn is_pep585_builtin(expr: &Expr, typing_imports: Option<&BTreeSet<&str>>) -> bool {
     match &expr.node {
         ExprKind::Attribute { attr, value, .. } => {
             if let ExprKind::Name { id, .. } = &value.node {
                 id == "typing" && PEP_585_BUILTINS_ELIGIBLE.contains(&attr.as_str())
             } else {
                 false
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/checks.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/checks.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/fixes.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/fixes.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/deprecated_unittest_alias.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/deprecated_unittest_alias.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/mod.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/mod.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/super_call_with_parameters.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/super_call_with_parameters.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/type_of_primitive.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/type_of_primitive.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/unnecessary_abspath.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/unnecessary_abspath.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/use_pep585_annotation.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/use_pep585_annotation.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/use_pep604_annotation.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/use_pep604_annotation.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/useless_metaclass_type.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/useless_metaclass_type.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/plugins/useless_object_inheritance.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/plugins/useless_object_inheritance.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/pyupgrade/types.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/pyupgrade/types.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/settings/configuration.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/settings/configuration.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/settings/mod.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/settings/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -80,22 +80,27 @@
             pep8_naming: Default::default(),
         }
     }
 }
 
 impl Hash for Settings {
     fn hash<H: Hasher>(&self, state: &mut H) {
-        self.line_length.hash(state);
+        // Add base properties in alphabetical order.
         self.dummy_variable_rgx.as_str().hash(state);
         for value in self.enabled.iter() {
             value.hash(state);
         }
+        self.line_length.hash(state);
         for value in self.per_file_ignores.iter() {
             value.hash(state);
         }
+        self.target_version.hash(state);
+        // Add plugin properties in alphabetical order.
+        self.flake8_quotes.hash(state);
+        self.pep8_naming.hash(state);
     }
 }
 
 /// Given a set of selected and ignored prefixes, resolve the set of enabled
 /// error codes.
 fn resolve_codes(
     select: &[CheckCodePrefix],
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/settings/options.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/settings/options.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/settings/pyproject.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/settings/pyproject.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/settings/types.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/settings/types.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 use glob::Pattern;
 use serde::{de, Deserialize, Deserializer, Serialize};
 
 use crate::checks::CheckCode;
 use crate::checks_gen::CheckCodePrefix;
 use crate::fs;
 
-#[derive(Clone, Debug, PartialOrd, PartialEq, Eq, Serialize, Deserialize)]
+#[derive(Clone, Debug, PartialOrd, PartialEq, Eq, Serialize, Deserialize, Hash)]
+#[serde(rename_all = "lowercase")]
 pub enum PythonVersion {
     Py33,
     Py34,
     Py35,
     Py36,
     Py37,
     Py38,
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/settings/user.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/settings/user.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__A001_A001.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__A001_A001.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__A002_A002.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__A002_A002.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B006_B006_B008.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B006_B006_B008.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B007_B007.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B007_B007.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B011_B011.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B011_B011.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B014_B014.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B014_B014.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B025_B025.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__B025_B025.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C405_C405.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F841_F841.py.snap`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 ---
 source: src/linter.rs
 expression: checks
 ---
 - kind:
-    UnnecessaryLiteralSet: list
+    UnusedVariable: e
   location:
-    row: 1
-    column: 5
+    row: 3
+    column: 0
   end_location:
-    row: 1
-    column: 16
+    row: 7
+    column: 0
   fix: ~
 - kind:
-    UnnecessaryLiteralSet: tuple
+    UnusedVariable: z
   location:
-    row: 2
+    row: 16
+    column: 4
+  end_location:
+    row: 16
     column: 5
+  fix: ~
+- kind:
+    UnusedVariable: foo
+  location:
+    row: 20
+    column: 4
   end_location:
-    row: 2
-    column: 16
+    row: 20
+    column: 7
   fix: ~
 - kind:
-    UnnecessaryLiteralSet: list
+    UnusedVariable: a
   location:
-    row: 3
+    row: 21
     column: 5
   end_location:
-    row: 3
-    column: 12
+    row: 21
+    column: 6
   fix: ~
 - kind:
-    UnnecessaryLiteralSet: tuple
+    UnusedVariable: b
   location:
-    row: 4
-    column: 5
+    row: 21
+    column: 8
   end_location:
-    row: 4
-    column: 12
+    row: 21
+    column: 9
   fix: ~
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C406_C406.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C403_C403.py.snap`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 ---
 source: src/linter.rs
 expression: checks
 ---
-- kind:
-    UnnecessaryLiteralDict: list
+- kind: UnnecessaryListComprehensionSet
   location:
     row: 1
-    column: 5
+    column: 4
   end_location:
     row: 1
-    column: 19
-  fix: ~
-- kind:
-    UnnecessaryLiteralDict: tuple
+    column: 30
+  fix:
+    patch:
+      content: "{x for x in range(3)}"
+      location:
+        row: 1
+        column: 4
+      end_location:
+        row: 1
+        column: 30
+    applied: false
+- kind: UnnecessaryListComprehensionSet
   location:
     row: 2
-    column: 5
-  end_location:
-    row: 2
-    column: 20
-  fix: ~
-- kind:
-    UnnecessaryLiteralDict: list
-  location:
-    row: 3
-    column: 5
-  end_location:
-    row: 3
-    column: 13
-  fix: ~
-- kind:
-    UnnecessaryLiteralDict: tuple
-  location:
-    row: 4
-    column: 5
+    column: 4
   end_location:
     row: 4
-    column: 13
-  fix: ~
+    column: 1
+  fix:
+    patch:
+      content: "{\n    x for x in range(3)\n}"
+      location:
+        row: 2
+        column: 4
+      end_location:
+        row: 4
+        column: 1
+    applied: false
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C408_C408.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__W605_W605.py.snap`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 ---
 source: src/linter.rs
 expression: checks
 ---
 - kind:
-    UnnecessaryCollectionCall: tuple
+    InvalidEscapeSequence: "."
   location:
-    row: 1
-    column: 4
+    row: 2
+    column: 9
   end_location:
-    row: 1
-    column: 11
+    row: 2
+    column: 10
   fix: ~
 - kind:
-    UnnecessaryCollectionCall: list
+    InvalidEscapeSequence: "."
   location:
-    row: 2
-    column: 4
+    row: 6
+    column: 1
   end_location:
-    row: 2
-    column: 10
+    row: 6
+    column: 2
   fix: ~
 - kind:
-    UnnecessaryCollectionCall: dict
+    InvalidEscapeSequence: _
   location:
-    row: 3
+    row: 11
     column: 5
   end_location:
-    row: 3
-    column: 11
+    row: 11
+    column: 6
   fix: ~
 - kind:
-    UnnecessaryCollectionCall: dict
+    InvalidEscapeSequence: _
   location:
-    row: 4
-    column: 5
+    row: 18
+    column: 6
   end_location:
-    row: 4
-    column: 14
+    row: 18
+    column: 7
   fix: ~
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C410_C410.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N813_N813.py.snap`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 ---
 source: src/linter.rs
 expression: checks
 ---
 - kind:
-    UnnecessaryLiteralWithinListCall: list
+    CamelcaseImportedAsLowercase:
+      - Camel
+      - camel
   location:
     row: 1
-    column: 5
+    column: 0
   end_location:
     row: 1
-    column: 17
+    column: 25
   fix: ~
 - kind:
-    UnnecessaryLiteralWithinListCall: tuple
+    CamelcaseImportedAsLowercase:
+      - CamelCase
+      - camelcase
   location:
     row: 2
-    column: 5
+    column: 0
   end_location:
     row: 2
-    column: 17
+    column: 38
   fix: ~
 - kind:
-    UnnecessaryLiteralWithinListCall: list
+    CamelcaseImportedAsLowercase:
+      - AnotherCamelCase
+      - another_camelcase
   location:
     row: 3
-    column: 5
+    column: 0
   end_location:
     row: 3
-    column: 13
-  fix: ~
-- kind:
-    UnnecessaryLiteralWithinListCall: tuple
-  location:
-    row: 4
-    column: 5
-  end_location:
-    row: 4
-    column: 13
+    column: 53
   fix: ~
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C414_C414.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C414_C414.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C415_C415.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C415_C415.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C417_C417.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C417_C417.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D201_D.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D201_D.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D202_D.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D202_D.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D203_D.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D203_D.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D204_D.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D204_D.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D205_D.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D205_D.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D207_D.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D207_D.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D208_D.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D208_D.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D210_D.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D210_D.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D211_D.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D211_D.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D213_D.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D213_D.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D215_sections.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D215_sections.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D300_D.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D300_D.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D400_D.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D400_D.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D405_sections.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D405_sections.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D406_sections.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D406_sections.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D407_sections.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D407_sections.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D409_sections.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D409_sections.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D410_sections.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D410_sections.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D411_sections.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D411_sections.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D414_sections.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D414_sections.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D415_D.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D415_D.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D417_sections.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__D417_sections.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E711_E711.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E711_E711.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E712_E712.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E712_E712.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E713_E713.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E713_E713.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E721_E721.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E721_E721.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E731_E731.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E731_E731.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E741_E741.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__E741_E741.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F401_F401_0.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F401_F401_0.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F401_F401_5.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F401_F401_5.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F702_F702.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F702_F702.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F821_F821_0.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F821_F821_0.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F821_F821_1.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F821_F821_1.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__F841_F841.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U001_U001.py.snap`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,39 @@
 ---
 source: src/linter.rs
 expression: checks
 ---
-- kind:
-    UnusedVariable: e
+- kind: UselessMetaclassType
   location:
-    row: 3
-    column: 0
-  end_location:
-    row: 7
-    column: 0
-  fix: ~
-- kind:
-    UnusedVariable: z
-  location:
-    row: 16
+    row: 2
     column: 4
   end_location:
-    row: 16
-    column: 5
-  fix: ~
-- kind:
-    UnusedVariable: foo
+    row: 2
+    column: 24
+  fix:
+    patch:
+      content: pass
+      location:
+        row: 2
+        column: 4
+      end_location:
+        row: 2
+        column: 24
+    applied: false
+- kind: UselessMetaclassType
   location:
-    row: 20
+    row: 6
     column: 4
   end_location:
-    row: 20
-    column: 7
-  fix: ~
-- kind:
-    UnusedVariable: a
-  location:
-    row: 21
-    column: 5
-  end_location:
-    row: 21
-    column: 6
-  fix: ~
-- kind:
-    UnusedVariable: b
-  location:
-    row: 21
-    column: 8
-  end_location:
-    row: 21
-    column: 9
-  fix: ~
+    row: 6
+    column: 24
+  fix:
+    patch:
+      content: ""
+      location:
+        row: 6
+        column: 0
+      end_location:
+        row: 7
+        column: 0
+    applied: false
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N801_N801.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N801_N801.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N802_N802.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N802_N802.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N811_N811.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N811_N811.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N812_N812.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N812_N812.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N813_N813.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N814_N814.py.snap`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 ---
 source: src/linter.rs
 expression: checks
 ---
 - kind:
-    CamelcaseImportedAsLowercase:
+    CamelcaseImportedAsConstant:
       - Camel
-      - camel
+      - CAMEL
   location:
     row: 1
     column: 0
   end_location:
     row: 1
     column: 25
   fix: ~
 - kind:
-    CamelcaseImportedAsLowercase:
+    CamelcaseImportedAsConstant:
       - CamelCase
-      - camelcase
+      - CAMELCASE
   location:
     row: 2
     column: 0
   end_location:
     row: 2
     column: 38
   fix: ~
 - kind:
-    CamelcaseImportedAsLowercase:
+    CamelcaseImportedAsConstant:
       - AnotherCamelCase
-      - another_camelcase
+      - ANOTHER_CAMELCASE
   location:
     row: 3
     column: 0
   end_location:
     row: 3
     column: 53
   fix: ~
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__N814_N814.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C400_C400.py.snap`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 ---
 source: src/linter.rs
 expression: checks
 ---
-- kind:
-    CamelcaseImportedAsConstant:
-      - Camel
-      - CAMEL
+- kind: UnnecessaryGeneratorList
   location:
     row: 1
-    column: 0
+    column: 4
   end_location:
     row: 1
-    column: 25
-  fix: ~
-- kind:
-    CamelcaseImportedAsConstant:
-      - CamelCase
-      - CAMELCASE
+    column: 29
+  fix:
+    patch:
+      content: "[x for x in range(3)]"
+      location:
+        row: 1
+        column: 4
+      end_location:
+        row: 1
+        column: 29
+    applied: false
+- kind: UnnecessaryGeneratorList
   location:
     row: 2
-    column: 0
+    column: 4
   end_location:
-    row: 2
-    column: 38
-  fix: ~
-- kind:
-    CamelcaseImportedAsConstant:
-      - AnotherCamelCase
-      - ANOTHER_CAMELCASE
-  location:
-    row: 3
-    column: 0
-  end_location:
-    row: 3
-    column: 53
-  fix: ~
+    row: 4
+    column: 1
+  fix:
+    patch:
+      content: "[\n    x for x in range(3)\n]"
+      location:
+        row: 2
+        column: 4
+      end_location:
+        row: 4
+        column: 1
+    applied: false
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__T203_T203.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__T203_T203.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U001_U001.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C416_C416.py.snap`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 ---
 source: src/linter.rs
 expression: checks
 ---
-- kind: UselessMetaclassType
+- kind:
+    UnnecessaryComprehension: list
   location:
     row: 2
-    column: 4
+    column: 0
   end_location:
     row: 2
-    column: 24
+    column: 14
   fix:
     patch:
-      content: pass
+      content: list(x)
       location:
         row: 2
-        column: 4
+        column: 0
       end_location:
         row: 2
-        column: 24
+        column: 14
     applied: false
-- kind: UselessMetaclassType
+- kind:
+    UnnecessaryComprehension: set
   location:
-    row: 6
-    column: 4
+    row: 3
+    column: 0
   end_location:
-    row: 6
-    column: 24
+    row: 3
+    column: 14
   fix:
     patch:
-      content: ""
+      content: set(x)
       location:
-        row: 6
+        row: 3
         column: 0
       end_location:
-        row: 7
-        column: 0
+        row: 3
+        column: 14
     applied: false
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U002_U002.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U002_U002.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U003_U003.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U003_U003.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U004_U004.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U004_U004.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U005_U005.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U005_U005.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U006_U006.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U006_U006.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U007_U007.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U007_U007.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U008_U008.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__U008_U008.py.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__W605_W605.py.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__C401_C401.py.snap`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 ---
 source: src/linter.rs
 expression: checks
 ---
-- kind:
-    InvalidEscapeSequence: "."
+- kind: UnnecessaryGeneratorSet
   location:
-    row: 2
-    column: 9
-  end_location:
-    row: 2
-    column: 10
-  fix: ~
-- kind:
-    InvalidEscapeSequence: "."
-  location:
-    row: 6
-    column: 1
+    row: 1
+    column: 4
   end_location:
-    row: 6
-    column: 2
-  fix: ~
-- kind:
-    InvalidEscapeSequence: _
+    row: 1
+    column: 28
+  fix:
+    patch:
+      content: "{x for x in range(3)}"
+      location:
+        row: 1
+        column: 4
+      end_location:
+        row: 1
+        column: 28
+    applied: false
+- kind: UnnecessaryGeneratorSet
   location:
-    row: 11
-    column: 5
-  end_location:
-    row: 11
-    column: 6
-  fix: ~
-- kind:
-    InvalidEscapeSequence: _
-  location:
-    row: 18
-    column: 6
+    row: 2
+    column: 4
   end_location:
-    row: 18
-    column: 7
-  fix: ~
+    row: 4
+    column: 1
+  fix:
+    patch:
+      content: "{\n    x for x in range(3)\n}"
+      location:
+        row: 2
+        column: 4
+      end_location:
+        row: 4
+        column: 1
+    applied: false
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__f841_dummy_variable_rgx.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__f841_dummy_variable_rgx.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/snapshots/ruff__linter__tests__m001.snap` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/snapshots/ruff__linter__tests__m001.snap`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/source_code_locator.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/source_code_locator.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/src/visibility.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/src/visibility.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/local_dependencies/ruff/tests/integration_test.rs` & `flake8_to_ruff-0.0.99_dev.0/local_dependencies/ruff/tests/integration_test.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/Cargo.toml` & `flake8_to_ruff-0.0.99_dev.0/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "flake8-to-ruff"
-version = "0.0.94-dev.1"
+version = "0.0.99-dev.0"
 edition = "2021"
 
 [lib]
 name = "flake8_to_ruff"
 
 [dependencies]
 anyhow = { version = "1.0.60" }
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/Cargo.lock` & `flake8_to_ruff-0.0.99_dev.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -767,15 +767,15 @@
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
 name = "flake8_to_ruff"
-version = "0.0.94"
+version = "0.0.99"
 dependencies = [
  "anyhow",
  "clap",
  "configparser",
  "once_cell",
  "regex",
  "ruff",
@@ -1406,15 +1406,15 @@
  "ws2_32-sys",
 ]
 
 [[package]]
 name = "net2"
 version = "0.2.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74d0df99cfcd2530b2e694f6e17e7f37b8e26bb23983ac530c0c97408837c631"
+checksum = "74d0df99cfcd2530b2e694f6e17e7f37b8e26bb23983ac530.0.98408837c631"
 dependencies = [
  "cfg-if 0.1.10",
  "libc",
  "winapi 0.3.9",
 ]
 
 [[package]]
@@ -1971,15 +1971,15 @@
  "untrusted",
  "web-sys",
  "winapi 0.3.9",
 ]
 
 [[package]]
 name = "ruff"
-version = "0.0.94"
+version = "0.0.99"
 dependencies = [
  "anyhow",
  "bincode",
  "cacache",
  "chrono",
  "clap",
  "clearscreen",
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/pyproject.toml` & `flake8_to_ruff-0.0.99_dev.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/src/main.rs` & `flake8_to_ruff-0.0.99_dev.0/src/main.rs`

 * *Files 18% similar despite different names*

```diff
@@ -2,34 +2,43 @@
 
 use std::path::PathBuf;
 
 use anyhow::Result;
 use clap::Parser;
 use configparser::ini::Ini;
 use flake8_to_ruff::converter;
+use flake8_to_ruff::plugin::Plugin;
 
 #[derive(Parser)]
 #[command(
     about = "Convert existing Flake8 configuration to Ruff.",
     long_about = None
 )]
 struct Cli {
     /// Path to the Flake8 configuration file (e.g., 'setup.cfg', 'tox.ini', or
     /// '.flake8').
     #[arg(required = true)]
     file: PathBuf,
+    /// List of plugins to enable.
+    #[arg(long, value_delimiter = ',')]
+    plugin: Option<Vec<Plugin>>,
 }
 
 fn main() -> Result<()> {
     let cli = Cli::parse();
 
     // Read the INI file.
     let mut ini = Ini::new_cs();
     ini.set_multiline(true);
     let config = ini.load(cli.file).map_err(|msg| anyhow::anyhow!(msg))?;
 
+    // Extract the Flake8 section.
+    let flake8 = config
+        .get("flake8")
+        .expect("Unable to find flake8 section in INI file.");
+
     // Create the pyproject.toml.
-    let pyproject = converter::convert(config)?;
+    let pyproject = converter::convert(flake8, cli.plugin)?;
     println!("{}", toml::to_string_pretty(&pyproject)?);
 
     Ok(())
 }
```

### Comparing `flake8_to_ruff-0.0.94_dev.1/src/parser.rs` & `flake8_to_ruff-0.0.99_dev.0/src/parser.rs`

 * *Files identical despite different names*

### Comparing `flake8_to_ruff-0.0.94_dev.1/PKG-INFO` & `flake8_to_ruff-0.0.99_dev.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-to-ruff
-Version: 0.0.94_dev.1
+Version: 0.0.99_dev.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -35,33 +35,84 @@
 
 ```shell
 pip install flake8-to-ruff
 ```
 
 ### Usage
 
-To run Ruff, try any of the following:
+To run `flake8-to-ruff`:
 
 ```shell
 flake8-to-ruff path/to/setup.cfg
 flake8-to-ruff path/to/tox.ini
 flake8-to-ruff path/to/.flake8
 ```
 
+`flake8-to-ruff` will print the relevant `pyproject.toml` sections to standard output, like so:
+
+```toml
+[tool.ruff]
+exclude = [
+    '.svn',
+    'CVS',
+    '.bzr',
+    '.hg',
+    '.git',
+    '__pycache__',
+    '.tox',
+    '.idea',
+    '.mypy_cache',
+    '.venv',
+    'node_modules',
+    '_state_machine.py',
+    'test_fstring.py',
+    'bad_coding2.py',
+    'badsyntax_*.py',
+]
+select = [
+    'A',
+    'E',
+    'F',
+    'Q',
+]
+ignore = []
+
+[tool.ruff.flake8-quotes]
+inline-quotes = 'single'
+
+[tool.ruff.pep8-naming]
+ignore-names = [
+    'foo',
+    'bar',
+]
+```
+
+### Plugins
+
+`flake8-to-ruff` will attempt to infer any activated plugins based on the settings provided in your
+configuration file.
+
+For example, if your `.flake8` file includes a `docstring-convention` property, `flake8-to-ruff`
+will enable the appropriate [`flake8-docstrings`](https://pypi.org/project/flake8-docstrings/)
+checks.
+
+Alternatively, you can manually specify plugins on the command-line:
+
+```shell
+flake8-to-ruff path/to/.flake8 --plugin flake8-builtins --plugin flake8-quotes
+```
+
 ## Limitations
 
 1. Ruff only supports a subset of the Flake configuration options. `flake8-to-ruff` will warn on and
    ignore unsupported options in the `.flake8` file (or equivalent). (Similarly, Ruff has a few
    configuration options that don't exist in Flake8.)
 2. Ruff will omit any error codes that are unimplemented or unsupported by Ruff, including error
    codes from unsupported plugins. (See the [Ruff README](https://github.com/charliermarsh/ruff#user-content-how-does-ruff-compare-to-flake8)
    for the complete list of supported plugins.)
-3. `flake8-to-ruff` does not auto-detect your Flake8 plugins, so any reliance on Flake8 plugins that
-   implicitly enable third-party checks will be ignored. Instead, add those error codes to your
-   `select` or `extend-select` fields, so that `flake8-to-ruff` can pick them up.
 
 ## License
 
 MIT
 
 ## Contributing
```

