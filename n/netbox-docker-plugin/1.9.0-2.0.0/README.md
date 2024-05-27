# Comparing `tmp/netbox_docker_plugin-1.9.0.tar.gz` & `tmp/netbox_docker_plugin-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_docker_plugin-1.9.0.tar", last modified: Wed May 15 13:27:04 2024, max compression
+gzip compressed data, was "netbox_docker_plugin-2.0.0.tar", last modified: Mon May 27 12:25:26 2024, max compression
```

## Comparing `netbox_docker_plugin-1.9.0.tar` & `netbox_docker_plugin-2.0.0.tar`

### file list

```diff
@@ -1,139 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.132426 netbox_docker_plugin-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-15 13:27:04.132426 netbox_docker_plugin-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.112426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.116426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/api/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15446 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.116426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/network_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.124426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0002_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0003_image_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0004_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0005_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0011_host_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0012_host_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0013_host_netbox_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0014_container_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0016_alter_env_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0017_network_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0020_container_hostname.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0021_registry_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0023_delete_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0025_alter_image_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0026_image_digest.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0027_container_restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0028_mount_and_bind_read_only.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0029_alter_container_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.124426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.112426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.124426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/container-layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/container-logs.html
--rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/container.html
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/host.html
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/image.html
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/network.html
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.124426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/templatetags/host.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.124426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.128426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11668 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_operation_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.128426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/host/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/host/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/host/test_host_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/host/test_host_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/host/test_replace_password.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.128426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/image/test_image_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/image/test_image_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.128426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/network/test_network_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/network/test_network_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.128426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/registry/test_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/registry/test_registry_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.128426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/volume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/volume/test_volume_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/volume/test_volume_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.128426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.132426 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/label.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/network_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:27:04.132426 netbox_docker_plugin-1.9.0/netbox_docker_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-15 13:27:04.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-05-15 13:27:04.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:27:04.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 13:27:04.000000 netbox_docker_plugin-1.9.0/netbox_docker_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-15 13:26:55.000000 netbox_docker_plugin-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:27:04.132426 netbox_docker_plugin-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.816354 netbox_docker_plugin-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-27 12:25:26.816354 netbox_docker_plugin-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.796355 netbox_docker_plugin-2.0.0/netbox_docker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.800355 netbox_docker_plugin-2.0.0/netbox_docker_plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/api/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16078 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.800355 netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/network_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.808354 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0002_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0003_image_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0004_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0005_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0011_host_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0012_host_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0013_host_netbox_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0014_container_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0016_alter_env_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0017_network_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0020_container_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0021_registry_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0023_delete_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0025_alter_image_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0026_image_digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0027_container_restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0028_mount_and_bind_read_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0029_alter_container_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0030_alter_container_containerid_alter_container_hostname_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.808354 netbox_docker_plugin-2.0.0/netbox_docker_plugin/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11875 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/models/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/models/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/models/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/models/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.796355 netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.808354 netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/container-exec.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/container-layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/container-logs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/container.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/host.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/image.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/network.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.808354 netbox_docker_plugin-2.0.0/netbox_docker_plugin/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/templatetags/host.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.812354 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.812354 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/container/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/container/test_container_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10740 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/container/test_container_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/container/test_container_api_exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11636 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/container/test_container_operation_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/container/test_container_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/container/test_container_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.812354 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/host/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/host/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/host/test_host_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/host/test_host_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/host/test_replace_password.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.812354 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/image/test_image_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/image/test_image_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.812354 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/network/test_network_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/network/test_network_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.812354 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/registry/test_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/registry/test_registry_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.816354 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/volume/test_volume_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/volume/test_volume_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11210 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.816354 netbox_docker_plugin-2.0.0/netbox_docker_plugin/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.816354 netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/network_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:25:26.816354 netbox_docker_plugin-2.0.0/netbox_docker_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-27 12:25:26.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-27 12:25:26.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:25:26.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 12:25:26.000000 netbox_docker_plugin-2.0.0/netbox_docker_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-27 12:25:23.000000 netbox_docker_plugin-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:25:26.816354 netbox_docker_plugin-2.0.0/setup.cfg
```

### Comparing `netbox_docker_plugin-1.9.0/LICENSE` & `netbox_docker_plugin-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/PKG-INFO` & `netbox_docker_plugin-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-docker-plugin
-Version: 1.9.0
+Version: 2.0.0
 Summary: Manage Docker with Netbox & style.
 Author-email: Vincent Simonin <vincent@saashup.com>, David Delassus <david.jose.delassus@gmail.com>
 Project-URL: Homepage, https://github.com/SaaShup/netbox-docker-plugin
 Project-URL: Bug Tracker, https://github.com/SaaShup/netbox-docker-plugin/issues
 Keywords: netbox,netbox-plugin,docker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `netbox_docker_plugin-1.9.0/README.md` & `netbox_docker_plugin-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/__init__.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Netbox Plugin Configuration"""
 
-from extras.plugins import PluginConfig
 from django.db.models.signals import post_migrate
+from netbox.plugins import PluginConfig
 from .utilities import create_webhook
 
 class NetBoxDockerConfig(PluginConfig):
     """Plugin Config Class"""
 
     name = "netbox_docker_plugin"
     verbose_name = " NetBox Docker Plugin"
     description = "Manage Docker"
-    version = "1.9.0"
+    version = "2.0.0"
     base_url = "docker"
+    min_version = "4.0.0"
     author= "Vincent Simonin <vincent@saashup.com>, David Delassus <david.jose.delassus@gmail.com>"
     author_email= "vincent@saashup.com, david.jose.delassus@gmail.com"
 
     def ready(self):
         from . import signals # pylint: disable=unused-import, import-outside-toplevel
 
         post_migrate.connect(create_webhook)
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/api/serializers.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/api/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """API Serializer definitions"""
 
 # pylint: disable=E1101
 
 from rest_framework import serializers
-from utilities.utils import dict_to_filter_params
+from utilities.query import dict_to_filter_params
 from users.api.nested_serializers import NestedTokenSerializer
 from netbox.api.serializers import NetBoxModelSerializer, WritableNestedSerializer
 from ..models.host import Host
 from ..models.image import Image
 from ..models.volume import Volume
 from ..models.network import Network
 from ..models.container import (
@@ -91,15 +91,15 @@
         if data is None:
             return None
 
         if isinstance(data, dict):
             params = dict_to_filter_params(data)
             if Volume.objects.filter(**params).count() == 0:
                 host = Host.objects.get(pk=params["host"])
-                volume = Volume(host= host, name= params["name"])
+                volume = Volume(host=host, name=params["name"])
                 volume.save()
                 return volume
 
         return super().to_internal_value(data)
 
 
 class NestedNetworkSerializer(WritableNestedSerializer):
@@ -225,14 +225,15 @@
             "Digest",
             "custom_fields",
             "created",
             "last_updated",
             "containers",
             "tags",
         )
+        brief_fields = NestedImageSerializer.Meta.fields
 
 
 class VolumeSerializer(NetBoxModelSerializer):
     """Volume Serializer class"""
 
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_docker_plugin-api:volume-detail"
@@ -253,14 +254,15 @@
             "driver",
             "custom_fields",
             "created",
             "last_updated",
             "mounts",
             "tags",
         )
+        brief_fields = NestedVolumeSerializer.Meta.fields
 
 
 class NetworkSerializer(NetBoxModelSerializer):
     """Network Serializer class"""
 
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_docker_plugin-api:network-detail"
@@ -283,14 +285,15 @@
             "state",
             "custom_fields",
             "created",
             "last_updated",
             "network_settings",
             "tags",
         )
+        brief_fields = NestedNetworkSerializer.Meta.fields
 
 
 class PortSerializer(serializers.ModelSerializer):
     """Container Port Serializer class"""
 
     class Meta:
         """Container Port Serializer Meta class"""
@@ -410,14 +413,15 @@
             "binds",
             "network_settings",
             "custom_fields",
             "created",
             "last_updated",
             "tags",
         )
+        brief_fields = NestedContainerSerializer.Meta.fields
 
     def validate(self, data):
         attrs = data.copy()
         attrs.pop("ports", None)
         attrs.pop("env", None)
         attrs.pop("labels", None)
         attrs.pop("mounts", None)
@@ -540,14 +544,15 @@
             "display",
             "serveraddress",
             "username",
             "password",
             "email",
             "images",
         )
+        brief_fields = NestedRegistrySerializer.Meta.fields
 
 
 class HostSerializer(NetBoxModelSerializer):
     """Host Serializer class"""
 
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_docker_plugin-api:host-detail"
@@ -580,7 +585,20 @@
             "tags",
             "images",
             "volumes",
             "networks",
             "containers",
             "registries",
         )
+        brief_fields = NestedHostSerializer.Meta.fields
+
+
+class ContainerCommandSerializer(serializers.Serializer):
+    """Container command Serializer class"""
+
+    cmd = serializers.ListField(child=serializers.CharField())
+
+    def create(self, validated_data):
+        pass
+
+    def update(self, instance, validated_data):
+        pass
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/api/views.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/api/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """API views definitions"""
 
 from collections.abc import Sequence
-from drf_spectacular.utils import extend_schema, OpenApiResponse, OpenApiExample
+import json
+import requests
 from rest_framework import status
+from rest_framework.renderers import JSONRenderer
 from rest_framework.decorators import action
 from rest_framework.response import Response
-import requests
-
+from drf_spectacular.utils import (
+    extend_schema,
+    OpenApiResponse,
+    OpenApiExample,
+)
 from users.models import Token
 from netbox.api.viewsets import NetBoxModelViewSet
-
 from .. import filtersets
 from .renderers import PlainTextRenderer
 from .serializers import (
     HostSerializer,
     ImageSerializer,
     VolumeSerializer,
     NetworkSerializer,
     ContainerSerializer,
     RegistrySerializer,
+    ContainerCommandSerializer,
 )
 from ..models.host import Host
 from ..models.image import Image
 from ..models.volume import Volume
 from ..models.network import Network
 from ..models.container import Container
 from ..models.registry import Registry
@@ -99,15 +104,14 @@
         "labels",
         "tags",
     )
     filterset_class = filtersets.ContainerFilterSet
     serializer_class = ContainerSerializer
     http_method_names = ["get", "post", "patch", "delete", "options"]
 
-
     @extend_schema(
         operation_id="plugins_docker_container_logs",
         responses={
             (200, "text/plain"): OpenApiResponse(
                 response=str,
                 examples=[
                     OpenApiExample(
@@ -131,15 +135,15 @@
     )
     @action(
         detail=True,
         methods=["get"],
         renderer_classes=[PlainTextRenderer],
     )
     def logs(self, _request, **_kwargs):
-        """ Fetch container's logs """
+        """Fetch container's logs"""
 
         container: Container = self.get_object()
         agent_url = container.host.endpoint
         container_id = container.ContainerID
 
         url = f"{agent_url}/api/engine/containers/{container_id}/logs"
 
@@ -156,14 +160,72 @@
 
         return Response(
             resp.text,
             status=status.HTTP_200_OK,
             content_type="text/plain",
         )
 
+    @extend_schema(
+        operation_id="plugins_docker_container_exec",
+        request=ContainerCommandSerializer,
+        responses={
+            (200, "text/plain"): OpenApiResponse(
+                response=str,
+                examples=[
+                    OpenApiExample(
+                        "Command output",
+                        value={"stdout": "..."},
+                        media_type="application/json",
+                    ),
+                ],
+            ),
+            (502, "text/plain"): OpenApiResponse(
+                response=str,
+                examples=[
+                    OpenApiExample(
+                        "Engine error",
+                        value="Error as returned by Agent",
+                        media_type="text/plain",
+                    ),
+                ],
+            ),
+        },
+    )
+    @action(detail=True, methods=["post"], renderer_classes=[JSONRenderer])
+    def exec(self, _request, **_kwargs):
+        """Exec a command on a Container"""
+
+        serializer = ContainerCommandSerializer(data=_request.data)
+        if not serializer.is_valid():
+            return Response(serializer.errors, status=status.HTTP_400_BAD_REQUEST)
+
+        container: Container = self.get_object()
+        agent_url = container.host.endpoint
+        container_id = container.ContainerID
+
+        url = f"{agent_url}/api/engine/containers/{container_id}/exec"
+
+        try:
+            resp = requests.put(
+                url,
+                data=json.dumps(serializer.validated_data),
+                timeout=30,
+                headers={"Content-Type": "application/json"},
+            )
+            resp.raise_for_status()
+
+        except requests.HTTPError:
+            return Response(
+                resp.text,
+                status=status.HTTP_502_BAD_GATEWAY,
+                content_type="text/plain",
+            )
+
+        return Response(data=json.loads(resp.text))
+
 
 class RegistryViewSet(NetBoxModelViewSet):
     """Registry view set class"""
 
     queryset = Registry.objects.prefetch_related("host", "images", "tags")
     filterset_class = filtersets.RegistryFilterSet
     serializer_class = RegistrySerializer
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/filtersets.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/bind.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/bind.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Mount Form definition"""
 
 from django import forms
-from utilities.forms.mixins import BootstrapMixin
 from utilities.forms.fields import (
     DynamicModelMultipleChoiceField,
     DynamicModelChoiceField,
 )
 from netbox.forms import (
     NetBoxModelFilterSetForm,
 )
 from ..models.container import Bind, Container
 
 
-class BindForm(BootstrapMixin, forms.ModelForm):
+class BindForm(forms.ModelForm):
     """Bind form definition class"""
 
     container = DynamicModelChoiceField(
         label="Container", queryset=Container.objects.all(), required=True
     )
 
     class Meta:
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/container.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/container.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Container Forms definitions"""
 
 from django import forms
+from utilities.forms.rendering import FieldSet
 from utilities.forms.fields import (
     TagFilterField,
     DynamicModelMultipleChoiceField,
     DynamicModelChoiceField,
 )
 from netbox.forms import (
     NetBoxModelForm,
@@ -48,14 +49,43 @@
             "host": "Host",
             "image": "Image",
             "hostname": "Hostname",
             "restart_policy": "Restart Policy",
         }
 
 
+class ContainerEditForm(NetBoxModelForm):
+    """Container form definition class"""
+
+    image = DynamicModelChoiceField(
+        label="Image",
+        queryset=Image.objects.all(),
+        required=True,
+        query_params={"host_id": "$host"},
+    )
+
+    class Meta:
+        """Container form definition Meta class"""
+
+        model = Container
+        fields = (
+            "image",
+            "name",
+            "hostname",
+            "restart_policy",
+            "tags",
+        )
+        labels = {
+            "name": "Name",
+            "image": "Image",
+            "hostname": "Hostname",
+            "restart_policy": "Restart Policy",
+        }
+
+
 class ContainerFilterForm(NetBoxModelFilterSetForm):
     """Container filter form definition class"""
 
     model = Volume
     name = forms.CharField(label="Name", max_length=256, min_length=1, required=False)
     ContainerID = forms.CharField(
         label="Name", max_length=128, min_length=1, required=False
@@ -116,15 +146,15 @@
         required=True,
     )
     hostname = forms.CharField(
         label="Hostname", max_length=256, min_length=1, required=False
     )
 
     model = Container
-    fieldsets = (("General", ("restart_policy", "hostname")),)
+    fieldsets = (FieldSet("restart_policy", "hostname", name="General"),)
 
 
 class ContainerOperationForm(NetBoxModelForm):
     """Container Operation form definition class"""
 
     class Meta:
         """Container form definition Meta class"""
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/env.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/env.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Env Form definition"""
 
 from django import forms
 from utilities.forms.fields import DynamicModelChoiceField
-from utilities.forms.mixins import BootstrapMixin
 from ..models.container import Env, Container
 
 
-class EnvForm(BootstrapMixin, forms.ModelForm):
+class EnvForm(forms.ModelForm):
     """Env form definition class"""
 
     container = DynamicModelChoiceField(
         label="Container", queryset=Container.objects.all(), required=True
     )
 
     class Meta:
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/host.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/host.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Host Forms definitions"""
 
 from django import forms
+from utilities.forms.rendering import FieldSet
 from utilities.forms.fields import TagFilterField
 from netbox.forms import (
     NetBoxModelForm,
     NetBoxModelImportForm,
     NetBoxModelFilterSetForm,
     NetBoxModelBulkEditForm,
 )
@@ -66,8 +67,8 @@
     """Host bulk edit form definition class"""
 
     endpoint = forms.CharField(
         required=False,
     )
 
     model = Host
-    fieldsets = (("General", ("endpoint",)),)
+    fieldsets = (FieldSet("endpoint", name="General"),)
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/image.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Image Forms definitions"""
 
 from django import forms
+from utilities.forms.rendering import FieldSet
 from utilities.forms.fields import (
     TagFilterField,
     DynamicModelMultipleChoiceField,
     DynamicModelChoiceField,
 )
 from netbox.forms import (
     NetBoxModelForm,
@@ -97,8 +98,8 @@
     """Image bulk edit form definition class"""
 
     version = forms.CharField(
         required=False,
     )
 
     model = Image
-    fieldsets = (("General", ("version",)),)
+    fieldsets = (FieldSet("version", name="General"),)
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/label.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/port.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-"""Label Form definition"""
+"""Port Form definition"""
 
 from django import forms
 from utilities.forms.fields import DynamicModelChoiceField
-from utilities.forms.mixins import BootstrapMixin
-from ..models.container import Label, Container
+from ..models.container import Port, Container
 
 
-class LabelForm(BootstrapMixin, forms.ModelForm):
-    """Label form definition class"""
+class PortForm(forms.ModelForm):
+    """Port form definition class"""
 
     container = DynamicModelChoiceField(
         label="Container", queryset=Container.objects.all(), required=True
     )
 
     class Meta:
-        """Label form definition Meta class"""
+        """Port form definition Meta class"""
 
-        model = Label
+        model = Port
         fields = (
             "container",
-            "key",
-            "value",
+            "public_port",
+            "private_port",
+            "type",
         )
         labels = {
             "container": "Container",
-            "key": "Key",
-            "value": "Value",
+            "public_port": "Public Port",
+            "private_port": "Private Port",
+            "type": "Type",
         }
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/mount.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/mount.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Mount Form definition"""
 
 from django import forms
-from utilities.forms.mixins import BootstrapMixin
 from utilities.forms.fields import (
     DynamicModelMultipleChoiceField,
     DynamicModelChoiceField,
 )
 from netbox.forms import (
     NetBoxModelFilterSetForm,
 )
 from ..models.container import Mount, Container
 from ..models.volume import Volume
 
 
-class MountForm(BootstrapMixin, forms.ModelForm):
+class MountForm(forms.ModelForm):
     """Mount form definition class"""
 
     container = DynamicModelChoiceField(
         label="Container", queryset=Container.objects.all(), required=True
     )
     volume = DynamicModelChoiceField(
         label="Volume", queryset=Volume.objects.all(), required=True
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/network.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Network Forms definitions"""
 
 from django import forms
+from utilities.forms.rendering import FieldSet
 from utilities.forms.fields import TagFilterField, DynamicModelMultipleChoiceField
 from utilities.choices import ChoiceSet
 from netbox.forms import (
     NetBoxModelForm,
     NetBoxModelImportForm,
     NetBoxModelFilterSetForm,
     NetBoxModelBulkEditForm,
@@ -99,13 +100,8 @@
 class NetworkBulkEditForm(NetBoxModelBulkEditForm):
     """Network bulk edit form definition class"""
 
     driver = forms.ChoiceField(choices=NetworkDriverChoices, required=False)
     NetworkID = forms.CharField(required=False, label="NetworkID")
 
     model = Network
-    fieldsets = (
-        (
-            "General",
-            ("driver", "NetworkID"),
-        ),
-    )
+    fieldsets =(FieldSet("driver", "NetworkID", name="General"),)
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/network_setting.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/network_setting.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """NetworkSetting Form definition"""
 
 from django import forms
 from utilities.forms.fields import (
     DynamicModelMultipleChoiceField,
     DynamicModelChoiceField,
 )
-from utilities.forms.mixins import BootstrapMixin
 from netbox.forms import (
     NetBoxModelFilterSetForm,
 )
 from ..models.container import NetworkSetting, Container
 from ..models.network import Network
 
 
-class NetworkSettingForm(BootstrapMixin, forms.ModelForm):
+class NetworkSettingForm(forms.ModelForm):
     """NetworkSetting form definition class"""
 
     container = DynamicModelChoiceField(
         label="Container", queryset=Container.objects.all(), required=True
     )
     network = DynamicModelChoiceField(
         label="Network", queryset=Network.objects.all(), required=True
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/registry.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/registry.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/forms/volume.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/forms/volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0001_initial.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0002_image.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0002_image.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0003_image_size.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0003_image_size.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0004_volume.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0004_volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0005_network.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0005_network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0011_host_token.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0011_host_token.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0012_host_state.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0012_host_state.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0013_host_netbox_url.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0013_host_netbox_url.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0016_alter_env_value.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0016_alter_env_value.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0020_container_hostname.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0020_container_hostname.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0021_registry_and_more.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0021_registry_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0023_delete_hosts.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0023_delete_hosts.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0025_alter_image_version.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0025_alter_image_version.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0026_image_digest.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0026_image_digest.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/0028_mount_and_bind_read_only.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/0028_mount_and_bind_read_only.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/migrations/__init__.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/container.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/models/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,28 +106,30 @@
     status = models.CharField(max_length=1024, blank=True, null=True)
     ContainerID = models.CharField(
         max_length=128,
         validators=[
             MinLengthValidator(limit_value=1),
             MaxLengthValidator(limit_value=128),
         ],
+        default=None,
         blank=True,
         null=True,
     )
     operation = models.CharField(
         max_length=32,
         choices=ContainerOperationChoices,
         default=ContainerOperationChoices.DEFAULT_VALUE,
     )
     hostname = models.CharField(
         max_length=256,
         validators=[
             MinLengthValidator(limit_value=1),
             MaxLengthValidator(limit_value=256),
         ],
+        default=None,
         blank=True,
         null=True,
     )
     restart_policy = models.CharField(
         max_length=32,
         choices=ContainerRestartPolicyChoices,
         default=ContainerRestartPolicyChoices.DEFAULT_VALUE,
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/host.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/models/host.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/image.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/models/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,23 +46,25 @@
     )
     ImageID = models.CharField(
         max_length=128,
         validators=[
             MinLengthValidator(limit_value=1),
             MaxLengthValidator(limit_value=128),
         ],
+        default=None,
         blank=True,
         null=True,
     )
     Digest = models.CharField(
         max_length=512,
         validators=[
             MinLengthValidator(limit_value=1),
             MaxLengthValidator(limit_value=512),
         ],
+        default=None,
         blank=True,
         null=True,
     )
 
     class Meta:
         """Image Model Meta Class"""
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/network.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/models/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     )
     NetworkID = models.CharField(
         max_length=128,
         validators=[
             MinLengthValidator(limit_value=1),
             MaxLengthValidator(limit_value=128),
         ],
+        default=None,
         blank=True,
         null=True,
     )
     state = models.CharField(
         max_length=32,
         choices=NetworkStateChoices,
         default=NetworkStateChoices.DEFAULT_VALUE,
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/registry.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/models/registry.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/models/volume.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/models/volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/navigation.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/navigation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,85 @@
 """Navigation Menu definitions"""
 
-from extras.plugins import (
+from netbox.plugins import (
     PluginMenu,
     PluginMenuItem,
     PluginMenuButton,
 )
-from utilities.choices import ButtonColorChoices
 
 host_buttons = [
     PluginMenuButton(
         link="plugins:netbox_docker_plugin:host_add",
         title="Add",
-        icon_class="mdi mdi-plus-thick",
-        color=ButtonColorChoices.GREEN,
+        icon_class="mdi mdi-plus-thick"
     ),
     PluginMenuButton(
         link="plugins:netbox_docker_plugin:host_import",
         title="Import",
-        icon_class="mdi mdi-upload",
-        color=ButtonColorChoices.CYAN,
+        icon_class="mdi mdi-upload"
     ),
 ]
 
 registry_button = [
     PluginMenuButton(
         link="plugins:netbox_docker_plugin:registry_add",
         title="Add",
-        icon_class="mdi mdi-plus-thick",
-        color=ButtonColorChoices.GREEN,
+        icon_class="mdi mdi-plus-thick"
     ),
 ]
 
 image_buttons = [
     PluginMenuButton(
         link="plugins:netbox_docker_plugin:image_add",
         title="Add",
-        icon_class="mdi mdi-plus-thick",
-        color=ButtonColorChoices.GREEN,
+        icon_class="mdi mdi-plus-thick"
     ),
     PluginMenuButton(
         link="plugins:netbox_docker_plugin:image_import",
         title="Import",
-        icon_class="mdi mdi-upload",
-        color=ButtonColorChoices.CYAN,
+        icon_class="mdi mdi-upload"
     ),
 ]
 
 volume_buttons = [
     PluginMenuButton(
         link="plugins:netbox_docker_plugin:volume_add",
         title="Add",
-        icon_class="mdi mdi-plus-thick",
-        color=ButtonColorChoices.GREEN,
+        icon_class="mdi mdi-plus-thick"
     ),
     PluginMenuButton(
         link="plugins:netbox_docker_plugin:volume_import",
         title="Import",
-        icon_class="mdi mdi-upload",
-        color=ButtonColorChoices.CYAN,
+        icon_class="mdi mdi-upload"
     ),
 ]
 
 network_buttons = [
     PluginMenuButton(
         link="plugins:netbox_docker_plugin:network_add",
         title="Add",
-        icon_class="mdi mdi-plus-thick",
-        color=ButtonColorChoices.GREEN,
+        icon_class="mdi mdi-plus-thick"
     ),
     PluginMenuButton(
         link="plugins:netbox_docker_plugin:network_import",
         title="Import",
-        icon_class="mdi mdi-upload",
-        color=ButtonColorChoices.CYAN,
+        icon_class="mdi mdi-upload"
     ),
 ]
 
 container_buttons = [
     PluginMenuButton(
         link="plugins:netbox_docker_plugin:container_add",
         title="Add",
-        icon_class="mdi mdi-plus-thick",
-        color=ButtonColorChoices.GREEN,
+        icon_class="mdi mdi-plus-thick"
     ),
     PluginMenuButton(
         link="plugins:netbox_docker_plugin:container_import",
         title="Import",
-        icon_class="mdi mdi-upload",
-        color=ButtonColorChoices.CYAN,
+        icon_class="mdi mdi-upload"
     ),
 ]
 
 host_item = [
     PluginMenuItem(
         link="plugins:netbox_docker_plugin:host_list",
         link_text="Hosts",
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/signals.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/signals.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 """ Hooks on Django model signals. """
 
 from django.db.models.signals import pre_delete, pre_save
+from django.core.exceptions import ObjectDoesNotExist
 from django.dispatch import receiver
 from utilities.exceptions import AbortRequest
-
 from .models import Container
 
 
+@receiver(pre_save, sender=Container)
+def prevent_changing_container_host(instance, **_kwargs):
+    """Prevent that a container's host cannot be changed"""
+
+    if _kwargs.get("created") is not True:
+        try:
+            previous = Container.objects.get(pk=instance.pk)
+        except ObjectDoesNotExist:
+            pass
+        else:
+            if previous.host.pk != instance.host.pk:
+                raise AbortRequest("Cannot change the host's container")
+
+
 @receiver(pre_delete, sender=Container)
 def prevent_deleting_running_containers(instance, **_kwargs):
-    """ Abort deletion if container is running. """
+    """Abort deletion if container is running."""
 
     if not instance.can_delete:
         raise AbortRequest(
             f"The container {instance.name} is running, please stop it before deletion"
         )
 
 
 @receiver(pre_save, sender=Container)
 def restrict_container_actions(instance, **_kwargs):
-    """ Check if the container's state is correct for the given action """
+    """Check if the container's state is correct for the given action"""
 
-    if any([
-        instance.operation == "create" and not instance.can_create,
-        instance.operation == "start" and not instance.can_start,
-        instance.operation == "restart" and not instance.can_restart,
-        instance.operation == "stop" and not instance.can_stop,
-        instance.operation == "recreate" and not instance.can_recreate,
-    ]):
+    if any(
+        [
+            instance.operation == "create" and not instance.can_create,
+            instance.operation == "start" and not instance.can_start,
+            instance.operation == "restart" and not instance.can_restart,
+            instance.operation == "stop" and not instance.can_stop,
+            instance.operation == "recreate" and not instance.can_recreate,
+        ]
+    ):
         raise AbortRequest(
             f"Cannot {instance.operation} container {instance.name} in state {instance.state}"
         )
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tables.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/container-layout.html` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/container-layout.html`

 * *Files 18% similar despite different names*

```diff
@@ -4,57 +4,57 @@
 
 {% block extra_controls %}
 <form action="{% url 'plugins:netbox_docker_plugin:container_operation' pk=object.id operation='start' %}" method="post">
   {% csrf_token %}
   <input type="hidden" name="operation" value="start">
   <button
     type="submit"
-    class="btn btn-sm btn-success"
+    class="btn btn-success"
     {% if not object.can_start %}
     disabled
     {% endif %}
   >
     <i class="mdi mdi-play"></i> Start
   </button>
 </form>
 
 <form action="{% url 'plugins:netbox_docker_plugin:container_operation' pk=object.id operation='stop' %}" method="post">
   {% csrf_token %}
   <input type="hidden" name="operation" value="stop">
   <button
     type="submit"
-    class="btn btn-sm btn-danger"
+    class="btn btn-danger"
     {% if not object.can_stop %}
     disabled
     {% endif %}
   >
     <i class="mdi mdi-stop"></i> Stop
   </button>
 </form>
 
 <form action="{% url 'plugins:netbox_docker_plugin:container_operation' pk=object.id operation='restart' %}" method="post">
   {% csrf_token %}
   <input type="hidden" name="operation" value="restart">
   <button
     type="submit"
-    class="btn btn-sm btn-light"
+    class="btn btn-light"
     {% if not object.can_restart %}
     disabled
     {% endif %}
   >
     <i class="mdi mdi-restart"></i> Restart
   </button>
 </form>
 
 <form action="{% url 'plugins:netbox_docker_plugin:container_operation' pk=object.id operation='recreate' %}" method="post">
   {% csrf_token %}
   <input type="hidden" name="operation" value="recreate">
   <button
     type="submit"
-    class="btn btn-sm btn-dark"
+    class="btn btn-primary"
     {% if not object.can_recreate %}
     disabled
     {% endif %}
   >
     <i class="mdi mdi-autorenew"></i> Recreate
   </button>
 </form>
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/container-logs.html` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/container-logs.html`

 * *Files 6% similar despite different names*

```diff
@@ -2,62 +2,54 @@
 
 {% load plugins %}
 
 {% block content %}
 <div class="row mb-3">
   <div class="col col-md-12">
     <div class="card">
-      <div class="card-header">
-        <div class="d-sm-flex p-2 flex-row align-items-center">
-          <h5 class="flex-grow-1">LOGS</h5>
-          <button
-            id="container-logs-button"
-            type="button"
-            class="btn btn-primary"
-          >
+      <div class="card-header d-flex">
+        <h5 class="flex-grow-1">LOGS</h5>
+        <div>
+          <button id="container-logs-button" type="button" class="btn btn-primary">
             <i id="container-logs-cb" class="mdi mdi-checkbox-marked"></i> Follow logs
           </button>
         </div>
+      </div>
       <div class="card-body">
-        <pre
-          id="container-logs-panel"
-          data-follow="true"
-          class="p-2 text-white border-dark"
-          style="height: 300px; overflow-y: auto; background-color: black;"
-          hx-get="/api/plugins/docker/containers/{{ object.pk }}/logs/"
-          hx-trigger="load, every 30s"
-        >
+        <pre id="container-logs-panel" data-follow="true" class="p-2 text-white border-dark"
+          style="height: 300px; overflow-y: auto; background-color: black; resize: vertical;"
+          hx-get="/api/plugins/docker/containers/{{ object.pk }}/logs/" hx-trigger="load, every 30s">
         </pre>
       </div>
     </div>
   </div>
 </div>
 {% endblock %}
 
 {% block head %}
 <script type="application/javascript">
-htmx.onLoad(function(elt) {
-  const logPanel = document.getElementById("container-logs-panel")
-  const followButton = document.getElementById("container-logs-button")
-  const checkbox = document.getElementById("container-logs-cb")
-
-  const isFollowEnabled = () => JSON.parse(logPanel.dataset.follow) === true
-  const toggleFollow = () => {
-    logPanel.dataset.follow = !isFollowEnabled()
-    followButton.classList.toggle("btn-primary")
-    followButton.classList.toggle("btn-outline-primary")
-    checkbox.classList.toggle("mdi-checkbox-marked")
-    checkbox.classList.toggle("mdi-checkbox-blank-outline")
-  }
-
-  logPanel.addEventListener("htmx:afterSwap", function() {
-    if (isFollowEnabled()) {
-      this.scrollTop = this.scrollHeight
+  htmx.onLoad(function (elt) {
+    const logPanel = document.getElementById("container-logs-panel")
+    const followButton = document.getElementById("container-logs-button")
+    const checkbox = document.getElementById("container-logs-cb")
+
+    const isFollowEnabled = () => JSON.parse(logPanel.dataset.follow) === true
+    const toggleFollow = () => {
+      logPanel.dataset.follow = !isFollowEnabled()
+      followButton.classList.toggle("btn-primary")
+      followButton.classList.toggle("btn-outline-primary")
+      checkbox.classList.toggle("mdi-checkbox-marked")
+      checkbox.classList.toggle("mdi-checkbox-blank-outline")
     }
-  })
 
-  followButton.addEventListener("click", function() {
-    toggleFollow()
+    logPanel.addEventListener("htmx:afterSwap", function () {
+      if (isFollowEnabled()) {
+        this.scrollTop = this.scrollHeight
+      }
+    })
+
+    followButton.addEventListener("click", function () {
+      toggleFollow()
+    })
   })
-})
 </script>
 {% endblock %}
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/container.html` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/container.html`

 * *Files 4% similar despite different names*

```diff
@@ -57,85 +57,85 @@
       <h5 class="card-header">PORT MAPPINGS</h5>
       <div class="card-body htmx-container table-responsive"
         hx-get="{% url 'plugins:netbox_docker_plugin:port_list' %}?container_id={{ object.pk }}"
         hx-trigger="load"
       ></div>
       {% if perms.netbox_docker_plugin.add_env %}
         <div class="card-footer text-end noprint">
-          <a href="{% url 'plugins:netbox_docker_plugin:port_add' %}?container={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
+          <a href="{% url 'plugins:netbox_docker_plugin:port_add' %}?container={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary">
             <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add a Port Mapping
           </a>
         </div>
       {% endif %}
     </div>
     <div class="card">
       <h5 class="card-header">MOUNTS</h5>
       <div class="card-body htmx-container table-responsive"
         hx-get="{% url 'plugins:netbox_docker_plugin:mount_list' %}?container_id={{ object.pk }}"
         hx-trigger="load"
       ></div>
       {% if perms.netbox_docker_plugin.add_env %}
         <div class="card-footer text-end noprint">
-          <a href="{% url 'plugins:netbox_docker_plugin:mount_add' %}?container={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
+          <a href="{% url 'plugins:netbox_docker_plugin:mount_add' %}?container={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary">
             <i class="mdi mdi-plus-thick" aria-hidden="true"></i> New Mount
           </a>
         </div>
       {% endif %}
     </div>
     <div class="card">
       <h5 class="card-header">BINDS</h5>
       <div class="card-body htmx-container table-responsive"
         hx-get="{% url 'plugins:netbox_docker_plugin:bind_list' %}?container_id={{ object.pk }}"
         hx-trigger="load"
       ></div>
       {% if perms.netbox_docker_plugin.add_env %}
         <div class="card-footer text-end noprint">
-          <a href="{% url 'plugins:netbox_docker_plugin:bind_add' %}?container={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
+          <a href="{% url 'plugins:netbox_docker_plugin:bind_add' %}?container={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary">
             <i class="mdi mdi-plus-thick" aria-hidden="true"></i> New Bind
           </a>
         </div>
       {% endif %}
     </div>
     <div class="card">
       <h5 class="card-header">NETWORK SETTINGS</h5>
       <div class="card-body htmx-container table-responsive"
         hx-get="{% url 'plugins:netbox_docker_plugin:networksetting_list' %}?container_id={{ object.pk }}"
         hx-trigger="load"
       ></div>
       {% if perms.netbox_docker_plugin.add_network_setting %}
         <div class="card-footer text-end noprint">
-          <a href="{% url 'plugins:netbox_docker_plugin:networksetting_add' %}?container={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
+          <a href="{% url 'plugins:netbox_docker_plugin:networksetting_add' %}?container={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary">
             <i class="mdi mdi-plus-thick" aria-hidden="true"></i> New Network Setting
           </a>
         </div>
       {% endif %}
     </div>
     <div class="card">
       <h5 class="card-header">ENV VARIABLE</h5>
       <div class="card-body htmx-container table-responsive"
         hx-get="{% url 'plugins:netbox_docker_plugin:env_list' %}?container_id={{ object.pk }}"
         hx-trigger="load"
       ></div>
       {% if perms.netbox_docker_plugin.add_env %}
         <div class="card-footer text-end noprint">
-          <a href="{% url 'plugins:netbox_docker_plugin:env_add' %}?container={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
+          <a href="{% url 'plugins:netbox_docker_plugin:env_add' %}?container={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary">
             <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add an Env Variable
           </a>
         </div>
       {% endif %}
     </div>
     <div class="card">
       <h5 class="card-header">LABELS</h5>
       <div class="card-body htmx-container table-responsive"
         hx-get="{% url 'plugins:netbox_docker_plugin:label_list' %}?container_id={{ object.pk }}"
         hx-trigger="load"
       ></div>
       {% if perms.netbox_docker_plugin.add_env %}
         <div class="card-footer text-end noprint">
-          <a href="{% url 'plugins:netbox_docker_plugin:label_add' %}?container={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
+          <a href="{% url 'plugins:netbox_docker_plugin:label_add' %}?container={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary">
             <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add a Label
           </a>
         </div>
       {% endif %}
     </div>
   </div>
 </div>
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/host.html` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/host.html`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
       <h5 class="card-header">Registry</h5>
       <div class="card-body htmx-container table-responsive"
         hx-get="{% url 'plugins:netbox_docker_plugin:registry_list' %}?host_id={{ object.pk }}"
         hx-trigger="load"
       ></div>
       {% if perms.netbox_docker_plugin.add_container %}
         <div class="card-footer text-end noprint">
-          <a href="{% url 'plugins:netbox_docker_plugin:registry_add' %}?host={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
+          <a href="{% url 'plugins:netbox_docker_plugin:registry_add' %}?host={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary">
             <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add a Registry
           </a>
         </div>
       {% endif %}
     </div>
     {% plugin_full_width_page object %}
   </div>
@@ -65,15 +65,15 @@
       <h5 class="card-header">Container</h5>
       <div class="card-body htmx-container table-responsive"
         hx-get="{% url 'plugins:netbox_docker_plugin:container_list' %}?host_id={{ object.pk }}"
         hx-trigger="load"
       ></div>
       {% if perms.netbox_docker_plugin.add_container %}
         <div class="card-footer text-end noprint">
-          <a href="{% url 'plugins:netbox_docker_plugin:container_add' %}?host={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
+          <a href="{% url 'plugins:netbox_docker_plugin:container_add' %}?host={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary">
             <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add a Container
           </a>
         </div>
       {% endif %}
     </div>
     {% plugin_full_width_page object %}
   </div>
@@ -82,15 +82,15 @@
       <h5 class="card-header">Images</h5>
       <div class="card-body htmx-container table-responsive"
         hx-get="{% url 'plugins:netbox_docker_plugin:image_list' %}?host_id={{ object.pk }}"
         hx-trigger="load"
       ></div>
       {% if perms.netbox_docker_plugin.add_image %}
         <div class="card-footer text-end noprint">
-          <a href="{% url 'plugins:netbox_docker_plugin:image_add' %}?host={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
+          <a href="{% url 'plugins:netbox_docker_plugin:image_add' %}?host={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary">
             <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add an Image
           </a>
         </div>
       {% endif %}
     </div>
     {% plugin_full_width_page object %}
   </div>
@@ -99,15 +99,15 @@
       <h5 class="card-header">Volumes</h5>
       <div class="card-body htmx-container table-responsive"
         hx-get="{% url 'plugins:netbox_docker_plugin:volume_list' %}?host_id={{ object.pk }}"
         hx-trigger="load"
       ></div>
       {% if perms.netbox_docker_plugin.add_volume %}
         <div class="card-footer text-end noprint">
-          <a href="{% url 'plugins:netbox_docker_plugin:volume_add' %}?host={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
+          <a href="{% url 'plugins:netbox_docker_plugin:volume_add' %}?host={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary">
             <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add a Volume
           </a>
         </div>
       {% endif %}
     </div>
     {% plugin_full_width_page object %}
   </div>
@@ -116,15 +116,15 @@
       <h5 class="card-header">Networks</h5>
       <div class="card-body htmx-container table-responsive"
         hx-get="{% url 'plugins:netbox_docker_plugin:network_list' %}?host_id={{ object.pk }}"
         hx-trigger="load"
       ></div>
       {% if perms.netbox_docker_plugin.add_network %}
         <div class="card-footer text-end noprint">
-          <a href="{% url 'plugins:netbox_docker_plugin:network_add' %}?host={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
+          <a href="{% url 'plugins:netbox_docker_plugin:network_add' %}?host={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary">
             <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add a Network
           </a>
         </div>
       {% endif %}
     </div>
     {% plugin_full_width_page object %}
   </div>
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/image.html` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/image.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/network.html` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/network.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
       <h5 class="card-header">Images</h5>
       <div class="card-body htmx-container table-responsive"
         hx-get="{% url 'plugins:netbox_docker_plugin:image_list' %}?registry_id={{ object.pk }}"
         hx-trigger="load"
       ></div>
       {% if perms.netbox_docker_plugin.add_image %}
         <div class="card-footer text-end noprint">
-          <a href="{% url 'plugins:netbox_docker_plugin:image_add' %}?registry={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
+          <a href="{% url 'plugins:netbox_docker_plugin:image_add' %}?registry={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary">
             <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add an Image
           </a>
         </div>
       {% endif %}
     </div>
     {% plugin_full_width_page object %}
   </div>
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/base.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/base.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_actions.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/container/test_container_actions.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_api.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/container/test_container_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # pylint: disable=R0801
 """Container Test Case"""
 
+import requests_mock
 from django.urls import reverse
-from django.contrib.contenttypes.models import ContentType
+from core.models import ObjectType
 from rest_framework import status
 from users.models import ObjectPermission
 from utilities.testing import APIViewTestCases
 from netbox_docker_plugin.models.container import Container, Bind, Env
 from netbox_docker_plugin.models.host import Host
 from netbox_docker_plugin.models.network import Network
 from netbox_docker_plugin.models.image import Image
 from netbox_docker_plugin.models.volume import Volume
 from netbox_docker_plugin.models.registry import Registry
 from netbox_docker_plugin.tests.base import BaseAPITestCase
 
-import requests_mock
-
 
 class ContainerApiTestCase(
     BaseAPITestCase,
     APIViewTestCases.GetObjectViewTestCase,
     APIViewTestCases.ListObjectsViewTestCase,
     APIViewTestCases.CreateObjectViewTestCase,
     APIViewTestCases.UpdateObjectViewTestCase,
@@ -169,28 +168,28 @@
                 "ports": [],
                 "env": [{"var_name": "ENV", "value": ""}],
                 "labels": [],
             },
         ]
 
     def test_that_patch_overwrites_data_only_when_explicitly_set(self):
-        """ Test that patch overwrites data only when explicitly set """
+        """Test that patch overwrites data only when explicitly set"""
 
         # Assign model-level permission
         obj_perm = ObjectPermission(
             name="Test permission", actions=["add", "change", "view"]
         )
         obj_perm.save()
         # pylint: disable=E1101
         obj_perm.users.add(self.user)
         # pylint: disable=E1101
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
-        obj_perm.object_types.add(ContentType.objects.get_for_model(Container))
-        obj_perm.object_types.add(ContentType.objects.get_for_model(Bind))
-        obj_perm.object_types.add(ContentType.objects.get_for_model(Env))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(Container))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(Bind))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(Env))
 
         host3 = Host.objects.create(
             endpoint="http://localhost:8080",
             name="host3",
         )
         registry3 = Registry.objects.create(
             host=host3,
@@ -237,40 +236,82 @@
         )
 
         self.assertHttpStatus(response, status.HTTP_200_OK)
 
         self.assertEqual(Bind.objects.filter(container=container11).count(), 0)
         self.assertEqual(Env.objects.filter(container=container11).count(), 1)
 
-
     def test_logs_endpoint(self):
-        """ Test logs endpoint """
+        """Test logs endpoint"""
 
         container = Container.objects.get(name="container1")
         container_id = container.ContainerID
 
         endpoint = reverse(
             viewname=f"plugins-api:{self._get_view_namespace()}:container-logs",
             kwargs={"pk": container.pk},
         )
 
         # Add object-level permission
         obj_perm = ObjectPermission(
-            name='Test permission',
+            name="Test permission",
             constraints={"pk": container.pk},
             actions=["view"],
         )
         obj_perm.save()
         # pylint: disable=E1101
         obj_perm.users.add(self.user)
         # pylint: disable=E1101
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
 
         with requests_mock.Mocker() as m:
             m.get(
                 f"http://localhost:8080/api/engine/containers/{container_id}/logs",
                 text="Hello World",
             )
 
             response = self.client.get(endpoint, **self.header)
             self.assertHttpStatus(response, status.HTTP_200_OK)
             self.assertEqual(response.data, "Hello World")
+
+    def test_that_container_host_cannot_be_changed(self):
+        """Test that container's host cannot be changed"""
+
+        host1 = Host.objects.create(name="host4")
+        host2 = Host.objects.create(name="host5")
+
+        registry1 = Registry.objects.create(
+            host=host1, name="registry4", serveraddress="http://localhost:8080"
+        )
+        registry2 = Registry.objects.create(
+            host=host2, name="registry5", serveraddress="http://localhost:8082"
+        )
+
+        image1 = Image.objects.create(host=host1, name="image", registry=registry1)
+        image2 = Image.objects.create(host=host2, name="image", registry=registry2)
+
+        container = Container.objects.create(host=host1, image=image1, name="container")
+
+        obj_perm = ObjectPermission(name="Test permission", actions=["change"])
+        obj_perm.save()
+        # pylint: disable=E1101
+        obj_perm.users.add(self.user)
+        # pylint: disable=E1101
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
+
+        response = self.client.patch(
+            reverse(f"plugins-api:{self._get_view_namespace()}:container-list"),
+            [
+                {
+                    "id": container.pk,
+                    "host": host2.pk,
+                    "image": image2.pk,
+                },
+            ],
+            format="json",
+            **self.header,
+        )
+
+        self.assertHttpStatus(response, status.HTTP_400_BAD_REQUEST)
+        self.assertEqual(
+            response.content, b'{"detail":"Cannot change the host\'s container"}'
+        )
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_operation_view.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/container/test_container_operation_view.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint: disable=R0801
 """Container operation Views Test Case"""
 
 from django.urls import reverse
 from django.test import override_settings
-from django.contrib.contenttypes.models import ContentType
+from core.models import ObjectType
 from utilities.testing import ModelViewTestCase
 from utilities.testing.utils import disable_warnings, post_data
 from users.models import ObjectPermission
 from extras.choices import ObjectChangeActionChoices
 from extras.models import ObjectChange
 from netbox_docker_plugin.models.host import Host
 from netbox_docker_plugin.models.container import Container
@@ -47,15 +47,15 @@
 
         # Assign model-level permission
         obj_perm = ObjectPermission(name="Test permission", actions=["change"])
         obj_perm.save()
         # pylint: disable=E1101
         obj_perm.users.add(self.user)
         # pylint: disable=E1101
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
 
         # Try GET with model-level permission
         self.assertHttpStatus(self.client.get(self._get_url("edit", instance)), 200)
 
         # Try POST with model-level permission
         request = {
             "path": reverse(
@@ -65,15 +65,15 @@
             "data": post_data({"operation": "start"}),
         }
         self.assertHttpStatus(self.client.post(**request), 302)
         instance = self._get_queryset().get(pk=instance.pk)
         self.assertInstanceEqual(instance, {"operation": "start"})
 
         objectchanges = ObjectChange.objects.filter(
-            changed_object_type=ContentType.objects.get_for_model(instance),
+            changed_object_type=ObjectType.objects.get_for_model(instance),
             changed_object_id=instance.pk,
         )
         self.assertEqual(len(objectchanges), 1)
         self.assertEqual(
             objectchanges[0].action, ObjectChangeActionChoices.ACTION_UPDATE
         )
 
@@ -103,15 +103,15 @@
 
         # Assign model-level permission
         obj_perm = ObjectPermission(name="Test permission", actions=["change"])
         obj_perm.save()
         # pylint: disable=E1101
         obj_perm.users.add(self.user)
         # pylint: disable=E1101
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
 
         # Try GET with model-level permission
         self.assertHttpStatus(self.client.get(self._get_url("edit", instance)), 200)
 
         # Try POST with model-level permission
         request = {
             "path": reverse(
@@ -121,15 +121,15 @@
             "data": post_data({"operation": "stop"}),
         }
         self.assertHttpStatus(self.client.post(**request), 302)
         instance = self._get_queryset().get(pk=instance.pk)
         self.assertInstanceEqual(instance, {"operation": "stop"})
 
         objectchanges = ObjectChange.objects.filter(
-            changed_object_type=ContentType.objects.get_for_model(instance),
+            changed_object_type=ObjectType.objects.get_for_model(instance),
             changed_object_id=instance.pk,
         )
         self.assertEqual(len(objectchanges), 1)
         self.assertEqual(
             objectchanges[0].action, ObjectChangeActionChoices.ACTION_UPDATE
         )
 
@@ -159,15 +159,15 @@
 
         # Assign model-level permission
         obj_perm = ObjectPermission(name="Test permission", actions=["change"])
         obj_perm.save()
         # pylint: disable=E1101
         obj_perm.users.add(self.user)
         # pylint: disable=E1101
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
 
         # Try GET with model-level permission
         self.assertHttpStatus(self.client.get(self._get_url("edit", instance)), 200)
 
         # Try POST with model-level permission
         request = {
             "path": reverse(
@@ -177,15 +177,15 @@
             "data": post_data({"operation": "restart"}),
         }
         self.assertHttpStatus(self.client.post(**request), 302)
         instance = self._get_queryset().get(pk=instance.pk)
         self.assertInstanceEqual(instance, {"operation": "restart"})
 
         objectchanges = ObjectChange.objects.filter(
-            changed_object_type=ContentType.objects.get_for_model(instance),
+            changed_object_type=ObjectType.objects.get_for_model(instance),
             changed_object_id=instance.pk,
         )
         self.assertEqual(len(objectchanges), 1)
         self.assertEqual(
             objectchanges[0].action, ObjectChangeActionChoices.ACTION_UPDATE
         )
 
@@ -215,15 +215,15 @@
 
         # Assign model-level permission
         obj_perm = ObjectPermission(name="Test permission", actions=["change"])
         obj_perm.save()
         # pylint: disable=E1101
         obj_perm.users.add(self.user)
         # pylint: disable=E1101
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
 
         # Try GET with model-level permission
         self.assertHttpStatus(self.client.get(self._get_url("edit", instance)), 200)
 
         # Try POST with model-level permission
         request = {
             "path": reverse(
@@ -233,15 +233,15 @@
             "data": post_data({"operation": "recreate"}),
         }
         self.assertHttpStatus(self.client.post(**request), 302)
         instance = self._get_queryset().get(pk=instance.pk)
         self.assertInstanceEqual(instance, {"operation": "recreate"})
 
         objectchanges = ObjectChange.objects.filter(
-            changed_object_type=ContentType.objects.get_for_model(instance),
+            changed_object_type=ObjectType.objects.get_for_model(instance),
             changed_object_id=instance.pk,
         )
         self.assertEqual(len(objectchanges), 1)
         self.assertEqual(
             objectchanges[0].action, ObjectChangeActionChoices.ACTION_UPDATE
         )
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_validation.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/container/test_container_validation.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/container/test_container_views.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/container/test_container_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/host/test_host_api.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/host/test_host_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Host API Test Case"""
 
-from django.contrib.contenttypes.models import ContentType
+from core.models import ObjectType
 from extras.choices import ObjectChangeActionChoices
 from extras.models import ObjectChange
 from users.models import ObjectPermission
 from rest_framework import status
 from utilities.testing import APIViewTestCases
 from netbox_docker_plugin.models.host import Host
 from netbox_docker_plugin.models.registry import Registry
@@ -57,15 +57,15 @@
         """
         # Add object-level permission
         obj_perm = ObjectPermission(name="Test permission", actions=["add"])
         obj_perm.save()
         # pylint: disable=E1101
         obj_perm.users.add(self.user)
         # pylint: disable=E1101
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
 
         initial_count = self._get_queryset().count()
         response = self.client.post(
             self._get_list_url(), self.create_data[0], format="json", **self.header
         )
         self.assertHttpStatus(response, status.HTTP_201_CREATED)
         self.assertEqual(self._get_queryset().count(), initial_count + 1)
@@ -76,15 +76,15 @@
             exclude=self.validation_excluded_fields,
             api=True,
         )
 
         # Verify ObjectChange creation
         if hasattr(self.model, "to_objectchange"):
             objectchanges = ObjectChange.objects.filter(
-                changed_object_type=ContentType.objects.get_for_model(instance),
+                changed_object_type=ObjectType.objects.get_for_model(instance),
                 changed_object_id=instance.pk,
             )
             self.assertEqual(len(objectchanges), 1)
             self.assertEqual(
                 objectchanges[0].action, ObjectChangeActionChoices.ACTION_CREATE
             )
 
@@ -100,22 +100,22 @@
 
         # Add object-level permission
         obj_perm = ObjectPermission(name="Test permission", actions=["delete"])
         obj_perm.save()
         # pylint: disable=E1101
         obj_perm.users.add(self.user)
         # pylint: disable=E1101
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
 
         response = self.client.delete(url, **self.header)
         self.assertHttpStatus(response, status.HTTP_204_NO_CONTENT)
         self.assertFalse(self._get_queryset().filter(pk=instance.pk).exists())
 
         objectchanges = ObjectChange.objects.filter(
-            changed_object_type=ContentType.objects.get_for_model(instance),
+            changed_object_type=ObjectType.objects.get_for_model(instance),
             changed_object_id=instance.pk,
         )
         self.assertEqual(len(objectchanges), 2)
         self.assertEqual(
             objectchanges[0].action, ObjectChangeActionChoices.ACTION_DELETE
         )
         self.assertEqual(
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/host/test_host_views.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/host/test_host_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Host Views Test Case"""
 
-from django.contrib.contenttypes.models import ContentType
+from core.models import ObjectType
 from django.core.exceptions import ObjectDoesNotExist
 from extras.choices import ObjectChangeActionChoices
 from extras.models import ObjectChange
 from users.models import ObjectPermission
 from utilities.testing import ViewTestCases, post_data
 from netbox_docker_plugin.models.host import Host
 from ..base import BaseModelViewTestCase
@@ -35,30 +35,30 @@
 
         # Assign model-level permission
         obj_perm = ObjectPermission(name="Test permission", actions=["delete"])
         obj_perm.save()
         # pylint: disable=E1101
         obj_perm.users.add(self.user)
         # pylint: disable=E1101
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
 
         # Try GET with model-level permission
         self.assertHttpStatus(self.client.get(self._get_url("delete", instance)), 200)
 
         # Try POST with model-level permission
         request = {
             "path": self._get_url("delete", instance),
             "data": post_data({"confirm": True}),
         }
         self.assertHttpStatus(self.client.post(**request), 302)
         with self.assertRaises(ObjectDoesNotExist):
             self._get_queryset().get(pk=instance.pk)
 
         objectchanges = ObjectChange.objects.filter(
-            changed_object_type=ContentType.objects.get_for_model(instance),
+            changed_object_type=ObjectType.objects.get_for_model(instance),
             changed_object_id=instance.pk,
         )
         self.assertEqual(len(objectchanges), 2)
         self.assertEqual(
             objectchanges[0].action, ObjectChangeActionChoices.ACTION_DELETE
         )
         self.assertEqual(
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/host/test_replace_password.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/host/test_replace_password.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/image/test_image_api.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/image/test_image_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/image/test_image_views.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/image/test_image_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/network/test_network_api.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/network/test_network_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/network/test_network_views.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/network/test_network_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/registry/test_registry_api.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/registry/test_registry_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/registry/test_registry_views.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/registry/test_registry_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/test_init.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/volume/test_volume_api.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/volume/test_volume_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Volume Test Case"""
 
 from django.urls import reverse
-from django.contrib.contenttypes.models import ContentType
+from core.models import ObjectType
 from rest_framework import status
 from users.models import ObjectPermission
 from utilities.testing import APIViewTestCases
 from netbox_docker_plugin.models.host import Host
 from netbox_docker_plugin.models.volume import Volume
 from netbox_docker_plugin.models.image import Image
 from netbox_docker_plugin.models.registry import Registry
@@ -57,18 +57,18 @@
         obj_perm = ObjectPermission(
             name="Test permission", actions=["add", "change", "view"]
         )
         obj_perm.save()
         # pylint: disable=E1101
         obj_perm.users.add(self.user)
         # pylint: disable=E1101
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
-        obj_perm.object_types.add(ContentType.objects.get_for_model(Container))
-        obj_perm.object_types.add(ContentType.objects.get_for_model(Mount))
-        obj_perm.object_types.add(ContentType.objects.get_for_model(Image))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(Container))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(Mount))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(Image))
 
         host = Host.objects.create(endpoint="http://localhost:8088", name="host8")
 
         registry = Registry.objects.create(
             host=host, name="registry8", serveraddress="http://localhost:8089"
         )
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/tests/volume/test_volume_views.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/tests/volume/test_volume_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/urls.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     path(
         "containers/",
         container_views.ContainerListView.as_view(),
         name="container_list",
     ),
     path(
         "containers/add/",
-        container_views.ContainerEditView.as_view(),
+        container_views.ContainerNewView.as_view(),
         name="container_add",
     ),
     path(
         "containers/import/",
         container_views.ContainerBulkImportView.as_view(),
         name="container_import",
     ),
@@ -198,14 +198,19 @@
     ),
     path(
         "containers/<int:pk>/logs",
         container_views.ContainerLogsView.as_view(),
         name="container_logs",
     ),
     path(
+        "containers/<int:pk>/exec",
+        container_views.ContainerExecView.as_view(),
+        name="container_exec",
+    ),
+    path(
         "containers/<int:pk>/edit/",
         container_views.ContainerEditView.as_view(),
         name="container_edit",
     ),
     path(
         "containers/<int:pk>/delete/",
         container_views.ContainerDeleteView.as_view(),
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/utilities/__init__.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/utilities/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
                     eventrule.save()
 
                     obj_content_type = ContentType.objects.get(
                         app_label="netbox_docker_plugin", model=webhook["content_types"]
                     )
 
                     # pylint: disable=E1101
-                    eventrule.content_types.set([obj_content_type.pk])
+                    eventrule.object_types.set([obj_content_type.pk])
                     eventrule.save()
 
             return
 
         for webhook in webhooks:
             results = Webhook.objects.filter(
                 payload_url=webhook["payload_url"],
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/bind.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/bind.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/container.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/container.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Container views definitions"""
 
-from utilities.utils import count_related
+from utilities.query import count_related
 from utilities.views import ViewTab, register_model_view
 from netbox.views import generic
 from .. import tables, filtersets
 from ..forms import container
 from ..models.container import (
     Container,
     Mount,
@@ -30,28 +30,44 @@
         "ports",
         "network_settings",
     )
 
 
 @register_model_view(Container, name="logs", path="logs")
 class ContainerLogsView(generic.ObjectView):
-    """ Logs tab in Container view """
+    """Logs tab in Container view"""
 
     queryset = Container.objects.all()
     tab = ViewTab(label="Logs")
     template_name = "netbox_docker_plugin/container-logs.html"
 
 
-class ContainerEditView(generic.ObjectEditView):
+@register_model_view(Container, name="exec", path="exec")
+class ContainerExecView(generic.ObjectView):
+    """Exec tab in Container view"""
+
+    queryset = Container.objects.all()
+    tab = ViewTab(label="Exec")
+    template_name = "netbox_docker_plugin/container-exec.html"
+
+
+class ContainerNewView(generic.ObjectEditView):
     """Container edition view definition"""
 
     queryset = Container.objects.all()
     form = container.ContainerForm
 
 
+class ContainerEditView(generic.ObjectEditView):
+    """Container edition view definition"""
+
+    queryset = Container.objects.all()
+    form = container.ContainerEditForm
+
+
 class ContainerListView(generic.ObjectListView):
     """Container list view definition"""
 
     queryset = Container.objects.annotate(
         port_count=count_related(Port, "container"),
         mount_count=count_related(Mount, "container"),
         bind_count=count_related(Bind, "container"),
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/env.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/env.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/host.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/host.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Host views definitions"""
 
 from users.models import Token
-from utilities.utils import count_related
+from utilities.query import count_related
 from netbox.views import generic
 from .. import tables, filtersets
 from ..forms import host
 from ..models.host import Host
 from ..models.image import Image
 from ..models.volume import Volume
 from ..models.network import Network
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/image.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Image views definitions"""
 
-from utilities.utils import count_related
+from utilities.query import count_related
 from netbox.views import generic
 from .. import tables, filtersets
 from ..forms import image
 from ..models.image import Image
 from ..models.container import Container
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/label.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/label.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/mount.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/mount.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/network.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Network views definitions"""
 
-from utilities.utils import count_related
+from utilities.query import count_related
 from netbox.views import generic
 from .. import tables, filtersets
 from ..forms import network
 from ..models.network import Network
 from ..models.container import NetworkSetting
 
 class NetworkView(generic.ObjectView):
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/network_setting.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/network_setting.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/port.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/port.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/registry.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Registry views definitions"""
 
-from utilities.utils import count_related
+from utilities.query import count_related
 from netbox.views import generic
 from .. import tables, filtersets
 from ..forms import registry
 from ..models.image import Image
 from ..models.registry import Registry
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin/views/volume.py` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin/views/volume.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Volume views definitions"""
 
-from utilities.utils import count_related
+from utilities.query import count_related
 from netbox.views import generic
 from .. import tables, filtersets
 from ..forms import volume
 from ..models.volume import Volume
 from ..models.container import Mount
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin.egg-info/PKG-INFO` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-docker-plugin
-Version: 1.9.0
+Version: 2.0.0
 Summary: Manage Docker with Netbox & style.
 Author-email: Vincent Simonin <vincent@saashup.com>, David Delassus <david.jose.delassus@gmail.com>
 Project-URL: Homepage, https://github.com/SaaShup/netbox-docker-plugin
 Project-URL: Bug Tracker, https://github.com/SaaShup/netbox-docker-plugin/issues
 Keywords: netbox,netbox-plugin,docker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `netbox_docker_plugin-1.9.0/netbox_docker_plugin.egg-info/SOURCES.txt` & `netbox_docker_plugin-2.0.0/netbox_docker_plugin.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -55,22 +55,24 @@
 netbox_docker_plugin/migrations/0023_delete_hosts.py
 netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py
 netbox_docker_plugin/migrations/0025_alter_image_version.py
 netbox_docker_plugin/migrations/0026_image_digest.py
 netbox_docker_plugin/migrations/0027_container_restart_policy.py
 netbox_docker_plugin/migrations/0028_mount_and_bind_read_only.py
 netbox_docker_plugin/migrations/0029_alter_container_state.py
+netbox_docker_plugin/migrations/0030_alter_container_containerid_alter_container_hostname_and_more.py
 netbox_docker_plugin/migrations/__init__.py
 netbox_docker_plugin/models/__init__.py
 netbox_docker_plugin/models/container.py
 netbox_docker_plugin/models/host.py
 netbox_docker_plugin/models/image.py
 netbox_docker_plugin/models/network.py
 netbox_docker_plugin/models/registry.py
 netbox_docker_plugin/models/volume.py
+netbox_docker_plugin/templates/netbox_docker_plugin/container-exec.html
 netbox_docker_plugin/templates/netbox_docker_plugin/container-layout.html
 netbox_docker_plugin/templates/netbox_docker_plugin/container-logs.html
 netbox_docker_plugin/templates/netbox_docker_plugin/container.html
 netbox_docker_plugin/templates/netbox_docker_plugin/host.html
 netbox_docker_plugin/templates/netbox_docker_plugin/image.html
 netbox_docker_plugin/templates/netbox_docker_plugin/network.html
 netbox_docker_plugin/templates/netbox_docker_plugin/registry.html
@@ -79,14 +81,15 @@
 netbox_docker_plugin/templatetags/host.py
 netbox_docker_plugin/tests/__init__.py
 netbox_docker_plugin/tests/base.py
 netbox_docker_plugin/tests/test_init.py
 netbox_docker_plugin/tests/container/__init__.py
 netbox_docker_plugin/tests/container/test_container_actions.py
 netbox_docker_plugin/tests/container/test_container_api.py
+netbox_docker_plugin/tests/container/test_container_api_exec.py
 netbox_docker_plugin/tests/container/test_container_operation_view.py
 netbox_docker_plugin/tests/container/test_container_validation.py
 netbox_docker_plugin/tests/container/test_container_views.py
 netbox_docker_plugin/tests/host/__init__.py
 netbox_docker_plugin/tests/host/test_host_api.py
 netbox_docker_plugin/tests/host/test_host_views.py
 netbox_docker_plugin/tests/host/test_replace_password.py
```

### Comparing `netbox_docker_plugin-1.9.0/pyproject.toml` & `netbox_docker_plugin-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-docker-plugin"
-version = "1.9.0"
+version = "2.0.0"
 authors = [
   { name="Vincent Simonin", email="vincent@saashup.com" },
   { name="David Delassus", email="david.jose.delassus@gmail.com" }
 ]
 description = "Manage Docker with Netbox & style."
 readme = "README.md"
 requires-python = ">=3.8"
```

