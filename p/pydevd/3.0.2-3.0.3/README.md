# Comparing `tmp/pydevd-3.0.2.tar.gz` & `tmp/pydevd-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydevd-3.0.2.tar", last modified: Thu Feb  1 00:11:27 2024, max compression
+gzip compressed data, was "pydevd-3.0.3.tar", last modified: Thu Feb  1 01:05:39 2024, max compression
```

## Comparing `pydevd-3.0.2.tar` & `pydevd-3.0.3.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.825694 pydevd-3.0.2/
--rw-rw-rw-   0        0        0    11715 2024-02-01 00:09:32.000000 pydevd-3.0.2/LICENSE-EPL
--rw-rw-rw-   0        0        0      796 2024-02-01 00:09:32.000000 pydevd-3.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3516 2024-02-01 00:11:27.825694 pydevd-3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2406 2024-02-01 00:09:32.000000 pydevd-3.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.731941 pydevd-3.0.2/_pydev_bundle/
--rw-rw-rw-   0        0        0        0 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/__init__.py
--rw-rw-rw-   0        0        0     4842 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/_pydev_calltip_util.py
--rw-rw-rw-   0        0        0     8811 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/_pydev_completer.py
--rw-rw-rw-   0        0        0      497 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/_pydev_execfile.py
--rw-rw-rw-   0        0        0     1136 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/_pydev_filesystem_encoding.py
--rw-rw-rw-   0        0        0     4588 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/_pydev_getopt.py
--rw-rw-rw-   0        0        0    12723 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/_pydev_imports_tipper.py
--rw-rw-rw-   0        0        0    17555 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/_pydev_jy_imports_tipper.py
--rw-rw-rw-   0        0        0      579 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/_pydev_log.py
--rw-rw-rw-   0        0        0     4814 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/_pydev_saved_modules.py
--rw-rw-rw-   0        0        0     2312 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/_pydev_sys_patch.py
--rw-rw-rw-   0        0        0     1279 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/_pydev_tipper_common.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.731941 pydevd-3.0.2/_pydev_bundle/fsnotify/
--rw-rw-rw-   0        0        0    13081 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/fsnotify/__init__.py
--rw-rw-rw-   0        0        0    24408 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/pydev_console_utils.py
--rw-rw-rw-   0        0        0     1362 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/pydev_import_hook.py
--rw-rw-rw-   0        0        0      417 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/pydev_imports.py
--rw-rw-rw-   0        0        0     3918 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/pydev_ipython_console.py
--rw-rw-rw-   0        0        0    21870 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/pydev_ipython_console_011.py
--rw-rw-rw-   0        0        0      719 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/pydev_is_thread_alive.py
--rw-rw-rw-   0        0        0     2137 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/pydev_localhost.py
--rw-rw-rw-   0        0        0     9450 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/pydev_log.py
--rw-rw-rw-   0        0        0    43572 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/pydev_monkey.py
--rw-rw-rw-   0        0        0     7522 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/pydev_monkey_qt.py
--rw-rw-rw-   0        0        0      906 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/pydev_override.py
--rw-rw-rw-   0        0        0     6459 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/pydev_umd.py
--rw-rw-rw-   0        0        0      526 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_bundle/pydev_versioncheck.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.731941 pydevd-3.0.2/_pydev_runfiles/
--rw-rw-rw-   0        0        0        0 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_runfiles/__init__.py
--rw-rw-rw-   0        0        0    32407 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_runfiles/pydev_runfiles.py
--rw-rw-rw-   0        0        0     3575 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_runfiles/pydev_runfiles_coverage.py
--rw-rw-rw-   0        0        0     7756 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_runfiles/pydev_runfiles_nose.py
--rw-rw-rw-   0        0        0     9739 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_runfiles/pydev_runfiles_parallel.py
--rw-rw-rw-   0        0        0     7936 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_runfiles/pydev_runfiles_parallel_client.py
--rw-rw-rw-   0        0        0    10151 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_runfiles/pydev_runfiles_pytest2.py
--rw-rw-rw-   0        0        0     6835 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_runfiles/pydev_runfiles_unittest.py
--rw-rw-rw-   0        0        0    10852 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydev_runfiles/pydev_runfiles_xml_rpc.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.763197 pydevd-3.0.2/_pydevd_bundle/
--rw-rw-rw-   0        0        0        0 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.763197 pydevd-3.0.2/_pydevd_bundle/_debug_adapter/
--rw-rw-rw-   0        0        0        0 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/_debug_adapter/__init__.py
--rw-rw-rw-   0        0        0    23677 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/_debug_adapter/__main__pydevd_gen_debug_adapter_protocol.py
--rw-rw-rw-   0        0        0     4145 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/_debug_adapter/pydevd_base_schema.py
--rw-rw-rw-   0        0        0   783010 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/_debug_adapter/pydevd_schema.py
--rw-rw-rw-   0        0        0     1301 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/_debug_adapter/pydevd_schema_log.py
--rw-rw-rw-   0        0        0    19568 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevconsole_code.py
--rw-rw-rw-   0        0        0     1526 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_additional_thread_info.py
--rw-rw-rw-   0        0        0    10703 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_additional_thread_info_regular.py
--rw-rw-rw-   0        0        0    52224 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_api.py
--rw-rw-rw-   0        0        0     6194 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_breakpoints.py
--rw-rw-rw-   0        0        0    29925 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_bytecode_utils.py
--rw-rw-rw-   0        0        0     3913 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_bytecode_utils_py311.py
--rw-rw-rw-   0        0        0    18233 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_code_to_source.py
--rw-rw-rw-   0        0        0    38479 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_collect_bytecode_info.py
--rw-rw-rw-   0        0        0    79256 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_comm.py
--rw-rw-rw-   0        0        0     6292 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_comm_constants.py
--rw-rw-rw-   0        0        0     6311 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_command_line_handling.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.763197 pydevd-3.0.2/_pydevd_bundle/pydevd_concurrency_analyser/
--rw-rw-rw-   0        0        0        0 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_concurrency_analyser/__init__.py
--rw-rw-rw-   0        0        0    17110 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_concurrency_analyser/pydevd_concurrency_logger.py
--rw-rw-rw-   0        0        0     2122 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_concurrency_analyser/pydevd_thread_wrappers.py
--rw-rw-rw-   0        0        0    10449 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_console.py
--rw-rw-rw-   0        0        0    28919 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_constants.py
--rw-rw-rw-   0        0        0     4515 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_custom_frames.py
--rw-rw-rw-   0        0        0  2670586 2024-02-01 00:10:17.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_cython.c
--rw-rw-rw-   0        0        0    98365 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_cython.pyx
--rw-rw-rw-   0        0        0     1913 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_cython_wrapper.py
--rw-rw-rw-   0        0        0     8474 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_daemon_thread.py
--rw-rw-rw-   0        0        0     2382 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_defaults.py
--rw-rw-rw-   0        0        0     3681 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_dont_trace.py
--rw-rw-rw-   0        0        0     6492 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_dont_trace_files.py
--rw-rw-rw-   0        0        0      163 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_exec2.py
--rw-rw-rw-   0        0        0     4015 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_extension_api.py
--rw-rw-rw-   0        0        0     2436 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_extension_utils.py
--rw-rw-rw-   0        0        0    13217 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_filtering.py
--rw-rw-rw-   0        0        0    64613 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_frame.py
--rw-rw-rw-   0        0        0    13613 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_frame_utils.py
--rw-rw-rw-   0        0        0     3970 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_gevent_integration.py
--rw-rw-rw-   0        0        0     1906 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_import_class.py
--rw-rw-rw-   0        0        0     8375 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_io.py
--rw-rw-rw-   0        0        0     6403 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_json_debug_options.py
--rw-rw-rw-   0        0        0     4734 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_net_command.py
--rw-rw-rw-   0        0        0    22903 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_net_command_factory_json.py
--rw-rw-rw-   0        0        0    23809 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_net_command_factory_xml.py
--rw-rw-rw-   0        0        0     7382 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_plugin_utils.py
--rw-rw-rw-   0        0        0    35944 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_process_net_command.py
--rw-rw-rw-   0        0        0    58398 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_process_net_command_json.py
--rw-rw-rw-   0        0        0    10013 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_referrers.py
--rw-rw-rw-   0        0        0    16206 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_reload.py
--rw-rw-rw-   0        0        0    30454 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_resolver.py
--rw-rw-rw-   0        0        0    13874 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_runpy.py
--rw-rw-rw-   0        0        0    14953 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_safe_repr.py
--rw-rw-rw-   0        0        0     3578 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_save_locals.py
--rw-rw-rw-   0        0        0     7084 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_signature.py
--rw-rw-rw-   0        0        0     6581 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_source_mapping.py
--rw-rw-rw-   0        0        0    17325 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_stackless.py
--rw-rw-rw-   0        0        0    21417 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_suspended_frames.py
--rw-rw-rw-   0        0        0     3965 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_thread_lifecycle.py
--rw-rw-rw-   0        0        0     8655 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_timeout.py
--rw-rw-rw-   0        0        0     3773 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_trace_dispatch.py
--rw-rw-rw-   0        0        0    22884 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_trace_dispatch_regular.py
--rw-rw-rw-   0        0        0     3371 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_traceproperty.py
--rw-rw-rw-   0        0        0    18360 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_utils.py
--rw-rw-rw-   0        0        0    31982 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_vars.py
--rw-rw-rw-   0        0        0     1619 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_vm_type.py
--rw-rw-rw-   0        0        0    15909 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_bundle/pydevd_xml.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.763197 pydevd-3.0.2/_pydevd_frame_eval/
--rw-rw-rw-   0        0        0        0 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_frame_eval/__init__.py
--rw-rw-rw-   0        0        0     1386 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_frame_eval/pydevd_frame_eval_cython_wrapper.py
--rw-rw-rw-   0        0        0     2370 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_frame_eval/pydevd_frame_eval_main.py
--rw-rw-rw-   0        0        0  1208349 2024-02-01 00:11:11.000000 pydevd-3.0.2/_pydevd_frame_eval/pydevd_frame_evaluator.c
--rw-rw-rw-   0        0        0     4341 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_frame_eval/pydevd_frame_tracing.py
--rw-rw-rw-   0        0        0    13910 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_frame_eval/pydevd_modify_bytecode.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.763197 pydevd-3.0.2/_pydevd_frame_eval/vendored/
--rw-rw-rw-   0        0        0        0 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_frame_eval/vendored/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.778822 pydevd-3.0.2/_pydevd_frame_eval/vendored/bytecode/
--rw-rw-rw-   0        0        0     4282 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_frame_eval/vendored/bytecode/__init__.py
--rw-rw-rw-   0        0        0     7353 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_frame_eval/vendored/bytecode/bytecode.py
--rw-rw-rw-   0        0        0    15854 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_frame_eval/vendored/bytecode/cfg.py
--rw-rw-rw-   0        0        0    22972 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_frame_eval/vendored/bytecode/concrete.py
--rw-rw-rw-   0        0        0     6201 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_frame_eval/vendored/bytecode/flags.py
--rw-rw-rw-   0        0        0    12117 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_frame_eval/vendored/bytecode/instr.py
--rw-rw-rw-   0        0        0    16231 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_frame_eval/vendored/bytecode/peephole_opt.py
--rw-rw-rw-   0        0        0     1850 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_frame_eval/vendored/pydevd_fix_code.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.778822 pydevd-3.0.2/_pydevd_sys_monitoring/
--rw-rw-rw-   0        0        0    70236 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_sys_monitoring/_pydevd_sys_monitoring.py
--rw-rw-rw-   0        0        0      572 2024-02-01 00:09:32.000000 pydevd-3.0.2/_pydevd_sys_monitoring/pydevd_sys_monitoring.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.778822 pydevd-3.0.2/build_tools/
--rw-rw-rw-   0        0        0     6871 2024-02-01 00:09:32.000000 pydevd-3.0.2/build_tools/build.py
--rw-rw-rw-   0        0        0     2027 2024-02-01 00:09:32.000000 pydevd-3.0.2/build_tools/build_binaries_osx.py
--rw-rw-rw-   0        0        0     2787 2024-02-01 00:09:32.000000 pydevd-3.0.2/build_tools/build_binaries_windows.py
--rw-rw-rw-   0        0        0     3615 2024-02-01 00:09:32.000000 pydevd-3.0.2/build_tools/check_no_git_modifications.py
--rw-rw-rw-   0        0        0     8167 2024-02-01 00:09:32.000000 pydevd-3.0.2/build_tools/generate_code.py
--rw-rw-rw-   0        0        0     6321 2024-02-01 00:09:32.000000 pydevd-3.0.2/build_tools/names_to_rename.py
--rw-rw-rw-   0        0        0     4254 2024-02-01 00:09:32.000000 pydevd-3.0.2/build_tools/rename_pep8.py
--rw-rw-rw-   0        0        0      712 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_app_engine_debug_startup.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.778822 pydevd-3.0.2/pydev_ipython/
--rw-rw-rw-   0        0        0        0 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_ipython/__init__.py
--rw-rw-rw-   0        0        0    20146 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_ipython/inputhook.py
--rw-rw-rw-   0        0        0     5829 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_ipython/inputhookglut.py
--rw-rw-rw-   0        0        0     1143 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_ipython/inputhookgtk.py
--rw-rw-rw-   0        0        0     1139 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_ipython/inputhookgtk3.py
--rw-rw-rw-   0        0        0     3347 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_ipython/inputhookpyglet.py
--rw-rw-rw-   0        0        0     7483 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_ipython/inputhookqt4.py
--rw-rw-rw-   0        0        0     7528 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_ipython/inputhookqt5.py
--rw-rw-rw-   0        0        0      771 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_ipython/inputhooktk.py
--rw-rw-rw-   0        0        0     6686 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_ipython/inputhookwx.py
--rw-rw-rw-   0        0        0     5527 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_ipython/matplotlibtools.py
--rw-rw-rw-   0        0        0      808 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_ipython/qt.py
--rw-rw-rw-   0        0        0     3738 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_ipython/qt_for_kernel.py
--rw-rw-rw-   0        0        0     8741 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_ipython/qt_loaders.py
--rw-rw-rw-   0        0        0     1548 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_ipython/version.py
--rw-rw-rw-   0        0        0     4862 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydev_run_in_console.py
--rw-rw-rw-   0        0        0    21697 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevconsole.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.794443 pydevd-3.0.2/pydevd.egg-info/
--rw-rw-rw-   0        0        0     3516 2024-02-01 00:11:27.000000 pydevd-3.0.2/pydevd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9745 2024-02-01 00:11:27.000000 pydevd-3.0.2/pydevd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-01 00:11:27.000000 pydevd-3.0.2/pydevd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-02-01 00:11:27.000000 pydevd-3.0.2/pydevd.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-02-01 00:11:27.000000 pydevd-3.0.2/pydevd.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      266 2024-02-01 00:11:27.000000 pydevd-3.0.2/pydevd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   157645 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.794443 pydevd-3.0.2/pydevd_attach_to_process/
--rw-rw-rw-   0        0        0      987 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/README.txt
--rw-rw-rw-   0        0        0      711 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/_always_live_program.py
--rw-rw-rw-   0        0        0      137 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/_check.py
--rw-rw-rw-   0        0        0      306 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/_test_attach_to_process.py
--rw-rw-rw-   0        0        0     2597 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/_test_attach_to_process_linux.py
--rw-rw-rw-   0        0        0    22932 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/add_code_to_python_process.py
--rw-rw-rw-   0        0        0    36352 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/attach_amd64.dll
--rw-rw-rw-   0        0        0    31424 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/attach_linux_amd64.so
--rw-rw-rw-   0        0        0    21388 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/attach_linux_x86.so
--rw-rw-rw-   0        0        0     2558 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/attach_pydevd.py
--rw-rw-rw-   0        0        0     8061 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/attach_script.py
--rw-rw-rw-   0        0        0    31232 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/attach_x86.dll
--rw-rw-rw-   0        0        0    55296 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/attach_x86_64.dylib
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.794443 pydevd-3.0.2/pydevd_attach_to_process/common/
--rw-rw-rw-   0        0        0     8591 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/common/py_custom_pyeval_settrace.hpp
--rw-rw-rw-   0        0        0     4174 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/common/py_custom_pyeval_settrace_310.hpp
--rw-rw-rw-   0        0        0     4388 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/common/py_custom_pyeval_settrace_311.hpp
--rw-rw-rw-   0        0        0     1931 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/common/py_custom_pyeval_settrace_common.hpp
--rw-rw-rw-   0        0        0     8016 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/common/py_settrace.hpp
--rw-rw-rw-   0        0        0     3894 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/common/py_utils.hpp
--rw-rw-rw-   0        0        0     2706 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/common/py_version.hpp
--rw-rw-rw-   0        0        0    22335 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/common/python.h
--rw-rw-rw-   0        0        0     1537 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/common/ref_utils.hpp
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.794443 pydevd-3.0.2/pydevd_attach_to_process/linux_and_mac/
--rw-rw-rw-   0        0        0     3814 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/linux_and_mac/attach.cpp
--rw-rw-rw-   0        0        0      286 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/linux_and_mac/compile_linux.sh
--rw-rw-rw-   0        0        0      236 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/linux_and_mac/compile_mac.sh
--rw-rw-rw-   0        0        0     1745 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/linux_and_mac/lldb_prepare.py
--rw-rw-rw-   0        0        0    16896 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/run_code_on_dllmain_amd64.dll
--rw-rw-rw-   0        0        0    14336 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/run_code_on_dllmain_x86.dll
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.810073 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/
--rw-rw-rw-   0        0        0     8180 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/__init__.py
--rw-rw-rw-   0        0        0   172990 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/breakpoint.py
--rw-rw-rw-   0        0        0     5412 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/compat.py
--rw-rw-rw-   0        0        0    67247 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/crash.py
--rw-rw-rw-   0        0        0    60252 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/debug.py
--rw-rw-rw-   0        0        0    25131 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/disasm.py
--rw-rw-rw-   0        0        0    69110 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/event.py
--rw-rw-rw-   0        0        0    85797 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/interactive.py
--rw-rw-rw-   0        0        0    72631 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/module.py
--rw-rw-rw-   0        0        0   188656 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/process.py
--rw-rw-rw-   0        0        0    22264 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/registry.py
--rw-rw-rw-   0        0        0    24463 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/search.py
--rw-rw-rw-   0        0        0    35990 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/sql.py
--rw-rw-rw-   0        0        0    47181 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/system.py
--rw-rw-rw-   0        0        0    64570 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/textio.py
--rw-rw-rw-   0        0        0    77605 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/thread.py
--rw-rw-rw-   0        0        0    37201 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/util.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.810073 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/
--rw-rw-rw-   0        0        0     2917 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/__init__.py
--rw-rw-rw-   0        0        0   124018 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/advapi32.py
--rw-rw-rw-   0        0        0    25899 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/context_amd64.py
--rw-rw-rw-   0        0        0    16557 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/context_i386.py
--rw-rw-rw-   0        0        0    47982 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/dbghelp.py
--rw-rw-rw-   0        0        0    23517 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/defines.py
--rw-rw-rw-   0        0        0    17336 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/gdi32.py
--rw-rw-rw-   0        0        0   169534 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/kernel32.py
--rw-rw-rw-   0        0        0    23386 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/ntdll.py
--rw-rw-rw-   0        0        0   162665 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/peb_teb.py
--rw-rw-rw-   0        0        0    14149 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/psapi.py
--rw-rw-rw-   0        0        0    14389 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/shell32.py
--rw-rw-rw-   0        0        0    26563 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/shlwapi.py
--rw-rw-rw-   0        0        0    58904 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/user32.py
--rw-rw-rw-   0        0        0    37851 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/version.py
--rw-rw-rw-   0        0        0    11501 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/wtsapi32.py
--rw-rw-rw-   0        0        0    25068 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/winappdbg/window.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.825694 pydevd-3.0.2/pydevd_attach_to_process/windows/
--rw-rw-rw-   0        0        0    28081 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/windows/attach.cpp
--rw-rw-rw-   0        0        0     1902 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/windows/attach.h
--rwxrwxrwx   0        0        0     2138 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/windows/compile_windows.bat
--rw-rw-rw-   0        0        0     4925 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/windows/inject_dll.cpp
--rw-rw-rw-   0        0        0     2555 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/windows/py_win_helpers.hpp
--rw-rw-rw-   0        0        0     3470 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/windows/run_code_in_memory.hpp
--rw-rw-rw-   0        0        0     2594 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/windows/run_code_on_dllmain.cpp
--rw-rw-rw-   0        0        0     1021 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/windows/stdafx.cpp
--rw-rw-rw-   0        0        0     1198 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/windows/stdafx.h
--rw-rw-rw-   0        0        0     1035 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_attach_to_process/windows/targetver.h
--rw-rw-rw-   0        0        0    37282 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_file_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.825694 pydevd-3.0.2/pydevd_plugins/
--rw-rw-rw-   0        0        0       68 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_plugins/__init__.py
--rw-rw-rw-   0        0        0    22636 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_plugins/django_debug.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.825694 pydevd-3.0.2/pydevd_plugins/extensions/
--rw-rw-rw-   0        0        0       68 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_plugins/extensions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-01 00:11:27.825694 pydevd-3.0.2/pydevd_plugins/extensions/types/
--rw-rw-rw-   0        0        0       68 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_plugins/extensions/types/__init__.py
--rw-rw-rw-   0        0        0      665 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_plugins/extensions/types/pydevd_helpers.py
--rw-rw-rw-   0        0        0     3338 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_plugins/extensions/types/pydevd_plugin_numpy_types.py
--rw-rw-rw-   0        0        0     6767 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_plugins/extensions/types/pydevd_plugin_pandas_types.py
--rw-rw-rw-   0        0        0      554 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_plugins/extensions/types/pydevd_plugins_django_form_str.py
--rw-rw-rw-   0        0        0    19294 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_plugins/jinja2_debug.py
--rw-rw-rw-   0        0        0     6393 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_plugins/pydevd_line_validation.py
--rw-rw-rw-   0        0        0    16022 2024-02-01 00:09:32.000000 pydevd-3.0.2/pydevd_tracing.py
--rw-rw-rw-   0        0        0      279 2024-02-01 00:09:32.000000 pydevd-3.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-01 00:11:27.825694 pydevd-3.0.2/setup.cfg
--rw-rw-rw-   0        0        0     7228 2024-02-01 00:09:32.000000 pydevd-3.0.2/setup.py
--rw-rw-rw-   0        0        0    11058 2024-02-01 00:09:32.000000 pydevd-3.0.2/setup_pydevd_cython.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.716673 pydevd-3.0.3/
+-rw-rw-rw-   0        0        0    11715 2024-02-01 01:04:41.000000 pydevd-3.0.3/LICENSE-EPL
+-rw-rw-rw-   0        0        0      796 2024-02-01 01:04:41.000000 pydevd-3.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3516 2024-02-01 01:05:39.716673 pydevd-3.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2406 2024-02-01 01:04:41.000000 pydevd-3.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.607297 pydevd-3.0.3/_pydev_bundle/
+-rw-rw-rw-   0        0        0        0 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/__init__.py
+-rw-rw-rw-   0        0        0     4842 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/_pydev_calltip_util.py
+-rw-rw-rw-   0        0        0     8811 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/_pydev_completer.py
+-rw-rw-rw-   0        0        0      497 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/_pydev_execfile.py
+-rw-rw-rw-   0        0        0     1136 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/_pydev_filesystem_encoding.py
+-rw-rw-rw-   0        0        0     4588 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/_pydev_getopt.py
+-rw-rw-rw-   0        0        0    12723 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/_pydev_imports_tipper.py
+-rw-rw-rw-   0        0        0    17555 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/_pydev_jy_imports_tipper.py
+-rw-rw-rw-   0        0        0      579 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/_pydev_log.py
+-rw-rw-rw-   0        0        0     4814 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/_pydev_saved_modules.py
+-rw-rw-rw-   0        0        0     2312 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/_pydev_sys_patch.py
+-rw-rw-rw-   0        0        0     1279 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/_pydev_tipper_common.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.607297 pydevd-3.0.3/_pydev_bundle/fsnotify/
+-rw-rw-rw-   0        0        0    13081 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/fsnotify/__init__.py
+-rw-rw-rw-   0        0        0    24408 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/pydev_console_utils.py
+-rw-rw-rw-   0        0        0     1362 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/pydev_import_hook.py
+-rw-rw-rw-   0        0        0      417 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/pydev_imports.py
+-rw-rw-rw-   0        0        0     3918 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/pydev_ipython_console.py
+-rw-rw-rw-   0        0        0    21870 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/pydev_ipython_console_011.py
+-rw-rw-rw-   0        0        0      719 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/pydev_is_thread_alive.py
+-rw-rw-rw-   0        0        0     2137 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/pydev_localhost.py
+-rw-rw-rw-   0        0        0     9450 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/pydev_log.py
+-rw-rw-rw-   0        0        0    43572 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/pydev_monkey.py
+-rw-rw-rw-   0        0        0     7522 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/pydev_monkey_qt.py
+-rw-rw-rw-   0        0        0      906 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/pydev_override.py
+-rw-rw-rw-   0        0        0     6459 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/pydev_umd.py
+-rw-rw-rw-   0        0        0      526 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_bundle/pydev_versioncheck.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.607297 pydevd-3.0.3/_pydev_runfiles/
+-rw-rw-rw-   0        0        0        0 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_runfiles/__init__.py
+-rw-rw-rw-   0        0        0    32407 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_runfiles/pydev_runfiles.py
+-rw-rw-rw-   0        0        0     3575 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_runfiles/pydev_runfiles_coverage.py
+-rw-rw-rw-   0        0        0     7756 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_runfiles/pydev_runfiles_nose.py
+-rw-rw-rw-   0        0        0     9739 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_runfiles/pydev_runfiles_parallel.py
+-rw-rw-rw-   0        0        0     7936 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_runfiles/pydev_runfiles_parallel_client.py
+-rw-rw-rw-   0        0        0    10151 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_runfiles/pydev_runfiles_pytest2.py
+-rw-rw-rw-   0        0        0     6835 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_runfiles/pydev_runfiles_unittest.py
+-rw-rw-rw-   0        0        0    10852 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydev_runfiles/pydev_runfiles_xml_rpc.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.638551 pydevd-3.0.3/_pydevd_bundle/
+-rw-rw-rw-   0        0        0        0 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.638551 pydevd-3.0.3/_pydevd_bundle/_debug_adapter/
+-rw-rw-rw-   0        0        0        0 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/_debug_adapter/__init__.py
+-rw-rw-rw-   0        0        0    23677 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/_debug_adapter/__main__pydevd_gen_debug_adapter_protocol.py
+-rw-rw-rw-   0        0        0     4145 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/_debug_adapter/pydevd_base_schema.py
+-rw-rw-rw-   0        0        0   783010 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/_debug_adapter/pydevd_schema.py
+-rw-rw-rw-   0        0        0     1301 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/_debug_adapter/pydevd_schema_log.py
+-rw-rw-rw-   0        0        0    19568 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevconsole_code.py
+-rw-rw-rw-   0        0        0     1526 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_additional_thread_info.py
+-rw-rw-rw-   0        0        0    10703 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_additional_thread_info_regular.py
+-rw-rw-rw-   0        0        0    52224 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_api.py
+-rw-rw-rw-   0        0        0     6194 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_breakpoints.py
+-rw-rw-rw-   0        0        0    29925 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_bytecode_utils.py
+-rw-rw-rw-   0        0        0     3913 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_bytecode_utils_py311.py
+-rw-rw-rw-   0        0        0    18233 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_code_to_source.py
+-rw-rw-rw-   0        0        0    38479 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_collect_bytecode_info.py
+-rw-rw-rw-   0        0        0    79256 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_comm.py
+-rw-rw-rw-   0        0        0     6292 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_comm_constants.py
+-rw-rw-rw-   0        0        0     6311 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_command_line_handling.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.638551 pydevd-3.0.3/_pydevd_bundle/pydevd_concurrency_analyser/
+-rw-rw-rw-   0        0        0        0 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_concurrency_analyser/__init__.py
+-rw-rw-rw-   0        0        0    17110 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_concurrency_analyser/pydevd_concurrency_logger.py
+-rw-rw-rw-   0        0        0     2122 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_concurrency_analyser/pydevd_thread_wrappers.py
+-rw-rw-rw-   0        0        0    10449 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_console.py
+-rw-rw-rw-   0        0        0    28919 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_constants.py
+-rw-rw-rw-   0        0        0     4515 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_custom_frames.py
+-rw-rw-rw-   0        0        0  2670586 2024-02-01 01:05:02.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_cython.c
+-rw-rw-rw-   0        0        0    98365 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_cython.pyx
+-rw-rw-rw-   0        0        0     1913 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_cython_wrapper.py
+-rw-rw-rw-   0        0        0     8474 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_daemon_thread.py
+-rw-rw-rw-   0        0        0     2382 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_defaults.py
+-rw-rw-rw-   0        0        0     3681 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_dont_trace.py
+-rw-rw-rw-   0        0        0     6492 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_dont_trace_files.py
+-rw-rw-rw-   0        0        0      163 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_exec2.py
+-rw-rw-rw-   0        0        0     4015 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_extension_api.py
+-rw-rw-rw-   0        0        0     2436 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_extension_utils.py
+-rw-rw-rw-   0        0        0    13217 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_filtering.py
+-rw-rw-rw-   0        0        0    64613 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_frame.py
+-rw-rw-rw-   0        0        0    13613 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_frame_utils.py
+-rw-rw-rw-   0        0        0     3970 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_gevent_integration.py
+-rw-rw-rw-   0        0        0     1906 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_import_class.py
+-rw-rw-rw-   0        0        0     8375 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_io.py
+-rw-rw-rw-   0        0        0     6403 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_json_debug_options.py
+-rw-rw-rw-   0        0        0     4734 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_net_command.py
+-rw-rw-rw-   0        0        0    22903 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_net_command_factory_json.py
+-rw-rw-rw-   0        0        0    23809 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_net_command_factory_xml.py
+-rw-rw-rw-   0        0        0     7382 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_plugin_utils.py
+-rw-rw-rw-   0        0        0    35944 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_process_net_command.py
+-rw-rw-rw-   0        0        0    58398 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_process_net_command_json.py
+-rw-rw-rw-   0        0        0    10013 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_referrers.py
+-rw-rw-rw-   0        0        0    16206 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_reload.py
+-rw-rw-rw-   0        0        0    30454 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_resolver.py
+-rw-rw-rw-   0        0        0    13874 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_runpy.py
+-rw-rw-rw-   0        0        0    14953 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_safe_repr.py
+-rw-rw-rw-   0        0        0     3578 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_save_locals.py
+-rw-rw-rw-   0        0        0     7084 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_signature.py
+-rw-rw-rw-   0        0        0     6581 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_source_mapping.py
+-rw-rw-rw-   0        0        0    17325 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_stackless.py
+-rw-rw-rw-   0        0        0    21417 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_suspended_frames.py
+-rw-rw-rw-   0        0        0     3965 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_thread_lifecycle.py
+-rw-rw-rw-   0        0        0     8655 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_timeout.py
+-rw-rw-rw-   0        0        0     3773 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_trace_dispatch.py
+-rw-rw-rw-   0        0        0    22884 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_trace_dispatch_regular.py
+-rw-rw-rw-   0        0        0     3371 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_traceproperty.py
+-rw-rw-rw-   0        0        0    18360 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_utils.py
+-rw-rw-rw-   0        0        0    31982 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_vars.py
+-rw-rw-rw-   0        0        0     1619 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_vm_type.py
+-rw-rw-rw-   0        0        0    15909 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_bundle/pydevd_xml.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.654178 pydevd-3.0.3/_pydevd_frame_eval/
+-rw-rw-rw-   0        0        0        0 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_frame_eval/__init__.py
+-rw-rw-rw-   0        0        0     1386 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_frame_eval/pydevd_frame_eval_cython_wrapper.py
+-rw-rw-rw-   0        0        0     2370 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_frame_eval/pydevd_frame_eval_main.py
+-rw-rw-rw-   0        0        0  1208349 2024-02-01 01:05:34.000000 pydevd-3.0.3/_pydevd_frame_eval/pydevd_frame_evaluator.c
+-rw-rw-rw-   0        0        0     4341 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_frame_eval/pydevd_frame_tracing.py
+-rw-rw-rw-   0        0        0    13910 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_frame_eval/pydevd_modify_bytecode.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.654178 pydevd-3.0.3/_pydevd_frame_eval/vendored/
+-rw-rw-rw-   0        0        0        0 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_frame_eval/vendored/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.654178 pydevd-3.0.3/_pydevd_frame_eval/vendored/bytecode/
+-rw-rw-rw-   0        0        0     4282 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_frame_eval/vendored/bytecode/__init__.py
+-rw-rw-rw-   0        0        0     7353 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_frame_eval/vendored/bytecode/bytecode.py
+-rw-rw-rw-   0        0        0    15854 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_frame_eval/vendored/bytecode/cfg.py
+-rw-rw-rw-   0        0        0    22972 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_frame_eval/vendored/bytecode/concrete.py
+-rw-rw-rw-   0        0        0     6201 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_frame_eval/vendored/bytecode/flags.py
+-rw-rw-rw-   0        0        0    12117 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_frame_eval/vendored/bytecode/instr.py
+-rw-rw-rw-   0        0        0    16231 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_frame_eval/vendored/bytecode/peephole_opt.py
+-rw-rw-rw-   0        0        0     1850 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_frame_eval/vendored/pydevd_fix_code.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.654178 pydevd-3.0.3/_pydevd_sys_monitoring/
+-rw-rw-rw-   0        0        0    70236 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_sys_monitoring/_pydevd_sys_monitoring.py
+-rw-rw-rw-   0        0        0      572 2024-02-01 01:04:41.000000 pydevd-3.0.3/_pydevd_sys_monitoring/pydevd_sys_monitoring.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.654178 pydevd-3.0.3/build_tools/
+-rw-rw-rw-   0        0        0     6830 2024-02-01 01:04:41.000000 pydevd-3.0.3/build_tools/build.py
+-rw-rw-rw-   0        0        0     2027 2024-02-01 01:04:41.000000 pydevd-3.0.3/build_tools/build_binaries_osx.py
+-rw-rw-rw-   0        0        0     2787 2024-02-01 01:04:41.000000 pydevd-3.0.3/build_tools/build_binaries_windows.py
+-rw-rw-rw-   0        0        0     3615 2024-02-01 01:04:41.000000 pydevd-3.0.3/build_tools/check_no_git_modifications.py
+-rw-rw-rw-   0        0        0     8167 2024-02-01 01:04:41.000000 pydevd-3.0.3/build_tools/generate_code.py
+-rw-rw-rw-   0        0        0     6321 2024-02-01 01:04:41.000000 pydevd-3.0.3/build_tools/names_to_rename.py
+-rw-rw-rw-   0        0        0     4254 2024-02-01 01:04:41.000000 pydevd-3.0.3/build_tools/rename_pep8.py
+-rw-rw-rw-   0        0        0      712 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_app_engine_debug_startup.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.669799 pydevd-3.0.3/pydev_ipython/
+-rw-rw-rw-   0        0        0        0 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_ipython/__init__.py
+-rw-rw-rw-   0        0        0    20146 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_ipython/inputhook.py
+-rw-rw-rw-   0        0        0     5829 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_ipython/inputhookglut.py
+-rw-rw-rw-   0        0        0     1143 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_ipython/inputhookgtk.py
+-rw-rw-rw-   0        0        0     1139 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_ipython/inputhookgtk3.py
+-rw-rw-rw-   0        0        0     3347 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_ipython/inputhookpyglet.py
+-rw-rw-rw-   0        0        0     7483 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_ipython/inputhookqt4.py
+-rw-rw-rw-   0        0        0     7528 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_ipython/inputhookqt5.py
+-rw-rw-rw-   0        0        0      771 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_ipython/inputhooktk.py
+-rw-rw-rw-   0        0        0     6686 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_ipython/inputhookwx.py
+-rw-rw-rw-   0        0        0     5527 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_ipython/matplotlibtools.py
+-rw-rw-rw-   0        0        0      808 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_ipython/qt.py
+-rw-rw-rw-   0        0        0     3738 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_ipython/qt_for_kernel.py
+-rw-rw-rw-   0        0        0     8741 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_ipython/qt_loaders.py
+-rw-rw-rw-   0        0        0     1548 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_ipython/version.py
+-rw-rw-rw-   0        0        0     4862 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydev_run_in_console.py
+-rw-rw-rw-   0        0        0    21697 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevconsole.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.669799 pydevd-3.0.3/pydevd.egg-info/
+-rw-rw-rw-   0        0        0     3516 2024-02-01 01:05:39.000000 pydevd-3.0.3/pydevd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9745 2024-02-01 01:05:39.000000 pydevd-3.0.3/pydevd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-01 01:05:39.000000 pydevd-3.0.3/pydevd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-02-01 01:05:39.000000 pydevd-3.0.3/pydevd.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-02-01 01:05:39.000000 pydevd-3.0.3/pydevd.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      266 2024-02-01 01:05:39.000000 pydevd-3.0.3/pydevd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   157645 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.669799 pydevd-3.0.3/pydevd_attach_to_process/
+-rw-rw-rw-   0        0        0      987 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/README.txt
+-rw-rw-rw-   0        0        0      711 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/_always_live_program.py
+-rw-rw-rw-   0        0        0      137 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/_check.py
+-rw-rw-rw-   0        0        0      306 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/_test_attach_to_process.py
+-rw-rw-rw-   0        0        0     2597 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/_test_attach_to_process_linux.py
+-rw-rw-rw-   0        0        0    22932 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/add_code_to_python_process.py
+-rw-rw-rw-   0        0        0    36352 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/attach_amd64.dll
+-rw-rw-rw-   0        0        0    31424 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/attach_linux_amd64.so
+-rw-rw-rw-   0        0        0    21388 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/attach_linux_x86.so
+-rw-rw-rw-   0        0        0     2558 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/attach_pydevd.py
+-rw-rw-rw-   0        0        0     8061 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/attach_script.py
+-rw-rw-rw-   0        0        0    31232 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/attach_x86.dll
+-rw-rw-rw-   0        0        0    55296 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/attach_x86_64.dylib
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.685423 pydevd-3.0.3/pydevd_attach_to_process/common/
+-rw-rw-rw-   0        0        0     8591 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/common/py_custom_pyeval_settrace.hpp
+-rw-rw-rw-   0        0        0     4174 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/common/py_custom_pyeval_settrace_310.hpp
+-rw-rw-rw-   0        0        0     4388 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/common/py_custom_pyeval_settrace_311.hpp
+-rw-rw-rw-   0        0        0     1931 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/common/py_custom_pyeval_settrace_common.hpp
+-rw-rw-rw-   0        0        0     8016 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/common/py_settrace.hpp
+-rw-rw-rw-   0        0        0     3894 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/common/py_utils.hpp
+-rw-rw-rw-   0        0        0     2706 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/common/py_version.hpp
+-rw-rw-rw-   0        0        0    22335 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/common/python.h
+-rw-rw-rw-   0        0        0     1537 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/common/ref_utils.hpp
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.685423 pydevd-3.0.3/pydevd_attach_to_process/linux_and_mac/
+-rw-rw-rw-   0        0        0     3814 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/linux_and_mac/attach.cpp
+-rw-rw-rw-   0        0        0      286 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/linux_and_mac/compile_linux.sh
+-rw-rw-rw-   0        0        0      236 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/linux_and_mac/compile_mac.sh
+-rw-rw-rw-   0        0        0     1745 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/linux_and_mac/lldb_prepare.py
+-rw-rw-rw-   0        0        0    16896 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/run_code_on_dllmain_amd64.dll
+-rw-rw-rw-   0        0        0    14336 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/run_code_on_dllmain_x86.dll
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.685423 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/
+-rw-rw-rw-   0        0        0     8180 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/__init__.py
+-rw-rw-rw-   0        0        0   172990 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/breakpoint.py
+-rw-rw-rw-   0        0        0     5412 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/compat.py
+-rw-rw-rw-   0        0        0    67247 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/crash.py
+-rw-rw-rw-   0        0        0    60252 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/debug.py
+-rw-rw-rw-   0        0        0    25131 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/disasm.py
+-rw-rw-rw-   0        0        0    69110 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/event.py
+-rw-rw-rw-   0        0        0    85797 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/interactive.py
+-rw-rw-rw-   0        0        0    72631 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/module.py
+-rw-rw-rw-   0        0        0   188656 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/process.py
+-rw-rw-rw-   0        0        0    22264 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/registry.py
+-rw-rw-rw-   0        0        0    24463 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/search.py
+-rw-rw-rw-   0        0        0    35990 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/sql.py
+-rw-rw-rw-   0        0        0    47181 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/system.py
+-rw-rw-rw-   0        0        0    64570 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/textio.py
+-rw-rw-rw-   0        0        0    77605 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/thread.py
+-rw-rw-rw-   0        0        0    37201 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/util.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.701048 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/
+-rw-rw-rw-   0        0        0     2917 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/__init__.py
+-rw-rw-rw-   0        0        0   124018 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/advapi32.py
+-rw-rw-rw-   0        0        0    25899 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/context_amd64.py
+-rw-rw-rw-   0        0        0    16557 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/context_i386.py
+-rw-rw-rw-   0        0        0    47982 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/dbghelp.py
+-rw-rw-rw-   0        0        0    23517 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/defines.py
+-rw-rw-rw-   0        0        0    17336 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/gdi32.py
+-rw-rw-rw-   0        0        0   169534 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/kernel32.py
+-rw-rw-rw-   0        0        0    23386 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/ntdll.py
+-rw-rw-rw-   0        0        0   162665 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/peb_teb.py
+-rw-rw-rw-   0        0        0    14149 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/psapi.py
+-rw-rw-rw-   0        0        0    14389 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/shell32.py
+-rw-rw-rw-   0        0        0    26563 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/shlwapi.py
+-rw-rw-rw-   0        0        0    58904 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/user32.py
+-rw-rw-rw-   0        0        0    37851 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/version.py
+-rw-rw-rw-   0        0        0    11501 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/wtsapi32.py
+-rw-rw-rw-   0        0        0    25068 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/winappdbg/window.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.701048 pydevd-3.0.3/pydevd_attach_to_process/windows/
+-rw-rw-rw-   0        0        0    28081 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/windows/attach.cpp
+-rw-rw-rw-   0        0        0     1902 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/windows/attach.h
+-rwxrwxrwx   0        0        0     2138 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/windows/compile_windows.bat
+-rw-rw-rw-   0        0        0     4925 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/windows/inject_dll.cpp
+-rw-rw-rw-   0        0        0     2555 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/windows/py_win_helpers.hpp
+-rw-rw-rw-   0        0        0     3470 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/windows/run_code_in_memory.hpp
+-rw-rw-rw-   0        0        0     2594 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/windows/run_code_on_dllmain.cpp
+-rw-rw-rw-   0        0        0     1021 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/windows/stdafx.cpp
+-rw-rw-rw-   0        0        0     1198 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/windows/stdafx.h
+-rw-rw-rw-   0        0        0     1035 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_attach_to_process/windows/targetver.h
+-rw-rw-rw-   0        0        0    37282 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_file_utils.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.701048 pydevd-3.0.3/pydevd_plugins/
+-rw-rw-rw-   0        0        0       68 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_plugins/__init__.py
+-rw-rw-rw-   0        0        0    22636 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_plugins/django_debug.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.701048 pydevd-3.0.3/pydevd_plugins/extensions/
+-rw-rw-rw-   0        0        0       68 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_plugins/extensions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-01 01:05:39.716673 pydevd-3.0.3/pydevd_plugins/extensions/types/
+-rw-rw-rw-   0        0        0       68 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_plugins/extensions/types/__init__.py
+-rw-rw-rw-   0        0        0      665 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_plugins/extensions/types/pydevd_helpers.py
+-rw-rw-rw-   0        0        0     3338 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_plugins/extensions/types/pydevd_plugin_numpy_types.py
+-rw-rw-rw-   0        0        0     6767 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_plugins/extensions/types/pydevd_plugin_pandas_types.py
+-rw-rw-rw-   0        0        0      554 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_plugins/extensions/types/pydevd_plugins_django_form_str.py
+-rw-rw-rw-   0        0        0    19294 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_plugins/jinja2_debug.py
+-rw-rw-rw-   0        0        0     6393 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_plugins/pydevd_line_validation.py
+-rw-rw-rw-   0        0        0    16022 2024-02-01 01:04:41.000000 pydevd-3.0.3/pydevd_tracing.py
+-rw-rw-rw-   0        0        0      279 2024-02-01 01:04:41.000000 pydevd-3.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-02-01 01:05:39.716673 pydevd-3.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     7306 2024-02-01 01:04:41.000000 pydevd-3.0.3/setup.py
+-rw-rw-rw-   0        0        0    11058 2024-02-01 01:04:41.000000 pydevd-3.0.3/setup_pydevd_cython.py
```

### Comparing `pydevd-3.0.2/LICENSE-EPL` & `pydevd-3.0.3/LICENSE-EPL`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/MANIFEST.in` & `pydevd-3.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/PKG-INFO` & `pydevd-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydevd
-Version: 3.0.2
+Version: 3.0.3
 Summary: PyDev.Debugger (used in PyDev, PyCharm and VSCode Python)
 Home-page: https://github.com/fabioz/PyDev.Debugger/
 Author: Fabio Zadrozny and others
 License: EPL
 Keywords: pydev,pydevd,pydev.debugger
 Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
```

### Comparing `pydevd-3.0.2/README.md` & `pydevd-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/_pydev_calltip_util.py` & `pydevd-3.0.3/_pydev_bundle/_pydev_calltip_util.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/_pydev_completer.py` & `pydevd-3.0.3/_pydev_bundle/_pydev_completer.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/_pydev_filesystem_encoding.py` & `pydevd-3.0.3/_pydev_bundle/_pydev_filesystem_encoding.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/_pydev_getopt.py` & `pydevd-3.0.3/_pydev_bundle/_pydev_getopt.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/_pydev_imports_tipper.py` & `pydevd-3.0.3/_pydev_bundle/_pydev_imports_tipper.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/_pydev_jy_imports_tipper.py` & `pydevd-3.0.3/_pydev_bundle/_pydev_jy_imports_tipper.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/_pydev_log.py` & `pydevd-3.0.3/_pydev_bundle/_pydev_log.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/_pydev_saved_modules.py` & `pydevd-3.0.3/_pydev_bundle/_pydev_saved_modules.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/_pydev_sys_patch.py` & `pydevd-3.0.3/_pydev_bundle/_pydev_sys_patch.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/_pydev_tipper_common.py` & `pydevd-3.0.3/_pydev_bundle/_pydev_tipper_common.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/fsnotify/__init__.py` & `pydevd-3.0.3/_pydev_bundle/fsnotify/__init__.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/pydev_console_utils.py` & `pydevd-3.0.3/_pydev_bundle/pydev_console_utils.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/pydev_import_hook.py` & `pydevd-3.0.3/_pydev_bundle/pydev_import_hook.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/pydev_ipython_console.py` & `pydevd-3.0.3/_pydev_bundle/pydev_ipython_console.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/pydev_ipython_console_011.py` & `pydevd-3.0.3/_pydev_bundle/pydev_ipython_console_011.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/pydev_is_thread_alive.py` & `pydevd-3.0.3/_pydev_bundle/pydev_is_thread_alive.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/pydev_localhost.py` & `pydevd-3.0.3/_pydev_bundle/pydev_localhost.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/pydev_log.py` & `pydevd-3.0.3/_pydev_bundle/pydev_log.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/pydev_monkey.py` & `pydevd-3.0.3/_pydev_bundle/pydev_monkey.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/pydev_monkey_qt.py` & `pydevd-3.0.3/_pydev_bundle/pydev_monkey_qt.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/pydev_override.py` & `pydevd-3.0.3/_pydev_bundle/pydev_override.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/pydev_umd.py` & `pydevd-3.0.3/_pydev_bundle/pydev_umd.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_bundle/pydev_versioncheck.py` & `pydevd-3.0.3/_pydev_bundle/pydev_versioncheck.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_runfiles/pydev_runfiles.py` & `pydevd-3.0.3/_pydev_runfiles/pydev_runfiles.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_runfiles/pydev_runfiles_coverage.py` & `pydevd-3.0.3/_pydev_runfiles/pydev_runfiles_coverage.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_runfiles/pydev_runfiles_nose.py` & `pydevd-3.0.3/_pydev_runfiles/pydev_runfiles_nose.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_runfiles/pydev_runfiles_parallel.py` & `pydevd-3.0.3/_pydev_runfiles/pydev_runfiles_parallel.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_runfiles/pydev_runfiles_parallel_client.py` & `pydevd-3.0.3/_pydev_runfiles/pydev_runfiles_parallel_client.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_runfiles/pydev_runfiles_pytest2.py` & `pydevd-3.0.3/_pydev_runfiles/pydev_runfiles_pytest2.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_runfiles/pydev_runfiles_unittest.py` & `pydevd-3.0.3/_pydev_runfiles/pydev_runfiles_unittest.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydev_runfiles/pydev_runfiles_xml_rpc.py` & `pydevd-3.0.3/_pydev_runfiles/pydev_runfiles_xml_rpc.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/_debug_adapter/__main__pydevd_gen_debug_adapter_protocol.py` & `pydevd-3.0.3/_pydevd_bundle/_debug_adapter/__main__pydevd_gen_debug_adapter_protocol.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/_debug_adapter/pydevd_base_schema.py` & `pydevd-3.0.3/_pydevd_bundle/_debug_adapter/pydevd_base_schema.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/_debug_adapter/pydevd_schema.py` & `pydevd-3.0.3/_pydevd_bundle/_debug_adapter/pydevd_schema.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/_debug_adapter/pydevd_schema_log.py` & `pydevd-3.0.3/_pydevd_bundle/_debug_adapter/pydevd_schema_log.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevconsole_code.py` & `pydevd-3.0.3/_pydevd_bundle/pydevconsole_code.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_additional_thread_info.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_additional_thread_info.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_additional_thread_info_regular.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_additional_thread_info_regular.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_api.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_api.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_breakpoints.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_breakpoints.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_bytecode_utils.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_bytecode_utils.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_bytecode_utils_py311.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_bytecode_utils_py311.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_code_to_source.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_code_to_source.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_collect_bytecode_info.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_collect_bytecode_info.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_comm.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_comm.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_comm_constants.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_comm_constants.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_command_line_handling.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_command_line_handling.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_concurrency_analyser/pydevd_concurrency_logger.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_concurrency_analyser/pydevd_concurrency_logger.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_concurrency_analyser/pydevd_thread_wrappers.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_concurrency_analyser/pydevd_thread_wrappers.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_console.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_console.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_constants.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_constants.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_custom_frames.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_custom_frames.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_cython.c` & `pydevd-3.0.3/_pydevd_bundle/pydevd_cython.c`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_cython.pyx` & `pydevd-3.0.3/_pydevd_bundle/pydevd_cython.pyx`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_cython_wrapper.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_cython_wrapper.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_daemon_thread.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_daemon_thread.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_defaults.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_defaults.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_dont_trace.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_dont_trace.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_dont_trace_files.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_dont_trace_files.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_extension_api.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_extension_api.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_extension_utils.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_extension_utils.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_filtering.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_filtering.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_frame.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_frame.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_frame_utils.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_frame_utils.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_gevent_integration.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_gevent_integration.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_import_class.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_import_class.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_io.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_io.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_json_debug_options.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_json_debug_options.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_net_command.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_net_command.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_net_command_factory_json.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_net_command_factory_json.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_net_command_factory_xml.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_net_command_factory_xml.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_plugin_utils.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_plugin_utils.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_process_net_command.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_process_net_command.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_process_net_command_json.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_process_net_command_json.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_referrers.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_referrers.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_reload.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_reload.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_resolver.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_resolver.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_runpy.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_runpy.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_safe_repr.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_safe_repr.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_save_locals.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_save_locals.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_signature.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_signature.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_source_mapping.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_source_mapping.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_stackless.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_stackless.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_suspended_frames.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_suspended_frames.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_thread_lifecycle.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_thread_lifecycle.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_timeout.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_timeout.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_trace_dispatch.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_trace_dispatch.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_trace_dispatch_regular.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_trace_dispatch_regular.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_traceproperty.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_traceproperty.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_utils.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_utils.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_vars.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_vars.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_vm_type.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_vm_type.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_bundle/pydevd_xml.py` & `pydevd-3.0.3/_pydevd_bundle/pydevd_xml.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_frame_eval/pydevd_frame_eval_cython_wrapper.py` & `pydevd-3.0.3/_pydevd_frame_eval/pydevd_frame_eval_cython_wrapper.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_frame_eval/pydevd_frame_eval_main.py` & `pydevd-3.0.3/_pydevd_frame_eval/pydevd_frame_eval_main.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_frame_eval/pydevd_frame_evaluator.c` & `pydevd-3.0.3/_pydevd_frame_eval/pydevd_frame_evaluator.c`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_frame_eval/pydevd_frame_tracing.py` & `pydevd-3.0.3/_pydevd_frame_eval/pydevd_frame_tracing.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_frame_eval/pydevd_modify_bytecode.py` & `pydevd-3.0.3/_pydevd_frame_eval/pydevd_modify_bytecode.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_frame_eval/vendored/bytecode/__init__.py` & `pydevd-3.0.3/_pydevd_frame_eval/vendored/bytecode/__init__.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_frame_eval/vendored/bytecode/bytecode.py` & `pydevd-3.0.3/_pydevd_frame_eval/vendored/bytecode/bytecode.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_frame_eval/vendored/bytecode/cfg.py` & `pydevd-3.0.3/_pydevd_frame_eval/vendored/bytecode/cfg.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_frame_eval/vendored/bytecode/concrete.py` & `pydevd-3.0.3/_pydevd_frame_eval/vendored/bytecode/concrete.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_frame_eval/vendored/bytecode/flags.py` & `pydevd-3.0.3/_pydevd_frame_eval/vendored/bytecode/flags.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_frame_eval/vendored/bytecode/instr.py` & `pydevd-3.0.3/_pydevd_frame_eval/vendored/bytecode/instr.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_frame_eval/vendored/bytecode/peephole_opt.py` & `pydevd-3.0.3/_pydevd_frame_eval/vendored/bytecode/peephole_opt.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_frame_eval/vendored/pydevd_fix_code.py` & `pydevd-3.0.3/_pydevd_frame_eval/vendored/pydevd_fix_code.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_sys_monitoring/_pydevd_sys_monitoring.py` & `pydevd-3.0.3/_pydevd_sys_monitoring/_pydevd_sys_monitoring.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/_pydevd_sys_monitoring/pydevd_sys_monitoring.py` & `pydevd-3.0.3/_pydevd_sys_monitoring/pydevd_sys_monitoring.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/build_tools/build.py` & `pydevd-3.0.3/build_tools/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,14 @@
     else:
         additional_args.append('--force-cython')  # Build always forces cython!
 
     args = [
         sys.executable, os.path.join(os.path.dirname(__file__), '..', 'setup_pydevd_cython.py'), 'build_ext', '--inplace',
     ] + additional_args
     print('Calling args: %s' % (args,))
-    env['PYDEVD_FORCE_BUILD_ALL'] = '1'
     subprocess.check_call(args, env=env,)
 
 
 if __name__ == '__main__':
     use_cython = os.getenv('PYDEVD_USE_CYTHON', '').lower()
     # Note: don't import pydevd during build (so, accept just yes/no in this case).
     if use_cython == 'yes':
```

### Comparing `pydevd-3.0.2/build_tools/build_binaries_osx.py` & `pydevd-3.0.3/build_tools/build_binaries_osx.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/build_tools/build_binaries_windows.py` & `pydevd-3.0.3/build_tools/build_binaries_windows.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/build_tools/check_no_git_modifications.py` & `pydevd-3.0.3/build_tools/check_no_git_modifications.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/build_tools/generate_code.py` & `pydevd-3.0.3/build_tools/generate_code.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/build_tools/names_to_rename.py` & `pydevd-3.0.3/build_tools/names_to_rename.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/build_tools/rename_pep8.py` & `pydevd-3.0.3/build_tools/rename_pep8.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydev_app_engine_debug_startup.py` & `pydevd-3.0.3/pydev_app_engine_debug_startup.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydev_ipython/inputhook.py` & `pydevd-3.0.3/pydev_ipython/inputhook.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydev_ipython/inputhookglut.py` & `pydevd-3.0.3/pydev_ipython/inputhookglut.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydev_ipython/inputhookgtk.py` & `pydevd-3.0.3/pydev_ipython/inputhookgtk.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydev_ipython/inputhookgtk3.py` & `pydevd-3.0.3/pydev_ipython/inputhookgtk3.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydev_ipython/inputhookpyglet.py` & `pydevd-3.0.3/pydev_ipython/inputhookpyglet.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydev_ipython/inputhookqt4.py` & `pydevd-3.0.3/pydev_ipython/inputhookqt4.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydev_ipython/inputhookqt5.py` & `pydevd-3.0.3/pydev_ipython/inputhookqt5.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydev_ipython/inputhooktk.py` & `pydevd-3.0.3/pydev_ipython/inputhooktk.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydev_ipython/inputhookwx.py` & `pydevd-3.0.3/pydev_ipython/inputhookwx.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydev_ipython/matplotlibtools.py` & `pydevd-3.0.3/pydev_ipython/matplotlibtools.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydev_ipython/qt.py` & `pydevd-3.0.3/pydev_ipython/qt.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydev_ipython/qt_for_kernel.py` & `pydevd-3.0.3/pydev_ipython/qt_for_kernel.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydev_ipython/qt_loaders.py` & `pydevd-3.0.3/pydev_ipython/qt_loaders.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydev_ipython/version.py` & `pydevd-3.0.3/pydev_ipython/version.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydev_run_in_console.py` & `pydevd-3.0.3/pydev_run_in_console.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevconsole.py` & `pydevd-3.0.3/pydevconsole.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd.egg-info/PKG-INFO` & `pydevd-3.0.3/pydevd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydevd
-Version: 3.0.2
+Version: 3.0.3
 Summary: PyDev.Debugger (used in PyDev, PyCharm and VSCode Python)
 Home-page: https://github.com/fabioz/PyDev.Debugger/
 Author: Fabio Zadrozny and others
 License: EPL
 Keywords: pydev,pydevd,pydev.debugger
 Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
```

### Comparing `pydevd-3.0.2/pydevd.egg-info/SOURCES.txt` & `pydevd-3.0.3/pydevd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd.py` & `pydevd-3.0.3/pydevd.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             'Please unset GEVENT_SUPPORT from the environment variables or install gevent.')
     else:
         pydevd_gevent_integration.log_gevent_debug_info()
 
 if USE_CUSTOM_SYS_CURRENT_FRAMES_MAP:
     from _pydevd_bundle.pydevd_constants import constructed_tid_to_last_frame
 
-__version_info__ = (3, 0, 2)
+__version_info__ = (3, 0, 3)
 __version_info_str__ = []
 for v in __version_info__:
     __version_info_str__.append(str(v))
 
 __version__ = '.'.join(__version_info_str__)
 
 # IMPORTANT: pydevd_constants must be the 1st thing defined because it'll keep a reference to the original sys._getframe
```

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/README.txt` & `pydevd-3.0.3/pydevd_attach_to_process/README.txt`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/_always_live_program.py` & `pydevd-3.0.3/pydevd_attach_to_process/_always_live_program.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/_test_attach_to_process_linux.py` & `pydevd-3.0.3/pydevd_attach_to_process/_test_attach_to_process_linux.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/add_code_to_python_process.py` & `pydevd-3.0.3/pydevd_attach_to_process/add_code_to_python_process.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/attach_amd64.dll` & `pydevd-3.0.3/pydevd_attach_to_process/attach_amd64.dll`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/attach_linux_amd64.so` & `pydevd-3.0.3/pydevd_attach_to_process/attach_linux_amd64.so`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/attach_linux_x86.so` & `pydevd-3.0.3/pydevd_attach_to_process/attach_linux_x86.so`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/attach_pydevd.py` & `pydevd-3.0.3/pydevd_attach_to_process/attach_pydevd.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/attach_script.py` & `pydevd-3.0.3/pydevd_attach_to_process/attach_script.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/attach_x86.dll` & `pydevd-3.0.3/pydevd_attach_to_process/attach_x86.dll`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/attach_x86_64.dylib` & `pydevd-3.0.3/pydevd_attach_to_process/attach_x86_64.dylib`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/common/py_custom_pyeval_settrace.hpp` & `pydevd-3.0.3/pydevd_attach_to_process/common/py_custom_pyeval_settrace.hpp`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/common/py_custom_pyeval_settrace_310.hpp` & `pydevd-3.0.3/pydevd_attach_to_process/common/py_custom_pyeval_settrace_310.hpp`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/common/py_custom_pyeval_settrace_311.hpp` & `pydevd-3.0.3/pydevd_attach_to_process/common/py_custom_pyeval_settrace_311.hpp`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/common/py_custom_pyeval_settrace_common.hpp` & `pydevd-3.0.3/pydevd_attach_to_process/common/py_custom_pyeval_settrace_common.hpp`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/common/py_settrace.hpp` & `pydevd-3.0.3/pydevd_attach_to_process/common/py_settrace.hpp`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/common/py_utils.hpp` & `pydevd-3.0.3/pydevd_attach_to_process/common/py_utils.hpp`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/common/py_version.hpp` & `pydevd-3.0.3/pydevd_attach_to_process/common/py_version.hpp`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/common/python.h` & `pydevd-3.0.3/pydevd_attach_to_process/common/python.h`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/common/ref_utils.hpp` & `pydevd-3.0.3/pydevd_attach_to_process/common/ref_utils.hpp`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/linux_and_mac/attach.cpp` & `pydevd-3.0.3/pydevd_attach_to_process/linux_and_mac/attach.cpp`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/linux_and_mac/lldb_prepare.py` & `pydevd-3.0.3/pydevd_attach_to_process/linux_and_mac/lldb_prepare.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/run_code_on_dllmain_amd64.dll` & `pydevd-3.0.3/pydevd_attach_to_process/run_code_on_dllmain_amd64.dll`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/run_code_on_dllmain_x86.dll` & `pydevd-3.0.3/pydevd_attach_to_process/run_code_on_dllmain_x86.dll`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/__init__.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/__init__.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/breakpoint.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/breakpoint.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/compat.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/compat.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/crash.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/crash.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/debug.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/debug.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/disasm.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/disasm.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/event.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/event.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/interactive.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/interactive.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/module.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/module.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/process.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/process.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/registry.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/registry.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/search.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/search.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/sql.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/sql.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/system.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/system.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/textio.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/textio.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/thread.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/thread.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/util.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/util.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/__init__.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/__init__.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/advapi32.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/advapi32.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/context_amd64.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/context_amd64.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/context_i386.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/context_i386.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/dbghelp.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/dbghelp.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/defines.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/defines.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/gdi32.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/gdi32.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/kernel32.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/kernel32.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/ntdll.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/ntdll.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/peb_teb.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/peb_teb.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/psapi.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/psapi.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/shell32.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/shell32.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/shlwapi.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/shlwapi.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/user32.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/user32.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/version.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/version.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/win32/wtsapi32.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/win32/wtsapi32.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/winappdbg/window.py` & `pydevd-3.0.3/pydevd_attach_to_process/winappdbg/window.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/windows/attach.cpp` & `pydevd-3.0.3/pydevd_attach_to_process/windows/attach.cpp`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/windows/attach.h` & `pydevd-3.0.3/pydevd_attach_to_process/windows/attach.h`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/windows/compile_windows.bat` & `pydevd-3.0.3/pydevd_attach_to_process/windows/compile_windows.bat`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/windows/inject_dll.cpp` & `pydevd-3.0.3/pydevd_attach_to_process/windows/inject_dll.cpp`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/windows/py_win_helpers.hpp` & `pydevd-3.0.3/pydevd_attach_to_process/windows/py_win_helpers.hpp`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/windows/run_code_in_memory.hpp` & `pydevd-3.0.3/pydevd_attach_to_process/windows/run_code_in_memory.hpp`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/windows/run_code_on_dllmain.cpp` & `pydevd-3.0.3/pydevd_attach_to_process/windows/run_code_on_dllmain.cpp`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/windows/stdafx.cpp` & `pydevd-3.0.3/pydevd_attach_to_process/windows/stdafx.cpp`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/windows/stdafx.h` & `pydevd-3.0.3/pydevd_attach_to_process/windows/stdafx.h`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_attach_to_process/windows/targetver.h` & `pydevd-3.0.3/pydevd_attach_to_process/windows/targetver.h`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_file_utils.py` & `pydevd-3.0.3/pydevd_file_utils.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_plugins/django_debug.py` & `pydevd-3.0.3/pydevd_plugins/django_debug.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_plugins/extensions/types/pydevd_helpers.py` & `pydevd-3.0.3/pydevd_plugins/extensions/types/pydevd_helpers.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_plugins/extensions/types/pydevd_plugin_numpy_types.py` & `pydevd-3.0.3/pydevd_plugins/extensions/types/pydevd_plugin_numpy_types.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_plugins/extensions/types/pydevd_plugin_pandas_types.py` & `pydevd-3.0.3/pydevd_plugins/extensions/types/pydevd_plugin_pandas_types.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_plugins/extensions/types/pydevd_plugins_django_form_str.py` & `pydevd-3.0.3/pydevd_plugins/extensions/types/pydevd_plugins_django_form_str.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_plugins/jinja2_debug.py` & `pydevd-3.0.3/pydevd_plugins/jinja2_debug.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_plugins/pydevd_line_validation.py` & `pydevd-3.0.3/pydevd_plugins/pydevd_line_validation.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/pydevd_tracing.py` & `pydevd-3.0.3/pydevd_tracing.py`

 * *Files identical despite different names*

### Comparing `pydevd-3.0.2/setup.py` & `pydevd-3.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,24 +172,26 @@
                 ["_pydevd_bundle/pydevd_cython.c", ],
                 define_macros=[('Py_BUILD_CORE_MODULE', '1')],
                 **kwargs
             )
         ]
 
     py_version = sys.version_info[:2]
-    if (3, 6) <= py_version <= (3, 11):
+    if (3, 6) <= py_version <= (3, 10):
         ext_modules.append(
             Extension(
                 '_pydevd_frame_eval.pydevd_frame_evaluator',
                 ["_pydevd_frame_eval/pydevd_frame_evaluator.c", ],
                 define_macros=[('Py_BUILD_CORE_MODULE', '1')],
                 **kwargs
             )
         )
 
+    # Note: 3.11 does not have frame eval implemented (nor sys.monitoring)
+
     if py_version >= (3, 12):
         ext_modules.append(
             Extension(
                 '_pydevd_sys_monitoring._pydevd_sys_monitoring_cython',
                 ["_pydevd_sys_monitoring/_pydevd_sys_monitoring_cython.c", ],
                 define_macros=[('Py_BUILD_CORE_MODULE', '1')],
                 **kwargs
```

### Comparing `pydevd-3.0.2/setup_pydevd_cython.py` & `pydevd-3.0.3/setup_pydevd_cython.py`

 * *Files identical despite different names*

