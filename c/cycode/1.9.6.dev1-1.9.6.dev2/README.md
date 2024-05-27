# Comparing `tmp/cycode-1.9.6.dev1.tar.gz` & `tmp/cycode-1.9.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-1.9.6.dev1.tar", max compression
+gzip compressed data, was "cycode-1.9.6.dev2.tar", max compression
```

## Comparing `cycode-1.9.6.dev1.tar` & `cycode-1.9.6.dev2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0    42867 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/README.md
--rw-r--r--   0        0        0      114 2024-05-20 09:40:04.535388 cycode-1.9.6.dev1/cycode/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/auth/__init__.py
--rw-r--r--   0        0        0     2897 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/auth/auth_command.py
--rw-r--r--   0        0        0     4722 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/auth/auth_manager.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/configure/__init__.py
--rw-r--r--   0        0        0     5423 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/configure/configure_command.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/ignore/__init__.py
--rw-r--r--   0        0        0     3873 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/ignore/ignore_command.py
--rw-r--r--   0        0        0     2497 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/main_cli.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/report/__init__.py
--rw-r--r--   0        0        0      563 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/report/report_command.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/report/sbom/__init__.py
--rw-r--r--   0        0        0     3429 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/report/sbom/common.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/report/sbom/path/__init__.py
--rw-r--r--   0        0        0     2821 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/report/sbom/path/path_command.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/report/sbom/repository_url/__init__.py
--rw-r--r--   0        0        0     2143 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py
--rw-r--r--   0        0        0     2358 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/report/sbom/sbom_command.py
--rw-r--r--   0        0        0     1533 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/report/sbom/sbom_report_file.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.575272 cycode-1.9.6.dev1/cycode/cli/commands/scan/__init__.py
--rw-r--r--   0        0        0    38584 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/scan/code_scanner.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/scan/commit_history/__init__.py
--rw-r--r--   0        0        0      975 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/scan/commit_history/commit_history_command.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/scan/path/__init__.py
--rw-r--r--   0        0        0      590 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/scan/path/path_command.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/scan/pre_commit/__init__.py
--rw-r--r--   0        0        0     1605 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/scan/pre_commit/pre_commit_command.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/scan/pre_receive/__init__.py
--rw-r--r--   0        0        0     2699 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/scan/pre_receive/pre_receive_command.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/scan/repository/__init__.py
--rw-r--r--   0        0        0     2710 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/scan/repository/repository_command.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/scan/scan_ci/__init__.py
--rw-r--r--   0        0        0     1588 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/scan/scan_ci/ci_integrations.py
--rw-r--r--   0        0        0      552 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/scan/scan_ci/scan_ci_command.py
--rw-r--r--   0        0        0     5082 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/scan/scan_command.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/version/__init__.py
--rw-r--r--   0        0        0      509 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/commands/version/version_command.py
--rw-r--r--   0        0        0      466 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/config.py
--rw-r--r--   0        0        0      463 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/config.yaml
--rw-r--r--   0        0        0     6194 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     2109 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0     1620 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/exceptions/handle_report_sbom_errors.py
--rw-r--r--   0        0        0     2785 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/exceptions/handle_scan_errors.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/files_collector/__init__.py
--rw-r--r--   0        0        0     5468 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/files_collector/excluder.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/files_collector/iac/__init__.py
--rw-r--r--   0        0        0     2457 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/files_collector/iac/tf_content_generator.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/files_collector/models/__init__.py
--rw-r--r--   0        0        0     1247 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/files_collector/models/in_memory_zip.py
--rw-r--r--   0        0        0     4393 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/files_collector/path_documents.py
--rw-r--r--   0        0        0     4940 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/files_collector/repository_documents.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/files_collector/sca/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/files_collector/sca/maven/__init__.py
--rw-r--r--   0        0        0     2417 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0     1136 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     3119 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     6398 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/files_collector/sca/sca_code_scanner.py
--rw-r--r--   0        0        0     1836 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/files_collector/zip_documents.py
--rw-r--r--   0        0        0      387 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/main.py
--rw-r--r--   0        0        0     2051 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/models.py
--rw-r--r--   0        0        0       93 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0     2395 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/printers/console_printer.py
--rw-r--r--   0        0        0     2290 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0     1613 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/printers/printer_base.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/printers/tables/__init__.py
--rw-r--r--   0        0        0     7660 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/printers/tables/sca_table_printer.py
--rw-r--r--   0        0        0     2281 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/printers/tables/table.py
--rw-r--r--   0        0        0      480 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/printers/tables/table_models.py
--rw-r--r--   0        0        0     5216 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/printers/tables/table_printer.py
--rw-r--r--   0        0        0     2400 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/printers/tables/table_printer_base.py
--rw-r--r--   0        0        0    10484 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      630 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4939 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     7591 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     2987 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0      745 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/user_settings/jwt_creator.py
--rw-r--r--   0        0        0        0 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0      211 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/utils/enum_utils.py
--rw-r--r--   0        0        0     1584 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/utils/get_api_client.py
--rw-r--r--   0        0        0     1953 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0     9716 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/utils/progress_bar.py
--rw-r--r--   0        0        0     2794 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/utils/scan_batch.py
--rw-r--r--   0        0        0      334 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      978 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     2034 2024-05-20 09:39:54.579272 cycode-1.9.6.dev1/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2748 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      934 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0       71 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1777 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     1072 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cyclient/client_creator.py
--rw-r--r--   0        0        0     2937 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      120 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      257 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     3570 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      670 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     3600 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0     1318 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cyclient/headers.py
--rw-r--r--   0        0        0    13226 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cyclient/models.py
--rw-r--r--   0        0        0     3971 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cyclient/report_client.py
--rw-r--r--   0        0        0    12573 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0     1658 2024-05-20 09:39:54.583272 cycode-1.9.6.dev1/cycode/cyclient/scan_config_base.py
--rw-r--r--   0        0        0     3458 2024-05-20 09:40:04.531388 cycode-1.9.6.dev1/pyproject.toml
--rw-r--r--   0        0        0    44445 1970-01-01 00:00:00.000000 cycode-1.9.6.dev1/PKG-INFO
+-rw-r--r--   0        0        0    42867 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/README.md
+-rw-r--r--   0        0        0      114 2024-05-27 09:34:13.427385 cycode-1.9.6.dev2/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/auth/__init__.py
+-rw-r--r--   0        0        0     2897 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/auth/auth_command.py
+-rw-r--r--   0        0        0     4726 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/auth/auth_manager.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/configure/__init__.py
+-rw-r--r--   0        0        0     5423 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/configure/configure_command.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/ignore/__init__.py
+-rw-r--r--   0        0        0     3873 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/ignore/ignore_command.py
+-rw-r--r--   0        0        0     2497 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/main_cli.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/__init__.py
+-rw-r--r--   0        0        0      563 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/report_command.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/__init__.py
+-rw-r--r--   0        0        0     3435 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/common.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/path/__init__.py
+-rw-r--r--   0        0        0     2821 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/path/path_command.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/repository_url/__init__.py
+-rw-r--r--   0        0        0     2143 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py
+-rw-r--r--   0        0        0     2358 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/sbom_command.py
+-rw-r--r--   0        0        0     1533 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/sbom_report_file.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/__init__.py
+-rw-r--r--   0        0        0    38773 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/code_scanner.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/commit_history/__init__.py
+-rw-r--r--   0        0        0      975 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/commit_history/commit_history_command.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/path/__init__.py
+-rw-r--r--   0        0        0      590 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/path/path_command.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/pre_commit/__init__.py
+-rw-r--r--   0        0        0     1605 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/pre_commit/pre_commit_command.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/pre_receive/__init__.py
+-rw-r--r--   0        0        0     2722 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/pre_receive/pre_receive_command.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/repository/__init__.py
+-rw-r--r--   0        0        0     2710 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/repository/repository_command.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/scan_ci/__init__.py
+-rw-r--r--   0        0        0     1588 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/scan_ci/ci_integrations.py
+-rw-r--r--   0        0        0      552 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/scan_ci/scan_ci_command.py
+-rw-r--r--   0        0        0     5082 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/scan/scan_command.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/version/__init__.py
+-rw-r--r--   0        0        0      509 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/commands/version/version_command.py
+-rw-r--r--   0        0        0      466 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/config.py
+-rw-r--r--   0        0        0      463 2024-05-27 09:34:03.007367 cycode-1.9.6.dev2/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     6194 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     2109 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/exceptions/handle_report_sbom_errors.py
+-rw-r--r--   0        0        0     2785 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/exceptions/handle_scan_errors.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/__init__.py
+-rw-r--r--   0        0        0     6243 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/excluder.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/iac/__init__.py
+-rw-r--r--   0        0        0     2457 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/iac/tf_content_generator.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/models/__init__.py
+-rw-r--r--   0        0        0     1247 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/models/in_memory_zip.py
+-rw-r--r--   0        0        0     4394 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/path_documents.py
+-rw-r--r--   0        0        0     4940 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/repository_documents.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/sca/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/sca/maven/__init__.py
+-rw-r--r--   0        0        0     2412 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0     1136 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     3119 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     6400 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/sca/sca_code_scanner.py
+-rw-r--r--   0        0        0     1873 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/files_collector/zip_documents.py
+-rw-r--r--   0        0        0      387 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/main.py
+-rw-r--r--   0        0        0     2051 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/models.py
+-rw-r--r--   0        0        0       93 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0     2395 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/console_printer.py
+-rw-r--r--   0        0        0     2290 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0     1613 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/printer_base.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/tables/__init__.py
+-rw-r--r--   0        0        0     7660 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/tables/sca_table_printer.py
+-rw-r--r--   0        0        0     2281 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/tables/table.py
+-rw-r--r--   0        0        0      480 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/tables/table_models.py
+-rw-r--r--   0        0        0     5216 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/tables/table_printer.py
+-rw-r--r--   0        0        0     2400 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/tables/table_printer_base.py
+-rw-r--r--   0        0        0    10484 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      630 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4939 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     7591 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     2987 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0      745 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/user_settings/jwt_creator.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0      211 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/enum_utils.py
+-rw-r--r--   0        0        0     1584 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/get_api_client.py
+-rw-r--r--   0        0        0     1953 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0     9940 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/progress_bar.py
+-rw-r--r--   0        0        0     2794 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/scan_batch.py
+-rw-r--r--   0        0        0      334 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      967 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     2034 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2748 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      934 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0       71 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1777 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     1072 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/client_creator.py
+-rw-r--r--   0        0        0     3349 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      120 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      257 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     3699 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      670 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     3600 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0     1319 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/headers.py
+-rw-r--r--   0        0        0    13226 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     3971 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/report_client.py
+-rw-r--r--   0        0        0    12573 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0     1658 2024-05-27 09:34:03.011367 cycode-1.9.6.dev2/cycode/cyclient/scan_config_base.py
+-rw-r--r--   0        0        0     3467 2024-05-27 09:34:13.423385 cycode-1.9.6.dev2/pyproject.toml
+-rw-r--r--   0        0        0    44445 1970-01-01 00:00:00.000000 cycode-1.9.6.dev2/PKG-INFO
```

### Comparing `cycode-1.9.6.dev1/README.md` & `cycode-1.9.6.dev2/README.md`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/auth/auth_command.py` & `cycode-1.9.6.dev2/cycode/cli/commands/auth/auth_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/auth/auth_manager.py` & `cycode-1.9.6.dev2/cycode/cli/commands/auth/auth_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,55 +25,55 @@
 
     def __init__(self) -> None:
         self.configuration_manager = ConfigurationManager()
         self.credentials_manager = CredentialsManager()
         self.auth_client = AuthClient()
 
     def authenticate(self) -> None:
-        logger.debug('generating pkce code pair')
+        logger.debug('Generating PKCE code pair')
         code_challenge, code_verifier = self._generate_pkce_code_pair()
 
-        logger.debug('starting authentication session')
+        logger.debug('Starting authentication session')
         session_id = self.start_session(code_challenge)
-        logger.debug('authentication session created, %s', {'session_id': session_id})
+        logger.debug('Authentication session created, %s', {'session_id': session_id})
 
-        logger.debug('opening browser and redirecting to cycode login page')
+        logger.debug('Opening browser and redirecting to Cycode login page')
         self.redirect_to_login_page(code_challenge, session_id)
 
-        logger.debug('starting get api token process')
+        logger.debug('Getting API token')
         api_token = self.get_api_token(session_id, code_verifier)
 
-        logger.debug('saving get api token')
+        logger.debug('Saving API token')
         self.save_api_token(api_token)
 
     def start_session(self, code_challenge: str) -> str:
         auth_session = self.auth_client.start_session(code_challenge)
         return auth_session.session_id
 
     def redirect_to_login_page(self, code_challenge: str, session_id: str) -> None:
         login_url = self._build_login_url(code_challenge, session_id)
         webbrowser.open(login_url)
 
     def get_api_token(self, session_id: str, code_verifier: str) -> 'ApiToken':
         api_token = self.get_api_token_polling(session_id, code_verifier)
         if api_token is None:
-            raise AuthProcessError('getting api token is completed, but the token is missing')
+            raise AuthProcessError('API token pulling is completed, but the token is missing')
         return api_token
 
     def get_api_token_polling(self, session_id: str, code_verifier: str) -> 'ApiToken':
         end_polling_time = time.time() + self.POLLING_TIMEOUT_IN_SECONDS
         while time.time() < end_polling_time:
-            logger.debug('trying to get api token...')
+            logger.debug('Trying to get API token...')
             api_token_polling_response = self.auth_client.get_api_token(session_id, code_verifier)
             if self._is_api_token_process_completed(api_token_polling_response):
-                logger.debug('get api token process completed')
+                logger.debug('Got API token process completion response')
                 return api_token_polling_response.api_token
             if self._is_api_token_process_failed(api_token_polling_response):
-                logger.debug('get api token process failed')
-                raise AuthProcessError('error during getting api token')
+                logger.debug('Got API token process failure response')
+                raise AuthProcessError('Error while obtaining API token')
             time.sleep(self.POLLING_WAIT_INTERVAL_IN_SECONDS)
 
         raise AuthProcessError('session expired')
 
     def save_api_token(self, api_token: 'ApiToken') -> None:
         self.credentials_manager.update_credentials(api_token.client_id, api_token.secret)
```

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/configure/configure_command.py` & `cycode-1.9.6.dev2/cycode/cli/commands/configure/configure_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/ignore/ignore_command.py` & `cycode-1.9.6.dev2/cycode/cli/commands/ignore/ignore_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/main_cli.py` & `cycode-1.9.6.dev2/cycode/cli/commands/main_cli.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/report/report_command.py` & `cycode-1.9.6.dev2/cycode/cli/commands/report/report_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/report/sbom/common.py` & `cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             'error_message': error_message,
             'execution_time': int(end_scan_time - start_scan_time),
             'request_zip_file_size': request_zip_file_size,
         }
 
         client.report_status(report_execution_id, scan_status)
     except Exception as e:
-        logger.debug(f'Failed to send report feedback: {e}')
+        logger.debug('Failed to send report feedback', exc_info=e)
 
 
 def create_sbom_report(
     progress_bar: 'BaseProgressBar',
     client: 'ReportClient',
     report_execution_id: int,
     output_file: Optional[pathlib.Path],
```

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/report/sbom/path/path_command.py` & `cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/path/path_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py` & `cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/repository_url/repository_url_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/report/sbom/sbom_command.py` & `cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/sbom_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/report/sbom/sbom_report_file.py` & `cycode-1.9.6.dev2/cycode/cli/commands/report/sbom/sbom_report_file.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/scan/code_scanner.py` & `cycode-1.9.6.dev2/cycode/cli/commands/scan/code_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 
         if local_scan_result:
             detections_count = local_scan_result.detections_count
             relevant_detections_count = local_scan_result.relevant_detections_count
             scan_id = local_scan_result.scan_id
 
         logger.debug(
-            'Finished scan process, %s',
+            'Processing scan results, %s',
             {
                 'all_violations_count': detections_count,
                 'relevant_violations_count': relevant_detections_count,
                 'scan_id': scan_id,
                 'zip_file_size': zip_file_size,
             },
         )
@@ -242,22 +242,22 @@
         return scan_sca_commit_range(context, path, commit_range)
 
     documents_to_scan = []
     commit_ids_to_scan = []
 
     repo = Repo(path)
     total_commits_count = int(repo.git.rev_list('--count', commit_range))
-    logger.debug(f'Calculating diffs for {total_commits_count} commits in the commit range {commit_range}')
+    logger.debug('Calculating diffs for %s commits in the commit range %s', total_commits_count, commit_range)
 
     progress_bar.set_section_length(ScanProgressBarSection.PREPARE_LOCAL_FILES, total_commits_count)
 
     scanned_commits_count = 0
     for commit in repo.iter_commits(rev=commit_range):
         if _does_reach_to_max_commits_to_scan_limit(commit_ids_to_scan, max_commits_count):
-            logger.debug(f'Reached to max commits to scan count. Going to scan only {max_commits_count} last commits')
+            logger.debug('Reached to max commits to scan count. Going to scan only %s last commits', max_commits_count)
             progress_bar.update(ScanProgressBarSection.PREPARE_LOCAL_FILES, total_commits_count - scanned_commits_count)
             break
 
         progress_bar.update(ScanProgressBarSection.PREPARE_LOCAL_FILES)
 
         commit_id = commit.hexsha
         commit_ids_to_scan.append(commit_id)
@@ -280,15 +280,15 @@
             {'path': path, 'commit_range': commit_range, 'commit_id': commit_id},
         )
 
         documents_to_scan.extend(exclude_irrelevant_documents_to_scan(scan_type, commit_documents_to_scan))
         scanned_commits_count += 1
 
     logger.debug('List of commit ids to scan, %s', {'commit_ids': commit_ids_to_scan})
-    logger.debug('Starting to scan commit range (It may take a few minutes)')
+    logger.debug('Starting to scan commit range (it may take a few minutes)')
 
     scan_documents(context, documents_to_scan, is_git_diff=True, is_commit_range=True)
     return None
 
 
 def scan_documents(
     context: click.Context,
@@ -303,15 +303,16 @@
     progress_bar = context.obj['progress_bar']
 
     if not documents_to_scan:
         progress_bar.stop()
         ConsolePrinter(context).print_error(
             CliError(
                 code='no_relevant_files',
-                message='Error: The scan could not be completed - relevant files to scan are not found.',
+                message='Error: The scan could not be completed - relevant files to scan are not found. '
+                'Enable verbose mode to see more details.',
             )
         )
         return
 
     scan_batch_thread_func = _get_scan_documents_thread_func(context, is_git_diff, is_commit_range, scan_parameters)
     errors, local_scan_results = run_parallel_batched_scan(
         scan_batch_thread_func, documents_to_scan, progress_bar=progress_bar
@@ -388,15 +389,15 @@
     detections_count = relevant_detections_count = 0
     if local_scan_result:
         detections_count = local_scan_result.detections_count
         relevant_detections_count = local_scan_result.relevant_detections_count
         scan_id = local_scan_result.scan_id
 
     logger.debug(
-        'Finished scan process, %s',
+        'Processing commit range scan results, %s',
         {
             'all_violations_count': detections_count,
             'relevant_violations_count': relevant_detections_count,
             'scan_id': scan_id,
             'zip_file_size': zip_file_size,
         },
     )
@@ -471,15 +472,15 @@
 def perform_scan_async(
     cycode_client: 'ScanClient',
     zipped_documents: 'InMemoryZip',
     scan_type: str,
     scan_parameters: dict,
 ) -> ZippedFileScanResult:
     scan_async_result = cycode_client.zipped_file_scan_async(zipped_documents, scan_type, scan_parameters)
-    logger.debug('scan request has been triggered successfully, scan id: %s', scan_async_result.scan_id)
+    logger.debug('Async scan request has been triggered successfully, %s', {'scan_id': scan_async_result.scan_id})
 
     return poll_scan_results(
         cycode_client,
         scan_async_result.scan_id,
         scan_type,
         scan_parameters.get('report'),
     )
@@ -488,15 +489,15 @@
 def perform_scan_sync(
     cycode_client: 'ScanClient',
     zipped_documents: 'InMemoryZip',
     scan_type: str,
     scan_parameters: dict,
 ) -> ZippedFileScanResult:
     scan_results = cycode_client.zipped_file_scan_sync(zipped_documents, scan_type, scan_parameters)
-    logger.debug('scan request has been triggered successfully, scan id: %s', scan_results.id)
+    logger.debug('Sync scan request has been triggered successfully, %s', {'scan_id': scan_results.id})
     return ZippedFileScanResult(
         did_detect=True,
         detections_per_file=_map_detections_per_file(scan_results.detection_messages),
         scan_id=scan_results.id,
     )
 
 
@@ -508,15 +509,17 @@
     scan_parameters: dict,
     timeout: Optional[int] = None,
 ) -> ZippedFileScanResult:
     scan_async_result = cycode_client.multiple_zipped_file_scan_async(
         from_commit_zipped_documents, to_commit_zipped_documents, scan_type, scan_parameters
     )
 
-    logger.debug('scan request has been triggered successfully, scan id: %s', scan_async_result.scan_id)
+    logger.debug(
+        'Async commit range scan request has been triggered successfully, %s', {'scan_id': scan_async_result.scan_id}
+    )
     return poll_scan_results(
         cycode_client, scan_async_result.scan_id, scan_type, scan_parameters.get('report'), timeout
     )
 
 
 def poll_scan_results(
     cycode_client: 'ScanClient',
@@ -548,39 +551,42 @@
 
         time.sleep(consts.SCAN_POLLING_WAIT_INTERVAL_IN_SECONDS)
 
     raise custom_exceptions.ScanAsyncError(f'Failed to complete scan after {polling_timeout} seconds')
 
 
 def print_debug_scan_details(scan_details_response: 'ScanDetailsResponse') -> None:
-    logger.debug(f'Scan update: (scan_id: {scan_details_response.id})')
-    logger.debug(f'Scan status: {scan_details_response.scan_status}')
+    logger.debug(
+        'Scan update, %s', {'scan_id': scan_details_response.id, 'scan_status': scan_details_response.scan_status}
+    )
 
     if scan_details_response.message:
-        logger.debug(f'Scan message: {scan_details_response.message}')
+        logger.debug('Scan message: %s', scan_details_response.message)
 
 
 def print_results(
     context: click.Context, local_scan_results: List[LocalScanResult], errors: Optional[Dict[str, 'CliError']] = None
 ) -> None:
     printer = ConsolePrinter(context)
     printer.print_scan_results(local_scan_results, errors)
 
 
 def get_document_detections(
     scan_result: ZippedFileScanResult, documents_to_scan: List[Document]
 ) -> List[DocumentDetections]:
-    logger.debug('Get document detections')
+    logger.debug('Getting document detections')
 
     document_detections = []
     for detections_per_file in scan_result.detections_per_file:
         file_name = get_path_by_os(detections_per_file.file_name)
         commit_id = detections_per_file.commit_id
 
-        logger.debug('Going to find document of violated file, %s', {'file_name': file_name, 'commit_id': commit_id})
+        logger.debug(
+            'Going to find the document of the violated file., %s', {'file_name': file_name, 'commit_id': commit_id}
+        )
 
         document = _get_document_by_file_name(documents_to_scan, file_name, commit_id)
         document_detections.append(DocumentDetections(document=document, detections=detections_per_file.detections))
 
     return document_detections
 
 
@@ -655,18 +661,18 @@
 
     return scan_parameters
 
 
 def try_get_git_remote_url(path: str) -> Optional[str]:
     try:
         remote_url = Repo(path).remotes[0].config_reader.get('url')
-        logger.debug(f'Found Git remote URL "{remote_url}" in path "{path}"')
+        logger.debug('Found Git remote URL, %s', {'remote_url': remote_url, 'path': path})
         return remote_url
     except Exception as e:
-        logger.debug('Failed to get git remote URL. %s', {'exception_message': str(e)})
+        logger.debug('Failed to get Git remote URL', exc_info=e)
         return None
 
 
 def exclude_irrelevant_detections(
     detections: List[Detection], scan_type: str, command_scan_type: str, severity_threshold: str
 ) -> List[Detection]:
     relevant_detections = _exclude_detections_by_exclusions_configuration(detections, scan_type)
@@ -715,43 +721,43 @@
     return [detection for detection in detections if not _should_exclude_detection(detection, exclusions)]
 
 
 def _should_exclude_detection(detection: Detection, exclusions: Dict) -> bool:
     exclusions_by_value = exclusions.get(consts.EXCLUSIONS_BY_VALUE_SECTION_NAME, [])
     if _is_detection_sha_configured_in_exclusions(detection, exclusions_by_value):
         logger.debug(
-            'Going to ignore violations because is in the values to ignore list, %s',
-            {'sha': detection.detection_details.get('sha512', '')},
+            'Going to ignore violations because they are on the values-to-ignore list, %s',
+            {'value_sha': detection.detection_details.get('sha512', '')},
         )
         return True
 
     exclusions_by_sha = exclusions.get(consts.EXCLUSIONS_BY_SHA_SECTION_NAME, [])
     if _is_detection_sha_configured_in_exclusions(detection, exclusions_by_sha):
         logger.debug(
-            'Going to ignore violations because is in the shas to ignore list, %s',
+            'Going to ignore violations because they are on the SHA ignore list, %s',
             {'sha': detection.detection_details.get('sha512', '')},
         )
         return True
 
     exclusions_by_rule = exclusions.get(consts.EXCLUSIONS_BY_RULE_SECTION_NAME, [])
     if exclusions_by_rule:
         detection_rule = detection.detection_rule_id
         if detection_rule in exclusions_by_rule:
             logger.debug(
-                'Going to ignore violations because is in the shas to ignore list, %s',
+                'Going to ignore violations because they are on the Rule ID ignore list, %s',
                 {'detection_rule': detection_rule},
             )
             return True
 
     exclusions_by_package = exclusions.get(consts.EXCLUSIONS_BY_PACKAGE_SECTION_NAME, [])
     if exclusions_by_package:
         package = _get_package_name(detection)
         if package in exclusions_by_package:
             logger.debug(
-                'Going to ignore violations because is in the packages to ignore list, %s', {'package': package}
+                'Going to ignore violations because they are on the packages-to-ignore list, %s', {'package': package}
             )
             return True
 
     return False
 
 
 def _is_detection_sha_configured_in_exclusions(detection: Detection, exclusions: List[str]) -> bool:
@@ -806,15 +812,15 @@
             'operation_system': platform(),
             'error_message': error_message,
             'scan_type': scan_type,
         }
 
         cycode_client.report_scan_status(scan_type, scan_id, scan_status, should_use_scan_service)
     except Exception as e:
-        logger.debug('Failed to report scan status, %s', {'exception_message': str(e)})
+        logger.debug('Failed to report scan status', exc_info=e)
 
 
 def _generate_unique_id() -> UUID:
     return uuid4()
 
 
 def _does_severity_match_severity_threshold(severity: str, severity_threshold: str) -> bool:
@@ -864,59 +870,61 @@
     if not should_get_report:
         return None
 
     try:
         report_url_response = cycode_client.get_scan_report_url(scan_id, scan_type)
         return report_url_response.report_url
     except Exception as e:
-        logger.debug('Failed to get report url: %s', str(e))
+        logger.debug('Failed to get report URL', exc_info=e)
 
 
 def wait_for_detections_creation(
     cycode_client: 'ScanClient', scan_type: str, scan_id: str, expected_detections_count: int
 ) -> None:
     logger.debug('Waiting for detections to be created')
 
     scan_persisted_detections_count = 0
     polling_timeout = consts.DETECTIONS_COUNT_VERIFICATION_TIMEOUT_IN_SECONDS
     end_polling_time = time.time() + polling_timeout
 
     while time.time() < end_polling_time:
         scan_persisted_detections_count = cycode_client.get_scan_detections_count(scan_type, scan_id)
         logger.debug(
-            f'Excepted {expected_detections_count} detections, got {scan_persisted_detections_count} detections '
-            f'({expected_detections_count - scan_persisted_detections_count} more; '
-            f'{round(end_polling_time - time.time())} seconds left)'
+            'Excepting %s detections, got %s detections (%s more; %s seconds left)',
+            expected_detections_count,
+            scan_persisted_detections_count,
+            expected_detections_count - scan_persisted_detections_count,
+            round(end_polling_time - time.time()),
         )
         if scan_persisted_detections_count == expected_detections_count:
             return
 
         time.sleep(consts.DETECTIONS_COUNT_VERIFICATION_WAIT_INTERVAL_IN_SECONDS)
 
-    logger.debug(f'{scan_persisted_detections_count} detections has been created')
+    logger.debug('%s detections has been created', scan_persisted_detections_count)
     raise custom_exceptions.ScanAsyncError(
         f'Failed to wait for detections to be created after {polling_timeout} seconds'
     )
 
 
 def _map_detections_per_file(detections: List[dict]) -> List[DetectionsPerFile]:
     detections_per_files = {}
     for detection in detections:
         try:
             detection['message'] = detection['correlation_message']
             file_name = _get_file_name_from_detection(detection)
             if file_name is None:
-                logger.debug('file name is missing from detection with id %s', detection.get('id'))
+                logger.debug('File name is missing from detection with ID %s', detection.get('id'))
                 continue
             if detections_per_files.get(file_name) is None:
                 detections_per_files[file_name] = [DetectionSchema().load(detection)]
             else:
                 detections_per_files[file_name].append(DetectionSchema().load(detection))
         except Exception as e:
-            logger.debug('Failed to parse detection: %s', str(e))
+            logger.debug('Failed to parse detection', exc_info=e)
             continue
 
     return [
         DetectionsPerFile(file_name=file_name, detections=file_detections)
         for file_name, file_detections in detections_per_files.items()
     ]
```

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/scan/commit_history/commit_history_command.py` & `cycode-1.9.6.dev2/cycode/cli/commands/scan/commit_history/commit_history_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/scan/path/path_command.py` & `cycode-1.9.6.dev2/cycode/cli/commands/scan/path/path_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/scan/pre_commit/pre_commit_command.py` & `cycode-1.9.6.dev2/cycode/cli/commands/scan/pre_commit/pre_commit_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/scan/pre_receive/pre_receive_command.py` & `cycode-1.9.6.dev2/cycode/cli/commands/scan/pre_receive/pre_receive_command.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,34 +28,35 @@
     try:
         scan_type = context.obj['scan_type']
         if scan_type != consts.SECRET_SCAN_TYPE:
             raise click.ClickException(f'Commit range scanning for {scan_type.upper()} is not supported')
 
         if should_skip_pre_receive_scan():
             logger.info(
-                'A scan has been skipped as per your request.'
-                ' Please note that this may leave your system vulnerable to secrets that have not been detected'
+                'A scan has been skipped as per your request. '
+                'Please note that this may leave your system vulnerable to secrets that have not been detected.'
             )
             return
 
         if is_verbose_mode_requested_in_pre_receive_scan():
             enable_verbose_mode(context)
-            logger.debug('Verbose mode enabled, all log levels will be displayed')
+            logger.debug('Verbose mode enabled: all log levels will be displayed.')
 
         command_scan_type = context.info_name
         timeout = configuration_manager.get_pre_receive_command_timeout(command_scan_type)
         with TimeoutAfter(timeout):
             if scan_type not in consts.COMMIT_RANGE_SCAN_SUPPORTED_SCAN_TYPES:
                 raise click.ClickException(f'Commit range scanning for {scan_type.upper()} is not supported')
 
             branch_update_details = parse_pre_receive_input()
             commit_range = calculate_pre_receive_commit_range(branch_update_details)
             if not commit_range:
                 logger.info(
-                    'No new commits found for pushed branch, %s', {'branch_update_details': branch_update_details}
+                    'No new commits found for pushed branch, %s',
+                    {'branch_update_details': branch_update_details},
                 )
                 return
 
             max_commits_to_scan = configuration_manager.get_pre_receive_max_commits_to_scan_count(command_scan_type)
             scan_commit_range(context, os.getcwd(), commit_range, max_commits_count=max_commits_to_scan)
             perform_post_pre_receive_scan_actions(context)
     except Exception as e:
```

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/scan/repository/repository_command.py` & `cycode-1.9.6.dev2/cycode/cli/commands/scan/repository/repository_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/scan/scan_ci/ci_integrations.py` & `cycode-1.9.6.dev2/cycode/cli/commands/scan/scan_ci/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/scan/scan_ci/scan_ci_command.py` & `cycode-1.9.6.dev2/cycode/cli/commands/scan/scan_ci/scan_ci_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/commands/scan/scan_command.py` & `cycode-1.9.6.dev2/cycode/cli/commands/scan/scan_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/consts.py` & `cycode-1.9.6.dev2/cycode/cli/consts.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/exceptions/custom_exceptions.py` & `cycode-1.9.6.dev2/cycode/cli/exceptions/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/exceptions/handle_report_sbom_errors.py` & `cycode-1.9.6.dev2/cycode/cli/exceptions/handle_report_sbom_errors.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/exceptions/handle_scan_errors.py` & `cycode-1.9.6.dev2/cycode/cli/exceptions/handle_scan_errors.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/files_collector/excluder.py` & `cycode-1.9.6.dev2/cycode/cli/files_collector/excluder.py`

 * *Files 25% similar despite different names*

```diff
@@ -58,71 +58,98 @@
 
 def _does_document_exceed_max_size_limit(content: str) -> bool:
     return get_content_size(content) > consts.FILE_MAX_SIZE_LIMIT_IN_BYTES
 
 
 def _is_relevant_file_to_scan(scan_type: str, filename: str) -> bool:
     if _is_subpath_of_cycode_configuration_folder(filename):
-        logger.debug('file is irrelevant because it is in cycode configuration directory, %s', {'filename': filename})
+        logger.debug(
+            'The file is irrelevant because it is in the Cycode configuration directory, %s',
+            {'filename': filename, 'configuration_directory': consts.CYCODE_CONFIGURATION_DIRECTORY},
+        )
         return False
 
     if _is_path_configured_in_exclusions(scan_type, filename):
-        logger.debug('file is irrelevant because the file path is in the ignore paths list, %s', {'filename': filename})
+        logger.debug('The file is irrelevant because its path is in the ignore paths list, %s', {'filename': filename})
         return False
 
     if not _is_file_extension_supported(scan_type, filename):
-        logger.debug('file is irrelevant because the file extension is not supported, %s', {'filename': filename})
+        logger.debug(
+            'The file is irrelevant because its extension is not supported, %s',
+            {'scan_type': scan_type, 'filename': filename},
+        )
         return False
 
     if is_binary_file(filename):
-        logger.debug('file is irrelevant because it is binary file, %s', {'filename': filename})
+        logger.debug('The file is irrelevant because it is a binary file, %s', {'filename': filename})
         return False
 
     if scan_type != consts.SCA_SCAN_TYPE and _does_file_exceed_max_size_limit(filename):
-        logger.debug('file is irrelevant because its exceeded max size limit, %s', {'filename': filename})
+        logger.debug(
+            'The file is irrelevant because it has exceeded the maximum size limit, %s',
+            {
+                'max_file_size': consts.FILE_MAX_SIZE_LIMIT_IN_BYTES,
+                'file_size': get_file_size(filename),
+                'filename': filename,
+            },
+        )
         return False
 
     if scan_type == consts.SCA_SCAN_TYPE and not _is_file_relevant_for_sca_scan(filename):
         return False
 
     return True
 
 
 def _is_file_relevant_for_sca_scan(filename: str) -> bool:
     if any(sca_excluded_path in filename for sca_excluded_path in consts.SCA_EXCLUDED_PATHS):
-        logger.debug("file is irrelevant because it is from node_modules's inner path, %s", {'filename': filename})
+        logger.debug(
+            'The file is irrelevant because it is from the inner path of node_modules, %s', {'filename': filename}
+        )
         return False
 
     return True
 
 
 def _is_relevant_document_to_scan(scan_type: str, filename: str, content: str) -> bool:
     if _is_subpath_of_cycode_configuration_folder(filename):
         logger.debug(
-            'document is irrelevant because it is in cycode configuration directory, %s', {'filename': filename}
+            'The document is irrelevant because it is in the Cycode configuration directory, %s',
+            {'filename': filename, 'configuration_directory': consts.CYCODE_CONFIGURATION_DIRECTORY},
         )
         return False
 
     if _is_path_configured_in_exclusions(scan_type, filename):
         logger.debug(
-            'document is irrelevant because the document path is in the ignore paths list, %s', {'filename': filename}
+            'The document is irrelevant because its path is in the ignore paths list, %s', {'filename': filename}
         )
         return False
 
     if not _is_file_extension_supported(scan_type, filename):
-        logger.debug('document is irrelevant because the file extension is not supported, %s', {'filename': filename})
+        logger.debug(
+            'The document is irrelevant because its extension is not supported, %s',
+            {'scan_type': scan_type, 'filename': filename},
+        )
         return False
 
     if is_binary_content(content):
-        logger.debug('document is irrelevant because it is binary, %s', {'filename': filename})
+        logger.debug('The document is irrelevant because it is a binary file, %s', {'filename': filename})
         return False
 
     if scan_type != consts.SCA_SCAN_TYPE and _does_document_exceed_max_size_limit(content):
-        logger.debug('document is irrelevant because its exceeded max size limit, %s', {'filename': filename})
+        logger.debug(
+            'The document is irrelevant because it has exceeded the maximum size limit, %s',
+            {
+                'max_document_size': consts.FILE_MAX_SIZE_LIMIT_IN_BYTES,
+                'document_size': get_content_size(content),
+                'filename': filename,
+            },
+        )
         return False
+
     return True
 
 
 def _is_file_extension_supported(scan_type: str, filename: str) -> bool:
     filename = filename.lower()
 
     if scan_type == consts.INFRA_CONFIGURATION_SCAN_TYPE:
```

### Comparing `cycode-1.9.6.dev1/cycode/cli/files_collector/iac/tf_content_generator.py` & `cycode-1.9.6.dev2/cycode/cli/files_collector/iac/tf_content_generator.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/files_collector/models/in_memory_zip.py` & `cycode-1.9.6.dev2/cycode/cli/files_collector/models/in_memory_zip.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/files_collector/path_documents.py` & `cycode-1.9.6.dev2/cycode/cli/files_collector/path_documents.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     # because some of them were excluded, we should subtract the excluded files count
     # from the progress bar section length
     excluded_files_count = len(all_files_to_scan) - len(relevant_files_to_scan)
     progress_bar_section_len = progress_bar_section_len - excluded_files_count
     progress_bar.set_section_length(progress_bar_section, progress_bar_section_len)
 
     logger.debug(
-        'Found all relevant files for scanning %s', {'paths': paths, 'file_to_scan_count': len(relevant_files_to_scan)}
+        'Found all relevant files for scanning, %s', {'paths': paths, 'file_to_scan_count': len(relevant_files_to_scan)}
     )
 
     return relevant_files_to_scan
 
 
 def _generate_document(file: str, scan_type: str, content: str, is_git_diff: bool) -> Document:
     if is_iac(scan_type) and is_tfplan_file(file, content):
```

### Comparing `cycode-1.9.6.dev1/cycode/cli/files_collector/repository_documents.py` & `cycode-1.9.6.dev2/cycode/cli/files_collector/repository_documents.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py` & `cycode-1.9.6.dev2/cycode/cli/files_collector/sca/maven/base_restore_maven_dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     return join_paths(get_file_dir(path), generated_file_name)
 
 
 def execute_command(command: List[str], file_name: str, command_timeout: int) -> Optional[str]:
     try:
         dependencies = shell(command, command_timeout)
     except Exception as e:
-        logger.debug('Failed to restore dependencies shell comment. %s', {'filename': file_name, 'exception': str(e)})
+        logger.debug('Failed to restore dependencies via shell command, %s', {'filename': file_name}, exc_info=e)
         return None
 
     return dependencies
 
 
 class BaseRestoreMavenDependencies(ABC):
     def __init__(self, context: click.Context, is_git_diff: bool, command_timeout: int) -> None:
```

### Comparing `cycode-1.9.6.dev1/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py` & `cycode-1.9.6.dev2/cycode/cli/files_collector/sca/maven/restore_gradle_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py` & `cycode-1.9.6.dev2/cycode/cli/files_collector/sca/maven/restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/files_collector/sca/sca_code_scanner.py` & `cycode-1.9.6.dev2/cycode/cli/files_collector/sca/sca_code_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 def add_ecosystem_related_files_if_exists(
     documents: List[Document], repo: Optional[Repo] = None, commit_rev: Optional[str] = None
 ) -> None:
     documents_to_add: List[Document] = []
     for doc in documents:
         ecosystem = get_project_file_ecosystem(doc)
         if ecosystem is None:
-            logger.debug('failed to resolve project file ecosystem: %s', doc.path)
+            logger.debug('Failed to resolve project file ecosystem: %s', doc.path)
             continue
 
         documents_to_add.extend(get_doc_ecosystem_related_project_files(doc, documents, ecosystem, commit_rev, repo))
 
     documents.extend(documents_to_add)
 
 
@@ -90,28 +90,28 @@
     documents_to_add: Dict[str, Document],
     restore_dependencies: 'BaseRestoreMavenDependencies',
     document: Document,
 ) -> None:
     if restore_dependencies.is_project(document):
         restore_dependencies_document = restore_dependencies.restore(document)
         if restore_dependencies_document is None:
-            logger.warning('Error occurred while trying to generate dependencies tree. %s', {'filename': document.path})
+            logger.warning('Error occurred while trying to generate dependencies tree, %s', {'filename': document.path})
             return
 
         if restore_dependencies_document.content is None:
-            logger.warning('Error occurred while trying to generate dependencies tree. %s', {'filename': document.path})
+            logger.warning('Error occurred while trying to generate dependencies tree, %s', {'filename': document.path})
             restore_dependencies_document.content = ''
         else:
             is_monitor_action = context.obj.get('monitor')
             project_path = context.params.get('path')
             manifest_file_path = get_manifest_file_path(document, is_monitor_action, project_path)
-            logger.debug(f'Succeeded to generate dependencies tree on path: {manifest_file_path}')
+            logger.debug('Succeeded to generate dependencies tree on path: %s', manifest_file_path)
 
         if restore_dependencies_document.path in documents_to_add:
-            logger.debug(f'Duplicate document on restore for path: {restore_dependencies_document.path}')
+            logger.debug('Duplicate document on restore for path: %s', restore_dependencies_document.path)
         else:
             documents_to_add[restore_dependencies_document.path] = restore_dependencies_document
 
 
 def add_dependencies_tree_document(
     context: click.Context, documents_to_scan: List[Document], is_git_diff: bool = False
 ) -> None:
@@ -143,9 +143,9 @@
         return None
 
 
 def perform_pre_scan_documents_actions(
     context: click.Context, scan_type: str, documents_to_scan: List[Document], is_git_diff: bool = False
 ) -> None:
     if scan_type == consts.SCA_SCAN_TYPE and not context.obj.get(consts.SCA_SKIP_RESTORE_DEPENDENCIES_FLAG):
-        logger.debug('Perform pre scan document add_dependencies_tree_document action')
+        logger.debug('Perform pre-scan document add_dependencies_tree_document action')
         add_dependencies_tree_document(context, documents_to_scan, is_git_diff)
```

### Comparing `cycode-1.9.6.dev1/cycode/cli/files_collector/zip_documents.py` & `cycode-1.9.6.dev2/cycode/cli/files_collector/zip_documents.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import time
+import timeit
 from pathlib import Path
 from typing import List, Optional
 
 from cycode.cli import consts
 from cycode.cli.exceptions import custom_exceptions
 from cycode.cli.files_collector.models.in_memory_zip import InMemoryZip
 from cycode.cli.models import Document
@@ -18,29 +18,30 @@
             raise custom_exceptions.ZipTooLargeError(consts.ZIP_MAX_SIZE_LIMIT_IN_BYTES)
 
 
 def zip_documents(scan_type: str, documents: List[Document], zip_file: Optional[InMemoryZip] = None) -> InMemoryZip:
     if zip_file is None:
         zip_file = InMemoryZip()
 
-    start_zip_creation_time = time.time()
+    start_zip_creation_time = timeit.default_timer()
 
     for index, document in enumerate(documents):
         _validate_zip_file_size(scan_type, zip_file.size)
 
         logger.debug(
-            'adding file to zip, %s', {'index': index, 'filename': document.path, 'unique_id': document.unique_id}
+            'Adding file to ZIP, %s',
+            {'index': index, 'filename': document.path, 'unique_id': document.unique_id},
         )
         zip_file.append(document.path, document.unique_id, document.content)
 
     zip_file.close()
 
-    end_zip_creation_time = time.time()
+    end_zip_creation_time = timeit.default_timer()
     zip_creation_time = int(end_zip_creation_time - start_zip_creation_time)
-    logger.debug('finished to create zip file, %s', {'zip_creation_time': zip_creation_time})
+    logger.debug('Finished to create ZIP file, %s', {'zip_creation_time': zip_creation_time})
 
     if zip_file.configuration_manager.get_debug_flag():
         zip_file_path = Path.joinpath(Path.cwd(), f'{scan_type}_scan_{end_zip_creation_time}.zip')
-        logger.debug('writing zip file to disk, %s', {'zip_file_path': zip_file_path})
+        logger.debug('Writing ZIP file to disk, %s', {'zip_file_path': zip_file_path})
         zip_file.write_on_disk(zip_file_path)
 
     return zip_file
```

### Comparing `cycode-1.9.6.dev1/cycode/cli/models.py` & `cycode-1.9.6.dev2/cycode/cli/models.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/printers/console_printer.py` & `cycode-1.9.6.dev2/cycode/cli/printers/console_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/printers/json_printer.py` & `cycode-1.9.6.dev2/cycode/cli/printers/json_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/printers/printer_base.py` & `cycode-1.9.6.dev2/cycode/cli/printers/printer_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/printers/tables/sca_table_printer.py` & `cycode-1.9.6.dev2/cycode/cli/printers/tables/sca_table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/printers/tables/table.py` & `cycode-1.9.6.dev2/cycode/cli/printers/tables/table.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/printers/tables/table_printer.py` & `cycode-1.9.6.dev2/cycode/cli/printers/tables/table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/printers/tables/table_printer_base.py` & `cycode-1.9.6.dev2/cycode/cli/printers/tables/table_printer_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/printers/text_printer.py` & `cycode-1.9.6.dev2/cycode/cli/printers/text_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/user_settings/base_file_manager.py` & `cycode-1.9.6.dev2/cycode/cli/user_settings/base_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/user_settings/config_file_manager.py` & `cycode-1.9.6.dev2/cycode/cli/user_settings/config_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/user_settings/configuration_manager.py` & `cycode-1.9.6.dev2/cycode/cli/user_settings/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/user_settings/credentials_manager.py` & `cycode-1.9.6.dev2/cycode/cli/user_settings/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/user_settings/jwt_creator.py` & `cycode-1.9.6.dev2/cycode/cli/user_settings/jwt_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/utils/get_api_client.py` & `cycode-1.9.6.dev2/cycode/cli/utils/get_api_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/utils/path_utils.py` & `cycode-1.9.6.dev2/cycode/cli/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/utils/progress_bar.py` & `cycode-1.9.6.dev2/cycode/cli/utils/progress_bar.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from cycode.cli.utils.enum_utils import AutoCountEnum
 from cycode.cyclient.config import get_logger
 
 if TYPE_CHECKING:
     from click._termui_impl import ProgressBar
     from click.termui import V as ProgressBarValue
 
-
-logger = get_logger('progress bar')
+# use LOGGING_LEVEL=DEBUG env var to see debug logs of this module
+logger = get_logger('progress bar', control_level_in_runtime=False)
 
 
 class ProgressBarSection(AutoCountEnum):
     def has_next(self) -> bool:
         return self.value < len(type(self)) - 1
 
     def next(self) -> 'ProgressBarSection':
@@ -180,15 +180,15 @@
             self.__enter__()
 
     def stop(self) -> None:
         if self._run:
             self.__exit__(None, None, None)
 
     def set_section_length(self, section: 'ProgressBarSection', length: int = 0) -> None:
-        logger.debug(f'set_section_length: {section} {length}')
+        logger.debug('Calling set_section_length, %s', {'section': str(section), 'length': length})
         self._section_lengths[section] = length
 
         if length == 0:
             self._skip_section(section)
         else:
             self._maybe_update_current_section()
 
@@ -199,16 +199,19 @@
     def _skip_section(self, section: 'ProgressBarSection') -> None:
         self._progress_bar.update(self._get_section_length(section))
         self._maybe_update_current_section()
 
     def _increment_section_value(self, section: 'ProgressBarSection', value: int) -> None:
         self._section_values[section] = self._section_values.get(section, 0) + value
         logger.debug(
-            f'_increment_section_value: {section} +{value}. '
-            f'{self._section_values[section]}/{self._section_lengths[section]}'
+            'Calling _increment_section_value: %s +%s. %s/%s',
+            section,
+            value,
+            self._section_values[section],
+            self._section_lengths[section],
         )
 
     def _rerender_progress_bar(self) -> None:
         """Used to update label right after changing the progress bar section."""
         self._progress_bar.update(0)
 
     def _increment_progress(self, section: 'ProgressBarSection') -> None:
@@ -221,15 +224,17 @@
         if not self._current_section.section.has_next():
             return
 
         max_val = self._section_lengths.get(self._current_section.section, 0)
         cur_val = self._section_values.get(self._current_section.section, 0)
         if cur_val >= max_val:
             next_section = self._progress_bar_sections[self._current_section.section.next()]
-            logger.debug(f'_update_current_section: {self._current_section.section} -> {next_section.section}')
+            logger.debug(
+                'Calling _update_current_section:  %s -> %s', self._current_section.section, next_section.section
+            )
 
             self._current_section = next_section
             self._current_section_value = 0
             self._rerender_progress_bar()
 
     def _get_increment_progress_value(self, section: 'ProgressBarSection') -> int:
         max_val = self._section_lengths[section]
```

### Comparing `cycode-1.9.6.dev1/cycode/cli/utils/scan_batch.py` & `cycode-1.9.6.dev2/cycode/cli/utils/scan_batch.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/utils/shell_executor.py` & `cycode-1.9.6.dev2/cycode/cli/utils/shell_executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 
 _SUBPROCESS_DEFAULT_TIMEOUT_SEC = 60
 
 
 def shell(
     command: Union[str, List[str]], timeout: int = _SUBPROCESS_DEFAULT_TIMEOUT_SEC, execute_in_shell: bool = False
 ) -> Optional[str]:
-    logger.debug(f'Executing shell command: {command}')
+    logger.debug('Executing shell command: %s', command)
 
     try:
         result = subprocess.run(
             command,
             timeout=timeout,
             shell=execute_in_shell,  # noqa: S603
             check=True,
             capture_output=True,
         )
 
         return result.stdout.decode('UTF-8').strip()
     except subprocess.CalledProcessError as e:
-        logger.debug(f'Error occurred while running shell command. Exception: {e.stderr}')
+        logger.debug('Error occurred while running shell command', exc_info=e)
     except subprocess.TimeoutExpired as e:
         raise click.Abort(f'Command "{command}" timed out') from e
     except Exception as e:
         raise click.ClickException(f'Unhandled exception: {e}') from e
 
     return None
```

### Comparing `cycode-1.9.6.dev1/cycode/cli/utils/string_utils.py` & `cycode-1.9.6.dev2/cycode/cli/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/utils/task_timer.py` & `cycode-1.9.6.dev2/cycode/cli/utils/task_timer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cli/utils/yaml_utils.py` & `cycode-1.9.6.dev2/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cyclient/auth_client.py` & `cycode-1.9.6.dev2/cycode/cyclient/auth_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cyclient/client_creator.py` & `cycode-1.9.6.dev2/cycode/cyclient/client_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cyclient/config.py` & `cycode-1.9.6.dev2/cycode/cyclient/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 import sys
-from typing import Optional, Union
+from typing import NamedTuple, Optional, Set, Union
 from urllib.parse import urlparse
 
 from cycode.cli import consts
 from cycode.cli.user_settings.configuration_manager import ConfigurationManager
 from cycode.cyclient import config_dev
 
 
@@ -38,34 +38,41 @@
     consts.TIMEOUT_ENV_VAR_NAME: 300,
     consts.LOGGING_LEVEL_ENV_VAR_NAME: logging.INFO,
     config_dev.DEV_MODE_ENV_VAR_NAME: 'false',
 }
 
 configuration = dict(DEFAULT_CONFIGURATION, **os.environ)
 
-_CREATED_LOGGERS = set()
+
+class CreatedLogger(NamedTuple):
+    logger: logging.Logger
+    control_level_in_runtime: bool
+
+
+_CREATED_LOGGERS: Set[CreatedLogger] = set()
 
 
 def get_logger_level() -> Optional[Union[int, str]]:
     config_level = get_val_as_string(consts.LOGGING_LEVEL_ENV_VAR_NAME)
     return logging.getLevelName(config_level)
 
 
-def get_logger(logger_name: Optional[str] = None) -> logging.Logger:
+def get_logger(logger_name: Optional[str] = None, control_level_in_runtime: bool = True) -> logging.Logger:
     new_logger = logging.getLogger(logger_name)
     new_logger.setLevel(get_logger_level())
 
-    _CREATED_LOGGERS.add(new_logger)
+    _CREATED_LOGGERS.add(CreatedLogger(logger=new_logger, control_level_in_runtime=control_level_in_runtime))
 
     return new_logger
 
 
 def set_logging_level(level: int) -> None:
     for created_logger in _CREATED_LOGGERS:
-        created_logger.setLevel(level)
+        if created_logger.control_level_in_runtime:
+            created_logger.logger.setLevel(level)
 
 
 def get_val_as_string(key: str) -> str:
     return configuration.get(key)
 
 
 def get_val_as_bool(key: str, default: str = '') -> bool:
@@ -79,26 +86,28 @@
         return int(val)
 
     return None
 
 
 def is_valid_url(url: str) -> bool:
     try:
-        urlparse(url)
-        return True
-    except ValueError as e:
-        logger.warning(f'Invalid cycode api url: {url}, using default value', e)
+        parsed_url = urlparse(url)
+        return all([parsed_url.scheme, parsed_url.netloc])
+    except ValueError:
         return False
 
 
 logger = get_logger('cycode cli')
 configuration_manager = ConfigurationManager()
 
 cycode_api_url = configuration_manager.get_cycode_api_url()
 if not is_valid_url(cycode_api_url):
+    logger.warning(
+        'Invalid Cycode API URL: %s, using default value (%s)', cycode_api_url, consts.DEFAULT_CYCODE_API_URL
+    )
     cycode_api_url = consts.DEFAULT_CYCODE_API_URL
 
 timeout = get_val_as_int(consts.CYCODE_CLI_REQUEST_TIMEOUT_ENV_VAR_NAME)
 if not timeout:
     timeout = get_val_as_int(consts.TIMEOUT_ENV_VAR_NAME)
 
 dev_mode = get_val_as_bool(config_dev.DEV_MODE_ENV_VAR_NAME)
```

### Comparing `cycode-1.9.6.dev1/cycode/cyclient/cycode_client_base.py` & `cycode-1.9.6.dev2/cycode/cyclient/cycode_client_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,27 +40,33 @@
         endpoint: str,
         headers: Optional[dict] = None,
         without_auth: bool = False,
         hide_response_content_log: bool = False,
         **kwargs,
     ) -> Response:
         url = self.build_full_url(self.api_url, endpoint)
-        logger.debug(f'Executing {method.upper()} request to {url}')
+        logger.debug(
+            'Executing request, %s',
+            {'method': method.upper(), 'url': url},
+        )
 
         timeout = self.timeout
         if 'timeout' in kwargs:
             timeout = kwargs['timeout']
             del kwargs['timeout']
 
         try:
             headers = self.get_request_headers(headers, without_auth=without_auth)
             response = request(method=method, url=url, timeout=timeout, headers=headers, **kwargs)
 
             content = 'HIDDEN' if hide_response_content_log else response.text
-            logger.debug(f'Response {response.status_code} from {url}. Content: {content}')
+            logger.debug(
+                'Receiving response, %s',
+                {'status_code': response.status_code, 'url': url, 'content': content},
+            )
 
             response.raise_for_status()
             return response
         except Exception as e:
             self._handle_exception(e)
 
     def get_request_headers(self, additional_headers: Optional[dict] = None, **kwargs) -> Dict[str, str]:
```

### Comparing `cycode-1.9.6.dev1/cycode/cyclient/cycode_dev_based_client.py` & `cycode-1.9.6.dev2/cycode/cyclient/cycode_dev_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cyclient/cycode_token_based_client.py` & `cycode-1.9.6.dev2/cycode/cyclient/cycode_token_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cyclient/headers.py` & `cycode-1.9.6.dev2/cycode/cyclient/headers.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,13 +34,13 @@
             Used across all requests to correlate logs and metrics.
             It doesn't depend on client instances.
             Lifetime is the same as the process.
         """
         if self._id is None:
             # example: 16fd2706-8baf-433b-82eb-8c7fada847da
             self._id = str(uuid4())
-            logger.debug(f'Correlation ID: {self._id}')
+            logger.debug('Correlation ID: %s', self._id)
 
         return self._id
 
 
 get_correlation_id = _CorrelationId().get_correlation_id
```

### Comparing `cycode-1.9.6.dev1/cycode/cyclient/models.py` & `cycode-1.9.6.dev2/cycode/cyclient/models.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cyclient/report_client.py` & `cycode-1.9.6.dev2/cycode/cyclient/report_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cyclient/scan_client.py` & `cycode-1.9.6.dev2/cycode/cyclient/scan_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/cycode/cyclient/scan_config_base.py` & `cycode-1.9.6.dev2/cycode/cyclient/scan_config_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.9.6.dev1/pyproject.toml` & `cycode-1.9.6.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycode"
-version = "1.9.6.dev1" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
+version = "1.9.6.dev2" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
 description = "Boost security in your dev lifecycle via SAST, SCA, Secrets & IaC scanning."
 keywords=["secret-scan", "cycode", "devops", "token", "secret", "security", "cycode", "code"]
 authors = ["Cycode <support@cycode.com>"]
 license = "MIT"
 repository = "https://github.com/cycodehq/cycode-cli"
 readme = "README.md"
 classifiers = [
@@ -92,14 +92,15 @@
     "RSE",
     "RUF",
     "SIM",
     "T20",
     "TCH",
     "TID",
     "YTT",
+    "G",
 ]
 line-length = 120
 target-version = "py37"
 ignore = [
     "ANN002", # Missing type annotation for `*args`
     "ANN003", # Missing type annotation for `**kwargs`
     "ANN101", # Missing type annotation for `self` in method
```

### Comparing `cycode-1.9.6.dev1/PKG-INFO` & `cycode-1.9.6.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 1.9.6.dev1
+Version: 1.9.6.dev2
 Summary: Boost security in your dev lifecycle via SAST, SCA, Secrets & IaC scanning.
 Home-page: https://github.com/cycodehq/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
 Requires-Python: >=3.7,<3.13
```

