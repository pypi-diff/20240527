# Comparing `tmp/multiversx_sdk_cli-9.5.5.tar.gz` & `tmp/multiversx_sdk_cli-9.6.0.tar.gz`

## Comparing `multiversx_sdk_cli-9.5.5.tar` & `multiversx_sdk_cli-9.6.0.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/__init__.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/accounts.py
--rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_accounts.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_config.py
--rw-r--r--   0        0        0    22514 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_contracts.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_data.py
--rw-r--r--   0        0        0    15634 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_delegation.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_deps.py
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_dns.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_ledger.py
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_localnet.py
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_output.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_password.py
--rw-r--r--   0        0        0    14251 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_shared.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_transactions.py
--rw-r--r--   0        0        0     8856 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_validators.py
--rw-r--r--   0        0        0    11681 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_wallet.py
--rw-r--r--   0        0        0     8226 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/config.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/constants.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/contract_verification.py
--rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/contracts.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cosign_transaction.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/custom_network_provider.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dependency_checker.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dns.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/docker.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/downloader.py
--rw-r--r--   0        0        0     5541 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/errors.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/guards.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/interfaces.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/myprocess.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/sign_verify.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/simulation.py
--rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/transactions.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/utils.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ux.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/version.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/workstation.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/.vscode/settings.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/delegation/__init__.py
--rw-r--r--   0        0        0    12763 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/delegation/staking_provider.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dependencies/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dependencies/install.py
--rw-r--r--   0        0        0    15051 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dependencies/modules.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dependencies/resolution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ledger/__init__.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ledger/config.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ledger/ledger_app_handler.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ledger/ledger_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/__init__.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_default.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_general.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_networking.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_part.py
--rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_root.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_sharding.py
--rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_software.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/constants.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/genesis.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/genesis_json.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/genesis_smart_contracts_json.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/libraries.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/node.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/node_config_toml.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/nodes_setup_json.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/p2p_toml.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/seednode_p2pKey.pem
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_build_software.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_clean.py
--rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_config.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_new.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_prerequisites.py
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_start.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/wallets.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/constants.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/core.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/interfaces.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/migrations.py
--rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/project_base.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/project_rust.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/shared.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/templates.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/do_report.py
--rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/report_creator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/__init__.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/common.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/extracted_feature.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/folder_report.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/project_report.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/wasm_report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/features/__init__.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/features/features.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/features/report_option.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/features/size.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/format/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/format/change_type.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/format/format_options.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/validators/__init__.py
--rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/validators/core.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/validators/validators_file.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/LICENSE
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/pyproject.toml
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.5.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/__init__.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/accounts.py
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_accounts.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_config.py
+-rw-r--r--   0        0        0    22514 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_contracts.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_data.py
+-rw-r--r--   0        0        0    15634 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_delegation.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_deps.py
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_dns.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_ledger.py
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_localnet.py
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_output.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_password.py
+-rw-r--r--   0        0        0    14251 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_shared.py
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_transactions.py
+-rw-r--r--   0        0        0     8856 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_validators.py
+-rw-r--r--   0        0        0    11681 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_wallet.py
+-rw-r--r--   0        0        0     8214 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/config.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/constants.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/contract_verification.py
+-rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/contracts.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cosign_transaction.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/custom_network_provider.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/dependency_checker.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/dns.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/docker.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/downloader.py
+-rw-r--r--   0        0        0     5541 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/errors.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/guards.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/interfaces.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/myprocess.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/sign_verify.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/simulation.py
+-rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/transactions.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/utils.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/ux.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/version.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/workstation.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/.vscode/settings.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/delegation/__init__.py
+-rw-r--r--   0        0        0    12793 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/delegation/staking_provider.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/dependencies/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/dependencies/install.py
+-rw-r--r--   0        0        0    15050 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/dependencies/modules.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/dependencies/resolution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/ledger/__init__.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/ledger/config.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/ledger/ledger_app_handler.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/ledger/ledger_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/__init__.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/config_default.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/config_general.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/config_networking.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/config_part.py
+-rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/config_root.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/config_sharding.py
+-rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/config_software.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/constants.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/genesis.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/genesis_json.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/genesis_smart_contracts_json.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/libraries.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/node.py
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/node_config_toml.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/nodes_setup_json.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/p2p_toml.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/seednode_p2pKey.pem
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/step_build_software.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/step_clean.py
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/step_config.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/step_new.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/step_prerequisites.py
+-rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/step_start.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/wallets.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/constants.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/core.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/interfaces.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/migrations.py
+-rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/project_base.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/project_rust.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/shared.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/templates.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/do_report.py
+-rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/report_creator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/data/__init__.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/data/common.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/data/extracted_feature.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/data/folder_report.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/data/project_report.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/data/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/data/wasm_report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/features/__init__.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/features/features.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/features/report_option.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/features/size.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/format/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/format/change_type.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/format/format_options.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/validators/__init__.py
+-rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/validators/core.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/validators/validators_file.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/LICENSE
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 multiversx_sdk_cli-9.6.0/PKG-INFO
```

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/accounts.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/accounts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_accounts.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_accounts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_config.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_contracts.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_contracts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_data.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_data.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_delegation.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_delegation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_deps.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_deps.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_dns.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_dns.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_ledger.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_ledger.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_localnet.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_localnet.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_output.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_output.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_shared.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_shared.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_transactions.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_transactions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_validators.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_validators.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cli_wallet.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cli_wallet.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/config.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
 def get_defaults() -> Dict[str, Any]:
     return {
         "dependencies.vmtools.tag": "v1.5.24",
         "dependencies.vmtools.urlTemplate.linux": "https://github.com/multiversx/mx-chain-vm-go/archive/{TAG}.tar.gz",
         "dependencies.vmtools.urlTemplate.osx": "https://github.com/multiversx/mx-chain-vm-go/archive/{TAG}.tar.gz",
         "dependencies.vmtools.urlTemplate.windows": "https://github.com/multiversx/mx-chain-vm-go/archive/{TAG}.tar.gz",
-        "dependencies.rust.tag": "nightly-2023-12-11",
+        "dependencies.rust.tag": "stable",
         "dependencies.golang.resolution": "SDK",
         "dependencies.golang.tag": "go1.20.7",
         "dependencies.golang.urlTemplate.linux": "https://golang.org/dl/{TAG}.linux-amd64.tar.gz",
         "dependencies.golang.urlTemplate.osx": "https://golang.org/dl/{TAG}.darwin-amd64.tar.gz",
         "dependencies.golang.urlTemplate.windows": "https://golang.org/dl/{TAG}.windows-amd64.zip",
         "dependencies.twiggy.tag": "",
         "dependencies.sc-meta.tag": "",
```

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/constants.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/constants.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/contract_verification.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/contract_verification.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/contracts.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/contracts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/cosign_transaction.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/cosign_transaction.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/custom_network_provider.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/custom_network_provider.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dns.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/dns.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/docker.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/docker.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/downloader.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/downloader.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/errors.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/errors.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/interfaces.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/interfaces.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/myprocess.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/myprocess.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/sign_verify.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/sign_verify.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/simulation.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/simulation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/transactions.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/transactions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/utils.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/utils.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ux.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/ux.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/version.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/version.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/workstation.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/workstation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/delegation/staking_provider.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/delegation/staking_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,15 @@
             delegation_contract=delegation_contract,
             public_keys=public_keys
         )
         tx.nonce = int(args.nonce)
         tx.version = int(args.version)
         tx.options = int(args.options)
         tx.guardian = args.guardian
+        tx.value = args.value
 
         if args.gas_limit:
             tx.gas_limit = int(args.gas_limit)
 
         tx.signature = bytes.fromhex(owner.sign_transaction(tx))
 
         return tx
```

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dependencies/install.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/dependencies/install.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/dependencies/modules.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/dependencies/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
 
         downloader.download(installer_url, str(installer_path))
         utils.mark_executable(str(installer_path))
 
         if tag:
             toolchain = tag
         else:
-            toolchain = "nightly"
+            toolchain = "stable"
 
         args = [str(installer_path), "--verbose", "--default-toolchain", toolchain, "--profile",
                 "minimal", "--target", "wasm32-unknown-unknown", "-y"]
 
         logger.info("Installing rust.")
         myprocess.run_process(args)
```

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ledger/config.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/ledger/config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ledger/ledger_app_handler.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/ledger/ledger_app_handler.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/ledger/ledger_functions.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/ledger/ledger_functions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_default.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/config_default.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_general.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/config_general.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_networking.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/config_networking.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_part.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/config_part.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_root.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/config_root.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_sharding.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/config_sharding.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/config_software.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/config_software.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/genesis_json.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/genesis_json.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,36 @@
 from typing import Any, Dict, List
 
-from multiversx_sdk_core import Address
-
 from multiversx_sdk_cli.accounts import Account
 from multiversx_sdk_cli.localnet import wallets
 from multiversx_sdk_cli.localnet.config_root import ConfigRoot
-from multiversx_sdk_cli.localnet.genesis import (get_delegation_address,
-                                                 is_foundational_node,
-                                                 is_last_user)
+from multiversx_sdk_cli.localnet.genesis import is_last_user
 
 ENTIRE_SUPPLY = 20000000000000000000000000
 # For localnet, we delegate for 1 node
 DELEGATED_VALUE = 2500000000000000000000
 
 
 def build(config: ConfigRoot) -> List[Any]:
     num_validators = config.num_all_validators()
     genesis_items: List[Dict[str, Any]] = []
     remaining_supply = ENTIRE_SUPPLY
-    remaining_to_delegate = DELEGATED_VALUE
-    delegation_address = get_delegation_address()
 
     for nickname, account in wallets.get_validator_wallets(num_validators).items():
-        if is_foundational_node(nickname):
-            continue
-
         value = 2500000000000000000000
         entry = _build_validator_entry(nickname, account, value)
         genesis_items.append(entry)
         remaining_supply -= value
 
     for nickname, account in wallets.get_users().items():
         # The last user (mike) gets all remaining tokens
         value = remaining_supply if is_last_user(nickname) else 100000000000000000000000
-        delegated_value = remaining_to_delegate if is_last_user(nickname) else 100000000000000000000
-        entry = _build_user_entry(nickname, account, value, delegated_value, delegation_address)
+        entry = _build_user_entry(nickname, account, value)
         genesis_items.append(entry)
         remaining_supply -= value
-        remaining_to_delegate -= delegated_value
 
     return genesis_items
 
 
 def _build_validator_entry(nickname: str, account: Account, value: int) -> Dict[str, Any]:
     return {
         "nickname": nickname,
@@ -52,19 +41,19 @@
         "delegation": {
             "address": "",
             "value": "0"
         }
     }
 
 
-def _build_user_entry(nickname: str, account: Account, value: int, delegated_value: int, delegation_address: Address) -> Dict[str, Any]:
+def _build_user_entry(nickname: str, account: Account, value: int) -> Dict[str, Any]:
     return {
         "nickname": nickname,
         "address": account.address.to_bech32(),
         "supply": str(value),
-        "balance": str(value - delegated_value),
+        "balance": str(value),
         "stakingvalue": "0",
         "delegation": {
-            "address": delegation_address.to_bech32(),
-            "value": str(delegated_value)
+            "address": "",
+            "value": "0"
         }
     }
```

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/libraries.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/libraries.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/node.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/node.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/nodes_setup_json.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/nodes_setup_json.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from typing import Any, Dict, List
 
-from multiversx_sdk_cli.accounts import Account
 from multiversx_sdk_cli.localnet import wallets
 from multiversx_sdk_cli.localnet.config_root import ConfigRoot
-from multiversx_sdk_cli.localnet.genesis import (get_delegation_address,
-                                                 is_foundational_node)
 
 CHAIN_ID = "localnet"
 
 
 def build(config: ConfigRoot) -> Any:
     num_validators = config.num_all_validators()
     initial_nodes: List[Dict[str, str]] = []
 
     for nickname, [pubkey, account] in wallets.get_validators(num_validators).items():
-        entry = _build_initial_nodes_entry(nickname, pubkey, account)
+        entry = {
+            "nickname": nickname,
+            "address": account.address.to_bech32(),
+            "pubkey": pubkey,
+        }
+
         initial_nodes.append(entry)
 
     # Then, patch the list of initial nodes, so that higher indexes will become metachain nodes.
     num_metachain_nodes = config.metashard.num_validators
     num_nodes = len(initial_nodes)
     initial_nodes = initial_nodes[num_nodes - num_metachain_nodes:] + initial_nodes[:num_nodes - num_metachain_nodes]
 
@@ -31,17 +33,7 @@
         "metaChainMinNodes": config.metashard.num_validators,
         "hysteresis": 0,
         "adaptivity": False,
         "chainID": CHAIN_ID,
         "minTransactionVersion": 1,
         "initialNodes": initial_nodes
     }
-
-
-def _build_initial_nodes_entry(nickname: str, pubkey: str, account: Account) -> Dict[str, str]:
-    address = get_delegation_address().bech32() if is_foundational_node(nickname) else account.address.bech32()
-
-    return {
-        "nickname": nickname,
-        "address": address,
-        "pubkey": pubkey,
-    }
```

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/p2p_toml.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/p2p_toml.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_build_software.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/step_build_software.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_config.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/step_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_prerequisites.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/step_prerequisites.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/step_start.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/step_start.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,16 @@
         to_run.append(run([
             "./node",
             "--use-log-view",
             "--log-save",
             f"--log-level={loglevel}",
             "--log-logger-name",
             f"--destination-shard-as-observer={observer.shard}",
-            f"--rest-api-interface={observer.api_interface()}"
+            f"--rest-api-interface={observer.api_interface()}",
+            "--operation-mode=historical-balances"
         ], cwd=observer.folder, delay=NODES_START_DELAY))
 
     # Validators
     for validator in config.validators():
         to_run.append(run([
             "./node",
             "--use-log-view",
```

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/localnet/wallets.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/localnet/wallets.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/__init__.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/core.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/core.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/migrations.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/migrations.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/project_base.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/project_base.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/project_rust.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/project_rust.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/templates.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/templates.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/do_report.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/do_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/report_creator.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/report_creator.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/common.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/data/common.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/extracted_feature.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/data/extracted_feature.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/folder_report.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/data/folder_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/project_report.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/data/project_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/report.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/data/report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/data/wasm_report.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/data/wasm_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/features/report_option.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/features/report_option.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/projects/report/format/change_type.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/projects/report/format/change_type.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/validators/__init__.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/validators/core.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/validators/core.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/multiversx_sdk_cli/validators/validators_file.py` & `multiversx_sdk_cli-9.6.0/multiversx_sdk_cli/validators/validators_file.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/LICENSE` & `multiversx_sdk_cli-9.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/README.md` & `multiversx_sdk_cli-9.6.0/README.md`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-9.5.5/pyproject.toml` & `multiversx_sdk_cli-9.6.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "multiversx-sdk-cli"
-version = "9.5.5"
+version = "9.6.0"
 authors = [
   { name="MultiversX" },
 ]
 license = "MIT"
 description = "MultiversX Smart Contracts Tools"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `multiversx_sdk_cli-9.5.5/PKG-INFO` & `multiversx_sdk_cli-9.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: multiversx-sdk-cli
-Version: 9.5.5
+Version: 9.6.0
 Summary: MultiversX Smart Contracts Tools
 Project-URL: Homepage, https://github.com/multiversx/mx-sdk-py-cli
 Author: MultiversX
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

