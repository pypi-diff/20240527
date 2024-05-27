# Comparing `tmp/ophyd_devices-1.0.2.tar.gz` & `tmp/ophyd_devices-1.1.0.tar.gz`

## Comparing `ophyd_devices-1.0.2.tar` & `ophyd_devices-1.1.0.tar`

### file list

```diff
@@ -1,387 +1,402 @@
--rw-r--r--   0        0        0     7769 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/.gitlab-ci.yml
--rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/README.md
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/.git_hooks/pre-commit
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/.gitlab/issue_templates/bug_report_template.md
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/.gitlab/issue_templates/documentation_update_template.md
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/.gitlab/issue_templates/feature_request_template.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/.gitlab/merge_request_templates/default.md
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.gitignore
--rw-r--r--   0        0        0    19819 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.gitlab-ci.yml
--rw-r--r--   0        0        0    18519 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.pylintrc
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.readthedocs.yaml
--rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/CHANGELOG.md
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/LICENSE
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/README.md
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_config_template.yaml
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.git_hooks/post-commit
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.git_hooks/pre-commit
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.gitlab/issue_templates/bug_report_template.md
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.gitlab/issue_templates/documentation_update_template.md
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.gitlab/issue_templates/feature_request_template.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.gitlab/merge_request_templates/default.md
--rw-r--r--   0        0        0     6867 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/demo.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/pyproject.toml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/__init__.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/bec_magics.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/bec_startup.py
--rw-r--r--   0        0        0     8631 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/main.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/prettytable.py
--rw-r--r--   0        0        0    11090 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/progressbar.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/signals.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/__init__.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/device_progress.py
--rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py
--rw-r--r--   0        0        0    12166 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/__init__.py
--rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/__init__.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/conftest.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py
--rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_bec_client.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_device_progress.py
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py
--rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_live_table.py
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_move_callback.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_pretty_table.py
--rw-r--r--   0        0        0    25202 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py
--rw-r--r--   0        0        0    11064 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/README.md
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/pyproject.toml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/__init__.py
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/alarm_handler.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/async_data.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bec_errors.py
--rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bec_service.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bec_yaml_loader.py
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bl_checks.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bl_conditions.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/callback_handler.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/channel_monitor.py
--rw-r--r--   0        0        0     9619 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/client.py
--rw-r--r--   0        0        0     9264 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/config_helper.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/connector.py
--rw-r--r--   0        0        0    12884 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/dap_plugin_objects.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/dap_plugins.py
--rw-r--r--   0        0        0    31017 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/device.py
--rw-r--r--   0        0        0    23466 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/devicemanager.py
--rw-r--r--   0        0        0    38756 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/endpoints.py
--rw-r--r--   0        0        0     9381 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/file_utils.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/lmfit_serializer.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/logbook_connector.py
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/logger.py
--rw-r--r--   0        0        0    24060 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/messages.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/numpy_encoder.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/observer.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/pdf_writer.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/plugin_helper.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/queue_items.py
--rw-r--r--   0        0        0    41753 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/redis_connector.py
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/request_items.py
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scan_data.py
--rw-r--r--   0        0        0    11042 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scan_items.py
--rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scan_manager.py
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scan_report.py
--rw-r--r--   0        0        0    16698 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scans.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scibec_validator.py
--rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/serialization.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/service_config.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/signature_serializer.py
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/user_scripts_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/configs/__init__.py
--rw-r--r--   0        0        0    41862 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/configs/demo_config.yaml
--rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/configs/openapi_schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/tests/__init__.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/tests/fixtures.py
--rw-r--r--   0        0        0    44047 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/tests/test_config.yaml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/tests/test_service_config.yaml
--rw-r--r--   0        0        0    22495 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/tests/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/__init__.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/import_utils.py
--rw-r--r--   0        0        0    11478 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/proxy.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/rpc_utils.py
--rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/scan_utils.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/threading_utils.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/conftest.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_async_data.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_beamline_checks.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_bec_logger.py
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_bec_messages.py
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_bec_service.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_bl_conditions.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_callback_handler.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_channel_monitor.py
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_config_helper.py
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_core_utils.py
--rw-r--r--   0        0        0    26550 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_dap_plugins.py
--rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_device_manager.py
--rw-r--r--   0        0        0    25863 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_devices.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_file_utils.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_import_utils.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_lmfit_serializer.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_observer.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_pdf_writer.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_plugin_helper.py
--rw-r--r--   0        0        0    15320 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_redis_connector.py
--rw-r--r--   0        0        0    22325 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_redis_connector_fakeredis.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_context.py
--rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_data.py
--rw-r--r--   0        0        0    16743 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_items.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_manager.py
--rw-r--r--   0        0        0     8832 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_object.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_report.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_scibec_validator.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_serializer.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_signature_serializer.py
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_user_scripts_mixin.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_yaml_loader.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/create_plugin_structure.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/init_config.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/gitignore
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/setup_device_server.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/post-commit
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/pre-commit
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/README.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/pyproject.toml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/launch.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/service_handler.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/dap_server.py
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/dap_service.py
--rw-r--r--   0        0        0     9729 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/dap_service_manager.py
--rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/lmfit1d_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/cli/__init__.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/cli/launch.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/__init__.py
--rw-r--r--   0        0        0    19037 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/device_server.py
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/rpc_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/cli/__init__.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/cli/launch.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/devices/__init__.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/devices/config_update_handler.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/devices/device_serializer.py
--rw-r--r--   0        0        0    22629 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/devices/devicemanager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/tests/__init__.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/tests/utils.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/__init__.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/default_writer.py
--rw-r--r--   0        0        0     8768 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/file_writer.py
--rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/file_writer_manager.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/merged_dicts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/cli/__init__.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/cli/launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer_plugins/__init__.py
--rw-r--r--   0        0        0    22204 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/__init__.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/bec_emitter.py
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/emitter.py
--rw-r--r--   0        0        0    16121 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/scan_bundler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/cli/__init__.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/cli/launch.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/__init__.py
--rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/device_validation.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/errors.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/path_optimization.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_assembler.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_guard.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_manager.py
--rw-r--r--   0        0        0    35246 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_queue.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_server.py
--rw-r--r--   0        0        0    18915 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_stubs.py
--rw-r--r--   0        0        0    35721 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_worker.py
--rw-r--r--   0        0        0    51830 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/cli/__init__.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/cli/launch.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_plugins/__init__.py
--rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/tests/__init__.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/tests/fixtures.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/tests/utils.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/__init__.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/repeated_timer.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scihub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/cli/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/cli/launch.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scibec/__init__.py
--rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scibec/config_handler.py
--rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py
--rw-r--r--   0        0        0    10735 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scilog/__init__.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scilog/scilog.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_bec_server_utils/test_main.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_data_processing/conftest.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_data_processing/test_dap_server.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/conftest.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_config_handler.py
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_device_serializer.py
--rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_device_server.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py
--rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_file_writer/conftest.py
--rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_file_writer/test_file_writer.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py
--rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/conftest.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_emitter.py
--rw-r--r--   0        0        0    25417 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/conftest.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_path_optimization.py
--rw-r--r--   0        0        0    11631 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_guard.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py
--rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py
--rw-r--r--   0        0        0    53947 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_worker.py
--rw-r--r--   0        0        0    87794 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scans.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/conftest.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_repeated_timer.py
--rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py
--rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scibec_connector.py
--rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scilog_connector.py
--rwxr-xr-x   0        0        0     3629 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bin/install_bec_dev.sh
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/ci/Dockerfile.run_pytest
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/ci/Dockerfile.run_server
--rwxr-xr-x   0        0        0      347 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/ci/build_python_services.sh
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/ci/docker-compose.yaml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/ci/functionalAccounts.json
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/ci/semantic_release.toml
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/ci/test_config.yaml
--rw-r--r--   0        0        0   307212 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/architecture/BEC.drawio
--rw-r--r--   0        0        0   124683 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/architecture/BEC_config_db.drawio
--rw-r--r--   0        0        0    11580 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/architecture/BEC_config_db.svg
--rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/architecture/bec_architecture.png
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/Makefile
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/conf.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/make.bat
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/requirements.txt
--rw-r--r--   0        0        0    41260 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/_static/bec.png
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/_static/switcher.json
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/_static/css/custom.css
--rw-r--r--   0        0        0  4672990 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/_static/gif/bec_plotter.gif
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0        0        0   310535 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/BEC_context_user_centric.png
--rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/bec_architecture.png
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/bec_device_structure.drawio
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/bec_device_structure.png
--rw-r--r--   0        0        0    17460 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/gauss_scatter_plot.png
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/simulation_context_diagram.drawio
--rw-r--r--   0        0        0    69323 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/simulation_context_diagram.png
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/tab-complete-devices.png
--rw-r--r--   0        0        0    37244 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/vscode_debug_button.png
--rw-r--r--   0        0        0   374770 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/vscode_with_annotations.drawio
--rw-r--r--   0        0        0   711275 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/vscode_with_annotations.png
--rw-r--r--   0        0        0    96330 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/wm-devices.png
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/architecture.md
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/bec_cli.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/bec_config.md
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/bec_gui.md
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/bec_plugins.md
--rw-r--r--   0        0        0     9531 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/bec_sim.md
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/contributing.md
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/data_access.md
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/developer.md
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/event_data.md
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/external_sources.md
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/glossary.md
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/install_developer_env.md
--rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/logs.md
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/modules.rst
--rw-r--r--   0        0        0    17464 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/ophyd.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/reference.md
--rw-r--r--   0        0        0    16016 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/scans.md
--rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/tests.md
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/vscode.md
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/introduction/introduction.md
--rw-r--r--   0        0        0    15455 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/user/command_line_interface.md
--rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/user/data_access_and_plotting.md
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/user/devices.md
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/user/graphical_user_interface.md
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/user/installation.md
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/user/user.md
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/pytest_bec_e2e/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/pytest_bec_e2e/pytest_bec_e2e/__init__.py
--rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/__init__.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/ophyd_patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/configs/__init__.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/configs/ophyd_devices_simulation.yaml
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/configs/ophyd_simulation.yaml
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/configs/sls_devices.yaml
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/SpmBase.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/XbpmBase.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/__init__.py
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/device_list.md
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/epics_motor_ex.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/mono_dccm.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/slits.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/sls_detector.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/sls_devices.py
--rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/specMotors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/interfaces/base_classes/__init__.py
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py
--rw-r--r--   0        0        0    18126 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py
--rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/interfaces/base_classes/psi_detector_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/interfaces/protocols/__init__.py
--rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/interfaces/protocols/bec_protocols.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/__init__.py
--rw-r--r--   0        0        0    27788 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/sim.py
--rw-r--r--   0        0        0    28125 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/sim_data.py
--rw-r--r--   0        0        0    12071 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/sim_frameworks.py
--rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/sim_signals.py
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/sim_test_devices.py
--rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/sim_xtreme.py
--rw-r--r--   0        0        0   671622 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt
--rw-r--r--   0        0        0   669534 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt
--rw-r--r--   0        0        0   670586 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt
--rw-r--r--   0        0        0   668300 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt
--rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/utils/__init__.py
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/utils/bec_device_base.py
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/utils/bec_scaninfo_mixin.py
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/utils/bec_utils.py
--rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/utils/controller.py
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/utils/dynamic_pseudo.py
--rw-r--r--   0        0        0     7309 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/utils/socket.py
--rw-r--r--   0        0        0    10748 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/utils/static_device_test.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/tests/test_controller.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/tests/test_dynamic_pseudo.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/tests/test_ophyd_status_obj.py
--rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/tests/test_simulation.py
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/tests/test_socket.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/tests/test_static_device_test.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/.gitignore
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/LICENSE
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     7769 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/README.md
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/.git_hooks/pre-commit
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/.gitlab/issue_templates/bug_report_template.md
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/.gitlab/issue_templates/documentation_update_template.md
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/.gitlab/issue_templates/feature_request_template.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/.gitlab/merge_request_templates/default.md
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.gitignore
+-rw-r--r--   0        0        0    19819 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.gitlab-ci.yml
+-rw-r--r--   0        0        0    18519 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.pylintrc
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.readthedocs.yaml
+-rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/CHANGELOG.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/LICENSE
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/README.md
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_config_template.yaml
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.git_hooks/post-commit
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.git_hooks/pre-commit
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.gitlab/issue_templates/bug_report_template.md
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.gitlab/issue_templates/documentation_update_template.md
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.gitlab/issue_templates/feature_request_template.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/.gitlab/merge_request_templates/default.md
+-rw-r--r--   0        0        0     6867 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/demo.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/pyproject.toml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/__init__.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/bec_magics.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/bec_startup.py
+-rw-r--r--   0        0        0     8631 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/main.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/prettytable.py
+-rw-r--r--   0        0        0    11090 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/progressbar.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/signals.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/__init__.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/device_progress.py
+-rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py
+-rw-r--r--   0        0        0    12166 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/__init__.py
+-rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/__init__.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/conftest.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py
+-rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_bec_client.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_device_progress.py
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py
+-rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_live_table.py
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_move_callback.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_pretty_table.py
+-rw-r--r--   0        0        0    25202 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py
+-rw-r--r--   0        0        0    11064 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/README.md
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/pyproject.toml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/__init__.py
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/alarm_handler.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/async_data.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bec_errors.py
+-rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bec_service.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bec_yaml_loader.py
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bl_checks.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bl_conditions.py
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/callback_handler.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/channel_monitor.py
+-rw-r--r--   0        0        0     9619 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/client.py
+-rw-r--r--   0        0        0     9264 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/config_helper.py
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/connector.py
+-rw-r--r--   0        0        0    12884 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/dap_plugin_objects.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/dap_plugins.py
+-rw-r--r--   0        0        0    31017 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/device.py
+-rw-r--r--   0        0        0    23466 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/devicemanager.py
+-rw-r--r--   0        0        0    38756 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/endpoints.py
+-rw-r--r--   0        0        0     9381 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/file_utils.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/lmfit_serializer.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/logbook_connector.py
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/logger.py
+-rw-r--r--   0        0        0    24060 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/messages.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/numpy_encoder.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/observer.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/pdf_writer.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/plugin_helper.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/queue_items.py
+-rw-r--r--   0        0        0    41753 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/redis_connector.py
+-rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/request_items.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scan_data.py
+-rw-r--r--   0        0        0    11042 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scan_items.py
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scan_manager.py
+-rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scan_report.py
+-rw-r--r--   0        0        0    16698 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scans.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scibec_validator.py
+-rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/serialization.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/service_config.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/signature_serializer.py
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/user_scripts_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/configs/__init__.py
+-rw-r--r--   0        0        0    41862 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/configs/demo_config.yaml
+-rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/configs/openapi_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/tests/__init__.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/tests/fixtures.py
+-rw-r--r--   0        0        0    44047 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/tests/test_config.yaml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/tests/test_service_config.yaml
+-rw-r--r--   0        0        0    22495 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/tests/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/__init__.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/import_utils.py
+-rw-r--r--   0        0        0    11478 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/proxy.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/rpc_utils.py
+-rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/scan_utils.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/threading_utils.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/conftest.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_async_data.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_beamline_checks.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_bec_logger.py
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_bec_messages.py
+-rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_bec_service.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_bl_conditions.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_callback_handler.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_channel_monitor.py
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_config_helper.py
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_core_utils.py
+-rw-r--r--   0        0        0    26550 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_dap_plugins.py
+-rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_device_manager.py
+-rw-r--r--   0        0        0    25863 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_devices.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_file_utils.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_import_utils.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_lmfit_serializer.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_observer.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_pdf_writer.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_plugin_helper.py
+-rw-r--r--   0        0        0    15320 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_redis_connector.py
+-rw-r--r--   0        0        0    22325 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_redis_connector_fakeredis.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_context.py
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_data.py
+-rw-r--r--   0        0        0    16743 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_items.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_manager.py
+-rw-r--r--   0        0        0     8832 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_object.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_report.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_scibec_validator.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_serializer.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_signature_serializer.py
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_user_scripts_mixin.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/tests/test_yaml_loader.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/create_plugin_structure.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/init_config.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/gitignore
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/setup_device_server.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/post-commit
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/pre-commit
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/README.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/pyproject.toml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/launch.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/service_handler.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/dap_server.py
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/dap_service.py
+-rw-r--r--   0        0        0     9729 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/dap_service_manager.py
+-rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/lmfit1d_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/cli/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/cli/launch.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/__init__.py
+-rw-r--r--   0        0        0    19037 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/device_server.py
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/rpc_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/cli/__init__.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/cli/launch.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/devices/__init__.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/devices/config_update_handler.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/devices/device_serializer.py
+-rw-r--r--   0        0        0    22629 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/devices/devicemanager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/tests/__init__.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/tests/utils.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/__init__.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/default_writer.py
+-rw-r--r--   0        0        0     8768 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/file_writer.py
+-rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/file_writer_manager.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/merged_dicts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/cli/__init__.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/cli/launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer_plugins/__init__.py
+-rw-r--r--   0        0        0    22204 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/__init__.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/bec_emitter.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/emitter.py
+-rw-r--r--   0        0        0    16121 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/scan_bundler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/cli/__init__.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/cli/launch.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/__init__.py
+-rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/device_validation.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/errors.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/path_optimization.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_assembler.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_guard.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_manager.py
+-rw-r--r--   0        0        0    35246 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_queue.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_server.py
+-rw-r--r--   0        0        0    18915 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_stubs.py
+-rw-r--r--   0        0        0    35721 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_worker.py
+-rw-r--r--   0        0        0    51830 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/cli/__init__.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/cli/launch.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_plugins/__init__.py
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/tests/__init__.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/tests/fixtures.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/tests/utils.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/__init__.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/repeated_timer.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scihub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/cli/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/cli/launch.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scibec/__init__.py
+-rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scibec/config_handler.py
+-rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py
+-rw-r--r--   0        0        0    10735 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scilog/__init__.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scilog/scilog.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_bec_server_utils/test_main.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_data_processing/conftest.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_data_processing/test_dap_server.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/conftest.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_config_handler.py
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_device_serializer.py
+-rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_device_server.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py
+-rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_file_writer/conftest.py
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_file_writer/test_file_writer.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py
+-rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/conftest.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_emitter.py
+-rw-r--r--   0        0        0    25417 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/conftest.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_path_optimization.py
+-rw-r--r--   0        0        0    11631 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_guard.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py
+-rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py
+-rw-r--r--   0        0        0    53947 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_worker.py
+-rw-r--r--   0        0        0    87794 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scans.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/conftest.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_repeated_timer.py
+-rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py
+-rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scibec_connector.py
+-rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scilog_connector.py
+-rwxr-xr-x   0        0        0     3629 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/bin/install_bec_dev.sh
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/ci/Dockerfile.run_pytest
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/ci/Dockerfile.run_server
+-rwxr-xr-x   0        0        0      347 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/ci/build_python_services.sh
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/ci/docker-compose.yaml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/ci/functionalAccounts.json
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/ci/semantic_release.toml
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/ci/test_config.yaml
+-rw-r--r--   0        0        0   307212 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/architecture/BEC.drawio
+-rw-r--r--   0        0        0   124683 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/architecture/BEC_config_db.drawio
+-rw-r--r--   0        0        0    11580 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/architecture/BEC_config_db.svg
+-rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/architecture/bec_architecture.png
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/Makefile
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/conf.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/make.bat
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/requirements.txt
+-rw-r--r--   0        0        0    41260 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/_static/bec.png
+-rw-r--r--   0        0        0    13487 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/_static/custom.css
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/_static/switcher.json
+-rw-r--r--   0        0        0  4672990 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/_static/gif/bec_plotter.gif
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/api_reference/api_reference.md
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/api_reference/modules.rst
+-rw-r--r--   0        0        0   310535 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/BEC_context_user_centric.png
+-rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/bec_architecture.png
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/bec_device_structure.drawio
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/bec_device_structure.png
+-rw-r--r--   0        0        0   185658 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/bec_widgets_glance.png
+-rw-r--r--   0        0        0    17460 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/gauss_scatter_plot.png
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/index_api.svg
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/index_contribute.svg
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/index_getting_started.svg
+-rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/index_user_guide.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/portrait_48dp.svg
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/precision_manufacturing_48dp.svg
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/rocket_launch_48dp.svg
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/simulation_context_diagram.drawio
+-rw-r--r--   0        0        0    69323 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/simulation_context_diagram.png
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/tab-complete-devices.png
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/timeline_48dp.svg
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/toc_48dp.svg
+-rw-r--r--   0        0        0    37244 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/vscode_debug_button.png
+-rw-r--r--   0        0        0   374770 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/vscode_with_annotations.drawio
+-rw-r--r--   0        0        0   711275 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/vscode_with_annotations.png
+-rw-r--r--   0        0        0    96330 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/assets/wm-devices.png
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/developer.md
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/glossary.md
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/data_acess/data_access.md
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/data_acess/event_data.md
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/devices/bec_sim.md
+-rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/devices/device_configuration.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/devices/devices.md
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/devices/external_sources.md
+-rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/devices/ophyd.md
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/architecture.md
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/bec_config.md
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/bec_plugins.md
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/contributing.md
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/getting_started.md
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/install_developer_env.md
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/logs.md
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/tests.md
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/vscode.md
+-rw-r--r--   0        0        0    16567 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/scans/scans.md
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/user_interfaces/bec_cli.md
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/user_interfaces/bec_gui.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/developer/user_interfaces/user_interfaces.md
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/introduction/introduction.md
+-rw-r--r--   0        0        0    15455 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/user/command_line_interface.md
+-rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/user/data_access_and_plotting.md
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/user/devices.md
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/user/graphical_user_interface.md
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/user/installation.md
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/docs/source/user/user.md
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/pytest_bec_e2e/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/pytest_bec_e2e/pytest_bec_e2e/__init__.py
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/__init__.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/ophyd_patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/configs/__init__.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/configs/ophyd_devices_simulation.yaml
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/configs/ophyd_simulation.yaml
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/configs/sls_devices.yaml
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/SpmBase.py
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/XbpmBase.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/__init__.py
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/device_list.md
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/epics_motor_ex.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/mono_dccm.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/slits.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/sls_detector.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/sls_devices.py
+-rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/devices/specMotors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/interfaces/base_classes/__init__.py
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py
+-rw-r--r--   0        0        0    18126 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py
+-rw-r--r--   0        0        0    11151 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/interfaces/base_classes/psi_detector_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/interfaces/protocols/bec_protocols.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/__init__.py
+-rw-r--r--   0        0        0    27788 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/sim.py
+-rw-r--r--   0        0        0    28125 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/sim_data.py
+-rw-r--r--   0        0        0    12071 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/sim_frameworks.py
+-rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/sim_signals.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/sim_test_devices.py
+-rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/sim_xtreme.py
+-rw-r--r--   0        0        0   671622 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt
+-rw-r--r--   0        0        0   669534 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt
+-rw-r--r--   0        0        0   670586 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt
+-rw-r--r--   0        0        0   668300 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/utils/__init__.py
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/utils/bec_device_base.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/utils/bec_scaninfo_mixin.py
+-rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/utils/bec_utils.py
+-rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/utils/controller.py
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/utils/dynamic_pseudo.py
+-rw-r--r--   0        0        0     7309 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/utils/socket.py
+-rw-r--r--   0        0        0    10748 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/ophyd_devices/utils/static_device_test.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/tests/test_base_classes.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/tests/test_controller.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/tests/test_dynamic_pseudo.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/tests/test_ophyd_status_obj.py
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/tests/test_simulation.py
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/tests/test_socket.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/tests/test_static_device_test.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ophyd_devices-1.1.0/PKG-INFO
```

### Comparing `ophyd_devices-1.0.2/.gitlab-ci.yml` & `ophyd_devices-1.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/CHANGELOG.md` & `ophyd_devices-1.1.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # CHANGELOG
 
 
 
+## v1.1.0 (2024-05-27)
+
+### Feature
+
+* feat: refactor psi_detector_base class, add tests ([`a0ac8c9`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/a0ac8c9ad701f52429f393a134fd0705583eddb1))
+
+### Refactor
+
+* refactor: add publish file location to base class ([`e8510fb`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/e8510fb249b136781c03849497d85dfb11cca43a))
+
+
 ## v1.0.2 (2024-05-23)
 
 ### Ci
 
 * ci: fixed dependency for bec ([`6630740`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/663074055977ca0a046a81bd9ba5187acf95afed))
 
 * ci: added ci token to update job ([`180891b`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/180891becdc1aa16da0c3b83c407e82a288d36d1))
@@ -143,18 +154,7 @@
 
 ### Feature
 
 * feat: move csaxs devices to plugin structure, fix imports and tests ([`74f6fa7`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/74f6fa7ffdf339399504e15f27564e3f0e43db56))
 
 
 ## v0.32.0 (2024-04-19)
-
-### Ci
-
-* ci: do not wait for additional tests to start ([`b88545f`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/b88545f6864a7d11ca39435906bcbd2cd0bb12b0))
-
-### Feature
-
-* feat: added support for nestes device configs ([`288f394`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/288f39483e83575d0bf3ec7a8e0d872b41b5b183))
-
-
-## v0.31.0 (2024-04-19)
```

### Comparing `ophyd_devices-1.0.2/README.md` & `ophyd_devices-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/.gitlab/issue_templates/documentation_update_template.md` & `ophyd_devices-1.1.0/.gitlab/issue_templates/documentation_update_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/.gitlab/issue_templates/feature_request_template.md` & `ophyd_devices-1.1.0/.gitlab/issue_templates/feature_request_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/.gitlab/merge_request_templates/default.md` & `ophyd_devices-1.1.0/.gitlab/merge_request_templates/default.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/.gitignore` & `ophyd_devices-1.1.0/bec/.gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/.gitlab-ci.yml` & `ophyd_devices-1.1.0/bec/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/.pylintrc` & `ophyd_devices-1.1.0/bec/.pylintrc`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/.readthedocs.yaml` & `ophyd_devices-1.1.0/bec/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/CHANGELOG.md` & `ophyd_devices-1.1.0/bec/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/LICENSE` & `ophyd_devices-1.1.0/bec/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/README.md` & `ophyd_devices-1.1.0/bec/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/.gitlab/issue_templates/documentation_update_template.md` & `ophyd_devices-1.1.0/bec/.gitlab/issue_templates/documentation_update_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/.gitlab/issue_templates/feature_request_template.md` & `ophyd_devices-1.1.0/bec/.gitlab/issue_templates/feature_request_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/.gitlab/merge_request_templates/default.md` & `ophyd_devices-1.1.0/bec/.gitlab/merge_request_templates/default.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/demo.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/demo.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/pyproject.toml` & `ophyd_devices-1.1.0/bec/bec_ipython_client/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/bec_magics.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/bec_magics.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/bec_startup.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/bec_startup.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/main.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/main.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/prettytable.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/prettytable.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/progressbar.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/progressbar.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/signals.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/signals.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/device_progress.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/device_progress.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml` & `ophyd_devices-1.1.0/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_bec_client.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_bec_client.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_device_progress.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_device_progress.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_live_table.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_live_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_move_callback.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/tests/client_tests/test_move_callback.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py` & `ophyd_devices-1.1.0/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/README.md` & `ophyd_devices-1.1.0/bec/bec_lib/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/pyproject.toml` & `ophyd_devices-1.1.0/bec/bec_lib/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/alarm_handler.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/alarm_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/async_data.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/async_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bec_service.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bec_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bec_yaml_loader.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bec_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bl_checks.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bl_checks.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bl_conditions.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/bl_conditions.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/callback_handler.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/callback_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/channel_monitor.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/channel_monitor.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/client.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/client.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/config_helper.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/config_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/connector.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/dap_plugin_objects.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/dap_plugin_objects.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/dap_plugins.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/dap_plugins.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/device.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/device.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/devicemanager.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/devicemanager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/endpoints.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/endpoints.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/file_utils.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/file_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/lmfit_serializer.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/logbook_connector.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/logbook_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/logger.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/logger.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/messages.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/messages.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/numpy_encoder.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/observer.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/observer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/pdf_writer.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/pdf_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/plugin_helper.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/plugin_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/queue_items.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/queue_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/redis_connector.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/redis_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/request_items.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/request_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scan_data.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scan_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scan_items.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scan_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scan_manager.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scan_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scan_report.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scan_report.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scans.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scans.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scibec_validator.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/serialization.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/serialization.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/service_config.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/service_config.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/signature_serializer.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/signature_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/user_scripts_mixin.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/configs/demo_config.yaml` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/configs/demo_config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/configs/openapi_schema.json` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/configs/openapi_schema.json`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/tests/fixtures.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/tests/test_config.yaml` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/tests/test_config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/tests/utils.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/import_utils.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/proxy.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/rpc_utils.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/rpc_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/scan_utils.py` & `ophyd_devices-1.1.0/bec/bec_lib/bec_lib/utils/scan_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_async_data.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_async_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_beamline_checks.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_beamline_checks.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_bec_logger.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_bec_logger.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_bec_messages.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_bec_messages.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_bec_service.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_bec_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_bl_conditions.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_bl_conditions.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_callback_handler.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_callback_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_channel_monitor.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_channel_monitor.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_config_helper.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_config_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_core_utils.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_core_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_dap_plugins.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_dap_plugins.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_device_manager.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_device_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_devices.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_file_utils.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_lmfit_serializer.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_observer.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_plugin_helper.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_plugin_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_redis_connector.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_redis_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_redis_connector_fakeredis.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_redis_connector_fakeredis.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_context.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_context.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_data.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_items.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_manager.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_object.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_object.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_report.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_scan_report.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_serializer.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_signature_serializer.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_signature_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_user_scripts_mixin.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/tests/test_yaml_loader.py` & `ophyd_devices-1.1.0/bec/bec_lib/tests/test_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/util_scripts/create_plugin_structure.py` & `ophyd_devices-1.1.0/bec/bec_lib/util_scripts/create_plugin_structure.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/util_scripts/init_config.py` & `ophyd_devices-1.1.0/bec/bec_lib/util_scripts/init_config.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md` & `ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/gitignore` & `ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py` & `ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py` & `ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml` & `ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py` & `ophyd_devices-1.1.0/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/pyproject.toml` & `ophyd_devices-1.1.0/bec/bec_server/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/launch.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/service_handler.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/service_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/dap_server.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/dap_server.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/dap_service.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/dap_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/dap_service_manager.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/lmfit1d_service.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/cli/launch.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/data_processing/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/device_server.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/device_server.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/rpc_mixin.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/cli/launch.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/devices/config_update_handler.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/devices/config_update_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/devices/device_serializer.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/devices/device_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/devices/devicemanager.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/devices/devicemanager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/tests/utils.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/device_server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/default_writer.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/default_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/file_writer.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/file_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/file_writer_manager.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/merged_dicts.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/merged_dicts.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/cli/launch.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/bec_emitter.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/bec_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/emitter.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/scan_bundler.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/scan_bundler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/cli/launch.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_bundler/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/device_validation.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/device_validation.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/path_optimization.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/path_optimization.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_assembler.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_assembler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_guard.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_guard.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_manager.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_queue.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_queue.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_server.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_server.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_stubs.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_stubs.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_worker.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_worker.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scans.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scans.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/cli/launch.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/tests/utils.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scan_server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/repeated_timer.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/repeated_timer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scihub.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/cli/launch.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scibec/config_handler.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scilog/scilog.py` & `ophyd_devices-1.1.0/bec/bec_server/bec_server/scihub/scilog/scilog.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_bec_server_utils/test_main.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_bec_server_utils/test_main.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/conftest.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/conftest.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_config_handler.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_config_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_device_serializer.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_device_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_device_server.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_device_server.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_file_writer/test_file_writer.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_file_writer/test_file_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/conftest.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/conftest.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_emitter.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_path_optimization.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_path_optimization.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_guard.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_guard.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_worker.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scan_worker.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scans.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scan_server/test_scans.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/conftest.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/conftest.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_repeated_timer.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_repeated_timer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scibec_connector.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scibec_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scilog_connector.py` & `ophyd_devices-1.1.0/bec/bec_server/tests/tests_scihub/test_scilog_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/bin/install_bec_dev.sh` & `ophyd_devices-1.1.0/bec/bin/install_bec_dev.sh`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/ci/Dockerfile.run_pytest` & `ophyd_devices-1.1.0/bec/ci/Dockerfile.run_pytest`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/ci/Dockerfile.run_server` & `ophyd_devices-1.1.0/bec/ci/Dockerfile.run_server`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/ci/docker-compose.yaml` & `ophyd_devices-1.1.0/bec/ci/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/ci/semantic_release.toml` & `ophyd_devices-1.1.0/bec/ci/semantic_release.toml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/architecture/BEC.drawio` & `ophyd_devices-1.1.0/bec/docs/architecture/BEC.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/architecture/BEC_config_db.drawio` & `ophyd_devices-1.1.0/bec/docs/architecture/BEC_config_db.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/architecture/BEC_config_db.svg` & `ophyd_devices-1.1.0/bec/docs/architecture/BEC_config_db.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/architecture/bec_architecture.png` & `ophyd_devices-1.1.0/bec/docs/architecture/bec_architecture.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/Makefile` & `ophyd_devices-1.1.0/bec/docs/source/Makefile`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/conf.py` & `ophyd_devices-1.1.0/bec/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,9 +69,9 @@
 language = "Python"
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "pydata_sphinx_theme"
 html_static_path = ["_static"]
-html_css_files = ["css/custom.css"]
+html_css_files = ["custom.css"]
 html_logo = "_static/bec.png"
```

### Comparing `ophyd_devices-1.0.2/bec/docs/source/make.bat` & `ophyd_devices-1.1.0/bec/docs/source/make.bat`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/_static/bec.png` & `ophyd_devices-1.1.0/bec/docs/source/_static/bec.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/_static/gif/bec_plotter.gif` & `ophyd_devices-1.1.0/bec/docs/source/_static/gif/bec_plotter.gif`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/_templates/custom-class-template.rst` & `ophyd_devices-1.1.0/bec/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/_templates/custom-module-template.rst` & `ophyd_devices-1.1.0/bec/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/assets/BEC_context_user_centric.png` & `ophyd_devices-1.1.0/bec/docs/source/assets/BEC_context_user_centric.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/assets/bec_architecture.png` & `ophyd_devices-1.1.0/bec/docs/source/assets/bec_architecture.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/assets/bec_device_structure.drawio` & `ophyd_devices-1.1.0/bec/docs/source/assets/bec_device_structure.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/assets/bec_device_structure.png` & `ophyd_devices-1.1.0/bec/docs/source/assets/bec_device_structure.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/assets/gauss_scatter_plot.png` & `ophyd_devices-1.1.0/bec/docs/source/assets/gauss_scatter_plot.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/assets/simulation_context_diagram.drawio` & `ophyd_devices-1.1.0/bec/docs/source/assets/simulation_context_diagram.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/assets/simulation_context_diagram.png` & `ophyd_devices-1.1.0/bec/docs/source/assets/simulation_context_diagram.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/assets/tab-complete-devices.png` & `ophyd_devices-1.1.0/bec/docs/source/assets/tab-complete-devices.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/assets/vscode_debug_button.png` & `ophyd_devices-1.1.0/bec/docs/source/assets/vscode_debug_button.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/assets/vscode_with_annotations.drawio` & `ophyd_devices-1.1.0/bec/docs/source/assets/vscode_with_annotations.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/assets/vscode_with_annotations.png` & `ophyd_devices-1.1.0/bec/docs/source/assets/vscode_with_annotations.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/assets/wm-devices.png` & `ophyd_devices-1.1.0/bec/docs/source/assets/wm-devices.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/developer/architecture.md` & `ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/architecture.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 (developer.architecture)= 
 # Architecture
-
 BEC is an event-driven system with Redis as the central component for message passing with a service-oriented backend server. The backend server is composed of multiple smaller services that can be deployed independently. The services are connected to Redis and can communicate with each other solely through the message broker.
 
-```{figure} ../assets/bec_architecture.png
+```{figure} ../../assets/bec_architecture.png
 Architecture diagram. BEC relies on a service-oriented backend server with multiple smaller services and Redis as a central message broker and in-memory database. Moreover, any client can be considered as another service to the entire system with access to the same message broker instance. 
 ```
 
 ## Scan Server
 The Scan Server acts as the primary interface for user requests, tasked with the choreography of the data acquisition. The primary components are:
 * **Scan Guard**: 
 The scan guard checks the incoming requests for validity and rejects invalid requests.
@@ -17,15 +16,15 @@
 The scan queue holds the scan instructions and is responsible for scheduling the scans. Although by default only the primary queue is set up, separate queues can be added, and their corresponding workers are added and removed automatically. This allows for multiple, independent scan queues if parallel activities are required.
 * **Scan Worker**:
 The scan worker executes the scan instructions and if necessary publishes device instructions to Redis. While it does not read out the devices, it potentially waits for devices to complete their operations before continuing with the scan.
 
 ## Device Server
 This service provides a thin layer on top of Bluesky’s Ophyd library to support remote procedure calls (RPC) through Redis. 
 It listens to device instructions sent to Redis and performs the specified operations on [Ophyd objects](#developer.ophyd). 
-The available Ophyd objects are determined by loading a device configuration, either through the client, e.g., through yaml files, or from the connected database. 
+The available Ophyd objects are determined by loading a [device configuration](#developer.ophyd_device_config), typically by loading a YAML file from the command-line interface.
 Providing Ophyd objects through a service layer also facilitates sharing access to devices that require a direct socket connection, bypassing the EPICS layer. 
 
 ## Scan Bundler
 Data streams in a control system are inherently asynchronous. 
 Yet, to simplify the user feedback and data analysis, asynchronous readouts are often synchronized afterwards. 
 The Scan Bundler creates such synchronization barriers based on metadata entries of the individual readouts (e.g., point IDs or time stamps) and broadcasts these synchronized readings as a new data stream to the BEC system.
```

### Comparing `ophyd_devices-1.0.2/bec/docs/source/developer/bec_plugins.md` & `ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/bec_plugins.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 (developer.bec_plugins)=
 # BEC Plugins
-
 BEC plugins are a way to extend the functionality of BEC. They are written in Python and can be used to add new features to BEC or to modify existing ones. This enables beamlines to customize BEC to their needs without having to modify the core code. Plugins can be used for various purposes but the most common ones are:
 * Adding new scan types
 * Adding new device types
 * Adding additional services, e.g. for data analysis
 * Customizing the BEC CLI startup procedure (e.g. to load additional modules)
 * Customizing the file structure
```

### Comparing `ophyd_devices-1.0.2/bec/docs/source/developer/bec_sim.md` & `ophyd_devices-1.1.0/bec/docs/source/developer/devices/bec_sim.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 (developer.bec_sim)=
-# BEC Simulation
-
+# Simulations
 The BEC simulation framework comprises a set of simulated devices. These devices offer a platform for developers to explore, test, or add new features to the core libraries of BEC and BEC-Widgets. Additionally, the end-to-end test framework enables the simulation of user behavior at the beamline, facilitating the testing of newly developed features against common user commands. These end-to-end tests encompass various scans, motions, and scenarios, such as requesting a motor to move beyond its limits or simulating system recovery from user interruptions (CTRL-C). Moreover, the framework enables users to develop scripts, GUIs, or data processing tools without requiring access to the physical devices, facilitating faster development cycles.
 
 ## Architecture
-```{figure} ../assets/simulation_context_diagram.png
+```{figure} ../../assets/simulation_context_diagram.png
 Architecture Diagram:  
 The BEC simulation currently hosts three main device types: `SimMonitor`, `SimPositioner`, and `SimCamera`. Their state, as well as readback value, can be configured within the simulation_state of the device. Additionally, we provide two examples of `DeviceProxies` demonstrating how multiple devices can be linked within the simulation to imitate specific scenarios.
 ```
 
 This architecture diagram illustrates the relevant classes for the simulation and their interconnections. To comprehend individual components fully, we recommend reading the following sections with the architecture in mind.
 
 ## Simulated Devices
```

### Comparing `ophyd_devices-1.0.2/bec/docs/source/developer/contributing.md` & `ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/contributing.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 (developer.contributing)=
 # Contributing
-
 Thank you for considering contributing to BEC! Contributions are essential for improving the project and helping it grow. 
 We welcome your bug reports and feature requests via [GitLab issues](https://gitlab.psi.ch/bec/bec/-/issues?sort=created_date&state=opened), as well as contribution for documentation improvements, and code extensions or improvements.
 
 ## Reporting Bugs or Requesting Features:
 
 - Before submitting a bug report or feature request, please check the [issue tracker](https://gitlab.psi.ch/bec/bec/issues) to avoid duplication.
 - If the issue or feature hasn't been reported, open a new issue with a clear title and description. Be sure to provide steps to reproduce bugs, including _package version_ of the deployed BEC services (e.g. `bec_lib`) and information of your operating system, which will increase chances of reproducing and fixing the reported bug.
```

### Comparing `ophyd_devices-1.0.2/bec/docs/source/developer/external_sources.md` & `ophyd_devices-1.1.0/bec/docs/source/developer/devices/external_sources.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/developer/glossary.md` & `ophyd_devices-1.1.0/bec/docs/source/developer/glossary.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/developer/install_developer_env.md` & `ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/install_developer_env.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 (developer.install_developer_env)=
 # Install developer environment
-
 If your goal is to install BEC in an environment for code development purposes, this section will guide you through the steps.
 In contrast to a deployed production system of BEC, this installation will allow you to edit the code base of BEC actively while you are operating the system.
 In that sense, installing BEC in _[dev]_ mode, is the right choice in case you like to:
 
 - Integrate a new ophyd device at the beamline
 - Add a new feature to the code base of BEC
 - Allow more flexibility within code base, in particular useful during beamline commissioning
```

### Comparing `ophyd_devices-1.0.2/bec/docs/source/developer/logs.md` & `ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/logs.md`

 * *Files 0% similar despite different names*

```diff
@@ -47,19 +47,20 @@
 ## BEC's log monitor
 To monitor the log messages of BEC, BEC provides a log monitor. The log monitor is a cli-based tool that allows you to monitor the log messages of BEC in real-time. The log monitor can be started via
 
 ```bash
 bec-log-monitor
 ```
 
-```{note}
+````{note}
 If redis is running on a different host or port, you can specify the redis address via the `--redis` flag, e.g. 
 ```bash
 bec-log-monitor --redis my_bec_vm:6379
 ```
+````
 
 The log monitor also allows you to filter log messages by strings or regular expressions. To this end, you can specify the filter via the `--filter` flag, e.g. 
 
 ```bash
 bec-log-monitor --filter "my_device"
 ```
```

### Comparing `ophyd_devices-1.0.2/bec/docs/source/developer/ophyd.md` & `ophyd_devices-1.1.0/bec/docs/source/developer/devices/ophyd.md`

 * *Files 25% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Based on the type of device, BEC expects ophyd devices to provide certain functionality.
 Signal and Device are the most simple type of devices that are used within BEC.
 A signal has no sub-components, while a devices may contain sub-devices as well as sub-signals.
 Nevertheless, the interface provided by Ophyd allows both to share a similar interface. 
 Overall, BEC differentiates between `device`, `signal`, `positioner` and `flyer`.
 A diagram with the hierarchy of inheritance is shown below.
 
-```{figure} ../assets/bec_device_structure.png
+```{figure} ../../assets/bec_device_structure.png
 Inheritance scheme for devices and signals in BEC.
 ```
 We note that this hierarchy is inspired by different base class from Ophyd:
 `Device`, `Signal`, `PositionerBase` and `FlyerInterface`, while also enhancing certain aspects of these classes for ease of use.
 
 ### Core functionality
 The following section lists core properties and methods. 
@@ -172,115 +172,7 @@
 
 * **kickoff() -> ophyd.DeviceStatus**\
 Upon calling kickoff, the flyer should start and return a status object that resolves once the flyer flies, i.e. is ready to or already acquiring data.
 
 * **complete() -> ophyd.DeviceStatus**\
 The complete method of the flyer returns a status object. 
 This status should resolve once the flyer finishes, thus, the method can be used to identify when a flyer is finished.
-
-(developer.ophyd_device_config)=
-## Ophyd device configuration
-As mentioned before, BEC creates representative devices and signals dynamically on the devices server, following the specifications given in the device configuration. 
-As explained in the [device configuration](#developer.bec_config) section, the device configuration can be loaded from and stored to a yaml file and contains all necessary information about the devices. 
-
-An example of an ophyd device based on EPICS is a single PV, e.g. the synchrotron's ring current: 
-
-```yaml
-curr:
-  readoutPriority: baseline
-  description: SLS ring current
-  deviceClass: EpicsSignalRO
-  deviceConfig:
-    auto_monitor: true
-    read_pv: ARIDI-PCT:CURRENT
-  deviceTags:
-    - cSAXS
-  onFailure: buffer
-  enabled: true
-  readOnly: true
-  softwareTrigger: false
-```
-
-The following sections explain the different parts of the device configuration in more detail.
-
-* **deviceClass** \
-The device class specifies the type of the device. In the example above, the device class is `EpicsSignalRO`, which is a read-only signal based on EPICS. Another example is `EpicsMotor` for motors based on EPICS. For a full list of available device classes, please refer to the [Ophyd documentation](https://nsls-ii.github.io/ophyd/architecture.html#device-classes) and the [Ophyd devices repository](https://gitlab.psi.ch/bec/ophyd_devices).
-
-* **deviceConfig** \
-The device config contains the configuration of the device. In the example above, the device config contains the read PV (`read_pv`). The read PV is the PV that is read out by the device. In this case, the read PV is `ARIDI-PCT:CURRENT`. The device config can contain any configuration parameter that is supported by the device class. 
-The device is constructed by passing the device config to the device class. In the example above, the device is constructed by calling `EpicsSignalRO(name='curr', read_pv='ARIDI-PCT:CURRENT', auto_monitor=True)`.
-
-* **readoutPriority** \
-The readout priority specifies the priority with which the device is read out. For BEC controlled readouts, set the readout priority either to `on_request`, `baseline` or `monitored`. The "on_request" priority is used for devices that should not be read out during the scan, yet are configured to be read out manually. The baseline priority is used for devices that are read out at the beginning of the scan and whose value does not change during the scan. The monitored priority is used for devices that are read out during the scan and whose value may change during the scan. If the readout of the device is asynchronous to the monitored devices, set the readout priority to `async`. For devices that are read out continuously, set the readout priority to `continuous`. 
-
-* **enabled** \
-The enabled status specifies whether the device is enabled. 
-
-* **readOnly** \
-The read only indicates if the device is read-only. When set to true, writing to the device is disabled. It's optional in the device configuration and defaults to false.
-
-* **softwareTrigger** \
-The software trigger determines if BEC should explicitly invoke the device's trigger method during a scan. It's an optional parameter in the device configuration, defaulting to false
-
-* **deviceTags** \
-The device tags contain the tags of the device. The tags are used to group devices and to filter devices.
-
-* **onFailure** \
-The on failure parameter specifies the behavior of the device in case of a failure. It can be either `buffer`, `retry` or `raise`. If an error occurs and the on failure parameter is set to `buffer`, the device readout will fall back to the last value in Redis. If the on failure parameter is set to `retry`, the device readout will retry to read the device and raises an error if it fails again. If the on failure parameter is set to `raise`, the device readout will raise an error immediately.
-
-* **description** \
-The description contains the description of the device. It is used to provide additional information about the device.
-
-## Combining config files
-The device configuration can be split into multiple files. This can be useful to group devices by their functionality or to split the configuration into smaller files for better maintainability. To combine multiple device configuration files, use the `!include` tag in the device configuration.  The paths can be either relative or absolute. Please note that the `!include` tag cannot be placed at the root level of the device configuration and must be within a dictionary, e.g.:
-
-```yaml
-base_config:
-  - !include ./path/to/base_config.yaml
-
-endstation:
-  - !include ./path/to/endstation_config.yaml
-
-curr:
-  readoutPriority: baseline
-  description: SLS ring current
-  deviceClass: EpicsSignalRO
-  deviceConfig:
-    auto_monitor: true
-    read_pv: ARIDI-PCT:CURRENT
-  deviceTags:
-    - cSAXS
-  onFailure: buffer
-  enabled: true
-  readOnly: true
-  softwareTrigger: false
-```
-
-In the example above, the `base_config.yaml` and `endstation_config.yaml` files are included in the device configuration. The `curr` device is defined directly in the device configuration. Alternatively, the `base_config.yaml` and `endstation_config.yaml` files can bec combined into a single tag:
-  
-```yaml
-external_config:
-  - !include ./path/to/base_config.yaml
-  - !include ./path/to/endstation_config.yaml
-```
-
-For a single file, the `!include` tag can also be merged into a single line:
-
-```yaml
-base_config: !include ./path/to/base_config.yaml
-```
-
-
-(developer.ophyd.config_validation)=
-## Validation of the device config
-To avoid errors during loading of the device config, the device config should be validated before loading it. This can be done by installing the `ophyd_devices` package and running the following command:
-
-```bash
-ophyd_test --config ./path/to/my/config/file.yaml
-```
-
-This will perform a static validation of the device config and will print any errors that are found. For checking if the devices can be created and connect successfully, an additional flag can be passed:
-
-```bash
-ophyd_test --config ./path/to/my/config/file.yaml --connect
-``` 
-
```

### Comparing `ophyd_devices-1.0.2/bec/docs/source/developer/scans.md` & `ophyd_devices-1.1.0/bec/docs/source/developer/scans/scans.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 (developer.scans)=
-# BEC Scans
+# Scans
 BEC uses scans to orchestrate the data acquisition. While script-based scans can also be defined in the command-line interface, acquisitions that require more complex orchestration should be defined as scan plugins for the BEC scan server. This section describes the basic structure of a scan and how to create a scan plugin.
 
 ## Scan Structure
-A scan in BEC is a Python class that inherits from the `ScanBase` class and implements methods that should be executed in a specific order.
+A scan in BEC is a Python class that inherits from the [`ScanBase`](/api_reference/_autosummary/bec_server.scan_server.scans.ScanBase.rst#bec_server.scan_server.scans.ScanBase) class and implements methods that should be executed in a specific order.
 
 ````{dropdown} View code: ScanBase class
 :icon: code-square
 :animate: fade-in-slide-down
 
-```{literalinclude} ../../../bec_server/bec_server/scan_server/scans.py
+```{literalinclude} ../../../../bec_server/bec_server/scan_server/scans.py
 :language: python
 :pyobject: ScanBase
 ```
 ````
 
-The order of execution is defined by the `run` method, which is called by the scan server. By default, the `run` method calls the following methods in the following order:
+The order of execution is defined by the [`run`](/api_reference/_autosummary/bec_server.scan_server.scans.ScanBase.rst#bec_server.scan_server.scans.ScanBase.run) method, which is called by the scan server. By default, the `run` method calls the following methods in the following order:
 
-```{literalinclude} ../../../bec_server/bec_server/scan_server/scans.py
+```{literalinclude} ../../../../bec_server/bec_server/scan_server/scans.py
 :language: python
 :pyobject: ScanBase.run
 ```
 
 The `run` method is a generator function that, like most other scan methods, yields control to the scan server after each method call. This allows the scan server to handle asynchronous operations, such as moving motors or waiting for certain events. The scan server will call the next method in the scan after the current method has completed. All methods that set or retrieve data from devices must be implemented as generator functions.
 
 ```{seealso}
@@ -33,29 +33,29 @@
 The following structure is targeted at step scans, i.e. scans where the scan server is in control of the scan and the overall progress is determined by the number of steps within the scan. Modifications of the structure as needed for fly scans are described later on.
 
 #### Preparation for the scan
 After reading out the current scan motor positions with `read_scan_motors`, the scan server will call the `prepare_positions` method to prepare the scan positions. This method should calculate two values: the number of points in the scan (`self.num_pos`) and the positions of the scan motors (`self.positions`). The `num_pos` attribute must be of type `int` while the `positions` attribute must be of type `np.ndarray` with the shape `n x m`, where `n` is the number of points in the scan and `m` is the number of scan motors. The method should also ensure that the calculated positions are within soft limits of the devices. This can be achieved, for example, by calling the `_check_limits` method. 
 
 The default implementation of the `prepare_positions` method in the `ScanBase` class is as follows:
 
-```{literalinclude} ../../../bec_server/bec_server/scan_server/scans.py
+```{literalinclude} ../../../../bec_server/bec_server/scan_server/scans.py
 :language: python
 :pyobject: ScanBase.prepare_positions
 ``` 
 
 In addition to simply calculating the positions, the default implementation also respects the user's request to perform the scan relative to the current position or absolute (`relative=True` or `relative=False`) by adding the position offset using `_set_position_offset`.
 
 
 `````{note}
 New scans that only require a new way of calculating the positions can simply override the `_calculate_positions` method as it is done e.g. in the `FermatSpiralScan` class.
 ````{dropdown} View code: FermatSpiralScan class
 :icon: code-square
 :animate: fade-in-slide-down
 
-```{literalinclude} ../../../bec_server/bec_server/scan_server/scans.py
+```{literalinclude} ../../../../bec_server/bec_server/scan_server/scans.py
 :language: python
 :pyobject: FermatSpiralScan
 ```
 ````
 `````
 
 The `scan_report_instructions` method is then called to update the instructions for user interfaces. In particular, there are three options for the developer to choose from: 
@@ -66,31 +66,31 @@
 
 #### Starting the scan
 The scan server will then call the `open_scan` method to open the scan, followed by the `stage` method to stage all devices (see also: [ophyd devices](#developer.ophyd_devices.device)). 
 Once all devices are staged and thus ready for the upcoming scan, a baseline reading is triggered. This will read out all devices that are on `readout_priority="baseline"` and are currently enabled (see also: [ophyd device configuration](#developer.ophyd_device_config)).
 
 It is sometimes necessary to perform additional operations before the core of the scan is executed. In BEC, these operations can be implemented in the `pre_scan` method:
 
-```{literalinclude} ../../../bec_server/bec_server/scan_server/scans.py
+```{literalinclude} ../../../../bec_server/bec_server/scan_server/scans.py
 :language: python
 :pyobject: ScanBase.pre_scan
 ```
 
 If the class attribute `pre_move` is set to `True`, the default `pre_scan` method will move the scan motors to the first position before the scan core is executed and afterwards call the `pre_scan` method of all devices that have a `pre_scan` method implemented.
 
 Now that all motors are ready and in position, we are finally ready to start the core of the scan. This is done by calling the `scan_core` method. Its default implementation is quite simple:
 
-```{literalinclude} ../../../bec_server/bec_server/scan_server/scans.py
+```{literalinclude} ../../../../bec_server/bec_server/scan_server/scans.py
 :language: python
 :pyobject: ScanBase.scan_core
 ```
 
 For each position in the scan, the method `_at_each_point` is called, providing the current index and a list of positions. The default implementation of `_at_each_point` performs the following actions:
 
-```{literalinclude} ../../../bec_server/bec_server/scan_server/scans.py
+```{literalinclude} ../../../../bec_server/bec_server/scan_server/scans.py
 :language: python
 :pyobject: ScanBase._at_each_point
 ```
 
 1. Move the scan motors to the target position. 
 1. Let the device settle for a specified time (default: `settling_time=0`).
 1. Send out a trigger. 
@@ -131,15 +131,15 @@
 
 The following example shows the configuration of the line scan:
 
 ````{dropdown} View code: LineScan class
 :icon: code-square
 :animate: fade-in-slide-down
 
-```{literalinclude} ../../../bec_server/bec_server/scan_server/scans.py
+```{literalinclude} ../../../../bec_server/bec_server/scan_server/scans.py
 :language: python
 :pyobject: LineScan
 ```
 ````
 
 ### Scan Structure for a Fly Scan
 Fly scans are scans where the scan server does not trigger every step and thus cannot determine the overall progress. Instead, the progress is determined by a specified device, e.g. a detector's total number of acquired frames or the number of triggers sent out by a controller.
@@ -148,60 +148,60 @@
 Both types of fly scans provide dedicated base classes that can and should be used as a starting point for new fly scans. The base classes are `SyncFlyScanBase` and `AsyncFlyScanBase`. 
 `SyncFlyScanBase` unsets the `_calculate_positions`, `read_scan_motors`, `prepare_positions` and `scan_core` methods as they must be implemented differently for fly scans and are highly dependent on the specific requirements of the scan. In addition, the `SyncFlyScanBase` adds the `monitor_sync` property that must be implemented by the developer. This property should return the name of the device that is used to synchronize the scan.
 
 ````{dropdown} View code: SyncFlyScanBase class
 :icon: code-square
 :animate: fade-in-slide-down
 
-```{literalinclude} ../../../bec_server/bec_server/scan_server/scans.py
+```{literalinclude} ../../../../bec_server/bec_server/scan_server/scans.py
 :language: python
 :pyobject: SyncFlyScanBase
 ```
 ````
 
 `AsyncFlyScansBase` inherits from `SyncFlyScansBase` and set the `monitor_sync` property to "bec" as the monitored devices should be synced by BEC itself and not by an external device.
 
 ````{dropdown} View code: AsyncFlyScanBase class
 :icon: code-square
 :animate: fade-in-slide-down
 
-```{literalinclude} ../../../bec_server/bec_server/scan_server/scans.py
+```{literalinclude} ../../../../bec_server/bec_server/scan_server/scans.py
 :language: python
 :pyobject: AsyncFlyScanBase
 ```
 ````
 
 ### Scan stubs - the building blocks of a scan
 In order to simplify the creation of new scans, BEC provides a set of scan stubs that can be used as building blocks for new scans. The scan stubs are located in `bec_server/bec_server/scan_server/scan_stubs.py`. The following scan stubs are available:
 
 *Device operations*
-- [`set_and_wait`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.set_and_wait) Set a device to a value and wait for it to finish.
-- [`read_and_wait`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.read_and_wait) Read a device and wait for it to finish.
-- [`stage`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.stage) Stage a device.
-- [`unstage`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.unstage) Unstage a device.
-- [`kickoff`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.kickoff) Kickoff a device. Usually only needed for fly scans.
-- [`complete`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.complete) Wait for a device to finish.
-- [`get_req_status`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.get_req_status) Check if a device request status matches the given RID and DIID.
-- [`get_device_progress`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.get_device_progress) Get the progress of a device. 
-- [`pre_scan`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.pre_scan) Trigger the pre_scan method of a device.
-- [`baseline_reading`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.baseline_reading) Trigger the baseline readings. 
-- [`wait`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.wait) Wait for an event to finish. Could be a trigger, a readout or a movement. 
-- [`read`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.read) Read from a device.
-- [`trigger`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.trigger) Trigger a device.
-- [`set`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.set) Set a device to a value.
-- [`rpc`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.rpc) Send an RPC command to a device.
-- [`send_rpc_and_wait`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.send_rpc_and_wait) Send an RPC command to a device and wait for it to finish.
+- [`set_and_wait`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.set_and_wait) Set a device to a value and wait for it to finish.
+- [`read_and_wait`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.read_and_wait) Read a device and wait for it to finish.
+- [`stage`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.stage) Stage a device.
+- [`unstage`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.unstage) Unstage a device.
+- [`kickoff`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.kickoff) Kickoff a device. Usually only needed for fly scans.
+- [`complete`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.complete) Wait for a device to finish.
+- [`get_req_status`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.get_req_status) Check if a device request status matches the given RID and DIID.
+- [`get_device_progress`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.get_device_progress) Get the progress of a device. 
+- [`pre_scan`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.pre_scan) Trigger the pre_scan method of a device.
+- [`baseline_reading`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.baseline_reading) Trigger the baseline readings. 
+- [`wait`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.wait) Wait for an event to finish. Could be a trigger, a readout or a movement. 
+- [`read`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.read) Read from a device.
+- [`trigger`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.trigger) Trigger a device.
+- [`set`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.set) Set a device to a value.
+- [`rpc`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.rpc) Send an RPC command to a device.
+- [`send_rpc_and_wait`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.send_rpc_and_wait) Send an RPC command to a device and wait for it to finish.
 
 *Scan operations*
-- [`open_scan`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.open_scan) Open a scan.
-- [`close_scan`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.close_scan) Close a scan. 
-- [`publish_data_as_read`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.publish_data_as_read) Publish data as read.
-- [`open_scan_def`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.open_scan_def) Open a scan definition. 
-- [`close_scan_def`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.close_scan_def) Close a scan definition. 
-- [`scan_report_instruction`](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.scan_report_instruction) Update the scan report instruction.
+- [`open_scan`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.open_scan) Open a scan.
+- [`close_scan`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.close_scan) Close a scan. 
+- [`publish_data_as_read`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.publish_data_as_read) Publish data as read.
+- [`open_scan_def`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.open_scan_def) Open a scan definition. 
+- [`close_scan_def`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.close_scan_def) Close a scan definition. 
+- [`scan_report_instruction`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.scan_report_instruction) Update the scan report instruction.
 
-More information on the scan stubs can be found in the [API reference](./_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs).
+More information on the scan stubs can be found in the [API reference](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs).
```

### Comparing `ophyd_devices-1.0.2/bec/docs/source/developer/tests.md` & `ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/tests.md`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,14 @@
     - by default Redis stays filled with keys added during the test
     - the scope of the `bec_servers` fixture changes dynamically from "session" to "function" if `--flush-redis` option is given
     - note: if Redis flushing is enabled, BEC servers are restarted at each test (need `--start-servers`, see above)
 - `--bec-redis-cmd` can be used to specify the command line for Redis execution
     - could be `docker run ...` for example, otherwise it defaults to `redis-server`
 
 ### BEC client fixtures
-
 Depending how the new code interfaces with BEC, the following fixtures provide a `BECClient` object:
 
 - `bec_client_with_demo_config` is a fixture returning a `BECIPythonClient` object, which also initializes BEC with the demo config
 (simulation hardware).
 - _`bec_client_lib_with_demo_config` returns a simple `BECClient` object instead of IPython client)._
 - `bec_client_fixture` provides a BEC IPython object similar to `bec_client_with_demo_config`, with a cleaned scan queue.
 - _`bec_client_lib` is the same as `bec_client_fixture`, but with a `BECClient` object (no IPython)._
```

### Comparing `ophyd_devices-1.0.2/bec/docs/source/developer/vscode.md` & `ophyd_devices-1.1.0/bec/docs/source/developer/getting_started/vscode.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ## Extensions
 Visual Studio Code (VSCode) relies heavily on extensions to provide additional functionality. You can install extensions from the Extensions view (⇧⌘X on MacOS, Ctrl+Shift+X on Windows and Linux). The following extensions are recommended for developing Python applications with BEC:
 - Python (provided by Microsoft)
 - Black Formatter (provided by Microsoft)
 
 ## Configuration
 
-```{figure} ../assets/vscode_with_annotations.png
+```{figure} ../../assets/vscode_with_annotations.png
 :align: center
 :alt: VSCode editor with annotations
 :width: 800
 ```
 
 ### Appearance
 You can customize the appearance of Visual Studio Code by opening the command palette (⇧⌘P on MacOS, Ctrl+Shift+P on Windows and Linux) and typing "color theme". You can then select the color theme that you want to use. 
@@ -49,15 +49,16 @@
 
 ### Starting a service from VSCode
 Before you start a service from VSCode, you need to ensure that the service is installed and that the environment is set up correctly. 
 ```{note}
 Some services such as the device server, the file writer and the scan server are actively checking if another instance of the service is already running. If you start a service that is ought to be unique, you will get an error message saying that another instance of the service is already running. Please make sure to stop the service before starting a new instance.
 ```
 All services provide a `launch.py` file in their cli directory, e.g. `bec/bec_server/bec_server/device_server/cli/launch.py`. You can start the service by opening the `launch.py` file and then clicking on the "Debug" button in the top right corner of the window. This will start the service in debug mode, and you can see the output of the service in the Debug Console. 
-```{note}
+````{note}
 The debug button looks like a play button with a bug on it. If you don't see the debug button, you can click on the "Run" menu and select "Start Debugging".
-````{figure} ../assets/vscode_debug_button.png
+```{figure} ../../assets/vscode_debug_button.png
 :align: center
 :alt: Debug button in VSCode
 :width: 400
 ```
+````
```

### Comparing `ophyd_devices-1.0.2/bec/docs/source/introduction/introduction.md` & `ophyd_devices-1.1.0/bec/docs/source/introduction/introduction.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/user/command_line_interface.md` & `ophyd_devices-1.1.0/bec/docs/source/user/command_line_interface.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/user/data_access_and_plotting.md` & `ophyd_devices-1.1.0/bec/docs/source/user/data_access_and_plotting.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/user/devices.md` & `ophyd_devices-1.1.0/bec/docs/source/user/devices.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/user/graphical_user_interface.md` & `ophyd_devices-1.1.0/bec/docs/source/user/graphical_user_interface.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/user/installation.md` & `ophyd_devices-1.1.0/bec/docs/source/user/installation.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/docs/source/user/user.md` & `ophyd_devices-1.1.0/bec/docs/source/user/user.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 * [Command-Line Interface (CLI)](#user.command_line_interface): Interact with BEC through the CLI, including device access, motor control, and scan execution. Learn how to use the scan interface and write your own scripts and macros. 
 * [Graphical User Interface (GUI)](#user.graphical_user_interface): Learn how to utilize the modular widgets and functionalities of the GUI.
 * [Data Access and Plotting](#user.data_access_and_plotting): Examining and plotting scan data for live feedback and online data analysis.
 
 
 For detailed insights into BEC's underlying architecture, customization possibilities, or extensions to deployed systems at the beamline, please explore the [Developer](#developer) section. Enjoy exploring and experimenting with BEC!
 
+```{important}
+If you have any questions or feature requests, please feel free to open an issue on the [GitLab](https://gitlab.psi.ch/bec/bec/-/issues?sort=created_date&state=opened). We are happy to help you with any questions you might have.
+```
+
 ```{toctree}
 ---
 maxdepth: 1
 hidden: true
 ---
 
 installation
```

### Comparing `ophyd_devices-1.0.2/bec/pytest_bec_e2e/pyproject.toml` & `ophyd_devices-1.1.0/bec/pytest_bec_e2e/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py` & `ophyd_devices-1.1.0/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/__init__.py` & `ophyd_devices-1.1.0/ophyd_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/ophyd_patch.py` & `ophyd_devices-1.1.0/ophyd_devices/ophyd_patch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/configs/ophyd_devices_simulation.yaml` & `ophyd_devices-1.1.0/ophyd_devices/configs/ophyd_devices_simulation.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/configs/ophyd_simulation.yaml` & `ophyd_devices-1.1.0/ophyd_devices/configs/ophyd_simulation.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/devices/SpmBase.py` & `ophyd_devices-1.1.0/ophyd_devices/devices/SpmBase.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/devices/XbpmBase.py` & `ophyd_devices-1.1.0/ophyd_devices/devices/XbpmBase.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/devices/__init__.py` & `ophyd_devices-1.1.0/ophyd_devices/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/devices/device_list.md` & `ophyd_devices-1.1.0/ophyd_devices/devices/device_list.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/devices/epics_motor_ex.py` & `ophyd_devices-1.1.0/ophyd_devices/devices/epics_motor_ex.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/devices/mono_dccm.py` & `ophyd_devices-1.1.0/ophyd_devices/devices/mono_dccm.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/devices/slits.py` & `ophyd_devices-1.1.0/ophyd_devices/devices/slits.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/devices/sls_detector.py` & `ophyd_devices-1.1.0/ophyd_devices/devices/sls_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/devices/sls_devices.py` & `ophyd_devices-1.1.0/ophyd_devices/devices/sls_devices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/devices/specMotors.py` & `ophyd_devices-1.1.0/ophyd_devices/devices/specMotors.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py` & `ophyd_devices-1.1.0/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py` & `ophyd_devices-1.1.0/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/interfaces/base_classes/psi_detector_base.py` & `ophyd_devices-1.1.0/ophyd_devices/utils/static_device_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,330 +1,325 @@
+import argparse
+import copy
 import os
-import time
+import traceback
+from io import TextIOWrapper
 
-from bec_lib.device import DeviceStatus
-from bec_lib.file_utils import FileWriter
-from ophyd import Device
-from ophyd.device import Staged
+import ophyd
+from bec_lib.bec_yaml_loader import yaml_load
+from bec_lib.scibec_validator import SciBecValidator
 
-from ophyd_devices.utils import bec_utils
-from ophyd_devices.utils.bec_scaninfo_mixin import BecScaninfoMixin
+from ophyd_devices.utils.bec_device_base import BECDevice
 
+try:
+    from bec_server.device_server.devices.devicemanager import DeviceManagerDS as device_manager
+except ImportError:
+    device_manager = None
 
-class DetectorInitError(Exception):
-    """Raised when initiation of the device class fails,
-    due to missing device manager or not started in sim_mode."""
 
+class StaticDeviceAnalysisError(Exception):
+    """Error class for static device analysis"""
 
-class CustomDetectorMixin:
-    """
-    Mixin class for custom detector logic
 
-    This class is used to implement BL specific logic for the detector.
-    It is used in the PSIDetectorBase class.
+class StaticDeviceTest:
+    """Class to perform tests on an ophyd device config file."""
 
-    For the integration of a new detector, the following functions should
-    help with integrating functionality, but additional ones can be added.
+    def __init__(self, config: str, output_file: TextIOWrapper) -> None:
+        """
+        Args:
+            config(str): path to the config file
+            output_file(TextIOWrapper): file to write the output to
+        """
+        self.config_file = config
+        self.config = self.read_config(config)
+        self.file = output_file
 
-    Check PSIDetectorBase for the functions that are called during relevant function calls of
-    stage, unstage, trigger, stop and _init.
-    """
+    @staticmethod
+    def read_config(config) -> dict:
+        """
+        Read the config file
 
-    def __init__(self, *_args, parent: Device = None, **_kwargs) -> None:
-        self.parent = parent
+        Args:
+            config(str): path to the config file
 
-    def initialize_default_parameter(self) -> None:
+        Returns:
+            dict: config content
         """
-        Init parameters for the detector
+        content = yaml_load(config)
+        return content
 
-        Raises (optional):
-            DetectorTimeoutError: if detector cannot be initialized
+    def _check_all_signals_of_device(self, name: str, device: ophyd.Device) -> None:
         """
+        Check if all signals of the device that are not omitted are configured with auto_monitor=True
 
-    def initialize_detector(self) -> None:
+        Args:
+            name(str): name of the device
+            device(ophyd.Device): device object
         """
-        Init parameters for the detector
+        for _, sub_name, item in device.walk_components():
+            if not issubclass(item.cls, ophyd.signal.EpicsSignalBase):
+                continue
+            if not item.is_signal:
+                continue
+            if not item.kind == ophyd.Kind.omitted:
+                continue
+            # check if auto_monitor is in kwargs
+            self._has_auto_monitor(f"{name}/{sub_name}", item.kwargs)
 
-        Raises (optional):
-            DetectorTimeoutError: if detector cannot be initialized
+    def _check_epics_motor(self, name: str, config: dict) -> None:
         """
+        Check if the epics motor config is valid.
 
-    def initialize_detector_backend(self) -> None:
+        Args:
+            name(str): name of the device
+            config(dict): device config
         """
-        Init parameters for teh detector backend (filewriter)
+        if "prefix" in config["deviceConfig"]:
+            return
+        msg_suffix = ""
+
+        # check if the device specifies a read_pv instead of a prefix.
+        # This is a common copy-paste error.
+        if "read_pv" in config["deviceConfig"]:
+            msg_suffix = "Maybe a typo? The device specifies a read_pv instead."
+        raise ValueError(f"{name}: does not specify the prefix. {msg_suffix}")
 
-        Raises (optional):
-            DetectorTimeoutError: if filewriter cannot be initialized
+    def _check_epics_signal(self, name: str, config: dict) -> None:
         """
+        Check if the epics signal config is valid. The device must specify a read_pv.
 
-    def prepare_detector(self) -> None:
-        """
-        Prepare detector for the scan
+        Args:
+            name(str): name of the device
+            config(dict): device config
         """
+        self._has_auto_monitor(name, config["deviceConfig"])
+        if "read_pv" not in config["deviceConfig"]:
+            raise ValueError(f"{name}: does not specify the read_pv")
 
-    def prepare_detector_backend(self) -> None:
-        """
-        Prepare detector backend for the scan
+    def check_device_classes(self, name: str, conf: dict) -> int:
         """
+        Run checks on the device class
 
-    def stop_detector(self) -> None:
-        """
-        Stop the detector
-        """
+        Args:
+            name(str): name of the device
+            conf(dict): device config
 
-    def stop_detector_backend(self) -> None:
-        """
-        Stop the detector backend
+        Returns:
+            int: 0 if all checks passed, 1 otherwise
         """
+        try:
+            dev_class = device_manager._get_device_class(conf["deviceClass"])
+
+            if issubclass(dev_class, ophyd.EpicsMotor):
+                self._check_epics_motor(name, conf)
+                return 0
+
+            if issubclass(dev_class, ophyd.signal.EpicsSignalBase):
+                self._check_epics_signal(name, conf)
+                return 0
+
+            if issubclass(dev_class, ophyd.Device):
+                self._check_all_signals_of_device(name, dev_class)
+            return 0
 
-    def on_trigger(self) -> None:
+        except Exception as e:
+            self.print_and_write(f"ERROR: {name} is not valid: {e}")
+            return 1
+
+    def _has_auto_monitor(self, name: str, config: dict) -> None:
         """
-        Specify actions to be executed upon receiving trigger signal
+        Check if the config has an auto_monitor key and print a warning if not.
+
+        Args:
+            name(str): name of the device
+            config(dict): device config
         """
+        if "auto_monitor" not in config:
+            self.print_and_write(f"WARNING: Device {name} is configured without auto monitor.")
 
-    def pre_scan(self) -> None:
+    def connect_device(self, name: str, conf: dict) -> int:
         """
-        Specify actions to be executed right before a scan
+        Connect to the device
 
-        BEC calls pre_scan just before execution of the scan core.
-        It is convenient to execute time critical features of the detector,
-        e.g. arming it, but it is recommended to keep this function as short/fast as possible.
+        Args:
+            name(str): name of the device
+            conf(dict): device config
+
+        Returns:
+            int: 0 if all checks passed, 1 otherwise
         """
+        try:
+            conf_in = copy.deepcopy(conf)
+            conf_in["name"] = name
+            obj, _ = device_manager.construct_device_obj(conf_in, None)
+
+            device_manager.connect_device(obj, wait_for_all=True)
+            assert obj.connected is True
+            self.check_basic_ophyd_methods(obj)
+            obj.destroy()
+            if hasattr(obj, "component_names") and obj.component_names:
+                assert obj.connected is False
+                assert obj._destroyed is True
+            return 0
+
+        except Exception:
+            content = traceback.format_exc()
+            self.print_and_write(f"ERROR: {name} is not connectable: {content}")
+            return 1
 
-    def finished(self) -> None:
+    def check_basic_ophyd_methods(self, obj: ophyd.OphydObject) -> int:
         """
-        Specify actions to be executed during unstage
+        Check if the basic ophyd methods work
 
-        This may include checks if acquisition was succesful
+        Args:
+            obj(ophyd.OphydObject): device object
+
+        Returns:
 
-        Raises (optional):
-            DetectorTimeoutError: if detector cannot be stopped
         """
+        assert isinstance(obj, BECDevice)
+        assert isinstance(obj.name, str)
+        assert isinstance(obj.read(), dict)
+        assert isinstance(obj.read_configuration(), dict)
+        assert isinstance(obj.describe(), dict)
+        assert isinstance(obj.describe_configuration(), dict)
+        assert isinstance(obj.hints, dict)
 
-    def check_scan_id(self) -> None:
+    def validate_schema(self, name: str, conf: dict) -> None:
         """
-        Check if BEC is running on a new scan_id
+        Validate the device config against the BEC DB schema
+
+        Args:
+            name(str): name of the device
+            conf(dict): device config
         """
+        try:
+            validator = SciBecValidator()
+            db_config = self._translate_to_db_config(name, conf)
+            validator.validate_device(db_config)
+            return 0
+        except Exception as e:
+            self.print_and_write(f"ERROR: {name} is not valid: {e}")
+            return 1
 
-    def publish_file_location(self, done: bool = False, successful: bool = None) -> None:
+    @staticmethod
+    def _translate_to_db_config(name, config) -> dict:
         """
-        Publish the designated filepath from data backend to REDIS.
+        Translate the device config to a db config
 
-        Typically, the following two message types are published:
+        Args:
+            name(str): name of the device
+            config(dict): device config
 
-        - file_event: event for the filewriter
-        - public_file: event for any secondary service (e.g. radial integ code)
+        Returns:
+            dict: db config
         """
+        db_config = copy.deepcopy(config)
+        db_config["name"] = name
+        if "deviceConfig" in db_config and db_config["deviceConfig"] is None:
+            db_config["deviceConfig"] = {}
+        db_config.pop("deviceType", None)
+        return db_config
 
-    def wait_for_signals(
-        self,
-        signal_conditions: list,
-        timeout: float,
-        check_stopped: bool = False,
-        interval: float = 0.05,
-        all_signals: bool = False,
-    ) -> bool:
-        """Wait for signals to reach a certain condition
+    def run(self, connect: bool) -> None:
+        """
+        Run the tests
 
         Args:
-            signal_conditions (tuple): tuple of (get_current_state, condition) functions
-            timeout (float): timeout in seconds
-            interval (float): interval in seconds
-            all_signals (bool): True if all signals should be True, False if any signal should be True
-        Returns:
-            bool: True if all signals are in the desired state, False if timeout is reached
+            connect(bool): connect to the devices
         """
-        timer = 0
-        while True:
-            checks = [
-                get_current_state() == condition
-                for get_current_state, condition in signal_conditions
-            ]
-            if check_stopped is True and self.parent.stopped is True:
-                return False
-            if (all_signals and all(checks)) or (not all_signals and any(checks)):
-                return True
-            if timer > timeout:
-                return False
-            time.sleep(interval)
-            timer += interval
-
-
-class PSIDetectorBase(Device):
-    """
-    Abstract base class for SLS detectors
-
-    Class attributes:
-        custom_prepare_cls (object): class for custom prepare logic (BL specific)
-        Min_readout (float): minimum readout time for detector
-
-    Args:
-        prefix (str): EPICS PV prefix for component (optional)
-        name (str): name of the device, as will be reported via read()
-        kind (str): member of class 'ophydobj.Kind', defaults to Kind.normal
-                    omitted -> readout ignored for read 'ophydobj.read()'
-                    normal -> readout for read
-                    config -> config parameter for 'ophydobj.read_configuration()'
-                    hinted -> which attribute is readout for read
-        read_attrs (list): sequence of attribute names to read
-        configuration_attrs (list): sequence of attribute names via config_parameters
-        parent (object): instance of the parent device
-        device_manager (object): bec device manager
-        sim_mode (bool): simulation mode, if True, no device manager is required
-        **kwargs: keyword arguments
-
-        attributes: lazy_wait_for_connection : bool
-    """
-
-    custom_prepare_cls = CustomDetectorMixin
-
-    MIN_READOUT = 1e-3
-
-    # Specify which functions are revealed to the user in BEC client
-    USER_ACCESS = ["describe"]
-
-    def __init__(
-        self,
-        prefix="",
-        *,
-        name,
-        kind=None,
-        read_attrs=None,
-        configuration_attrs=None,
-        parent=None,
-        device_manager=None,
-        sim_mode=False,
-        **kwargs,
-    ):
-        super().__init__(
-            prefix=prefix,
-            name=name,
-            kind=kind,
-            read_attrs=read_attrs,
-            configuration_attrs=configuration_attrs,
-            parent=parent,
-            **kwargs,
-        )
-        if device_manager is None and not sim_mode:
-            raise DetectorInitError(
-                f"No device manager for device: {name}, and not started sim_mode: {sim_mode}. Add"
-                " DeviceManager to initialization or init with sim_mode=True"
-            )
-        # Init variables
-        self.sim_mode = sim_mode
-        self.stopped = False
-        self.name = name
-        self.service_cfg = None
-        self.scaninfo = None
-        self.filewriter = None
-        self.timeout = 5
-        self.wait_for_connection(all_signals=True)
-
-        # Init custom prepare class with BL specific logic
-        self.custom_prepare = self.custom_prepare_cls(parent=self, **kwargs)
-        if not sim_mode:
-            self._update_service_config()
-            self.device_manager = device_manager
+        failed_devices = []
+        for name, conf in self.config.items():
+            return_val = 0
+            self.print_and_write(f"Checking {name}...")
+            return_val += self.validate_schema(name, conf)
+            return_val += self.check_device_classes(name, conf)
+            if connect:
+                return_val += self.connect_device(name, conf)
+
+            if return_val == 0:
+                self.print_and_write("OK")
+            else:
+                self.print_and_write("FAILED")
+                failed_devices.append(name)
+
+        self.print_and_write("\n\n")
+        self.print_and_write("========================================")
+        # print summary
+        self.print_and_write("Summary:")
+        if len(failed_devices) == 0:
+            print("All devices passed the test.")
+            self.file.write("All devices passed the test.\n")
         else:
-            self.device_manager = bec_utils.DMMock()
-            base_path = kwargs["basepath"] if "basepath" in kwargs else "~/Data10/"
-            self.service_cfg = {"base_path": os.path.expanduser(base_path)}
-        self.connector = self.device_manager.connector
-        self._update_scaninfo()
-        self._update_filewriter()
-        self._init()
-
-    def _update_filewriter(self) -> None:
-        """Update filewriter with service config"""
-        self.filewriter = FileWriter(service_config=self.service_cfg, connector=self.connector)
-
-    def _update_scaninfo(self) -> None:
-        """Update scaninfo from BecScaninfoMixing
-        This depends on device manager and operation/sim_mode
-        """
-        self.scaninfo = BecScaninfoMixin(self.device_manager, self.sim_mode)
-        self.scaninfo.load_scan_metadata()
-
-    def _update_service_config(self) -> None:
-        """Update service config from BEC service config"""
-        from bec_lib.bec_service import SERVICE_CONFIG
-
-        self.service_cfg = SERVICE_CONFIG.config["service_config"]["file_writer"]
-
-    def _init(self) -> None:
-        """Initialize detector, filewriter and set default parameters"""
-        self.custom_prepare.initialize_default_parameter()
-        self.custom_prepare.initialize_detector()
-        self.custom_prepare.initialize_detector_backend()
-
-    def stage(self) -> list[object]:
-        """
-         Stage device in preparation for a scan
-
-        Internal Calls:
-        - _prep_backend           : prepare detector filewriter for measurement
-        - _prep_detector              : prepare detector for measurement
-
-        Returns:
-            list(object): list of objects that were staged
+            print(f"{len(failed_devices)} devices failed the test:")
+            self.file.write(f"{len(failed_devices)} devices failed the test:\n")
+            for device in failed_devices:
+                print(f"    {device}")
+                self.file.write(f"    {device}\n")
+            raise StaticDeviceAnalysisError(
+                f"The following devices failed the test in {self.config_file}: {failed_devices}. Check the report for more details."
+            )
 
+    def print_and_write(self, text: str) -> None:
         """
-        # Method idempotent, should rais ;obj;'RedudantStaging' if staged twice
-        if self._staged != Staged.no:
-            return super().stage()
-
-        # Reset flag for detector stopped
-        self.stopped = False
-        # Load metadata of the scan
-        self.scaninfo.load_scan_metadata()
-        # Prepare detector and file writer
-        self.custom_prepare.prepare_detector_backend()
-        self.custom_prepare.prepare_detector()
-        state = False
-        self.custom_prepare.publish_file_location(done=state)
-        # At the moment needed bc signal might not be reliable, BEC too fast.
-        # Consider removing this overhead in future!
-        time.sleep(0.05)
-        return super().stage()
-
-    def trigger(self) -> DeviceStatus:
-        """Trigger the detector, called from BEC."""
-        self.custom_prepare.on_trigger()
-        return super().trigger()
-
-    def unstage(self) -> list[object]:
-        """
-        Unstage device in preparation for a scan
-
-        Returns directly if self.stopped,
-        otherwise checks with self._finished
-        if data acquisition on device finished (an was successful)
-
-        Internal Calls:
-        - custom_prepare.check_scan_id          : check if scan_id changed or detector stopped
-        - custom_prepare.finished              : check if device finished acquisition (succesfully)
-        - custom_prepare.publish_file_location : publish file location to bec
+        Print and write to the output file
 
-        Returns:
-            list(object): list of objects that were unstaged
+        Args:
+            text(str): text to print and write
         """
-        self.custom_prepare.check_scan_id()
-        if self.stopped is True:
-            return super().unstage()
-        self.custom_prepare.finished()
-        state = True
-        self.custom_prepare.publish_file_location(done=state, successful=state)
-        self.stopped = False
-        return super().unstage()
-
-    def stop(self, *, success=False) -> None:
-        """
-        Stop the scan, with camera and file writer
-
-        Internal Calls:
-        - custom_prepare.stop_detector     : stop detector
-        - custom_prepare.stop_backend : stop detector filewriter
-        """
-        self.custom_prepare.stop_detector()
-        self.custom_prepare.stop_detector_backend()
-        super().stop(success=success)
-        self.stopped = True
+        print(text)
+        self.file.write(text + "\n")
+
+
+def launch() -> None:
+    """launch the test"""
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        description="Perform tests on an ophyd device config file.",
+    )
+
+    parser.add_argument("--config", help="path to the config file", required=True, type=str)
+    optional = parser.add_argument_group("optional arguments")
+    optional.add_argument(
+        "--output", default="./device_test_reports", help="path to the output directory"
+    )
+    optional.add_argument("--connect", action="store_true", help="connect to the devices")
+    parser.add_help = True
+
+    clargs = parser.parse_args()
+
+    if device_manager is None:
+        raise ImportError(
+            "bec-server is not installed. Please install it first with pip install bec-server."
+        )
+
+    if not os.path.exists(clargs.config):
+        raise FileNotFoundError(f"Config file {clargs.config} not found.")
+
+    if os.path.isdir(clargs.config):
+        files = []
+        for root, _, filenames in os.walk(clargs.config):
+            for filename in filenames:
+                if filename.endswith(".yaml") or filename.endswith(".yml"):
+                    files.append(os.path.join(root, filename))
+    else:
+        files = [clargs.config]
+
+    print(f"Running tests on the following files: {files}")
+
+    if not os.path.exists(clargs.output):
+        os.makedirs(clargs.output)
+
+    for file in files:
+        report_name = os.path.basename(file).split(".")[0]
+        with open(
+            os.path.join(clargs.output, f"report_{report_name}.txt"), "w", encoding="utf-8"
+        ) as report_file:
+            device_config_test = StaticDeviceTest(file, output_file=report_file)
+            device_config_test.run(clargs.connect)
+
+
+if __name__ == "__main__":  # pragma: no cover
+    import sys
+
+    sys.argv = ["", "--config", "../bec/bec_lib/bec_lib/configs/demo_config.yaml", "--connect"]
+    launch()
```

### Comparing `ophyd_devices-1.0.2/ophyd_devices/interfaces/protocols/bec_protocols.py` & `ophyd_devices-1.1.0/ophyd_devices/interfaces/protocols/bec_protocols.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/sim/sim.py` & `ophyd_devices-1.1.0/ophyd_devices/sim/sim.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/sim/sim_data.py` & `ophyd_devices-1.1.0/ophyd_devices/sim/sim_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/sim/sim_frameworks.py` & `ophyd_devices-1.1.0/ophyd_devices/sim/sim_frameworks.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/sim/sim_signals.py` & `ophyd_devices-1.1.0/ophyd_devices/sim/sim_signals.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/sim/sim_test_devices.py` & `ophyd_devices-1.1.0/ophyd_devices/sim/sim_test_devices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/sim/sim_xtreme.py` & `ophyd_devices-1.1.0/ophyd_devices/sim/sim_xtreme.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt` & `ophyd_devices-1.1.0/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt` & `ophyd_devices-1.1.0/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt` & `ophyd_devices-1.1.0/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt` & `ophyd_devices-1.1.0/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/tests/utils.py` & `ophyd_devices-1.1.0/ophyd_devices/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/utils/bec_device_base.py` & `ophyd_devices-1.1.0/ophyd_devices/utils/bec_device_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/utils/bec_scaninfo_mixin.py` & `ophyd_devices-1.1.0/ophyd_devices/utils/bec_scaninfo_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import getpass
 
 from bec_lib import bec_logger, messages
 from bec_lib.devicemanager import DeviceManagerBase
 from bec_lib.endpoints import MessageEndpoints
 
+from ophyd_devices.utils.bec_utils import DMMock
+
 logger = bec_logger.logger
 
 
 class BECInfoMsgMock:
     """Mock BECInfoMsg class
 
     This class is used for mocking BECInfoMsg for testing purposes
@@ -59,19 +61,17 @@
         device_manager (DeviceManagerBase): DeviceManagerBase object
         sim_mode (bool): Simulation mode flag
         bec_info_msg (dict): BECInfoMsg object
     Returns:
         BecScaninfoMixin: BecScaninfoMixin object
     """
 
-    def __init__(
-        self, device_manager: DeviceManagerBase = None, sim_mode: bool = False, bec_info_msg=None
-    ) -> None:
+    def __init__(self, device_manager: DeviceManagerBase = None, bec_info_msg=None) -> None:
+        self.sim_mode = bool(isinstance(device_manager, DMMock))
         self.device_manager = device_manager
-        self.sim_mode = sim_mode
         self.scan_msg = None
         self.scan_id = None
         if bec_info_msg is None:
             infomsgmock = BECInfoMsgMock()
             self.bec_info_msg = infomsgmock.get_bec_info_msg()
         else:
             self.bec_info_msg = bec_info_msg
```

### Comparing `ophyd_devices-1.0.2/ophyd_devices/utils/bec_utils.py` & `ophyd_devices-1.1.0/ophyd_devices/utils/bec_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/utils/controller.py` & `ophyd_devices-1.1.0/ophyd_devices/utils/controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/utils/dynamic_pseudo.py` & `ophyd_devices-1.1.0/ophyd_devices/utils/dynamic_pseudo.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/ophyd_devices/utils/socket.py` & `ophyd_devices-1.1.0/ophyd_devices/utils/socket.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/tests/test_controller.py` & `ophyd_devices-1.1.0/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/tests/test_dynamic_pseudo.py` & `ophyd_devices-1.1.0/tests/test_dynamic_pseudo.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/tests/test_ophyd_status_obj.py` & `ophyd_devices-1.1.0/tests/test_ophyd_status_obj.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/tests/test_simulation.py` & `ophyd_devices-1.1.0/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/tests/test_socket.py` & `ophyd_devices-1.1.0/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/.gitignore` & `ophyd_devices-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/LICENSE` & `ophyd_devices-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.2/pyproject.toml` & `ophyd_devices-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ophyd_devices"
-version = "1.0.2"
+version = "1.1.0"
 description = "Custom device implementations based on the ophyd hardware abstraction layer"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `ophyd_devices-1.0.2/PKG-INFO` & `ophyd_devices-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ophyd_devices
-Version: 1.0.2
+Version: 1.1.0
 Summary: Custom device implementations based on the ophyd hardware abstraction layer
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/ophyd_devices/issues
 Project-URL: Homepage, https://gitlab.psi.ch/bec/ophyd_devices
 Project-URL: documentation, https://bec.readthedocs.org
 Project-URL: changelog, https://gitlab.psi.ch/bec/ophyd_devices/blob/main/CHANGELOG.md
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

