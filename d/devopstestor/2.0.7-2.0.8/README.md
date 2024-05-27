# Comparing `tmp/devopstestor-2.0.7.tar.gz` & `tmp/devopstestor-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopstestor-2.0.7.tar", last modified: Thu May 23 08:54:18 2024, max compression
+gzip compressed data, was "devopstestor-2.0.8.tar", last modified: Mon May 27 11:51:14 2024, max compression
```

## Comparing `devopstestor-2.0.7.tar` & `devopstestor-2.0.8.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.248955 devopstestor-2.0.7/
--rw-rw-rw-   0 root         (0) root         (0)    22958 2024-05-23 08:54:06.000000 devopstestor-2.0.7/LICENCE
--rw-rw-rw-   0 root         (0) root         (0)      228 2024-05-23 08:54:06.000000 devopstestor-2.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      908 2024-05-23 08:54:18.248955 devopstestor-2.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      316 2024-05-23 08:54:06.000000 devopstestor-2.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.225956 devopstestor-2.0.7/bin/
--rwxrwxrwx   0 root         (0) root         (0)      405 2024-05-23 08:54:06.000000 devopstestor-2.0.7/bin/devopstestor-presets
--rwxrwxrwx   0 root         (0) root         (0)       89 2024-05-23 08:54:06.000000 devopstestor-2.0.7/bin/devopstestor-saltstack
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.225956 devopstestor-2.0.7/devopstestor/
--rw-rw-rw-   0 root         (0) root         (0)      430 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.228956 devopstestor-2.0.7/devopstestor/config/
--rw-rw-rw-   0 root         (0) root         (0)     2965 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/config/arguments.yml
--rw-rw-rw-   0 root         (0) root         (0)      340 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/config/core.yml
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/config/machine.yml
--rw-rw-rw-   0 root         (0) root         (0)      353 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/config/provisionner.yml
--rw-rw-rw-   0 root         (0) root         (0)      568 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/config/report.yml
--rw-rw-rw-   0 root         (0) root         (0)     1343 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/config/source_manager.yml
--rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/config/testcase.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.228956 devopstestor-2.0.7/devopstestor/presets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/presets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.228956 devopstestor-2.0.7/devopstestor/presets/saltstack/
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/presets/saltstack/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/presets/saltstack/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      689 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/presets/saltstack/build4docker.bash
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.230955 devopstestor-2.0.7/devopstestor/presets/saltstack/config/
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/presets/saltstack/config/arguments.yml
--rw-rw-rw-   0 root         (0) root         (0)      961 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/presets/saltstack/config/machine.yml
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/presets/saltstack/config/provisionner.yml
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/presets/saltstack/config/report.yml
--rw-rw-rw-   0 root         (0) root         (0)      329 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/presets/saltstack/config/source_manager.yml
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/presets/saltstack/config/testcase.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.230955 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.217956 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.216956 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/etc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.216956 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/etc/salt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.230955 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/etc/salt/master.d/
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/etc/salt/master.d/override.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.230955 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/tmp/
--rw-rw-rw-   0 root         (0) root         (0)     1095 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/tmp/install_base.bash
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.217956 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/usr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.217956 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/usr/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.217956 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.217956 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.217956 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.231955 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/modules/
--rw-rw-rw-   0 root         (0) root         (0)      468 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/modules/sdb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.231955 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/runners/
--rw-rw-rw-   0 root         (0) root         (0)      345 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/runners/sdb.py
--rw-rw-rw-   0 root         (0) root         (0)      717 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/presets/saltstack/machine/salt-machine-debian
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.231955 devopstestor-2.0.7/devopstestor/src/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.232956 devopstestor-2.0.7/devopstestor/src/abstract/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/abstract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5424 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/abstract/abstract_machine_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/abstract/abstract_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     3498 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/abstract/abstract_report.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/abstract/abstract_source_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.234955 devopstestor-2.0.7/devopstestor/src/core/
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5789 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/core/devopstestor.py
--rw-rw-rw-   0 root         (0) root         (0)     1469 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/core/devopstestor_client.py
--rw-rw-rw-   0 root         (0) root         (0)     2230 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/core/devopstestor_server.py
--rw-rw-rw-   0 root         (0) root         (0)     8427 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/core/global_config_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8219 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/core/machines_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     4851 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/core/ordonnanceur.py
--rw-rw-rw-   0 root         (0) root         (0)     2532 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/core/report_render_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2083 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/core/source_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/core/testcase_executor_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.235955 devopstestor-2.0.7/devopstestor/src/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2835 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/lib/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2664 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/lib/core_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/lib/json_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2719 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/lib/log_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    11155 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/lib/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.236956 devopstestor-2.0.7/devopstestor/src/machine/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/machine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2093 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/machine/debug_controller.py
--rw-rw-rw-   0 root         (0) root         (0)    10096 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/machine/docker_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     3568 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/machine/docker_no_volume_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     3754 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/machine/local_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     7265 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/machine/vagrant_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.238955 devopstestor-2.0.7/devopstestor/src/provisionner/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/provisionner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/provisionner/empty_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     4850 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/provisionner/logstash_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     9335 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/provisionner/minion_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/provisionner/systemd_provisionner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.239956 devopstestor-2.0.7/devopstestor/src/reporting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/reporting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/reporting/campaign_report.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/reporting/deployment_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5666 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/reporting/report_elk_renderer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.240955 devopstestor-2.0.7/devopstestor/src/reporting/report_html_renderer/
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/reporting/report_html_renderer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9223 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja
--rw-rw-rw-   0 root         (0) root         (0)     7258 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/reporting/report_text_renderer.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/reporting/scenario_report.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/reporting/testcase_report.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/reporting/verifier_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.241955 devopstestor-2.0.7/devopstestor/src/scenarios/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/scenarios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/scenarios/devopstestor.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/scenarios/logstash.py
--rw-rw-rw-   0 root         (0) root         (0)     6473 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/scenarios/mock_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/scenarios/saltastck.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/scenarios/systemd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.242955 devopstestor-2.0.7/devopstestor/src/sources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2604 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/sources/copytemplate_source_accessor.py
--rw-rw-rw-   0 root         (0) root         (0)     2334 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/sources/dirlink_source_accessor.py
--rw-rw-rw-   0 root         (0) root         (0)     2587 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/sources/git_source_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.243955 devopstestor-2.0.7/devopstestor/src/testcase/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/testcase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8757 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/testcase/scenario_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     6314 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/testcase/test_case.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/testcase/testcase_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     3114 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/src/testcase/tests_cases_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.220955 devopstestor-2.0.7/devopstestor/testconf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.223955 devopstestor-2.0.7/devopstestor/testconf/verifiers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.244955 devopstestor-2.0.7/devopstestor/testconf/verifiers/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/fixtures/context_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/fixtures/logstash_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.244955 devopstestor-2.0.7/devopstestor/testconf/verifiers/service/
--rw-rw-rw-   0 root         (0) root         (0)     4529 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/service/http_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.244955 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.244955 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/http_logger/
--rw-rw-rw-   0 root         (0) root         (0)     1317 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.245955 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/logstash/
--rw-rw-rw-   0 root         (0) root         (0)     5411 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.245955 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.245955 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/filesystem/
--rw-rw-rw-   0 root         (0) root         (0)     1581 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.246955 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/packages/
--rw-rw-rw-   0 root         (0) root         (0)      776 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.246955 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/systemd/
--rw-rw-rw-   0 root         (0) root         (0)      720 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py
--rw-rw-rw-   0 root         (0) root         (0)     2256 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py
--rw-rw-rw-   0 root         (0) root         (0)     3336 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.246955 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/users/
--rw-rw-rw-   0 root         (0) root         (0)      826 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.247955 devopstestor-2.0.7/devopstestor/testconf/verifiers/utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.247955 devopstestor-2.0.7/devopstestor/testconf/verifiers/utils/logstash/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/utils/logstash/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6214 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py
--rw-rw-rw-   0 root         (0) root         (0)     4964 2024-05-23 08:54:06.000000 devopstestor-2.0.7/devopstestor/testconf/verifiers/utils/verififier_luncher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 08:54:18.247955 devopstestor-2.0.7/devopstestor.egg-info/
--rw-r--r--   0 root         (0) root         (0)      908 2024-05-23 08:54:18.000000 devopstestor-2.0.7/devopstestor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5415 2024-05-23 08:54:18.000000 devopstestor-2.0.7/devopstestor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 08:54:18.000000 devopstestor-2.0.7/devopstestor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2024-05-23 08:54:18.000000 devopstestor-2.0.7/devopstestor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-23 08:54:18.000000 devopstestor-2.0.7/devopstestor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 08:54:18.248955 devopstestor-2.0.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-23 08:54:06.000000 devopstestor-2.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.310602 devopstestor-2.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)    22958 2024-05-27 11:51:02.000000 devopstestor-2.0.8/LICENCE
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-05-27 11:51:02.000000 devopstestor-2.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      908 2024-05-27 11:51:14.309602 devopstestor-2.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      316 2024-05-27 11:51:02.000000 devopstestor-2.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.285602 devopstestor-2.0.8/bin/
+-rwxrwxrwx   0 root         (0) root         (0)      405 2024-05-27 11:51:02.000000 devopstestor-2.0.8/bin/devopstestor-presets
+-rwxrwxrwx   0 root         (0) root         (0)       89 2024-05-27 11:51:02.000000 devopstestor-2.0.8/bin/devopstestor-saltstack
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.285602 devopstestor-2.0.8/devopstestor/
+-rw-rw-rw-   0 root         (0) root         (0)      430 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.288602 devopstestor-2.0.8/devopstestor/config/
+-rw-rw-rw-   0 root         (0) root         (0)     2965 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/config/arguments.yml
+-rw-rw-rw-   0 root         (0) root         (0)      340 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/config/core.yml
+-rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/config/machine.yml
+-rw-rw-rw-   0 root         (0) root         (0)      353 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/config/provisionner.yml
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/config/report.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/config/source_manager.yml
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/config/testcase.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.288602 devopstestor-2.0.8/devopstestor/presets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/presets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.289602 devopstestor-2.0.8/devopstestor/presets/saltstack/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/presets/saltstack/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/presets/saltstack/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      689 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/presets/saltstack/build4docker.bash
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.290602 devopstestor-2.0.8/devopstestor/presets/saltstack/config/
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/presets/saltstack/config/arguments.yml
+-rw-rw-rw-   0 root         (0) root         (0)      961 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/presets/saltstack/config/machine.yml
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/presets/saltstack/config/provisionner.yml
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/presets/saltstack/config/report.yml
+-rw-rw-rw-   0 root         (0) root         (0)      329 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/presets/saltstack/config/source_manager.yml
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/presets/saltstack/config/testcase.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.290602 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.279602 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.278602 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/etc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.279602 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/etc/salt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.291602 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/etc/salt/master.d/
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/etc/salt/master.d/override.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.291602 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/tmp/
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/tmp/install_base.bash
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.279602 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/usr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.279602 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/usr/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.279602 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.279602 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.280602 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.291602 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/modules/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/modules/sdb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.291602 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/runners/
+-rw-rw-rw-   0 root         (0) root         (0)      345 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/runners/sdb.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/presets/saltstack/machine/salt-machine-debian
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.291602 devopstestor-2.0.8/devopstestor/src/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.293602 devopstestor-2.0.8/devopstestor/src/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/abstract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5424 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/abstract/abstract_machine_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/abstract/abstract_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3498 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/abstract/abstract_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/abstract/abstract_source_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.295602 devopstestor-2.0.8/devopstestor/src/core/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5789 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/core/devopstestor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/core/devopstestor_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2230 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/core/devopstestor_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     8427 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/core/global_config_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8219 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/core/machines_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4851 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/core/ordonnanceur.py
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/core/report_render_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2083 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/core/source_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/core/testcase_executor_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.296602 devopstestor-2.0.8/devopstestor/src/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2835 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/lib/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/lib/core_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/lib/json_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/lib/log_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    11155 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/lib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.297602 devopstestor-2.0.8/devopstestor/src/machine/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/machine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/machine/debug_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    10230 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/machine/docker_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     4109 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/machine/docker_no_volume_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     3754 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/machine/local_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     7265 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/machine/vagrant_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.299602 devopstestor-2.0.8/devopstestor/src/provisionner/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/provisionner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/provisionner/empty_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/provisionner/logstash_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     9335 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/provisionner/minion_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/provisionner/systemd_provisionner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.300602 devopstestor-2.0.8/devopstestor/src/reporting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/reporting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/reporting/campaign_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/reporting/deployment_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5666 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/reporting/report_elk_renderer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.301602 devopstestor-2.0.8/devopstestor/src/reporting/report_html_renderer/
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/reporting/report_html_renderer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9223 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja
+-rw-rw-rw-   0 root         (0) root         (0)     7258 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/reporting/report_text_renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/reporting/scenario_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/reporting/testcase_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/reporting/verifier_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.302602 devopstestor-2.0.8/devopstestor/src/scenarios/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/scenarios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/scenarios/devopstestor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/scenarios/logstash.py
+-rw-rw-rw-   0 root         (0) root         (0)     6473 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/scenarios/mock_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/scenarios/saltastck.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/scenarios/systemd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.303602 devopstestor-2.0.8/devopstestor/src/sources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2604 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/sources/copytemplate_source_accessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/sources/dirlink_source_accessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2587 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/sources/git_source_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.304602 devopstestor-2.0.8/devopstestor/src/testcase/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/testcase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8757 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/testcase/scenario_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6314 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/testcase/test_case.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/testcase/testcase_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3114 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/src/testcase/tests_cases_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.282602 devopstestor-2.0.8/devopstestor/testconf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.283602 devopstestor-2.0.8/devopstestor/testconf/verifiers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.305602 devopstestor-2.0.8/devopstestor/testconf/verifiers/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/fixtures/context_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/fixtures/logstash_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.305602 devopstestor-2.0.8/devopstestor/testconf/verifiers/service/
+-rw-rw-rw-   0 root         (0) root         (0)     4529 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/service/http_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.305602 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.306602 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/http_logger/
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.306602 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/logstash/
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.306602 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.307602 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/filesystem/
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.307602 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/packages/
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.308602 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/systemd/
+-rw-rw-rw-   0 root         (0) root         (0)      720 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py
+-rw-rw-rw-   0 root         (0) root         (0)     3336 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.308602 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/users/
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.308602 devopstestor-2.0.8/devopstestor/testconf/verifiers/utils/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.309602 devopstestor-2.0.8/devopstestor/testconf/verifiers/utils/logstash/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/utils/logstash/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6214 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4964 2024-05-27 11:51:02.000000 devopstestor-2.0.8/devopstestor/testconf/verifiers/utils/verififier_luncher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 11:51:14.309602 devopstestor-2.0.8/devopstestor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      908 2024-05-27 11:51:14.000000 devopstestor-2.0.8/devopstestor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5415 2024-05-27 11:51:14.000000 devopstestor-2.0.8/devopstestor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 11:51:14.000000 devopstestor-2.0.8/devopstestor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2024-05-27 11:51:14.000000 devopstestor-2.0.8/devopstestor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-27 11:51:14.000000 devopstestor-2.0.8/devopstestor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 11:51:14.310602 devopstestor-2.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-27 11:51:02.000000 devopstestor-2.0.8/setup.py
```

### Comparing `devopstestor-2.0.7/LICENCE` & `devopstestor-2.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/PKG-INFO` & `devopstestor-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopstestor
-Version: 2.0.7
+Version: 2.0.8
 Summary: Framwork to auto test machine provisioning
 Home-page: https://gitlab.com/alexis.porzier.pro/devopstestor
 Author: Alexis PORZIER
 Author-email: alexis.porzier.pro@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `devopstestor-2.0.7/devopstestor/config/arguments.yml` & `devopstestor-2.0.8/devopstestor/config/arguments.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/config/machine.yml` & `devopstestor-2.0.8/devopstestor/config/machine.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/config/report.yml` & `devopstestor-2.0.8/devopstestor/config/report.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/config/source_manager.yml` & `devopstestor-2.0.8/devopstestor/config/source_manager.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/config/testcase.yml` & `devopstestor-2.0.8/devopstestor/config/testcase.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/presets/saltstack/build4docker.bash` & `devopstestor-2.0.8/devopstestor/presets/saltstack/build4docker.bash`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/presets/saltstack/config/machine.yml` & `devopstestor-2.0.8/devopstestor/presets/saltstack/config/machine.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/presets/saltstack/machine/ressources/tmp/install_base.bash` & `devopstestor-2.0.8/devopstestor/presets/saltstack/machine/ressources/tmp/install_base.bash`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/presets/saltstack/machine/salt-machine-debian` & `devopstestor-2.0.8/devopstestor/presets/saltstack/machine/salt-machine-debian`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/abstract/abstract_machine_controller.py` & `devopstestor-2.0.8/devopstestor/src/abstract/abstract_machine_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/abstract/abstract_provisionner.py` & `devopstestor-2.0.8/devopstestor/src/abstract/abstract_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/abstract/abstract_report.py` & `devopstestor-2.0.8/devopstestor/src/abstract/abstract_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/abstract/abstract_source_accessor.py` & `devopstestor-2.0.8/devopstestor/src/abstract/abstract_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/core/devopstestor.py` & `devopstestor-2.0.8/devopstestor/src/core/devopstestor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/core/devopstestor_client.py` & `devopstestor-2.0.8/devopstestor/src/core/devopstestor_client.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/core/devopstestor_server.py` & `devopstestor-2.0.8/devopstestor/src/core/devopstestor_server.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/core/global_config_factory.py` & `devopstestor-2.0.8/devopstestor/src/core/global_config_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/core/machines_factory.py` & `devopstestor-2.0.8/devopstestor/src/core/machines_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/core/ordonnanceur.py` & `devopstestor-2.0.8/devopstestor/src/core/ordonnanceur.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/core/report_render_manager.py` & `devopstestor-2.0.8/devopstestor/src/core/report_render_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/core/source_manager.py` & `devopstestor-2.0.8/devopstestor/src/core/source_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/core/testcase_executor_factory.py` & `devopstestor-2.0.8/devopstestor/src/core/testcase_executor_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/lib/config.py` & `devopstestor-2.0.8/devopstestor/src/lib/config.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/lib/core_utils.py` & `devopstestor-2.0.8/devopstestor/src/lib/core_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/lib/json_utils.py` & `devopstestor-2.0.8/devopstestor/src/lib/json_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/lib/log_manager.py` & `devopstestor-2.0.8/devopstestor/src/lib/log_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/lib/utils.py` & `devopstestor-2.0.8/devopstestor/src/lib/utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/machine/debug_controller.py` & `devopstestor-2.0.8/devopstestor/src/machine/debug_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/machine/docker_controller.py` & `devopstestor-2.0.8/devopstestor/src/machine/docker_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,27 +107,25 @@
             config_docker['volumes'] = []
         binds_host_config = {}
         for name, accessor in list(source_manager.get_accessors().items()):          
             self.share_source_accessor(accessor=accessor, config_docker=config_docker, binds_host_config=binds_host_config)
 
         logger.debut("container_"+machine_name, "Creation d'un conteneur", container_name=machine_name, config_docker=config_docker, binds_host_config=binds_host_config)
         config_docker['host_config'] = client.api.create_host_config(binds=binds_host_config, **machine_configuration.config.get('host_config',{}))
+        config_docker['environment'] = machine_configuration.config.get('run',{}).get('env', {})
         if global_config.get('machine::proxy') is not False:
             # Activate proxy config in docker build
             proxy_url = global_config.get('machine::proxy')     
-            config_docker['environment'] = [
-                'http_proxy='+proxy_url,
-                'https_proxy='+proxy_url,
-                'HTTP_PROXY='+proxy_url,
-                'HTTPS_PROXY='+proxy_url
-            ]
+            config_docker['environment']['http_proxy'] = proxy_url
+            config_docker['environment']['https_proxy'] = proxy_url
+            config_docker['environment']['HTTP_PROXY'] = proxy_url
+            config_docker['environment']['HTTPS_PROXY'] = proxy_url
         # Low level api, tag is in image name
         config_docker['image'] += ':'+config_docker['tag']
         del config_docker['tag']
-        
         container_id = client.api.create_container(**config_docker)
         client.api.connect_container_to_network(container=container_id, net_id="testauto")
         self.container = client.containers.get(machine_name)
         self.container.start()
 
     def share_source_accessor(self, accessor:AbstractSourceAccessor, config_docker, binds_host_config, **kwargs):
         """
```

### Comparing `devopstestor-2.0.7/devopstestor/src/machine/docker_no_volume_controller.py` & `devopstestor-2.0.8/devopstestor/src/machine/docker_no_volume_controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,23 @@
         config_docker['name'] = self.machine_name
         if not 'hostname' in config_docker:
             config_docker['hostname'] = self.machine_name.replace('testauto_','')
 
         logger.debut("container_"+machine_name, "Creation d'un conteneur", container_name=machine_name, config_docker=config_docker)
         config_docker['host_config'] = client.api.create_host_config(**machine_configuration.config.get('host_config',{}))
 
+        config_docker['environment'] = machine_configuration.config.get('run',{}).get('env', {})
+        if global_config.get('machine::proxy') is not False:
+            # Activate proxy config in docker build
+            proxy_url = global_config.get('machine::proxy')
+            config_docker['environment']['http_proxy'] = proxy_url
+            config_docker['environment']['https_proxy'] = proxy_url
+            config_docker['environment']['HTTP_PROXY'] = proxy_url
+            config_docker['environment']['HTTPS_PROXY'] = proxy_url
+
         # Low level api, tag is in image name
         config_docker['image'] += ':'+config_docker['tag']
         del config_docker['tag']
         
         container_id = client.api.create_container(**config_docker)
         client.api.connect_container_to_network(container=container_id, net_id="testauto")
         self.container = client.containers.get(machine_name)
```

### Comparing `devopstestor-2.0.7/devopstestor/src/machine/local_controller.py` & `devopstestor-2.0.8/devopstestor/src/machine/local_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/machine/vagrant_controller.py` & `devopstestor-2.0.8/devopstestor/src/machine/vagrant_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/provisionner/empty_provisionner.py` & `devopstestor-2.0.8/devopstestor/src/provisionner/empty_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/provisionner/logstash_provisionner.py` & `devopstestor-2.0.8/devopstestor/src/provisionner/logstash_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/provisionner/minion_provisionner.py` & `devopstestor-2.0.8/devopstestor/src/provisionner/minion_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/provisionner/systemd_provisionner.py` & `devopstestor-2.0.8/devopstestor/src/provisionner/systemd_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/reporting/report_elk_renderer.py` & `devopstestor-2.0.8/devopstestor/src/reporting/report_elk_renderer.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/reporting/report_html_renderer/__init__.py` & `devopstestor-2.0.8/devopstestor/src/reporting/report_html_renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja` & `devopstestor-2.0.8/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/reporting/report_text_renderer.py` & `devopstestor-2.0.8/devopstestor/src/reporting/report_text_renderer.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/reporting/scenario_report.py` & `devopstestor-2.0.8/devopstestor/src/reporting/scenario_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/reporting/testcase_report.py` & `devopstestor-2.0.8/devopstestor/src/reporting/testcase_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/reporting/verifier_report.py` & `devopstestor-2.0.8/devopstestor/src/reporting/verifier_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/scenarios/devopstestor.py` & `devopstestor-2.0.8/devopstestor/src/scenarios/devopstestor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/scenarios/logstash.py` & `devopstestor-2.0.8/devopstestor/src/scenarios/logstash.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/scenarios/mock_utils.py` & `devopstestor-2.0.8/devopstestor/src/scenarios/mock_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/scenarios/saltastck.py` & `devopstestor-2.0.8/devopstestor/src/scenarios/saltastck.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/scenarios/systemd.py` & `devopstestor-2.0.8/devopstestor/src/scenarios/systemd.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/sources/copytemplate_source_accessor.py` & `devopstestor-2.0.8/devopstestor/src/sources/copytemplate_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/sources/dirlink_source_accessor.py` & `devopstestor-2.0.8/devopstestor/src/sources/dirlink_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/sources/git_source_accessor.py` & `devopstestor-2.0.8/devopstestor/src/sources/git_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/testcase/scenario_executor.py` & `devopstestor-2.0.8/devopstestor/src/testcase/scenario_executor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/testcase/test_case.py` & `devopstestor-2.0.8/devopstestor/src/testcase/test_case.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/testcase/testcase_executor.py` & `devopstestor-2.0.8/devopstestor/src/testcase/testcase_executor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/src/testcase/tests_cases_loader.py` & `devopstestor-2.0.8/devopstestor/src/testcase/tests_cases_loader.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/testconf/verifiers/fixtures/context_fixtures.py` & `devopstestor-2.0.8/devopstestor/testconf/verifiers/fixtures/context_fixtures.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py` & `devopstestor-2.0.8/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/testconf/verifiers/service/http_logger.py` & `devopstestor-2.0.8/devopstestor/testconf/verifiers/service/http_logger.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py` & `devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py` & `devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py` & `devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py` & `devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py` & `devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py` & `devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py` & `devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py` & `devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py` & `devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py` & `devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py` & `devopstestor-2.0.8/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py` & `devopstestor-2.0.8/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor/testconf/verifiers/utils/verififier_luncher.py` & `devopstestor-2.0.8/devopstestor/testconf/verifiers/utils/verififier_luncher.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/devopstestor.egg-info/PKG-INFO` & `devopstestor-2.0.8/devopstestor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopstestor
-Version: 2.0.7
+Version: 2.0.8
 Summary: Framwork to auto test machine provisioning
 Home-page: https://gitlab.com/alexis.porzier.pro/devopstestor
 Author: Alexis PORZIER
 Author-email: alexis.porzier.pro@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `devopstestor-2.0.7/devopstestor.egg-info/SOURCES.txt` & `devopstestor-2.0.8/devopstestor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.7/setup.py` & `devopstestor-2.0.8/setup.py`

 * *Files identical despite different names*

